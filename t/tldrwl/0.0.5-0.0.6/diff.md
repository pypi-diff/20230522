# Comparing `tmp/tldrwl-0.0.5.tar.gz` & `tmp/tldrwl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.5.tar", last modified: Mon May 22 07:30:25 2023, max compression
+gzip compressed data, was "tldrwl-0.0.6.tar", last modified: Mon May 22 07:37:29 2023, max compression
```

## Comparing `tldrwl-0.0.5.tar` & `tldrwl-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:30:25.690584 tldrwl-0.0.5/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.5/MANIFEST.in
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:30:25.690584 tldrwl-0.0.5/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    11716 2023-05-22 07:29:21.000000 tldrwl-0.0.5/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.5/requirements.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 07:30:25.690584 tldrwl-0.0.5/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 07:30:13.000000 tldrwl-0.0.5/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:30:25.690584 tldrwl-0.0.5/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.5/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      907 2023-05-22 06:42:51.000000 tldrwl-0.0.5/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.5/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.5/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1146 2023-05-22 06:59:34.000000 tldrwl-0.0.5/tldrwl/summarize.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     4811 2023-05-22 06:57:55.000000 tldrwl-0.0.5/tldrwl/summarize_text.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2147 2023-05-22 06:55:40.000000 tldrwl-0.0.5/tldrwl/summarize_webpage.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1770 2023-05-22 06:43:53.000000 tldrwl-0.0.5/tldrwl/summarize_youtube.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:30:25.690584 tldrwl-0.0.5/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:30:25.000000 tldrwl-0.0.5/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 07:30:25.000000 tldrwl-0.0.5/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 07:30:25.000000 tldrwl-0.0.5/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 07:30:25.000000 tldrwl-0.0.5/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 07:30:25.000000 tldrwl-0.0.5/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.6/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:37:29.810449 tldrwl-0.0.6/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    11716 2023-05-22 07:29:21.000000 tldrwl-0.0.6/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.6/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 07:37:29.810449 tldrwl-0.0.6/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 07:37:15.000000 tldrwl-0.0.6/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.6/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      907 2023-05-22 06:42:51.000000 tldrwl-0.0.6/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.6/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.6/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1146 2023-05-22 06:59:34.000000 tldrwl-0.0.6/tldrwl/summarize.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     4811 2023-05-22 07:36:42.000000 tldrwl-0.0.6/tldrwl/summarize_text.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2147 2023-05-22 06:55:40.000000 tldrwl-0.0.6/tldrwl/summarize_webpage.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1770 2023-05-22 06:43:53.000000 tldrwl-0.0.6/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.5/PKG-INFO` & `tldrwl-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `tldrwl-0.0.5/README.md` & `tldrwl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/setup.py` & `tldrwl-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="0.0.5",
+    version="0.0.6",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-0.0.5/tldrwl/ai_interface.py` & `tldrwl-0.0.6/tldrwl/ai_interface.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl/exception.py` & `tldrwl-0.0.6/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl/register.py` & `tldrwl-0.0.6/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl/summarize.py` & `tldrwl-0.0.6/tldrwl/summarize.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl/summarize_text.py` & `tldrwl-0.0.6/tldrwl/summarize_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         if len(summaries) == 0:
             return Summary(text="", num_tokens=0, model=self._model)
         elif len(summaries) == 1:
             return summaries[0]
         else:
             final_input = " ".join(s.text for s in summaries)
             final_summary = await self._summarize_chunk_async(
-                final_input, max_tokens=2000
+                final_input, max_tokens=1500
             )
             return Summary(
                 text=final_summary.text,
                 num_tokens=final_summary.num_tokens
                 + sum(s.num_tokens for s in summaries),
                 model=self._model,
             )
```

### Comparing `tldrwl-0.0.5/tldrwl/summarize_webpage.py` & `tldrwl-0.0.6/tldrwl/summarize_webpage.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl/summarize_youtube.py` & `tldrwl-0.0.6/tldrwl/summarize_youtube.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.5/tldrwl.egg-info/PKG-INFO` & `tldrwl-0.0.6/tldrwl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

