# Comparing `tmp/py-helper-mod-0.0.27.tar.gz` & `tmp/py-helper-mod-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp5f67m_9w/py-helper-mod-0.0.27.tar", last modified: Sat May 20 03:04:04 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmprfcujclm/py-helper-mod-0.0.28.tar", last modified: Mon May 22 19:26:32 2023, max compression
```

## Comparing `py-helper-mod-0.0.27.tar` & `py-helper-mod-0.0.28.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.27/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.27/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.27/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.27/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-20 03:04:04.000000 py-helper-mod-0.0.27/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80848 2023-05-20 03:00:35.000000 py-helper-mod-0.0.27/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.28/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.28/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-22 19:26:32.000000 py-helper-mod-0.0.28/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80910 2023-05-22 19:25:28.000000 py-helper-mod-0.0.28/py_helper.py
```

### Comparing `py-helper-mod-0.0.27/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.28/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.27
+Version: 0.0.28
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.27/LICENSE` & `py-helper-mod-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.27/PKG-INFO` & `py-helper-mod-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.27
+Version: 0.0.28
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.27/py_helper.py` & `py-helper-mod-0.0.28/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,27)
+VERSION=(0,0,28)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1126,23 +1126,24 @@
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
 				DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","Yes","yes","y","Y" ] else False
 
-def IsDebugEnabled(dbglabel):
+def IsDebugEnabled(dbglabel,test=None):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugEnabled
 
 	enabled = True
+	test = test if test is not None else True
 
 	if DebugEnabled is not None and dbglabel is not None:
-		if dbglabel in DebugEnabled:
+		if dbglabel in DebugEnabled and test:
 			enabled = DebugEnabled[dbglabel]
 
 	return enabled
 
 # A Centrally Controlled Debug Messaging System
 # msg : Message to print
 # func : A simple function to pass the message to (optional)
```

