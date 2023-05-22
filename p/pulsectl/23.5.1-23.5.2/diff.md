# Comparing `tmp/pulsectl-23.5.1.tar.gz` & `tmp/pulsectl-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-23.5.1.tar", last modified: Sat May  6 17:34:26 2023, max compression
+gzip compressed data, was "pulsectl-23.5.2.tar", last modified: Mon May 22 20:49:27 2023, max compression
```

## Comparing `pulsectl-23.5.1.tar` & `pulsectl-23.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 17:34:26.667192 pulsectl-23.5.1/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2022-03-23 05:40:50.000000 pulsectl-23.5.1/CHANGES.rst
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-23.5.1/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-23.5.1/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-06 17:34:26.667192 pulsectl-23.5.1/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16561 2023-05-05 23:05:28.000000 pulsectl-23.5.1/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 17:34:26.667192 pulsectl-23.5.1/pulsectl/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-23.5.1/pulsectl/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22571 2023-05-06 17:30:48.000000 pulsectl-23.5.1/pulsectl/_pulsectl.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-23.5.1/pulsectl/lookup.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41085 2023-05-05 23:00:23.000000 pulsectl-23.5.1/pulsectl/pulsectl.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 17:34:26.667192 pulsectl-23.5.1/pulsectl/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-23.5.1/pulsectl/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-04-09 14:42:09.000000 pulsectl-23.5.1/pulsectl/tests/test_with_dummy_instance.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-06 17:34:26.667192 pulsectl-23.5.1/pulsectl.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-06 17:34:26.000000 pulsectl-23.5.1/pulsectl.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2023-05-06 17:34:26.000000 pulsectl-23.5.1/pulsectl.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-06 17:34:26.000000 pulsectl-23.5.1/pulsectl.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2023-05-06 17:34:26.000000 pulsectl-23.5.1/pulsectl.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2023-05-06 17:34:26.668192 pulsectl-23.5.1/setup.cfg
--rw-------   0 fraggod   (1000) fraggod   (1000)     1247 2023-05-06 17:31:32.000000 pulsectl-23.5.1/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.479202 pulsectl-23.5.2/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2023-05-22 20:48:38.000000 pulsectl-23.5.2/CHANGES.rst
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-23.5.2/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-23.5.2/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-22 20:49:27.479202 pulsectl-23.5.2/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16561 2023-05-05 23:05:28.000000 pulsectl-23.5.2/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.478202 pulsectl-23.5.2/pulsectl/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-23.5.2/pulsectl/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22570 2023-05-22 20:45:39.000000 pulsectl-23.5.2/pulsectl/_pulsectl.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-23.5.2/pulsectl/lookup.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41085 2023-05-05 23:00:23.000000 pulsectl-23.5.2/pulsectl/pulsectl.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.479202 pulsectl-23.5.2/pulsectl/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-23.5.2/pulsectl/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-04-09 14:42:09.000000 pulsectl-23.5.2/pulsectl/tests/test_with_dummy_instance.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-22 20:49:27.478202 pulsectl-23.5.2/pulsectl.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2023-05-22 20:49:27.000000 pulsectl-23.5.2/pulsectl.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2023-05-22 20:49:27.479202 pulsectl-23.5.2/setup.cfg
+-rw-------   0 fraggod   (1000) fraggod   (1000)     1247 2023-05-22 20:48:14.000000 pulsectl-23.5.2/setup.py
```

### Comparing `pulsectl-23.5.1/CHANGES.rst` & `pulsectl-23.5.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Only (unlikely) intentional breaking changes and new/added non-trivial
 functionality is listed here, no bugfixes or commit messages.
 
 Each entry is a package version which change first appears in,
 followed by description of the change itself.
 
-Last synced/updated: 22.3.2
+Last synced/updated: 23.5.2
 
 ---------------------------------------------------------------------------
 
 - 21.10.4: Add channel_list_enum to compare channel_list values with something
   in a typo-free way, expose channel_list_raw with C enum values [#66].
 
 - 21.5.0: Fix PA_VOLUME_MAX and PA_VOLUME_UI_MAX values, both were incorrect [#53].
```

### Comparing `pulsectl-23.5.1/COPYING` & `pulsectl-23.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/PKG-INFO` & `pulsectl-23.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 23.5.1
+Version: 23.5.2
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulsectl-23.5.1/README.rst` & `pulsectl-23.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/pulsectl/__init__.py` & `pulsectl-23.5.2/pulsectl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/pulsectl/_pulsectl.py` & `pulsectl-23.5.2/pulsectl/_pulsectl.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
 class PA_IO_EVENT(Structure): pass
 
 
 class PA_SAMPLE_SPEC(Structure):
 	_fields_ = [
 		('format', c_int),
 		('rate', c_uint32),
-		('channels', c_uint32)
+		('channels', c_uint8)
 	]
 
 class PA_CHANNEL_MAP(Structure):
 	_fields_ = [
 		('channels', c_uint8),
 		('map', c_int * PA_CHANNELS_MAX)
 	]
```

### Comparing `pulsectl-23.5.1/pulsectl/lookup.py` & `pulsectl-23.5.2/pulsectl/lookup.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/pulsectl/pulsectl.py` & `pulsectl-23.5.2/pulsectl/pulsectl.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/pulsectl/tests/test_with_dummy_instance.py` & `pulsectl-23.5.2/pulsectl/tests/test_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-23.5.1/pulsectl.egg-info/PKG-INFO` & `pulsectl-23.5.2/pulsectl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 23.5.1
+Version: 23.5.2
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulsectl-23.5.1/setup.py` & `pulsectl-23.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	readme = open(os.path.join(
 		os.path.dirname(__file__), 'README.rst' )).read()
 except IOError: readme = ''
 
 setup(
 
 	name = 'pulsectl',
-	version = '23.5.1',
+	version = '23.5.2',
 	author = 'George Filipkin, Mike Kazantsev',
 	author_email = 'mk.fraggod@gmail.com',
 	license = 'MIT',
 	keywords = [
 		'pulseaudio', 'libpulse', 'pulse', 'pa', 'bindings',
 		'sound', 'audio',
 		'ctypes', 'control', 'mixer', 'volume', 'mute', 'source', 'sink' ],
```

