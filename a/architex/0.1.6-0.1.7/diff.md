# Comparing `tmp/architex-0.1.6.tar.gz` & `tmp/architex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.6.tar", max compression
+gzip compressed data, was "architex-0.1.7.tar", max compression
```

## Comparing `architex-0.1.6.tar` & `architex-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.6/README.md
--rw-r--r--   0        0        0      426 2023-05-10 12:49:37.748401 architex-0.1.6/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.6/architex/__main__.py
--rw-r--r--   0        0        0    10697 2023-05-10 12:48:55.614362 architex-0.1.6/architex/controller.py
--rw-r--r--   0        0        0      936 2023-05-10 07:11:17.514948 architex-0.1.6/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-10 12:49:37.572565 architex-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.6/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-18 04:41:44.332373 architex-0.1.7/README.md
+-rw-r--r--   0        0        0      426 2023-05-22 03:23:32.832400 architex-0.1.7/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.7/architex/__main__.py
+-rw-r--r--   0        0        0    10347 2023-05-18 10:49:45.779180 architex-0.1.7/architex/controller.py
+-rw-r--r--   0        0        0      942 2023-05-18 06:55:18.830557 architex-0.1.7/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-22 03:23:32.666026 architex-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.7/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.7/PKG-INFO
```

### Comparing `architex-0.1.6/architex/controller.py` & `architex-0.1.7/architex/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import yaml
 import os
-import sys
 import crossplane
 import urllib.parse
 from yaml.loader import SafeLoader
 from diagrams import Diagram
 from diagrams.c4 import Person, Container, Database, SystemBoundary, Relationship
 
-graph_attr = {
-    "splines": "spline",
-}
 global_names = []
 
 
 def container_name2service_name(container_name):
     for item in global_names:
         if item['container_name'] == container_name:
             return item['service_name']
 
 
-def get_filepaths(repo_path):
-    res = []
-    for (dir_path, dir_names, file_names) in os.walk(repo_path):
-        for file_name in file_names:
-            res.append(f'{dir_path}/{file_name}')
-    return res
+def populate_composes(docker_composes, compose_files, repo_path, search):
+    def get_filepaths(repo_path):
+        res = []
+        for (dir_path, dir_names, file_names) in os.walk(repo_path):
+            for file_name in file_names:
+                res.append(f'{dir_path}/{file_name}')
+        return res
+
+    filepaths = get_filepaths(repo_path) if search else repo_path
+    for filepath in filepaths:
+        if (".yml" in filepath or ".yaml" in filepath):
+            file = open(filepath)
+            loadedYaml = {}
+            try:
+                loadedYaml = yaml.load(file, Loader=SafeLoader)
+                loadedYaml = {} if loadedYaml is None else loadedYaml
+            except:
+                None
+            if loadedYaml.get("services"):
+                docker_composes.append(loadedYaml)
+                compose_files.append(filepath)
+            file.close()
 
 
 def service_to_container(name, service):
     withNetworks = ', '.join([x for x in service.get(
         'networks') if x != 'default']) if service.get(
         'networks') != None else None
 
@@ -101,16 +113,19 @@
     with composeNetwork:
         for name, service in docker_compose["services"].items():
             containers[name] = service_to_container(name, service)
 
             global global_names
             if "nginx" in name or (service.get("image") is not None and "nginx" in service.get("image")) or (service.get("volumes") is not None and len([volume_string for volume_string in service['volumes'] if 'nginx' in volume_string])):
                 path_strings = compose_file.split('/')[:-1]
-                path_strings.append(f'{service["build"]["context"]}/nginx.conf' if service.get('build') else [
-                                    volume_string for volume_string in service['volumes']if 'nginx' in volume_string and 'conf' in volume_string][0].split(':')[0])
+                to_be_appended = [
+                    volume_string for volume_string in service['volumes']if 'nginx' in volume_string and 'conf' in volume_string][0].split(':')[0]
+                if (to_be_appended is None and service.get('build')):
+                    to_be_appended = f'{service["build"]["context"]}/nginx.conf'
+                path_strings.append(to_be_appended)
                 global_names.append({'service_name': name, 'container_name':  service.get(
                     "container_name") if "container_name" in service else name, 'nginx_path': '/'.join(path_strings)})
             else:
                 global_names.append({'service_name': name, 'container_name':  service.get(
                     "container_name") if "container_name" in service else name})
 
 
@@ -142,90 +157,64 @@
             if block["directive"] == "proxy_pass":
                 proxy_blocks.append(block.get("args")[0])
             if block["directive"] == "fastcgi_pass":
                 fastcgi_blocks.append(block.get("args")[0])
             if block["directive"] == "proxy_http_version":
                 version = block.get("args")[0]
 
-        if root_blocks:
-            web = Container(
-                name="web client",
-                technology="static web",
-                description=f'{root_blocks[0]} nginx service directory',
-            )
-            containers[nginx_container_name] >> Relationship(
-                f'{location_block.get("args")[0]} simple redirection') >> web
-        elif proxy_blocks:
+        def pass_block_to_relationship(pass_block, is_fastcgi=False):
             target_container_name = urllib.parse.urlparse(
-                proxy_blocks[0]).netloc.split(":")[0]
+                pass_block).netloc.split(":")[0]
             target_container = None
             if containers.get(
                     target_container_name):
                 target_container = containers[target_container_name]
             elif containers.get(container_name2service_name(target_container_name)):
                 target_container = containers[container_name2service_name(
                     target_container_name)]
             else:
                 target_container = Container(
                     name=target_container_name,
-                    technology=f'proxy_http_version {version}',
-                    description=proxy_blocks[0],
+                    technology=target_container_name if is_fastcgi else f'proxy_http_version {version}',
+                    description=pass_block,
                 )
                 containers[target_container_name] = target_container
 
             containers[nginx_container_name] >> Relationship(
-                f'{location_block.get("args")[0]} proxy pass') >> target_container
-        elif fastcgi_blocks:
-            target_container_name = urllib.parse.urlparse(
-                fastcgi_blocks[0]).netloc.split(":")[0]
-            target_container = None
-            if containers.get(
-                    target_container_name):
-                target_container = containers[target_container_name]
-            elif containers.get(container_name2service_name(target_container_name)):
-                target_container = containers[container_name2service_name(
-                    target_container_name)]
-            else:
-                target_container = Container(
-                    name=target_container_name,
-                    technology=target_container_name,
-                    description=fastcgi_blocks[0],
+                f'{location_block.get("args")[0]} {"fastcgi" if is_fastcgi else "proxy"} pass') >> target_container
+
+        if root_blocks:
+            for root_block in root_blocks:
+                web = Container(
+                    name="web client",
+                    technology="static web",
+                    description=f'{root_block} nginx service directory',
                 )
-                containers[target_container_name] = target_container
+                containers[nginx_container_name] >> Relationship(
+                    f'{location_block.get("args")[0]} simple redirection') >> web
 
-            containers[nginx_container_name] >> Relationship(
-                f'{location_block.get("args")[0]} fastcgi pass') >> target_container
+        elif proxy_blocks:
+            for proxy_block in proxy_blocks:
+                pass_block_to_relationship(proxy_block)
+
+        elif fastcgi_blocks:
+            for fastcgi_block in fastcgi_blocks:
+                pass_block_to_relationship(fastcgi_block, True)
 
 
 def start_drawing(repo_path, search):
     docker_composes, compose_files = [], []
-    filepaths = get_filepaths(repo_path[0]) if search else repo_path
-    if (search):
-        repo_path = repo_path[0]
-    else:
-        None
-    for filepath in filepaths:
-        if (".yml" in filepath or ".yaml" in filepath):
-            file = open(filepath)
-            loadedYaml = {}
-            try:
-                loadedYaml = yaml.load(file, Loader=SafeLoader)
-                loadedYaml = {} if loadedYaml is None else loadedYaml
-            except:
-                loadedYaml = {}
-            if loadedYaml.get("services"):
-                docker_composes.append(loadedYaml)
-                compose_files.append(filepath)
-            file.close()
-
-    reponame = "current"
-    if (search):
-        reponame = repo_path.split(
-            "/")[-1] if "/" in repo_path else "current"
-    with Diagram(f'{reponame} Architectural Diagram', filename=f'{reponame}_architecture',  graph_attr=graph_attr, show=False):
+    repo_path = repo_path[0] if search else repo_path
+    reponame = repo_path.split(
+        "/")[-1] if search and "/" in repo_path else "current"
+
+    populate_composes(docker_composes, compose_files, repo_path, search)
+    with Diagram(f'{reponame} Architectural Diagram', filename=f'{reponame}_architecture',  graph_attr={
+        "splines": "spline",
+    }, show=False):
         containers, databases, user = {}, {}, Person(
             name="User", description="General User")
 
         for index, docker_compose in enumerate(docker_composes):
             populate_databases(docker_compose, databases)
             populate_containers(docker_compose, containers,
                                 compose_files[index], repo_path if search else "")
```

### Comparing `architex-0.1.6/architex/view.py` & `architex-0.1.7/architex/view.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     )
 ) -> None:
     return
 
 
 @app.command()
 def draw(
-    repo_path: List[str] = typer.Argument(...),
+    list_of_path: List[str] = typer.Argument(...),
     search: bool = typer.Option(False, "--search", "-s"),
 ) -> None:
     """Draw software architecture diagram."""
-    controller.start_drawing(repo_path, search)
+    controller.start_drawing(list_of_path, search)
     typer.secho(
         f"""Your architectural diagram is completed""",
         fg=typer.colors.GREEN,
     )
```

### Comparing `architex-0.1.6/pyproject.toml` & `architex-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.6"
+version = "0.1.7"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `architex-0.1.6/setup.py` & `architex-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytest==6.2.4',
  'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `architex-0.1.6/PKG-INFO` & `architex-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.6
+Version: 0.1.7
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

