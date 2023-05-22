# Comparing `tmp/poetry_multiproject_plugin-1.2.1.tar.gz` & `tmp/poetry_multiproject_plugin-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_multiproject_plugin-1.2.1.tar", max compression
+gzip compressed data, was "poetry_multiproject_plugin-1.2.2.tar", max compression
```

## Comparing `poetry_multiproject_plugin-1.2.1.tar` & `poetry_multiproject_plugin-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.2.1/LICENSE
--rw-r--r--   0        0        0     5409 2023-02-13 19:04:54.429748 poetry_multiproject_plugin-1.2.1/README.md
--rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/__init__.py
--rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/__init__.py
--rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/buildproject/__init__.py
--rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/buildproject/project.py
--rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/checkproject/__init__.py
--rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/checkproject/check.py
--rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/__init__.py
--rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/check/__init__.py
--rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/check/mypy_checker.py
--rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/deps/__init__.py
--rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/deps/installer.py
--rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/parsing/__init__.py
--rw-r--r--   0        0        0     1665 2023-02-13 19:04:54.453532 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/parsing/rewrite.py
--rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/__init__.py
--rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/cleanup.py
--rw-r--r--   0        0        0      511 2023-02-13 19:04:54.454463 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/create.py
--rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/dist.py
--rw-r--r--   0        0        0      875 2023-02-13 19:04:54.455402 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/packages.py
--rw-r--r--   0        0        0     1016 2023-02-13 19:04:54.456329 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/prepare.py
--rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/__init__.py
--rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/generate.py
--rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/packages.py
--rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/read.py
--rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/plugin.py
--rw-r--r--   0        0        0      841 2023-02-15 17:23:23.135876 poetry_multiproject_plugin-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-01-23 14:15:18.822524 poetry_multiproject_plugin-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5409 2023-02-13 19:04:54.429748 poetry_multiproject_plugin-1.2.2/README.md
+-rw-r--r--   0        0        0      122 2022-10-30 09:31:55.254657 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-27 21:12:19.215558 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/__init__.py
+-rw-r--r--   0        0        0       92 2022-10-29 17:34:08.279274 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/__init__.py
+-rw-r--r--   0        0        0     2848 2023-02-15 17:23:23.134947 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/project.py
+-rw-r--r--   0        0        0       88 2022-12-26 11:25:28.111604 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/__init__.py
+-rw-r--r--   0        0        0     2462 2023-01-06 16:42:40.541575 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/check.py
+-rw-r--r--   0        0        0        0 2022-10-29 17:34:08.280190 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/__init__.py
+-rw-r--r--   0        0        0      118 2022-12-26 11:25:28.113080 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/__init__.py
+-rw-r--r--   0        0        0     1080 2023-01-06 16:42:40.542392 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/mypy_checker.py
+-rw-r--r--   0        0        0      106 2022-12-27 09:13:24.664513 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/__init__.py
+-rw-r--r--   0        0        0      683 2023-01-06 22:56:24.237617 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/installer.py
+-rw-r--r--   0        0        0      111 2023-02-13 19:04:54.452935 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/__init__.py
+-rw-r--r--   0        0        0     1713 2023-05-22 19:10:23.672824 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/rewrite.py
+-rw-r--r--   0        0        0      141 2022-10-29 17:34:08.281001 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/__init__.py
+-rw-r--r--   0        0        0      274 2022-12-28 08:58:51.305973 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/cleanup.py
+-rw-r--r--   0        0        0      541 2023-05-22 19:10:23.673577 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/create.py
+-rw-r--r--   0        0        0      304 2022-12-26 11:25:28.115615 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/dist.py
+-rw-r--r--   0        0        0      875 2023-02-13 19:04:54.455402 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/packages.py
+-rw-r--r--   0        0        0     1016 2023-02-13 19:04:54.456329 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/prepare.py
+-rw-r--r--   0        0        0      125 2022-10-29 17:34:08.284437 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/__init__.py
+-rw-r--r--   0        0        0     1634 2023-02-13 19:04:54.457639 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/generate.py
+-rw-r--r--   0        0        0      592 2023-02-12 16:50:12.589435 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/packages.py
+-rw-r--r--   0        0        0      631 2023-02-13 19:04:54.458759 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/read.py
+-rw-r--r--   0        0        0      909 2022-12-26 11:25:28.122982 poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/plugin.py
+-rw-r--r--   0        0        0      841 2023-05-22 19:10:23.674333 poetry_multiproject_plugin-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 poetry_multiproject_plugin-1.2.2/PKG-INFO
```

### Comparing `poetry_multiproject_plugin-1.2.1/LICENSE` & `poetry_multiproject_plugin-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/README.md` & `poetry_multiproject_plugin-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/buildproject/project.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/buildproject/project.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/commands/checkproject/check.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/commands/checkproject/check.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/check/mypy_checker.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/check/mypy_checker.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/deps/installer.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/deps/installer.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/parsing/rewrite.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/parsing/rewrite.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 
     return False
 
 
 def rewrite_module(path: pathlib.Path, namespaces: List[str], top_ns: str) -> bool:
     file_path = path.as_posix()
 
-    with open(file_path, "r") as f:
+    with open(file_path, "r", encoding="utf-8") as f:
         tree = ast.parse(f.read(), path.name)
 
     res = {mutate_imports(node, namespaces, top_ns) for node in ast.walk(tree)}
 
     if True in res:
         rewritten_source_code = ast.unparse(tree)  # type: ignore[attr-defined]
 
-        with open(file_path, "w") as f:
+        with open(file_path, "w", encoding="utf-8", newline="") as f:
             f.write(rewritten_source_code)
 
         return True
 
     return False
```

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/packages.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/packages.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/project/prepare.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/project/prepare.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/generate.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/generate.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/packages.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/packages.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/components/toml/read.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/components/toml/read.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/poetry_multiproject_plugin/plugin.py` & `poetry_multiproject_plugin-1.2.2/poetry_multiproject_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_multiproject_plugin-1.2.1/pyproject.toml` & `poetry_multiproject_plugin-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-multiproject-plugin"
-version = "1.2.1"
+version = "1.2.2"
 description = "A Poetry plugin that makes it possible to use relative package includes."
 authors = ["David Vujic"]
 homepage = "https://github.com/davidvujic/poetry-multiproject-plugin"
 repository = "https://github.com/davidvujic/poetry-multiproject-plugin"
 readme = "README.md"
 packages = [{include = "poetry_multiproject_plugin"}]
```

### Comparing `poetry_multiproject_plugin-1.2.1/PKG-INFO` & `poetry_multiproject_plugin-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-multiproject-plugin
-Version: 1.2.1
+Version: 1.2.2
 Summary: A Poetry plugin that makes it possible to use relative package includes.
 Home-page: https://github.com/davidvujic/poetry-multiproject-plugin
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

