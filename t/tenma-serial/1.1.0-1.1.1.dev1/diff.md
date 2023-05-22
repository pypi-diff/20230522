# Comparing `tmp/tenma-serial-1.1.0.tar.gz` & `tmp/tenma-serial-1.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenma-serial-1.1.0.tar", last modified: Mon Aug 29 08:44:37 2022, max compression
+gzip compressed data, was "tenma-serial-1.1.1.dev1.tar", last modified: Mon May 22 11:40:14 2023, max compression
```

## Comparing `tenma-serial-1.1.0.tar` & `tenma-serial-1.1.1.dev1.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      390 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/AUTHORS
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2527 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/ChangeLog
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35148 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/LICENSE.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4845 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3223 2022-08-29 08:43:17.000000 tenma-serial-1.1.0/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/docs/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      634 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/Makefile
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2012 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/conf.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      513 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/index.rst
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/docs/library/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      951 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/library/api.rst
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      795 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/make.bat
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/docs/tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      599 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/tools/tenma-applet.rst
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1297 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/docs/tools/tenma-control.rst
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/examples/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/examples/python/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      736 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/examples/python/output_plotting.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/requirements.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1058 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      118 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/tenma/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       26 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/tenma/__init__.py
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)     8919 2022-08-29 08:43:17.000000 tenma-serial-1.1.0/tenma/gtkIndicator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1242 2022-08-29 08:42:04.000000 tenma-serial-1.1.0/tenma/logo.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7167 2022-08-29 08:43:08.000000 tenma-serial-1.1.0/tenma/tenmaControl.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34898 2022-08-29 08:43:17.000000 tenma-serial-1.1.0/tenma/tenmaDcLib.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2022-08-29 08:44:37.155918 tenma-serial-1.1.0/tenma_serial.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4845 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      625 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      182 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/not-zip-safe
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       47 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/pbr.json
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        9 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        6 2022-08-29 08:44:37.000000 tenma-serial-1.1.0/tenma_serial.egg-info/top_level.txt
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

### Comparing `tenma-serial-1.1.0/ChangeLog` & `tenma-serial-1.1.1.dev1/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 CHANGES
 =======
 
+* Add support for Tenma model 72-2705, tested on HW (#11)
+
 v1.1.0
 ------
 
 * Cleanup code and improved README.md a bit
 * Updated Readme
 * Basic formatting cleanup
 * 72-13330 3-channel PSU support (#10)
```

### Comparing `tenma-serial-1.1.0/LICENSE.txt` & `tenma-serial-1.1.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/README.md` & `tenma-serial-1.1.1.dev1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Supports the following models with predefined limits:
 
     * 72-2545 -> Tested on HW (@kxtells)
     * 72-2535 -> Set as manufacturer manual (not tested)
     * 72-2540 -> Set as manufacturer manual (not tested)
     * 72-2550 -> Tested on HW (@kxtells)
+    * 72-2705 -> Tested on HW (@ollie1400)
     * 72-2930 -> Set as manufacturer manual (not tested)
     * 72-2940 -> Set as manufacturer manual (not tested)
     * 72-13320 -> Set as manufacturer manual (not tested)
     * 72-13330 -> Tested on HW (thomas-phillips-nz)
 
 Also, even if not described, should support [Koradka
 models](https://sigrok.org/wiki/Korad_KAxxxxP_series) and other Velleman units
```

### Comparing `tenma-serial-1.1.0/docs/Makefile` & `tenma-serial-1.1.1.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/docs/conf.py` & `tenma-serial-1.1.1.dev1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'tenma-serial'
 copyright = '2020, Jordi Castells'
 author = 'Jordi Castells'
 
 # The full version, including alpha/beta/rc tags
-release = '1.0.0'
+release = '1.1.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `tenma-serial-1.1.0/docs/index.rst` & `tenma-serial-1.1.1.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/docs/library/api.rst` & `tenma-serial-1.1.1.dev1/docs/library/api.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/docs/make.bat` & `tenma-serial-1.1.1.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/docs/tools/tenma-applet.rst` & `tenma-serial-1.1.1.dev1/docs/tools/tenma-applet.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/docs/tools/tenma-control.rst` & `tenma-serial-1.1.1.dev1/docs/tools/tenma-control.rst`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/examples/python/output_plotting.py` & `tenma-serial-1.1.1.dev1/examples/python/output_plotting.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/setup.cfg` & `tenma-serial-1.1.1.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/tenma/gtkIndicator.py` & `tenma-serial-1.1.1.dev1/tenma/gtkIndicator.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/tenma/logo.png` & `tenma-serial-1.1.1.dev1/tenma/logo.png`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/tenma/tenmaControl.py` & `tenma-serial-1.1.1.dev1/tenma/tenmaControl.py`

 * *Files identical despite different names*

### Comparing `tenma-serial-1.1.0/tenma/tenmaDcLib.py` & `tenma-serial-1.1.1.dev1/tenma/tenmaDcLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 
 """
     tenmaDcLib is small python library to control a Tenma 72-XXXX programmable
     DC power supply, either from USB or Serial.
 
     Supported models:
 
-     * 72_2545 -> tested on HW
+     * 72_2545 -> Tested on HW
      * 72_2535 -> Set as manufacturer manual (not tested)
      * 72_2540 -> Set as manufacturer manual (not tested)
      * 72_2550 -> Tested on HW
+     * 72-2705 -> Tested on HW
      * 72_2930 -> Set as manufacturer manual (not tested)
      * 72_2940 -> Set as manufacturer manual (not tested)
      * 72_13320 -> Set as manufacturer manual (not tested)
      * 72_13330 -> Tested on HW
 
     Other units from Korad or Vellman might work as well since
     they use the same serial protocol.
@@ -684,14 +685,27 @@
     NCONFS = 5
     #:
     MAX_MA = 10000
     #:
     MAX_MV = 30000
 
 
+class Tenma72_2705(Tenma72Base):
+    #:
+    MATCH_STR = ["72-2705"]
+    #:
+    NCHANNELS = 1
+    #:
+    NCONFS = 5
+    #:
+    MAX_MA = 3100
+    #:
+    MAX_MV = 31000
+
+
 class Tenma72_2940(Tenma72Base):
     #:
     MATCH_STR = ["72-2940"]
     #:
     NCHANNELS = 1
     #:
     NCONFS = 5
```

### Comparing `tenma-serial-1.1.0/tenma_serial.egg-info/SOURCES.txt` & `tenma-serial-1.1.1.dev1/tenma_serial.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,10 +19,9 @@
 tenma/tenmaControl.py
 tenma/tenmaDcLib.py
 tenma_serial.egg-info/PKG-INFO
 tenma_serial.egg-info/SOURCES.txt
 tenma_serial.egg-info/dependency_links.txt
 tenma_serial.egg-info/entry_points.txt
 tenma_serial.egg-info/not-zip-safe
-tenma_serial.egg-info/pbr.json
 tenma_serial.egg-info/requires.txt
 tenma_serial.egg-info/top_level.txt
```

