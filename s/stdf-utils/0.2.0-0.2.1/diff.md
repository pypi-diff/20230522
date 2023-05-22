# Comparing `tmp/stdf-utils-0.2.0.tar.gz` & `tmp/stdf-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf-utils-0.2.0.tar", last modified: Sat May 20 07:49:24 2023, max compression
+gzip compressed data, was "stdf-utils-0.2.1.tar", last modified: Mon May 22 05:33:13 2023, max compression
```

## Comparing `stdf-utils-0.2.0.tar` & `stdf-utils-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.290698 stdf-utils-0.2.0/
--rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1340 2023-05-20 07:49:24.288697 stdf-utils-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 07:49:24.291697 stdf-utils-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-20 07:32:15.000000 stdf-utils-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.226051 stdf-utils-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.257050 stdf-utils-0.2.0/src/stdf_utils/
--rw-rw-rw-   0        0        0      208 2023-05-20 06:47:21.000000 stdf-utils-0.2.0/src/stdf_utils/__init__.py
--rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_patch.py
--rw-rw-rw-   0        0        0     2340 2023-05-20 07:27:00.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_per_td.py
--rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_record.py
--rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_to_csv.py
--rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.0/src/stdf_utils/stdf_to_txt.py
--rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.0/src/stdf_utils/util.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.270049 stdf-utils-0.2.0/src/stdf_utils.egg-info/
--rw-rw-rw-   0        0        0     1340 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 07:49:24.000000 stdf-utils-0.2.0/src/stdf_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 07:49:24.285715 stdf-utils-0.2.0/tests/
--rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.0/tests/test_stdf_patch.py
--rw-rw-rw-   0        0        0      449 2023-05-20 07:30:00.000000 stdf-utils-0.2.0/tests/test_stdf_per_td.py
--rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.0/tests/test_stdf_record.py
--rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.0/tests/test_stdf_to_csv.py
--rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.0/tests/test_stdf_to_txt.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.653240 stdf-utils-0.2.1/
+-rw-rw-rw-   0        0        0     1103 2023-05-16 00:45:08.000000 stdf-utils-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1340 2023-05-22 05:33:13.652239 stdf-utils-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-16 00:45:08.000000 stdf-utils-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:33:13.654240 stdf-utils-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-22 05:32:16.000000 stdf-utils-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.573937 stdf-utils-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.613965 stdf-utils-0.2.1/src/stdf_utils/
+-rw-rw-rw-   0        0        0      212 2023-05-22 05:24:16.000000 stdf-utils-0.2.1/src/stdf_utils/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-05-20 05:29:38.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_patch.py
+-rw-rw-rw-   0        0        0     2472 2023-05-22 05:26:05.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_per_part.py
+-rw-rw-rw-   0        0        0    27579 2023-05-20 05:25:28.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_record.py
+-rw-rw-rw-   0        0        0     2655 2023-05-20 06:45:50.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_to_csv.py
+-rw-rw-rw-   0        0        0      503 2023-05-20 04:14:04.000000 stdf-utils-0.2.1/src/stdf_utils/stdf_to_txt.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 03:02:13.000000 stdf-utils-0.2.1/src/stdf_utils/util.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.627964 stdf-utils-0.2.1/src/stdf_utils.egg-info/
+-rw-rw-rw-   0        0        0     1340 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 05:33:13.000000 stdf-utils-0.2.1/src/stdf_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 05:33:13.647965 stdf-utils-0.2.1/tests/
+-rw-rw-rw-   0        0        0      728 2023-05-20 06:30:13.000000 stdf-utils-0.2.1/tests/test_stdf_patch.py
+-rw-rw-rw-   0        0        0      544 2023-05-22 05:28:49.000000 stdf-utils-0.2.1/tests/test_stdf_per_part.py
+-rw-rw-rw-   0        0        0      505 2023-05-20 06:31:39.000000 stdf-utils-0.2.1/tests/test_stdf_record.py
+-rw-rw-rw-   0        0        0      677 2023-05-20 07:41:12.000000 stdf-utils-0.2.1/tests/test_stdf_to_csv.py
+-rw-rw-rw-   0        0        0      407 2023-05-20 07:24:32.000000 stdf-utils-0.2.1/tests/test_stdf_to_txt.py
```

### Comparing `stdf-utils-0.2.0/LICENSE` & `stdf-utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/PKG-INFO` & `stdf-utils-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.0/setup.py` & `stdf-utils-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 NAME = 'stdf-utils'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'stdf file parser and emitter'
 LONG_DESCRIPTION = """\
 stdf is the standard format of ATE result, and this pacakge supports
 reading and (possibly) editing the stdf file comes form ATE.
 """
 AUTHOR = "Peter JC. Wu"
 AUTHOR_EMAIL = "wolf952@gmail.com"
```

### Comparing `stdf-utils-0.2.0/src/stdf_utils/stdf_patch.py` & `stdf-utils-0.2.1/src/stdf_utils/stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/src/stdf_utils/stdf_per_td.py` & `stdf-utils-0.2.1/src/stdf_utils/stdf_per_part.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import os.path
 from collections import defaultdict
 from copy import copy
 from .stdf_record import StdfRecord
 from .util import OpenFile
 
 
-class StdfPerTD:
-    def __init__(self, stdf_path: str, ptr_filter=None, ptr_extra_fields=None):
+class StdfPerPart:
+    def __init__(self,
+                 stdf_path: str,
+                 ptr_filter=None,
+                 ptr_extra_fields=None,
+                 extra_handler=None):
         self.stdf_path = stdf_path
-        self.ptr_filter = ptr_filter or (lambda x: True)
-        self.ptr_extra_fields = ptr_extra_fields or (lambda x: {})
+        self.ptr_filter = ptr_filter or (lambda d: True)
+        self.ptr_extra_fields = ptr_extra_fields or (lambda d: {})
         self.previous_rec: dict = {}
         self.handlers = {
             "Mir": self.mir_handler,
             "Ptr": self.ptr_handler,
             "Prr": self.prr_handler,
+            **(extra_handler or {}),
         }
         # cache
         self.mir = {}
         self.prr = {}
         self.ptr = defaultdict(list)
 
     def __iter__(self):
```

### Comparing `stdf-utils-0.2.0/src/stdf_utils/stdf_record.py` & `stdf-utils-0.2.1/src/stdf_utils/stdf_record.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/src/stdf_utils/stdf_to_csv.py` & `stdf-utils-0.2.1/src/stdf_utils/stdf_to_csv.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/src/stdf_utils/util.py` & `stdf-utils-0.2.1/src/stdf_utils/util.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/src/stdf_utils.egg-info/PKG-INFO` & `stdf-utils-0.2.1/src/stdf_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: stdf file parser and emitter
 Author: Peter JC. Wu
 Author-email: wolf952@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/peterjcwu/stdf-utils
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `stdf-utils-0.2.0/tests/test_stdf_patch.py` & `stdf-utils-0.2.1/tests/test_stdf_patch.py`

 * *Files identical despite different names*

### Comparing `stdf-utils-0.2.0/tests/test_stdf_to_csv.py` & `stdf-utils-0.2.1/tests/test_stdf_to_csv.py`

 * *Files identical despite different names*

