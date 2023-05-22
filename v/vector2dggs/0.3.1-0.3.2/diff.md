# Comparing `tmp/vector2dggs-0.3.1.tar.gz` & `tmp/vector2dggs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.3.1.tar", max compression
+gzip compressed data, was "vector2dggs-0.3.2.tar", max compression
```

## Comparing `vector2dggs-0.3.1.tar` & `vector2dggs-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7920 2023-05-03 01:16:48.563418 vector2dggs-0.3.1/README.md
--rw-r--r--   0        0        0     1092 2023-05-03 01:16:53.215440 vector2dggs-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/cli.py
--rw-r--r--   0        0        0     9399 2023-05-03 01:16:28.111317 vector2dggs-0.3.1/vector2dggs/h3.py
--rw-r--r--   0        0        0     3074 2023-05-02 23:30:16.752288 vector2dggs-0.3.1/vector2dggs/katana.py
--rw-r--r--   0        0        0     9354 1970-01-01 00:00:00.000000 vector2dggs-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     8006 2023-05-22 02:22:17.187783 vector2dggs-0.3.2/README.md
+-rw-r--r--   0        0        0     1092 2023-05-22 02:20:46.867330 vector2dggs-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.2/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.2/vector2dggs/cli.py
+-rw-r--r--   0        0        0     9400 2023-05-22 02:22:11.423754 vector2dggs-0.3.2/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.2/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 vector2dggs-0.3.2/PKG-INFO
```

### Comparing `vector2dggs-0.3.1/README.md` & `vector2dggs-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
 
   VECTOR_INPUT is the path to input vector geospatial data. OUTPUT_DIRECTORY
-  should be a directory, not a file, as it will be the write location for an
-  Apache Parquet data store.
+  should be a directory, not a file or database table, as it will instead be
+  the write location for an Apache Parquet data store.
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
   -id, --id_field TEXT            Field to use as an ID; defaults to a
@@ -65,16 +65,16 @@
                                   [default: 7]
   -tbl, --table TEXT              Name of the table to read when using a
                                   spatial database connection as input
   -g, --geom_col TEXT             Column name to use when using a spatial
                                   database connection as input  [default:
                                   geom]
   -o, --overwrite
+  --version                       Show the version and exit.
   --help                          Show this message and exit.
-
 ```
 
 ### Example 
 
 
 
 
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.1},
+  version={0.3.2},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.2) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.3.1/pyproject.toml` & `vector2dggs-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.3.1"
+version = "0.3.2"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.3.1/vector2dggs/cli.py` & `vector2dggs-0.3.2/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.1/vector2dggs/h3.py` & `vector2dggs-0.3.2/vector2dggs/h3.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     geom_col: str,
     overwrite: bool,
 ):
     """
     Ingest a vector dataset and index it to the H3 DGGS.
 
     VECTOR_INPUT is the path to input vector geospatial data.
-    OUTPUT_DIRECTORY should be a directory, not a file or database table, as it willinstead be the write location for an Apache Parquet data store.
+    OUTPUT_DIRECTORY should be a directory, not a file or database table, as it will instead be the write location for an Apache Parquet data store.
     """
     con: sqlalchemy.engine.Connection = None
     scheme: str = urlparse(vector_input).scheme
     if bool(scheme) and scheme != "file":
         # Assume database connection
         con = sqlalchemy.create_engine(vector_input)
     elif not Path(vector_input).exists():
```

### Comparing `vector2dggs-0.3.1/vector2dggs/katana.py` & `vector2dggs-0.3.2/vector2dggs/katana.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 
 def katana(geometry, threshold, count=0) -> GeometryCollection:
     """
     Split a polygon into two parts across it's shortest dimension.
     Invalid input `geometry` will silently be made valid (if possible).
     """
+    if geometry is None:
+        # Empty geometry collection
+        return GeometryCollection([])
     if not geometry.is_valid:
         # print(explain_validity(geometry))
         geometry = make_valid(geometry)
     bounds = geometry.bounds
     width = bounds[2] - bounds[0]
     height = bounds[3] - bounds[1]
     if max(width, height) <= threshold or count == 250:
```

### Comparing `vector2dggs-0.3.1/PKG-INFO` & `vector2dggs-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -58,16 +58,16 @@
 ```bash
 vector2dggs h3 --help
 Usage: vector2dggs h3 [OPTIONS] VECTOR_INPUT OUTPUT_DIRECTORY
 
   Ingest a vector dataset and index it to the H3 DGGS.
 
   VECTOR_INPUT is the path to input vector geospatial data. OUTPUT_DIRECTORY
-  should be a directory, not a file, as it will be the write location for an
-  Apache Parquet data store.
+  should be a directory, not a file or database table, as it will instead be
+  the write location for an Apache Parquet data store.
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
   -id, --id_field TEXT            Field to use as an ID; defaults to a
@@ -100,16 +100,16 @@
                                   [default: 7]
   -tbl, --table TEXT              Name of the table to read when using a
                                   spatial database connection as input
   -g, --geom_col TEXT             Column name to use when using a spatial
                                   database connection as input  [default:
                                   geom]
   -o, --overwrite
+  --version                       Show the version and exit.
   --help                          Show this message and exit.
-
 ```
 
 ### Example 
 
 
 
 
@@ -183,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.1},
+  version={0.3.2},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.2) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

