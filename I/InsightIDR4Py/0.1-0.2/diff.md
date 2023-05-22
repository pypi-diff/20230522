# Comparing `tmp/InsightIDR4Py-0.1.tar.gz` & `tmp/InsightIDR4Py-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InsightIDR4Py-0.1.tar", last modified: Mon May 22 17:21:45 2023, max compression
+gzip compressed data, was "InsightIDR4Py-0.2.tar", last modified: Mon May 22 18:25:03 2023, max compression
```

## Comparing `InsightIDR4Py-0.1.tar` & `InsightIDR4Py-0.2.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 17:21:45.757893 InsightIDR4Py-0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-22 16:57:04.000000 InsightIDR4Py-0.1/LICENSE
--rw-rw-rw-   0        0        0     5811 2023-05-22 17:21:45.757893 InsightIDR4Py-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5393 2023-05-22 17:15:17.000000 InsightIDR4Py-0.1/README.md
--rw-rw-rw-   0        0        0       99 2023-05-22 16:55:58.000000 InsightIDR4Py-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-05-22 17:21:45.765911 InsightIDR4Py-0.1/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-05-22 17:21:41.000000 InsightIDR4Py-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:21:45.693886 InsightIDR4Py-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 17:21:45.709888 InsightIDR4Py-0.1/src/InsightIDR4Py/
--rw-rw-rw-   0        0        0    23819 2023-05-22 16:50:25.000000 InsightIDR4Py-0.1/src/InsightIDR4Py/InsightIDR4Py.py
--rw-rw-rw-   0        0        0        0 2023-05-21 23:14:06.000000 InsightIDR4Py-0.1/src/InsightIDR4Py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:21:45.757893 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/
--rw-rw-rw-   0        0        0     5811 2023-05-22 17:21:45.000000 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-22 17:21:45.000000 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 17:21:45.000000 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 17:21:45.000000 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 17:21:45.000000 InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/
+drwxrwxrwx   0        0        0        0 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/
+-rw-rw-rw-   0        0        0     5973 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 18:25:03.000000 InsightIDR4Py-0.2/InsightIDR4Py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23729 2023-05-22 18:17:07.000000 InsightIDR4Py-0.2/InsightIDR4Py.py
+-rw-rw-rw-   0        0        0     1092 2023-05-22 16:57:04.000000 InsightIDR4Py-0.2/LICENSE
+-rw-rw-rw-   0        0        0     5973 2023-05-22 18:25:03.122037 InsightIDR4Py-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5555 2023-05-22 17:35:51.000000 InsightIDR4Py-0.2/README.md
+-rw-rw-rw-   0        0        0       99 2023-05-22 16:55:58.000000 InsightIDR4Py-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-05-22 18:25:03.123037 InsightIDR4Py-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      692 2023-05-22 18:22:40.000000 InsightIDR4Py-0.2/setup.py
```

### Comparing `InsightIDR4Py-0.1/LICENSE` & `InsightIDR4Py-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `InsightIDR4Py-0.1/PKG-INFO` & `InsightIDR4Py-0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: InsightIDR4Py
-Version: 0.1
-Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
-Home-page: https://github.com/mbabinski/InsightIDR4Py
-Author: Micah Babinski
-Author-email: m.babinski.88@gmail.com
-License: MIT
-Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # InsightIDR4Py
 A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 
 InsightIDR4Py allows analysts to query log data from Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/), analyze it within Python, and/or feed it to other APIs like VirusTotal, AbuseIPDB, or others. This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
 
 InsightIDR4Py also offers access to some of the additional APIs in the InsightIDR ecosystem. These include:
 ## Investigations
@@ -35,14 +23,20 @@
 * Create Saved Query
 * Replace a Saved Query
 * Update a Saved Query
 * Delete a Saved Query
 
 Happy analyzing!:monocle_face:
 
+# Installation
+InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
+```
+pip install InsightIDR4Py
+```
+
 # Prerequisites
 You will need obtain an API key from the InsightIDR system. The documentation for this can be found [here](https://docs.rapid7.com/insight/managing-platform-api-keys/). From there, you'll use this API key value to create the InsightIDR API object as shown below:
 ```python
 import InsightIDR4Py as idr
 
 # define API key (store this value securely)
 api_key = "API_Key_Here"
@@ -144,8 +138,8 @@
 	print("----------")
 ```
 
 # License
 This repository is licensed under an [MIT license](https://github.com/mbabinski/InsightIDR4Py/blob/main/LICENSE), which grants extensive permission to use this material however you wish.
 
 # Contributing
-You are welcome to contribute however you wish! I appreciate feedback in any format.
+You are welcome to contribute however you wish! I appreciate feedback in any format.
```

### Comparing `InsightIDR4Py-0.1/README.md` & `InsightIDR4Py-0.2/InsightIDR4Py.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: InsightIDR4Py
+Version: 0.2
+Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
+Home-page: https://github.com/mbabinski/InsightIDR4Py
+Author: Micah Babinski
+Author-email: m.babinski.88@gmail.com
+License: MIT
+Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # InsightIDR4Py
 A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 
 InsightIDR4Py allows analysts to query log data from Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/), analyze it within Python, and/or feed it to other APIs like VirusTotal, AbuseIPDB, or others. This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
 
 InsightIDR4Py also offers access to some of the additional APIs in the InsightIDR ecosystem. These include:
 ## Investigations
@@ -23,14 +35,20 @@
 * Create Saved Query
 * Replace a Saved Query
 * Update a Saved Query
 * Delete a Saved Query
 
 Happy analyzing!:monocle_face:
 
+# Installation
+InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
+```
+pip install InsightIDR4Py
+```
+
 # Prerequisites
 You will need obtain an API key from the InsightIDR system. The documentation for this can be found [here](https://docs.rapid7.com/insight/managing-platform-api-keys/). From there, you'll use this API key value to create the InsightIDR API object as shown below:
 ```python
 import InsightIDR4Py as idr
 
 # define API key (store this value securely)
 api_key = "API_Key_Here"
@@ -132,8 +150,8 @@
 	print("----------")
 ```
 
 # License
 This repository is licensed under an [MIT license](https://github.com/mbabinski/InsightIDR4Py/blob/main/LICENSE), which grants extensive permission to use this material however you wish.
 
 # Contributing
-You are welcome to contribute however you wish! I appreciate feedback in any format.
+You are welcome to contribute however you wish! I appreciate feedback in any format.
```

### Comparing `InsightIDR4Py-0.1/setup.py` & `InsightIDR4Py-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="InsightIDR4Py",
-    version="0.1",
+    version="0.2",
     description="A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Micah Babinski",
     author_email="m.babinski.88@gmail.com",
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
+    py_modules=["InsightIDR4Py"],
     url="https://github.com/mbabinski/InsightIDR4Py",
     keywords="Rapid7, InsightIDR, SIEM, Logsearch, Investigations, Threats",
     install_requires=[
           "requests",
       ],
 
 )
```

### Comparing `InsightIDR4Py-0.1/src/InsightIDR4Py/InsightIDR4Py.py` & `InsightIDR4Py-0.2/InsightIDR4Py.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 import requests, json, time
 from datetime import datetime, timedelta, timezone
 
+def GetDefaultStartTime():
+    """
+    Get default start time for time-based queries.
+    """
+    default_start_time = (datetime.now(timezone.utc) - timedelta(28)).strftime("%Y-%m-%dT%H:%M:%SZ")
+
+    return default_start_time
+
+def GetDefaultEndTime():
+    """
+    Get default end time (now) for time-based queries.
+    """
+    default_end_time = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
+    
+    return default_end_time
+
 class InsightIDR(object):
     def __init__(self, api_key, region=None):
         self.session = requests.Session()
         self.session.headers = {"X-Api-Key": api_key}
         if not region:
             self.region = self._get_region()
         else:
@@ -22,31 +38,14 @@
         pass that in when creating the InsightIDR object.
         """
         self.regions = ["us", "us2", "us3", "eu", "ca", "au", "ap"]
         for region in self.regions:
             self.response = self.session.get("https://{}.rest.logs.insight.rapid7.com/management/logs".format(region))
             if self.response.status_code == 200:
                 return region
-
-    def GetDefaultStartTime(self):
-        """
-        Get default start time for time-based queries.
-        """
-        default_start_time = (datetime.now(timezone.utc) - timedelta(28)).strftime("%Y-%m-%dT%H:%M:%SZ")
-
-        return default_start_time
-
-    def GetDefaultEndTime(self):
-        """
-        Get default end time (now) for time-based queries.
-        """
-        default_end_time = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
-        
-        return default_end_time
-        
       
     def GetLogInfo(self):
         """Returns metadata about the available log sources."""
         response = self.session.get(self.log_mgmt_url).json()["logs"]
         
         return response
 
@@ -185,16 +184,16 @@
             value = int(result[key]["count"])
             groups[key] = value
 
         return groups
 
     def ListInvestigations(self,
                            assignee_email=None,
-                           start_time=self.GetDefaultStartTime(),
-                           end_time=self.GetDefaultEndTime(),
+                           start_time=GetDefaultStartTime(),
+                           end_time=GetDefaultEndTime(),
                            multi_customer=False,
                            priorities=["LOW", "MEDIUM", "HIGH", "CRITICAL"],
                            sort="priority,DESC",
                            sources=None,
                            statuses=["OPEN", "INVESTIGATING", "CLOSED"],
                            tags=None):
         """
@@ -276,16 +275,16 @@
         url = self.investigations_url
         self.session.headers["Accept-version"] = "investigations-preview"
         response = self.session.post(url, json=data)
         result = response.json()
 
         return result
 
-    def CloseInvestigationsInBulk(self, source, from_time=self.GetDefaultStartTime(),
-                                  to_time=self.GetDefaultEndTime(), alert_type=None,
+    def CloseInvestigationsInBulk(self, source, from_time=GetDefaultStartTime(),
+                                  to_time=GetDefaultEndTime(), alert_type=None,
                                   disposition=None, detection_rule_rrn=None,
                                   max_investigations_to_close=None):
         """
         Closes investigations in bulk according to selected criteria.
         """
         data = {
             "source": source.upper(),
```

### Comparing `InsightIDR4Py-0.1/src/InsightIDR4Py.egg-info/PKG-INFO` & `InsightIDR4Py-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InsightIDR4Py
-Version: 0.1
+Version: 0.2
 Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 Home-page: https://github.com/mbabinski/InsightIDR4Py
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 License: MIT
 Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
 Description-Content-Type: text/markdown
@@ -35,14 +35,20 @@
 * Create Saved Query
 * Replace a Saved Query
 * Update a Saved Query
 * Delete a Saved Query
 
 Happy analyzing!:monocle_face:
 
+# Installation
+InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
+```
+pip install InsightIDR4Py
+```
+
 # Prerequisites
 You will need obtain an API key from the InsightIDR system. The documentation for this can be found [here](https://docs.rapid7.com/insight/managing-platform-api-keys/). From there, you'll use this API key value to create the InsightIDR API object as shown below:
 ```python
 import InsightIDR4Py as idr
 
 # define API key (store this value securely)
 api_key = "API_Key_Here"
```

