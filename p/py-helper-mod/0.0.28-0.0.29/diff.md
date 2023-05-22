# Comparing `tmp/py-helper-mod-0.0.28.tar.gz` & `tmp/py-helper-mod-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmprfcujclm/py-helper-mod-0.0.28.tar", last modified: Mon May 22 19:26:32 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp7fufnvi9/py-helper-mod-0.0.29.tar", last modified: Mon May 22 19:37:16 2023, max compression
```

## Comparing `py-helper-mod-0.0.28.tar` & `py-helper-mod-0.0.29.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.28/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80910 2023-05-22 19:25:28.000000 py-helper-mod-0.0.28/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.29/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81087 2023-05-22 19:36:13.000000 py-helper-mod-0.0.29/py_helper.py
```

### Comparing `py-helper-mod-0.0.28/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.29/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.28
+Version: 0.0.29
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.28/LICENSE` & `py-helper-mod-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.28/PKG-INFO` & `py-helper-mod-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.28
+Version: 0.0.29
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.28/setup.cfg` & `py-helper-mod-0.0.29/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.28
+version = 0.0.29
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

### Comparing `py-helper-mod-0.0.28/py_helper.py` & `py-helper-mod-0.0.29/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,28)
+VERSION=(0,0,29)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1140,14 +1140,21 @@
 
 	if DebugEnabled is not None and dbglabel is not None:
 		if dbglabel in DebugEnabled and test:
 			enabled = DebugEnabled[dbglabel]
 
 	return enabled
 
+def Breakpoint(dbglabel,test=None):
+	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
+
+	enabled = IsDebugEnabled(dbglabel,test)
+
+	return (DebugMode() and enabled)
+
 # A Centrally Controlled Debug Messaging System
 # msg : Message to print
 # func : A simple function to pass the message to (optional)
 # If "func" is supplied, DbgMsg uses it for output instead of printing to stdout
 def DbgMsg(msg,func=None,prefix="***",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""
 	Messaging function that only prints when in DebugMode.
```

