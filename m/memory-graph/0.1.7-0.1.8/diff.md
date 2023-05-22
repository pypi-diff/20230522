# Comparing `tmp/memory_graph-0.1.7.tar.gz` & `tmp/memory_graph-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.7.tar", last modified: Sun May 21 17:25:36 2023, max compression
+gzip compressed data, was "memory_graph-0.1.8.tar", last modified: Mon May 22 07:56:15 2023, max compression
```

## Comparing `memory_graph-0.1.7.tar` & `memory_graph-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.7/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.7/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-21 17:25:36.443849 memory_graph-0.1.7/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4366 2023-05-20 18:13:48.000000 memory_graph-0.1.7/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.7/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1190 2023-05-21 17:24:25.000000 memory_graph-0.1.7/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5216 2023-05-21 17:18:14.000000 memory_graph-0.1.7/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4498 2023-05-20 18:49:23.000000 memory_graph-0.1.7/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1142 2023-05-20 17:02:48.000000 memory_graph-0.1.7/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.7/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-21 17:25:36.443849 memory_graph-0.1.7/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-21 17:24:38.000000 memory_graph-0.1.7/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.8/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.8/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 07:56:15.214232 memory_graph-0.1.8/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4696 2023-05-22 07:47:22.000000 memory_graph-0.1.8/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.8/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      865 2023-05-22 07:55:43.000000 memory_graph-0.1.8/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5234 2023-05-21 18:05:01.000000 memory_graph-0.1.8/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4288 2023-05-22 07:48:47.000000 memory_graph-0.1.8/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1098 2023-05-22 07:43:38.000000 memory_graph-0.1.8/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.8/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 07:56:15.214232 memory_graph-0.1.8/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-22 07:56:15.000000 memory_graph-0.1.8/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-22 07:56:15.214232 memory_graph-0.1.8/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-22 07:55:56.000000 memory_graph-0.1.8/setup.py
```

### Comparing `memory_graph-0.1.7/LICENSE.txt` & `memory_graph-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.7/PKG-INFO` & `memory_graph-0.1.8/memory_graph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: memory_graph
-Version: 0.1.7
+Name: memory-graph
+Version: 0.1.8
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -43,21 +43,21 @@
 ```
 
 ## Graph all Local Variables ##
 
 Often it is useful to graph all the local variables using:
 
 ```
-memory_graph.show( memory_graph.filter(locals()) )
+memory_graph.show( locals(), block=True )
 ```
 
 Also useful to set as 'watch' in a debugger tool:
 
 ```
-memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+memory_graph.render( locals(), "my_debug_graph.pdf" )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -104,46 +104,50 @@
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
 - ***memory_graph.graphviz_nodes.uncategorized_color*** : string
   - color used for uncategorized types
+- ***memory_graph.graphviz_nodes.padding*** : int
+  - amount of padding for node cells
+- ***memory_graph.graphviz_nodes.spacing*** : int
+  - amount of spacing for node cells
 
 See for color names: [graphviz colors](https://graphviz.org/doc/info/colors.html)
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config Node Structure, rewrite_to_node ###
+### Config Graph Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
-  - the types we copy to a node instead of drawing a reference to it
+  - the types we add to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict/mappingproxy) for classes
+  - determines if we reduce the reference (to dictionary) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
+- ***memory_graph.rewrite.ignore_types*** : set
+  - all types that we ignore, these will not be in the graph
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
-  - all types rewritten to node as dictionary values (dict)
-- ***memory_graph.rewrite.mappingproxy_types*** : set
-  - all types rewritten to node as mappingproxy values (mappingproxy)
-- ***memory_graph.rewrite.mappingproxy_ignore_dunder_keys*** : bool
-  - determines if we ignore dunder keys ('`__example__`') in mappingproxy
+  - all types rewritten to node as dictionary values (dict, mappingproxy)
+- ***memory_graph.rewrite.dict_ignore_dunder_keys*** : bool
+  - determines if we ignore dunder keys ('`__example`') in dict_types
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
@@ -151,14 +155,22 @@
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
+## Troubleshooting ##
+
+When edges overlap it can be hard to distinguish them. Using an
+interactive graphviz viewer, such as
+[xdot](https://github.com/jrfonseca/xdot.py), on a '*.gv' output file
+will help.
+
+
 ## Author ##
 Bas Terwijn
 
 
 ## Inspiration ##
 Inspired by [PythonTutor](https://pythontutor.com/visualize.html).
```

### Comparing `memory_graph-0.1.7/README.md` & `memory_graph-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 ```
 
 ## Graph all Local Variables ##
 
 Often it is useful to graph all the local variables using:
 
 ```
-memory_graph.show( memory_graph.filter(locals()) )
+memory_graph.show( locals(), block=True )
 ```
 
 Also useful to set as 'watch' in a debugger tool:
 
 ```
-memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+memory_graph.render( locals(), "my_debug_graph.pdf" )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -87,46 +87,50 @@
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
 - ***memory_graph.graphviz_nodes.uncategorized_color*** : string
   - color used for uncategorized types
+- ***memory_graph.graphviz_nodes.padding*** : int
+  - amount of padding for node cells
+- ***memory_graph.graphviz_nodes.spacing*** : int
+  - amount of spacing for node cells
 
 See for color names: [graphviz colors](https://graphviz.org/doc/info/colors.html)
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config Node Structure, rewrite_to_node ###
+### Config Graph Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
-  - the types we copy to a node instead of drawing a reference to it
+  - the types we add to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict/mappingproxy) for classes
+  - determines if we reduce the reference (to dictionary) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
+- ***memory_graph.rewrite.ignore_types*** : set
+  - all types that we ignore, these will not be in the graph
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
-  - all types rewritten to node as dictionary values (dict)
-- ***memory_graph.rewrite.mappingproxy_types*** : set
-  - all types rewritten to node as mappingproxy values (mappingproxy)
-- ***memory_graph.rewrite.mappingproxy_ignore_dunder_keys*** : bool
-  - determines if we ignore dunder keys ('`__example__`') in mappingproxy
+  - all types rewritten to node as dictionary values (dict, mappingproxy)
+- ***memory_graph.rewrite.dict_ignore_dunder_keys*** : bool
+  - determines if we ignore dunder keys ('`__example`') in dict_types
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
@@ -134,13 +138,21 @@
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
+## Troubleshooting ##
+
+When edges overlap it can be hard to distinguish them. Using an
+interactive graphviz viewer, such as
+[xdot](https://github.com/jrfonseca/xdot.py), on a '*.gv' output file
+will help.
+
+
 ## Author ##
 Bas Terwijn
 
 
 ## Inspiration ##
 Inspired by [PythonTutor](https://pythontutor.com/visualize.html).
```

### Comparing `memory_graph-0.1.7/memory_graph/Node.py` & `memory_graph-0.1.8/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.7/memory_graph/graphviz_nodes.py` & `memory_graph-0.1.8/memory_graph/graphviz_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 layout_vertical=True
 type_category_to_color_map={
     "NoneType":"gray", "type":"lime", "bool":"pink", "int":"green", "float":"yellow", "str":"cyan", # fundamental types
     "tuple":"orange", "list":"brown1", "set":"darkolivegreen1", "frozenset":"darkolivegreen3", "dict":"royalblue1", "mappingproxy":"royalblue3", "class":"orchid" # containers
 }
 uncategorized_color="red"
 padding=0
-spacing=3
+spacing=5
 
 
 taken_children=set()
 
 def type_category_to_color(type_catergory):
     if type_catergory in type_category_to_color_map:
         return type_category_to_color_map[type_catergory]
@@ -41,27 +41,27 @@
                                          "}":  r"\}",
                                          })) # TODO
     return label
 
 def get_element_label(element):
     value=element.get_value()
     if value is None:
-        return "&nbsp;"
+        return "&nbsp;&nbsp;"
     return add_escape_chars(str(value))
 
 def build_label_line(node,border=1):
     color=type_category_to_color(get_type_category(node))
     if len(node.get_elements())>0:
         if layout_vertical:
             cells="".join( (f'<TR><TD PORT="f{index}"> {get_element_label(element)} </TD></TR>' for index,element in enumerate(node.get_elements())) )
         else:
             cells="<TR>"+ "".join( (f'<TD PORT="f{index}">{get_element_label(element)}</TD>' for index,element in enumerate(node.get_elements())) ) +"</TR>"
         table=f'<TABLE BORDER="{border}" CELLSPACING="{spacing}" CELLPADDING="{padding}">{cells}</TABLE>'
         return f'<<TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0" BGCOLOR="{color}"><TR><TD PORT="X"> {table} </TD></TR></TABLE>>'
-    return f'<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="0" BGCOLOR="{color}"><TR><TD PORT="X"> &nbsp; </TD></TR></TABLE>>'
+    return f'<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="0" BGCOLOR="{color}"><TR><TD PORT="X"> &nbsp;&nbsp; </TD></TR></TABLE>>'
     
 def build_label_key_value(node,border=1):
     color=type_category_to_color(get_type_category(node))
     if len(node.get_elements())>0:
         iterator=iter(enumerate(node.get_elements()))
         cells=""
         while True:
@@ -69,15 +69,15 @@
                 ki,k=next(iterator)
                 vi,v=next(iterator)
                 cells+=f'<TR><TD PORT="f{ki}"> {get_element_label(k)} </TD><TD PORT="f{vi}"> {get_element_label(v)} </TD></TR>'
             except StopIteration:
                 break
             table=f'<TABLE BORDER="{border}" CELLSPACING="{spacing}" CELLPADDING="{padding}" BGCOLOR="{color}">{cells}</TABLE>'
         return f'<<TABLE BORDER="0" CELLSPACING="0" CELLPADDING="0"><TR><TD PORT="X"> {table} </TD></TR></TABLE>>'
-    return f'<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="0" BGCOLOR="{color}"><TR><TD PORT="X"> &nbsp; </TD></TR></TABLE>>'
+    return f'<<TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0" CELLPADDING="0" BGCOLOR="{color}"><TR><TD PORT="X"> &nbsp;&nbsp; </TD></TR></TABLE>>'
     
 def get_node_label(node,border=1):
     if rewrite.is_dict_type(node.get_original_data()) or rewrite.is_type_with_dict(node.get_original_data()):
         return build_label_key_value(node,border)
     return build_label_line(node,border)
 
 def get_refs(node,all_nodes):
```

### Comparing `memory_graph-0.1.7/memory_graph/rewrite.py` & `memory_graph-0.1.8/memory_graph/rewrite.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from types import NoneType
-from types import MappingProxyType
+import types
 
 # the types of the values we rewrite
-
-singular_types={NoneType, bool, int, float, complex, str, range, bytes}
+ignore_types={types.FunctionType,types.ModuleType}
+singular_types={types.NoneType, bool, int, float, complex, str, range, bytes}
 linear_types={tuple, list, set, frozenset, bytearray}
-dict_types={dict}
-mappingproxy_types={MappingProxyType}
-mappingproxy_ignore_dunder_keys=True
+dict_types={dict,types.MappingProxyType}
+dict_ignore_dunder_keys=True
+
+known_types=singular_types | linear_types | dict_types | {type} # add 'type' for classes and class variables
 
-known_types=singular_types | linear_types | dict_types | mappingproxy_types | {type} # add 'type' for classes and class variables
+def is_ignore_type(value):
+    return type(value) in ignore_types
 
 def is_singular_type(value):
     return type(value) in singular_types
 
 def is_linear_type(value):
     return type(value) in linear_types
 
 def is_dict_type(value):
     return type(value) in dict_types
 
-def is_mappingproxy_type(value):
-    return type(value) in mappingproxy_types
-
 def is_known_type(value):
     return type(value) in known_types
 
 def is_type_with_dict(value):
     return has_dict_attribute(value)
 
 def is_iterable_type(value):
@@ -89,51 +87,47 @@
         return memo[identifier],True
     return memo[identifier],False
 
 def rewrite_iterable(iterable):
     new_iterable,is_just_constructed=remember_or_construct_iterable(iterable)
     if is_just_constructed:
         for i in iterable:
-            add_to_iterable_fun(new_iterable,rewrite(i))
+            if not is_ignore_type(i):
+                add_to_iterable_fun(new_iterable,rewrite(i))
     return new_iterable
 
 def rewrite_dict(dictionary):
     new_iterable,is_just_constructed=remember_or_construct_iterable(dictionary)
     if is_just_constructed:
         for key in dictionary:
-            add_to_iterable_fun(new_iterable,rewrite(key))
-            add_to_iterable_fun(new_iterable,rewrite(dictionary[key]))
-    return new_iterable
-
-def rewrite_mappingproxy(dictionary):
-    new_iterable,is_just_constructed=remember_or_construct_iterable(dictionary)
-    if is_just_constructed:
-        for key in dictionary:
-            if not mappingproxy_ignore_dunder_keys or not is_dunder_name(key):
-                add_to_iterable_fun(new_iterable,rewrite(key))
-                add_to_iterable_fun(new_iterable,rewrite(dictionary[key]))
+            if not type(key) or not is_dunder_name(key):
+                if not is_ignore_type(key):
+                    value=dictionary[key]
+                    if not is_ignore_type(value):
+                        add_to_iterable_fun(new_iterable,rewrite(key))
+                        add_to_iterable_fun(new_iterable,rewrite(value))
     return new_iterable
 
 def rewrite_object_with_dict(obj):
     new_iterable,is_just_constructed=remember_or_construct_iterable(obj)
     if is_just_constructed:
         add_to_iterable_fun(new_iterable,rewrite(get_dict_attribute(obj)))
     return new_iterable
 
 def rewrite(data):
-    if type(data) is NoneType:
-        return rewrite_singular("None") # special case, make a string because value 'None' is used for not-specified in software
+    if is_ignore_type(data):
+        rewrite_singular("ignore_type")
+    elif type(data) is types.NoneType:
+        return rewrite_singular("None") # special case, make a string because value 'None' is later used for not-specified in this software
     elif is_singular_type(data):
         return rewrite_singular(data)
     elif is_linear_type(data):
         return rewrite_iterable(data)
     elif is_dict_type(data):
         return rewrite_dict(data)
-    elif is_mappingproxy_type(data):
-        return rewrite_mappingproxy(data)
     elif is_type_with_dict(data):
         return rewrite_object_with_dict(data)
     return rewrite_singular("??"+type_name(data)+"??") # unknown type
 
 def rewrite_data(data):
     memo.clear() # forget all previous values
     return rewrite(data)
```

### Comparing `memory_graph-0.1.7/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.8/memory_graph/rewrite_to_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,16 @@
     node.add_element(Node.Element(value=data))
     return node
 
 def my_construct_iterable(data):
     return Node.Node(data)
     
 def my_add_to_iterable(iterable,data):
-    if is_duplication_type(data.get_original_data()):
-        iterable.add_elements(data.get_elements())
-    elif reduce_references_for_classes and rewrite.is_type_with_dict(iterable.get_original_data()):
+    if ( is_duplication_type(data.get_original_data()) or
+         (reduce_references_for_classes and rewrite.is_type_with_dict(iterable.get_original_data()) ):
         iterable.add_elements(data.get_elements())
     else:
         iterable.add_element(data.get_ref())
 
 rewrite.construct_singular_fun=my_construct_singular
 rewrite.construct_iterable_fun=my_construct_iterable
 rewrite.add_to_iterable_fun=my_add_to_iterable
```

### Comparing `memory_graph-0.1.7/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.8/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.7/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: memory-graph
-Version: 0.1.7
+Name: memory_graph
+Version: 0.1.8
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -43,21 +43,21 @@
 ```
 
 ## Graph all Local Variables ##
 
 Often it is useful to graph all the local variables using:
 
 ```
-memory_graph.show( memory_graph.filter(locals()) )
+memory_graph.show( locals(), block=True )
 ```
 
 Also useful to set as 'watch' in a debugger tool:
 
 ```
-memory_graph.render( memory_graph.filter(locals()), "my_debug_graph.pdf" )
+memory_graph.render( locals(), "my_debug_graph.pdf" )
 ```
 
 ## Larger Example ##
 
 This larger example shows objects that share a class (static) variable and
 also shows we can handle recursive references just fine.
 
@@ -104,46 +104,50 @@
 
 - ***memory_graph.graphviz_nodes.layout_vertical*** : bool
   - determines if list/tuple/... are drawn vertically
 - ***memory_graph.graphviz_nodes.type_category_to_color_map*** : dict
   - a mapping from type to color
 - ***memory_graph.graphviz_nodes.uncategorized_color*** : string
   - color used for uncategorized types
+- ***memory_graph.graphviz_nodes.padding*** : int
+  - amount of padding for node cells
+- ***memory_graph.graphviz_nodes.spacing*** : int
+  - amount of spacing for node cells
 
 See for color names: [graphviz colors](https://graphviz.org/doc/info/colors.html)
 
 To configure more about the visualization use:
 ```
 digraph = memory_graph.create_graph( memory_graph.filter(locals()) )
 ```
 and see the [graphviz api](https://graphviz.readthedocs.io/en/stable/api.html) to render it in many different ways.
 
-### Config Node Structure, rewrite_to_node ###
+### Config Graph Structure, rewrite_to_node ###
 
 Configure the structure of the nodes in the graph with:
 
 - ***memory_graph.rewrite_to_node.reduce_reference_types*** : set
-  - the types we copy to a node instead of drawing a reference to it
+  - the types we add to a node instead of drawing a reference to it
 - ***memory_graph.rewrite_to_node.reduce_references_for_classes*** : bool
-  - determines if we reduce the references (to dict/mappingproxy) for classes
+  - determines if we reduce the reference (to dictionary) for classes
 
 ### Config Node Creation, rewrite ###
 
 Configure what nodes are created based on reading the given data structure:
 
+- ***memory_graph.rewrite.ignore_types*** : set
+  - all types that we ignore, these will not be in the graph
 - ***memory_graph.rewrite.singular_types*** : set
   - all types rewritten to node as singular values (bool, int, float, ...)
 - ***memory_graph.rewrite.linear_types*** : set
   - all types rewritten to node as linear values (tuple, list, set, ...)
 - ***memory_graph.rewrite.dict_types*** : set
-  - all types rewritten to node as dictionary values (dict)
-- ***memory_graph.rewrite.mappingproxy_types*** : set
-  - all types rewritten to node as mappingproxy values (mappingproxy)
-- ***memory_graph.rewrite.mappingproxy_ignore_dunder_keys*** : bool
-  - determines if we ignore dunder keys ('`__example__`') in mappingproxy
+  - all types rewritten to node as dictionary values (dict, mappingproxy)
+- ***memory_graph.rewrite.dict_ignore_dunder_keys*** : bool
+  - determines if we ignore dunder keys ('`__example`') in dict_types
 
 ### Config example ###
 
 With configuration:
 ```
 memory_graph.graphviz_nodes.layout_vertical = False                       # draw lists,tuples,sets,... horizontally
 memory_graph.graphviz_nodes.type_category_to_color_map['list'] = 'yellow' # change color of 'list' type
@@ -151,14 +155,22 @@
 ```
 
 the last example looks like:
 
 ![image](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/example3.png)
 
 
+## Troubleshooting ##
+
+When edges overlap it can be hard to distinguish them. Using an
+interactive graphviz viewer, such as
+[xdot](https://github.com/jrfonseca/xdot.py), on a '*.gv' output file
+will help.
+
+
 ## Author ##
 Bas Terwijn
 
 
 ## Inspiration ##
 Inspired by [PythonTutor](https://pythontutor.com/visualize.html).
```

### Comparing `memory_graph-0.1.7/setup.py` & `memory_graph-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.7',
+    version = '0.1.8',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

