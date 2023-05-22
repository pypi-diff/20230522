# Comparing `tmp/NanoRepeat-1.4.1.tar.gz` & `tmp/NanoRepeat-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NanoRepeat-1.4.1.tar", last modified: Wed May 17 15:32:35 2023, max compression
+gzip compressed data, was "NanoRepeat-1.5.tar", last modified: Mon May 22 06:20:17 2023, max compression
```

## Comparing `NanoRepeat-1.4.1.tar` & `NanoRepeat-1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.4.1/LICENSE
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16293 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.4.1/README.md
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/setup.cfg
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      803 2023-05-17 15:31:55.000000 NanoRepeat-1.4.1/setup.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.220437 NanoRepeat-1.4.1/src/
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/src/NanoRepeat/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.4.1/src/NanoRepeat/__init__.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat-joint.py
--rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10986 2023-05-17 12:43:34.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    30089 2023-05-17 13:59:27.000000 NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat_bam.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.4.1/src/NanoRepeat/paf.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)     4446 2023-05-13 06:08:18.000000 NanoRepeat-1.4.1/src/NanoRepeat/repeat_region.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.4.1/src/NanoRepeat/split_alleles.py
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.4.1/src/NanoRepeat/tk.py
-drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-17 15:32:35.224437 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/
--rw-rw-r--   0 fangli    (1002) fangli    (1002)    16293 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/PKG-INFO
--rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/SOURCES.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/dependency_links.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/requires.txt
--rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-05-17 15:32:35.000000 NanoRepeat-1.4.1/src/NanoRepeat.egg-info/top_level.txt
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     1097 2023-05-11 08:33:58.000000 NanoRepeat-1.5/LICENSE
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-05-22 06:20:17.450181 NanoRepeat-1.5/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    15958 2023-05-17 14:33:11.000000 NanoRepeat-1.5/README.md
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       38 2023-05-22 06:20:17.450181 NanoRepeat-1.5/setup.cfg
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      801 2023-05-22 01:47:21.000000 NanoRepeat-1.5/setup.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.446181 NanoRepeat-1.5/src/
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/src/NanoRepeat/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      186 2023-05-11 08:33:58.000000 NanoRepeat-1.5/src/NanoRepeat/__init__.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    36432 2023-05-13 06:07:32.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat-joint.py
+-rwxrwxr-x   0 fangli    (1002) fangli    (1002)    10989 2023-05-22 01:41:48.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    30089 2023-05-17 13:59:27.000000 NanoRepeat-1.5/src/NanoRepeat/nanoRepeat_bam.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     3078 2023-05-13 06:08:14.000000 NanoRepeat-1.5/src/NanoRepeat/paf.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)     4446 2023-05-13 06:08:18.000000 NanoRepeat-1.5/src/NanoRepeat/repeat_region.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    31135 2023-05-14 07:24:25.000000 NanoRepeat-1.5/src/NanoRepeat/split_alleles.py
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16195 2023-05-17 13:58:21.000000 NanoRepeat-1.5/src/NanoRepeat/tk.py
+drwxrwxr-x   0 fangli    (1002) fangli    (1002)        0 2023-05-22 06:20:17.450181 NanoRepeat-1.5/src/NanoRepeat.egg-info/
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)    16291 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/PKG-INFO
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)      446 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/SOURCES.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)        1 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/dependency_links.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       53 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/requires.txt
+-rw-rw-r--   0 fangli    (1002) fangli    (1002)       11 2023-05-22 06:20:17.000000 NanoRepeat-1.5/src/NanoRepeat.egg-info/top_level.txt
```

### Comparing `NanoRepeat-1.4.1/LICENSE` & `NanoRepeat-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/PKG-INFO` & `NanoRepeat-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.4.1
+Version: 1.5
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NanoRepeat-1.4.1/README.md` & `NanoRepeat-1.5/README.md`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/setup.py` & `NanoRepeat-1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
     
 setup(
     name='NanoRepeat',
-    version='1.4.1',
+    version='1.5',
     description='NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data',
     long_description = readme,
     long_description_content_type = 'text/markdown',
     url='https://github.com/WGLab/NanoRepeat',
     author='Li Fang, Kai Wang',
     author_email='fangli9@sysu.edu.cn',
     license='MIT',
```

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat-joint.py` & `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat-joint.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat.py` & `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     if os.path.exists(sorted_bam_file):
         os.remove(sorted_bam_file)
 
     sleep_time = 5
 
     preset = tk.get_preset_for_minimap2(data_type)
-    cmd = f'{minimap2} {preset} -t {num_cpu} {ref_fasta_file} {in_fastq_file} > {sam_file} 2> /dev/null'
+    cmd = f'{minimap2} -a {preset} -t {num_cpu} {ref_fasta_file} {in_fastq_file} > {sam_file} 2> /dev/null'
     tk.run_system_cmd(cmd)
     time.sleep(sleep_time)
 
     cmd = f'{samtools} view -hb -@ {num_cpu} {sam_file} > {bam_file} 2> /dev/null'
     tk.run_system_cmd(cmd)
     time.sleep(sleep_time)
```

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/nanoRepeat_bam.py` & `NanoRepeat-1.5/src/NanoRepeat/nanoRepeat_bam.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/paf.py` & `NanoRepeat-1.5/src/NanoRepeat/paf.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/repeat_region.py` & `NanoRepeat-1.5/src/NanoRepeat/repeat_region.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/split_alleles.py` & `NanoRepeat-1.5/src/NanoRepeat/split_alleles.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat/tk.py` & `NanoRepeat-1.5/src/NanoRepeat/tk.py`

 * *Files identical despite different names*

### Comparing `NanoRepeat-1.4.1/src/NanoRepeat.egg-info/PKG-INFO` & `NanoRepeat-1.5/src/NanoRepeat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NanoRepeat
-Version: 1.4.1
+Version: 1.5
 Summary: NanoRepeat: quantification of Short Tandem Repeats (STRs) from long-read sequencing data
 Home-page: https://github.com/WGLab/NanoRepeat
 Author: Li Fang, Kai Wang
 Author-email: fangli9@sysu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

