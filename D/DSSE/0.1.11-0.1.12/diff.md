# Comparing `tmp/DSSE-0.1.11.tar.gz` & `tmp/DSSE-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSSE-0.1.11.tar", last modified: Mon May 22 19:05:09 2023, max compression
+gzip compressed data, was "DSSE-0.1.12.tar", last modified: Mon May 22 19:18:06 2023, max compression
```

## Comparing `DSSE-0.1.11.tar` & `DSSE-0.1.12.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.222473 DSSE-0.1.11/
--rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DSSE-0.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0    14620 2023-05-22 19:05:09.222473 DSSE-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0    14054 2023-05-22 19:04:05.000000 DSSE-0.1.11/README.md
--rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DSSE-0.1.11/license.txt
--rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DSSE-0.1.11/pyproject.toml
--rw-rw-rw-   0        0        0      738 2023-05-22 19:05:09.222473 DSSE-0.1.11/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.178332 DSSE-0.1.11/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.198223 DSSE-0.1.11/src/DSSE/
--rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DSSE-0.1.11/src/DSSE/__init__.py
--rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DSSE-0.1.11/src/DSSE/env.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.214385 DSSE-0.1.11/src/DSSE/generator/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DSSE-0.1.11/src/DSSE/generator/__init__.py
--rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DSSE-0.1.11/src/DSSE/generator/dynamic_probability.py
--rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DSSE-0.1.11/src/DSSE/generator/map.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.222473 DSSE-0.1.11/src/DSSE/imgs/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DSSE-0.1.11/src/DSSE/imgs/__init__.py
--rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DSSE-0.1.11/src/DSSE/imgs/drone.png
--rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DSSE-0.1.11/src/DSSE/imgs/person-swimming.png
-drwxrwxrwx   0        0        0        0 2023-05-22 19:05:09.206240 DSSE-0.1.11/src/DSSE.egg-info/
--rw-rw-rw-   0        0        0    14620 2023-05-22 19:05:09.000000 DSSE-0.1.11/src/DSSE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-05-22 19:05:09.000000 DSSE-0.1.11/src/DSSE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:05:09.000000 DSSE-0.1.11/src/DSSE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 19:05:09.000000 DSSE-0.1.11/src/DSSE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.983030 DSSE-0.1.12/
+-rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DSSE-0.1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    14585 2023-05-22 19:18:06.983030 DSSE-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0    14019 2023-05-22 19:17:37.000000 DSSE-0.1.12/README.md
+-rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DSSE-0.1.12/license.txt
+-rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DSSE-0.1.12/pyproject.toml
+-rw-rw-rw-   0        0        0      738 2023-05-22 19:18:06.983030 DSSE-0.1.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.924181 DSSE-0.1.12/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.951015 DSSE-0.1.12/src/DSSE/
+-rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DSSE-0.1.12/src/DSSE/__init__.py
+-rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DSSE-0.1.12/src/DSSE/env.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.975031 DSSE-0.1.12/src/DSSE/generator/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DSSE-0.1.12/src/DSSE/generator/__init__.py
+-rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DSSE-0.1.12/src/DSSE/generator/dynamic_probability.py
+-rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DSSE-0.1.12/src/DSSE/generator/map.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.983030 DSSE-0.1.12/src/DSSE/imgs/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DSSE-0.1.12/src/DSSE/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DSSE-0.1.12/src/DSSE/imgs/drone.png
+-rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DSSE-0.1.12/src/DSSE/imgs/person-swimming.png
+drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.967036 DSSE-0.1.12/src/DSSE.egg-info/
+-rw-rw-rw-   0        0        0    14585 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/top_level.txt
```

### Comparing `DSSE-0.1.11/PKG-INFO` & `DSSE-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.1.11
+Version: 0.1.12
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -77,27 +77,26 @@
 
 In order to use the environment download the dependencies using the following command `pip install -r requirements.txt`.
 
 ### General Info
 | Import            | from core.environment.env import DroneSwarmSearch  |
 | -------------     | -------------                                      |
 | Action Space      | Discrete (5)                                       |
-| Action Values     | [0,1,2,3,4,5]                                      |  
+| Action Values     | [0,1,2,3,4]                                        |  
 | Agents            | N                                                  |
 | Observation Space | {droneN: {observation: ((x, y), probability_matrix}|
 
 ### Action Space
 | Value         | Meaning       |
 | ------------- | ------------- |
 | 0             | Move Left     |
 | 1             | Move Right    |
 | 2             | Move Up       |
 | 3             | Move Down     |
 | 4             | Search Cell   |
-| 5             | Idle          |
 
 ### Inputs
 | Inputs                    | Possible Values       | Default Values            |
 | -------------             | -------------         | -------------             |
 | `grid_size`               | `int(N)`              | `7`                       |
 | `render_mode`             | `"ansi" or "human"`   | `"ansi"`                  |
 | `render_grid`             | `bool`                | `False`                   |
```

### Comparing `DSSE-0.1.11/README.md` & `DSSE-0.1.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,27 +64,26 @@
 
 In order to use the environment download the dependencies using the following command `pip install -r requirements.txt`.
 
 ### General Info
 | Import            | from core.environment.env import DroneSwarmSearch  |
 | -------------     | -------------                                      |
 | Action Space      | Discrete (5)                                       |
-| Action Values     | [0,1,2,3,4,5]                                      |  
+| Action Values     | [0,1,2,3,4]                                        |  
 | Agents            | N                                                  |
 | Observation Space | {droneN: {observation: ((x, y), probability_matrix}|
 
 ### Action Space
 | Value         | Meaning       |
 | ------------- | ------------- |
 | 0             | Move Left     |
 | 1             | Move Right    |
 | 2             | Move Up       |
 | 3             | Move Down     |
 | 4             | Search Cell   |
-| 5             | Idle          |
 
 ### Inputs
 | Inputs                    | Possible Values       | Default Values            |
 | -------------             | -------------         | -------------             |
 | `grid_size`               | `int(N)`              | `7`                       |
 | `render_mode`             | `"ansi" or "human"`   | `"ansi"`                  |
 | `render_grid`             | `bool`                | `False`                   |
```

### Comparing `DSSE-0.1.11/license.txt` & `DSSE-0.1.12/license.txt`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/setup.cfg` & `DSSE-0.1.12/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 5353 450d 0a76 6572 7369 6f6e   = DSSE..version
-00000020: 203d 2030 2e31 2e31 310d 0a61 7574 686f   = 0.1.11..autho
+00000020: 203d 2030 2e31 2e31 320d 0a61 7574 686f   = 0.1.12..autho
 00000030: 7220 3d20 4c75 6973 2046 696c 6970 6520  r = Luis Filipe 
 00000040: 4361 7272 6574 652c 204d 616e 7565 6c20  Carrete, Manuel 
 00000050: 4361 7374 616e 6172 6573 2c20 456e 7269  Castanares, Enri
 00000060: 636f 2044 616d 6961 6e69 2c20 4c65 6f6e  co Damiani, Leon
 00000070: 6172 646f 204d 616c 7461 0d0a 6465 7363  ardo Malta..desc
 00000080: 7269 7074 696f 6e20 3d20 416e 2065 6e76  ription = An env
 00000090: 6972 6f6e 6d65 6e74 2074 6f20 7472 6169  ironment to trai
```

### Comparing `DSSE-0.1.11/src/DSSE/env.py` & `DSSE-0.1.12/src/DSSE/env.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/src/DSSE/generator/dynamic_probability.py` & `DSSE-0.1.12/src/DSSE/generator/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/src/DSSE/generator/map.py` & `DSSE-0.1.12/src/DSSE/generator/map.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/src/DSSE/imgs/drone.png` & `DSSE-0.1.12/src/DSSE/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/src/DSSE/imgs/person-swimming.png` & `DSSE-0.1.12/src/DSSE/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.11/src/DSSE.egg-info/PKG-INFO` & `DSSE-0.1.12/src/DSSE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.1.11
+Version: 0.1.12
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -77,27 +77,26 @@
 
 In order to use the environment download the dependencies using the following command `pip install -r requirements.txt`.
 
 ### General Info
 | Import            | from core.environment.env import DroneSwarmSearch  |
 | -------------     | -------------                                      |
 | Action Space      | Discrete (5)                                       |
-| Action Values     | [0,1,2,3,4,5]                                      |  
+| Action Values     | [0,1,2,3,4]                                        |  
 | Agents            | N                                                  |
 | Observation Space | {droneN: {observation: ((x, y), probability_matrix}|
 
 ### Action Space
 | Value         | Meaning       |
 | ------------- | ------------- |
 | 0             | Move Left     |
 | 1             | Move Right    |
 | 2             | Move Up       |
 | 3             | Move Down     |
 | 4             | Search Cell   |
-| 5             | Idle          |
 
 ### Inputs
 | Inputs                    | Possible Values       | Default Values            |
 | -------------             | -------------         | -------------             |
 | `grid_size`               | `int(N)`              | `7`                       |
 | `render_mode`             | `"ansi" or "human"`   | `"ansi"`                  |
 | `render_grid`             | `bool`                | `False`                   |
```

