# Comparing `tmp/kerbitat-0.0.1.tar.gz` & `tmp/kerbitat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerbitat-0.0.1.tar", last modified: Sun May 21 20:13:14 2023, max compression
+gzip compressed data, was "kerbitat-0.0.2.tar", last modified: Mon May 22 08:34:36 2023, max compression
```

## Comparing `kerbitat-0.0.1.tar` & `kerbitat-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-21 20:13:14.446187 kerbitat-0.0.1/
--rw-rw-r--   0 sist     (14287) sist     (14287)    11357 2023-05-21 19:30:18.000000 kerbitat-0.0.1/LICENSE
--rw-rw-r--   0 sist     (14287) sist     (14287)     2343 2023-05-21 20:13:14.446187 kerbitat-0.0.1/PKG-INFO
--rw-rw-r--   0 sist     (14287) sist     (14287)     1850 2023-05-21 19:55:12.000000 kerbitat-0.0.1/README.md
--rw-rw-r--   0 sist     (14287) sist     (14287)      663 2023-05-21 20:11:31.000000 kerbitat-0.0.1/pyproject.toml
--rw-rw-r--   0 sist     (14287) sist     (14287)       38 2023-05-21 20:13:14.446187 kerbitat-0.0.1/setup.cfg
-drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-21 20:13:14.442187 kerbitat-0.0.1/src/
-drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-21 20:13:14.446187 kerbitat-0.0.1/src/kerbitat/
--rw-rw-r--   0 sist     (14287) sist     (14287)        0 2023-05-21 19:56:04.000000 kerbitat-0.0.1/src/kerbitat/__init__.py
--rw-rw-r--   0 sist     (14287) sist     (14287)     4082 2023-05-21 19:35:15.000000 kerbitat-0.0.1/src/kerbitat/kerbitat.py
-drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-21 20:13:14.446187 kerbitat-0.0.1/src/kerbitat.egg-info/
--rw-rw-r--   0 sist     (14287) sist     (14287)     2343 2023-05-21 20:13:14.000000 kerbitat-0.0.1/src/kerbitat.egg-info/PKG-INFO
--rw-rw-r--   0 sist     (14287) sist     (14287)      226 2023-05-21 20:13:14.000000 kerbitat-0.0.1/src/kerbitat.egg-info/SOURCES.txt
--rw-rw-r--   0 sist     (14287) sist     (14287)        1 2023-05-21 20:13:14.000000 kerbitat-0.0.1/src/kerbitat.egg-info/dependency_links.txt
--rw-rw-r--   0 sist     (14287) sist     (14287)        9 2023-05-21 20:13:14.000000 kerbitat-0.0.1/src/kerbitat.egg-info/top_level.txt
+drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-22 08:34:36.104549 kerbitat-0.0.2/
+-rw-rw-r--   0 sist     (14287) sist     (14287)    11357 2023-05-21 19:30:18.000000 kerbitat-0.0.2/LICENSE
+-rw-rw-r--   0 sist     (14287) sist     (14287)       27 2023-05-22 07:39:44.000000 kerbitat-0.0.2/MANIFEST.in
+-rw-rw-r--   0 sist     (14287) sist     (14287)     2391 2023-05-22 08:34:36.104549 kerbitat-0.0.2/PKG-INFO
+-rw-rw-r--   0 sist     (14287) sist     (14287)     1898 2023-05-22 06:46:48.000000 kerbitat-0.0.2/README.md
+-rw-rw-r--   0 sist     (14287) sist     (14287)      663 2023-05-22 07:44:45.000000 kerbitat-0.0.2/pyproject.toml
+-rw-rw-r--   0 sist     (14287) sist     (14287)       38 2023-05-22 08:34:36.104549 kerbitat-0.0.2/setup.cfg
+drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-22 08:34:36.100548 kerbitat-0.0.2/src/
+drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-22 08:34:36.100548 kerbitat-0.0.2/src/kerbitat/
+-rw-rw-r--   0 sist     (14287) sist     (14287)      375 2023-05-22 07:55:15.000000 kerbitat-0.0.2/src/kerbitat/__init__.py
+drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-22 08:34:36.100548 kerbitat-0.0.2/src/kerbitat/data/
+-rwxrwxr-x   0 sist     (14287) sist     (14287)   144691 2023-05-21 19:32:36.000000 kerbitat-0.0.2/src/kerbitat/data/kernel_to_id.pkl
+-rw-rw-r--   0 sist     (14287) sist     (14287)  1254809 2023-05-22 08:26:42.000000 kerbitat-0.0.2/src/kerbitat/data/predictor.pt
+-rw-rw-r--   0 sist     (14287) sist     (14287)     5241 2023-05-22 08:31:04.000000 kerbitat-0.0.2/src/kerbitat/kerbitat.py
+drwxrwxr-x   0 sist     (14287) sist     (14287)        0 2023-05-22 08:34:36.100548 kerbitat-0.0.2/src/kerbitat.egg-info/
+-rw-rw-r--   0 sist     (14287) sist     (14287)     2391 2023-05-22 08:34:36.000000 kerbitat-0.0.2/src/kerbitat.egg-info/PKG-INFO
+-rw-rw-r--   0 sist     (14287) sist     (14287)      304 2023-05-22 08:34:36.000000 kerbitat-0.0.2/src/kerbitat.egg-info/SOURCES.txt
+-rw-rw-r--   0 sist     (14287) sist     (14287)        1 2023-05-22 08:34:36.000000 kerbitat-0.0.2/src/kerbitat.egg-info/dependency_links.txt
+-rw-rw-r--   0 sist     (14287) sist     (14287)        9 2023-05-22 08:34:36.000000 kerbitat-0.0.2/src/kerbitat.egg-info/top_level.txt
```

### Comparing `kerbitat-0.0.1/LICENSE` & `kerbitat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerbitat-0.0.1/PKG-INFO` & `kerbitat-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerbitat
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small tool to pridict running time of a DNN model on NVIDIA GPUs.
 Author-email: Siyuan Zhang <zhangsy3@shanghaitech.edu.cn>
 Project-URL: Homepage, https://github.com/murez/kerbitat
 Project-URL: Bug Tracker, https://github.com/murez/kerbitat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,14 +12,20 @@
 License-File: LICENSE
 
 # Kerbitat
 
 Kerbitat is a profiling tool for pridicting running time of a DNN model on NVIDIA GPUs.
 It can predict the performance of the target GPU from the profiling result of the source GPU.
 
+
+# Install
+```
+pip install kerbitat==0.0.1
+```
+
 # How it works
 
 1. Kerbitat use KernelProfiler from habitat to get mangled kernel names of running DNN model.
 2. Kerbitat convert the mangled kernel names to feature vector.
 3. Kerbitat use a trained model to predict the performance of the target GPU from the 
    feature vector.
 4. Kerbitat use the predicted performance to estimate the execution time of the target GPU.
```

### Comparing `kerbitat-0.0.1/README.md` & `kerbitat-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Kerbitat
 
 Kerbitat is a profiling tool for pridicting running time of a DNN model on NVIDIA GPUs.
 It can predict the performance of the target GPU from the profiling result of the source GPU.
 
+
+# Install
+```
+pip install kerbitat==0.0.1
+```
+
 # How it works
 
 1. Kerbitat use KernelProfiler from habitat to get mangled kernel names of running DNN model.
 2. Kerbitat convert the mangled kernel names to feature vector.
 3. Kerbitat use a trained model to predict the performance of the target GPU from the 
    feature vector.
 4. Kerbitat use the predicted performance to estimate the execution time of the target GPU.
```

### Comparing `kerbitat-0.0.1/pyproject.toml` & `kerbitat-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "deepview-profile>=0.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kerbitat"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Siyuan Zhang", email="zhangsy3@shanghaitech.edu.cn" },
 ]
 description = "A small tool to pridict running time of a DNN model on NVIDIA GPUs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `kerbitat-0.0.1/src/kerbitat.egg-info/PKG-INFO` & `kerbitat-0.0.2/src/kerbitat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerbitat
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small tool to pridict running time of a DNN model on NVIDIA GPUs.
 Author-email: Siyuan Zhang <zhangsy3@shanghaitech.edu.cn>
 Project-URL: Homepage, https://github.com/murez/kerbitat
 Project-URL: Bug Tracker, https://github.com/murez/kerbitat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,14 +12,20 @@
 License-File: LICENSE
 
 # Kerbitat
 
 Kerbitat is a profiling tool for pridicting running time of a DNN model on NVIDIA GPUs.
 It can predict the performance of the target GPU from the profiling result of the source GPU.
 
+
+# Install
+```
+pip install kerbitat==0.0.1
+```
+
 # How it works
 
 1. Kerbitat use KernelProfiler from habitat to get mangled kernel names of running DNN model.
 2. Kerbitat convert the mangled kernel names to feature vector.
 3. Kerbitat use a trained model to predict the performance of the target GPU from the 
    feature vector.
 4. Kerbitat use the predicted performance to estimate the execution time of the target GPU.
```

