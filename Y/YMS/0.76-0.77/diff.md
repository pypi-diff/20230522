# Comparing `tmp/YMS-0.76.tar.gz` & `tmp/YMS-0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.76.tar", last modified: Sun May 21 14:06:55 2023, max compression
+gzip compressed data, was "YMS-0.77.tar", last modified: Mon May 22 13:28:29 2023, max compression
```

## Comparing `YMS-0.76.tar` & `YMS-0.77.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.911554 YMS-0.76/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 14:06:55.911554 YMS-0.76/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.76/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.907554 YMS-0.76/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-21 14:06:55.911554 YMS-0.76/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-21 14:06:48.000000 YMS-0.76/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.911554 YMS-0.76/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.76/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.76/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11186 2023-05-21 14:06:05.000000 YMS-0.76/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.76/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.76/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.76/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 13:28:29.743837 YMS-0.77/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-22 13:28:29.739837 YMS-0.77/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.77/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 13:28:29.739837 YMS-0.77/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-22 13:28:29.000000 YMS-0.77/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-22 13:28:29.743837 YMS-0.77/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-22 13:28:17.000000 YMS-0.77/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-22 13:28:29.739837 YMS-0.77/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.77/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.77/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11011 2023-05-22 13:25:50.000000 YMS-0.77/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.77/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.77/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.77/yamas/utilities.py
```

### Comparing `YMS-0.76/README.md` & `YMS-0.77/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.76/yamas/__init__.py` & `YMS-0.77/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.76/yamas/create_visualization.py` & `YMS-0.77/yamas/create_visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,57 +131,50 @@
 def metaphlan_extraction(reads_data, dataset_id):
     fastq_path = os.path.join(reads_data.dir_path, "fastq")
     export_path = os.path.join(reads_data.dir_path, "export")
     run_cmd([f"mkdir {export_path}"])
     final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
     run_cmd([f"touch {final_output_path}"])
     args = []
-    for fastq in tqdm([a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]):
-        input = os.path.join(fastq_path,fastq)
-        output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
-        command = [f"metaphlan {input} --input_type fastq --nproc 16 > {output} "]
+    fastq_files = [a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]
+
+    for i in tqdm(range(len(fastq_files) - 1)):
+        fastq_1 = os.path.join(fastq_path,fastq_files[i])
+        fastq_2 = os.path.join(fastq_path,fastq_files[i+1])
+        output = f"{dataset_id}.bowtie2.bz2"
+        command = [f"metaphlan {fastq_1},{fastq_2} --input_type fastq --bowtie2out {output} --nproc 24"]
         run_cmd(command)
-        args.append(output)
+        args.append(os.path.join(fastq_path,output))
     merge(args, open(final_output_path, 'w'), gtdb=False)
-    # profiles = [os.listdir(os.path.join(reads_data.dir_path, 'qza'))
-    # merge(profiles)
 
 def metaphlan_txt_csv(reads_data, dataset_id):
     export_path = os.path.join(reads_data.dir_path, "export")
     input_file = os.path.join(export_path,f"{dataset_id}_final.txt")
-    data = []
-
-    with open(input_file, 'r') as file:
-        lines = file.readlines()
-
-        for line in lines:
-            line = line.strip()
+    output_file = os.path.join(export_path,f"{dataset_id}_final_table.txt")
+    with open(input_file, 'r') as txt_file:
+        lines = txt_file.readlines()
+
+    # Extract data from the text file
+    headers = lines[0].strip().split('\t')
+    data = [line.strip().split('\t') for line in lines[1:]]
+
+    # Replace "|" with ","
+    headers = [header.replace('|', ',') for header in headers]
+    data = [[entry.replace('|', ',') for entry in row] for row in data]
+
+    # Transpose the data
+    transposed_data = list(map(list, zip(*data)))
+
+    # Write the transposed data to a CSV file
+    with open(output_file, 'w', newline='') as csv_file:
+        writer = csv.writer(csv_file)
+        writer.writerow(headers)
+        writer.writerows(transposed_data)
 
-            if line.startswith('#') or line.startswith('SampleID') or line.startswith('clade_name'):
-                continue
-
-            fields = line.split('\t')
-
-            if len(fields) >= 4:
-                bacteria = fields[0]
-                relative_abundance = fields[2]
-                data.append([bacteria, relative_abundance])
-
-    total_abundance = sum(float(row[1]) for row in data)
-
-    for row in data:
-        relative_abundance = float(row[1])
-        percentage = (relative_abundance / total_abundance) * 100
-        row[1] = f'{percentage:.2f}%'
-    output_file = os.path.join(export_path, f'{dataset_id}_table.csv')
-    run_cmd([f"touch {output_file}"])
-    with open(output_file, 'w', newline='') as file:
-        writer = csv.writer(file)
-        writer.writerow(['Bacteria', 'Percentage'])
-        writer.writerows(data)
+    print(f"CSV file '{output_file}' has been created.")
 
 def visualization(acc_list, dataset_id, data_type, verbose_print, specific_location):
     verbose_print("\n")
     verbose_print(datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S'))
     dir_name = f"{dataset_id}-{datetime.datetime.now().strftime('%d-%m-%Y_%H-%M-%S')}"
     verbose_print("Starting conversion to VIS file")
```

### Comparing `YMS-0.76/yamas/dataset_downloading.py` & `YMS-0.77/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.76/yamas/export_data.py` & `YMS-0.77/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.76/yamas/utilities.py` & `YMS-0.77/yamas/utilities.py`

 * *Files identical despite different names*

