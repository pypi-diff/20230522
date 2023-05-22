# Comparing `tmp/julienne-0.7.1.tar.gz` & `tmp/julienne-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julienne-0.7.1.tar", last modified: Fri Mar 17 19:30:45 2023, max compression
+gzip compressed data, was "julienne-0.8.0.tar", last modified: Mon May 22 14:52:43 2023, max compression
```

## Comparing `julienne-0.7.1.tar` & `julienne-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-17 19:30:45.216044 julienne-0.7.1/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1076 2022-10-24 19:55:49.000000 julienne-0.7.1/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11790 2023-03-17 19:30:45.216189 julienne-0.7.1/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)    10930 2023-03-17 15:51:25.000000 julienne-0.7.1/README.rst
--rw-r--r--   0 ctrudeau   (501) staff       (20)       90 2022-10-24 20:30:47.000000 julienne-0.7.1/pyproject.toml
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1220 2023-03-17 19:30:45.217090 julienne-0.7.1/setup.cfg
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-17 19:30:45.189019 julienne-0.7.1/src/
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-17 19:30:45.212480 julienne-0.7.1/src/julienne/
--rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-03-17 19:30:21.000000 julienne-0.7.1/src/julienne/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1108 2023-01-18 21:54:41.000000 julienne-0.7.1/src/julienne/cmd.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    10293 2023-03-17 19:22:10.000000 julienne-0.7.1/src/julienne/filemodel.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6862 2023-03-17 17:50:58.000000 julienne-0.7.1/src/julienne/nodes.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    13022 2023-03-17 19:21:18.000000 julienne-0.7.1/src/julienne/parsers.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-17 19:30:45.214805 julienne-0.7.1/src/julienne.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11790 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      442 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       43 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/entry_points.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)      136 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/requires.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-03-17 19:30:45.000000 julienne-0.7.1/src/julienne.egg-info/top_level.txt
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-03-17 19:30:45.215801 julienne-0.7.1/tests/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2523 2023-03-17 19:24:24.000000 julienne-0.7.1/tests/test_files.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5466 2023-03-17 18:56:03.000000 julienne-0.7.1/tests/test_pparser.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5219 2023-03-17 19:21:41.000000 julienne-0.7.1/tests/test_xparser.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.800991 julienne-0.8.0/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1076 2022-10-24 19:55:49.000000 julienne-0.8.0/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-05-22 14:52:43.801135 julienne-0.8.0/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11087 2023-05-22 14:47:13.000000 julienne-0.8.0/README.rst
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       90 2022-10-24 20:30:47.000000 julienne-0.8.0/pyproject.toml
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1220 2023-05-22 14:52:43.801977 julienne-0.8.0/setup.cfg
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.695540 julienne-0.8.0/src/
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.796324 julienne-0.8.0/src/julienne/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-05-22 14:38:20.000000 julienne-0.8.0/src/julienne/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1897 2023-03-17 20:26:54.000000 julienne-0.8.0/src/julienne/cmd.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11708 2023-03-17 21:00:23.000000 julienne-0.8.0/src/julienne/filemodel.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6862 2023-03-17 20:27:23.000000 julienne-0.8.0/src/julienne/nodes.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    13488 2023-05-22 14:47:51.000000 julienne-0.8.0/src/julienne/parsers.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.799358 julienne-0.8.0/src/julienne.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      442 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       43 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/entry_points.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      136 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/requires.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/top_level.txt
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.800625 julienne-0.8.0/tests/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2523 2023-03-17 19:24:24.000000 julienne-0.8.0/tests/test_files.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5466 2023-05-22 14:48:15.000000 julienne-0.8.0/tests/test_pparser.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5218 2023-05-22 14:49:19.000000 julienne-0.8.0/tests/test_xparser.py
```

### Comparing `julienne-0.7.1/LICENSE` & `julienne-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `julienne-0.7.1/PKG-INFO` & `julienne-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julienne
-Version: 0.7.1
+Version: 0.8.0
 Summary: Splits code into copies based on version numbers in comments
 Home-page: https://github.com/cltrudeau/julienne
 Author: Christopher Trudeau
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -30,15 +30,15 @@
 showing progress to your students as you introduce new concepts. Keeping
 several versions is painful though, especially when you find a bug that is
 common to each copy.
 
 Enter: julienne. It slices, it dices, well... it actually only slices. This
 library comes with the ``juli`` script which reads code and interprets special
 directives in the comments, generating multiple versions of the code. The
-directives allow you to limit which versions a block of code exists in. 
+directives allow you to limit which versions a block of code exists in.
 
 The goal for this toolset once complete is to allow you to maintain a single
 version of your project in its completed state. Running ``juli`` on your
 project will generate a separate copy of each version of your code.
 
 
 Juli Comment Markers
@@ -90,14 +90,15 @@
 
 * ``#@=`` -- A single line conditional to a range of chapters, comment after the code
 * ``#@@`` -- Single line conditional to a range where code is commented out
 * ``#@+`` -- Start a conditional block that is commented out, applies to a range of chapters
 * ``#@-`` -- Part of a conditional block that is commented out. Must appear after a ``#@+``
 * ``#@[`` -- Start a conditional block that is not commented out, applies to a range of chapters
 * ``#@]`` -- End a conditional block that is not commented. Must appear after a ``#@[``
+* ``#@*`` -- A julienne comment, one not included in the output code
 
 The ``#@=``, ``#@@`, ``#@+``, and ``#@[`` markers expect a range that
 indicates what chapters a line or block participates within. Ranges can
 indicate a single chapter, a range of chapters, up-to-and-including a chapter,
 and including-and-after a chapter. A space is expected between the julienne
 type and the beginning of the range specifier. Example ranges:
 
@@ -117,15 +118,15 @@
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
     b = "In chapters 1-3"   # comment on conditional
-    c = "In chapters 1-2"   
+    c = "In chapters 1-2"
 
     x = "In chapters 1-2"
 
     for x in range(10):
         # block header with comment
         g= "In chapters 1 and 2"
         h = "In all chapters"
@@ -134,15 +135,15 @@
 Chapter four would contain:
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
-    d = "In chapters 2 on"  
+    d = "In chapters 2 on"
 
     e = "In chapters 3 to 4"  # inline comment
     f = "  as a block"
 
     for x in range(10):
         h = "In all chapters"
 
@@ -164,14 +165,15 @@
 follows:
 
 * ``<!--@= 1-3 comment -->`` -- Inline marker, anything appearing before this on the line is included in the range.
 * ``<!--@+ 1-3 comment`` -- Opening for a block. Subsequent lines between this and the closing marker are conditional.
 * ``@+-->`` -- Closing for a block, must be paired with an opening
 * ``<!--@[ 1-3 comment -->`` -- opening for a block that is not commented out, all content until the matching closing marker is conditional
 * ``<!--@] -->`` -- closing maker for a block
+* ``<!--@* -->`` -- a julienne comment, one not included in the output code, **only use on a single line!**
 
 The same kinds of range specifiers are supported as Python-style (3, 1-3, 1-,
 and -3). Any additional text found in a comment marker is added as a comment
 in the result. If there is no additional comment in the marker, there is no
 corresponding line in the result.
 
 
@@ -179,25 +181,25 @@
 ========================
 
 The ``juli`` uses a `TOML <https://toml.io>`_ file for configuration. The file
 must contain two key/value pairs that indicate the source and output
 directories for the parser.
 
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
 
 
-The above will cause ``juli`` to look for a directory named ``code`` relative 
-to the configuration file. The source found in that directory will be parsed. 
+The above will cause ``juli`` to look for a directory named ``code`` relative
+to the configuration file. The source found in that directory will be parsed.
 The generated chapters will be put in a directory named ``last_output``. If
-your source specified two chapters, running ``juli`` will result in the 
-creation of two directories: ``last_output/ch1/code`` and 
+your source specified two chapters, running ``juli`` will result in the
+creation of two directories: ``last_output/ch1/code`` and
 ``last_output/ch2/code``.
 
 Both the ``output_dir`` and ``src_dir`` values can be absolute paths or
 relative to the TOML configuration file.
 
 Additional, optional configuration values are:
 
@@ -209,15 +211,15 @@
 * ``skip_dirs`` -- A list of sub-directories that should not be processed.
 * ``skip_patterns`` -- A list of strings that if they show up in the path the path is ignored. Useful for things like `__pycache__`
 * ``[chapter_map]`` -- Chapter numbers are integers, but you may not always want that in your output structure. This map allows you to change the suffix part of a chapter directory name. Keys in the map are the chapter numbers while values are what should be used in the chapter suffix.
 * ``[ranged_files.XYZ]`` -- Files or directories can be marked as conditional using this TOML map. This map must specify ``range`` and ``files`` attributes. The ``range`` attribute indicates what chapters this directory participates in, and ``files`` is listing of file or directory names. In the case of files they will only participate in parsing if the match the range value. If a file contains a marker outside the range it will be ignored. The ``XYZ`` portion of the TOML nested map is ignored, it is there so you can have multiple conditional directories.
 
 Here is a full example of a configuration file:
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
     skip_dirs = ['bad_dir', ]
     skip_patterns = ['__pycache__', ]
 
     chapter_prefix = "chap"
@@ -229,15 +231,15 @@
     [ranged_files.foo]
     range = '2-4'
     files = ['code/between24', 'only24.py']
 
     [ranged_files.bar]
     range = '4-'
     files = ['code/after4', ]
-        
+
 
 If your code directory contained:
 
 .. code-block:: text
 
     code/script.py
     code/only24.py
```

### Comparing `julienne-0.7.1/README.rst` & `julienne-0.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 showing progress to your students as you introduce new concepts. Keeping
 several versions is painful though, especially when you find a bug that is
 common to each copy.
 
 Enter: julienne. It slices, it dices, well... it actually only slices. This
 library comes with the ``juli`` script which reads code and interprets special
 directives in the comments, generating multiple versions of the code. The
-directives allow you to limit which versions a block of code exists in. 
+directives allow you to limit which versions a block of code exists in.
 
 The goal for this toolset once complete is to allow you to maintain a single
 version of your project in its completed state. Running ``juli`` on your
 project will generate a separate copy of each version of your code.
 
 
 Juli Comment Markers
@@ -68,14 +68,15 @@
 
 * ``#@=`` -- A single line conditional to a range of chapters, comment after the code
 * ``#@@`` -- Single line conditional to a range where code is commented out
 * ``#@+`` -- Start a conditional block that is commented out, applies to a range of chapters
 * ``#@-`` -- Part of a conditional block that is commented out. Must appear after a ``#@+``
 * ``#@[`` -- Start a conditional block that is not commented out, applies to a range of chapters
 * ``#@]`` -- End a conditional block that is not commented. Must appear after a ``#@[``
+* ``#@*`` -- A julienne comment, one not included in the output code
 
 The ``#@=``, ``#@@`, ``#@+``, and ``#@[`` markers expect a range that
 indicates what chapters a line or block participates within. Ranges can
 indicate a single chapter, a range of chapters, up-to-and-including a chapter,
 and including-and-after a chapter. A space is expected between the julienne
 type and the beginning of the range specifier. Example ranges:
 
@@ -95,15 +96,15 @@
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
     b = "In chapters 1-3"   # comment on conditional
-    c = "In chapters 1-2"   
+    c = "In chapters 1-2"
 
     x = "In chapters 1-2"
 
     for x in range(10):
         # block header with comment
         g= "In chapters 1 and 2"
         h = "In all chapters"
@@ -112,15 +113,15 @@
 Chapter four would contain:
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
-    d = "In chapters 2 on"  
+    d = "In chapters 2 on"
 
     e = "In chapters 3 to 4"  # inline comment
     f = "  as a block"
 
     for x in range(10):
         h = "In all chapters"
 
@@ -142,14 +143,15 @@
 follows:
 
 * ``<!--@= 1-3 comment -->`` -- Inline marker, anything appearing before this on the line is included in the range.
 * ``<!--@+ 1-3 comment`` -- Opening for a block. Subsequent lines between this and the closing marker are conditional.
 * ``@+-->`` -- Closing for a block, must be paired with an opening
 * ``<!--@[ 1-3 comment -->`` -- opening for a block that is not commented out, all content until the matching closing marker is conditional
 * ``<!--@] -->`` -- closing maker for a block
+* ``<!--@* -->`` -- a julienne comment, one not included in the output code, **only use on a single line!**
 
 The same kinds of range specifiers are supported as Python-style (3, 1-3, 1-,
 and -3). Any additional text found in a comment marker is added as a comment
 in the result. If there is no additional comment in the marker, there is no
 corresponding line in the result.
 
 
@@ -157,25 +159,25 @@
 ========================
 
 The ``juli`` uses a `TOML <https://toml.io>`_ file for configuration. The file
 must contain two key/value pairs that indicate the source and output
 directories for the parser.
 
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
 
 
-The above will cause ``juli`` to look for a directory named ``code`` relative 
-to the configuration file. The source found in that directory will be parsed. 
+The above will cause ``juli`` to look for a directory named ``code`` relative
+to the configuration file. The source found in that directory will be parsed.
 The generated chapters will be put in a directory named ``last_output``. If
-your source specified two chapters, running ``juli`` will result in the 
-creation of two directories: ``last_output/ch1/code`` and 
+your source specified two chapters, running ``juli`` will result in the
+creation of two directories: ``last_output/ch1/code`` and
 ``last_output/ch2/code``.
 
 Both the ``output_dir`` and ``src_dir`` values can be absolute paths or
 relative to the TOML configuration file.
 
 Additional, optional configuration values are:
 
@@ -187,15 +189,15 @@
 * ``skip_dirs`` -- A list of sub-directories that should not be processed.
 * ``skip_patterns`` -- A list of strings that if they show up in the path the path is ignored. Useful for things like `__pycache__`
 * ``[chapter_map]`` -- Chapter numbers are integers, but you may not always want that in your output structure. This map allows you to change the suffix part of a chapter directory name. Keys in the map are the chapter numbers while values are what should be used in the chapter suffix.
 * ``[ranged_files.XYZ]`` -- Files or directories can be marked as conditional using this TOML map. This map must specify ``range`` and ``files`` attributes. The ``range`` attribute indicates what chapters this directory participates in, and ``files`` is listing of file or directory names. In the case of files they will only participate in parsing if the match the range value. If a file contains a marker outside the range it will be ignored. The ``XYZ`` portion of the TOML nested map is ignored, it is there so you can have multiple conditional directories.
 
 Here is a full example of a configuration file:
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
     skip_dirs = ['bad_dir', ]
     skip_patterns = ['__pycache__', ]
 
     chapter_prefix = "chap"
@@ -207,15 +209,15 @@
     [ranged_files.foo]
     range = '2-4'
     files = ['code/between24', 'only24.py']
 
     [ranged_files.bar]
     range = '4-'
     files = ['code/after4', ]
-        
+
 
 If your code directory contained:
 
 .. code-block:: text
 
     code/script.py
     code/only24.py
```

### Comparing `julienne-0.7.1/setup.cfg` & `julienne-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `julienne-0.7.1/src/julienne/filemodel.py` & `julienne-0.8.0/src/julienne/filemodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,31 @@
     for child in node.children:
         if isinstance(child, DirNode) and child.should_traverse(chapter):
             _traverse(chapter, child, cmd, *args)
         else:
             fn = getattr(child, cmd)
             fn(*args)
 
+
+def _walk_node(node):
+    if isinstance(node, DirNode):
+        for child in node.children:
+            yield from _walk_node(child)
+    else:
+        yield node
+
+
+def _print_node_contents(node):
+    print("***", node.path)
+    if isinstance(node, _BaseFileNode):
+        for line in node.parser.lines:
+            lower = '*' if line.lower is None else str(line.lower)
+            upper = '*' if line.upper is None else str(line.upper)
+            print(f"{lower:>2}-{upper:2} |", line.content)
+
 # ===========================================================================
 # File Tree
 # ===========================================================================
 
 class FileTree:
     def __init__(self, config, base_path, base_dir, verbose=False):
         self.base_path = base_path
@@ -210,15 +227,15 @@
             _traverse(num, self.root, 'copy', num, parent_path, output_path)
 
 # ===========================================================================
 # File Generation
 # ===========================================================================
 
 def generate_files(config_file, verbose=False, info_only=False, 
-        single_chapter=None):
+        single_chapter=None, debug=''):
     path = Path(config_file)
     path.resolve()
     base_path = path.parent
 
     config = tomli.loads(path.read_text())
 
     # Check for / create output directory
@@ -240,14 +257,26 @@
     if info_only:
         # If only showing info force verbose
         verbose = True
 
     # Build the tree and then generate the output
     tree = FileTree(config, base_path, base_dir, verbose)
 
+    if debug:
+        # Debug mode, show all the line info for everything in matching files
+        match = False
+        for node in _walk_node(tree.root):
+            if debug in str(node.path):
+                match = True
+                _print_node_contents(node)
+
+        if not match:
+            print(f"!!! No file name matching *{debug}*")
+        exit()
+
     if info_only:
         # Don't generate chapters, you're done
         print('\nLargest chapter detected', tree.biggest)
         print('\n**Info only, no chapters generated**')
         exit()
 
     # Optionally remove the output directory before processing
@@ -269,7 +298,26 @@
             import black    # import only if being used
             black.main()
         except SystemExit:
             # black calls quit(), ignore it
             pass
 
     return tree
+
+# ===========================================================================
+# File Display
+# ===========================================================================
+
+def display_pound_files(files):
+    for filename in files:
+        path = Path(filename)
+        node = PoundFileNode(path)
+        node.parse_file()
+        _print_node_contents(node)
+
+
+def display_xml_files(files):
+    for filename in files:
+        path = Path(filename)
+        node = XMLFileNode(path)
+        node.parse_file()
+        _print_node_contents(node)
```

### Comparing `julienne-0.7.1/src/julienne/nodes.py` & `julienne-0.8.0/src/julienne/nodes.py`

 * *Files identical despite different names*

### Comparing `julienne-0.7.1/src/julienne/parsers.py` & `julienne-0.8.0/src/julienne/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # ===========================================================================
 
 ParseMode = Enum('ParseMode', ['NORMAL', 'BLOCK_COMMENT', 'BLOCK_OPEN'])
 
 Marker = namedtuple('Marker', ["jtype", "lower", "upper", "comment"])
 
-ALL_JTYPES = ('@', '=', '+', '-', '[', ']')
+ALL_JTYPES = ('@', '=', '+', '-', '[', ']', '*')
 RANGED_JTYPES = ('@', '=', '+', '[')
 
 # ===========================================================================
 
 class Parser:
     CONTENT_TYPES = Enum('ParserContentTypes', ['POUND', 'XML'])
 
@@ -93,15 +93,15 @@
             else:
                 if line.lower is not None and line.lower > biggest:
                     biggest = line.lower
                 elif line.upper is not None and line.upper > biggest:
                     biggest = line.upper
 
         return bottom, top, biggest
-            
+
 # ===========================================================================
 
 chapter_in_range = lambda chapter, conditional, lower, upper: \
     not conditional or (upper is None and lower <= chapter) or \
         (lower <= chapter <= upper)
 
 
@@ -209,21 +209,27 @@
         index = text.find("#@")
         if index == -1:
             if parser.mode == ParseMode.BLOCK_OPEN:
                 # Inside an open block, add conditional line based on parent
                 parent = parser.parent_marker
                 parser.add_line(text, True, parent.lower, parent.upper)
             else:
-                # No juli comment, keep the line unconditionally
-                parser.add_line(text, False, None, None)
-                parser.all_conditional = False
-
+                # No juli comment, could be closing the block
                 if parser.mode == ParseMode.BLOCK_COMMENT:
                     parser.close_nest()
 
+                if len(parser.stack) == 1:
+                    # Not nested, keep the line unconditionally
+                    parser.add_line(text, False, None, None)
+                    parser.all_conditional = False
+                else:
+                    # Nested, keep the line using parent's conditions
+                    parent = parser.parent_marker
+                    parser.add_line(text, True, parent.lower, parent.upper)
+
             continue
 
         # Found a conditional line, behaviour changes based on the type of
         # conditional
         line_text = ''
         marker = parse_marker(text[index+2:], line_no)
 
@@ -261,26 +267,27 @@
                 error = (f"Block marker found without header on line "
                     f"{line_no} *{text}*")
                 raise ValueError(error)
 
             # Remove the "#@- " token from the text, preserve any leading
             # spaces
             line_text = text[0:index] + text[index+4:]
-
-            if line_text:
-                parent = parser.parent_marker
-                parser.add_line(line_text, True, parent.lower, parent.upper)
+            parent = parser.parent_marker
+            parser.add_line(line_text, True, parent.lower, parent.upper)
         elif marker.jtype == '[':
-            # Header for an open block 
+            # Header for an open block
             parser.nest(ParseMode.BLOCK_OPEN, marker)
             parser.add_if_commented(text, index, marker)
         elif marker.jtype == ']':
             # Closing marker for open blocks, reset to normal
             parser.close_nest()
             parser.add_if_commented(text, index, marker)
+        elif marker.jtype == '*':
+            # Juli comment, do nothing
+            pass
 
     return parser
 
 # ---------------------------------------------------------------------------
 # XML Style parser
 
 def parse_xml_content(content):
@@ -355,16 +362,19 @@
             parser.nest(ParseMode.BLOCK_COMMENT, marker)
             parser.add_if_commented(text, index, marker)
         elif marker.jtype == '-':
             error = ("Unsupported marker type '-' for XML doc on line"
                 f"{line_no} *{text}*")
             raise ValueError(error)
         elif marker.jtype == '[':
-            # Header for an open block 
+            # Header for an open block
             parser.nest(ParseMode.BLOCK_OPEN, marker)
             parser.add_if_commented(text, index, marker)
         elif marker.jtype == ']':
             # Closing marker for open blocks, reset to normal
             parser.close_nest()
             parser.add_if_commented(text, index, marker)
+        elif marker.jtype == '*':
+            # Juli comment, do nothing
+            pass
 
     return parser
```

### Comparing `julienne-0.7.1/src/julienne.egg-info/PKG-INFO` & `julienne-0.8.0/src/julienne.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julienne
-Version: 0.7.1
+Version: 0.8.0
 Summary: Splits code into copies based on version numbers in comments
 Home-page: https://github.com/cltrudeau/julienne
 Author: Christopher Trudeau
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -30,15 +30,15 @@
 showing progress to your students as you introduce new concepts. Keeping
 several versions is painful though, especially when you find a bug that is
 common to each copy.
 
 Enter: julienne. It slices, it dices, well... it actually only slices. This
 library comes with the ``juli`` script which reads code and interprets special
 directives in the comments, generating multiple versions of the code. The
-directives allow you to limit which versions a block of code exists in. 
+directives allow you to limit which versions a block of code exists in.
 
 The goal for this toolset once complete is to allow you to maintain a single
 version of your project in its completed state. Running ``juli`` on your
 project will generate a separate copy of each version of your code.
 
 
 Juli Comment Markers
@@ -90,14 +90,15 @@
 
 * ``#@=`` -- A single line conditional to a range of chapters, comment after the code
 * ``#@@`` -- Single line conditional to a range where code is commented out
 * ``#@+`` -- Start a conditional block that is commented out, applies to a range of chapters
 * ``#@-`` -- Part of a conditional block that is commented out. Must appear after a ``#@+``
 * ``#@[`` -- Start a conditional block that is not commented out, applies to a range of chapters
 * ``#@]`` -- End a conditional block that is not commented. Must appear after a ``#@[``
+* ``#@*`` -- A julienne comment, one not included in the output code
 
 The ``#@=``, ``#@@`, ``#@+``, and ``#@[`` markers expect a range that
 indicates what chapters a line or block participates within. Ranges can
 indicate a single chapter, a range of chapters, up-to-and-including a chapter,
 and including-and-after a chapter. A space is expected between the julienne
 type and the beginning of the range specifier. Example ranges:
 
@@ -117,15 +118,15 @@
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
     b = "In chapters 1-3"   # comment on conditional
-    c = "In chapters 1-2"   
+    c = "In chapters 1-2"
 
     x = "In chapters 1-2"
 
     for x in range(10):
         # block header with comment
         g= "In chapters 1 and 2"
         h = "In all chapters"
@@ -134,15 +135,15 @@
 Chapter four would contain:
 
 .. code-block:: python
 
     # This is a sample file
 
     a = "In all chapters"   # inline comment
-    d = "In chapters 2 on"  
+    d = "In chapters 2 on"
 
     e = "In chapters 3 to 4"  # inline comment
     f = "  as a block"
 
     for x in range(10):
         h = "In all chapters"
 
@@ -164,14 +165,15 @@
 follows:
 
 * ``<!--@= 1-3 comment -->`` -- Inline marker, anything appearing before this on the line is included in the range.
 * ``<!--@+ 1-3 comment`` -- Opening for a block. Subsequent lines between this and the closing marker are conditional.
 * ``@+-->`` -- Closing for a block, must be paired with an opening
 * ``<!--@[ 1-3 comment -->`` -- opening for a block that is not commented out, all content until the matching closing marker is conditional
 * ``<!--@] -->`` -- closing maker for a block
+* ``<!--@* -->`` -- a julienne comment, one not included in the output code, **only use on a single line!**
 
 The same kinds of range specifiers are supported as Python-style (3, 1-3, 1-,
 and -3). Any additional text found in a comment marker is added as a comment
 in the result. If there is no additional comment in the marker, there is no
 corresponding line in the result.
 
 
@@ -179,25 +181,25 @@
 ========================
 
 The ``juli`` uses a `TOML <https://toml.io>`_ file for configuration. The file
 must contain two key/value pairs that indicate the source and output
 directories for the parser.
 
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
 
 
-The above will cause ``juli`` to look for a directory named ``code`` relative 
-to the configuration file. The source found in that directory will be parsed. 
+The above will cause ``juli`` to look for a directory named ``code`` relative
+to the configuration file. The source found in that directory will be parsed.
 The generated chapters will be put in a directory named ``last_output``. If
-your source specified two chapters, running ``juli`` will result in the 
-creation of two directories: ``last_output/ch1/code`` and 
+your source specified two chapters, running ``juli`` will result in the
+creation of two directories: ``last_output/ch1/code`` and
 ``last_output/ch2/code``.
 
 Both the ``output_dir`` and ``src_dir`` values can be absolute paths or
 relative to the TOML configuration file.
 
 Additional, optional configuration values are:
 
@@ -209,15 +211,15 @@
 * ``skip_dirs`` -- A list of sub-directories that should not be processed.
 * ``skip_patterns`` -- A list of strings that if they show up in the path the path is ignored. Useful for things like `__pycache__`
 * ``[chapter_map]`` -- Chapter numbers are integers, but you may not always want that in your output structure. This map allows you to change the suffix part of a chapter directory name. Keys in the map are the chapter numbers while values are what should be used in the chapter suffix.
 * ``[ranged_files.XYZ]`` -- Files or directories can be marked as conditional using this TOML map. This map must specify ``range`` and ``files`` attributes. The ``range`` attribute indicates what chapters this directory participates in, and ``files`` is listing of file or directory names. In the case of files they will only participate in parsing if the match the range value. If a file contains a marker outside the range it will be ignored. The ``XYZ`` portion of the TOML nested map is ignored, it is there so you can have multiple conditional directories.
 
 Here is a full example of a configuration file:
 
-.. code-block:: TOML 
+.. code-block:: TOML
 
     output_dir = 'last_output'
     src_dir = 'code'
     skip_dirs = ['bad_dir', ]
     skip_patterns = ['__pycache__', ]
 
     chapter_prefix = "chap"
@@ -229,15 +231,15 @@
     [ranged_files.foo]
     range = '2-4'
     files = ['code/between24', 'only24.py']
 
     [ranged_files.bar]
     range = '4-'
     files = ['code/after4', ]
-        
+
 
 If your code directory contained:
 
 .. code-block:: text
 
     code/script.py
     code/only24.py
```

### Comparing `julienne-0.7.1/tests/test_files.py` & `julienne-0.8.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `julienne-0.7.1/tests/test_pparser.py` & `julienne-0.8.0/tests/test_pparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 self.assertIn(str(num), line.content)
 
     def test_bad_parsing(self):
         text = 'x = 3 #@'
         with self.assertRaises(ValueError):
             parse_pound_content(text)
 
-        text = 'x = 3 #@*'
+        text = 'x = 3 #@!'
         with self.assertRaises(ValueError):
             parse_pound_content(text)
 
     def test_block_parsing(self):
         #--- Test a conditional block
         parser = parse_pound_content(CODE_BLOCK1)
         self.assertParser(parser, True, EXPECTED_BLOCK1, 3, 4)
```

### Comparing `julienne-0.7.1/tests/test_xparser.py` & `julienne-0.8.0/tests/test_xparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 self.assertIn(str(num), line.content)
 
     def test_bad_parsing(self):
         text = 'x = 3 <!--@ -->'
         with self.assertRaises(ValueError):
             parse_xml_content(text)
 
-        text = 'x = 3 <!--@* -->'
+        text = 'x = 3 <!--@! -->'
         with self.assertRaises(ValueError):
             parse_xml_content(text)
 
     def test_block_parsing(self):
         #--- Test a conditional block
         parser = parse_xml_content(BLOCK1)
         self.assertParser(parser, True, EXPECTED_BLOCK1, 3, 4)
@@ -157,15 +157,15 @@
         with noted_raise("[chapter={chapter}]"):
             for chapter in range(1, 4):
                 content = parser.lines[0].get_content(chapter)
                 self.assertIsNotNone(content)
                 content = parser.lines[3].get_content(chapter)
                 self.assertIsNotNone(content)
 
-                # Line[1] and Line[2] are conditional, showing in 
+                # Line[1] and Line[2] are conditional, showing in
                 # chapters 1-2 only
                 if chapter <= 2:
                     content = parser.lines[1].get_content(chapter)
                     self.assertIsNotNone(content)
                     content = parser.lines[2].get_content(chapter)
                     self.assertIsNotNone(content)
                 else:
```

