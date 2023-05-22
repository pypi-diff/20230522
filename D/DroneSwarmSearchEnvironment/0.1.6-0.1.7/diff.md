# Comparing `tmp/DroneSwarmSearchEnvironment-0.1.6.tar.gz` & `tmp/DroneSwarmSearchEnvironment-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DroneSwarmSearchEnvironment-0.1.6.tar", last modified: Sun May 21 21:16:13 2023, max compression
+gzip compressed data, was "DroneSwarmSearchEnvironment-0.1.7.tar", last modified: Mon May 22 14:29:32 2023, max compression
```

## Comparing `DroneSwarmSearchEnvironment-0.1.6.tar` & `DroneSwarmSearchEnvironment-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.255978 DroneSwarmSearchEnvironment-0.1.6/
--rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DroneSwarmSearchEnvironment-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    14709 2023-05-21 21:16:13.255978 DroneSwarmSearchEnvironment-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    14121 2023-05-21 15:13:23.000000 DroneSwarmSearchEnvironment-0.1.6/README.md
--rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DroneSwarmSearchEnvironment-0.1.6/license.txt
--rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DroneSwarmSearchEnvironment-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-05-21 21:16:13.255978 DroneSwarmSearchEnvironment-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.172258 DroneSwarmSearchEnvironment-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.199982 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/
--rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/__init__.py
--rw-rw-rw-   0        0        0    17051 2023-05-21 21:15:06.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/env.py
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.247980 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/__init__.py
--rw-rw-rw-   0        0        0     6191 2023-05-20 18:31:57.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py
--rw-rw-rw-   0        0        0     1266 2023-04-24 18:09:38.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/map.py
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.247980 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/__init__.py
--rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/drone.png
--rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png
-drwxrwxrwx   0        0        0        0 2023-05-21 21:16:13.239978 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/
--rw-rw-rw-   0        0        0    14709 2023-05-21 21:16:13.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2023-05-21 21:16:13.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 21:16:13.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-21 21:16:13.000000 DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.287117 DroneSwarmSearchEnvironment-0.1.7/
+-rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DroneSwarmSearchEnvironment-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    14709 2023-05-22 14:29:32.288116 DroneSwarmSearchEnvironment-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    14121 2023-05-21 15:13:23.000000 DroneSwarmSearchEnvironment-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DroneSwarmSearchEnvironment-0.1.7/license.txt
+-rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DroneSwarmSearchEnvironment-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-05-22 14:29:32.289117 DroneSwarmSearchEnvironment-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.254116 DroneSwarmSearchEnvironment-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.266117 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/
+-rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/__init__.py
+-rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/env.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.278116 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/__init__.py
+-rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py
+-rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/map.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.286118 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/drone.png
+-rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png
+drwxrwxrwx   0        0        0        0 2023-05-22 14:29:32.274119 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/
+-rw-rw-rw-   0        0        0    14709 2023-05-22 14:29:32.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2023-05-22 14:29:32.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:29:32.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-22 14:29:32.000000 DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/top_level.txt
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/PKG-INFO` & `DroneSwarmSearchEnvironment-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroneSwarmSearchEnvironment
-Version: 0.1.6
+Version: 0.1.7
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/README.md` & `DroneSwarmSearchEnvironment-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.6/license.txt` & `DroneSwarmSearchEnvironment-0.1.7/license.txt`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.6/setup.cfg` & `DroneSwarmSearchEnvironment-0.1.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 726f 6e65 5377 6172 6d53 6561   = DroneSwarmSea
 00000020: 7263 6845 6e76 6972 6f6e 6d65 6e74 0d0a  rchEnvironment..
-00000030: 7665 7273 696f 6e20 3d20 302e 312e 360d  version = 0.1.6.
+00000030: 7665 7273 696f 6e20 3d20 302e 312e 370d  version = 0.1.7.
 00000040: 0a61 7574 686f 7220 3d20 4c75 6973 2046  .author = Luis F
 00000050: 696c 6970 6520 4361 7272 6574 652c 204d  ilipe Carrete, M
 00000060: 616e 7565 6c20 4361 7374 616e 6172 6573  anuel Castanares
 00000070: 2c20 456e 7269 636f 2044 616d 6961 6e69  , Enrico Damiani
 00000080: 2c20 4c65 6f6e 6172 646f 204d 616c 7461  , Leonardo Malta
 00000090: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000a0: 416e 2065 6e76 6972 6f6e 6d65 6e74 2074  An environment t
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/env.py` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,30 +309,28 @@
 
         return observations, rewards, terminations, truncations, infos
 
     def enable_render(self, mode="human"):
         if not self.renderOn and mode == "human":
             self.screen = pygame.display.set_mode(self.screen.get_size())
 
-
             self.drone_img = pygame.image.load(
                 os.path.dirname(__file__)+"/imgs/drone.png"
             ).convert()
             self.drone_img = pygame.transform.scale(
                 self.drone_img, (self.block_size, self.block_size)
             )
 
             self.person_img = pygame.image.load(
                 os.path.dirname(__file__)+"/imgs/person-swimming.png"
             ).convert()
             self.person_img = pygame.transform.scale(
                 self.person_img, (self.block_size, self.block_size)
             )
 
-
             self.renderOn = True
 
     def render(self):
         """Renders the environment."""
         self.enable_render(self.render_mode)
         self.draw()
         if self.render_mode == "human":
@@ -449,8 +447,8 @@
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent):
         # TODO: If x and y are the observation, then this should the observation space
         return MultiDiscrete([self.grid_size] * 2)
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent):
-        return [0, 1, 2, 3, 4]
+        return [0, 1, 2, 3, 4]
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/dynamic_probability.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,23 @@
             self.y = 0
         self.x += self.vector[0]
         self.y += self.vector[1]
         map_copy = zeros((len(self.map), len(self.map[0])), dtype=float)
         if self.initial_position[0] + int(self.y) < len(
             self.map
         ) and self.initial_position[1] + int(self.x) < len(self.map[0]):
-            map_copy[self.initial_position[0] + int(self.y)][
-                self.initial_position[1] + int(self.x)
-            ] += self.map[self.initial_position[0]][self.initial_position[1]]
-            self.initial_position[0] += int(self.y)
-            self.initial_position[1] += int(self.x)
+            if (
+                self.initial_position[0] + int(self.y) >= 0
+                and self.initial_position[1] + int(self.x) >= 0
+            ):
+                map_copy[self.initial_position[0] + int(self.y)][
+                    self.initial_position[1] + int(self.x)
+                ] += self.map[self.initial_position[0]][self.initial_position[1]]
+                self.initial_position[0] += int(self.y)
+                self.initial_position[1] += int(self.x)
         self.diffuse_probability(map_copy)
 
     def step(self):
         self.dynamic_probability()
         self.params = [
             1 + self.increase_area,
             1 + self.increase_area,
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/generator/map.py` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/generator/map.py`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/drone.png` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroneSwarmSearchEnvironment
-Version: 0.1.6
+Version: 0.1.7
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `DroneSwarmSearchEnvironment-0.1.6/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt` & `DroneSwarmSearchEnvironment-0.1.7/src/DroneSwarmSearchEnvironment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

