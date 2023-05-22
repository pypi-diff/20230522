# Comparing `tmp/rbtoolz-1.2.9.tar.gz` & `tmp/rbtoolz-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rbtoolz-1.2.9.tar", last modified: Sat Mar  4 10:54:23 2023, max compression
+gzip compressed data, was "rbtoolz-1.3.0.tar", last modified: Mon May 22 17:02:11 2023, max compression
```

## Comparing `rbtoolz-1.2.9.tar` & `rbtoolz-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)     2423 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/PKG-INFO
--rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)     1340 2023-03-04 10:54:11.000000 rbtoolz-1.2.9/README.md
-drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz/
--rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)        0 2020-04-08 21:31:45.000000 rbtoolz-1.2.9/rbtoolz/__init__.py
--rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)    12638 2023-03-04 10:47:47.000000 rbtoolz-1.2.9/rbtoolz/plotting.py
-drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)     2423 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/PKG-INFO
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)      222 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/SOURCES.txt
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)        1 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/dependency_links.txt
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)       28 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/requires.txt
--rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)        8 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/rbtoolz.egg-info/top_level.txt
--rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)       79 2023-03-04 10:54:23.000000 rbtoolz-1.2.9/setup.cfg
--rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)      755 2023-03-04 10:54:21.000000 rbtoolz-1.2.9/setup.py
+drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-05-22 17:02:11.764290 rbtoolz-1.3.0/
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)     1065 2020-04-08 21:31:44.000000 rbtoolz-1.3.0/LICENSE
+-rw-rw-r--   0 rbonallo  (1000) rbonallo  (1000)     1728 2023-05-22 17:02:11.764290 rbtoolz-1.3.0/PKG-INFO
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)     1295 2023-05-22 17:01:20.000000 rbtoolz-1.3.0/README.md
+drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-05-22 17:02:11.764290 rbtoolz-1.3.0/rbtoolz/
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)        0 2020-04-08 21:31:44.000000 rbtoolz-1.3.0/rbtoolz/__init__.py
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)    12640 2023-05-22 16:58:47.000000 rbtoolz-1.3.0/rbtoolz/plotting.py
+drwxrwxr-x   0 rbonallo  (1000) rbonallo  (1000)        0 2023-05-22 17:02:11.764290 rbtoolz-1.3.0/rbtoolz.egg-info/
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)     1728 2023-05-22 17:02:11.000000 rbtoolz-1.3.0/rbtoolz.egg-info/PKG-INFO
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)      230 2023-05-22 17:02:11.000000 rbtoolz-1.3.0/rbtoolz.egg-info/SOURCES.txt
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)        1 2023-05-22 17:02:11.000000 rbtoolz-1.3.0/rbtoolz.egg-info/dependency_links.txt
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)       28 2023-05-22 17:02:11.000000 rbtoolz-1.3.0/rbtoolz.egg-info/requires.txt
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)        8 2023-05-22 17:02:11.000000 rbtoolz-1.3.0/rbtoolz.egg-info/top_level.txt
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)       79 2023-05-22 17:02:11.768290 rbtoolz-1.3.0/setup.cfg
+-rw-r--r--   0 rbonallo  (1000) rbonallo  (1000)      755 2023-05-22 16:58:29.000000 rbtoolz-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rbtoolz-1.2.9/PKG-INFO` & `rbtoolz-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,90 @@
 Metadata-Version: 2.1
 Name: rbtoolz
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python-Pandas Postprocessing Library
 Home-page: https://github.com/rbonallo/rbtoolz
 Author: Ross Bonallo
 Author-email: rossbonallo@gmail.com
-License: UNKNOWN
-Description: # RBToolz
-        
-        RBToolz is a package of generic tools for use in Jupyter Notebooks that currently cover:
-        
-          - Plotly wrapper for quick rendering of Pandas DataFrames.
-        
-        ### Tech
-        
-        RBToolz wraps around a number of projects:
-        
-        * Jupyter Notebook
-        * Pandas
-        * Plotly
-        * Orca
-        
-        ### Installation
-        Install using regular pip 3.7
-        
-        ```sh
-        $ pip install rbtoolz
-        ```
-        ### Notebook Setup and Plotting Example
-        
-        Following steps are required to setup notebook and use postprocessing tools.
-        
-        Rendering to PNG files requires Orca/PIO installation:
-        
-        ```bash
-        conda install -c plotly plotly-orca psutil
-        ```
-        
-        * Notebook Cell HTML changes
-        
-        ```python
-        from IPython.core.display import display, SVG, HTML
-        from IPython.display import Image
-        display(HTML("<style>.container { width:100% !important; }</style>"))
-        ```
-        
-        * Plotly offline functions
-        ```python
-        import plotly.graph_objs as go
-        from plotly.offline import init_notebook_mode, iplot
-        ```
-        
-        * Import auto_plot from RBToolz
-        ```python
-        from rbtoolz.plotting import auto_plot
-        ```
-        
-        * Finally run a demo
-        ```python
-        df = pd.DataFrame([1,2,3],['A','B','C'])
-        fig = auto_plot(df)
-        iplot(fig)
-        ```
-        
-        * And for rendering figure to png
-        
-        ```python
-        import plotly.io as pio
-        
-        def save_fig(fig, filename):
-            pio.write_image(fig, format="png", file=filename)
-        
-        save_fig(fig,'data_chart.png')
-        
-        display(Image('data_chart.png'))
-        ```
-        
-        License
-        ----
-        
-        MIT
-        
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# RBToolz
+
+RBToolz is a package of generic tools for use in Jupyter Notebooks that currently cover:
+
+  - Quick postprocessing of Pandas DataFrames wrapped around Plotly
+
+### Tech
+
+RBToolz wraps around a number of projects:
+
+* Jupyter Notebook
+* Pandas
+* Plotly
+* Orca
+
+### Installation
+Install using regular pip 3.7
+
+```sh
+$ pip install rbtoolz
+```
+### Notebook Setup and Plotting Example
+
+Following steps are required to setup notebook and use postprocessing tools.
+
+Rendering to PNG files requires Orca/PIO installation:
+
+```bash
+conda install -c plotly plotly-orca psutil
+```
+
+* Notebook cell width to 100% (optional)
+
+```python
+from IPython.core.display import display, SVG, HTML
+from IPython.display import Image
+display(HTML("<style>.container { width:100% !important; }</style>"))
+```
+
+* Import Plotly offline functions
+```python
+from plotly.offline import init_notebook_mode, iplot
+```
+
+* Import functions from RBToolz
+```python
+from rbtoolz.plotting import auto_plot, save_fig
+```
+
+* Run a plotting demo
+```python
+df = pd.DataFrame([1,2,3],['A','B','C'])
+
+line_fig = auto_plot(df)
+bar_fig = auto_plot(df, mode='bar')
+
+iplot(line_fig)
+iplot(bar_fig)
+```
+
+* And for rendering figure to png
+
+```python
+save_fig(line_fig,'chart.png')
+
+display(Image('chart.png'))
+```
+
+License
+----
+
+MIT
+
+
+
+
```

### Comparing `rbtoolz-1.2.9/README.md` & `rbtoolz-1.3.0/rbtoolz.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+Metadata-Version: 2.1
+Name: rbtoolz
+Version: 1.3.0
+Summary: Python-Pandas Postprocessing Library
+Home-page: https://github.com/rbonallo/rbtoolz
+Author: Ross Bonallo
+Author-email: rossbonallo@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # RBToolz
 
 RBToolz is a package of generic tools for use in Jupyter Notebooks that currently cover:
 
-  - Plotly wrapper for quick rendering of Pandas DataFrames.
+  - Quick postprocessing of Pandas DataFrames wrapped around Plotly
 
 ### Tech
 
 RBToolz wraps around a number of projects:
 
 * Jupyter Notebook
 * Pandas
@@ -25,51 +39,49 @@
 
 Rendering to PNG files requires Orca/PIO installation:
 
 ```bash
 conda install -c plotly plotly-orca psutil
 ```
 
-* Notebook Cell HTML changes
+* Notebook cell width to 100% (optional)
 
 ```python
 from IPython.core.display import display, SVG, HTML
 from IPython.display import Image
 display(HTML("<style>.container { width:100% !important; }</style>"))
 ```
 
-* Plotly offline functions
+* Import Plotly offline functions
 ```python
-import plotly.graph_objs as go
 from plotly.offline import init_notebook_mode, iplot
 ```
 
-* Import auto_plot from RBToolz
+* Import functions from RBToolz
 ```python
-from rbtoolz.plotting import auto_plot
+from rbtoolz.plotting import auto_plot, save_fig
 ```
 
-* Finally run a demo
+* Run a plotting demo
 ```python
 df = pd.DataFrame([1,2,3],['A','B','C'])
-fig = auto_plot(df)
-iplot(fig)
+
+line_fig = auto_plot(df)
+bar_fig = auto_plot(df, mode='bar')
+
+iplot(line_fig)
+iplot(bar_fig)
 ```
 
 * And for rendering figure to png
 
 ```python
-import plotly.io as pio
-
-def save_fig(fig, filename):
-    pio.write_image(fig, format="png", file=filename)
-
-save_fig(fig,'data_chart.png')
+save_fig(line_fig,'chart.png')
 
-display(Image('data_chart.png'))
+display(Image('chart.png'))
 ```
 
 License
 ----
 
 MIT
```

### Comparing `rbtoolz-1.2.9/rbtoolz/plotting.py` & `rbtoolz-1.3.0/rbtoolz/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     Supports line, scatter and bar charts as well as histograms for N series.
 """
 
 
 __author__ = 'Ross Bonallo'
 __license__ = 'MIT Licence'
-__version__ = '1.2.8'
+__version__ = '1.3.0'
 
 
 import plotly.graph_objs as go
 from plotly import subplots
 import pandas as pd
 import numpy as np
 import matplotlib
@@ -187,15 +187,15 @@
     fig['layout'].update(height=rows*550, title=title, showlegend=showlegend,
                          paper_bgcolor='white', plot_bgcolor='white',
                          yaxis=dict(gridcolor='lightgrey'),
                          xaxis=dict(gridcolor='lightgrey'),
                          yaxis2=dict(gridcolor='lightgrey'),
                          xaxis2=dict(gridcolor='lightgrey'))
 
-    for i in range(2, rows*columns):
+    for i in range(2, rows*columns+1):
         fig['layout']['yaxis'+str(i)]['gridcolor'] = 'lightgrey'
         fig['layout']['xaxis'+str(i)]['gridcolor'] = 'lightgrey'
 
     if extra_layout:
         fig['layout'].update(extra_layout)
 
     return fig
```

### Comparing `rbtoolz-1.2.9/setup.py` & `rbtoolz-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rbtoolz", 
-    version="1.2.9",
+    version="1.3.0",
     author="Ross Bonallo",
     author_email="rossbonallo@gmail.com",
     description="Python-Pandas Postprocessing Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rbonallo/rbtoolz",
     packages=setuptools.find_packages(),
```

