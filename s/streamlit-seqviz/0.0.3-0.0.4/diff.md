# Comparing `tmp/streamlit-seqviz-0.0.3.tar.gz` & `tmp/streamlit-seqviz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-seqviz-0.0.3.tar", last modified: Mon May 22 07:39:11 2023, max compression
+gzip compressed data, was "streamlit-seqviz-0.0.4.tar", last modified: Mon May 22 07:42:57 2023, max compression
```

## Comparing `streamlit-seqviz-0.0.3.tar` & `streamlit-seqviz-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/
--rw-rw-r--   0 utente    (1000) utente    (1000)       92 2023-05-21 16:23:08.000000 streamlit-seqviz-0.0.3/MANIFEST.in
--rw-rw-r--   0 utente    (1000) utente    (1000)     2057 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/PKG-INFO
--rw-rw-r--   0 utente    (1000) utente    (1000)     4142 2023-05-22 07:38:56.000000 streamlit-seqviz-0.0.3/README.md
--rw-rw-r--   0 utente    (1000) utente    (1000)       38 2023-05-22 07:39:11.023860 streamlit-seqviz-0.0.3/setup.cfg
--rw-rw-r--   0 utente    (1000) utente    (1000)     1039 2023-05-22 07:39:02.000000 streamlit-seqviz-0.0.3/setup.py
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/streamlit_seqviz/
--rw-rw-r--   0 utente    (1000) utente    (1000)     1558 2023-05-20 17:34:33.000000 streamlit-seqviz-0.0.3/streamlit_seqviz/__init__.py
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/assets/
--rw-rw-r--   0 utente    (1000) utente    (1000)   228669 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/assets/index-2420fc27.js
--rw-rw-r--   0 utente    (1000) utente    (1000)      540 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/index.html
--rw-rw-r--   0 utente    (1000) utente    (1000)     1497 2023-05-21 16:18:17.000000 streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/vite.svg
-drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:39:11.019860 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/
--rw-rw-r--   0 utente    (1000) utente    (1000)     2057 2023-05-22 07:39:10.000000 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/PKG-INFO
--rw-rw-r--   0 utente    (1000) utente    (1000)      396 2023-05-22 07:39:10.000000 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/SOURCES.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)        1 2023-05-22 07:39:10.000000 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/dependency_links.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)       16 2023-05-22 07:39:10.000000 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/requires.txt
--rw-rw-r--   0 utente    (1000) utente    (1000)       17 2023-05-22 07:39:10.000000 streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/top_level.txt
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/
+-rw-rw-r--   0 utente    (1000) utente    (1000)       92 2023-05-21 16:23:08.000000 streamlit-seqviz-0.0.4/MANIFEST.in
+-rw-rw-r--   0 utente    (1000) utente    (1000)     2035 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/PKG-INFO
+-rw-rw-r--   0 utente    (1000) utente    (1000)     4142 2023-05-22 07:38:56.000000 streamlit-seqviz-0.0.4/README.md
+-rw-rw-r--   0 utente    (1000) utente    (1000)       38 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/setup.cfg
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1039 2023-05-22 07:42:48.000000 streamlit-seqviz-0.0.4/setup.py
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/streamlit_seqviz/
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1558 2023-05-20 17:34:33.000000 streamlit-seqviz-0.0.4/streamlit_seqviz/__init__.py
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.489360 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/assets/
+-rw-rw-r--   0 utente    (1000) utente    (1000)   228669 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/assets/index-2420fc27.js
+-rw-rw-r--   0 utente    (1000) utente    (1000)      540 2023-05-21 16:18:18.000000 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/index.html
+-rw-rw-r--   0 utente    (1000) utente    (1000)     1497 2023-05-21 16:18:17.000000 streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/vite.svg
+drwxrwxr-x   0 utente    (1000) utente    (1000)        0 2023-05-22 07:42:57.493360 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/
+-rw-rw-r--   0 utente    (1000) utente    (1000)     2035 2023-05-22 07:42:57.000000 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/PKG-INFO
+-rw-rw-r--   0 utente    (1000) utente    (1000)      396 2023-05-22 07:42:57.000000 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)        1 2023-05-22 07:42:57.000000 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)       16 2023-05-22 07:42:57.000000 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/requires.txt
+-rw-rw-r--   0 utente    (1000) utente    (1000)       17 2023-05-22 07:42:57.000000 streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/top_level.txt
```

### Comparing `streamlit-seqviz-0.0.3/PKG-INFO` & `streamlit-seqviz-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: streamlit-seqviz
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library is a streamlit app for chemical or medical use that show DNA sequences effectively
 Home-page: https://gitlab.com/nicolalandro/streamlit-seqviz
 Author: Nicola Landro
 Author-email: nicolaxx94@live.it
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nicolalandro/streamlit-seqviz
 Keywords: dna,streamlit,chemistry
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 [![Open in Streamlit](https://huggingface.co/datasets/huggingface/badges/raw/refs%2Fpr%2F11/open-in-hf-spaces-md-dark.svg)](https://huggingface.co/spaces/z-uo/DNASequenceVisualization)
 
 # Streamlit seqviz
-=============================
 
 This library is a streamlit app for chemical or medical use that show DNA sequences effectively based on [seqviz](https://github.com/Lattice-Automation/seqviz) js library.
 
 |white theme | dark theme |
 |------------|------------|
-|![Streamlit sample white theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/white_screen.png)|![Streamlit sample dark theme]( https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/black_screen.png)|
+|![Streamlit sample white theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/raw/main/imgs/white_screen.png)|![Streamlit sample dark theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/raw/main/imgs/black_screen.png)|
 
 Install with:
-```
+
+```bash
 pip install streamlit-seqviz
 ```
 
 Usage example:
 
-```
+```python
 from streamlit_seqviz import streamlit_seqviz
 
 streamlit_seqviz(
     name = "J23100",
     seq = "TTGACGGCTAGCTCAGTCCTAGGTACAGTGCTAGC",
     annotations = [{ "name": "promoter", "start": 0, "end": 30, "direction": 1 }],
     style =  { "height": "100vh", "width": "100vw" },
```

### Comparing `streamlit-seqviz-0.0.3/README.md` & `streamlit-seqviz-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.3/setup.py` & `streamlit-seqviz-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'streamlit_seqviz/pypi_readme.md'), 'r') as f:
   long_des = f.read()
 
 setuptools.setup(
     name="streamlit-seqviz",
-    version="0.0.3",
+    version="0.0.4",
     author="Nicola Landro",
     author_email="nicolaxx94@live.it",
     description="This library is a streamlit app for chemical or medical use that show DNA sequences effectively",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/nicolalandro/streamlit-seqviz",
     keywords = ['dna', 'streamlit', 'chemistry'],
```

### Comparing `streamlit-seqviz-0.0.3/streamlit_seqviz/__init__.py` & `streamlit-seqviz-0.0.4/streamlit_seqviz/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/assets/index-2420fc27.js` & `streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/assets/index-2420fc27.js`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/index.html` & `streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.3/streamlit_seqviz/frontend/dist/vite.svg` & `streamlit-seqviz-0.0.4/streamlit_seqviz/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `streamlit-seqviz-0.0.3/streamlit_seqviz.egg-info/PKG-INFO` & `streamlit-seqviz-0.0.4/streamlit_seqviz.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: streamlit-seqviz
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library is a streamlit app for chemical or medical use that show DNA sequences effectively
 Home-page: https://gitlab.com/nicolalandro/streamlit-seqviz
 Author: Nicola Landro
 Author-email: nicolaxx94@live.it
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/nicolalandro/streamlit-seqviz
 Keywords: dna,streamlit,chemistry
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 [![Open in Streamlit](https://huggingface.co/datasets/huggingface/badges/raw/refs%2Fpr%2F11/open-in-hf-spaces-md-dark.svg)](https://huggingface.co/spaces/z-uo/DNASequenceVisualization)
 
 # Streamlit seqviz
-=============================
 
 This library is a streamlit app for chemical or medical use that show DNA sequences effectively based on [seqviz](https://github.com/Lattice-Automation/seqviz) js library.
 
 |white theme | dark theme |
 |------------|------------|
-|![Streamlit sample white theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/white_screen.png)|![Streamlit sample dark theme]( https://gitlab.com/nicolalandro/streamlit-seqviz/-/blob/main/imgs/black_screen.png)|
+|![Streamlit sample white theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/raw/main/imgs/white_screen.png)|![Streamlit sample dark theme](https://gitlab.com/nicolalandro/streamlit-seqviz/-/raw/main/imgs/black_screen.png)|
 
 Install with:
-```
+
+```bash
 pip install streamlit-seqviz
 ```
 
 Usage example:
 
-```
+```python
 from streamlit_seqviz import streamlit_seqviz
 
 streamlit_seqviz(
     name = "J23100",
     seq = "TTGACGGCTAGCTCAGTCCTAGGTACAGTGCTAGC",
     annotations = [{ "name": "promoter", "start": 0, "end": 30, "direction": 1 }],
     style =  { "height": "100vh", "width": "100vw" },
```

