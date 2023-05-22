# Comparing `tmp/krutils-0.20230522.1605.tar.gz` & `tmp/krutils-0.20230522.1619.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1605.tar", last modified: Mon May 22 07:05:41 2023, max compression
+gzip compressed data, was "krutils-0.20230522.1619.tar", last modified: Mon May 22 07:19:14 2023, max compression
```

## Comparing `krutils-0.20230522.1605.tar` & `krutils-0.20230522.1619.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 07:05:41.030408 krutils-0.20230522.1605/
--rw-rw-rw-   0        0        0      526 2023-05-22 07:05:41.013046 krutils-0.20230522.1605/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1605/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 07:05:40.703219 krutils-0.20230522.1605/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1605/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1605/krutils/CONST.py
--rw-rw-rw-   0        0        0       96 2023-05-22 04:22:41.000000 krutils-0.20230522.1605/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1605/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     1989 2023-05-22 06:47:48.000000 krutils-0.20230522.1605/krutils/futils.py
--rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230522.1605/krutils/logger.py
--rw-rw-rw-   0        0        0    18549 2023-05-22 06:46:23.000000 krutils-0.20230522.1605/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:05:40.799025 krutils-0.20230522.1605/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 07:05:40.000000 krutils-0.20230522.1605/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-05-22 07:05:40.000000 krutils-0.20230522.1605/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 07:05:40.000000 krutils-0.20230522.1605/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 07:05:40.000000 krutils-0.20230522.1605/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 07:05:40.000000 krutils-0.20230522.1605/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 07:05:41.035887 krutils-0.20230522.1605/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 07:05:39.000000 krutils-0.20230522.1605/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 07:05:40.968760 krutils-0.20230522.1605/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230522.1605/test/test_futils.py
--rw-rw-rw-   0        0        0      308 2023-05-22 06:46:23.000000 krutils-0.20230522.1605/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:19:14.114298 krutils-0.20230522.1619/
+-rw-rw-rw-   0        0        0      526 2023-05-22 07:19:14.112358 krutils-0.20230522.1619/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1619/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 07:19:13.899955 krutils-0.20230522.1619/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1619/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1619/krutils/CONST.py
+-rw-rw-rw-   0        0        0       94 2023-05-22 07:06:16.000000 krutils-0.20230522.1619/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1619/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2697 2023-05-22 07:18:54.000000 krutils-0.20230522.1619/krutils/futils.py
+-rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230522.1619/krutils/logger.py
+-rw-rw-rw-   0        0        0    18549 2023-05-22 06:46:23.000000 krutils-0.20230522.1619/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:19:14.095688 krutils-0.20230522.1619/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-22 07:19:13.000000 krutils-0.20230522.1619/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-05-22 07:19:13.000000 krutils-0.20230522.1619/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:19:13.000000 krutils-0.20230522.1619/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 07:19:13.000000 krutils-0.20230522.1619/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 07:19:13.000000 krutils-0.20230522.1619/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:19:14.114298 krutils-0.20230522.1619/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-22 07:19:12.000000 krutils-0.20230522.1619/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:19:14.109568 krutils-0.20230522.1619/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230522.1619/test/test_futils.py
+-rw-rw-rw-   0        0        0      308 2023-05-22 06:46:23.000000 krutils-0.20230522.1619/test/test_logger.py
```

### Comparing `krutils-0.20230522.1605/PKG-INFO` & `krutils-0.20230522.1619/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1605
+Version: 0.20230522.1619
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1605/krutils/CONST.py` & `krutils-0.20230522.1619/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1605/krutils/_dbmgr.py` & `krutils-0.20230522.1619/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1605/krutils/futils.py` & `krutils-0.20230522.1619/krutils/futils.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,7 +49,76 @@
                 curr_dir = os.path.abspath(os.path.join(curr_dir, '..'))
 
     # print("find_first_file_to_root() -> [{0}]".format(file_path))
     return file_path
 
 
 
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+##########################################
+##      DATA 형식으로 변환
+##########################################
+def get_json_file_path_fr(file_name: str) -> dict():
+
+    if file_name == None or len(file_name.strip()) == 0:
+        raise Exception('찾고자하는 파일명을 입력해 주세요')
+
+    data_file_path = get_file_path_fr(file_name)
+
+    if (data_file_path == None):
+        raise Exception('지정한 파일을 찾을 수 없습니다 [{0}]'.format(file_name))
+
+    import json
+    with open(account) as af:
+        json_data = json.load(af)
+
+    return json_data
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `krutils-0.20230522.1605/krutils/logger.py` & `krutils-0.20230522.1619/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1605/krutils/utils.py` & `krutils-0.20230522.1619/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1605/krutils.egg-info/PKG-INFO` & `krutils-0.20230522.1619/krutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1605
+Version: 0.20230522.1619
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1605/setup.py` & `krutils-0.20230522.1619/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1605",
+    version="0.20230522.1619",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

