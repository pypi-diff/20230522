# Comparing `tmp/swoopyui-1.3.1.tar.gz` & `tmp/swoopyui-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoopyui-1.3.1.tar", last modified: Sat May 20 23:05:00 2023, max compression
+gzip compressed data, was "swoopyui-1.4.tar", last modified: Mon May 22 18:26:14 2023, max compression
```

## Comparing `swoopyui-1.3.1.tar` & `swoopyui-1.4.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-20 23:04:49.000000 swoopyui-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 23:04:49.000000 swoopyui-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 23:05:00.515981 swoopyui-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-20 23:04:49.000000 swoopyui-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 23:04:49.000000 swoopyui-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:05:00.515981 swoopyui-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-20 23:04:49.000000 swoopyui-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/UIkits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/UIkits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   280787 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/assets/swoopyui.zip
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/swoopyui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/on_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/run_swiftUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/run_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/navigationview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-20 23:04:49.000000 swoopyui-1.3.1/swoopyui/views/textfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:05:00.515981 swoopyui-1.3.1/swoopyui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 23:05:00.000000 swoopyui-1.3.1/swoopyui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 18:26:03.000000 swoopyui-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 18:26:03.000000 swoopyui-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 18:26:14.962065 swoopyui-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 18:26:03.000000 swoopyui-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 18:26:03.000000 swoopyui-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:26:14.962065 swoopyui-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-22 18:26:03.000000 swoopyui-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/UIkits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/UIkits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   322687 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/assets/swoopyui.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/swoopyui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/swoopyui/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/check_if_mac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/on_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/pyinstaller_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/run_swiftUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/run_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/swoopyui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/scrollview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/top_level.txt
```

### Comparing `swoopyui-1.3.1/LICENSE` & `swoopyui-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/PKG-INFO` & `swoopyui-1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.3.1
+Version: 1.4
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # swoopyui
 A simple python library that allow you to build swiftUI apps using python.
 
 ## How does it work ?
```

### Comparing `swoopyui-1.3.1/README.md` & `swoopyui-1.4/README.md`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/setup.py` & `swoopyui-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='swoopyui',
-    version='1.3.1',
+    version='1.4',
     author='SKbarbon',
     description='A python library that allow you to build swiftUI apps using python.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/swoopyui',
     install_requires=["flask", "requests"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows"
+        "Operating System :: MacOS :: MacOS X"
     ],
     include_dirs=["assets"],
     package_data={"assets": ["swoopyui.zip"]},
     include_package_data=True
 )
```

### Comparing `swoopyui-1.3.1/swoopyui/protocol.py` & `swoopyui-1.4/swoopyui/protocol.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/swoopyui/swoopyui.py` & `swoopyui-1.4/swoopyui/swoopyui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from flask import Flask, request
 import socketserver
 import tempfile
 import threading
 import logging
 import shutil
 import os
+import sys
 
 from .protocol import onClientRequestUpdate
 from .tools.run_target import run_the_target
 from .tools.run_swiftUI import run_swiftUI_app
+from .tools.pyinstaller_check import is_run_on_pyinstaller
 from .view import View
 
 
 def run_swiftUI_on_new_process (PORT, tmp_dir):
     if not os.path.isdir (tmp_dir):
         print("Cannot found the temp dir.")
         os._exit(0)
@@ -77,15 +79,18 @@
                 shutil.rmtree(self.current_tmp_dir)
             # exit the script.
             os._exit(0)
 
         with socketserver.TCPServer(("localhost", 0), None) as s:
             free_port = s.server_address[1]
         
-        self.current_tmp_dir = tempfile.mkdtemp()
+        if is_run_on_pyinstaller():
+            self.current_tmp_dir = getattr(sys, "_MEIPASS", os.path.dirname(os.path.abspath(__file__)))
+        else:
+            self.current_tmp_dir = tempfile.mkdtemp()
         threading.Thread(target=run_swiftUI_on_new_process, args=[free_port, self.current_tmp_dir]).start()
         flask_app.run(port=free_port)
     
     def set_for_the_next_update_get (self, action_name:str, action_content:dict):
         self.__update_number = self.__update_number + 1
         cont = {"action":f"{action_name}", "action_content":action_content, "update_number":self.__update_number}
         self.__all_waited_updates.append(cont)
```

### Comparing `swoopyui-1.3.1/swoopyui/tools/run_swiftUI.py` & `swoopyui-1.4/swoopyui/tools/run_swiftUI.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/swoopyui/view.py` & `swoopyui-1.4/swoopyui/view.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/swoopyui/views/button.py` & `swoopyui-1.4/swoopyui/views/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,14 @@
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
-        self.__id = self.__mother_view.get_new_view_id()
-        self.__mother_view.update(self)
-        self.__last_view_id = self.__id
     
     def view_action (self, action_data):
         action_name = action_data["action_name"]
         if action_name == "on_click":
             on_view_action(self.on_click, [self])
     
     def update (self):
```

### Comparing `swoopyui-1.3.1/swoopyui/views/navigationlink.py` & `swoopyui-1.4/swoopyui/views/navigationlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,14 @@
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
-        self.__id = self.__mother_view.get_new_view_id()
-        self.__mother_view.update(self)
-        self.__last_view_id = self.__id
     
     def view_action (self, action_data):
         action_name = action_data['action_name']
         if action_name == "on_navigate":
             on_view_action(self.on_navigate, [self])
     
     def update (self):
```

### Comparing `swoopyui-1.3.1/swoopyui/views/navigationstack.py` & `swoopyui-1.4/swoopyui/views/navigationstack.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,17 +49,14 @@
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
-        self.__id = self.__mother_view.get_new_view_id()
-        self.__mother_view.update(self)
-        self.__last_view_id = self.__id
     
     def view_action (self, action_data):
         action_name = action_data['action_name']
         if action_name == "on_appear":
             on_view_action(self.on_appear, [self])
     
     def update (self):
```

### Comparing `swoopyui-1.3.1/swoopyui/views/navigationview.py` & `swoopyui-1.4/swoopyui/views/navigationview.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,17 +51,14 @@
         if self.__mother_view == None:
             raise Exception("Cannot add sub-views while this view not have an active mother view.")
         
         for subv in sub_view:
             subv.respown (new_id=self.__mother_view.get_new_view_id(), mother_view=self.__mother_view, parent=self)
             self.__mother_view.sub_views_history.append(subv)
             self.__subviews.append(subv)
-        self.__id = self.__mother_view.get_new_view_id()
-        self.__mother_view.update(self)
-        self.__last_view_id = self.__id
     
     def view_action (self, action_data):
         action_name = action_data['action_name']
         if action_name == "on_appear":
             on_view_action(self.on_appear, [self])
     
     def update (self):
```

### Comparing `swoopyui-1.3.1/swoopyui/views/text.py` & `swoopyui-1.4/swoopyui/views/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from ..tools.on_action import on_view_action
 
 
 class Text (object):
-    def __init__(self, text, foreground_color="primary", on_hover=None) -> None:
+    def __init__(self, text, foreground_color="primary", on_hover=None, bold:bool=False, size:float=18) -> None:
         self.__last_view_id = None # This is used becuase swiftUI will not know that this updated without it
         self.__id = None
         self.__mother_view = None
         self.__parent_view = None
 
-        self.__text = text
-        self.__foreground_color = foreground_color
+        self.__text : str = text
+        self.__foreground_color : str = foreground_color
         self.on_hover = on_hover
+        self.__bold : bool = bold
+        self.__size : str = size
     
 
     def get_dict_content (self):
         return {
             "last_view_id" : self.__last_view_id,
             "view_id" : self.__id,
             "vname" : "Text",
             "text" : self.__text,
-            "fgcolor" : self.__foreground_color
+            "fgcolor" : self.__foreground_color,
+            "bold" : self.__bold,
+            "size" : self.__size
         }
 
     def respown (self, new_id=None, mother_view=None, parent=None):
         if new_id == None: return
         if mother_view == None: return
         if parent == None: return
 
@@ -67,8 +71,37 @@
     def foreground_color (self, value):
         if self.__mother_view == None:
             raise Exception("Cannot change the sub_view property while its not on the screen.")
         
         self.__foreground_color = value
         self.__id = self.__mother_view.get_new_view_id()
         self.__mother_view.update(self)
+        self.__last_view_id = self.__id
+    
+
+    @property
+    def bold (self):
+        return self.__bold
+    
+    @bold.setter
+    def bold (self, value:bool):
+        if self.__mother_view == None:
+            raise Exception("Cannot change the sub_view property while its not on the screen.")
+        
+        self.__bold = value
+        self.__id = self.__mother_view.get_new_view_id()
+        self.__mother_view.update(self)
+        self.__last_view_id = self.__id
+    
+    @property
+    def size (self):
+        return self.__size
+    
+    @size.setter
+    def size (self, value:float):
+        if self.__mother_view == None:
+            raise Exception("Cannot change the sub_view property while its not on the screen.")
+        
+        self.__size = value
+        self.__id = self.__mother_view.get_new_view_id()
+        self.__mother_view.update(self)
         self.__last_view_id = self.__id
```

### Comparing `swoopyui-1.3.1/swoopyui/views/textfield.py` & `swoopyui-1.4/swoopyui/views/textfield.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.3.1/swoopyui.egg-info/PKG-INFO` & `swoopyui-1.4/swoopyui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: swoopyui
-Version: 1.3.1
+Version: 1.4
 Summary: A python library that allow you to build swiftUI apps using python.
 Home-page: https://github.com/SKbarbon/swoopyui
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # swoopyui
 A simple python library that allow you to build swiftUI apps using python.
 
 ## How does it work ?
```

### Comparing `swoopyui-1.3.1/swoopyui.egg-info/SOURCES.txt` & `swoopyui-1.4/swoopyui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 swoopyui.egg-info/dependency_links.txt
 swoopyui.egg-info/requires.txt
 swoopyui.egg-info/top_level.txt
 swoopyui/UIkits/__init__.py
 swoopyui/assets/__init__.py
 swoopyui/assets/swoopyui.zip
 swoopyui/tools/__init__.py
+swoopyui/tools/check_if_mac.py
 swoopyui/tools/on_action.py
+swoopyui/tools/pyinstaller_check.py
 swoopyui/tools/run_swiftUI.py
 swoopyui/tools/run_target.py
 swoopyui/tools/unzip_assets.py
 swoopyui/views/__init__.py
 swoopyui/views/button.py
 swoopyui/views/navigationlink.py
 swoopyui/views/navigationstack.py
 swoopyui/views/navigationview.py
+swoopyui/views/scrollview.py
+swoopyui/views/stack.py
 swoopyui/views/text.py
 swoopyui/views/textfield.py
```

