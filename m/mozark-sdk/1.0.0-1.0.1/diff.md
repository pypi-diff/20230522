# Comparing `tmp/mozark_sdk-1.0.0.tar.gz` & `tmp/mozark_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozark_sdk-1.0.0.tar", last modified: Mon May 22 11:11:36 2023, max compression
+gzip compressed data, was "mozark_sdk-1.0.1.tar", last modified: Mon May 22 12:10:24 2023, max compression
```

## Comparing `mozark_sdk-1.0.0.tar` & `mozark_sdk-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1062 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/LICENSE.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/PKG-INFO
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     7542 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/README.md
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/mozark_sdk/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        0 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/__init__.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    40977 2023-05-22 11:03:25.000000 mozark_sdk-1.0.0/mozark_sdk/client.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     4737 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/device.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    17986 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/executetest.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    14359 2023-05-22 11:06:07.000000 mozark_sdk-1.0.0/mozark_sdk/file.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     3926 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/project.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      778 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/schedule.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    31570 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/test_analytics.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     6704 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/tray.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      877 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/user.py
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/mozark_sdk.egg-info/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      431 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        1 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       37 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/requires.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       11 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/top_level.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       79 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/setup.cfg
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1483 2023-05-22 11:08:22.000000 mozark_sdk-1.0.0/setup.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 12:10:24.056285 mozark_sdk-1.0.1/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1062 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/LICENSE.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 12:10:24.056285 mozark_sdk-1.0.1/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     7542 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/README.md
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 12:10:24.056285 mozark_sdk-1.0.1/mozark_sdk/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        0 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/__init__.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    40977 2023-05-22 11:03:25.000000 mozark_sdk-1.0.1/mozark_sdk/client.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     4737 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/device.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    17986 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/executetest.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    14363 2023-05-22 12:07:18.000000 mozark_sdk-1.0.1/mozark_sdk/file.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     3926 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/project.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      778 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/schedule.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    31570 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/test_analytics.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     6704 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/tray.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      877 2023-05-21 06:48:24.000000 mozark_sdk-1.0.1/mozark_sdk/user.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 12:10:24.056285 mozark_sdk-1.0.1/mozark_sdk.egg-info/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 12:10:24.000000 mozark_sdk-1.0.1/mozark_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      431 2023-05-22 12:10:24.000000 mozark_sdk-1.0.1/mozark_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        1 2023-05-22 12:10:24.000000 mozark_sdk-1.0.1/mozark_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       37 2023-05-22 12:10:24.000000 mozark_sdk-1.0.1/mozark_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       11 2023-05-22 12:10:24.000000 mozark_sdk-1.0.1/mozark_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       79 2023-05-22 12:10:24.056285 mozark_sdk-1.0.1/setup.cfg
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1483 2023-05-22 12:09:25.000000 mozark_sdk-1.0.1/setup.py
```

### Comparing `mozark_sdk-1.0.0/LICENSE.txt` & `mozark_sdk-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/PKG-INFO` & `mozark_sdk-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozark_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark_sdk-1.0.0/README.md` & `mozark_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/client.py` & `mozark_sdk-1.0.1/mozark_sdk/client.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/device.py` & `mozark_sdk-1.0.1/mozark_sdk/device.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/executetest.py` & `mozark_sdk-1.0.1/mozark_sdk/executetest.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/file.py` & `mozark_sdk-1.0.1/mozark_sdk/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,18 +141,18 @@
             if response.json()['status'] == 409:
                 return "Error: File `" + file_name + "` already exists."
         else:
             return "Error: " + response.text
 
         s3_file_upload_url = response.json()['data']['uploadUrl']
 
-        print("\n s3 link: ", s3_file_upload_url)
+        # print("\n s3 link: ", s3_file_upload_url)
         # Leg 2 - upload the file using s3 upload URL
         response = requests.put(s3_file_upload_url, files=files)
-        print("\n s3 response: ", response)
+        # print("\n s3 response: ", response)
         if response.status_code == 200:
             return "Success: File `" + file_name + "` uploaded successfully."
         else:
             return "Failure: File `" + file_name + "` not uploaded."
 
     def get_file_info_list(self, file_category=None, project_name=None):
         new_headers = {'Authorization': "Bearer " + self.config.get("api_access_token"),
```

### Comparing `mozark_sdk-1.0.0/mozark_sdk/project.py` & `mozark_sdk-1.0.1/mozark_sdk/project.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/schedule.py` & `mozark_sdk-1.0.1/mozark_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/test_analytics.py` & `mozark_sdk-1.0.1/mozark_sdk/test_analytics.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/tray.py` & `mozark_sdk-1.0.1/mozark_sdk/tray.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk/user.py` & `mozark_sdk-1.0.1/mozark_sdk/user.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-1.0.0/mozark_sdk.egg-info/PKG-INFO` & `mozark_sdk-1.0.1/mozark_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozark-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark_sdk-1.0.0/setup.py` & `mozark_sdk-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # from distutils.core import setup
 from setuptools import setup
 
 setup(
     name='mozark_sdk',
     packages=['mozark_sdk'],
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     description='Automation test APIs',
     author='Mozark',
     author_email='mozark-aws-staging@mozark.ai',
     url='https://mozark.ai',
     # download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     # long_description_content_type = "text/markdown",
```

