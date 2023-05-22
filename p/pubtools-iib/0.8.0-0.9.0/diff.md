# Comparing `tmp/pubtools-iib-0.8.0.tar.gz` & `tmp/pubtools-iib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pubtools-iib-0.8.0.tar", last modified: Wed Mar  4 18:08:14 2020, max compression
+gzip compressed data, was "dist/pubtools-iib-0.9.0.tar", last modified: Wed Mar  4 19:44:23 2020, max compression
```

## Comparing `pubtools-iib-0.8.0.tar` & `pubtools-iib-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      137 2020-02-21 15:14:47.000000 pubtools-iib-0.8.0/MANIFEST.in
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     3561 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/PKG-INFO
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     1318 2020-02-21 15:15:46.000000 pubtools-iib-0.8.0/README.rst
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/docs/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      613 2020-02-25 11:22:04.000000 pubtools-iib-0.8.0/docs/Makefile
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/docs/source/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      711 2020-03-04 18:06:29.000000 pubtools-iib-0.8.0/docs/source/CHANGELOG.rst
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     1318 2020-02-21 15:15:46.000000 pubtools-iib-0.8.0/docs/source/README.rst
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     5000 2020-02-25 11:22:04.000000 pubtools-iib-0.8.0/docs/source/conf.py
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      355 2020-02-25 11:22:04.000000 pubtools-iib-0.8.0/docs/source/index.rst
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/docs/source/modules/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      653 2020-02-25 11:22:04.000000 pubtools-iib-0.8.0/docs/source/modules/add_bundles.rst
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      647 2020-02-25 11:22:04.000000 pubtools-iib-0.8.0/docs/source/modules/rm_operators.rst
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)       85 2020-02-21 15:14:58.000000 pubtools-iib-0.8.0/pubtools/__init__.py
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools/iib/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)       20 2020-02-21 15:14:58.000000 pubtools-iib-0.8.0/pubtools/iib/__init__.py
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     8377 2020-03-04 17:57:02.000000 pubtools-iib-0.8.0/pubtools/iib/iib_ops.py
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     2663 2020-03-04 17:40:54.000000 pubtools-iib-0.8.0/pubtools/iib/utils.py
-drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     3561 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/PKG-INFO
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      529 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/SOURCES.txt
--rw-rw-r--   0 jluza     (1000) jluza     (1000)       69 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/dependency_links.txt
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      159 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/entry_points.txt
--rw-rw-r--   0 jluza     (1000) jluza     (1000)       64 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/requires.txt
--rw-rw-r--   0 jluza     (1000) jluza     (1000)        9 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/pubtools_iib.egg-info/top_level.txt
--rw-rw-r--   0 jluza     (1000) jluza     (1000)      243 2020-03-04 18:08:14.000000 pubtools-iib-0.8.0/setup.cfg
--rw-rw-r--   0 jluza     (1000) jluza     (1000)     2500 2020-03-04 18:06:47.000000 pubtools-iib-0.8.0/setup.py
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/docs/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      613 2020-02-25 11:22:04.000000 pubtools-iib-0.9.0/docs/Makefile
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/docs/source/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      783 2020-03-04 19:34:15.000000 pubtools-iib-0.9.0/docs/source/CHANGELOG.rst
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      355 2020-02-25 11:22:04.000000 pubtools-iib-0.9.0/docs/source/index.rst
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/docs/source/modules/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      647 2020-02-25 11:22:04.000000 pubtools-iib-0.9.0/docs/source/modules/rm_operators.rst
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      653 2020-02-25 11:22:04.000000 pubtools-iib-0.9.0/docs/source/modules/add_bundles.rst
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     5000 2020-02-25 11:22:04.000000 pubtools-iib-0.9.0/docs/source/conf.py
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     1318 2020-02-21 15:15:46.000000 pubtools-iib-0.9.0/docs/source/README.rst
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      529 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/SOURCES.txt
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)       69 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/dependency_links.txt
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      159 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/entry_points.txt
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)        9 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/top_level.txt
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     3665 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/PKG-INFO
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)       64 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools_iib.egg-info/requires.txt
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      243 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/setup.cfg
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)       85 2020-02-21 15:14:58.000000 pubtools-iib-0.9.0/pubtools/__init__.py
+drwxrwxr-x   0 jluza     (1000) jluza     (1000)        0 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/pubtools/iib/
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     8583 2020-03-04 19:27:29.000000 pubtools-iib-0.9.0/pubtools/iib/iib_ops.py
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)       20 2020-02-21 15:14:58.000000 pubtools-iib-0.9.0/pubtools/iib/__init__.py
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     2663 2020-03-04 17:40:54.000000 pubtools-iib-0.9.0/pubtools/iib/utils.py
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     2500 2020-03-04 19:34:25.000000 pubtools-iib-0.9.0/setup.py
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)      137 2020-02-21 15:14:47.000000 pubtools-iib-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     1318 2020-02-21 15:15:46.000000 pubtools-iib-0.9.0/README.rst
+-rw-rw-r--   0 jluza     (1000) jluza     (1000)     3665 2020-03-04 19:44:23.000000 pubtools-iib-0.9.0/PKG-INFO
```

### Comparing `pubtools-iib-0.8.0/PKG-INFO` & `pubtools-iib-0.9.0/pubtools_iib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-iib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pubtools-iib
 Home-page: https://gitlab.cee.redhat.com/jluza/pubtools-iib
 Author: Jindrich Luza
 Author-email: jluza@redhat.com
 License: UNKNOWN
 Description: ==============
          pubtools-iib
@@ -59,14 +59,18 @@
             --index-image container-registry.example.com/index/image:latest
             --operator bundle/image:123
             --arch x86_64
         
         ChangeLog
         =========
         
+        0.9.0 (2020-03-04)
+        ------------------
+        * succesful build dump to output
+        
         0.8.0 (2020-03-04)
         ------------------
         * fixed repo sync attributes
         
         0.7.0 (2020-03-04)
         ------------------
         * added iib-insecure attribute
```

### Comparing `pubtools-iib-0.8.0/README.rst` & `pubtools-iib-0.9.0/docs/source/README.rst`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/docs/Makefile` & `pubtools-iib-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/docs/source/CHANGELOG.rst` & `pubtools-iib-0.9.0/docs/source/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ChangeLog
 =========
 
+0.9.0 (2020-03-04)
+------------------
+* succesful build dump to output
+
 0.8.0 (2020-03-04)
 ------------------
 * fixed repo sync attributes
 
 0.7.0 (2020-03-04)
 ------------------
 * added iib-insecure attribute
```

### Comparing `pubtools-iib-0.8.0/docs/source/README.rst` & `pubtools-iib-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/docs/source/conf.py` & `pubtools-iib-0.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/docs/source/modules/add_bundles.rst` & `pubtools-iib-0.9.0/docs/source/modules/add_bundles.rst`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/docs/source/modules/rm_operators.rst` & `pubtools-iib-0.9.0/docs/source/modules/rm_operators.rst`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/pubtools/iib/iib_ops.py` & `pubtools-iib-0.9.0/pubtools/iib/iib_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,14 +215,15 @@
         json.dump(
             build_details.to_dict(),
             sys.stderr,
             sort_keys=True,
             indent=4,
             separators=(",", ": "),
         )
+        sys.stderr.write("\n")
         sys.exit(1)
 
     LOG.info("IIB build finished")
     LOG.debug("Getting pulp repository: %s", args.pulp_repository)
     container_repo = pulp_c.get_repository(args.pulp_repository)
     feed, path = build_details.index_image.split("/", 1)
     upstream_name, tag = path.split(":")
@@ -253,14 +254,22 @@
         entry_func()
 
     push_items = push_items_from_build(
         build_details, items_final_state, args.pulp_repository
     )
     LOG.info("IIB push finished")
     pc.update_push_items(push_items)
+    json.dump(
+        build_details.to_dict(),
+        sys.stdout,
+        sort_keys=True,
+        indent=4,
+        separators=(",", ": "),
+    )
+    sys.stdout.write("\n")
     return build_details
 
 
 def make_add_bundles_parser():
     return setup_arg_parser(ADD_CMD_ARGS)
```

### Comparing `pubtools-iib-0.8.0/pubtools/iib/utils.py` & `pubtools-iib-0.9.0/pubtools/iib/utils.py`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/pubtools_iib.egg-info/PKG-INFO` & `pubtools-iib-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubtools-iib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pubtools-iib
 Home-page: https://gitlab.cee.redhat.com/jluza/pubtools-iib
 Author: Jindrich Luza
 Author-email: jluza@redhat.com
 License: UNKNOWN
 Description: ==============
          pubtools-iib
@@ -59,14 +59,18 @@
             --index-image container-registry.example.com/index/image:latest
             --operator bundle/image:123
             --arch x86_64
         
         ChangeLog
         =========
         
+        0.9.0 (2020-03-04)
+        ------------------
+        * succesful build dump to output
+        
         0.8.0 (2020-03-04)
         ------------------
         * fixed repo sync attributes
         
         0.7.0 (2020-03-04)
         ------------------
         * added iib-insecure attribute
```

### Comparing `pubtools-iib-0.8.0/pubtools_iib.egg-info/SOURCES.txt` & `pubtools-iib-0.9.0/pubtools_iib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubtools-iib-0.8.0/setup.py` & `pubtools-iib-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 extras_require = {"reST": ["Sphinx"]}
 if os.environ.get("READTHEDOCS", None):
     extras_require["reST"].append("recommonmark")
 
 setup(
     name="pubtools-iib",
-    version="0.8.0",
+    version="0.9.0",
     description="Pubtools-iib",
     long_description=long_description,
     author="Jindrich Luza",
     author_email="jluza@redhat.com",
     url="https://gitlab.cee.redhat.com/jluza/pubtools-iib",
     classifiers=classifiers,
     packages=find_packages(exclude=["tests"]),
```

