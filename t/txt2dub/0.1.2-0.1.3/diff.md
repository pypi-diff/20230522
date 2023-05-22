# Comparing `tmp/txt2dub-0.1.2.tar.gz` & `tmp/txt2dub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2dub-0.1.2.tar", max compression
+gzip compressed data, was "txt2dub-0.1.3.tar", max compression
```

## Comparing `txt2dub-0.1.2.tar` & `txt2dub-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1085 2023-05-21 00:55:17.765711 txt2dub-0.1.2/LICENSE
--rw-r--r--   0        0        0     2910 2023-05-22 14:42:48.689668 txt2dub-0.1.2/README.md
--rw-r--r--   0        0        0      756 2023-05-22 14:42:48.691341 txt2dub-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-22 14:42:48.691675 txt2dub-0.1.2/txt2dub/__init__.py
--rw-r--r--   0        0        0       28 2023-05-21 00:55:17.768751 txt2dub-0.1.2/txt2dub/__main__.py
--rw-r--r--   0        0        0     6390 2023-05-21 00:55:17.768918 txt2dub-0.1.2/txt2dub/app.py
--rw-r--r--   0        0        0      151 2023-05-21 00:55:17.769129 txt2dub-0.1.2/txt2dub/models/__init__.py
--rw-r--r--   0        0        0      671 2023-05-21 00:55:17.769290 txt2dub-0.1.2/txt2dub/models/base.py
--rw-r--r--   0        0        0     6879 2023-05-21 00:55:17.769482 txt2dub-0.1.2/txt2dub/models/script.py
--rw-r--r--   0        0        0        0 2023-05-21 00:55:17.769639 txt2dub-0.1.2/txt2dub/screens/__init__.py
--rw-r--r--   0        0        0      265 2023-05-21 00:55:17.769844 txt2dub-0.1.2/txt2dub/screens/file/__init__.py
--rw-r--r--   0        0        0     8515 2023-05-21 00:55:17.770025 txt2dub-0.1.2/txt2dub/screens/file/screen.py
--rw-r--r--   0        0        0     1321 2023-05-21 00:55:17.770181 txt2dub-0.1.2/txt2dub/screens/file/widgets.py
--rw-r--r--   0        0        0       62 2023-05-21 00:55:17.770388 txt2dub-0.1.2/txt2dub/screens/script/__init__.py
--rw-r--r--   0        0        0     1470 2023-05-21 00:55:17.770540 txt2dub-0.1.2/txt2dub/screens/script/messages.py
--rw-r--r--   0        0        0    25548 2023-05-21 00:55:17.770770 txt2dub-0.1.2/txt2dub/screens/script/screen.py
--rw-r--r--   0        0        0    16904 2023-05-21 00:55:17.771058 txt2dub-0.1.2/txt2dub/screens/script/widgets.py
--rw-r--r--   0        0        0        0 2023-05-21 00:55:17.771337 txt2dub-0.1.2/txt2dub/services/__init__.py
--rw-r--r--   0        0        0     2076 2023-05-21 00:55:17.771526 txt2dub-0.1.2/txt2dub/services/actions.py
--rw-r--r--   0        0        0     3110 2023-05-22 14:30:51.093950 txt2dub-0.1.2/txt2dub/services/tts.py
--rw-r--r--   0        0        0     5690 2023-05-22 14:34:52.768498 txt2dub-0.1.2/txt2dub/styles/app.css
--rw-r--r--   0        0        0        0 2023-05-21 00:55:17.772437 txt2dub-0.1.2/txt2dub/tts/__init__.py
--rw-r--r--   0        0        0      104 2023-05-21 00:55:17.772613 txt2dub-0.1.2/txt2dub/tts/__main__.py
--rw-r--r--   0        0        0     5192 2023-05-22 14:42:48.692063 txt2dub-0.1.2/txt2dub/tts/interpreter.py
--rw-r--r--   0        0        0        0 2023-05-21 00:55:17.773094 txt2dub-0.1.2/txt2dub/widgets/__init__.py
--rw-r--r--   0        0        0      784 2023-05-21 00:55:17.773375 txt2dub-0.1.2/txt2dub/widgets/base.py
--rw-r--r--   0        0        0      479 2023-05-21 00:55:17.773647 txt2dub-0.1.2/txt2dub/widgets/logo.py
--rw-r--r--   0        0        0     3793 1970-01-01 00:00:00.000000 txt2dub-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-21 00:55:17.765711 txt2dub-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2910 2023-05-22 14:42:48.689668 txt2dub-0.1.3/README.md
+-rw-r--r--   0        0        0      666 2023-05-22 15:37:45.849363 txt2dub-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-22 15:37:45.849702 txt2dub-0.1.3/txt2dub/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-21 00:55:17.768751 txt2dub-0.1.3/txt2dub/__main__.py
+-rw-r--r--   0        0        0     6390 2023-05-21 00:55:17.768918 txt2dub-0.1.3/txt2dub/app.py
+-rw-r--r--   0        0        0      151 2023-05-21 00:55:17.769129 txt2dub-0.1.3/txt2dub/models/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-21 00:55:17.769290 txt2dub-0.1.3/txt2dub/models/base.py
+-rw-r--r--   0        0        0     6879 2023-05-21 00:55:17.769482 txt2dub-0.1.3/txt2dub/models/script.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.769639 txt2dub-0.1.3/txt2dub/screens/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-21 00:55:17.769844 txt2dub-0.1.3/txt2dub/screens/file/__init__.py
+-rw-r--r--   0        0        0     8515 2023-05-21 00:55:17.770025 txt2dub-0.1.3/txt2dub/screens/file/screen.py
+-rw-r--r--   0        0        0     1321 2023-05-21 00:55:17.770181 txt2dub-0.1.3/txt2dub/screens/file/widgets.py
+-rw-r--r--   0        0        0       62 2023-05-21 00:55:17.770388 txt2dub-0.1.3/txt2dub/screens/script/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-21 00:55:17.770540 txt2dub-0.1.3/txt2dub/screens/script/messages.py
+-rw-r--r--   0        0        0    25548 2023-05-21 00:55:17.770770 txt2dub-0.1.3/txt2dub/screens/script/screen.py
+-rw-r--r--   0        0        0    16904 2023-05-21 00:55:17.771058 txt2dub-0.1.3/txt2dub/screens/script/widgets.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.771337 txt2dub-0.1.3/txt2dub/services/__init__.py
+-rw-r--r--   0        0        0     2076 2023-05-21 00:55:17.771526 txt2dub-0.1.3/txt2dub/services/actions.py
+-rw-r--r--   0        0        0     3110 2023-05-22 14:30:51.093950 txt2dub-0.1.3/txt2dub/services/tts.py
+-rw-r--r--   0        0        0     5690 2023-05-22 14:34:52.768498 txt2dub-0.1.3/txt2dub/styles/app.css
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.772437 txt2dub-0.1.3/txt2dub/tts/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-21 00:55:17.772613 txt2dub-0.1.3/txt2dub/tts/__main__.py
+-rw-r--r--   0        0        0     5192 2023-05-22 14:42:48.692063 txt2dub-0.1.3/txt2dub/tts/interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-21 00:55:17.773094 txt2dub-0.1.3/txt2dub/widgets/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-21 00:55:17.773375 txt2dub-0.1.3/txt2dub/widgets/base.py
+-rw-r--r--   0        0        0      479 2023-05-21 00:55:17.773647 txt2dub-0.1.3/txt2dub/widgets/logo.py
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 txt2dub-0.1.3/PKG-INFO
```

### Comparing `txt2dub-0.1.2/LICENSE` & `txt2dub-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/README.md` & `txt2dub-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/pyproject.toml` & `txt2dub-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "txt2dub"
-version = "0.1.2"
+version = "0.1.3"
 homepage = "https://github.com/NotYourDadsMath/txt2dub"
 description = "A text-based UI application for editing voiceover scripts and generating text to speech performances."
 authors = ["Mike Kibbel", "Not Your Dad's Math"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 textual = "^0.26.0"
 pyobjc = {version = "9.0.1", platform = "darwin"}
-pyttsx3 = {git = "https://github.com/skibblenybbles/pyttsx3", rev = "a83dd354bdec4c5011f6d31f887fb5638ec2d7e2"}
+pyttsx3-alt = "^2.91"
 
 [tool.poetry.group.dev.dependencies]
 textual-dev = "^0.0.2"
 
 [tool.poetry.scripts]
 txt2dub = "txt2dub.app:run"
```

### Comparing `txt2dub-0.1.2/txt2dub/app.py` & `txt2dub-0.1.3/txt2dub/app.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/models/base.py` & `txt2dub-0.1.3/txt2dub/models/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/models/script.py` & `txt2dub-0.1.3/txt2dub/models/script.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/screens/file/screen.py` & `txt2dub-0.1.3/txt2dub/screens/file/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/screens/file/widgets.py` & `txt2dub-0.1.3/txt2dub/screens/file/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/screens/script/messages.py` & `txt2dub-0.1.3/txt2dub/screens/script/messages.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/screens/script/screen.py` & `txt2dub-0.1.3/txt2dub/screens/script/screen.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/screens/script/widgets.py` & `txt2dub-0.1.3/txt2dub/screens/script/widgets.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/services/actions.py` & `txt2dub-0.1.3/txt2dub/services/actions.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/services/tts.py` & `txt2dub-0.1.3/txt2dub/services/tts.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/styles/app.css` & `txt2dub-0.1.3/txt2dub/styles/app.css`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/tts/interpreter.py` & `txt2dub-0.1.3/txt2dub/tts/interpreter.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/txt2dub/widgets/base.py` & `txt2dub-0.1.3/txt2dub/widgets/base.py`

 * *Files identical despite different names*

### Comparing `txt2dub-0.1.2/PKG-INFO` & `txt2dub-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: txt2dub
-Version: 0.1.2
+Version: 0.1.3
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
 Requires-Dist: pyobjc (==9.0.1) ; sys_platform == "darwin"
-Requires-Dist: pyttsx3 @ git+https://github.com/skibblenybbles/pyttsx3@a83dd354bdec4c5011f6d31f887fb5638ec2d7e2
+Requires-Dist: pyttsx3-alt (>=2.91,<3.0)
 Requires-Dist: textual (>=0.26.0,<0.27.0)
 Description-Content-Type: text/markdown
 
 txt2dub
 =======
 
 A text-based UI application for editing voiceover scripts and generating text to speech performances.
```

