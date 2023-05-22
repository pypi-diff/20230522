# Comparing `tmp/bw_graph_tools-0.2.2.tar.gz` & `tmp/bw_graph_tools-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.2.2.tar", last modified: Mon May  8 06:16:36 2023, max compression
+gzip compressed data, was "bw_graph_tools-0.2.3.tar", last modified: Mon May 22 20:03:36 2023, max compression
```

## Comparing `bw_graph_tools-0.2.2.tar` & `bw_graph_tools-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.576629 bw_graph_tools-0.2.2/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.2/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.2/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-08 06:16:36.576688 bw_graph_tools-0.2.2/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     2290 2023-05-07 12:27:17.000000 bw_graph_tools-0.2.2/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.574410 bw_graph_tools-0.2.2/bw_graph_tools/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-05-08 06:16:12.000000 bw_graph_tools-0.2.2/bw_graph_tools/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      652 2023-05-07 12:32:09.000000 bw_graph_tools-0.2.2/bw_graph_tools/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      123 2023-05-07 12:43:29.000000 bw_graph_tools-0.2.2/bw_graph_tools/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    25891 2023-05-07 12:32:18.000000 bw_graph_tools-0.2.2/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2074 2023-05-07 12:32:31.000000 bw_graph_tools-0.2.2/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8742 2023-05-07 11:32:56.000000 bw_graph_tools-0.2.2/bw_graph_tools/matrix_tools.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1265 2023-05-08 06:15:47.000000 bw_graph_tools-0.2.2/bw_graph_tools/testing.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.2.2/bw_graph_tools/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.575209 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-08 06:16:36.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      888 2023-05-08 06:16:36.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-08 06:16:36.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      175 2023-05-08 06:16:36.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-05-08 06:16:36.000000 bw_graph_tools-0.2.2/bw_graph_tools.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.572671 bw_graph_tools-0.2.2/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.2.2/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.2/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1702 2023-05-08 06:16:36.577066 bw_graph_tools-0.2.2/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.576408 bw_graph_tools-0.2.2/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5819 2023-05-07 12:32:46.000000 bw_graph_tools-0.2.2/tests/test_first_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.2.2/tests/test_get_path_from_matrix.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1176 2023-05-07 12:33:16.000000 bw_graph_tools-0.2.2/tests/test_matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-05-07 12:33:27.000000 bw_graph_tools-0.2.2/tests/test_second_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-05-07 12:33:33.000000 bw_graph_tools-0.2.2/tests/test_third_heuristic.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 06:16:36.574171 bw_graph_tools-0.2.2/tests/traversal/
--rw-r--r--   0 chrismutel   (501) staff       (20)     7103 2023-05-08 06:12:24.000000 bw_graph_tools-0.2.2/tests/traversal/test_negative_production.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7095 2023-05-08 06:12:07.000000 bw_graph_tools-0.2.2/tests/traversal/test_nonunitary_production_with_recursion.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4550 2023-05-08 06:11:53.000000 bw_graph_tools-0.2.2/tests/traversal/test_only_one_layer.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7254 2023-05-08 06:11:38.000000 bw_graph_tools-0.2.2/tests/traversal/test_separate_production.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.177734 bw_graph_tools-0.2.3/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-22 20:03:36.177821 bw_graph_tools-0.2.3/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2290 2023-05-07 12:27:17.000000 bw_graph_tools-0.2.3/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.175410 bw_graph_tools-0.2.3/bw_graph_tools/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-05-22 19:57:10.000000 bw_graph_tools-0.2.3/bw_graph_tools/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      652 2023-05-07 12:32:09.000000 bw_graph_tools-0.2.3/bw_graph_tools/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      123 2023-05-07 12:43:29.000000 bw_graph_tools-0.2.3/bw_graph_tools/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    25891 2023-05-07 12:32:18.000000 bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2074 2023-05-07 12:32:31.000000 bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8742 2023-05-07 11:32:56.000000 bw_graph_tools-0.2.3/bw_graph_tools/matrix_tools.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1265 2023-05-08 06:15:47.000000 bw_graph_tools-0.2.3/bw_graph_tools/testing.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.2.3/bw_graph_tools/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.176319 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      928 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      183 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.173592 bw_graph_tools-0.2.3/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.2.3/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-05-22 20:03:36.178212 bw_graph_tools-0.2.3/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.177499 bw_graph_tools-0.2.3/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5819 2023-05-07 12:32:46.000000 bw_graph_tools-0.2.3/tests/test_first_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.2.3/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1176 2023-05-07 12:33:16.000000 bw_graph_tools-0.2.3/tests/test_matrix_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-05-07 12:33:27.000000 bw_graph_tools-0.2.3/tests/test_second_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-05-07 12:33:33.000000 bw_graph_tools-0.2.3/tests/test_third_heuristic.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.175151 bw_graph_tools-0.2.3/tests/traversal/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5256 2023-05-22 19:43:23.000000 bw_graph_tools-0.2.3/tests/traversal/test_marc_vd_meide.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7103 2023-05-08 06:12:24.000000 bw_graph_tools-0.2.3/tests/traversal/test_negative_production.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7095 2023-05-08 06:12:07.000000 bw_graph_tools-0.2.3/tests/traversal/test_nonunitary_production_with_recursion.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4550 2023-05-08 06:11:53.000000 bw_graph_tools-0.2.3/tests/traversal/test_only_one_layer.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7254 2023-05-08 06:11:38.000000 bw_graph_tools-0.2.3/tests/traversal/test_separate_production.py
```

### Comparing `bw_graph_tools-0.2.2/LICENSE` & `bw_graph_tools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/PKG-INFO` & `bw_graph_tools-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_graph_tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_graph_tools-0.2.2/README.md` & `bw_graph_tools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools/__init__.py` & `bw_graph_tools-0.2.3/bw_graph_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools/matrix_tools.py` & `bw_graph_tools-0.2.3/bw_graph_tools/matrix_tools.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools/testing.py` & `bw_graph_tools-0.2.3/bw_graph_tools/testing.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools.egg-info/PKG-INFO` & `bw_graph_tools-0.2.3/bw_graph_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-graph-tools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_graph_tools-0.2.2/bw_graph_tools.egg-info/SOURCES.txt` & `bw_graph_tools-0.2.3/bw_graph_tools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ./bw_graph_tools/errors.py
 ./bw_graph_tools/graph_traversal.py
 ./bw_graph_tools/graph_traversal_utils.py
 ./bw_graph_tools/matrix_tools.py
 ./bw_graph_tools/testing.py
 ./bw_graph_tools/utils.py
 ./docs/conf.py
+./tests/traversal/test_marc_vd_meide.py
 ./tests/traversal/test_negative_production.py
 ./tests/traversal/test_nonunitary_production_with_recursion.py
 ./tests/traversal/test_only_one_layer.py
 ./tests/traversal/test_separate_production.py
 bw_graph_tools/VERSION
 bw_graph_tools.egg-info/PKG-INFO
 bw_graph_tools.egg-info/SOURCES.txt
```

### Comparing `bw_graph_tools-0.2.2/docs/conf.py` & `bw_graph_tools-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/setup.cfg` & `bw_graph_tools-0.2.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 package_dir = 
 	=.
 python_requires = >=3.8
 install_requires = 
 	bw2calc >=2.0.dev13
 	matrix_utils
 	numpy
-	scikit-network
+	scikit-network ==0.30.0
 	scipy
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
```

### Comparing `bw_graph_tools-0.2.2/tests/test_first_heuristic.py` & `bw_graph_tools-0.2.3/tests/test_first_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.2.3/tests/test_get_path_from_matrix.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/test_matrix_utils.py` & `bw_graph_tools-0.2.3/tests/test_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/test_second_heuristic.py` & `bw_graph_tools-0.2.3/tests/test_second_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/test_third_heuristic.py` & `bw_graph_tools-0.2.3/tests/test_third_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/traversal/test_negative_production.py` & `bw_graph_tools-0.2.3/tests/traversal/test_negative_production.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/traversal/test_nonunitary_production_with_recursion.py` & `bw_graph_tools-0.2.3/tests/traversal/test_nonunitary_production_with_recursion.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/traversal/test_only_one_layer.py` & `bw_graph_tools-0.2.3/tests/traversal/test_only_one_layer.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.2/tests/traversal/test_separate_production.py` & `bw_graph_tools-0.2.3/tests/traversal/test_separate_production.py`

 * *Files identical despite different names*

