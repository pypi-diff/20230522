# Comparing `tmp/qnpy-template-2.0.1.tar.gz` & `tmp/qnpy-template-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnpy-template-2.0.1.tar", last modified: Sun May 21 23:04:23 2023, max compression
+gzip compressed data, was "qnpy-template-2.0.2.tar", last modified: Mon May 22 04:13:33 2023, max compression
```

## Comparing `qnpy-template-2.0.1.tar` & `qnpy-template-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.083133 qnpy-template-2.0.1/
--rw-r--r--   0 nan        (501) staff       (20)      145 2023-05-21 22:36:42.000000 qnpy-template-2.0.1/LICENSE.txt
--rw-r--r--   0 nan        (501) staff       (20)      834 2023-05-21 23:04:23.083316 qnpy-template-2.0.1/PKG-INFO
--rw-r--r--   0 nan        (501) staff       (20)      227 2023-05-21 22:11:21.000000 qnpy-template-2.0.1/README.md
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.075787 qnpy-template-2.0.1/configuration/
--rw-r--r--   0 nan        (501) staff       (20)       19 2023-05-21 22:12:02.000000 qnpy-template-2.0.1/configuration/data.json
--rw-r--r--   0 nan        (501) staff       (20)     1486 2023-05-21 23:04:04.000000 qnpy-template-2.0.1/pyproject.toml
--rw-r--r--   0 nan        (501) staff       (20)     1135 2023-05-21 23:04:23.084197 qnpy-template-2.0.1/setup.cfg
--rw-r--r--   0 nan        (501) staff       (20)      250 2023-05-21 23:00:45.000000 qnpy-template-2.0.1/setup.py
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.073240 qnpy-template-2.0.1/src/
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.077653 qnpy-template-2.0.1/src/qnpy/
--rw-r--r--   0 nan        (501) staff       (20)       17 2023-05-21 22:52:30.000000 qnpy-template-2.0.1/src/qnpy/__init__.py
--rw-r--r--   0 nan        (501) staff       (20)     1441 2023-05-21 06:49:27.000000 qnpy-template-2.0.1/src/qnpy/calculator.py
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.081391 qnpy-template-2.0.1/src/qnpy_template.egg-info/
--rw-r--r--   0 nan        (501) staff       (20)      834 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/PKG-INFO
--rw-r--r--   0 nan        (501) staff       (20)      431 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/SOURCES.txt
--rw-r--r--   0 nan        (501) staff       (20)        1 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/dependency_links.txt
--rw-r--r--   0 nan        (501) staff       (20)       76 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/entry_points.txt
--rw-r--r--   0 nan        (501) staff       (20)       32 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/requires.txt
--rw-r--r--   0 nan        (501) staff       (20)        5 2023-05-21 23:04:23.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/top_level.txt
--rw-r--r--   0 nan        (501) staff       (20)        1 2023-05-21 22:35:05.000000 qnpy-template-2.0.1/src/qnpy_template.egg-info/zip-safe
-drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-21 23:04:23.082401 qnpy-template-2.0.1/test/
--rw-r--r--   0 nan        (501) staff       (20)       54 2023-05-21 01:03:18.000000 qnpy-template-2.0.1/test/test_calculator.py
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.282848 qnpy-template-2.0.2/
+-rw-r--r--   0 nan        (501) staff       (20)      145 2023-05-21 22:36:42.000000 qnpy-template-2.0.2/LICENSE.txt
+-rw-r--r--   0 nan        (501) staff       (20)       26 2023-05-22 03:39:01.000000 qnpy-template-2.0.2/MANIFEST.in
+-rw-r--r--   0 nan        (501) staff       (20)      834 2023-05-22 04:13:33.282982 qnpy-template-2.0.2/PKG-INFO
+-rw-r--r--   0 nan        (501) staff       (20)      227 2023-05-21 22:11:21.000000 qnpy-template-2.0.2/README.md
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.278145 qnpy-template-2.0.2/configuration/
+-rw-r--r--   0 nan        (501) staff       (20)      105 2023-05-22 03:20:35.000000 qnpy-template-2.0.2/configuration/sample.json
+-rw-r--r--   0 nan        (501) staff       (20)     1486 2023-05-21 23:04:04.000000 qnpy-template-2.0.2/pyproject.toml
+-rw-r--r--   0 nan        (501) staff       (20)     1135 2023-05-22 04:13:33.283819 qnpy-template-2.0.2/setup.cfg
+-rw-r--r--   0 nan        (501) staff       (20)      654 2023-05-22 04:10:52.000000 qnpy-template-2.0.2/setup.py
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.275235 qnpy-template-2.0.2/src/
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.279469 qnpy-template-2.0.2/src/qnpy/
+-rw-r--r--   0 nan        (501) staff       (20)       18 2023-05-22 04:13:05.000000 qnpy-template-2.0.2/src/qnpy/__init__.py
+-rw-r--r--   0 nan        (501) staff       (20)     1508 2023-05-22 03:23:22.000000 qnpy-template-2.0.2/src/qnpy/calculator.py
+-rw-r--r--   0 nan        (501) staff       (20)      201 2023-05-22 03:39:56.000000 qnpy-template-2.0.2/src/qnpy/data.json
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.281870 qnpy-template-2.0.2/src/qnpy_template.egg-info/
+-rw-r--r--   0 nan        (501) staff       (20)      834 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/PKG-INFO
+-rw-r--r--   0 nan        (501) staff       (20)      482 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/SOURCES.txt
+-rw-r--r--   0 nan        (501) staff       (20)        1 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/dependency_links.txt
+-rw-r--r--   0 nan        (501) staff       (20)       76 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/entry_points.txt
+-rw-r--r--   0 nan        (501) staff       (20)       32 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/requires.txt
+-rw-r--r--   0 nan        (501) staff       (20)        5 2023-05-22 04:13:33.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/top_level.txt
+-rw-r--r--   0 nan        (501) staff       (20)        1 2023-05-22 04:13:32.000000 qnpy-template-2.0.2/src/qnpy_template.egg-info/zip-safe
+drwxr-xr-x   0 nan        (501) staff       (20)        0 2023-05-22 04:13:33.282580 qnpy-template-2.0.2/test/
+-rw-r--r--   0 nan        (501) staff       (20)       54 2023-05-21 01:03:18.000000 qnpy-template-2.0.2/test/test_calculator.py
+-rw-r--r--   0 nan        (501) staff       (20)      297 2023-05-22 04:09:55.000000 qnpy-template-2.0.2/test/test_data.py
```

### Comparing `qnpy-template-2.0.1/PKG-INFO` & `qnpy-template-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnpy-template
-Version: 2.0.1
+Version: 2.0.2
 Summary: python library template repo
 Author-email: World Automation <allworldautomation@gmail.com>
 License: Copyright (C) Nan Qin - All Rights Reserved
         Unauthorized copying of this file, via any medium is strictly prohibited
         Proprietary and confidential
 Keywords: template
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qnpy-template-2.0.1/pyproject.toml` & `qnpy-template-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qnpy-template-2.0.1/setup.cfg` & `qnpy-template-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `qnpy-template-2.0.1/src/qnpy/calculator.py` & `qnpy-template-2.0.2/src/qnpy/calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import math
 
 
+
 class Speed:
     def __init__(self, tire_spec, gear_ratios, axle_ratio) -> None:
         self.tire_spec = tire_spec
         self.gear_ratios = gear_ratios
         self.axle_ratio = axle_ratio
-        
+
         self.tire_diameter = self._tire_diameter()
 
     def _tire_diameter(self):
         return 2 * self.tire_spec[0] * self.tire_spec[1] / 100 + self.tire_spec[2] * 25.4
-    
-    def speed(self, rpm_range, mph = False):
-        print(f"{len(self.gear_ratios)} gears: ratio {', '.join(map(str, self.gear_ratios))}, final drive axle ratio {self.axle_ratio}, tire spec {self.tire_spec[0]}/{self.tire_spec[1]} R{self.tire_spec[2]}, diameter {self.tire_diameter}mm")
+
+    def speed(self, rpm_range, mph=False):
+        print(
+            f"{len(self.gear_ratios)} gears: ratio {', '.join(map(str, self.gear_ratios))}, final drive axle ratio {self.axle_ratio}, tire spec {self.tire_spec[0]}/{self.tire_spec[1]} R{self.tire_spec[2]}, diameter {self.tire_diameter}mm"
+        )
         print(f'speed in {"mph" if mph else "km/h"}')
         wheel_perimeter = self.tire_diameter * math.pi
         for rpm in rpm_range:
             speed_in_km_per_hour = []
             for gear_ratio in self.gear_ratios:
                 wheel_rpm = rpm / gear_ratio / self.axle_ratio
                 distance_mm_per_minute = wheel_rpm * wheel_perimeter
                 speed_in_km_per_hour.append(distance_mm_per_minute * 60 / 1000_000)
 
             ratio = 0.621371 if mph else 1
-            print(', '.join([f'RPM@{rpm}'] + [str(round(speed * ratio)) for speed in speed_in_km_per_hour]))
-    
+            print(
+                ", ".join(
+                    [f"RPM@{rpm}"] + [str(round(speed * ratio)) for speed in speed_in_km_per_hour]
+                )
+            )
 
-    
 
 speed = Speed((215, 40, 18), [3.63, 2.19, 1.54, 1.21, 1.0, 0.77], 4.1)
 speed.speed(range(100, 1000, 100), True)
 speed.speed(range(1000, 10000, 1000), True)
```

### Comparing `qnpy-template-2.0.1/src/qnpy_template.egg-info/PKG-INFO` & `qnpy-template-2.0.2/src/qnpy_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnpy-template
-Version: 2.0.1
+Version: 2.0.2
 Summary: python library template repo
 Author-email: World Automation <allworldautomation@gmail.com>
 License: Copyright (C) Nan Qin - All Rights Reserved
         Unauthorized copying of this file, via any medium is strictly prohibited
         Proprietary and confidential
 Keywords: template
 Classifier: Programming Language :: Python :: 3
```

