# Comparing `tmp/jupyterhub-backendspawner-0.3.0.tar.gz` & `tmp/jupyterhub-backendspawner-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.3.0.tar", last modified: Wed May 17 13:03:16 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.3.1.tar", last modified: Mon May 22 14:43:38 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.3.0.tar` & `jupyterhub-backendspawner-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.0/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.0/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.3.0/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10231 2023-05-17 12:59:06.000000 jupyterhub-backendspawner-0.3.0/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-17 13:03:16.000000 jupyterhub-backendspawner-0.3.0/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-17 13:03:16.351825 jupyterhub-backendspawner-0.3.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-17 12:59:38.000000 jupyterhub-backendspawner-0.3.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.1/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.1/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.3.1/backendspawner/backendspawner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10209 2023-05-22 14:42:59.000000 jupyterhub-backendspawner-0.3.1/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-22 14:43:05.000000 jupyterhub-backendspawner-0.3.1/setup.py
```

### Comparing `jupyterhub-backendspawner-0.3.0/LICENSE` & `jupyterhub-backendspawner-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.0/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.3.1/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.0/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.3.1/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.0/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.3.1/backendspawner/eventspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class EventBackendSpawner(BackendSpawner):
     _yielded_events = []
     _cancel_event_yielded = False
     latest_events = []
     events = {}
-    clear_events = True
     yield_wait_seconds = 1
 
     def get_state(self):
         """get the current state"""
         state = super().get_state()
         if self.events:
             if type(self.events) != dict:
@@ -47,22 +46,21 @@
         return state
 
     def load_state(self, state):
         """load state from the database"""
         super().load_state(state)
         if "events" in state:
             self.events = state["events"]
+            if "latest" in self.events:
+                self.latest_events = self.events["latest"]
 
     def clear_state(self):
         """clear any state (called after shutdown)"""
         super().clear_state()
         self._cancel_event_yielded = False
-        if self.clear_events:
-            self.events = {}
-            self.clear_events = False
 
     async def _generate_progress(self):
         """Private wrapper of progress generator
 
         This method is always an async generator and will always yield at least one event.
         """
         if not self._spawn_pending:
```

### Comparing `jupyterhub-backendspawner-0.3.0/setup.py` & `jupyterhub-backendspawner-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.3.0",
+    version="0.3.1",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

