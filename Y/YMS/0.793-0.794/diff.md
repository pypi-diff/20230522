# Comparing `tmp/YMS-0.793.tar.gz` & `tmp/YMS-0.794.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.793.tar", last modified: Mon May 22 15:21:54 2023, max compression
+gzip compressed data, was "YMS-0.794.tar", last modified: Mon May 22 15:33:40 2023, max compression
```

## Comparing `YMS-0.793.tar` & `YMS-0.794.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:21:54.043583 YMS-0.793/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 15:21:54.043583 YMS-0.793/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.793/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:21:54.043583 YMS-0.793/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 15:21:53.000000 YMS-0.793/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 15:21:54.000000 YMS-0.793/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 15:21:53.000000 YMS-0.793/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 15:21:53.000000 YMS-0.793/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 15:21:53.000000 YMS-0.793/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 15:21:53.000000 YMS-0.793/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 15:21:54.043583 YMS-0.793/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      477 2023-05-22 15:20:38.000000 YMS-0.793/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:21:54.043583 YMS-0.793/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.793/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.793/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11622 2023-05-22 15:21:31.000000 YMS-0.793/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.793/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.793/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.793/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:33:40.243557 YMS-0.794/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 15:33:40.243557 YMS-0.794/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.794/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:33:40.243557 YMS-0.794/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 15:33:40.000000 YMS-0.794/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 15:33:40.243557 YMS-0.794/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      477 2023-05-22 15:33:02.000000 YMS-0.794/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 15:33:40.243557 YMS-0.794/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.794/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.794/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11622 2023-05-22 15:32:57.000000 YMS-0.794/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.794/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.794/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.794/yamas/utilities.py
```

### Comparing `YMS-0.793/README.md` & `YMS-0.794/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.793/yamas/__init__.py` & `YMS-0.794/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.793/yamas/create_visualization.py` & `YMS-0.794/yamas/create_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
 def metaphlan_extraction(reads_data, dataset_id):
     paired = reads_data.rev and reads_data.fwd
     fastq_path = os.path.join(reads_data.dir_path, "fastq")
     export_path = os.path.join(reads_data.dir_path, "export")
     qza_path = os.path.join(reads_data.dir_path, "qza")
     run_cmd([f"mkdir {export_path}"])
-    final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
+    final_output_path = os.path.join(export_path, f'{dataset_id}_final.csv')
     fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
     args = []
     if paired:
         print("paired")
         for i, j in tqdm(zip(fastq_files[::2], fastq_files[1::2])):
             fastq_1 = os.path.join(fastq_path, fastq_files[i])
             fastq_2 = os.path.join(fastq_path, fastq_files[j])
```

### Comparing `YMS-0.793/yamas/dataset_downloading.py` & `YMS-0.794/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.793/yamas/export_data.py` & `YMS-0.794/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.793/yamas/utilities.py` & `YMS-0.794/yamas/utilities.py`

 * *Files identical despite different names*

