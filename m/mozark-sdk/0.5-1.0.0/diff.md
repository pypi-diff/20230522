# Comparing `tmp/mozark-sdk-0.5.tar.gz` & `tmp/mozark_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozark-sdk-0.5.tar", last modified: Tue Apr 11 06:32:40 2023, max compression
+gzip compressed data, was "mozark_sdk-1.0.0.tar", last modified: Mon May 22 11:11:36 2023, max compression
```

## Comparing `mozark-sdk-0.5.tar` & `mozark_sdk-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.627141 mozark-sdk-0.5/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1062 2023-04-01 18:14:03.000000 mozark-sdk-0.5/LICENSE.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      842 2023-04-11 06:32:40.627141 mozark-sdk-0.5/PKG-INFO
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     7542 2023-04-01 18:14:03.000000 mozark-sdk-0.5/README.md
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.623141 mozark-sdk-0.5/mozark-sdk/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        0 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/__init__.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    39744 2023-04-06 08:34:52.000000 mozark-sdk-0.5/mozark-sdk/client.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     4737 2023-04-05 09:59:13.000000 mozark-sdk-0.5/mozark-sdk/device.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    17986 2023-04-06 08:38:18.000000 mozark-sdk-0.5/mozark-sdk/executetest.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    11228 2023-04-05 06:30:41.000000 mozark-sdk-0.5/mozark-sdk/file.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     3926 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/project.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      778 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/schedule.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    31570 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/test_analytics.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     6704 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/tray.py
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      877 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/user.py
-drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.627141 mozark-sdk-0.5/mozark_sdk.egg-info/
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      842 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      431 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        1 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       37 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/requires.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       11 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/top_level.txt
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       79 2023-04-11 06:32:40.627141 mozark-sdk-0.5/setup.cfg
--rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1481 2023-04-11 06:28:39.000000 mozark-sdk-0.5/setup.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1062 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/LICENSE.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     7542 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/README.md
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/mozark_sdk/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        0 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/__init__.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    40977 2023-05-22 11:03:25.000000 mozark_sdk-1.0.0/mozark_sdk/client.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     4737 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/device.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    17986 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/executetest.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    14359 2023-05-22 11:06:07.000000 mozark_sdk-1.0.0/mozark_sdk/file.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     3926 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/project.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      778 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/schedule.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    31570 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/test_analytics.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     6704 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/tray.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      877 2023-05-21 06:48:24.000000 mozark_sdk-1.0.0/mozark_sdk/user.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/mozark_sdk.egg-info/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      844 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      431 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        1 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       37 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       11 2023-05-22 11:11:36.000000 mozark_sdk-1.0.0/mozark_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       79 2023-05-22 11:11:36.586339 mozark_sdk-1.0.0/setup.cfg
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1483 2023-05-22 11:08:22.000000 mozark_sdk-1.0.0/setup.py
```

### Comparing `mozark-sdk-0.5/LICENSE.txt` & `mozark_sdk-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/PKG-INFO` & `mozark_sdk-1.0.0/mozark_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozark-sdk
-Version: 0.5
+Version: 1.0.0
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark-sdk-0.5/README.md` & `mozark_sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/client.py` & `mozark_sdk-1.0.0/mozark_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,50 @@
 
             Note: "projectName" will be present in response if passed in a filter, else the value will be ""
         """
         file = File(client=self)
         app_list = file.get_application_list(file_category=file_category, project_name=project_name)
         return app_list
 
+    def get_application_list_all(self):
+        """ Returns list of all application file information
+
+        Args:
+            file_category (str): mandatory 'android-application' or 'ios-application'
+            project_name (str): optional project_name to filter the android application files
+
+        Returns:
+            fileinfo (list): dictionary containing the metadata about the file
+
+            [
+                {
+                    "fileName" : "",
+                    "fileCategory": "android-application",
+                    "md5": "",
+                    "fileURL": "",
+                    "fileUUID": "",
+                    "packageName": "",
+                    "projectName": ""
+                },
+                {
+                    "fileName" : "",
+                    "fileCategory": "ios-application",
+                    "md5": "",
+                    "fileURL": "",
+                    "fileUUID": "",
+                    "projectName": ""
+                }
+            ]
+
+            Note: "projectName" will be present in response if passed in a filter, else the value will be ""
+        """
+        file = File(client=self)
+        app_list = file.get_application_list_all()
+        return app_list
+
     # Native Test Application
 
     def upload_native_test_application(self, file_category=None, project_name=None, file_path=None):
         """ Upload native test application(.apk or .ipa) from given file path
 
         Args:
             file_category (str): Mandatory 'android-application' or 'ios-application'
```

### Comparing `mozark-sdk-0.5/mozark-sdk/device.py` & `mozark_sdk-1.0.0/mozark_sdk/device.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/executetest.py` & `mozark_sdk-1.0.0/mozark_sdk/executetest.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/file.py` & `mozark_sdk-1.0.0/mozark_sdk/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,27 +86,29 @@
             for f in status_message:
                 if f["fileCategory"] == "android-application" or f["fileCategory"] == "ios-application":
                     status_message_filtered.append(f)
             return status_message_filtered
         except TypeError:
             return "Error: Project Name or File Name doesn't exist"
 
+    def get_application_list_all(self):
+        status_message = self.get_file_info_list_all()
+        return status_message
     # Native Test Application
 
     def upload_native_test_application(self, file_category=None, project_name=None, file_path=None):
         status_message = self.upload_application(self, file_category=file_category,
                                                  project_name=project_name,
                                                  file_path=file_path)
         return status_message
 
     def get_native_test_application_info(self, file_name=None):
         status_message = self.get_application_info(file_name=file_name)
         return status_message
 
-
     def get_native_test_application_list(self, file_category=None, project_name=None):
         status_message = self.get_file_info_list(file_category=file_category, project_name=project_name)
         status_message_filtered = []
         try:
             for f in status_message:
                 if f["fileCategory"] == "android-test-application" or f["fileCategory"] == "ios-test-application":
                     status_message_filtered.append(f)
@@ -122,15 +124,14 @@
                 file_bytes = f.read()  # read file as bytes
                 readable_hash = hashlib.md5(file_bytes).hexdigest()
                 md5_hash = readable_hash
             return md5_hash
         except FileNotFoundError:
             return "Error: No such file or directory "
 
-
     def __upload(self, data=None, files=None):
         new_headers = {'Authorization': "Bearer " + self.config.get("api_access_token"),
                        'Content-Type': 'application/json'}
 
         file_api_url = self.config.get("api_url") + "testexecute/files"
         file_name = data["fileName"]
         # Leg 1 - get the s3 file upload URL
@@ -140,17 +141,18 @@
             if response.json()['status'] == 409:
                 return "Error: File `" + file_name + "` already exists."
         else:
             return "Error: " + response.text
 
         s3_file_upload_url = response.json()['data']['uploadUrl']
 
+        print("\n s3 link: ", s3_file_upload_url)
         # Leg 2 - upload the file using s3 upload URL
         response = requests.put(s3_file_upload_url, files=files)
-
+        print("\n s3 response: ", response)
         if response.status_code == 200:
             return "Success: File `" + file_name + "` uploaded successfully."
         else:
             return "Failure: File `" + file_name + "` not uploaded."
 
     def get_file_info_list(self, file_category=None, project_name=None):
         new_headers = {'Authorization': "Bearer " + self.config.get("api_access_token"),
@@ -212,14 +214,69 @@
                                  "fileUUID": f['uuid'],
                                  "XCTestRunFileUrl": f['fileParameters']['xctestrunFileUrl'],
                                  "projectName": project_name
                                  }
                     return_message.append(file_info)
             return return_message
 
+    def get_file_info_list_all(self):
+        new_headers = {'Authorization': "Bearer " + self.config.get("api_access_token"),
+                       'Content-Type': 'application/json'}
+
+        file_api_url = self.config.get("api_url") + "testexecute/files"
+        # Fetch list of files uploaded
+        response = requests.get(file_api_url, headers=new_headers)
+
+        file_list = response.json()['data']['list']
+        return_message = []
+
+        if len(file_list) > 0:
+            for f in file_list:
+                file_category = f['fileCategory']
+                if file_category == 'android-application':
+                    file_info = {"fileName": f['fileName'],
+                                 "fileCategory": f['fileCategory'],
+                                 "md5": f['meta']['md5sum'],
+                                 "fileURL": f['meta']['s3Url'],
+                                 "fileUUID": f['uuid'],
+                                 "projectName": ""
+                                 }
+                    return_message.append(file_info)
+                elif file_category == 'ios-application':
+                    file_info = {"fileName": f['fileName'],
+                                 "fileCategory": f['fileCategory'],
+                                 "md5": f['meta']['md5sum'],
+                                 "fileURL": f['meta']['s3Url'],
+                                 "fileUUID": f['uuid'],
+                                 "projectName": ""
+                                 }
+                    return_message.append(file_info)
+                elif file_category == 'android-test-application':
+                    file_info = {"fileName": f['fileName'],
+                                 "fileCategory": f['fileCategory'],
+                                 "md5": f['meta']['md5sum'],
+                                 "fileURL": f['meta']['s3Url'],
+                                 "fileUUID": f['uuid'],
+                                 "testCodePackageName": f['fileParameters']['testCodePackageName'],
+                                 "testRunnerName": f['fileParameters']['testRunnerName'],
+                                 "projectName": ""
+                                 }
+                    return_message.append(file_info)
+                elif file_category == 'ios-test-application':
+                    file_info = {"fileName": f['fileName'],
+                                 "fileCategory": f['fileCategory'],
+                                 "md5": f['meta']['md5sum'],
+                                 "fileURL": f['meta']['s3Url'],
+                                 "fileUUID": f['uuid'],
+                                 "XCTestRunFileUrl": f['fileParameters']['xctestrunFileUrl'],
+                                 "projectName": ""
+                                 }
+                    return_message.append(file_info)
+            return return_message
+
     def delete_file(self, file_name=None):
         new_headers = {'Authorization': "Bearer " + self.config.get("api_access_token"),
                        'Content-Type': 'application/json'}
 
         file_info = self.get_application_info(file_name=file_name)
         try:
             file_api_url = self.config.get("api_url") + "testexecute/files?fileId=" + file_info["fileUUID"]
```

### Comparing `mozark-sdk-0.5/mozark-sdk/project.py` & `mozark_sdk-1.0.0/mozark_sdk/project.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/schedule.py` & `mozark_sdk-1.0.0/mozark_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/test_analytics.py` & `mozark_sdk-1.0.0/mozark_sdk/test_analytics.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/tray.py` & `mozark_sdk-1.0.0/mozark_sdk/tray.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark-sdk/user.py` & `mozark_sdk-1.0.0/mozark_sdk/user.py`

 * *Files identical despite different names*

### Comparing `mozark-sdk-0.5/mozark_sdk.egg-info/PKG-INFO` & `mozark_sdk-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mozark-sdk
-Version: 0.5
+Name: mozark_sdk
+Version: 1.0.0
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark-sdk-0.5/setup.py` & `mozark_sdk-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # from distutils.core import setup
 from setuptools import setup
 
 setup(
-    name='mozark-sdk',
-    packages=['mozark-sdk'],
-    version='0.5',
+    name='mozark_sdk',
+    packages=['mozark_sdk'],
+    version='1.0.0',
     license='MIT',
     description='Automation test APIs',
     author='Mozark',
     author_email='mozark-aws-staging@mozark.ai',
     url='https://mozark.ai',
     # download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     # long_description_content_type = "text/markdown",
```

