# Comparing `tmp/DroneSwarmSearchEnvironment-0.1.8.tar.gz` & `tmp/DroneSwarmSearchEnvironment-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DroneSwarmSearchEnvironment-0.1.8.tar", last modified: Mon May 22 14:40:30 2023, max compression
+gzip compressed data, was "DroneSwarmSearchEnvironment-0.1.9.tar", last modified: Mon May 22 18:58:10 2023, max compression
```

## Comparing `DroneSwarmSearchEnvironment-0.1.8.tar` & `DroneSwarmSearchEnvironment-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.527335 DroneSwarmSearchEnvironment-0.1.8/
--rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DroneSwarmSearchEnvironment-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    14676 2023-05-22 14:40:30.528336 DroneSwarmSearchEnvironment-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    14088 2023-05-22 14:40:11.000000 DroneSwarmSearchEnvironment-0.1.8/README.md
--rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DroneSwarmSearchEnvironment-0.1.8/license.txt
--rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DroneSwarmSearchEnvironment-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-05-22 14:40:30.529333 DroneSwarmSearchEnvironment-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.490335 DroneSwarmSearchEnvironment-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.511334 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/
--rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/__init__.py
--rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/env.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.522332 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/__init__.py
--rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py
--rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/map.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.526334 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/__init__.py
--rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/drone.png
--rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png
-drwxrwxrwx   0        0        0        0 2023-05-22 14:40:30.517334 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/
--rw-rw-rw-   0        0        0    14676 2023-05-22 14:40:30.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2023-05-22 14:40:30.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:40:30.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-22 14:40:30.000000 DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.141144 DroneSwarmSearchEnvironment-0.1.9/
+-rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DroneSwarmSearchEnvironment-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    14676 2023-05-22 18:58:10.141144 DroneSwarmSearchEnvironment-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    14088 2023-05-22 14:44:31.000000 DroneSwarmSearchEnvironment-0.1.9/README.md
+-rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DroneSwarmSearchEnvironment-0.1.9/license.txt
+-rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DroneSwarmSearchEnvironment-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-05-22 18:58:10.149144 DroneSwarmSearchEnvironment-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.093509 DroneSwarmSearchEnvironment-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.117131 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/
+-rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/__init__.py
+-rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/env.py
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.125144 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/__init__.py
+-rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/dynamic_probability.py
+-rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/map.py
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.133148 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/drone.png
+-rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/person-swimming.png
+drwxrwxrwx   0        0        0        0 2023-05-22 18:58:10.141144 DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/
+-rw-rw-rw-   0        0        0    14676 2023-05-22 18:58:10.000000 DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-05-22 18:58:10.000000 DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 18:58:10.000000 DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-22 18:58:10.000000 DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/top_level.txt
```

### Comparing `DroneSwarmSearchEnvironment-0.1.8/PKG-INFO` & `DroneSwarmSearchEnvironment-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroneSwarmSearchEnvironment
-Version: 0.1.8
+Version: 0.1.9
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `DroneSwarmSearchEnvironment-0.1.8/README.md` & `DroneSwarmSearchEnvironment-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/license.txt` & `DroneSwarmSearchEnvironment-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/setup.cfg` & `DroneSwarmSearchEnvironment-0.1.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 726f 6e65 5377 6172 6d53 6561   = DroneSwarmSea
 00000020: 7263 6845 6e76 6972 6f6e 6d65 6e74 0d0a  rchEnvironment..
-00000030: 7665 7273 696f 6e20 3d20 302e 312e 380d  version = 0.1.8.
+00000030: 7665 7273 696f 6e20 3d20 302e 312e 390d  version = 0.1.9.
 00000040: 0a61 7574 686f 7220 3d20 4c75 6973 2046  .author = Luis F
 00000050: 696c 6970 6520 4361 7272 6574 652c 204d  ilipe Carrete, M
 00000060: 616e 7565 6c20 4361 7374 616e 6172 6573  anuel Castanares
 00000070: 2c20 456e 7269 636f 2044 616d 6961 6e69  , Enrico Damiani
 00000080: 2c20 4c65 6f6e 6172 646f 204d 616c 7461  , Leonardo Malta
 00000090: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000a0: 416e 2065 6e76 6972 6f6e 6d65 6e74 2074  An environment t
```

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/env.py` & `DroneSwarmSearchEnvironment-0.1.9/src/DSSE/env.py`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py` & `DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/generator/map.py` & `DroneSwarmSearchEnvironment-0.1.9/src/DSSE/generator/map.py`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/drone.png` & `DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png` & `DroneSwarmSearchEnvironment-0.1.9/src/DSSE/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.8/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO` & `DroneSwarmSearchEnvironment-0.1.9/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroneSwarmSearchEnvironment
-Version: 0.1.8
+Version: 0.1.9
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

