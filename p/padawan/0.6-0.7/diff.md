# Comparing `tmp/padawan-0.6.tar.gz` & `tmp/padawan-0.7.tar.gz`

## Comparing `padawan-0.6.tar` & `padawan-0.7.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.6/.readthedocs.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/README.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.6/docs/Makefile
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 padawan-0.6/docs/api.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.6/docs/conf.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.6/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.6/docs/requirements.txt
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/__init__.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/collated_dataset.py
--rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/dataset.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/in_memory_dataset.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/joined_dataset.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/json_io.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/mapped_dataset.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/metadata.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/ordering.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/parallelize.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/persisted_dataset.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/reindexed_dataset.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/renamed_dataset.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/repartitioned_dataset.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.6/src/padawan/sliced_dataset.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.6/tests/fixtures.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_collate.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_from_polars.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_io.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_join.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_map.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_rename.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_repartition.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.6/tests/test_slice.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.6/tests/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.6/.gitignore
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.6/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.6/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.6/pyproject.toml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.6/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.7/.readthedocs.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 padawan-0.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.7/docs/Makefile
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 padawan-0.7/docs/api.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.7/docs/conf.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.7/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.7/docs/requirements.txt
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/collated_dataset.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/concatenated_dataset.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/dataset.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/in_memory_dataset.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/joined_dataset.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/json_io.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/mapped_dataset.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/metadata.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/ordering.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/parallelize.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/persisted_dataset.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/reindexed_dataset.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/renamed_dataset.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/repartitioned_dataset.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.7/src/padawan/sliced_dataset.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.7/tests/fixtures.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_collate.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_concat.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_from_polars.py
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_io.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_join.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_map.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_rename.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_repartition.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.7/tests/test_slice.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.7/tests/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.7/.gitignore
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.7/LICENSE
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.7/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 padawan-0.7/pyproject.toml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 padawan-0.7/PKG-INFO
```

### Comparing `padawan-0.6/.pytest_cache/v/cache/nodeids` & `padawan-0.7/.pytest_cache/v/cache/nodeids`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9692307692307692%*

 * *Differences: {'insert': "[(2, 'tests/test_concat.py::test__concat'), (3, "*

 * *           "'tests/test_concat.py::test__concat__with_empty')]"}*

```diff
@@ -1,10 +1,12 @@
 [
     "tests/test_collate.py::test__collate__parallel",
     "tests/test_collate.py::test__collate__sequential",
+    "tests/test_concat.py::test__concat",
+    "tests/test_concat.py::test__concat__with_empty",
     "tests/test_from_polars.py::test__from_polars__with_index_columns",
     "tests/test_from_polars.py::test__from_polars__without_index_columns",
     "tests/test_io.py::test__collect__parallel",
     "tests/test_io.py::test__collect__sequential",
     "tests/test_io.py::test__collect_stats__no_index_cols",
     "tests/test_io.py::test__collect_stats__parallel",
     "tests/test_io.py::test__collect_stats__sequential",
```

### Comparing `padawan-0.6/docs/Makefile` & `padawan-0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `padawan-0.6/docs/conf.py` & `padawan-0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/docs/index.rst` & `padawan-0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `padawan-0.6/docs/make.bat` & `padawan-0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/collated_dataset.py` & `padawan-0.7/src/padawan/collated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/dataset.py` & `padawan-0.7/src/padawan/dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/in_memory_dataset.py` & `padawan-0.7/src/padawan/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/joined_dataset.py` & `padawan-0.7/src/padawan/joined_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/json_io.py` & `padawan-0.7/src/padawan/json_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/mapped_dataset.py` & `padawan-0.7/src/padawan/mapped_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/metadata.py` & `padawan-0.7/src/padawan/metadata.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/ordering.py` & `padawan-0.7/src/padawan/ordering.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/parallelize.py` & `padawan-0.7/src/padawan/parallelize.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/persisted_dataset.py` & `padawan-0.7/src/padawan/persisted_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/reindexed_dataset.py` & `padawan-0.7/src/padawan/reindexed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/renamed_dataset.py` & `padawan-0.7/src/padawan/renamed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/repartitioned_dataset.py` & `padawan-0.7/src/padawan/repartitioned_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/src/padawan/sliced_dataset.py` & `padawan-0.7/src/padawan/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/fixtures.py` & `padawan-0.7/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_collate.py` & `padawan-0.7/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_from_polars.py` & `padawan-0.7/tests/test_from_polars.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_io.py` & `padawan-0.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_join.py` & `padawan-0.7/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_map.py` & `padawan-0.7/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_rename.py` & `padawan-0.7/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_repartition.py` & `padawan-0.7/tests/test_repartition.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/tests/test_slice.py` & `padawan-0.7/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `padawan-0.6/LICENSE` & `padawan-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `padawan-0.6/README.md` & `padawan-0.7/README.md`

 * *Files identical despite different names*

### Comparing `padawan-0.6/pyproject.toml` & `padawan-0.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padawan"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Martin Wiebusch" },
 ]
 description = "Wrangle partitioned data with polars."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `padawan-0.6/PKG-INFO` & `padawan-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padawan
-Version: 0.6
+Version: 0.7
 Summary: Wrangle partitioned data with polars.
 Project-URL: Homepage, https://github.com/mwiebusch78/padawan
 Project-URL: Bug Tracker, https://github.com/mwiebusch78/padawan/issues
 Project-URL: Documentation, https://padawan.readthedocs.io/en/latest/
 Author: Martin Wiebusch
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

