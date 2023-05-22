# Comparing `tmp/crossmark-jotform-api-0.3.3.tar.gz` & `tmp/crossmark-jotform-api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.3.3.tar", last modified: Sat May 20 20:29:00 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.3.4.tar", last modified: Mon May 22 18:55:12 2023, max compression
```

## Comparing `crossmark-jotform-api-0.3.3.tar` & `crossmark-jotform-api-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.387090 crossmark-jotform-api-0.3.3/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-05-20 20:29:00.385892 crossmark-jotform-api-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.3/README.md
--rw-rw-rw-   0        0        0      789 2023-05-20 20:25:57.000000 crossmark-jotform-api-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 20:29:00.387090 crossmark-jotform-api-0.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.372732 crossmark-jotform-api-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.376894 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12743 2023-05-20 20:25:52.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.382895 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2770 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.383893 crossmark-jotform-api-0.3.3/test/
--rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.3/test/test_jotform_class.py
+drwxrwxrwx   0        0        0        0 2023-05-22 18:55:12.215830 crossmark-jotform-api-0.3.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     2895 2023-05-22 18:55:12.214830 crossmark-jotform-api-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-05-22 18:54:36.000000 crossmark-jotform-api-0.3.4/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-22 18:53:54.000000 crossmark-jotform-api-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 18:55:12.215830 crossmark-jotform-api-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 18:55:12.182830 crossmark-jotform-api-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 18:55:12.194828 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12761 2023-05-22 18:53:23.000000 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-22 18:55:12.211829 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2895 2023-05-22 18:55:12.000000 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-22 18:55:12.000000 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 18:55:12.000000 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-22 18:55:12.000000 crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 18:55:12.213833 crossmark-jotform-api-0.3.4/test/
+-rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.4/test/test_jotform_class.py
```

### Comparing `crossmark-jotform-api-0.3.3/LICENSE` & `crossmark-jotform-api-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.3/PKG-INFO` & `crossmark-jotform-api-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,7 +42,10 @@
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
 - 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
 - 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
+- 2023-05-22: 
+  * change of default submission value return from none to 1, 
+  * default timeout form 30 secs to 45 secs
```

### Comparing `crossmark-jotform-api-0.3.3/README.md` & `crossmark-jotform-api-0.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,11 @@
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
 - 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
-- 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
+- 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
+- 2023-05-22: 
+  * change of default submission value return from none to 1, 
+  * default timeout form 30 secs to 45 secs
```

### Comparing `crossmark-jotform-api-0.3.3/pyproject.toml` & `crossmark-jotform-api-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.3.4/src/crossmark_jotform_api/jotForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC
 import requests
 from datetime import datetime
 from urllib.parse import quote
 
 
 class JotForm(ABC):
-    def __init__(self, api_key, form_id, timeout=30, debug=False):
+    def __init__(self, api_key, form_id, timeout=45, debug=False):
         self.update_timestamp = datetime.now().timestamp()
         self.api_key = api_key
         self.form_id = form_id
         self.url = "https://api.jotform.com/form/" + form_id + \
             "/submissions?limit=1000&apiKey=" + api_key
         self.set_url_param("offset", "0")
         self.submission_ids = set()
@@ -191,14 +191,15 @@
         else:
             return None
 
     def get_submissions_count(self):
         form = self.get_form()
         if form:
             return int(form['content']['count'])
+        return 1
 
     def update(self):
         if not self.updating_process:
             self.updating_process = True
             count = self.get_submissions_count()
             if count <= self.submission_count:
                 self.__print("[INFO] No new submissions.")
```

### Comparing `crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.3.4/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,7 +42,10 @@
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
 - 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
 - 2023-05-16: summary for get_form function, format document, cleared some of the self.update and its fucntionality for faster performance
+- 2023-05-22: 
+  * change of default submission value return from none to 1, 
+  * default timeout form 30 secs to 45 secs
```

