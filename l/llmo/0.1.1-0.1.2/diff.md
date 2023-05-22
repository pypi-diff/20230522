# Comparing `tmp/llmo-0.1.1.tar.gz` & `tmp/llmo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.1.1.tar", last modified: Mon May 22 07:56:42 2023, max compression
+gzip compressed data, was "llmo-0.1.2.tar", last modified: Mon May 22 08:01:10 2023, max compression
```

## Comparing `llmo-0.1.1.tar` & `llmo-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.1/LICENSE
--rw-r--r--   0        0        0     2136 2023-05-22 07:56:21.885668 llmo-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.1/llmo/__init__.py
--rw-r--r--   0        0        0    18345 2023-05-22 07:50:07.144972 llmo-0.1.1/llmo/chat.py
--rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.1/llmo/layout.css
--rw-r--r--   0        0        0      614 2023-05-22 07:56:42.452059 llmo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 llmo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2136 2023-05-22 07:56:21.885668 llmo-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.2/llmo/__init__.py
+-rw-r--r--   0        0        0    18346 2023-05-22 08:00:50.504525 llmo-0.1.2/llmo/chat.py
+-rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.2/llmo/layout.css
+-rw-r--r--   0        0        0      614 2023-05-22 08:01:10.976346 llmo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 llmo-0.1.2/PKG-INFO
```

### Comparing `llmo-0.1.1/LICENSE` & `llmo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.1.1/README.md` & `llmo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.1.1/llmo/chat.py` & `llmo-0.1.2/llmo/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         action="store_true",
         help="enable rich text mode (not recommended for programming)",
     )
     parser.add_argument(
         "-s",
         "--shell-mode",
         action="store_true",
-        help="pure shell mode (no UI)",
+        help="pure shell mode (no GUI)",
     )
 
     disable_personality_env_var = os.getenv("LLMO_DISABLE_PERSONALITY", "")
 
     if (
         disable_personality_env_var.lower().startswith("t")
         or disable_personality_env_var == "1"
```

### Comparing `llmo-0.1.1/pyproject.toml` & `llmo-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.1.1"
+version = "0.1.2"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.1.1/PKG-INFO` & `llmo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
 Description-Content-Type: text/markdown
```

