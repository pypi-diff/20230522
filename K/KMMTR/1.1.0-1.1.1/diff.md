# Comparing `tmp/KMMTR-1.1.0.tar.gz` & `tmp/KMMTR-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-1.1.0.tar", last modified: Sun May 21 00:09:29 2023, max compression
+gzip compressed data, was "KMMTR-1.1.1.tar", last modified: Mon May 22 00:15:06 2023, max compression
```

## Comparing `KMMTR-1.1.0.tar` & `KMMTR-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.770659 KMMTR-1.1.0/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.769792 KMMTR-1.1.0/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6822 2023-05-21 00:08:04.000000 KMMTR-1.1.0/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6660 2023-05-21 00:08:25.000000 KMMTR-1.1.0/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.0/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-21 00:09:29.770366 KMMTR-1.1.0/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-21 00:09:29.000000 KMMTR-1.1.0/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-21 00:09:29.770532 KMMTR-1.1.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.0/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-21 00:09:29.770698 KMMTR-1.1.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-21 00:08:51.000000 KMMTR-1.1.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.228455 KMMTR-1.1.1/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.227547 KMMTR-1.1.1/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6821 2023-05-22 00:14:25.000000 KMMTR-1.1.1/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6660 2023-05-21 00:08:25.000000 KMMTR-1.1.1/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-1.1.1/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-22 00:15:06.228146 KMMTR-1.1.1/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-22 00:15:06.000000 KMMTR-1.1.1/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-22 00:15:06.228316 KMMTR-1.1.1/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-1.1.1/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-22 00:15:06.228495 KMMTR-1.1.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-22 00:14:40.000000 KMMTR-1.1.1/setup.py
```

### Comparing `KMMTR-1.1.0/KMMTR/KMM.py` & `KMMTR-1.1.1/KMMTR/KMM.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         
         Returns:
             An instantiated kernel function object.
         """
         Xtrain = np.array(self.target_data)
         Ytrain = np.array(self.target_response)
         ker = self.call_kernel()
-        noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.01))
+        noise_ker = WhiteKernel(noise_level_bounds=(0.001,0.5))
         # cal the data nosie by maximazing the likelihood 
         GPr = GPR(kernel=ker+noise_ker,normalize_y=True).fit(Xtrain,Ytrain)
         noise_level = np.exp(GPr.kernel_.theta[1])
         print('Trained noise is %f' % noise_level)
 
         GPr_fit = GPR(kernel=ker, alpha = noise_level,normalize_y=True).fit(Xtrain,Ytrain)
         print('Trained Kernel Function :', GPr_fit.kernel_)
```

### Comparing `KMMTR-1.1.0/KMMTR/KMMTR.py` & `KMMTR-1.1.1/KMMTR/KMMTR.py`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.0/KMMTR.egg-info/PKG-INFO` & `KMMTR-1.1.1/KMMTR.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.0
+Version: 1.1.1
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.0/PKG-INFO` & `KMMTR-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 1.1.0
+Version: 1.1.1
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-1.1.0/README.md` & `KMMTR-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-1.1.0/setup.py` & `KMMTR-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='1.1.0',  # 版本
+    version='1.1.1',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

