# Comparing `tmp/pitop.robotics-0.30.0.post1.tar.gz` & `tmp/pitop.robotics-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.robotics-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:44 2022, max compression
+gzip compressed data, was "dist/pitop.robotics-0.31.0.post2.tar", last modified: Mon May 22 19:13:13 2023, max compression
```

## Comparing `pitop.robotics-0.30.0.post1.tar` & `pitop.robotics-0.31.0.post2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      977 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      141 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/blockpi_rover.py
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/configurations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8112 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/drive_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    40267 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/kalman.py
--rw-r--r--   0 runner    (1001) docker     (122)     1521 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/json/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/json/alex.json
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/json/bobbie.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/driving_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/goal_criteria.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/measurement_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9443 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/robot_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9014 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/navigation_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6937 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/navigation/navigator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/pan_tilt_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/pan_tilt_object_tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/pincer_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     9360 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/PID.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/PID.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7934 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/tilt_roll_head_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     4550 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/pitop/robotics/two_servo_assembly_calibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      977 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:44.000000 pitop.robotics-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-12-16 14:07:48.000000 pitop.robotics-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/blockpi_rover.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8112 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/drive_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40171 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/kalman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/json/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/json/alex.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/json/bobbie.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/driving_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/goal_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/measurement_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9443 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/robot_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9014 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/navigation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6937 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/navigation/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/pan_tilt_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/pan_tilt_object_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/pincer_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9360 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/PID.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/PID.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/tilt_roll_head_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4550 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/pitop/robotics/two_servo_assembly_calibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:13.000000 pitop.robotics-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-05-22 19:12:55.000000 pitop.robotics-0.31.0.post2/setup.py
```

### Comparing `pitop.robotics-0.30.0.post1/PKG-INFO` & `pitop.robotics-0.31.0.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.robotics
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Robotics
```

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/blockpi_rover.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/blockpi_rover.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/configurations.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/configurations.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/drive_controller.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/drive_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/LICENSE.md` & `pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/common.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
 
 
 def pretty_str(label, arr):
-    """
-    Generates a pretty printed NumPy array with an assignment. Optionally
+    """Generates a pretty printed NumPy array with an assignment. Optionally
     transposes column vectors so they are drawn on one line. Strictly speaking
-    arr can be any time convertible by `str(arr)`, but the output may not
-    be what you want if the type of the variable is not a scalar or an
-    ndarray.
+    arr can be any time convertible by `str(arr)`, but the output may not be
+    what you want if the type of the variable is not a scalar or an ndarray.
+
     Examples
     --------
     >>> pprint('cov', np.array([[4., .1], [.1, 5]]))
     cov = [[4.  0.1]
            [0.1 5. ]]
     >>> print(pretty_str('x', np.array([[1], [2], [3]])))
     x = [[1 2 3]].T
```

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/kalman.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/kalman.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,17 +231,17 @@
         self._log_likelihood = log(sys.float_info.min)
         self._likelihood = sys.float_info.min
         self._mahalanobis = None
 
         self.inv = np.linalg.inv
 
     def predict(self, u=None, B=None, F=None, Q=None):
-        """
-        Predict next state (prior) using the Kalman filter state propagation
+        """Predict next state (prior) using the Kalman filter state propagation
         equations.
+
         Parameters
         ----------
         u : np.array, default 0
             Optional control vector.
         B : np.array(dim_x, dim_u), or None
             Optional control transition matrix; a value of None
             will cause the filter to use `self.B`.
@@ -272,18 +272,18 @@
         self.P = self._alpha_sq * dot(dot(F, self.P), F.T) + Q
 
         # save prior
         self.x_prior = self.x.copy()
         self.P_prior = self.P.copy()
 
     def update(self, z, R=None, H=None):
-        """
-        Add a new measurement (z) to the Kalman filter.
-        If z is None, nothing is computed. However, x_post and P_post are
-        updated with the prior (x_prior, P_prior), and self.z is set to None.
+        """Add a new measurement (z) to the Kalman filter. If z is None,
+        nothing is computed. However, x_post and P_post are updated with the
+        prior (x_prior, P_prior), and self.z is set to None.
+
         Parameters
         ----------
         z : (dim_z, 1): array_like
             measurement for this update. z can be a scalar if dim_z is 1,
             otherwise it must be convertible to a column vector.
             If you pass in a value of H, z must be a column vector the
             of the correct size.
@@ -345,19 +345,19 @@
 
         # save measurement and posterior state
         self.z = deepcopy(z)
         self.x_post = self.x.copy()
         self.P_post = self.P.copy()
 
     def predict_steadystate(self, u=0, B=None):
-        """
-        Predict state (prior) using the Kalman filter state propagation
+        """Predict state (prior) using the Kalman filter state propagation
         equations. Only x is updated, P is left unchanged. See
         update_steadstate() for a longer explanation of when to use this
         method.
+
         Parameters
         ----------
         u : np.array
             Optional control vector. If non-zero, it is multiplied by B
             to create the control input into the system.
         B : np.array(dim_x, dim_u), or None
             Optional control transition matrix; a value of None
@@ -374,26 +374,24 @@
             self.x = dot(self.F, self.x)
 
         # save prior
         self.x_prior = self.x.copy()
         self.P_prior = self.P.copy()
 
     def update_steadystate(self, z):
-        """
-        Add a new measurement (z) to the Kalman filter without recomputing
-        the Kalman gain K, the state covariance P, or the system
-        uncertainty S.
+        """Add a new measurement (z) to the Kalman filter without recomputing
+        the Kalman gain K, the state covariance P, or the system uncertainty S.
         You can use this for LTI systems since the Kalman gain and covariance
         converge to a fixed value. Precompute these and assign them explicitly,
         or run the Kalman filter using the normal predict()/update(0 cycle
-        until they converge.
-        The main advantage of this call is speed. We do significantly less
-        computation, notably avoiding a costly matrix inversion.
-        Use in conjunction with predict_steadystate(), otherwise P will grow
-        without bound.
+        until they converge. The main advantage of this call is speed. We do
+        significantly less computation, notably avoiding a costly matrix
+        inversion. Use in conjunction with predict_steadystate(), otherwise P
+        will grow without bound.
+
         Parameters
         ----------
         z : (dim_z, 1): array_like
             measurement for this update. z can be a scalar if dim_z is 1,
             otherwise it must be convertible to a column vector.
         Examples
         --------
@@ -441,19 +439,19 @@
 
         # set to None to force recompute
         self._log_likelihood = None
         self._likelihood = None
         self._mahalanobis = None
 
     def update_correlated(self, z, R=None, H=None):
-        """Add a new measurement (z) to the Kalman filter assuming that
-        process noise and measurement noise are correlated as defined in
-        the `self.M` matrix.
-        A partial derivation can be found in [1]
-        If z is None, nothing is changed.
+        """Add a new measurement (z) to the Kalman filter assuming that process
+        noise and measurement noise are correlated as defined in the `self.M`
+        matrix. A partial derivation can be found in [1] If z is None, nothing
+        is changed.
+
         Parameters
         ----------
         z : (dim_z, 1): array_like
             measurement for this update. z can be a scalar if dim_z is 1,
             otherwise it must be convertible to a column vector.
         R : np.array, scalar, or None
             Optionally provide R to override the measurement noise for this
@@ -530,14 +528,15 @@
         Rs=None,
         Bs=None,
         us=None,
         update_first=False,
         saver=None,
     ):
         """Batch processes a sequences of measurements.
+
          Parameters
          ----------
          zs : list-like
              list of measurements at each time step `self.dt`. Missing
              measurements must be represented by `None`.
          Fs : None, list-like, default=None
              optional value or list of values to use for the state transition
@@ -635,46 +634,44 @@
 
         # state covariances from Kalman Filter
         covariances = zeros((n, self.dim_x, self.dim_x))
         covariances_p = zeros((n, self.dim_x, self.dim_x))
 
         if update_first:
             for i, (z, F, Q, H, R, B, u) in enumerate(zip(zs, Fs, Qs, Hs, Rs, Bs, us)):
-
                 self.update(z, R=R, H=H)
                 means[i, :] = self.x
                 covariances[i, :, :] = self.P
 
                 self.predict(u=u, B=B, F=F, Q=Q)
                 means_p[i, :] = self.x
                 covariances_p[i, :, :] = self.P
 
                 if saver is not None:
                     saver.save()
         else:
             for i, (z, F, Q, H, R, B, u) in enumerate(zip(zs, Fs, Qs, Hs, Rs, Bs, us)):
-
                 self.predict(u=u, B=B, F=F, Q=Q)
                 means_p[i, :] = self.x
                 covariances_p[i, :, :] = self.P
 
                 self.update(z, R=R, H=H)
                 means[i, :] = self.x
                 covariances[i, :, :] = self.P
 
                 if saver is not None:
                     saver.save()
 
         return (means, covariances, means_p, covariances_p)
 
     def rts_smoother(self, Xs, Ps, Fs=None, Qs=None, inv=np.linalg.inv):
-        """
-        Runs the Rauch-Tung-Striebel Kalman smoother on a set of
-        means and covariances computed by a Kalman filter. The usual input
-        would come from the output of `KalmanFilter.batch_filter()`.
+        """Runs the Rauch-Tung-Striebel Kalman smoother on a set of means and
+        covariances computed by a Kalman filter. The usual input would come
+        from the output of `KalmanFilter.batch_filter()`.
+
         Parameters
         ----------
         Xs : numpy.array
            array of the means (state variable x) of the output of a Kalman
            filter.
         Ps : numpy.array
             array of the covariances of the output of a kalman filter.
@@ -727,17 +724,17 @@
             K[k] = dot(dot(P[k], Fs[k + 1].T), inv(Pp[k]))
             x[k] += dot(K[k], x[k + 1] - dot(Fs[k + 1], x[k]))
             P[k] += dot(dot(K[k], P[k + 1] - Pp[k]), K[k].T)
 
         return (x, P, K, Pp)
 
     def get_prediction(self, u=None, B=None, F=None, Q=None):
-        """
-        Predict next state (prior) using the Kalman filter state propagation
+        """Predict next state (prior) using the Kalman filter state propagation
         equations and returns it without modifying the object.
+
         Parameters
         ----------
         u : np.array, default 0
             Optional control vector.
         B : np.array(dim_x, dim_u), or None
             Optional control transition matrix; a value of None
             will cause the filter to use `self.B`.
@@ -770,17 +767,17 @@
 
         # P = FPF' + Q
         P = self._alpha_sq * dot(dot(F, self.P), F.T) + Q
 
         return x, P
 
     def get_update(self, z=None):
-        """
-        Computes the new estimate based on measurement `z` and returns it
+        """Computes the new estimate based on measurement `z` and returns it
         without altering the state of the filter.
+
         Parameters
         ----------
         z : (dim_z, 1): array_like
             measurement for this update. z can be a scalar if dim_z is 1,
             otherwise it must be convertible to a column vector.
         Returns
         -------
@@ -823,16 +820,16 @@
 
         Does not alter the state of the filter.
         """
         z = reshape_z(z, self.dim_z, self.x.ndim)
         return z - dot(self.H, self.x_prior)
 
     def measurement_of_state(self, x):
-        """
-        Helper function that converts a state into a measurement.
+        """Helper function that converts a state into a measurement.
+
         Parameters
         ----------
         x : np.array
             kalman state vector
         Returns
         -------
         z : (dim_z, 1): array_like
@@ -862,17 +859,17 @@
             self._likelihood = exp(self.log_likelihood)
             if self._likelihood == 0:
                 self._likelihood = sys.float_info.min
         return self._likelihood
 
     @property
     def mahalanobis(self):
-        """
-        Mahalanobis distance of measurement. E.g. 3 means measurement
-        was 3 standard deviations away from the predicted value.
+        """Mahalanobis distance of measurement. E.g. 3 means measurement was 3
+        standard deviations away from the predicted value.
+
         Returns
         -------
         mahalanobis : float
         """
         if self._mahalanobis is None:
             self._mahalanobis = sqrt(float(dot(dot(self.y.T, self.SI), self.y)))
         return self._mahalanobis
```

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/filterpy/stats.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/filterpy/stats.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/json/alex.json` & `pitop.robotics-0.31.0.post2/pitop/robotics/json/alex.json`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/json/bobbie.json` & `pitop.robotics-0.31.0.post2/pitop/robotics/json/bobbie.json`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/driving_manager.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/driving_manager.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/goal_criteria.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/goal_criteria.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/measurement_scheduler.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/measurement_scheduler.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/robot_state.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/robot_state.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/core/utils.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/core/utils.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/navigation_controller.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/navigation/navigator.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/navigation/navigator.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/pan_tilt_controller.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/pan_tilt_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/pan_tilt_object_tracker.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/pan_tilt_object_tracker.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/pincer_controller.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/pincer_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/LICENSE.md` & `pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/PID.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/PID.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/simple_pid/PID.pyi` & `pitop.robotics-0.31.0.post2/pitop/robotics/simple_pid/PID.pyi`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/tilt_roll_head_controller.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/tilt_roll_head_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         self.__start_servo_oscillation(
             oscillate_request, thread_control=self.__nod_thread_control
         )
 
     def __start_servo_oscillation(
         self, oscillate_request: OscillateRequest, thread_control: ThreadControl
     ):
-
         if thread_control.thread.is_alive():
             thread_control.cancel = True
             thread_control.thread.join()
             thread_control.cancel = False
 
         if oscillate_request.block:
             self.__oscillate_servo(
```

### Comparing `pitop.robotics-0.30.0.post1/pitop/robotics/two_servo_assembly_calibrator.py` & `pitop.robotics-0.31.0.post2/pitop/robotics/two_servo_assembly_calibrator.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/PKG-INFO` & `pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.robotics
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Robotics
```

### Comparing `pitop.robotics-0.30.0.post1/pitop.robotics.egg-info/SOURCES.txt` & `pitop.robotics-0.31.0.post2/pitop.robotics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.30.0.post1/setup.py` & `pitop.robotics-0.31.0.post2/setup.py`

 * *Files identical despite different names*

