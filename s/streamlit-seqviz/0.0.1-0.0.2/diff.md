# Comparing `tmp/streamlit-seqviz-0.0.1.tar.gz` & `tmp/streamlit-seqviz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-seqviz-0.0.1.tar", last modified: Sun May 21 16:17:04 2023, max compression
+gzip compressed data, was "streamlit-seqviz-0.0.2.tar", last modified: Mon May 22 07:32:13 2023, max compression
```

## Comparing `streamlit-seqviz-0.0.1.tar` & `streamlit-seqviz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-21 16:17:04.620346 streamlit-seqviz-0.0.1/
--rw-rw-r--   0 utente    (1000) utente    (1000)       89 2023-05-21 16:17:01.000000 streamlit-seqviz-0.0.1/MANIFEST.in
--rw-rw-r--   0 utente    (1000) utente    (1000)     1742 2023-05-21 16:17:04.620346 streamlit-seqviz-0.0.1/PKG-INFO
--rw-rw-r--   0 utente    (1000) utente    (1000)     2427 2023-05-21 16:06:11.000000 streamlit-seqviz-0.0.1/README.md
--rw-rw-r--   0 utente    (1000) utente    (1000)       38 2023-05-21 16:17:04.620346 streamlit-seqviz-0.0.1/setup.cfg
--rw-rw-r--   0 utente    (1000) utente    (1000)     1020 2023-05-21 16:06:57.000000 streamlit-seqviz-0.0.1/setup.py
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-21 16:17:04.620346 streamlit-seqviz-0.0.1/streamlit_seqviz/
--rw-rw-r--   0 utente    (1000) utente    (1000)     1558 2023-05-20 17:34:33.000000 streamlit-seqviz-0.0.1/streamlit_seqviz/__init__.py
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-21 16:17:04.620346 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/
--rw-rw-r--   0 utente    (1000) utente    (1000)     1742 2023-05-21 16:17:04.000000 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/PKG-INFO
--rw-rw-r--   0 utente    (1000) utente    (1000)      258 2023-05-21 16:17:04.000000 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/SOURCES.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)        1 2023-05-21 16:17:04.000000 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/dependency_links.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)       16 2023-05-21 16:17:04.000000 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/requires.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)       17 2023-05-21 16:17:04.000000 streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/top_level.txt
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.526805 streamlit-seqviz-0.0.2/
+-rw-rw-r--   0 utente    (1000) utente    (1000)       92 2023-05-21 16:23:08.000000 streamlit-seqviz-0.0.2/MANIFEST.in
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1969 2023-05-22 07:32:13.526805 streamlit-seqviz-0.0.2/PKG-INFO
+-rw-rw-r--   0 utente    (1000) utente    (1000)     4078 2023-05-22 07:30:36.000000 streamlit-seqviz-0.0.2/README.md
+-rw-rw-r--   0 utente    (1000) utente    (1000)       38 2023-05-22 07:32:13.526805 streamlit-seqviz-0.0.2/setup.cfg
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1037 2023-05-22 07:32:02.000000 streamlit-seqviz-0.0.2/setup.py
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.522805 streamlit-seqviz-0.0.2/streamlit_seqviz/
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1558 2023-05-20 17:34:33.000000 streamlit-seqviz-0.0.2/streamlit_seqviz/__init__.py
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.522805 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.522805 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/dist/
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.522805 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/dist/assets/
+-rw-rw-r--   0 utente    (1000) utente    (1000)   228669 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/dist/assets/index-2420fc27.js
+-rw-rw-r--   0 utente    (1000) utente    (1000)      540 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/dist/index.html
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1497 2023-05-21 16:18:17.000000 streamlit-seqviz-0.0.2/streamlit_seqviz/frontend/dist/vite.svg
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1487 2023-05-21 17:05:27.000000 streamlit-seqviz-0.0.2/streamlit_seqviz/pypi_readme.rst
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:32:13.522805 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1969 2023-05-22 07:32:13.000000 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/PKG-INFO
+-rw-rw-r--   0 utente    (1000) utente    (1000)      429 2023-05-22 07:32:13.000000 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)        1 2023-05-22 07:32:13.000000 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)       16 2023-05-22 07:32:13.000000 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/requires.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)       17 2023-05-22 07:32:13.000000 streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/top_level.txt
```

### Comparing `streamlit-seqviz-0.0.1/PKG-INFO` & `streamlit-seqviz-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: streamlit-seqviz
-Version: 0.0.1
+Version: 0.0.2
 Summary: This library is a streamlit app for chemical or medical use that show DNA sequences effectively
 Home-page: https://gitlab.com/nicolalandro/streamlit-seqviz
 Author: Nicola Landro
 Author-email: nicolaxx94@live.it
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nicolalandro/streamlit-seqviz
 Keywords: dna,streamlit,chemistry
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
 
+|huggingface badge|
+
+.. |huggingface badge| image:: https://huggingface.co/datasets/huggingface/badges/raw/refs%2Fpr%2F11/open-in-hf-spaces-md-dark.svg
+    :target: https://huggingface.co/spaces/z-uo/DNASequenceVisualization
+
+
 Streamlit seqviz
 =============================
 
 This library is a streamlit app for chemical or medical use that show DNA sequences effectively based on `seqviz <https://github.com/Lattice-Automation/seqviz>`_ js library.
 
 .. image:: https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/white_screen.png
   :alt: Streamlit app example
```

### Comparing `streamlit-seqviz-0.0.1/setup.py` & `streamlit-seqviz-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 import os
-with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'pypi_readme.rst'), 'r') as f:
+with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'streamlit_seqviz/pypi_readme.rst'), 'r') as f:
   long_des = f.read()
 
 setuptools.setup(
     name="streamlit-seqviz",
-    version="0.0.1",
+    version="0.0.2",
     author="Nicola Landro",
     author_email="nicolaxx94@live.it",
     description="This library is a streamlit app for chemical or medical use that show DNA sequences effectively",
     long_description=long_des,
     long_description_content_type="text/plain",
     url="https://gitlab.com/nicolalandro/streamlit-seqviz",
     keywords = ['dna', 'streamlit', 'chemistry'],
```

### Comparing `streamlit-seqviz-0.0.1/streamlit_seqviz/__init__.py` & `streamlit-seqviz-0.0.2/streamlit_seqviz/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.1/streamlit_seqviz.egg-info/PKG-INFO` & `streamlit-seqviz-0.0.2/streamlit_seqviz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: streamlit-seqviz
-Version: 0.0.1
+Version: 0.0.2
 Summary: This library is a streamlit app for chemical or medical use that show DNA sequences effectively
 Home-page: https://gitlab.com/nicolalandro/streamlit-seqviz
 Author: Nicola Landro
 Author-email: nicolaxx94@live.it
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nicolalandro/streamlit-seqviz
 Keywords: dna,streamlit,chemistry
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
 
+|huggingface badge|
+
+.. |huggingface badge| image:: https://huggingface.co/datasets/huggingface/badges/raw/refs%2Fpr%2F11/open-in-hf-spaces-md-dark.svg
+    :target: https://huggingface.co/spaces/z-uo/DNASequenceVisualization
+
+
 Streamlit seqviz
 =============================
 
 This library is a streamlit app for chemical or medical use that show DNA sequences effectively based on `seqviz <https://github.com/Lattice-Automation/seqviz>`_ js library.
 
 .. image:: https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/white_screen.png
   :alt: Streamlit app example
```

