# Comparing `tmp/proteinflow-1.3.3.tar.gz` & `tmp/proteinflow-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.3.tar", last modified: Wed May 17 13:00:24 2023, max compression
+gzip compressed data, was "proteinflow-1.3.4.tar", last modified: Mon May 22 16:51:19 2023, max compression
```

## Comparing `proteinflow-1.3.3.tar` & `proteinflow-1.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-17 13:00:09.000000 proteinflow-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 13:00:24.077890 proteinflow-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-17 13:00:09.000000 proteinflow-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.073890 proteinflow-1.3.3/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)   100557 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-17 13:00:09.000000 proteinflow-1.3.3/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 13:00:24.000000 proteinflow-1.3.3/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 13:00:09.000000 proteinflow-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:00:24.077890 proteinflow-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:00:24.077890 proteinflow-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-17 13:00:10.000000 proteinflow-1.3.3/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-22 16:51:07.000000 proteinflow-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-22 16:51:19.497694 proteinflow-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-22 16:51:07.000000 proteinflow-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   100565 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-22 16:51:07.000000 proteinflow-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:51:19.497694 proteinflow-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.3/LICENSE` & `proteinflow-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/PKG-INFO` & `proteinflow-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.3
+Version: 1.3.4
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.3 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.4 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.3/README.md` & `proteinflow-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/__init__.py` & `proteinflow-1.3.4/proteinflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,15 +769,15 @@
 
         Returns
         -------
         chain_M : torch.Tensor
             a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
             0 is everything else
         """
-
+        
         if "cdr" in batch and "cdr_id" in batch:
             chain_M = torch.zeros_like(batch["cdr"])
             for i, cdr_arr in enumerate(batch["cdr"]):
                 chain_M[i] = cdr_arr == batch["cdr_id"][i]
         else:
             chain_M = torch.zeros(batch["S"].shape)
             for i, coords in enumerate(batch["X"]):
@@ -870,19 +870,19 @@
                 [
                     torch.cat([b[key], torch.zeros((pad, *b[key].shape[1:]))], 0)
                     for b, pad in zip(batch, to_pad)
                 ],
                 0,
             )
         out["chain_id"] = torch.tensor([b["chain_id"] for b in batch])
+        if "cdr_id" in batch[0]:
+            out["cdr_id"] = torch.tensor([b["cdr_id"] for b in batch])
         out["masked_res"] = self._get_masked_sequence(out)
         out["chain_dict"] = [b["chain_dict"] for b in batch]
         out["pdb_id"] = [b["pdb_id"] for b in batch]
-        if "cdr_id" in batch[0]:
-            out["cdr_id"] = torch.tensor([b["cdr_id"] for b in batch])
         return out
 
     def __call__(self, batch):
         return self.pad_collate(batch)
 
 
 def _get_pdb_ids(
```

### Comparing `proteinflow-1.3.3/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.4/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/async_download.py` & `proteinflow-1.3.4/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.4/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.4/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.4/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/filter_database.py` & `proteinflow-1.3.4/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.4/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.4/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.4/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.4/proteinflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.3
+Version: 1.3.4
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.3 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.4 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.3/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.4/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/pyproject.toml` & `proteinflow-1.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-1.3.3/tests/test_download.py` & `proteinflow-1.3.4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/tests/test_generate.py` & `proteinflow-1.3.4/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.3/tests/test_sabdab.py` & `proteinflow-1.3.4/tests/test_sabdab.py`

 * *Files identical despite different names*

