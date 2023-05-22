# Comparing `tmp/audiconnectpy-1.4.2.tar.gz` & `tmp/audiconnectpy-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.4.2.tar", last modified: Sat May 20 15:50:38 2023, max compression
+gzip compressed data, was "audiconnectpy-1.4.3.tar", last modified: Mon May 22 06:56:27 2023, max compression
```

## Comparing `audiconnectpy-1.4.2.tar` & `audiconnectpy-1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:50:38.620926 audiconnectpy-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 15:50:37.000000 audiconnectpy-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.118575 audiconnectpy-1.4.3/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 06:56:26.000000 audiconnectpy-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/tests/__init__.py
```

### Comparing `audiconnectpy-1.4.2/LICENSE` & `audiconnectpy-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/PKG-INFO` & `audiconnectpy-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.2
+Version: 1.4.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.2/README.md` & `audiconnectpy-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/audiconnectpy/api.py` & `audiconnectpy-1.4.3/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/audiconnectpy/auth.py` & `audiconnectpy-1.4.3/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/audiconnectpy/helpers.py` & `audiconnectpy-1.4.3/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/audiconnectpy/models.py` & `audiconnectpy-1.4.3/audiconnectpy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,16 @@
         )
 
     @property
     def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         settings = self.data.getr("charger.settings", {})
         status = self.data.getr("charger.status", {})
-        charging = status.get("chargingStatusData", {})
-        cruising = status.get("cruisingRangeStatusData", {})
+        charging = status.getr("chargingStatusData", {})
+        cruising = status.getr("cruisingRangeStatusData", {})
         attrs = {
             "max_charge_current": settings.getr("maxChargeCurrent.content"),
             "charging_state": charging.getr("chargingState.content"),
             "actual_charge_rate": charging.getr("actualChargeRate.content"),
             "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
             "charging_power": charging.getr("chargingPower.content"),
             "charging_mode": charging.getr("chargingMode.content"),
```

### Comparing `audiconnectpy-1.4.2/audiconnectpy/services.py` & `audiconnectpy-1.4.3/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.4.3/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.2
+Version: 1.4.3
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.2/pyproject.toml` & `audiconnectpy-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.2/setup.py` & `audiconnectpy-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.4.2",
+    version="1.4.3",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

