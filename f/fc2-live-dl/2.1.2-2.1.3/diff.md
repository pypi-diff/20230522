# Comparing `tmp/fc2-live-dl-2.1.2.tar.gz` & `tmp/fc2-live-dl-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc2-live-dl-2.1.2.tar", last modified: Wed Apr  5 15:16:22 2023, max compression
+gzip compressed data, was "fc2-live-dl-2.1.3.tar", last modified: Mon May 22 02:59:43 2023, max compression
```

## Comparing `fc2-live-dl-2.1.2.tar` & `fc2-live-dl-2.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-04-05 15:16:22.110037 fc2-live-dl-2.1.2/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     1064 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/LICENSE
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-04-05 15:16:22.110037 fc2-live-dl-2.1.2/PKG-INFO
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     9890 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/README.md
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-04-05 15:16:22.110037 fc2-live-dl-2.1.2/fc2_live_dl/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    14915 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/FC2LiveDL.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     6125 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/__init__.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       58 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/__main__.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4160 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/autofc2.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10405 2023-04-04 06:42:28.000000 fc2-live-dl-2.1.2/fc2_live_dl/fc2.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     2249 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/ffmpeg.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     5448 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/hls.py
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4357 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/fc2_live_dl/util.py
-drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-04-05 15:16:22.110037 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/PKG-INFO
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      446 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/SOURCES.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)        1 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/dependency_links.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       84 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/entry_points.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       29 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/requires.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)       12 2023-04-05 15:16:22.000000 fc2-live-dl-2.1.2/fc2_live_dl.egg-info/top_level.txt
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      104 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.2/pyproject.toml
--rw-r--r--   0 kitsune   (1000) kitsune   (1000)      947 2023-04-05 15:16:22.110037 fc2-live-dl-2.1.2/setup.cfg
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     1064 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/LICENSE
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/PKG-INFO
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     9890 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/README.md
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/fc2_live_dl/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    15362 2023-05-22 02:52:09.000000 fc2-live-dl-2.1.3/fc2_live_dl/FC2LiveDL.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     6125 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/__init__.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       58 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/__main__.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4160 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/autofc2.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10405 2023-04-04 06:42:28.000000 fc2-live-dl-2.1.3/fc2_live_dl/fc2.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     2751 2023-05-22 02:52:39.000000 fc2-live-dl-2.1.3/fc2_live_dl/ffmpeg.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     5448 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/hls.py
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)     4357 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/fc2_live_dl/util.py
+drwxr-xr-x   0 kitsune   (1000) kitsune   (1000)        0 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)    10594 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/PKG-INFO
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      446 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)        1 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       84 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/entry_points.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       29 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/requires.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)       12 2023-05-22 02:59:43.000000 fc2-live-dl-2.1.3/fc2_live_dl.egg-info/top_level.txt
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      104 2023-03-05 12:06:34.000000 fc2-live-dl-2.1.3/pyproject.toml
+-rw-r--r--   0 kitsune   (1000) kitsune   (1000)      947 2023-05-22 02:59:43.361342 fc2-live-dl-2.1.3/setup.cfg
```

### Comparing `fc2-live-dl-2.1.2/LICENSE` & `fc2-live-dl-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/PKG-INFO` & `fc2-live-dl-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc2-live-dl
-Version: 2.1.2
+Version: 2.1.3
 Summary: Download live streams from FC2
 Home-page: https://github.com/HoloArchivists/fc2-live-dl
 Author: Hizkia Felix
 Author-email: felix@hizkifw.me
 Project-URL: Bug Tracker, https://github.com/HoloArchivists/fc2-live-dl/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `fc2-live-dl-2.1.2/README.md` & `fc2-live-dl-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/FC2LiveDL.py` & `fc2-live-dl-2.1.3/fc2_live_dl/FC2LiveDL.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,26 @@
         # Sleep for 250ms to allow SSL connections to close.
         # See: https://github.com/aio-libs/aiohttp/issues/1925
         # See: https://github.com/aio-libs/aiohttp/issues/4324
         await asyncio.sleep(0.250)
         self._session = None
 
     async def download(self, channel_id):
+        # Check ffmpeg
+        if not await FFMpeg.is_available():
+            if self.params["remux"]:
+                self._logger.error(
+                    "ffmpeg not found in PATH, remuxing is not available"
+                )
+                self._logger.error(
+                    "please install ffmpeg or disable remuxing with --no-remux"
+                )
+                raise FileNotFoundError(FFMpeg.FFMPEG_BIN)
+
+        # Initialize
         self._logger = Logger("fc2 " + channel_id)
         tasks = []
         fname_stream = None
         try:
             live = FC2LiveStream(self._session, channel_id)
 
             self._logger.info("Fetching stream info")
```

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/__init__.py` & `fc2-live-dl-2.1.3/fc2_live_dl/__init__.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/autofc2.py` & `fc2-live-dl-2.1.3/fc2_live_dl/autofc2.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/fc2.py` & `fc2-live-dl-2.1.3/fc2_live_dl/fc2.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/ffmpeg.py` & `fc2-live-dl-2.1.3/fc2_live_dl/ffmpeg.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,32 @@
     FFMPEG_BIN = "ffmpeg"
 
     def __init__(self, flags):
         self._logger = Logger("ffmpeg")
         self._ffmpeg = None
         self._flags = flags
 
+    @classmethod
+    async def is_available(cls):
+        """
+        Check if ffmpeg binary exists and is executable.
+        """
+
+        try:
+            proc = await asyncio.create_subprocess_exec(
+                cls.FFMPEG_BIN,
+                "-version",
+                stdout=asyncio.subprocess.DEVNULL,
+                stderr=asyncio.subprocess.DEVNULL,
+            )
+            ret = await proc.wait()
+            return ret == 0
+        except FileNotFoundError:
+            return False
+
     async def __aenter__(self):
         self._loop = asyncio.get_running_loop()
         self._ffmpeg = await asyncio.create_subprocess_exec(
             self.FFMPEG_BIN,
             *self._flags,
             stdout=asyncio.subprocess.DEVNULL,
             stderr=asyncio.subprocess.PIPE,
```

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/hls.py` & `fc2-live-dl-2.1.3/fc2_live_dl/hls.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl/util.py` & `fc2-live-dl-2.1.3/fc2_live_dl/util.py`

 * *Files identical despite different names*

### Comparing `fc2-live-dl-2.1.2/fc2_live_dl.egg-info/PKG-INFO` & `fc2-live-dl-2.1.3/fc2_live_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc2-live-dl
-Version: 2.1.2
+Version: 2.1.3
 Summary: Download live streams from FC2
 Home-page: https://github.com/HoloArchivists/fc2-live-dl
 Author: Hizkia Felix
 Author-email: felix@hizkifw.me
 Project-URL: Bug Tracker, https://github.com/HoloArchivists/fc2-live-dl/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `fc2-live-dl-2.1.2/setup.cfg` & `fc2-live-dl-2.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fc2-live-dl
-version = 2.1.2
+version = 2.1.3
 author = Hizkia Felix
 author_email = felix@hizkifw.me
 description = Download live streams from FC2
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HoloArchivists/fc2-live-dl
 project_urls =
```

