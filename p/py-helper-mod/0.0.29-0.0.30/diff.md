# Comparing `tmp/py-helper-mod-0.0.29.tar.gz` & `tmp/py-helper-mod-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp7fufnvi9/py-helper-mod-0.0.29.tar", last modified: Mon May 22 19:37:16 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmpbu2zj0d4/py-helper-mod-0.0.30.tar", last modified: Mon May 22 19:47:01 2023, max compression
```

## Comparing `py-helper-mod-0.0.29.tar` & `py-helper-mod-0.0.30.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.29/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.29/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 19:37:16.000000 py-helper-mod-0.0.29/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81087 2023-05-22 19:36:13.000000 py-helper-mod-0.0.29/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.30/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.30/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.30/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.30/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 19:47:01.000000 py-helper-mod-0.0.30/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    81044 2023-05-22 19:46:00.000000 py-helper-mod-0.0.30/py_helper.py
```

### Comparing `py-helper-mod-0.0.29/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.30/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.29
+Version: 0.0.30
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.29/LICENSE` & `py-helper-mod-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.29/PKG-INFO` & `py-helper-mod-0.0.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.29
+Version: 0.0.30
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.29/py_helper.py` & `py-helper-mod-0.0.30/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,29)
+VERSION=(0,0,30)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1126,29 +1126,28 @@
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
 				DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","Yes","yes","y","Y" ] else False
 
-def IsDebugEnabled(dbglabel,test=None):
+def IsDebugEnabled(dbglabel,test=True):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugEnabled
 
 	enabled = True
-	test = test if test is not None else True
 
 	if DebugEnabled is not None and dbglabel is not None:
 		if dbglabel in DebugEnabled and test:
 			enabled = DebugEnabled[dbglabel]
 
 	return enabled
 
-def Breakpoint(dbglabel,test=None):
+def Breakpoint(dbglabel,test=True):
 	"""Check if Debug Label is Enabled AND We Are In DebugMode"""
 
 	enabled = IsDebugEnabled(dbglabel,test)
 
 	return (DebugMode() and enabled)
 
 # A Centrally Controlled Debug Messaging System
```

