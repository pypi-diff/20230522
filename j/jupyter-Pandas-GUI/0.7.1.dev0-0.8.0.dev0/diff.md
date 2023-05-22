# Comparing `tmp/jupyter_Pandas_GUI-0.7.1.dev0.tar.gz` & `tmp/jupyter_Pandas_GUI-0.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_Pandas_GUI-0.7.1.dev0.tar", last modified: Sun Dec 18 20:37:46 2022, max compression
+gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev0.tar", last modified: Mon May 22 20:04:23 2023, max compression
```

## Comparing `jupyter_Pandas_GUI-0.7.1.dev0.tar` & `jupyter_Pandas_GUI-0.8.0.dev0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-12-18 20:37:46.693811 jupyter_Pandas_GUI-0.7.1.dev0/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.7.1.dev0/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8931 2022-12-18 20:37:46.693811 jupyter_Pandas_GUI-0.7.1.dev0/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8185 2022-12-18 20:37:08.000000 jupyter_Pandas_GUI-0.7.1.dev0/README.md
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-12-18 20:37:46.693811 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8931 2022-12-18 20:37:46.000000 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2022-12-18 20:37:46.000000 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2022-12-18 20:37:46.000000 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      135 2022-12-18 20:37:46.000000 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2022-12-18 20:37:46.000000 jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2022-12-18 20:37:46.693811 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 20:31:15.000000 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49556 2022-07-15 21:38:13.000000 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/fit_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11896 2022-07-15 21:38:13.000000 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/new_pandas_column_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29284 2022-07-15 21:38:13.000000 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/plot_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    13802 2022-07-15 21:38:13.000000 jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2022-12-18 20:37:46.693811 jupyter_Pandas_GUI-0.7.1.dev0/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1291 2022-12-18 16:43:34.000000 jupyter_Pandas_GUI-0.7.1.dev0/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev0/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev0/README.md
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-22 20:04:23.000000 jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49764 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/fit_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/new_pandas_column_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/plot_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14280 2023-05-22 19:12:16.000000 jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-22 20:04:23.658833 jupyter_Pandas_GUI-0.8.0.dev0/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1324 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev0/setup.py
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/LICENSE` & `jupyter_Pandas_GUI-0.8.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_Pandas_GUI
-Version: 0.7.1.dev0
+Version: 0.8.0.dev0
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -151,14 +151,17 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
+* 0.8.0dev (2023-5-)
+  * In Jupyter Lab results of running code now replace the GUI rather than 
+    appearing in the Console.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/README.md` & `jupyter_Pandas_GUI-0.8.0.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,17 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
+* 0.8.0dev (2023-5-)
+  * In Jupyter Lab results of running code now replace the GUI rather than 
+    appearing in the Console.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev0/jupyter_Pandas_GUI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-Pandas-GUI
-Version: 0.7.1.dev0
+Version: 0.8.0.dev0
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -151,14 +151,17 @@
 *Development*
 
 Simply replace `$ pip install jupyter-Pandas-GUI` with `$ pip 
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
+* 0.8.0dev (2023-5-)
+  * In Jupyter Lab results of running code now replace the GUI rather than 
+    appearing in the Console.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/__init__.py` & `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/fit_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/fit_Pandas_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,34 +49,34 @@
     
     :keyword bool findframes: default = True. If set to false and dataframes
     are passed in dfs_info, will not search for dataframes in the user
     namespace.
     """
     from ipywidgets import Layout, Box, HBox, VBox, GridBox, Tab, \
         Accordion, Dropdown, Label, Text, Button, Checkbox, FloatText, \
-        RadioButtons, BoundedIntText
+        RadioButtons, BoundedIntText, Output
     from ipywidgets import HTML as richLabel
     from ipywidgets import HTMLMath as texLabel
     from IPython.display import display, HTML
     from IPython.display import Javascript as JS
     from IPython import get_ipython
     from JPSLUtils.utils import new_cell_immediately_below,\
         select_cell_immediately_below, move_cursor_in_current_cell, \
         insert_text_into_next_cell, insert_text_at_beginning_of_current_cell, \
         insert_newline_at_end_of_current_cell, select_containing_cell, \
         delete_selected_cell, iconselector, notice_group, \
         replace_text_of_current_cell, pseudoLatexToLatex
-    import JPSLUtils
     from lmfit import models
-    if JPSLUtils.notebookenv != 'colab':
-        import plotly.graph_objects as go
 
     from .utils import find_pandas_dataframe_names, build_run_snip_widget
     from IPython import get_ipython
     global_dict = get_ipython().user_ns
+    JPSLUtils = global_dict["JPSLUtils"]
+    if JPSLUtils.notebookenv != 'colab':
+        import plotly.graph_objects as go
     dfs_info = []
     if isinstance(df_info,list):
         for k in df_info:
             dfs_info.append(k)
     findframes = kwargs.pop('findframes',True)
     if findframes:
         for k in find_pandas_dataframe_names():
@@ -289,24 +289,26 @@
     step3str = ''
     step4str = ''
     step5str = ''
     step6str = ''
     range_chosen = False
     #### Define GUI Elements ####
     # Those followed by a * are required.
-    display(HTML(
-        "<h3 id ='pandasfitGUI' style='text-align:center;'>Pandas Fit "
-        "Composer</h3> <div style='text-align:center;'>"
-        "<span style='color:green;'>Steps with a * are required.</span> The "
-        "code that will generate the fit is being "
-        "built in the cell immediately below.</div><div "
-        "style='text-align:center;'>This composer uses a subset of "
-        "<a href ='https://lmfit.github.io/lmfit-py/'> the lmfit package</a>"
-        " and <a href ='https://plotly.com/python/line-and-scatter/#'> "
-        "the plotly scatter plot</a> capabilities.</div>"))
+    output = Output()
+    with output:
+        display(HTML(
+            "<h3 id ='pandasfitGUI' style='text-align:center;'>Pandas Fit "
+            "Composer</h3> <div style='text-align:center;'>"
+            "<span style='color:green;'>Steps with a * are required.</span> The "
+            "code that will generate the fit is being "
+            "built in the cell immediately below.</div><div "
+            "style='text-align:center;'>This composer uses a subset of "
+            "<a href ='https://lmfit.github.io/lmfit-py/'> the lmfit package</a>"
+            " and <a href ='https://plotly.com/python/line-and-scatter/#'> "
+            "the plotly scatter plot</a> capabilities.</div>"))
 
     longdesc = {'description_width':'initial'}
 
     # Notices for the Final Check Tab.
     makeplot_notices = notice_group(['Need data to fit',
                                      'Need a fit model',
                                      'Axes must have labels.'],
@@ -556,15 +558,15 @@
             params_set.children[i].children[1].children[1].value = value
             params_set.children[i].children[1].children[2].value = min
             params_set.children[i].children[1].children[3].value = max
         pass
 
     def make_param_set():
         '''
-        Creates at VBox with 7 parameters each having fields in an HBox:
+        Creates a VBox with 7 parameters each having fields in an HBox:
         1. fixcheck (checkbox for fixing the value)
         2. valuefield (floatText for setting the value)
         3. minfield (floatText for setting the minimum allowed value)
         4. maxfield (floatText for setting the maximum allowed value)
         By default the all VBox components have their `layout.display=none`.
         :return: VBox
         '''
@@ -1019,15 +1021,19 @@
         else:
             codearea.sniptext.value = importstr + step1str + step2str + \
                                       step3str + step4str + step5str + \
                                       pseudoLatexToLatex(step6str)
         pass
 
     steps.observe(tab_changed, names = 'selected_index')
-    display(steps)
+    with output:
+        display(steps)
     if JPSLUtils.notebookenv == 'NBClassic':
+        display(output)
         select_containing_cell('pandasfitGUI')
         new_cell_immediately_below()
     else:
-        codearea = build_run_snip_widget('')
-        display(codearea)
+        codearea = build_run_snip_widget('', output)
+        with output:
+            display(codearea)
+        display(output)
     pass
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/new_pandas_column_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/new_pandas_column_GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import JPSLUtils
-
 def new_pandas_column_GUI(df_info=None, show_text_col = False, **kwargs):
     """
     If passed no parameters this will look for all the dataframes in the user
     namespace and make them available for adding a new column to. Once a
     dataframe is chosen only the numerical columns from that dataframe will
     be available for inclusion in the new column expression.
 
@@ -24,28 +22,28 @@
       
     :keyword bool findframes: default = True. If set to false and dataframes
     are passed in dfs_info, will not search for dataframes in the user
     namespace.
     """
 
     from ipywidgets import Layout, Box, HBox, VBox, GridBox, Tab, \
-        Dropdown, Label, Text, Textarea, Button, Checkbox
+        Dropdown, Label, Text, Textarea, Button, Checkbox, Output
     from ipywidgets import HTML as richLabel
     from IPython.display import display, HTML
     from IPython import get_ipython
     from JPSLUtils.utils import new_cell_immediately_below,\
         select_cell_immediately_below, move_cursor_in_current_cell, \
         insert_text_into_next_cell, insert_text_at_beginning_of_current_cell, \
         insert_newline_at_end_of_current_cell, select_containing_cell, \
         delete_selected_cell, replace_text_of_next_cell
-    from JPSLUtils import notebookenv
 
     from .utils import find_pandas_dataframe_names, build_run_snip_widget
     from IPython import get_ipython
     global_dict = get_ipython().user_ns
+    JPSLUtils = global_dict["JPSLUtils"]
     dfs_info = []
     if isinstance(df_info,list):
         for k in df_info:
             dfs_info.append(k)
     findframes = kwargs.pop('findframes',True)
     if findframes:
         for k in find_pandas_dataframe_names():
@@ -264,23 +262,28 @@
     step4 = HBox(children=[step4instr, step4act])
 
     steps = Tab(children=[step1, step2, step3, step4])
     steps.set_title(0, 'Step 1')
     steps.set_title(1, 'Step 2')
     steps.set_title(2, 'Step 3')
     steps.set_title(3, 'Step 4')
+    
+    output = Output()
+    codearea = build_run_snip_widget(importstr, output)
 
-    codearea = build_run_snip_widget(importstr)
-
-    display(HTML(
+    with output:
+        display(HTML(
         "<h3 id ='newcolGUI' style='text-align:center;'>Pandas New Calculated "
         "Column "
         "Composer</h3>"))
-    display(steps)
+        display(steps)
     if JPSLUtils.notebookenv == 'NBClassic':
+        display(output)
         select_containing_cell('newcolGUI')
         new_cell_immediately_below()
         select_containing_cell('newcolGUI')
         replace_text_of_next_cell(importstr)
     else:
-        display(codearea)
+        with output:
+            display(codearea)
+        display(output)
     pass
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/plot_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/plot_Pandas_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,30 +26,30 @@
 
     :keyword bool findframes: default = True. If set to false and dataframes
     are passed in dfs_info, will not search for dataframes in the user
     namespace.
     """
     from ipywidgets import Layout, Box, HBox, VBox, GridBox, Tab, \
         Accordion, Dropdown, Label, Text, Button, Checkbox, FloatText, \
-        RadioButtons, BoundedIntText
+        RadioButtons, BoundedIntText, Output
     from ipywidgets import HTML as richLabel
     from IPython.display import display, HTML
     from IPython.display import Javascript as JS
     from IPython import get_ipython
     from JPSLUtils.utils import new_cell_immediately_below,\
         select_cell_immediately_below, move_cursor_in_current_cell, \
         insert_text_into_next_cell, insert_text_at_beginning_of_current_cell, \
         insert_newline_at_end_of_current_cell, select_containing_cell, \
         delete_selected_cell, iconselector, notice_group, notebookenv, \
         replace_text_of_next_cell
-    import JPSLUtils
 
     from .utils import find_pandas_dataframe_names, build_run_snip_widget
     from IPython import get_ipython
     global_dict = get_ipython().user_ns
+    JPSLUtils = global_dict["JPSLUtils"]
     dfs_info = []
     if isinstance(df_info,list):
         for k in df_info:
             dfs_info.append(k)
     findframes = kwargs.pop('findframes',True)
     if findframes:
         for k in find_pandas_dataframe_names():
@@ -64,15 +64,17 @@
         raise UserWarning (str(figname) + ' already exists. Choose a '
                                           'different name for the figure.')
     if figname == None:
         figname = 'Figure_'+str(len(figlst)+1)
 
     #### Define GUI Elements ####
     # Those followed by a * are required.
-    display(HTML(
+    output = Output()
+    with output:
+        display(HTML(
         "<h3 id ='pandasplotGUI' style='text-align:center;'>Pandas Plot "
         "Composer</h3> <div style='text-align:center;'>"
         "<span style='color:green;'>Steps with a * are required.</span> The "
         "code that will generate the plot is being "
         "built in the cell immediately below.</div><div "
         "style='text-align:center;'>This composer uses a subset of "
         "<a href ='https://plotly.com/python/line-and-scatter/#'> "
@@ -621,16 +623,21 @@
                     importstr+step1str+step2str+step3str+text)
             else:
                 codearea.sniptext.value = importstr+step1str+step2str+step3str+text
 
         pass
 
     steps.observe(tab_changed, names = 'selected_index')
-    display(steps)
+    with output:
+        display(steps)
     if JPSLUtils.notebookenv == 'NBClassic':
+        display(output)
         select_containing_cell('pandasplotGUI')
         new_cell_immediately_below()
         insert_text_into_next_cell(importstr+step1str+step2str+step3str)
     else:
-        codearea = build_run_snip_widget(importstr+step1str+step2str+step3str)
-        display(codearea)
+        codearea = build_run_snip_widget(
+            importstr+step1str+step2str+step3str, output)
+        with output:
+            display(codearea)
+        display(output)
     pass
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/pandas_GUI/utils.py` & `jupyter_Pandas_GUI-0.8.0.dev0/pandas_GUI/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -303,56 +303,66 @@
         for j in self.active:
             notice_txt += itemstart + self.noticelist[j]+'</li>'
         notice_txt += notice_footer
         return notice_txt
 
 class build_run_snip_widget(ipywidgets.GridBox):
 
-    def __init__(self, defaulttxt):
+    def __init__(self, defaulttxt, output_elem):
+        """
+        Defines a widget that runs code built in it and replaces itself with
+        the results.
+        :param defaulttxt: Initial text in the codebox
+        :param output_elem: Where this element will be located (an ipywidget
+        `Output()` element). Must be created before creating this object.
+        """
         from ipywidgets import Textarea, Layout, Button, VBox, GridBox
         from ipywidgets import HTML as richLabel
         from IPython.display import display, HTML, clear_output
         self.sniptext = Textarea(
             layout=Layout(width='98%', height='200px'),
             value=defaulttxt
         )
         self.value = self.sniptext.value
         self.dobutton = Button(description='Run Code')
         self.instructions = richLabel(value = '<div style="line-height:1;">' \
-                                      '<p><span style="color:red;">If you ' \
-                                      'are running in Jupyter Lab</span>, ' \
-                                      'the results of running ' \
-                                      'the code will be output to the ' \
-                                      'log console instead of the output of ' \
-                                      'this cell. To show the results in ' \
-                                      'the output of a code cell, copy the ' \
-                                      'code at left into a code cell ' \
-                                      'and run it.</p>' \
-                                      '<p><span style = "color:blue;">' \
-                                      'If you are running in Colab</span>, ' \
+                                      '<p>If you are running in ' \
+                                      '<span style="color:red;">Jupyter ' \
+                                      'Lab</span>, ' \
+                                      'or in <span style = "color:blue;">' \
+                                      'Colab</span>, ' \
                                       'clicking on the "Run Code" button ' \
                                       'will replace this GUI with the ' \
                                       'results of running the code. Copying ' \
                                       'the code in the collapsed "Code ' \
                                       'that was run" summary to a code cell ' \
                                       'will prevent the code ' \
                                       'from being lost if outputs are ' \
-                                      'cleared.</p></div>')
+                                      'cleared.</p><br/>' \
+                                      '<p>POWER USER HINT: ' \
+                                      'You can repeatedly try different ' \
+                                      'settings by copying the completed ' \
+                                      'code from the text box at left into ' \
+                                      'a code cell. Then run it. Then use ' \
+                                      'the GUI tools to update the code at ' \
+                                      'left and try again.' \
+                                      '</p></div>')
         self.dobox = VBox([self.dobutton,self.instructions])
         def onRunCode(change):
             from IPython import get_ipython
             shell = get_ipython()
-            clear_output()
-            display(HTML(
+            output_elem.clear_output()
+            with output_elem:
+                display(HTML(
                 '<details><summary style="cursor:pointer;"><span style="font-weight:bold;"><a>' \
                 'Code that was run</a></span>(click to toggle visibility)</summary>' \
                 '<div style="background:#eff0f1;white-space:pre-line;white-space:pre-wrap;">' \
                 '<pre>' + self.sniptext.value + '</pre></div></details>'))
-            display(HTML('<h3>Result<h3>'))
-            exec(str(self.sniptext.value), shell.user_ns)
+                display(HTML('<h3>Result<h3>'))
+                exec(str(self.sniptext.value), shell.user_ns)
             pass
 
         self.dobutton.on_click(onRunCode)
 
         super(build_run_snip_widget, self).__init__([self.sniptext,
                                              self.dobox],
                                             layout=Layout(
```

### Comparing `jupyter_Pandas_GUI-0.7.1.dev0/setup.py` & `jupyter_Pandas_GUI-0.8.0.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="jupyter_Pandas_GUI",
-    version="0.7.1dev",
+    version="0.8.0dev",
     description="Pandas expression composers using Jupyter widgets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="fitting, data-analysis, plotting, learning to code",
     license="GPL-3.0+",
     packages=setuptools.find_packages(),
     package_data={},
     include_package_data=True,
     install_requires=[
         # 'python>=3.6',
         'jupyter>=1.0.0',
+        'jupyterlab>=3.6, <4.0',
         'pandas>=1.5.2',
         'numpy>=1.23.0',
         'plotly>=5.5.0',
         'ipywidgets>=7.6.2, <8.0',
         'JPSLUtils>=0.7.0',
         'lmfit>=1.1.0',
         'round-using-error>=1.2.0',
```

