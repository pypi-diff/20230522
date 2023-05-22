# Comparing `tmp/txt2dub-0.1.1.tar.gz` & `tmp/txt2dub-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2dub-0.1.1.tar", max compression
+gzip compressed data, was "txt2dub-0.1.2.tar", max compression
```

## Comparing `txt2dub-0.1.1.tar` & `txt2dub-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1085 2023-05-06 01:45:13.483547 txt2dub-0.1.1/LICENSE
--rw-r--r--   0        0        0      611 2023-05-19 01:48:49.871969 txt2dub-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2891 2023-05-19 01:48:49.866974 txt2dub-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-05-19 01:48:49.871969 txt2dub-0.1.1/txt2dub/__init__.py
--rw-r--r--   0        0        0       28 2023-05-18 14:24:43.461740 txt2dub-0.1.1/txt2dub/__main__.py
--rw-r--r--   0        0        0     6390 2023-05-18 14:24:43.461740 txt2dub-0.1.1/txt2dub/app.py
--rw-r--r--   0        0        0      151 2023-05-18 14:24:43.462739 txt2dub-0.1.1/txt2dub/models/__init__.py
--rw-r--r--   0        0        0      671 2023-05-18 14:24:43.463739 txt2dub-0.1.1/txt2dub/models/base.py
--rw-r--r--   0        0        0     6879 2023-05-18 14:24:43.463739 txt2dub-0.1.1/txt2dub/models/script.py
--rw-r--r--   0        0        0        0 2023-05-09 00:54:47.921658 txt2dub-0.1.1/txt2dub/screens/__init__.py
--rw-r--r--   0        0        0      265 2023-05-18 14:24:43.464738 txt2dub-0.1.1/txt2dub/screens/file/__init__.py
--rw-r--r--   0        0        0     8515 2023-05-18 14:24:43.464738 txt2dub-0.1.1/txt2dub/screens/file/screen.py
--rw-r--r--   0        0        0     1321 2023-05-18 14:24:43.465737 txt2dub-0.1.1/txt2dub/screens/file/widgets.py
--rw-r--r--   0        0        0       62 2023-05-18 14:24:43.465737 txt2dub-0.1.1/txt2dub/screens/script/__init__.py
--rw-r--r--   0        0        0     1470 2023-05-18 14:24:43.466737 txt2dub-0.1.1/txt2dub/screens/script/messages.py
--rw-r--r--   0        0        0    25548 2023-05-18 14:24:43.467736 txt2dub-0.1.1/txt2dub/screens/script/screen.py
--rw-r--r--   0        0        0    16904 2023-05-18 14:24:43.468736 txt2dub-0.1.1/txt2dub/screens/script/widgets.py
--rw-r--r--   0        0        0        0 2023-05-18 14:24:43.468736 txt2dub-0.1.1/txt2dub/services/__init__.py
--rw-r--r--   0        0        0     2076 2023-05-18 14:24:43.469737 txt2dub-0.1.1/txt2dub/services/actions.py
--rw-r--r--   0        0        0     3110 2023-05-18 14:24:43.469737 txt2dub-0.1.1/txt2dub/services/tts.py
--rw-r--r--   0        0        0     5690 2023-05-19 01:48:49.872969 txt2dub-0.1.1/txt2dub/styles/app.css
--rw-r--r--   0        0        0        0 2023-05-18 14:24:43.470737 txt2dub-0.1.1/txt2dub/tts/__init__.py
--rw-r--r--   0        0        0      104 2023-05-18 14:24:43.471736 txt2dub-0.1.1/txt2dub/tts/__main__.py
--rw-r--r--   0        0        0     4971 2023-05-18 14:24:43.471736 txt2dub-0.1.1/txt2dub/tts/interpreter.py
--rw-r--r--   0        0        0        0 2023-05-07 00:47:14.411074 txt2dub-0.1.1/txt2dub/widgets/__init__.py
--rw-r--r--   0        0        0      784 2023-05-18 14:24:43.472735 txt2dub-0.1.1/txt2dub/widgets/base.py
--rw-r--r--   0        0        0      479 2023-05-07 00:51:34.735297 txt2dub-0.1.1/txt2dub/widgets/logo.py
--rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 txt2dub-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-21 00:55:17.765711 txt2dub-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2910 2023-05-22 14:42:48.689668 txt2dub-0.1.2/README.md
+-rw-r--r--   0        0        0      756 2023-05-22 14:42:48.691341 txt2dub-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-22 14:42:48.691675 txt2dub-0.1.2/txt2dub/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-21 00:55:17.768751 txt2dub-0.1.2/txt2dub/__main__.py
+-rw-r--r--   0        0        0     6390 2023-05-21 00:55:17.768918 txt2dub-0.1.2/txt2dub/app.py
+-rw-r--r--   0        0        0      151 2023-05-21 00:55:17.769129 txt2dub-0.1.2/txt2dub/models/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-21 00:55:17.769290 txt2dub-0.1.2/txt2dub/models/base.py
+-rw-r--r--   0        0        0     6879 2023-05-21 00:55:17.769482 txt2dub-0.1.2/txt2dub/models/script.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.769639 txt2dub-0.1.2/txt2dub/screens/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-21 00:55:17.769844 txt2dub-0.1.2/txt2dub/screens/file/__init__.py
+-rw-r--r--   0        0        0     8515 2023-05-21 00:55:17.770025 txt2dub-0.1.2/txt2dub/screens/file/screen.py
+-rw-r--r--   0        0        0     1321 2023-05-21 00:55:17.770181 txt2dub-0.1.2/txt2dub/screens/file/widgets.py
+-rw-r--r--   0        0        0       62 2023-05-21 00:55:17.770388 txt2dub-0.1.2/txt2dub/screens/script/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-21 00:55:17.770540 txt2dub-0.1.2/txt2dub/screens/script/messages.py
+-rw-r--r--   0        0        0    25548 2023-05-21 00:55:17.770770 txt2dub-0.1.2/txt2dub/screens/script/screen.py
+-rw-r--r--   0        0        0    16904 2023-05-21 00:55:17.771058 txt2dub-0.1.2/txt2dub/screens/script/widgets.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.771337 txt2dub-0.1.2/txt2dub/services/__init__.py
+-rw-r--r--   0        0        0     2076 2023-05-21 00:55:17.771526 txt2dub-0.1.2/txt2dub/services/actions.py
+-rw-r--r--   0        0        0     3110 2023-05-22 14:30:51.093950 txt2dub-0.1.2/txt2dub/services/tts.py
+-rw-r--r--   0        0        0     5690 2023-05-22 14:34:52.768498 txt2dub-0.1.2/txt2dub/styles/app.css
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.772437 txt2dub-0.1.2/txt2dub/tts/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-21 00:55:17.772613 txt2dub-0.1.2/txt2dub/tts/__main__.py
+-rw-r--r--   0        0        0     5192 2023-05-22 14:42:48.692063 txt2dub-0.1.2/txt2dub/tts/interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.773094 txt2dub-0.1.2/txt2dub/widgets/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-21 00:55:17.773375 txt2dub-0.1.2/txt2dub/widgets/base.py
+-rw-r--r--   0        0        0      479 2023-05-21 00:55:17.773647 txt2dub-0.1.2/txt2dub/widgets/logo.py
+-rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 txt2dub-0.1.2/PKG-INFO
```

### Comparing `txt2dub-0.1.1/LICENSE` & `txt2dub-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/pyproject.toml` & `txt2dub-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "txt2dub"
-version = "0.1.1"
+version = "0.1.2"
 homepage = "https://github.com/NotYourDadsMath/txt2dub"
 description = "A text-based UI application for editing voiceover scripts and generating text to speech performances."
 authors = ["Mike Kibbel", "Not Your Dad's Math"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pyttsx3 = "^2.90"
-textual = "^0.25.0"
+textual = "^0.26.0"
+pyobjc = {version = "9.0.1", platform = "darwin"}
+pyttsx3 = {git = "https://github.com/skibblenybbles/pyttsx3", rev = "a83dd354bdec4c5011f6d31f887fb5638ec2d7e2"}
 
 [tool.poetry.group.dev.dependencies]
 textual-dev = "^0.0.2"
 
 [tool.poetry.scripts]
 txt2dub = "txt2dub.app:run"
```

### Comparing `txt2dub-0.1.1/README.md` & `txt2dub-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 
 `txt2dub` aims to unlock access to the text-to-speech services provided by your operating system, all wrapped in a simple application that tries to improve the workflow for voiceover script writing. It is built on top of the [Textual](https://textual.textualize.io/) rapid application development framework for text-based UIs. This makes it easy to install and run in [any supported terminal](https://textual.textualize.io/getting_started/#requirements) with Python 3.7 or later.
 
 This project doesn't require a subscription, a new account or payment. It's entirely open source, free to use, and it doesn't share your data or the content you create using it with anyone.
 
 ## Is `txt2dub` ready for production use?
 
-It has been used successfully for production work by the project's author in Windows 10. Testing on Mac will proceed in the near future. Linux testing will be community-driven. Please report issues with details about your OS (Windows, Mac, Linux + version) and Python environment (version) if you encounter bugs.
+It has been used successfully for production work by the project's author in Windows 10 and macOS Monterey. Testing on Mac will proceed in the near future. Linux testing will be community-driven. Please report issues with details about your OS (Windows, Mac, Linux + version) and Python environment (version) if you encounter bugs.
```

### Comparing `txt2dub-0.1.1/txt2dub/app.py` & `txt2dub-0.1.2/txt2dub/app.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/models/base.py` & `txt2dub-0.1.2/txt2dub/models/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/models/script.py` & `txt2dub-0.1.2/txt2dub/models/script.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/screens/file/screen.py` & `txt2dub-0.1.2/txt2dub/screens/file/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/screens/file/widgets.py` & `txt2dub-0.1.2/txt2dub/screens/file/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/screens/script/messages.py` & `txt2dub-0.1.2/txt2dub/screens/script/messages.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/screens/script/screen.py` & `txt2dub-0.1.2/txt2dub/screens/script/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/screens/script/widgets.py` & `txt2dub-0.1.2/txt2dub/screens/script/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/services/actions.py` & `txt2dub-0.1.2/txt2dub/services/actions.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/services/tts.py` & `txt2dub-0.1.2/txt2dub/services/tts.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/styles/app.css` & `txt2dub-0.1.2/txt2dub/styles/app.css`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/txt2dub/tts/interpreter.py` & `txt2dub-0.1.2/txt2dub/tts/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import pathlib
+import platform
 import signal
 import sys
 import tempfile
 import zipfile
 
 import pyttsx3
 
@@ -112,31 +113,38 @@
         self.engine.setProperty("voice", voice)
         self.engine.setProperty("rate", rate)
         self.engine.say(text)
         self.engine.runAndWait()
         return "ok"
 
     def generate(self, path, script):
+        ext = (
+            ".aiff"
+                if platform.system() == "Darwin"
+                else ".mp3")
         with zipfile.ZipFile(path, "w") as zf:
             with zf.open("lines.txt", "w") as f:
                 for n, line in enumerate(script["lines"]):
                     text = line["text"].strip()
                     f.write(f"{n:0>4d}: {text}\n".encode("utf-8"))
             with zf.open("script.txt", "w") as f:
                 for line in script["lines"]:
                     text = line["text"].strip()
                     if text:
                         f.write(f"{text}\n".encode("utf-8"))
-            with tempfile.TemporaryDirectory() as tmp:
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                batch = []
                 for n, line in enumerate(script["lines"]):
                     text = line["text"].strip()
                     if text:
-                        name = pathlib.Path(f"{n:0>4d}.mp3")
-                        tmp_path = pathlib.Path(tmp) / name
+                        name = pathlib.Path(f"{n:0>4d}{ext}")
+                        tmp = pathlib.Path(tmp_dir) / name
                         self.engine.setProperty("voice", line["voice"]["id"])
                         self.engine.setProperty("rate", line["voice"]["rate"])
-                        self.engine.save_to_file(text, f"{tmp_path}")
-                        self.engine.runAndWait()
-                        with open(tmp_path, "r+b") as t:
-                            with zf.open(f"{name}", "w") as f:
-                                f.write(t.read())
+                        self.engine.save_to_file(text, f"{tmp}")
+                        batch.append((name, tmp))
+                self.engine.runAndWait()
+                for name, tmp in batch:
+                    with open(tmp, "r+b") as t:
+                        with zf.open(f"{name}", "w") as f:
+                            f.write(t.read())
         return "ok"
```

### Comparing `txt2dub-0.1.1/txt2dub/widgets/base.py` & `txt2dub-0.1.2/txt2dub/widgets/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.1/PKG-INFO` & `txt2dub-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: txt2dub
-Version: 0.1.1
+Version: 0.1.2
 Summary: A text-based UI application for editing voiceover scripts and generating text to speech performances.
 Home-page: https://github.com/NotYourDadsMath/txt2dub
 License: MIT
 Author: Mike Kibbel
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pyttsx3 (>=2.90,<3.0)
-Requires-Dist: textual (>=0.25.0,<0.26.0)
+Requires-Dist: pyobjc (==9.0.1) ; sys_platform == "darwin"
+Requires-Dist: pyttsx3 @ git+https://github.com/skibblenybbles/pyttsx3@a83dd354bdec4c5011f6d31f887fb5638ec2d7e2
+Requires-Dist: textual (>=0.26.0,<0.27.0)
 Description-Content-Type: text/markdown
 
 txt2dub
 =======
 
 A text-based UI application for editing voiceover scripts and generating text to speech performances.
 
@@ -59,9 +60,9 @@
 
 `txt2dub` aims to unlock access to the text-to-speech services provided by your operating system, all wrapped in a simple application that tries to improve the workflow for voiceover script writing. It is built on top of the [Textual](https://textual.textualize.io/) rapid application development framework for text-based UIs. This makes it easy to install and run in [any supported terminal](https://textual.textualize.io/getting_started/#requirements) with Python 3.7 or later.
 
 This project doesn't require a subscription, a new account or payment. It's entirely open source, free to use, and it doesn't share your data or the content you create using it with anyone.
 
 ## Is `txt2dub` ready for production use?
 
-It has been used successfully for production work by the project's author in Windows 10. Testing on Mac will proceed in the near future. Linux testing will be community-driven. Please report issues with details about your OS (Windows, Mac, Linux + version) and Python environment (version) if you encounter bugs.
+It has been used successfully for production work by the project's author in Windows 10 and macOS Monterey. Testing on Mac will proceed in the near future. Linux testing will be community-driven. Please report issues with details about your OS (Windows, Mac, Linux + version) and Python environment (version) if you encounter bugs.
```

