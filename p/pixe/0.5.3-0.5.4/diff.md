# Comparing `tmp/pixe-0.5.3.tar.gz` & `tmp/pixe-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixe-0.5.3.tar", last modified: Tue Feb 21 15:25:27 2023, max compression
+gzip compressed data, was "pixe-0.5.4.tar", last modified: Mon May 22 00:33:14 2023, max compression
```

## Comparing `pixe-0.5.3.tar` & `pixe-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 iroh      (1000) iroh      (1000)        0 2023-02-21 15:25:27.202983 pixe-0.5.3/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)    11357 2023-01-13 03:09:37.000000 pixe-0.5.3/LICENSE
--rw-r--r--   0 iroh      (1000) iroh      (1000)     2620 2023-02-21 15:25:27.202983 pixe-0.5.3/PKG-INFO
--rw-r--r--   0 iroh      (1000) iroh      (1000)     1999 2023-02-21 14:55:14.000000 pixe-0.5.3/README.md
-drwxr-xr-x   0 iroh      (1000) iroh      (1000)        0 2023-02-21 15:25:27.201983 pixe-0.5.3/pixe.egg-info/
--rw-r--r--   0 iroh      (1000) iroh      (1000)     2620 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/PKG-INFO
--rw-r--r--   0 iroh      (1000) iroh      (1000)      255 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/SOURCES.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)        1 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/dependency_links.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)       34 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/entry_points.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)      126 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/requires.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)        5 2023-02-21 15:25:27.000000 pixe-0.5.3/pixe.egg-info/top_level.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)     6970 2023-02-19 04:21:52.000000 pixe-0.5.3/pixe.py
--rw-r--r--   0 iroh      (1000) iroh      (1000)      867 2023-02-21 15:25:18.000000 pixe-0.5.3/pyproject.toml
--rw-r--r--   0 iroh      (1000) iroh      (1000)       38 2023-02-21 15:25:27.202983 pixe-0.5.3/setup.cfg
-drwxr-xr-x   0 iroh      (1000) iroh      (1000)        0 2023-02-21 15:25:27.201983 pixe-0.5.3/tests/
--rw-r--r--   0 iroh      (1000) iroh      (1000)     3683 2023-02-19 05:20:40.000000 pixe-0.5.3/tests/test_integration.py
--rw-r--r--   0 iroh      (1000) iroh      (1000)     1744 2023-02-19 05:20:40.000000 pixe-0.5.3/tests/test_unit.py
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 00:33:14.136283 pixe-0.5.4/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)    11357 2023-02-28 15:56:19.000000 pixe-0.5.4/LICENSE
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 00:33:14.136283 pixe-0.5.4/PKG-INFO
+-rw-r--r--   0 iroh      (1000) iroh      (1000)     3382 2023-05-22 00:30:49.000000 pixe-0.5.4/README.md
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 00:33:14.135283 pixe-0.5.4/pixe.egg-info/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/PKG-INFO
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)      255 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/SOURCES.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)        1 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/dependency_links.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)       34 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/entry_points.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)      126 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/requires.txt
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)        5 2023-05-22 00:33:14.000000 pixe-0.5.4/pixe.egg-info/top_level.txt
+-rw-r--r--   0 iroh      (1000) iroh      (1000)     7001 2023-05-22 00:30:49.000000 pixe-0.5.4/pixe.py
+-rw-r--r--   0 iroh      (1000) iroh      (1000)      867 2023-05-22 00:30:49.000000 pixe-0.5.4/pyproject.toml
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)       38 2023-05-22 00:33:14.136283 pixe-0.5.4/setup.cfg
+drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 00:33:14.136283 pixe-0.5.4/tests/
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     3683 2023-02-28 15:56:19.000000 pixe-0.5.4/tests/test_integration.py
+-rw-rw-r--   0 iroh      (1000) iroh      (1000)     1744 2023-02-28 15:56:19.000000 pixe-0.5.4/tests/test_unit.py
```

### Comparing `pixe-0.5.3/LICENSE` & `pixe-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixe-0.5.3/pixe.py` & `pixe-0.5.4/pixe.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """
     cdate = _extract_date(file_path)
     cdate_str = cdate.strftime("%Y%m%d_%H%M%S")
     hash_str = _calc_checksum(file_path)
     filename = file_path.with_stem(f"{cdate_str}_{hash_str}").with_suffix(file_path.suffix.lower())
     dest_path = pathlib.Path(dest_str).joinpath(str(cdate.year), str(cdate.month))
 
-    # if the a similarly named file exists at the destination it means we have a duplicate file
+    # if a similarly named file exists at the destination it means we have a duplicate file
     # prepend 'dups' and the START_TIME of this move process to the destination filepath
     if dest_path.joinpath(filename.name).exists():
         dest_path = pathlib.Path(dest_str).joinpath(
             f"dups/{START_TIME.strftime('%Y%m%d_%H%M%S')}",
             str(cdate.year),
             str(cdate.month),
         )
@@ -132,14 +132,15 @@
     :param kwargs: additional options (likely exif tags)
     """
     pool = multiprocessing.Pool()
     for file in file_list:
         pool.apply_async(
             _process_file,
             args=(file, dest, move),
+            kwds=kwargs,
             callback=(lambda res: print(res, flush=True)),
         )
     pool.close()
     pool.join()
 
 
 def serial_process_files(file_list: list, dest: str, move: bool, **kwargs):
@@ -147,15 +148,15 @@
     process a list of files serially
     :param file_list: a list of files to be processed
     :param dest: the destination for the process operation
     :param move: is this a move or copy operation
     :param kwargs: additional options (likely exif tags)
     """
     for file in file_list:
-        print(_process_file(file, dest, move))
+        print(_process_file(file, dest, move, **kwargs))
 
 
 @click.command()
 @click.argument("src")
 @click.option("--dest", "-d", default=".", help="desired destination")
 @click.option(
     "--recurse",
```

### Comparing `pixe-0.5.3/pyproject.toml` & `pixe-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixe"
-version = "0.5.3"
+version = "0.5.4"
 description = "A digital helper to keep your files neat and tidy"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache License, Version 2.0"}
 keywords = ["archive", "photos", "organize"]
 authors = [
     {name = "Chris Wells", email = "chris@ithuna.com"},
```

### Comparing `pixe-0.5.3/tests/test_integration.py` & `pixe-0.5.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pixe-0.5.3/tests/test_unit.py` & `pixe-0.5.4/tests/test_unit.py`

 * *Files identical despite different names*

