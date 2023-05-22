# Comparing `tmp/YMS-0.79.tar.gz` & `tmp/YMS-0.791.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.79.tar", last modified: Mon May 22 14:33:12 2023, max compression
+gzip compressed data, was "YMS-0.791.tar", last modified: Mon May 22 14:42:07 2023, max compression
```

## Comparing `YMS-0.79.tar` & `YMS-0.791.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:33:12.679692 YMS-0.79/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-22 14:33:12.679692 YMS-0.79/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.79/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:33:12.679692 YMS-0.79/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 14:33:12.000000 YMS-0.79/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 14:33:12.679692 YMS-0.79/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-22 14:33:07.000000 YMS-0.79/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:33:12.679692 YMS-0.79/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.79/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.79/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11610 2023-05-22 14:32:57.000000 YMS-0.79/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.79/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.79/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.79/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:42:07.471672 YMS-0.791/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 14:42:07.471672 YMS-0.791/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.791/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:42:07.471672 YMS-0.791/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      157 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 14:42:07.000000 YMS-0.791/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 14:42:07.471672 YMS-0.791/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      477 2023-05-22 14:41:52.000000 YMS-0.791/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 14:42:07.471672 YMS-0.791/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.791/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.791/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11545 2023-05-22 14:41:49.000000 YMS-0.791/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.791/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.791/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.791/yamas/utilities.py
```

### Comparing `YMS-0.79/README.md` & `YMS-0.791/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.79/yamas/__init__.py` & `YMS-0.791/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.79/yamas/create_visualization.py` & `YMS-0.791/yamas/create_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,29 +130,28 @@
 
 def metaphlan_extraction(reads_data, dataset_id):
     paired = reads_data.rev and reads_data.fwd
     fastq_path = os.path.join(reads_data.dir_path, "fastq")
     export_path = os.path.join(reads_data.dir_path, "export")
     qza_path = os.path.join(reads_data.dir_path, "qza")
     run_cmd([f"mkdir {export_path}"])
+    final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
+    fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
     args = []
     if paired:
-        fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
-
         for i, j in tqdm(zip(fastq_files[::2], fastq_files[1::2])):
             fastq_1 = os.path.join(fastq_path, fastq_files[i])
             fastq_2 = os.path.join(fastq_path, fastq_files[j])
             output = os.path.join(qza_path, "{fastq_1.split('_')[0]}.bowtie2.bz2")
             command = [f"metaphlan {fastq_1},{fastq_2} --input_type fastq --bowtie2out {output} --nproc 24"]
             run_cmd(command)
             args.append(os.path.join(fastq_path, output))
     else:
-        final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
         run_cmd([f"touch {final_output_path}"])
-        for fastq in tqdm([a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]):
+        for fastq in tqdm(fastq_files):
             output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
             command = [f"metaphlan {input} --input_type fastq --nproc 16"
                        f" > {output} "]
             run_cmd(command)
             args.append(output)
     merge(args, open(final_output_path, 'w'), gtdb=False)
```

### Comparing `YMS-0.79/yamas/dataset_downloading.py` & `YMS-0.791/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.79/yamas/export_data.py` & `YMS-0.791/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.79/yamas/utilities.py` & `YMS-0.791/yamas/utilities.py`

 * *Files identical despite different names*

