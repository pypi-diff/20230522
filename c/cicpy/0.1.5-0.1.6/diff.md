# Comparing `tmp/cicpy-0.1.5.tar.gz` & `tmp/cicpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicpy-0.1.5.tar", last modified: Mon May 22 17:34:22 2023, max compression
+gzip compressed data, was "cicpy-0.1.6.tar", last modified: Mon May 22 17:40:52 2023, max compression
```

## Comparing `cicpy-0.1.5.tar` & `cicpy-0.1.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.399498 cicpy-0.1.5/
--rw-r--r--   0 wulff      (502) staff       (20)     1070 2023-01-22 20:54:20.000000 cicpy-0.1.5/LICENSE
--rw-r--r--   0 wulff      (502) staff       (20)     2261 2023-05-22 17:34:22.399074 cicpy-0.1.5/PKG-INFO
--rw-r--r--   0 wulff      (502) staff       (20)     1699 2023-05-22 17:33:32.000000 cicpy-0.1.5/README.md
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.371879 cicpy-0.1.5/cicpy/
--rw-r--r--   0 wulff      (502) staff       (20)     1616 2023-05-22 17:26:30.000000 cicpy-0.1.5/cicpy/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     7068 2023-05-14 07:09:04.000000 cicpy-0.1.5/cicpy/cic.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.379236 cicpy-0.1.5/cicpy/ckt/
--rw-r--r--   0 wulff      (502) staff       (20)       96 2023-05-22 17:22:17.000000 cicpy-0.1.5/cicpy/ckt/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     2115 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/ckt/cktinstance.py
--rw-r--r--   0 wulff      (502) staff       (20)     2651 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/ckt/cktobject.py
--rw-r--r--   0 wulff      (502) staff       (20)     1962 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/ckt/device.py
--rw-r--r--   0 wulff      (502) staff       (20)     2487 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/ckt/subckt.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.385600 cicpy-0.1.5/cicpy/core/
--rw-r--r--   0 wulff      (502) staff       (20)      218 2023-05-22 17:23:40.000000 cicpy-0.1.5/cicpy/core/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)    11851 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/cell.py
--rw-r--r--   0 wulff      (502) staff       (20)     2661 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/design.py
--rw-r--r--   0 wulff      (502) staff       (20)     2509 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/instance.py
--rw-r--r--   0 wulff      (502) staff       (20)     3173 2023-04-06 19:28:47.000000 cicpy-0.1.5/cicpy/core/layoutcell.py
--rw-r--r--   0 wulff      (502) staff       (20)     2603 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/point.py
--rw-r--r--   0 wulff      (502) staff       (20)     2530 2023-04-06 15:50:55.000000 cicpy-0.1.5/cicpy/core/port.py
--rw-r--r--   0 wulff      (502) staff       (20)     9352 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/rect.py
--rw-r--r--   0 wulff      (502) staff       (20)     5331 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/rules.py
--rw-r--r--   0 wulff      (502) staff       (20)     1879 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/core/text.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.387077 cicpy-0.1.5/cicpy/eda/
--rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:24:03.000000 cicpy-0.1.5/cicpy/eda/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     4489 2023-05-14 17:16:19.000000 cicpy-0.1.5/cicpy/eda/xschem.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.388816 cicpy-0.1.5/cicpy/place/
--rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:27:10.000000 cicpy-0.1.5/cicpy/place/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     6181 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/place/placer.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.397758 cicpy-0.1.5/cicpy/printer/
--rw-r--r--   0 wulff      (502) staff       (20)      312 2023-05-22 17:25:51.000000 cicpy-0.1.5/cicpy/printer/__init__.py
--rw-r--r--   0 wulff      (502) staff       (20)     3315 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/cellinfoprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     3664 2023-04-06 15:22:29.000000 cicpy-0.1.5/cicpy/printer/designprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     8190 2023-04-08 17:44:20.000000 cicpy-0.1.5/cicpy/printer/magicprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     7426 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/mcprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     5650 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/skilllayprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)    18588 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/skillschprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     5680 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/spiceprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     6300 2023-05-22 16:57:28.000000 cicpy-0.1.5/cicpy/printer/svgprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)     2442 2023-01-22 20:54:20.000000 cicpy-0.1.5/cicpy/printer/verilogprinter.py
--rw-r--r--   0 wulff      (502) staff       (20)    15647 2023-04-10 14:59:58.000000 cicpy-0.1.5/cicpy/printer/xschemprinter.py
-drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:34:22.375755 cicpy-0.1.5/cicpy.egg-info/
--rw-r--r--   0 wulff      (502) staff       (20)     2261 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/PKG-INFO
--rw-r--r--   0 wulff      (502) staff       (20)      988 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/SOURCES.txt
--rw-r--r--   0 wulff      (502) staff       (20)        1 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/dependency_links.txt
--rw-r--r--   0 wulff      (502) staff       (20)       40 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/entry_points.txt
--rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/requires.txt
--rw-r--r--   0 wulff      (502) staff       (20)        6 2023-05-22 17:34:22.000000 cicpy-0.1.5/cicpy.egg-info/top_level.txt
--rw-r--r--   0 wulff      (502) staff       (20)      569 2023-05-22 17:08:51.000000 cicpy-0.1.5/pyproject.toml
--rw-r--r--   0 wulff      (502) staff       (20)       38 2023-05-22 17:34:22.399648 cicpy-0.1.5/setup.cfg
--rw-r--r--   0 wulff      (502) staff       (20)     1106 2023-05-22 17:08:46.000000 cicpy-0.1.5/setup.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:52.269121 cicpy-0.1.6/
+-rw-r--r--   0 wulff      (502) staff       (20)     1070 2023-01-22 20:54:20.000000 cicpy-0.1.6/LICENSE
+-rw-r--r--   0 wulff      (502) staff       (20)     2261 2023-05-22 17:40:52.268690 cicpy-0.1.6/PKG-INFO
+-rw-r--r--   0 wulff      (502) staff       (20)     1699 2023-05-22 17:33:32.000000 cicpy-0.1.6/README.md
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:51.741044 cicpy-0.1.6/cicpy/
+-rw-r--r--   0 wulff      (502) staff       (20)     1616 2023-05-22 17:26:30.000000 cicpy-0.1.6/cicpy/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     7068 2023-05-14 07:09:04.000000 cicpy-0.1.6/cicpy/cic.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:51.894254 cicpy-0.1.6/cicpy/ckt/
+-rw-r--r--   0 wulff      (502) staff       (20)       96 2023-05-22 17:22:17.000000 cicpy-0.1.6/cicpy/ckt/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2115 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/ckt/cktinstance.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2651 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/ckt/cktobject.py
+-rw-r--r--   0 wulff      (502) staff       (20)     1962 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/ckt/device.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2487 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/ckt/subckt.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:52.029225 cicpy-0.1.6/cicpy/core/
+-rw-r--r--   0 wulff      (502) staff       (20)      218 2023-05-22 17:23:40.000000 cicpy-0.1.6/cicpy/core/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)    11851 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/cell.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2661 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/design.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2509 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/instance.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3173 2023-04-06 19:28:47.000000 cicpy-0.1.6/cicpy/core/layoutcell.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2603 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/point.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2530 2023-04-06 15:50:55.000000 cicpy-0.1.6/cicpy/core/port.py
+-rw-r--r--   0 wulff      (502) staff       (20)     9352 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/rect.py
+-rw-r--r--   0 wulff      (502) staff       (20)     5331 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/rules.py
+-rw-r--r--   0 wulff      (502) staff       (20)     1879 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/core/text.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:52.051470 cicpy-0.1.6/cicpy/eda/
+-rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:24:03.000000 cicpy-0.1.6/cicpy/eda/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     4489 2023-05-14 17:16:19.000000 cicpy-0.1.6/cicpy/eda/xschem.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:52.094881 cicpy-0.1.6/cicpy/place/
+-rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:27:10.000000 cicpy-0.1.6/cicpy/place/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     6181 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/place/placer.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:52.247554 cicpy-0.1.6/cicpy/printer/
+-rw-r--r--   0 wulff      (502) staff       (20)      312 2023-05-22 17:25:51.000000 cicpy-0.1.6/cicpy/printer/__init__.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3315 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/cellinfoprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     3664 2023-04-06 15:22:29.000000 cicpy-0.1.6/cicpy/printer/designprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     8190 2023-04-08 17:44:20.000000 cicpy-0.1.6/cicpy/printer/magicprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     7426 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/mcprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     5650 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/skilllayprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)    18588 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/skillschprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     5680 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/spiceprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     6300 2023-05-22 16:57:28.000000 cicpy-0.1.6/cicpy/printer/svgprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)     2442 2023-01-22 20:54:20.000000 cicpy-0.1.6/cicpy/printer/verilogprinter.py
+-rw-r--r--   0 wulff      (502) staff       (20)    15647 2023-04-10 14:59:58.000000 cicpy-0.1.6/cicpy/printer/xschemprinter.py
+drwxr-xr-x   0 wulff      (502) staff       (20)        0 2023-05-22 17:40:51.828276 cicpy-0.1.6/cicpy.egg-info/
+-rw-r--r--   0 wulff      (502) staff       (20)     2261 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/PKG-INFO
+-rw-r--r--   0 wulff      (502) staff       (20)      988 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wulff      (502) staff       (20)        1 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wulff      (502) staff       (20)       40 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/entry_points.txt
+-rw-r--r--   0 wulff      (502) staff       (20)       46 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/requires.txt
+-rw-r--r--   0 wulff      (502) staff       (20)        6 2023-05-22 17:40:51.000000 cicpy-0.1.6/cicpy.egg-info/top_level.txt
+-rw-r--r--   0 wulff      (502) staff       (20)      569 2023-05-22 17:40:16.000000 cicpy-0.1.6/pyproject.toml
+-rw-r--r--   0 wulff      (502) staff       (20)       38 2023-05-22 17:40:52.290488 cicpy-0.1.6/setup.cfg
+-rw-r--r--   0 wulff      (502) staff       (20)     1089 2023-05-22 17:39:45.000000 cicpy-0.1.6/setup.py
```

### Comparing `cicpy-0.1.5/LICENSE` & `cicpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/PKG-INFO` & `cicpy-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cicpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Custom IC Creator Python Frontend
 Home-page: https://github.com/wulffern/cicpy
 Author: Carsten Wulff
 Author-email: Carsten Wulff <carsten@wulff.no>
 Project-URL: Homepage, https://github.com/wulffern/cicpy
 Project-URL: Bug Tracker, https://github.com/wulffern/cicpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Custom IC Creator Python
```

### Comparing `cicpy-0.1.5/README.md` & `cicpy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/__init__.py` & `cicpy-0.1.6/cicpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/cic.py` & `cicpy-0.1.6/cicpy/cic.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/ckt/cktinstance.py` & `cicpy-0.1.6/cicpy/ckt/cktinstance.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/ckt/cktobject.py` & `cicpy-0.1.6/cicpy/ckt/cktobject.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/ckt/device.py` & `cicpy-0.1.6/cicpy/ckt/device.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/ckt/subckt.py` & `cicpy-0.1.6/cicpy/ckt/subckt.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/cell.py` & `cicpy-0.1.6/cicpy/core/cell.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/design.py` & `cicpy-0.1.6/cicpy/core/design.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/instance.py` & `cicpy-0.1.6/cicpy/core/instance.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/layoutcell.py` & `cicpy-0.1.6/cicpy/core/layoutcell.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/point.py` & `cicpy-0.1.6/cicpy/core/point.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/port.py` & `cicpy-0.1.6/cicpy/core/port.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/rect.py` & `cicpy-0.1.6/cicpy/core/rect.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/rules.py` & `cicpy-0.1.6/cicpy/core/rules.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/core/text.py` & `cicpy-0.1.6/cicpy/core/text.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/eda/xschem.py` & `cicpy-0.1.6/cicpy/eda/xschem.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/place/placer.py` & `cicpy-0.1.6/cicpy/place/placer.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/cellinfoprinter.py` & `cicpy-0.1.6/cicpy/printer/cellinfoprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/designprinter.py` & `cicpy-0.1.6/cicpy/printer/designprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/magicprinter.py` & `cicpy-0.1.6/cicpy/printer/magicprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/mcprinter.py` & `cicpy-0.1.6/cicpy/printer/mcprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/skilllayprinter.py` & `cicpy-0.1.6/cicpy/printer/skilllayprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/skillschprinter.py` & `cicpy-0.1.6/cicpy/printer/skillschprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/spiceprinter.py` & `cicpy-0.1.6/cicpy/printer/spiceprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/svgprinter.py` & `cicpy-0.1.6/cicpy/printer/svgprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/verilogprinter.py` & `cicpy-0.1.6/cicpy/printer/verilogprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy/printer/xschemprinter.py` & `cicpy-0.1.6/cicpy/printer/xschemprinter.py`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/cicpy.egg-info/PKG-INFO` & `cicpy-0.1.6/cicpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cicpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Custom IC Creator Python Frontend
 Home-page: https://github.com/wulffern/cicpy
 Author: Carsten Wulff
 Author-email: Carsten Wulff <carsten@wulff.no>
 Project-URL: Homepage, https://github.com/wulffern/cicpy
 Project-URL: Bug Tracker, https://github.com/wulffern/cicpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Custom IC Creator Python
```

### Comparing `cicpy-0.1.5/cicpy.egg-info/SOURCES.txt` & `cicpy-0.1.6/cicpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cicpy-0.1.5/pyproject.toml` & `cicpy-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cicpy"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Carsten Wulff", email="carsten@wulff.no" },
 ]
 description = "Custom IC Creator Python Frontend"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cicpy-0.1.5/setup.py` & `cicpy-0.1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicpy",
-    version="0.1.5",
+    version="0.1.6",
     author="Carsten Wulff",
     author_email="carsten@wulff.no",
     description="Custom IC Creator Python Frontend",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wulffern/cicpy",
-    packages=setuptools.find_packages(),
-    python_requires='>=3.7',
+    packages=['cicpy'],
+    python_requires='>=3.8',
     entry_points = {'console_scripts': [
         'cicpy = cicpy.cic:cli',
     ]},
     install_requires = 'matplotlib numpy click svgwrite pyyaml pandas'.split(),
     classifiers = [
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
```

