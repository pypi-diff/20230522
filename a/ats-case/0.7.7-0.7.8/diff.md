# Comparing `tmp/ats_case-0.7.7.tar.gz` & `tmp/ats_case-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.7.7.tar", last modified: Mon May 22 01:25:12 2023, max compression
+gzip compressed data, was "ats_case-0.7.8.tar", last modified: Mon May 22 06:57:58 2023, max compression
```

## Comparing `ats_case-0.7.7.tar` & `ats_case-0.7.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:12.080151 ats_case-0.7.7/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-22 01:25:12.076160 ats_case-0.7.7/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:11.485723 ats_case-0.7.7/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.7/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:11.863730 ats_case-0.7.7/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.7/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18348 2023-05-22 01:24:16.000000 ats_case-0.7.7/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11101 2023-05-18 05:15:05.000000 ats_case-0.7.7/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.7/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.7.7/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:11.937533 ats_case-0.7.7/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.7/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.7/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.7/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:12.017318 ats_case-0.7.7/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.7/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.7/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.7/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:12.066187 ats_case-0.7.7/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.7/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2473 2023-05-18 05:24:57.000000 ats_case-0.7.7/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-22 01:25:11.727079 ats_case-0.7.7/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-22 01:25:10.000000 ats_case-0.7.7/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-22 01:25:10.000000 ats_case-0.7.7/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 01:25:10.000000 ats_case-0.7.7/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-22 01:25:10.000000 ats_case-0.7.7/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 01:25:10.000000 ats_case-0.7.7/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 01:25:12.081147 ats_case-0.7.7/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-22 01:25:03.000000 ats_case-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.641798 ats_case-0.7.8/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-22 06:57:58.639836 ats_case-0.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.253261 ats_case-0.7.8/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.8/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.469134 ats_case-0.7.8/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.8/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18505 2023-05-22 06:55:42.000000 ats_case-0.7.8/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11101 2023-05-18 05:15:05.000000 ats_case-0.7.8/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.8/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.7.8/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.533909 ats_case-0.7.8/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.8/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.8/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.8/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.592933 ats_case-0.7.8/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.8/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.8/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.8/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.630828 ats_case-0.7.8/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.8/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2473 2023-05-18 05:24:57.000000 ats_case-0.7.8/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-22 06:57:58.350731 ats_case-0.7.8/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-22 06:57:57.000000 ats_case-0.7.8/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-22 06:57:57.000000 ats_case-0.7.8/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:57:57.000000 ats_case-0.7.8/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-22 06:57:57.000000 ats_case-0.7.8/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 06:57:57.000000 ats_case-0.7.8/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:57:58.642795 ats_case-0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-22 06:57:25.000000 ats_case-0.7.8/setup.py
```

### Comparing `ats_case-0.7.7/PKG-INFO` & `ats_case-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.7.7
+Version: 0.7.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.7/README.md` & `ats_case-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/case/command.py` & `ats_case-0.7.8/ats_case/case/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,14 +380,15 @@
         self._parameter = None
         self._function = None
         self._interval = None
         self._result = None
         self._exec_times = 0
         self._sleep = 0
         self._expect_result = None
+        self._func_parameter = {}
 
     def operation(self, command: str):
         self._operation = command
         return self
 
     def parameter(self, param=None):
         self._parameter = param
@@ -403,14 +404,15 @@
 
     def interval(self, times=0):
         self._interval = times
         return self
 
     def compare(self, data):
         self._expect_result = data.get('expect_result', None)
+        self._func_parameter = data.get('parameter', {})
 
         return self
 
     def encode(self, context: Context):
         logger.info(
             '~ @BENCH-> manufacture:{} operation:{} parameter:{}'.format(context.bench.manufacture, self._operation,
                                                                          self._parameter))
@@ -440,14 +442,15 @@
     def acv(self, context: Context):
         data = func.to_dict(result=self._result)
         try:
             if self._expect_result is None:
                 data['expect_result'] = context.runtime.steps[context.runtime.step - 1]
             else:
                 data['expect_result'] = context.runtime.steps[int(self._expect_result)]
+            data['parameter'] = _replace(self._func_parameter)
         except:
             pass
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             'bench', self._operation, self._result))
         result = udm.handle(module='bench', function=self._operation
                             , data=data, debug_url=context.acd_url)
```

### Comparing `ats_case-0.7.7/ats_case/case/context.py` & `ats_case-0.7.8/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/case/executor.py` & `ats_case-0.7.8/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/case/translator.py` & `ats_case-0.7.8/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/common/error.py` & `ats_case-0.7.8/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/manage/core.py` & `ats_case-0.7.8/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/manage/start.py` & `ats_case-0.7.8/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case/template/testcase_v1.tmp` & `ats_case-0.7.8/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/ats_case.egg-info/PKG-INFO` & `ats_case-0.7.8/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.7.7
+Version: 0.7.8
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.7.7/ats_case.egg-info/SOURCES.txt` & `ats_case-0.7.8/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.7.7/setup.py` & `ats_case-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.7.7",
+    version="0.7.8",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

