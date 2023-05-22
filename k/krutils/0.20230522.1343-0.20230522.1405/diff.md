# Comparing `tmp/krutils-0.20230522.1343.tar.gz` & `tmp/krutils-0.20230522.1405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1343.tar", last modified: Mon May 22 04:43:52 2023, max compression
+gzip compressed data, was "krutils-0.20230522.1405.tar", last modified: Mon May 22 05:05:21 2023, max compression
```

## Comparing `krutils-0.20230522.1343.tar` & `krutils-0.20230522.1405.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:43:52.437324 krutils-0.20230522.1343/
--rw-rw-rw-   0        0        0      526 2023-05-22 04:43:52.436167 krutils-0.20230522.1343/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1343/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:43:52.410446 krutils-0.20230522.1343/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1343/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1343/krutils/CONST.py
--rw-rw-rw-   0        0        0       96 2023-05-22 04:22:41.000000 krutils-0.20230522.1343/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1343/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1343/krutils/logger.py
--rw-rw-rw-   0        0        0    21579 2023-05-22 04:38:05.000000 krutils-0.20230522.1343/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:43:52.432797 krutils-0.20230522.1343/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 04:43:52.000000 krutils-0.20230522.1343/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-22 04:43:52.000000 krutils-0.20230522.1343/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:43:52.000000 krutils-0.20230522.1343/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 04:43:52.000000 krutils-0.20230522.1343/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 04:43:52.000000 krutils-0.20230522.1343/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 04:43:52.437757 krutils-0.20230522.1343/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 04:43:51.000000 krutils-0.20230522.1343/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:43:52.434772 krutils-0.20230522.1343/test/
--rw-rw-rw-   0        0        0      316 2023-05-22 04:37:45.000000 krutils-0.20230522.1343/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:05:21.353653 krutils-0.20230522.1405/
+-rw-rw-rw-   0        0        0      526 2023-05-22 05:05:21.352348 krutils-0.20230522.1405/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1405/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 05:05:21.233267 krutils-0.20230522.1405/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1405/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1405/krutils/CONST.py
+-rw-rw-rw-   0        0        0       96 2023-05-22 04:22:41.000000 krutils-0.20230522.1405/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1405/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230522.1405/krutils/logger.py
+-rw-rw-rw-   0        0        0    21472 2023-05-22 04:57:29.000000 krutils-0.20230522.1405/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:05:21.337687 krutils-0.20230522.1405/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-22 05:05:20.000000 krutils-0.20230522.1405/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-22 05:05:21.000000 krutils-0.20230522.1405/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 05:05:20.000000 krutils-0.20230522.1405/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 05:05:20.000000 krutils-0.20230522.1405/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 05:05:20.000000 krutils-0.20230522.1405/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 05:05:21.354487 krutils-0.20230522.1405/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-22 05:05:20.000000 krutils-0.20230522.1405/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 05:05:21.342249 krutils-0.20230522.1405/test/
+-rw-rw-rw-   0        0        0      316 2023-05-22 04:37:45.000000 krutils-0.20230522.1405/test/test_logger.py
```

### Comparing `krutils-0.20230522.1343/PKG-INFO` & `krutils-0.20230522.1405/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1343
+Version: 0.20230522.1405
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1343/krutils/CONST.py` & `krutils-0.20230522.1405/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1343/krutils/_dbmgr.py` & `krutils-0.20230522.1405/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1343/krutils/logger.py` & `krutils-0.20230522.1405/krutils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,15 @@
 
         caller_path = ____file__
 
         # 인자로 받은 호출자 경로로 부터 root까지 탐색하며 config 파일을 찾는다.
         # 존재시 설정을 덮어 씌운다
         cfp = _logger_util().find_config_file_path(caller_path)
 
-        if (is_empty(cfp) != True):
+        if (cfp != None and len(cfp.strip()) > 0):
             parsed_config = _logger_util().parse_config_file(cfp)
 
             if (parsed_config != None):
                 self.config = parsed_config
                 self.config.CONFIG_FILE_PATH = cfp
```

### Comparing `krutils-0.20230522.1343/krutils/utils.py` & `krutils-0.20230522.1405/krutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,25 +786,23 @@
 
     or
 
     from krutils import logger
     logger = logger(__file__)
     '''
 
-    # logger에 필요한 변수와 기능이 담겨있는 super 클래스를 초기화 한다.
-    super().__init__()
-
     caller_path = ____file__
 
-    if is_empty(caller_path):
+    if is_empty(caller_path) == True:
         caller_path = __file__
 
 
-    import logger
-    return logger.logger(caller_path)
+    from krutils import logger
+    return logger(caller_path)
+
```

### Comparing `krutils-0.20230522.1343/krutils.egg-info/PKG-INFO` & `krutils-0.20230522.1405/krutils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1343
+Version: 0.20230522.1405
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1343/setup.py` & `krutils-0.20230522.1405/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1343",
+    version="0.20230522.1405",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

