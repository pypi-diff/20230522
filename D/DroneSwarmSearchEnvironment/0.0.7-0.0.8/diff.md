# Comparing `tmp/DroneSwarmSearchEnvironment-0.0.7-py3-none-any.whl.zip` & `tmp/DroneSwarmSearchEnvironment-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 13197 bytes, number of entries: 10
+Zip file size: 13369 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        4 b- defN 23-May-20 21:07 DroneSwarmSearchEnvironment/__init__.py
 -rw-rw-rw-  2.0 fat    17049 b- defN 23-May-20 21:20 DroneSwarmSearchEnvironment/env.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 21:18 DroneSwarmSearchEnvironment/generator/__init__.py
 -rw-rw-rw-  2.0 fat     6191 b- defN 23-May-20 18:31 DroneSwarmSearchEnvironment/generator/dynamic_probability.py
 -rw-rw-rw-  2.0 fat     1266 b- defN 23-Apr-24 18:09 DroneSwarmSearchEnvironment/generator/map.py
--rw-rw-rw-  2.0 fat    14385 b- defN 23-May-20 21:22 DroneSwarmSearchEnvironment-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 21:22 DroneSwarmSearchEnvironment-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1090 b- defN 23-May-20 21:22 DroneSwarmSearchEnvironment-0.0.7.dist-info/license.txt
--rw-rw-rw-  2.0 fat       28 b- defN 23-May-20 21:22 DroneSwarmSearchEnvironment-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      997 b- defN 23-May-20 21:22 DroneSwarmSearchEnvironment-0.0.7.dist-info/RECORD
-10 files, 41102 bytes uncompressed, 11437 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment/imgs/__init__.py
+-rw-rw-rw-  2.0 fat    14385 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment-0.0.8.dist-info/license.txt
+-rw-rw-rw-  2.0 fat       28 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1095 b- defN 23-May-20 21:27 DroneSwarmSearchEnvironment-0.0.8.dist-info/RECORD
+11 files, 41200 bytes uncompressed, 11445 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: DroneSwarmSearchEnvironment/generator/dynamic_probability.py
 Comment: 
 
 Filename: DroneSwarmSearchEnvironment/generator/map.py
 Comment: 
 
-Filename: DroneSwarmSearchEnvironment-0.0.7.dist-info/METADATA
+Filename: DroneSwarmSearchEnvironment/imgs/__init__.py
 Comment: 
 
-Filename: DroneSwarmSearchEnvironment-0.0.7.dist-info/WHEEL
+Filename: DroneSwarmSearchEnvironment-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: DroneSwarmSearchEnvironment-0.0.7.dist-info/license.txt
+Filename: DroneSwarmSearchEnvironment-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: DroneSwarmSearchEnvironment-0.0.7.dist-info/top_level.txt
+Filename: DroneSwarmSearchEnvironment-0.0.8.dist-info/license.txt
 Comment: 
 
-Filename: DroneSwarmSearchEnvironment-0.0.7.dist-info/RECORD
+Filename: DroneSwarmSearchEnvironment-0.0.8.dist-info/top_level.txt
+Comment: 
+
+Filename: DroneSwarmSearchEnvironment-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `DroneSwarmSearchEnvironment-0.0.7.dist-info/METADATA` & `DroneSwarmSearchEnvironment-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroneSwarmSearchEnvironment
-Version: 0.0.7
+Version: 0.0.8
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

## Comparing `DroneSwarmSearchEnvironment-0.0.7.dist-info/license.txt` & `DroneSwarmSearchEnvironment-0.0.8.dist-info/license.txt`

 * *Files identical despite different names*

## Comparing `DroneSwarmSearchEnvironment-0.0.7.dist-info/RECORD` & `DroneSwarmSearchEnvironment-0.0.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 DroneSwarmSearchEnvironment/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
 DroneSwarmSearchEnvironment/env.py,sha256=M5qn1vrh84mmYVA5Zm5bNKF_bpIKylwqnnaEqlr9FL4,17049
 DroneSwarmSearchEnvironment/generator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 DroneSwarmSearchEnvironment/generator/dynamic_probability.py,sha256=aafdljjaS-ko-YGISrwpIYUT0phQOHHOA8Qn0Wbd77s,6191
 DroneSwarmSearchEnvironment/generator/map.py,sha256=xdZVpoS4RPcv1nxzjphIxhTWDdSvfYhHqCLcOeYYA4c,1266
-DroneSwarmSearchEnvironment-0.0.7.dist-info/METADATA,sha256=Onpm7qoun3t3wV7ZSDTUy50zpWSVV5BrH_kX5VftUSw,14385
-DroneSwarmSearchEnvironment-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-DroneSwarmSearchEnvironment-0.0.7.dist-info/license.txt,sha256=g_5JdLm9CtfJcyvf2TcAh8HoUfX1ScU7q0QvODRJJnw,1090
-DroneSwarmSearchEnvironment-0.0.7.dist-info/top_level.txt,sha256=YvUtPwwnBOa4RluV1tzcvbAh-jnJnzIbIEHsnGyG1yQ,28
-DroneSwarmSearchEnvironment-0.0.7.dist-info/RECORD,,
+DroneSwarmSearchEnvironment/imgs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+DroneSwarmSearchEnvironment-0.0.8.dist-info/METADATA,sha256=bTDqNNWsjGKDBbon9rCN_hcH7-h_Ss6WPmN_o9GvIeo,14385
+DroneSwarmSearchEnvironment-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+DroneSwarmSearchEnvironment-0.0.8.dist-info/license.txt,sha256=g_5JdLm9CtfJcyvf2TcAh8HoUfX1ScU7q0QvODRJJnw,1090
+DroneSwarmSearchEnvironment-0.0.8.dist-info/top_level.txt,sha256=YvUtPwwnBOa4RluV1tzcvbAh-jnJnzIbIEHsnGyG1yQ,28
+DroneSwarmSearchEnvironment-0.0.8.dist-info/RECORD,,
```

