# Comparing `tmp/nsdotpy-1.3.3.tar.gz` & `tmp/nsdotpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.3.3.tar", max compression
+gzip compressed data, was "nsdotpy-1.3.4.tar", max compression
```

## Comparing `nsdotpy-1.3.3.tar` & `nsdotpy-1.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-22 07:36:09.269865 nsdotpy-1.3.3/LICENSE.md
--rw-r--r--   0        0        0     2440 2023-05-22 07:36:09.269865 nsdotpy-1.3.3/README.md
--rw-r--r--   0        0        0      790 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/__init__.py
--rw-r--r--   0        0        0    46894 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/nsdotpy/valid.py
--rw-r--r--   0        0        0      719 2023-05-22 07:36:09.285865 nsdotpy-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-22 08:06:54.591861 nsdotpy-1.3.4/LICENSE.md
+-rw-r--r--   0        0        0     2440 2023-05-22 08:06:54.591861 nsdotpy-1.3.4/README.md
+-rw-r--r--   0        0        0      790 2023-05-22 08:06:54.607861 nsdotpy-1.3.4/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    46894 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/nsdotpy/valid.py
+-rw-r--r--   0        0        0      719 2023-05-22 08:06:54.611861 nsdotpy-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.4/PKG-INFO
```

### Comparing `nsdotpy-1.3.3/LICENSE.md` & `nsdotpy-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.3/README.md` & `nsdotpy-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.3/nsdotpy/__init__.py` & `nsdotpy-1.3.4/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.3/nsdotpy/session.py` & `nsdotpy-1.3.4/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.3.3"
+        self.VERSION = "1.3.4"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -81,29 +81,29 @@
         # https://forum.nationstates.net/viewtopic.php?p=16394966&sid=be37623536dbc8cee42d8d043945b887#p16394966
         self._lock: bool = False
         self._set_user_agent(
             script_name, script_version, script_author, script_user, link_to_src
         )
         # If a link to the source code is provided, add it to the user agent
         self._ns_server = "1"
-        # Make sure the nations in the user agent actually exist
-        if not self._validate_nations([script_author, script_user]):
-            raise ValueError(
-                "One of, or both, of the nations in the user agent do not exist. Make sure you're only including the nation name in the constructor, e.g. 'Thorn1000' instead of 'Devved by Thorn1000'"
-            )
         # Initialize nationstates specific stuff
         self._auth_region = "rwby"
         self.chk: str = ""
         self.localid: str = ""
         self.pin: str = ""
         self.nation: str = ""
         self.region: str = ""
         self.api_pin: str = ""
         self.current_page: tuple[str, str] = ("", "")
         self.keybind = keybind
+        # Make sure the nations in the user agent actually exist
+        if not self._validate_nations([script_author, script_user]):
+            raise ValueError(
+                "One of, or both, of the nations in the user agent do not exist. Make sure you're only including the nation name in the constructor, e.g. 'Thorn1000' instead of 'Devved by Thorn1000'"
+            )
         self.logger.info(f"Initialized. Keybind to continue is {self.keybind}.")
 
     def _set_user_agent(
         self,
         script_name: str,
         script_version: str,
         script_author: str,
```

### Comparing `nsdotpy-1.3.3/nsdotpy/valid.py` & `nsdotpy-1.3.4/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.3/pyproject.toml` & `nsdotpy-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.3.3"
+version = "1.3.4"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.3.3/PKG-INFO` & `nsdotpy-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

