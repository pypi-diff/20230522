# Comparing `tmp/seaplayer-0.4a3.tar.gz` & `tmp/seaplayer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.4a3.tar", max compression
+gzip compressed data, was "seaplayer-0.5.0.tar", max compression
```

## Comparing `seaplayer-0.4a3.tar` & `seaplayer-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,45 @@
--rw-r--r--   0        0        0     1085 2023-04-25 14:05:19.406661 seaplayer-0.4a3/LICENSE
--rw-r--r--   0        0        0     1020 2023-05-19 19:33:28.838346 seaplayer-0.4a3/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-05-18 14:07:36.121280 seaplayer-0.4a3/README.md
--rw-r--r--   0        0        0        0 2023-05-02 23:42:08.763410 seaplayer-0.4a3/seaplayer/__init__.py
--rw-r--r--   0        0        0      295 2023-05-17 19:11:05.795693 seaplayer-0.4a3/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-10 21:24:30.252393 seaplayer-0.4a3/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     4485 2023-05-18 16:45:40.489905 seaplayer-0.4a3/seaplayer/codecs.py
--rw-r--r--   0        0        0     1855 2023-05-18 18:50:26.106124 seaplayer-0.4a3/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     5851 2023-05-18 20:05:55.893843 seaplayer-0.4a3/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-03 15:09:20.919585 seaplayer-0.4a3/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1447 2023-05-19 19:05:56.985432 seaplayer-0.4a3/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-19 18:52:39.760564 seaplayer-0.4a3/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-02 23:29:23.509840 seaplayer-0.4a3/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-19 19:34:40.039165 seaplayer-0.4a3/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1278 2023-05-19 19:35:29.716179 seaplayer-0.4a3/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-02 22:35:56.414811 seaplayer-0.4a3/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-12 20:40:27.939248 seaplayer-0.4a3/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0    13356 2023-05-19 19:02:05.310349 seaplayer-0.4a3/seaplayer/objects.py
--rw-r--r--   0        0        0     6778 2023-05-19 19:45:06.250790 seaplayer-0.4a3/seaplayer/screens.py
--rw-r--r--   0        0        0    17707 2023-05-19 19:30:43.886684 seaplayer-0.4a3/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     4159 2023-05-18 12:58:01.336447 seaplayer-0.4a3/seaplayer/types.py
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 seaplayer-0.4a3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-22 09:27:56.937522 seaplayer-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-22 09:27:56.937522 seaplayer-0.5.0/README.md
+-rw-r--r--   0        0        0     1445 2023-05-22 12:14:42.150487 seaplayer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0     2351 2023-05-22 09:27:56.937522 seaplayer-0.5.0/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      459 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2732 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      455 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      457 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      574 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0      134 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     1859 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     5700 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1491 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      555 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      260 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      374 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1367 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      868 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     2938 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1094 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0      950 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5430 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      759 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1240 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0      316 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-22 09:37:07.994732 seaplayer-0.5.0/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      547 2023-05-22 11:43:33.516175 seaplayer-0.5.0/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      730 2023-05-22 11:43:57.779447 seaplayer-0.5.0/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     6978 2023-05-22 11:53:22.805667 seaplayer-0.5.0/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2100 2023-05-22 11:41:34.889889 seaplayer-0.5.0/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0     5729 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0      982 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0       83 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0    19012 2023-05-22 12:12:29.419425 seaplayer-0.5.0/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0     2547 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1553 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0       63 2023-05-22 09:27:56.940856 seaplayer-0.5.0/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1402 2023-05-22 12:14:15.214859 seaplayer-0.5.0/seaplayer/units.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 seaplayer-0.5.0/PKG-INFO
```

### Comparing `seaplayer-0.4a3/LICENSE` & `seaplayer-0.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Romanin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Romanin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `seaplayer-0.4a3/pyproject.toml` & `seaplayer-0.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-[tool.poetry]
-name = "SeaPlayer"
-version = "0.4a3"
-description = "SeaPlayer is a player that works in the terminal."
-repository = "https://github.com/romanin-rf/SeaPlayer"
-authors = ["Romanin <semina054@gmail.com>"]
-keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
-license = "MIT"
-readme = "README.md"
-packages = [{ include = "seaplayer" }]
-include = [
-    "seaplayer/modules/__init__.py",
-    "seaplayer/modules/colorizer.py",
-    "seaplayer/assets/image-not-found.png",
-    "seaplayer/css/configurate.css",
-    "seaplayer/css/objects.css",
-    "seaplayer/css/seaplayer.css",
-    "seaplayer/css/unknown.css"
-]
-
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pillow = "^9.5.0"
-aiofiles = "^23.1.0"
-rich = ">=13.3.5"
-mutagen = "1.45.1"
-textual = ">=0.24.1"
-playsoundsimple-py = "0.6.3"
-properties-py = "1.1.0"
-typing-inspect = "^0.8.0"
-ripix = ">=2.2.3"
-platformdirs = "^3.5.1"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "SeaPlayer"
+version = "0.5.0"
+description = "SeaPlayer is a player that works in the terminal."
+repository = "https://github.com/romanin-rf/SeaPlayer"
+authors = ["Romanin <semina054@gmail.com>"]
+keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
+license = "MIT"
+readme = "README.md"
+classifiers = [
+    "Environment :: Console",
+    "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Operating System :: Microsoft :: Windows :: Windows 11",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
+]
+packages = [{ include = "seaplayer" }]
+include = [
+    "seaplayer/modules/__init__.py",
+    "seaplayer/modules/colorizer.py",
+    "seaplayer/assets/image-not-found.png",
+    "seaplayer/css/configurate.css",
+    "seaplayer/css/objects.css",
+    "seaplayer/css/seaplayer.css",
+    "seaplayer/css/unknown.css"
+]
+
+[tool.poetry.scripts]
+seaplayer = "seaplayer.__main__:run"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+pillow = "^9.5.0"
+aiofiles = "^23.1.0"
+rich = ">=13.3.5"
+mutagen = "1.45.1"
+textual = ">=0.25.0"
+playsoundsimple-py = "0.7.0"
+properties-py = "1.1.0"
+typing-inspect = "^0.8.0"
+ripix = ">=2.2.3"
+platformdirs = "^3.5.1"
+pydantic = "^1.10.7"
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `seaplayer-0.4a3/README.md` & `seaplayer-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-<div id="header" align="center">
-    <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
-</div>
-<div id="header" align="center"><h1>SeaPlayer</h1></div>
-
-## Descriptions
-SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` files.
-
-## Install
-
-
-1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
-2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
-3.  ```
-    pip install --upgrade seaplayer
-    ```
-
-### For MIDI playback
-***If you have Windows*** you can skip this part as ***Windows*** has a default decoder for `MIDI` and ***does not need to be installed***.
-
-
-***For Linux or MacOS users:***
-
-You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
-
-## Using
-```shell
-python -m seaplayer # Method for `downloaded repository` or `installed via pip`
-```
-![MainScreen-v0.4a1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/c0fb3ad6-53ac-4360-b7dc-dd96a1d5a5ea)
-![ConfigurateScreen-v0.4a1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/6e2dcded-8ffb-4f05-8dd8-26d5951cd89b)
+<div id="header" align="center">
+    <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
+</div>
+<div id="header" align="center"><h1>SeaPlayer</h1></div>
+
+## Descriptions
+SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` and `FLAC` files.
+
+## Install
+
+
+1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
+2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
+3.  ```
+    pip install --upgrade seaplayer
+    ```
+
+### For MIDI playback
+***If you have Windows*** you can skip this part as ***Windows*** has a default decoder for `MIDI` and ***does not need to be installed***.
+
+
+***For Linux or MacOS users:***
+
+You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
+
+## Using
+```shell
+python -m seaplayer # Method for `downloaded repository` or `installed via pip`
+```
+
+![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
+![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
```

### Comparing `seaplayer-0.4a3/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.0/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.4a3/seaplayer/codeсbase.py` & `seaplayer-0.5.0/seaplayer/codeсbase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,65 @@
-from typing import Optional
-
-# ! Functions
-def formater(**kwargs) -> str:
-    return ", ".join([f"{key}={repr(value)}" for key, value in kwargs.items()])
-
-# ! Codecs Base
-class CodecBase:
-    # * Codec Info
-    codec_name: str = "None"
-    
-    # * Info
-    name: str
-    duration: float
-    channels: int
-    samplerate: int
-    bitrate: int
-    
-    # * Sound Info
-    title: Optional[str]
-    artist: Optional[str]
-    album: Optional[str]
-    icon_data: Optional[bytes]
-    
-    # * Playback Info
-    playing: bool
-    paused: bool
-    
-    # ! Initializing Functions
-    def __init__(self, path: str, **kwargs) -> None: ...
-    def __repr__(self):
-        return \
-            "{0}({1})".format(
-                self.__class__.__name__,
-                formater(
-                    name=self.name,
-                    duration=self.duration,
-                    channels=self.channels,
-                    samplerate=self.samplerate,
-                    bitrate=self.bitrate,
-                    title=self.title,
-                    artist=self.artist,
-                    album=self.album
-                )
-            )
-    
-    def __sha1__(self, buffer_size: int) -> str: ...
-    async def __aio_sha1__(self, buffer_size: int) -> str: ...
-    
-    # ! Testing Functions
-    @staticmethod
-    def is_this_codec(path: str) -> bool: return False
-    @staticmethod
-    async def aio_is_this_codec(path: str) -> bool: return False
-    
-    # ! Playback Functions
-    def play(self) -> None: ...
-    def stop(self) -> None: ...
-    def pause(self) -> None: ...
-    def unpause(self) -> None: ...
-    def get_volume(self) -> float: return 1.0
-    def set_volume(self, value: float) -> None: ...
-    def get_pos(self) -> float: return 0.0
-    def set_pos(self, value: float) -> None: ...
+from typing import Optional
+
+# ! Functions
+def formater(**kwargs) -> str:
+    return ", ".join([f"{key}={repr(value)}" for key, value in kwargs.items()])
+
+# ! Codecs Base
+class CodecBase:
+    # * Codec Info
+    codec_name: str = "None"
+    
+    # * Info
+    name: str
+    duration: float
+    channels: int
+    samplerate: int
+    bitrate: int
+    
+    # * Sound Info
+    title: Optional[str]
+    artist: Optional[str]
+    album: Optional[str]
+    icon_data: Optional[bytes]
+    
+    # * Playback Info
+    playing: bool
+    paused: bool
+    
+    # ! Initializing Functions
+    def __init__(self, path: str, **kwargs) -> None: ...
+    #async def __aio_init__(self, path: str, **kwargs) -> None: ...
+    def __repr__(self):
+        return \
+            "{0}({1})".format(
+                self.__class__.__name__,
+                formater(
+                    name=self.name,
+                    duration=self.duration,
+                    channels=self.channels,
+                    samplerate=self.samplerate,
+                    bitrate=self.bitrate,
+                    title=self.title,
+                    artist=self.artist,
+                    album=self.album
+                )
+            )
+    
+    def __sha1__(self, buffer_size: int) -> str: ...
+    async def __aio_sha1__(self, buffer_size: int) -> str: ...
+    
+    # ! Testing Functions
+    @staticmethod
+    def is_this_codec(path: str) -> bool: return False
+    @staticmethod
+    async def aio_is_this_codec(path: str) -> bool: return False
+    
+    # ! Playback Functions
+    def play(self) -> None: ...
+    def stop(self) -> None: ...
+    def pause(self) -> None: ...
+    def unpause(self) -> None: ...
+    def get_volume(self) -> float: return 1.0
+    def set_volume(self, value: float) -> None: ...
+    def get_pos(self) -> float: return 0.0
+    def set_pos(self, value: float) -> None: ...
```

### Comparing `seaplayer-0.4a3/seaplayer/config.py` & `seaplayer-0.5.0/seaplayer/config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-import properties
-from pathlib import Path
-from typing import Dict, Any, Optional, TypeVar, Union, Literal
-
-T = TypeVar("T")
-
-DEFAULT_CONFIG_DATA = {
-    "sound": {
-        "sound_font_path": None,                # * Optional[str]
-    },
-    "image": {
-        "image_update_method": "sync",          # * Literal["sync", "async"]
-        "image_resample_method": "bilinear",    # * Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]
-    },
-    "playback": {
-        "volume_change_percent": 0.05,
-        "rewind_count_seconds": 5,
-        "max_volume_percent": 2.0
-    },
-    "playlist": {
-        "recursive_search": False
-    },
-    "keys": {
-        "quit": "q,й",
-        "rewind_forward": "*",
-        "rewind_back": "/",
-        "volume_up": "+",
-        "volume_down": "-"
-    },
-    "debag": {
-        "log_menu_enable": False
-    }
-}
-
-class SeaPlayerConfig:
-    @staticmethod
-    def dump(filepath: Path, data: Dict[str, Any]) -> None:
-        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
-            properties.dump_tree(data, file)
-    
-    @staticmethod
-    def load(filepath: Path, default: Dict[str, Any]) -> Dict[str, Any]:
-        with open(filepath, "r", encoding="utf-8", errors="ignore") as file:
-            try: return properties.load_tree(file)
-            except: pass
-        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
-            properties.dump_tree(default, file)
-        return default
-    
-    def refresh(self) -> None: self.dump(self.filepath, self.config)
-    
-    def __init__(
-        self,
-        filepath: str,
-        *,
-        default_data: Dict[str, Any]=DEFAULT_CONFIG_DATA
-    ) -> None:
-        self.filepath = Path(filepath)
-        self.default_data = default_data
-        if self.filepath.exists():
-            self.config = self.load(self.filepath, self.default_data)
-            config_temp = self.default_data.copy()
-            config_temp.update(self.config)
-            self.config = config_temp.copy()
-            del config_temp
-        else:
-            self.config = default_data.copy()
-        self.refresh()
-    
-    @staticmethod
-    def tevey(key_path: str, *, sep: str=".") -> str:
-        return "".join([f"[{repr(key)}]" for key in key_path.split(sep)])
-    def get(self, key: str, default: T=None) -> Union[Any, T]:
-        try: return eval(f"self.config{self.tevey(key)}")
-        except: return default
-    def set(self, key: str, value: Any) -> None:
-        try: exec(f"self.config{self.tevey(key)} = value") ; self.refresh()
-        except: pass
-    
-    # ! Sound
-    @property
-    def sound_font_path(self) -> Optional[str]: return self.get("sound.sound_font_path")
-    @sound_font_path.setter
-    def sound_font_path(self, value: Optional[str]): self.set("sound.sound_font_path", value)
-    
-    # ! Image
-    @property
-    def image_update_method(self) -> Literal["sync", "async"]: return self.get("image.image_update_method")
-    @image_update_method.setter
-    def image_update_method(self, value: Literal["sync", "async"]): self.set("image.image_update_method", value)
-    
-    @property
-    def image_resample_method(self) -> Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]:
-        return self.get("image.image_resample_method")
-    @image_resample_method.setter
-    def image_resample_method(self, value: Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]):
-        self.set("image.image_resample_method", value)
-    
-    # ! Playback
-    @property
-    def volume_change_percent(self) -> float: return self.get("playback.volume_change_percent")
-    @volume_change_percent.setter
-    def volume_change_percent(self, value: float): self.set("playback.volume_change_percent", value)
-    
-    @property
-    def rewind_count_seconds(self) -> int: return self.get("playback.rewind_count_seconds")
-    @rewind_count_seconds.setter
-    def rewind_count_seconds(self, value: int): self.set("playback.rewind_count_seconds", value)
-    
-    @property
-    def max_volume_percent(self) -> float: return self.get("playback.max_volume_percent")
-    @max_volume_percent.setter
-    def max_volume_percent(self, value: float): self.set("playback.max_volume_percent", value)
-    
-    # ! Playlist
-    @property
-    def recursive_search(self) -> bool: return self.get("playlist.recursive_search")
-    @recursive_search.setter
-    def recursive_search(self, value: bool): self.set("playlist.recursive_search", value)
-    
-    # ! Keys
-    @property
-    def key_quit(self) -> str: return self.get("keys.quit")
-    @key_quit.setter
-    def key_quit(self, value: str): self.set("keys.quit", value)
-    
-    @property
-    def key_rewind_forward(self) -> str: return self.get("keys.rewind_forward")
-    @key_rewind_forward.setter
-    def key_rewind_forward(self, value: str): self.set("keys.rewind_forward", value)
-    
-    @property
-    def key_rewind_back(self) -> str: return self.get("keys.rewind_back")
-    @key_rewind_back.setter
-    def key_rewind_back(self, value: str): self.set("keys.rewind_back", value)
-    
-    @property
-    def key_volume_up(self) -> str: return self.get("keys.volume_up")
-    @key_volume_up.setter
-    def key_volume_up(self, value: str): self.set("keys.volume_up", value)
-    
-    @property
-    def key_volume_down(self) -> str: return self.get("keys.volume_down")
-    @key_volume_down.setter
-    def key_volume_down(self, value: str): self.set("keys.volume_down", value)
-    
-    # ! Debag
-    @property
-    def log_menu_enable(self) -> bool: return self.get("debag.log_menu_enable")
-    @log_menu_enable.setter
-    def log_menu_enable(self, value: bool): self.set("debag.log_menu_enable", value)
+import properties
+from pathlib import Path
+from typing import Dict, Any, Optional, TypeVar, Union, Literal
+
+T = TypeVar("T")
+
+DEFAULT_CONFIG_DATA = {
+    "sound": {
+        "sound_font_path": None,                # * Optional[str]
+    },
+    "image": {
+        "image_update_method": "sync",          # * Literal["sync", "async"]
+        "image_resample_method": "bilinear",    # * Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]
+    },
+    "playback": {
+        "volume_change_percent": 0.05,
+        "rewind_count_seconds": 5,
+        "max_volume_percent": 2.0
+    },
+    "playlist": {
+        "recursive_search": False
+    },
+    "keys": {
+        "quit": "q,й",
+        "rewind_forward": "*",
+        "rewind_back": "/",
+        "volume_up": "+",
+        "volume_down": "-"
+    },
+    "debag": {
+        "log_menu_enable": False
+    }
+}
+
+class SeaPlayerConfig:
+    @staticmethod
+    def dump(filepath: Path, data: Dict[str, Any]) -> None:
+        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
+            properties.dump_tree(data, file)
+    
+    @staticmethod
+    def load(filepath: Path, default: Dict[str, Any]) -> Dict[str, Any]:
+        with open(filepath, "r", encoding="utf-8", errors="ignore") as file:
+            try: return properties.load_tree(file)
+            except: pass
+        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
+            properties.dump_tree(default, file)
+        return default
+    
+    def refresh(self) -> None: self.dump(self.filepath, self.config)
+    
+    def __init__(
+        self,
+        filepath: str,
+        *,
+        default_data: Dict[str, Any]=DEFAULT_CONFIG_DATA
+    ) -> None:
+        self.filepath = Path(filepath)
+        self.default_data = default_data
+        if self.filepath.exists():
+            self.config = self.load(self.filepath, self.default_data)
+            config_temp = self.default_data.copy()
+            config_temp.update(self.config)
+            self.config = config_temp.copy()
+            del config_temp
+        else:
+            self.config = default_data.copy()
+        self.refresh()
+    
+    @staticmethod
+    def tevey(key_path: str, *, sep: str=".") -> str:
+        return "".join([f"[{repr(key)}]" for key in key_path.split(sep)])
+    def get(self, key: str, default: T=None) -> Union[Any, T]:
+        try: return eval(f"self.config{self.tevey(key)}")
+        except: return default
+    def set(self, key: str, value: Any) -> None:
+        try: exec(f"self.config{self.tevey(key)} = value") ; self.refresh()
+        except: pass
+    
+    # ! Sound
+    @property
+    def sound_font_path(self) -> Optional[str]: return self.get("sound.sound_font_path")
+    @sound_font_path.setter
+    def sound_font_path(self, value: Optional[str]): self.set("sound.sound_font_path", value)
+    
+    # ! Image
+    @property
+    def image_update_method(self) -> Literal["sync", "async"]: return self.get("image.image_update_method")
+    @image_update_method.setter
+    def image_update_method(self, value: Literal["sync", "async"]): self.set("image.image_update_method", value)
+    
+    @property
+    def image_resample_method(self) -> Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]:
+        return self.get("image.image_resample_method")
+    @image_resample_method.setter
+    def image_resample_method(self, value: Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]):
+        self.set("image.image_resample_method", value)
+    
+    # ! Playback
+    @property
+    def volume_change_percent(self) -> float: return self.get("playback.volume_change_percent")
+    @volume_change_percent.setter
+    def volume_change_percent(self, value: float): self.set("playback.volume_change_percent", value)
+    
+    @property
+    def rewind_count_seconds(self) -> int: return self.get("playback.rewind_count_seconds")
+    @rewind_count_seconds.setter
+    def rewind_count_seconds(self, value: int): self.set("playback.rewind_count_seconds", value)
+    
+    @property
+    def max_volume_percent(self) -> float: return self.get("playback.max_volume_percent")
+    @max_volume_percent.setter
+    def max_volume_percent(self, value: float): self.set("playback.max_volume_percent", value)
+    
+    # ! Playlist
+    @property
+    def recursive_search(self) -> bool: return self.get("playlist.recursive_search")
+    @recursive_search.setter
+    def recursive_search(self, value: bool): self.set("playlist.recursive_search", value)
+    
+    # ! Keys
+    @property
+    def key_quit(self) -> str: return self.get("keys.quit")
+    @key_quit.setter
+    def key_quit(self, value: str): self.set("keys.quit", value)
+    
+    @property
+    def key_rewind_forward(self) -> str: return self.get("keys.rewind_forward")
+    @key_rewind_forward.setter
+    def key_rewind_forward(self, value: str): self.set("keys.rewind_forward", value)
+    
+    @property
+    def key_rewind_back(self) -> str: return self.get("keys.rewind_back")
+    @key_rewind_back.setter
+    def key_rewind_back(self, value: str): self.set("keys.rewind_back", value)
+    
+    @property
+    def key_volume_up(self) -> str: return self.get("keys.volume_up")
+    @key_volume_up.setter
+    def key_volume_up(self, value: str): self.set("keys.volume_up", value)
+    
+    @property
+    def key_volume_down(self) -> str: return self.get("keys.volume_down")
+    @key_volume_down.setter
+    def key_volume_down(self, value: str): self.set("keys.volume_down", value)
+    
+    # ! Debag
+    @property
+    def log_menu_enable(self) -> bool: return self.get("debag.log_menu_enable")
+    @log_menu_enable.setter
+    def log_menu_enable(self, value: bool): self.set("debag.log_menu_enable", value)
```

### Comparing `seaplayer-0.4a3/seaplayer/css/objects.css` & `seaplayer-0.5.0/seaplayer/css/objects.css`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,95 @@
-/* ! Music List */
-.music-list-view {
-    height: 1fr;
-}
-
-.music-list-view-item {
-    height: 4;
-}
-
-.music-list-view-item-title-label {
-    height: 1;
-    color: #cacaca;
-}
-
-.music-list-view-item-subtitle-label {
-    height: 1;
-    color: #a9a9a9;
-}
-
-.music-list-screen-add-box {
-    height: 3;
-}
-
-.music-list-screen-add-input {
-    width: 1fr;
-}
-
-/* ! IndeterminateProgress */
-.indeterminate-progress-bar { height: 1; }
-
-/* ! Image Label */
-.image-label {
-    height: 1fr;
-    width: 1fr;
-    align: center middle;
-    text-align: center;
-}
-
-/* ! Configurate List */
-.configurate-list-view {
-    border: solid cadetblue;
-    height: 1fr;
-    width: 1fr;
-}
-
-.configurate-list-view-item {
-    border: solid dodgerblue;
-    background: #0000;
-    border-title-color: #aaaaaa;
-    border-subtitle-color: #6b6b6b;
-}
-
-/* ! Any Elements CSS */
-.pass-one-width { width: 1; }
-
-/* ! Log Menu */
-.log-menu {
-    background: $surface;
-    color: $text;
-    height: 50vh;
-    dock: bottom;
-    layer: notes;
-    border-top: hkey $primary;
-    offset-y: 0;
-    transition: offset 400ms in_out_cubic;
-    padding: 0 1 1 1;
-}
-
-.log-menu:focus {
-    offset: 0 0 !important;
-}
-
-.log-menu.-hidden {
-    offset-y: 100%;
-}
-
-Nofy {
-    dock: top;
-    layer: nofys;
-    width: auto;
-    margin: 2 4;
-    padding: 1 2;
-    background: $background;
-    color: $text;
-    height: auto;
+/* ! Music List */
+.music-list-view {
+    height: 1fr;
+}
+
+.music-list-view-item {
+    height: 4;
+}
+
+.music-list-view-item-title-label {
+    height: 1;
+    color: #cacaca;
+}
+
+.music-list-view-item-subtitle-label {
+    height: 1;
+    color: #a9a9a9;
+}
+
+.music-list-screen-add-box {
+    height: 3;
+}
+
+.music-list-screen-add-input {
+    width: 1fr;
+}
+
+/* ! IndeterminateProgress */
+.indeterminate-progress-bar { height: 1; }
+
+/* ! Image Label */
+.image-label {
+    height: 1fr;
+    width: 1fr;
+    align: center middle;
+    text-align: center;
+}
+
+/* ! Configurate List */
+.configurate-list-view {
+    border: solid cadetblue;
+    height: 1fr;
+    width: 1fr;
+}
+
+.configurate-list-view-item {
+    border: solid dodgerblue;
+    background: #0000;
+    border-title-color: #aaaaaa;
+    border-subtitle-color: #6b6b6b;
+    height: auto;
+}
+
+/* ! Any Elements CSS */
+.pass-one-width { width: 1; }
+
+/* ! Log Menu */
+.log-menu {
+    background: $surface;
+    color: $text;
+    height: 50vh;
+    dock: bottom;
+    layer: notes;
+    border-top: hkey $primary;
+    offset-y: 0;
+    transition: offset 400ms in_out_cubic;
+    padding: 0 1 1 1;
+}
+
+.log-menu:focus {
+    offset: 0 0 !important;
+}
+
+.log-menu.-hidden {
+    offset-y: 100%;
+}
+
+/* ! Nofy */
+Nofy {
+    layer: nofys;
+    background: $background;
+    margin: 2 4;
+    padding: 1 2;
+    width: auto;
+    height: auto;
+}
+
+CallNofy {
+    layer: nofys;
+    background: $background;
+    margin: 2 4;
+    padding: 1 2;
+    width: auto;
+    height: auto;
 }
```

### Comparing `seaplayer-0.4a3/seaplayer/css/seaplayer.css` & `seaplayer-0.5.0/seaplayer/css/seaplayer.css`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-/* ! Main Screen */
-#_default  {
-    layout: horizontal;
-}
-
-.screen-box {
-    border: solid cornflowerblue;
-    width: 1fr;
-    height: 100%;
-}
-
-.test-box-border {
-    border: solid cadetblue;
-}
-
-/* ! Play Screen */
-.player-visual-panel {
-    border: solid cadetblue;
-    height: 1fr;
-}
-
-.player-contol-panel {
-    border: solid cadetblue;
-    height: 7;
-}
-
-.box-buttons-sound-control {
-    height: 3;
-}
-
-.button-sound-control {
-    width: 1fr;
-}
-
-.music-selected-label {
-    width: 1fr;
-    height: 1;
-    align: center middle;
-    text-align: center;
-}
+/* ! Main Screen */
+#_default  {
+    layout: horizontal;
+}
+
+.screen-box {
+    border: solid cornflowerblue;
+    width: 1fr;
+    height: 100%;
+}
+
+.test-box-border {
+    border: solid cadetblue;
+}
+
+/* ! Play Screen */
+.player-visual-panel {
+    border: solid cadetblue;
+    height: 1fr;
+}
+
+.player-contol-panel {
+    border: solid cadetblue;
+    height: 7;
+}
+
+.box-buttons-sound-control {
+    height: 3;
+}
+
+.button-sound-control {
+    width: 1fr;
+}
+
+.music-selected-label {
+    width: 1fr;
+    height: 1;
+    align: center middle;
+    text-align: center;
+}
```

### Comparing `seaplayer-0.4a3/seaplayer/modules/colorizer.py` & `seaplayer-0.5.0/seaplayer/modules/colorizer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Dict
-from typing_inspect import (
-    is_optional_type,
-    is_union_type,
-    is_literal_type,
-    is_tuple_type,
-    get_args,
-    get_origin
-)
-
-# ! Vars
-REPLACE_TYPES = {
-    "str": "[green]str[/]",
-    "bool": "[green]bool[/]",
-    "int": "[green]int[/]",
-    "float": "[green]float[/]",
-    "bytes": "[green]bytes[/]",
-    "bytearray": "[green]bytearray[/]",
-    "complex": "[green]complex[/]",
-    "list": "[green]list[/]",
-    "tuple": "[green]tuple[/]",
-    "dict": "[green]dict[/]",
-    "None": "[cyan]None[/]",
-    "Tuple": "[green]Tuple[/]",
-    "Dict": "[green]Dict[/]",
-    "List": "[green]List[/]",
-    "Any": "[white]Any[/]",
-    "Literal": "[green]Literal[/]",
-    "['": "[[yellow]'",
-    ", '": ", [yellow]'",
-    "']": "'[/]]",
-    "', ": "'[/], "
-}
-
-# ! Other Functions
-def is_list_type(tp) -> bool: return get_origin(tp) == list
-def is_dict_type(tp) -> bool: return get_origin(tp) == dict
-def replaces(string: str, replacement: Dict[str, str]) -> str:
-    for _old, _new in replacement.items(): string = string.replace(_old, _new)
-    return string
-
-# ! Functions
-def pullyper(tp: type) -> str:
-    if tp is None: return "None"
-    elif is_optional_type(tp):
-       return f"{pullyper(get_args(tp)[0])} | None"
-    elif is_union_type(tp):
-        return " | ".join(pullyper(arg) for arg in get_args(tp))
-    elif is_literal_type(tp):
-        return f"Literal[{', '.join(repr(arg) for arg in get_args(tp))}]"
-    elif is_tuple_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"Tuple[{', '.join(pullyper(arg) for arg in args)}]"
-        return "Tuple"
-    elif is_list_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"List[{pullyper(args[0])}]"
-        return "List"
-    elif is_dict_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"Dict[{', '.join(pullyper(arg) for arg in args)}]"
-        return "Dict"
-    return tp.__name__
-
+from typing import Dict
+from typing_inspect import (
+    is_optional_type,
+    is_union_type,
+    is_literal_type,
+    is_tuple_type,
+    get_args,
+    get_origin
+)
+
+# ! Vars
+REPLACE_TYPES = {
+    "str": "[green]str[/]",
+    "bool": "[green]bool[/]",
+    "int": "[green]int[/]",
+    "float": "[green]float[/]",
+    "bytes": "[green]bytes[/]",
+    "bytearray": "[green]bytearray[/]",
+    "complex": "[green]complex[/]",
+    "list": "[green]list[/]",
+    "tuple": "[green]tuple[/]",
+    "dict": "[green]dict[/]",
+    "None": "[cyan]None[/]",
+    "Tuple": "[green]Tuple[/]",
+    "Dict": "[green]Dict[/]",
+    "List": "[green]List[/]",
+    "Any": "[white]Any[/]",
+    "Literal": "[green]Literal[/]",
+    "['": "[[yellow]'",
+    ", '": ", [yellow]'",
+    "']": "'[/]]",
+    "', ": "'[/], "
+}
+
+# ! Other Functions
+def is_list_type(tp) -> bool: return get_origin(tp) == list
+def is_dict_type(tp) -> bool: return get_origin(tp) == dict
+def replaces(string: str, replacement: Dict[str, str]) -> str:
+    for _old, _new in replacement.items(): string = string.replace(_old, _new)
+    return string
+
+# ! Functions
+def pullyper(tp: type) -> str:
+    if tp is None: return "None"
+    elif is_optional_type(tp):
+       return f"{pullyper(get_args(tp)[0])} | None"
+    elif is_union_type(tp):
+        return " | ".join(pullyper(arg) for arg in get_args(tp))
+    elif is_literal_type(tp):
+        return f"Literal[{', '.join(repr(arg) for arg in get_args(tp))}]"
+    elif is_tuple_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"Tuple[{', '.join(pullyper(arg) for arg in args)}]"
+        return "Tuple"
+    elif is_list_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"List[{pullyper(args[0])}]"
+        return "List"
+    elif is_dict_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"Dict[{', '.join(pullyper(arg) for arg in args)}]"
+        return "Dict"
+    return tp.__name__
+
 def richefication(tp: type) -> str: return replaces(pullyper(tp), REPLACE_TYPES)
```

### Comparing `seaplayer-0.4a3/seaplayer/seaplayer.py` & `seaplayer-0.5.0/seaplayer/seaplayer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,395 +1,439 @@
-import os
-import sys
-import glob
-import asyncio
-from platformdirs import user_config_dir
-# > Graphics
-from textual import on
-from textual.binding import Binding
-from textual.app import App, ComposeResult
-from textual.containers import Horizontal, Vertical
-from textual.widgets import Header, Footer, Static, Label, Button
-# > Image Works
-from PIL import Image
-from PIL.Image import Resampling
-# > Typing
-from typing import Optional, Literal, Tuple, List, Type
-# > Local Imports
-from .config import *
-from .codeсbase import CodecBase
-from .screens import Unknown, Configurate, UNKNOWN_OPEN_KEY
-from .codecs import MP3Codec, WAVECodec, OGGCodec, MIDICodec
-from .functions import (
-    aiter,
-    check_status,
-    image_from_bytes,
-    get_sound_basename
-)
-from .objects import (
-    Nofy,
-    LogMenu,
-    InputField,
-    MusicListView,
-    AsyncImageLabel,
-    MusicListViewItem,
-    StandartImageLabel,
-    IndeterminateProgress
-)
-
-# ! Metadata
-__title__ = "SeaPlayer"
-__version__ = "0.4a3"
-__author__ = "Romanin"
-__email__ = "semina054@gmail.com"
-__url__ = "https://github.com/romanin-rf/SeaPlayer"
-
-# ! Paths
-if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
-    LOCALDIR = os.path.dirname(sys.executable)
-else:
-    LOCALDIR = os.path.dirname(os.path.dirname(__file__))
-
-CSS_LOCALDIR = os.path.join(os.path.dirname(__file__), "css")
-ASSETS_DIRPATH = os.path.join(os.path.dirname(__file__), "assets")
-
-CONFIG_DIRPATH = user_config_dir(__title__, __author__, ensure_exists=True)
-CONFIG_FILEPATH = os.path.join(CONFIG_DIRPATH, "config.properties")
-
-# ! Assets Paths
-IMGPATH_IMAGE_NOT_FOUND = os.path.join(ASSETS_DIRPATH, "image-not-found.png")
-
-# ! Constants
-RESAMPLING_SAFE = {
-    "nearest": Resampling.NEAREST,
-    "bilinear": Resampling.BILINEAR,
-    "bicubic": Resampling.BICUBIC,
-    "lanczos": Resampling.LANCZOS,
-    "hamming": Resampling.HAMMING,
-    "box": Resampling.BOX
-}
-
-# ! Main Functions
-def build_bindings(config: SeaPlayerConfig):
-    yield Binding(config.key_quit, "quit", "Quit")
-    yield Binding("c,с", "push_screen('configurate')", "Configurate")
-    if config.log_menu_enable:
-        yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
-    yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
-    yield Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec")
-    yield Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%")
-    yield Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%")
-    yield Binding("ctrl+s", "screenshot", "Screenshot")
-    yield Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
-
-# ! Main
-class SeaPlayer(App):
-    # ! Textual Configuration
-    TITLE = f"{__title__} v{__version__}"
-    CSS_PATH = [
-        os.path.join(CSS_LOCALDIR, "seaplayer.css"),
-        os.path.join(CSS_LOCALDIR, "configurate.css"),
-        os.path.join(CSS_LOCALDIR, "unknown.css"),
-        os.path.join(CSS_LOCALDIR, "objects.css")
-    ]
-    SCREENS = {
-        "unknown": Unknown(id="screen_unknown"),
-        "configurate": Configurate(id="screen_configurate")
-    }
-    
-    # ! SeaPlayer Configuration
-    config = SeaPlayerConfig(CONFIG_FILEPATH)
-    max_volume_percent: float = config.max_volume_percent
-    
-    # ! Textual Keys Configuration
-    BINDINGS = list(build_bindings(config))
-    
-    # ! Template Configuration
-    currect_sound_uuid: Optional[str] = None
-    currect_sound: Optional[CodecBase] = None
-    currect_volume = 1.0
-    last_playback_status: Optional[Literal["Stoped", "Playing", "Paused"]] = None
-    playback_mode: int = 0
-    playback_mode_blocked: bool = False
-    last_paths_globalized: List[str] = []
-    started: bool = True
-    
-    # ! Codecs Configuration
-    CODECS: List[Type[CodecBase]] = [ MP3Codec, WAVECodec, OGGCodec, MIDICodec ]
-    CODECS_KWARGS: Dict[str, Any] = {"sound_font_path": config.sound_font_path}
-    
-    # ! Init Objects
-    log_menu = LogMenu(enable_logging=config.log_menu_enable, wrap=True, highlight=True, markup=True)
-    
-    # ! Log Functions
-    info = log_menu.info
-    error = log_menu.error
-    warn = log_menu.warn
-    
-    # ! Inherited Functions
-    async def action_push_screen(self, screen: str) -> None:
-        if self.SCREENS[screen].id != self.screen.id:
-            await super().action_push_screen(screen)
-    
-    # ! Functions, Workers and other...
-    def nofy(
-        self,
-        text: str,
-        life_time: float=3,
-        dosk: Literal["bottom", "left", "right", "top"]="top"
-    ) -> None:
-        self.screen.mount(Nofy(text, life_time, dosk))
-    
-    async def aio_nofy(
-        self,
-        text: str,
-        life_time: float=3,
-        dosk: Literal["bottom", "left", "right", "top"]="top"
-    ) -> None:
-        await self.screen.mount(Nofy(text, life_time, dosk))
-    
-    def gcs(self) -> Optional[CodecBase]:
-        if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
-            self.currect_sound = self.music_list_view.music_list.get(self.currect_sound_uuid)
-        return self.currect_sound
-    
-    async def aio_gcs(self):
-        if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
-            self.currect_sound = await self.music_list_view.music_list.aio_get(self.currect_sound_uuid)
-        return self.currect_sound
-
-    async def get_sound_seek(self) -> Tuple[str, Optional[float], Optional[float]]:
-        if (sound:=await self.aio_gcs()) is not None:
-            pos = sound.get_pos()
-            minutes, seconds = round(pos // 60), round(pos % 60)
-            return f"{minutes}:{str(seconds).rjust(2,'0')} | {str(round(sound.get_volume()*100)).rjust(3)}%", pos, sound.duration
-        return "0:00 |   0%", None, None
-    
-    def get_sound_selected_label_text(self) -> str:
-        if (sound:=self.gcs()) is not None:
-            return f"({check_status(sound)}): {get_sound_basename(sound)}"
-        return "<sound not selected>"
-    
-    async def aio_get_sound_selected_label_text(self) -> str:
-        if (sound:=await self.aio_gcs()) is not None:
-            return f"({check_status(sound)}): {get_sound_basename(sound)}"
-        return "<sound not selected>"
-    
-    def gpms(self, modes: Tuple[str, str, str]=("(MODE): PLAY", "(MODE): REPLAY SOUND", "(MODE): REPLAY LIST")) -> str: return modes[self.playback_mode]
-    def switch_playback_mode(self) -> None:
-        if self.playback_mode == 2: self.playback_mode = 0
-        else: self.playback_mode += 1
-    
-    async def update_loop_playback(self) -> None:
-        while self.started:
-            if (sound:=await self.aio_gcs()) is not None:
-                status = check_status(sound)
-                if (self.last_playback_status is not None) and (self.last_playback_status != status):
-                    self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
-                
-                if (status == "Stoped") and (self.last_playback_status == "Playing"):
-                    if self.playback_mode == 1:
-                        sound.play()
-                        self.info(f"Replay sound: {repr(sound)}")
-                    elif self.playback_mode == 2:
-                        if (sound:=await self.set_sound_for_playback(sound_uuid:=await self.music_list_view.aio_get_next_sound_uuid(self.currect_sound_uuid), True)) is not None:
-                            self.playback_mode_blocked = True
-                            await self.music_list_view.aio_select_list_item_from_sound_uuid(sound_uuid)
-                            sound.play()
-                            self.info(f"Playing the next sound: {repr(sound)}")
-                
-                self.last_playback_status = status
-            await asyncio.sleep(0.33)
-    
-    def compose(self) -> ComposeResult:
-        # * Other
-        self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
-        self.info(f"Source         : {__url__}")
-        self.info(f"Codecs         : {repr(self.CODECS)}")
-        self.info(f"Config Path    : {repr(self.config.filepath)}")
-        self.info(f"CSS Dirpath    : {repr(CSS_LOCALDIR)}")
-        self.info(f"Assets Dirpath : {repr(ASSETS_DIRPATH)}")
-        
-        # * Play Screen
-        self.music_play_screen = Static(classes="screen-box")
-        self.music_play_screen.border_title = "Player"
-        
-        # * Image Object Init
-        self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
-        if self.config.image_update_method == "sync":
-            self.music_image = StandartImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
-        elif self.config.image_update_method == "async":
-            self.music_image = AsyncImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
-        else:
-            raise RuntimeError("The configuration 'image_update_method' is incorrect.")
-        self.info(f"The picture from the media file is rendered using the {repr(self.config.image_update_method)} method.")
-        
-        # * Compositions Screen
-        self.music_list_screen = Static(classes="screen-box")
-        self.music_list_screen.border_title = "Playlist"
-        
-        self.music_list_view = MusicListView()
-        
-        async def _spm(input: InputField, value: Any) -> None: await self.submit_plus_sound(value)
-        self.music_list_add_input = InputField(submit=_spm, placeholder="Filepath / Search Mask", classes="music-list-screen-add-input")
-        
-        # * Adding
-        yield Header()
-        with self.music_play_screen:
-            with Vertical():
-                with Static(classes="player-visual-panel"):
-                    yield self.music_image
-                with Static(classes="player-contol-panel"):
-                    yield self.music_selected_label
-                    yield IndeterminateProgress(getfunc=self.get_sound_seek)
-                    with Horizontal(classes="box-buttons-sound-control"):
-                        yield Button("Play/Stop", id="button-play-stop", variant="warning", classes="button-sound-control")
-                        yield Static(classes="pass-one-width")
-                        yield Button("Pause/Unpause", id="button-pause-unpause", variant="success", classes="button-sound-control")
-                        yield Static(classes="pass-one-width")
-                        yield Button(self.gpms(), id="switch-playback-mode", variant="primary", classes="button-sound-control")
-        with self.music_list_screen:
-            yield self.music_list_view
-            yield self.music_list_add_input
-        if self.config.log_menu_enable:
-            yield self.log_menu
-        yield Footer()
-        
-        self.run_worker(
-            self.update_loop_playback,
-            name="PLAYBACK_CONTROLLER",
-            group="CONTROL_UPDATER-LOOP",
-            description="Control of playback modes and status updates."
-        )
-    
-    async def add_sounds_to_list(self) -> None:
-        added_oks = 0
-        async for path in aiter(self.last_paths_globalized):
-            async for codec in aiter(self.CODECS):
-                if await codec.aio_is_this_codec(path):
-                    try: sound = codec(path, **self.CODECS_KWARGS)
-                    except: sound = None
-                    if sound is not None:
-                        if not await self.music_list_view.music_list.aio_exists_sha1(sound):
-                            await self.music_list_view.aio_add_sound(sound)
-                            self.info(f"Song added: {repr(sound)}")
-                            added_oks += 1
-                            break
-            if sound is None:
-                self.error(f"The sound could not be loaded: {repr(path)}")
-        self.info(f"Added [cyan]{added_oks}[/cyan] songs!")
-        await self.aio_nofy(f"Added [cyan]{added_oks}[/cyan] songs!")
-    
-    async def currect_sound_stop(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Stoped"
-            sound.stop()
-    
-    async def currect_sound_play(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Playing"
-            sound.play()
-    
-    async def currect_sound_pause(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Paused"
-            sound.pause()
-    
-    async def currect_sound_unpause(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Playing"
-            sound.unpause()
-    
-    async def on_button_pressed(self, event: Button.Pressed) -> None:
-        if event.button.id == "switch-playback-mode":
-            self.switch_playback_mode()
-            event.button.label = self.gpms()
-    
-    @on(Button.Pressed, "#button-pause-unpause")
-    async def bp_pause_unpause(self) -> None:
-        if (sound:=await self.aio_gcs()) is not None:
-            if sound.playing:
-                if sound.paused: await self.currect_sound_unpause(sound)
-                else: await self.currect_sound_pause(sound)
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
-    
-    @on(Button.Pressed, "#button-play-stop")
-    async def bp_play_stop(self) -> None:
-        if (sound:=await self.aio_gcs()) is not None:
-            if sound.playing: await self.currect_sound_stop(sound)
-            else: await self.currect_sound_play(sound)
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
-    
-    async def submit_plus_sound(self, value: str) -> None:
-        if value.replace(" ", "") != "":
-            try: self.last_paths_globalized = glob.glob(value, recursive=self.config.recursive_search)
-            except: self.last_paths_globalized = [ value ]
-            if len(self.last_paths_globalized) > 0:
-                self.run_worker(
-                    self.add_sounds_to_list,
-                    name="ADD_SOUND",
-                    group="PLAYLIST_UPDATE",
-                    description="The process of adding sounds to a playlist."
-                )
-    
-    async def set_sound_for_playback(
-        self,
-        sound_uuid: Optional[str],
-        playback_mode_blocked: Optional[bool]=None
-    ) -> Optional[CodecBase]:
-        if playback_mode_blocked is not None:
-            self.playback_mode_blocked = playback_mode_blocked
-        if sound_uuid is not None:
-            if not self.playback_mode_blocked:
-                if (sound:=await self.aio_gcs()) is not None:
-                    self.last_playback_status = "Stoped"
-                    sound.stop()
-            self.playback_mode_blocked = False
-            
-            self.currect_sound_uuid = sound_uuid
-            if (sound:=self.music_list_view.get_sound(self.currect_sound_uuid)) is not None:
-                sound.set_volume(self.currect_volume)
-                await self.music_image.update_image(image_from_bytes(sound.icon_data))
-                self.info(f"A new sound has been selected: {repr(sound)}")
-            self.currect_sound = sound
-            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
-            return sound
-    
-    async def on_list_view_selected(self, selected: MusicListView.Selected):
-        if isinstance(selected.item, MusicListViewItem):
-            await self.set_sound_for_playback(getattr(selected.item, "sound_uuid", None))
-    
-    async def action_plus_rewind(self):
-        if (sound:=await self.aio_gcs()) is not None:
-            sound.set_pos(sound.get_pos()+self.config.rewind_count_seconds)
-    
-    async def action_minus_rewind(self):
-        if (sound:=await self.aio_gcs()) is not None:
-            sound.set_pos(sound.get_pos()-self.config.rewind_count_seconds)
-    
-    async def action_plus_volume(self) -> None:
-        if (sound:=await self.aio_gcs()) is not None:
-            if (vol:=round(sound.get_volume()+self.config.volume_change_percent, 2)) <= self.max_volume_percent:
-                self.currect_volume = vol
-                sound.set_volume(vol)
-    
-    async def action_minus_volume(self) -> None:
-        if (sound:=await self.aio_gcs()) is not None:
-            if (vol:=round(sound.get_volume()-self.config.volume_change_percent, 2)) >= 0:
-                self.currect_volume = vol
-                sound.set_volume(vol)
-    
-    async def action_screenshot(self) -> None:
-        path = self.save_screenshot(path=LOCALDIR)
-        self.info(f"Screenshot saved to: {repr(path)}")
-        await self.aio_nofy(f"Screenshot saved to: [green]{repr(path)}[/]")
-    
-    async def action_quit(self):
-        self.started = False
-        if (sound:=await self.aio_gcs()) is not None:
-            sound.unpause()
-            sound.stop()
-        return await super().action_quit()
+import os
+import glob
+import asyncio
+# > Graphics
+from textual import on
+from textual.binding import Binding
+from textual.app import App, ComposeResult
+from textual.containers import Horizontal, Vertical
+from textual.widgets import Header, Footer, Static, Label, Button
+# > Image Works
+from PIL import Image
+# > Typing
+from typing import Optional, Literal, Tuple, List, Type
+# > Local Imports
+from .config import *
+from .plug import PluginLoader
+from .codeсbase import CodecBase
+from .screens import Unknown, Configurate, UNKNOWN_OPEN_KEY
+from .codecs import MP3Codec, WAVECodec, OGGCodec, MIDICodec, FLACCodec
+from .functions import (
+    aiter,
+    check_status,
+    rich_exception,
+    image_from_bytes,
+    get_sound_basename
+)
+from .objects import (
+    Nofy,
+    LogMenu,
+    CallNofy,
+    InputField,
+    MusicListView,
+    AsyncImageLabel,
+    MusicListViewItem,
+    StandartImageLabel,
+    IndeterminateProgress
+)
+from .units import (
+    __title__,
+    __version__,
+    __author__,
+    __email__,
+    __url__,
+    CSS_LOCALDIR,
+    CONFIG_FILEPATH,
+    ASSETS_DIRPATH,
+    IMGPATH_IMAGE_NOT_FOUND,
+    RESAMPLING_SAFE,
+    LOCALDIR,
+    PLUGINS_CONFIG_PATH,
+    PLUGINS_DIRPATH
+)
+
+# ! Main Functions
+def build_bindings(config: SeaPlayerConfig):
+    yield Binding(config.key_quit, "quit", "Quit")
+    yield Binding("c,с", "push_screen('configurate')", "Configurate")
+    if config.log_menu_enable:
+        yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
+    yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
+    yield Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec")
+    yield Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%")
+    yield Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%")
+    yield Binding("ctrl+s", "screenshot", "Screenshot")
+    yield Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
+
+# ! Main
+class SeaPlayer(App):
+    # ! Textual Configuration
+    TITLE = f"{__title__} v{__version__}"
+    CSS_PATH = [
+        os.path.join(CSS_LOCALDIR, "seaplayer.css"),
+        os.path.join(CSS_LOCALDIR, "configurate.css"),
+        os.path.join(CSS_LOCALDIR, "unknown.css"),
+        os.path.join(CSS_LOCALDIR, "objects.css")
+    ]
+    SCREENS = {
+        "unknown": Unknown(id="screen_unknown"),
+        "configurate": Configurate(id="screen_configurate")
+    }
+    
+    # ! SeaPlayer Configuration
+    config = SeaPlayerConfig(CONFIG_FILEPATH)
+    max_volume_percent: float = config.max_volume_percent
+    
+    # ! Textual Keys Configuration
+    BINDINGS = list(build_bindings(config))
+    
+    # ! Template Configuration
+    currect_sound_uuid: Optional[str] = None
+    currect_sound: Optional[CodecBase] = None
+    currect_volume = 1.0
+    last_playback_status: Optional[Literal["Stoped", "Playing", "Paused"]] = None
+    playback_mode: int = 0
+    playback_mode_blocked: bool = False
+    last_paths_globalized: List[str] = []
+    started: bool = True
+    
+    # ! Codecs Configuration
+    CODECS: List[Type[CodecBase]] = [ MP3Codec, WAVECodec, OGGCodec, MIDICodec, FLACCodec ]
+    CODECS_KWARGS: Dict[str, Any] = {"sound_fonts_path": config.sound_font_path}
+    
+    # ! Init Objects
+    log_menu = LogMenu(enable_logging=config.log_menu_enable, wrap=True, highlight=True, markup=True)
+    
+    # ! Log Functions
+    info = log_menu.info
+    error = log_menu.error
+    warn = log_menu.warn
+
+    # ! App Init
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.plugin_loader = PluginLoader(self)
+        self.plugin_loader.on_init()
+    
+    # ! Inherited Functions
+    async def action_push_screen(self, screen: str) -> None:
+        if self.SCREENS[screen].id != self.screen.id:
+            await super().action_push_screen(screen)
+    
+    # ! Nofy's
+    def nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        self.screen.mount(Nofy(text, life_time, dosk))
+    
+    async def aio_nofy(
+        self,
+        text: str,
+        life_time: float=3,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> None:
+        await self.screen.mount(Nofy(text, life_time, dosk))
+    
+    def callnofy(
+        self,
+        text: str,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> CallNofy:
+        cn = CallNofy(text, dosk)
+        self.screen.mount(cn)
+        return cn
+    
+    async def aio_callnofy(
+        self,
+        text: str,
+        dosk: Literal["bottom", "left", "right", "top"]="top"
+    ) -> CallNofy:
+        cn = CallNofy(text, dosk)
+        await self.screen.mount(cn)
+        return cn
+
+    # ! Functions, Workers and other...
+    def gcs(self) -> Optional[CodecBase]:
+        if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
+            self.currect_sound = self.music_list_view.music_list.get(self.currect_sound_uuid)
+        return self.currect_sound
+    
+    async def aio_gcs(self):
+        if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
+            self.currect_sound = await self.music_list_view.music_list.aio_get(self.currect_sound_uuid)
+        return self.currect_sound
+
+    async def get_sound_seek(self) -> Tuple[str, Optional[float], Optional[float]]:
+        if (sound:=await self.aio_gcs()) is not None:
+            pos = sound.get_pos()
+            minutes, seconds = round(pos // 60), round(pos % 60)
+            return f"{minutes}:{str(seconds).rjust(2,'0')} | {str(round(sound.get_volume()*100)).rjust(3)}%", pos, sound.duration
+        return "0:00 |   0%", None, None
+    
+    def get_sound_selected_label_text(self) -> str:
+        if (sound:=self.gcs()) is not None:
+            return f"({check_status(sound)}): {get_sound_basename(sound)}"
+        return "<sound not selected>"
+    
+    async def aio_get_sound_selected_label_text(self) -> str:
+        if (sound:=await self.aio_gcs()) is not None:
+            return f"({check_status(sound)}): {get_sound_basename(sound)}"
+        return "<sound not selected>"
+    
+    def gpms(self, modes: Tuple[str, str, str]=("(MODE): PLAY", "(MODE): REPLAY SOUND", "(MODE): REPLAY LIST")) -> str: return modes[self.playback_mode]
+    def switch_playback_mode(self) -> None:
+        if self.playback_mode == 2: self.playback_mode = 0
+        else: self.playback_mode += 1
+    
+    async def update_loop_playback(self) -> None:
+        while self.started:
+            if (sound:=await self.aio_gcs()) is not None:
+                status = check_status(sound)
+                if (self.last_playback_status is not None) and (self.last_playback_status != status):
+                    self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+                
+                if (status == "Stoped") and (self.last_playback_status == "Playing"):
+                    if self.playback_mode == 1:
+                        sound.play()
+                        self.info(f"Replay sound: {repr(sound)}")
+                    elif self.playback_mode == 2:
+                        if (sound:=await self.set_sound_for_playback(sound_uuid:=await self.music_list_view.aio_get_next_sound_uuid(self.currect_sound_uuid), True)) is not None:
+                            self.playback_mode_blocked = True
+                            await self.music_list_view.aio_select_list_item_from_sound_uuid(sound_uuid)
+                            sound.play()
+                            self.info(f"Playing the next sound: {repr(sound)}")
+                
+                self.last_playback_status = status
+            await asyncio.sleep(0.2)
+    
+    def compose(self) -> ComposeResult:     
+        # * Other
+        self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
+        self.info(f"Source              : {__url__}")
+        self.info(f"Codecs              : {repr(self.CODECS)}")
+        self.info(f"Config Path         : {repr(self.config.filepath)}")
+        self.info(f"CSS Dirpath         : {repr(CSS_LOCALDIR)}")
+        self.info(f"Assets Dirpath      : {repr(ASSETS_DIRPATH)}")
+        self.info(f"Codecs Kwargs       : {repr(self.CODECS_KWARGS)}")
+        self.info(f"Plugins Dirpath     : {repr(PLUGINS_DIRPATH)}")
+        self.info(f"Plugins Config Path : {repr(PLUGINS_CONFIG_PATH)}")
+        
+        # * Play Screen
+        self.music_play_screen = Static(classes="screen-box")
+        self.music_play_screen.border_title = "Player"
+        
+        # * Image Object Init
+        self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
+        if self.config.image_update_method == "sync":
+            self.music_image = StandartImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
+        elif self.config.image_update_method == "async":
+            self.music_image = AsyncImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
+        else:
+            raise RuntimeError("The configuration 'image_update_method' is incorrect.")
+        self.info(f"The picture from the media file is rendered using the {repr(self.config.image_update_method)} method.")
+        
+        # * Compositions Screen
+        self.music_list_screen = Static(classes="screen-box")
+        self.music_list_screen.border_title = "Playlist"
+        
+        self.music_list_view = MusicListView()
+        
+        async def _spm(input: InputField, value: Any) -> None: await self.submit_plus_sound(value)
+        self.music_list_add_input = InputField(submit=_spm, placeholder="Filepath / Search Mask", classes="music-list-screen-add-input")
+        
+        # * Adding
+        yield Header()
+        with self.music_play_screen:
+            with Vertical():
+                with Static(classes="player-visual-panel"):
+                    yield self.music_image
+                with Static(classes="player-contol-panel"):
+                    yield self.music_selected_label
+                    yield IndeterminateProgress(getfunc=self.get_sound_seek)
+                    with Horizontal(classes="box-buttons-sound-control"):
+                        yield Button("Play/Stop", id="button-play-stop", variant="warning", classes="button-sound-control")
+                        yield Static(classes="pass-one-width")
+                        yield Button("Pause/Unpause", id="button-pause-unpause", variant="success", classes="button-sound-control")
+                        yield Static(classes="pass-one-width")
+                        yield Button(self.gpms(), id="switch-playback-mode", variant="primary", classes="button-sound-control")
+        with self.music_list_screen:
+            yield self.music_list_view
+            yield self.music_list_add_input
+        if self.config.log_menu_enable:
+            yield self.log_menu
+        yield Footer()
+        
+        self.run_worker(
+            self.update_loop_playback,
+            name="PLAYBACK_CONTROLLER",
+            group="CONTROL_UPDATER-LOOP",
+            description="Control of playback modes and status updates."
+        )
+        self.run_worker(
+            self.plugin_loader.on_compose,
+            name="ON_COMPOSE",
+            group="PluginLoader",
+            description="<method PluginLoader.on_compose>"
+        )
+    
+    async def add_sounds_to_list(self) -> None:
+        added_oks = 0
+        loading_nofy = await self.aio_callnofy(
+            f"Found [cyan]{len(self.last_paths_globalized)}[/cyan] values. Loading..."
+        )
+        async for path in aiter(self.last_paths_globalized):
+            sound = None
+            async for codec in aiter(self.CODECS):
+                try:
+                    if await codec.aio_is_this_codec(path):
+                        if not hasattr(codec, "__aio_init__"):
+                            try:
+                                sound = codec(path, **self.CODECS_KWARGS)
+                            except Exception as e:
+                                self.error(rich_exception(e))
+                                sound = None
+                        else:
+                            try:
+                                sound: CodecBase = await codec.__aio_init__(path, **self.CODECS_KWARGS)
+                            except Exception as e:
+                                self.error(rich_exception(e))
+                                sound = None
+                        if sound is not None:
+                            if not await self.music_list_view.music_list.aio_exists_sha1(sound):
+                                await self.music_list_view.aio_add_sound(sound)
+                                self.info(f"Song added: {repr(sound)}")
+                                added_oks += 1
+                                break
+                except FileNotFoundError:
+                    self.error(f"The file does not exist or is a directory: {repr(path)}")
+                    break
+                except Exception as e:
+                    self.error(rich_exception(e))
+            if sound is None:
+                self.error(f"The sound could not be loaded: {repr(path)}")
+        await loading_nofy.remove()
+        self.info(f"Added [cyan]{added_oks}[/cyan] songs!")
+        await self.aio_nofy(f"Added [cyan]{added_oks}[/cyan] songs!")
+    
+    async def currect_sound_stop(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Stoped"
+            sound.stop()
+    
+    async def currect_sound_play(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Playing"
+            sound.play()
+    
+    async def currect_sound_pause(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Paused"
+            sound.pause()
+    
+    async def currect_sound_unpause(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Playing"
+            sound.unpause()
+    
+    async def on_button_pressed(self, event: Button.Pressed) -> None:
+        if event.button.id == "switch-playback-mode":
+            self.switch_playback_mode()
+            event.button.label = self.gpms()
+    
+    @on(Button.Pressed, "#button-pause-unpause")
+    async def bp_pause_unpause(self) -> None:
+        if (sound:=await self.aio_gcs()) is not None:
+            if sound.playing:
+                if sound.paused: await self.currect_sound_unpause(sound)
+                else: await self.currect_sound_pause(sound)
+            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+    
+    @on(Button.Pressed, "#button-play-stop")
+    async def bp_play_stop(self) -> None:
+        if (sound:=await self.aio_gcs()) is not None:
+            if sound.playing: await self.currect_sound_stop(sound)
+            else: await self.currect_sound_play(sound)
+            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+    
+    async def submit_plus_sound(self, value: str) -> None:
+        if value.replace(" ", "") != "":
+            try: self.last_paths_globalized = glob.glob(value, recursive=self.config.recursive_search)
+            except: self.last_paths_globalized = [ value ]
+            self.info(f"Submit 'plus_sound' values: {repr(self.last_paths_globalized)}")
+            if len(self.last_paths_globalized) > 0:
+                self.run_worker(
+                    self.add_sounds_to_list,
+                    name="ADD_SOUND",
+                    group="PLAYLIST_UPDATE",
+                    description="The process of adding sounds to a playlist."
+                )
+    
+    async def set_sound_for_playback(
+        self,
+        sound_uuid: Optional[str],
+        playback_mode_blocked: Optional[bool]=None
+    ) -> Optional[CodecBase]:
+        if playback_mode_blocked is not None:
+            self.playback_mode_blocked = playback_mode_blocked
+        if sound_uuid is not None:
+            if not self.playback_mode_blocked:
+                if (sound:=await self.aio_gcs()) is not None:
+                    self.last_playback_status = "Stoped"
+                    sound.stop()
+            self.playback_mode_blocked = False
+            
+            self.currect_sound_uuid = sound_uuid
+            if (sound:=self.music_list_view.get_sound(self.currect_sound_uuid)) is not None:
+                sound.set_volume(self.currect_volume)
+                await self.music_image.update_image(image_from_bytes(sound.icon_data))
+                self.info(f"A new sound has been selected: {repr(sound)}")
+            self.currect_sound = sound
+            self.music_selected_label.update(await self.aio_get_sound_selected_label_text())
+            return sound
+    
+    async def on_list_view_selected(self, selected: MusicListView.Selected):
+        if isinstance(selected.item, MusicListViewItem):
+            await self.set_sound_for_playback(getattr(selected.item, "sound_uuid", None))
+    
+    async def action_plus_rewind(self):
+        if (sound:=await self.aio_gcs()) is not None:
+            sound.set_pos(sound.get_pos()+self.config.rewind_count_seconds)
+    
+    async def action_minus_rewind(self):
+        if (sound:=await self.aio_gcs()) is not None:
+            sound.set_pos(sound.get_pos()-self.config.rewind_count_seconds)
+    
+    async def action_plus_volume(self) -> None:
+        if (sound:=await self.aio_gcs()) is not None:
+            if (vol:=round(sound.get_volume()+self.config.volume_change_percent, 2)) <= self.max_volume_percent:
+                self.currect_volume = vol
+                sound.set_volume(vol)
+    
+    async def action_minus_volume(self) -> None:
+        if (sound:=await self.aio_gcs()) is not None:
+            if (vol:=round(sound.get_volume()-self.config.volume_change_percent, 2)) >= 0:
+                self.currect_volume = vol
+                sound.set_volume(vol)
+    
+    async def action_screenshot(self) -> None:
+        path = self.save_screenshot(path=LOCALDIR)
+        self.info(f"Screenshot saved to: {repr(path)}")
+        await self.aio_nofy(f"Screenshot saved to: [green]{repr(path)}[/]")
+    
+    async def action_quit(self):
+        self.started = False
+        if (sound:=await self.aio_gcs()) is not None:
+            sound.unpause()
+            sound.stop()
+            await self.plugin_loader.on_quit()
+        return await super().action_quit()
+
+    def run(self, *args, **kwargs):
+        self.plugin_loader.on_run()
+        super().run(*args, **kwargs)
```

### Comparing `seaplayer-0.4a3/PKG-INFO` & `seaplayer-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.4a3
+Version: 0.5.0
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: mutagen (==1.45.1)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
-Requires-Dist: playsoundsimple-py (==0.6.3)
+Requires-Dist: playsoundsimple-py (==0.7.0)
 Requires-Dist: properties-py (==1.1.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
-Requires-Dist: textual (>=0.24.1)
+Requires-Dist: textual (>=0.25.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
 
 <div id="header" align="center">
     <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
 </div>
 <div id="header" align="center"><h1>SeaPlayer</h1></div>
 
 ## Descriptions
-SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` files.
+SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` and `FLAC` files.
 
 ## Install
 
 
 1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
 2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
 3.  ```
@@ -51,10 +60,11 @@
 
 You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
 
 ## Using
 ```shell
 python -m seaplayer # Method for `downloaded repository` or `installed via pip`
 ```
-![MainScreen-v0.4a1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/c0fb3ad6-53ac-4360-b7dc-dd96a1d5a5ea)
-![ConfigurateScreen-v0.4a1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/6e2dcded-8ffb-4f05-8dd8-26d5951cd89b)
+
+![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
+![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
```

