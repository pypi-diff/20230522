# Comparing `tmp/tenma-serial-1.1.1.tar.gz` & `tmp/tenma-serial-1.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenma-serial-1.1.1.tar", last modified: Mon May 22 11:47:51 2023, max compression
+gzip compressed data, was "tenma-serial-1.1.1.dev1.tar", last modified: Mon May 22 11:40:14 2023, max compression
```

## Comparing `tenma-serial-1.1.1.tar` & `tenma-serial-1.1.1.dev1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      423 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/AUTHORS
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2599 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/ChangeLog
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35148 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/LICENSE.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3266 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/docs/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      634 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/Makefile
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2012 2023-05-22 10:21:39.000000 tenma-serial-1.1.1/docs/conf.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      513 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/index.rst
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/docs/library/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      951 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/library/api.rst
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      795 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/make.bat
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/docs/tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      599 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/tools/tenma-applet.rst
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1297 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/docs/tools/tenma-control.rst
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.164883 tenma-serial-1.1.1/examples/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/examples/python/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      736 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/examples/python/output_plotting.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/requirements.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1058 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      118 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/tenma/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       26 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/tenma/__init__.py
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)     8919 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/tenma/gtkIndicator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1242 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/tenma/logo.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7167 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/tenma/tenmaControl.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35097 2023-05-22 10:20:23.000000 tenma-serial-1.1.1/tenma/tenmaDcLib.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:47:51.168884 tenma-serial-1.1.1/tenma_serial.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      594 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      182 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-22 11:40:14.000000 tenma-serial-1.1.1/tenma_serial.egg-info/not-zip-safe
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        6 2023-05-22 11:47:51.000000 tenma-serial-1.1.1/tenma_serial.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      423 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/AUTHORS
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2586 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/ChangeLog
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35148 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/LICENSE.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4068 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3266 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/docs/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      634 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/Makefile
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2012 2023-05-22 10:21:39.000000 tenma-serial-1.1.1.dev1/docs/conf.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      513 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/index.rst
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/docs/library/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      951 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/library/api.rst
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      795 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/make.bat
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/docs/tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      599 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/tools/tenma-applet.rst
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1297 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/docs/tools/tenma-control.rst
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.841845 tenma-serial-1.1.1.dev1/examples/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/examples/python/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      736 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/examples/python/output_plotting.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/requirements.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1058 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      118 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/tenma/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       26 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/tenma/__init__.py
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)     8919 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/tenma/gtkIndicator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1242 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/tenma/logo.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7167 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/tenma/tenmaControl.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35097 2023-05-22 10:20:23.000000 tenma-serial-1.1.1.dev1/tenma/tenmaDcLib.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-22 11:40:14.845845 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4068 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      594 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      182 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/not-zip-safe
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        6 2023-05-22 11:40:14.000000 tenma-serial-1.1.1.dev1/tenma_serial.egg-info/top_level.txt
```

### Comparing `tenma-serial-1.1.1/ChangeLog` & `tenma-serial-1.1.1.dev1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 CHANGES
 =======
 
-1.1.1
------
-
 * Add support for Tenma model 72-2705, tested on HW (#11)
 
 v1.1.0
 ------
 
 * Cleanup code and improved README.md a bit
 * Updated Readme
```

### Comparing `tenma-serial-1.1.1/LICENSE.txt` & `tenma-serial-1.1.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/PKG-INFO` & `tenma-serial-1.1.1.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenma-serial
-Version: 1.1.1
+Version: 1.1.1.dev1
 Summary: Serial control of tenma device
 Home-page: https://github.com/kxtells/tenma-serial
 Author: Jordi Castells
 Author-email: jordi.kstells@gmail.com
 License: GNU-3
 Project-URL: Documentation, https://tenma-serial.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -14,15 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
-License-File: AUTHORS
 
 # Tenma DC power supply controllers
 
 Provides two basic controllers (tested on Linux) for a TENMA DC power supply via serial interface. Working on python 2.7 and python 3.
 
  * tenmaControl.py (tenma-control) (command line utility)
  * gtkIndicator.py (tenma-applet) (GTK indicator to sit on tray)
```

### Comparing `tenma-serial-1.1.1/README.md` & `tenma-serial-1.1.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/Makefile` & `tenma-serial-1.1.1.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/conf.py` & `tenma-serial-1.1.1.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/index.rst` & `tenma-serial-1.1.1.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/library/api.rst` & `tenma-serial-1.1.1.dev1/docs/library/api.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/make.bat` & `tenma-serial-1.1.1.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/tools/tenma-applet.rst` & `tenma-serial-1.1.1.dev1/docs/tools/tenma-applet.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/docs/tools/tenma-control.rst` & `tenma-serial-1.1.1.dev1/docs/tools/tenma-control.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/examples/python/output_plotting.py` & `tenma-serial-1.1.1.dev1/examples/python/output_plotting.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/setup.cfg` & `tenma-serial-1.1.1.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/tenma/gtkIndicator.py` & `tenma-serial-1.1.1.dev1/tenma/gtkIndicator.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/tenma/logo.png` & `tenma-serial-1.1.1.dev1/tenma/logo.png`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/tenma/tenmaControl.py` & `tenma-serial-1.1.1.dev1/tenma/tenmaControl.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/tenma/tenmaDcLib.py` & `tenma-serial-1.1.1.dev1/tenma/tenmaDcLib.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.1/tenma_serial.egg-info/PKG-INFO` & `tenma-serial-1.1.1.dev1/tenma_serial.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenma-serial
-Version: 1.1.1
+Version: 1.1.1.dev1
 Summary: Serial control of tenma device
 Home-page: https://github.com/kxtells/tenma-serial
 Author: Jordi Castells
 Author-email: jordi.kstells@gmail.com
 License: GNU-3
 Project-URL: Documentation, https://tenma-serial.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -14,15 +14,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
-License-File: AUTHORS
 
 # Tenma DC power supply controllers
 
 Provides two basic controllers (tested on Linux) for a TENMA DC power supply via serial interface. Working on python 2.7 and python 3.
 
  * tenmaControl.py (tenma-control) (command line utility)
  * gtkIndicator.py (tenma-applet) (GTK indicator to sit on tray)
```

### Comparing `tenma-serial-1.1.1/tenma_serial.egg-info/SOURCES.txt` & `tenma-serial-1.1.1.dev1/tenma_serial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

