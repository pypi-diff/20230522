# Comparing `tmp/arequestsHelper-0.4.3.tar.gz` & `tmp/arequestsHelper-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arequestsHelper-0.4.3.tar", last modified: Tue May 16 10:00:48 2023, max compression
+gzip compressed data, was "arequestsHelper-0.4.4.tar", last modified: Mon May 22 16:26:03 2023, max compression
```

## Comparing `arequestsHelper-0.4.3.tar` & `arequestsHelper-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/LICENSE
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      365 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/README.md
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.283650 arequestsHelper-0.4.3/arequestsHelper/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       61 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/arequestsHelper/__init__.py
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     5287 2023-05-16 09:55:03.000000 arequestsHelper-0.4.3/arequestsHelper/arequestsHelper.py
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/arequestsHelper/errors.py
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/arequestsHelper.egg-info/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/requires.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/top_level.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/setup.cfg
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1757 2023-05-16 10:00:42.000000 arequestsHelper-0.4.3/setup.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-22 16:26:03.031681 arequestsHelper-0.4.4/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2023-05-07 16:38:56.000000 arequestsHelper-0.4.4/LICENSE
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-22 16:26:03.031681 arequestsHelper-0.4.4/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      365 2023-05-07 16:38:56.000000 arequestsHelper-0.4.4/README.md
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-22 16:26:03.031681 arequestsHelper-0.4.4/arequestsHelper/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       61 2023-05-07 16:38:56.000000 arequestsHelper-0.4.4/arequestsHelper/__init__.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     5823 2023-05-22 16:24:52.000000 arequestsHelper-0.4.4/arequestsHelper/arequestsHelper.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2023-05-07 16:38:56.000000 arequestsHelper-0.4.4/arequestsHelper/errors.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-22 16:26:03.031681 arequestsHelper-0.4.4/arequestsHelper.egg-info/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-22 16:26:02.000000 arequestsHelper-0.4.4/arequestsHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-05-22 16:26:03.000000 arequestsHelper-0.4.4/arequestsHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-05-22 16:26:02.000000 arequestsHelper-0.4.4/arequestsHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-05-22 16:26:02.000000 arequestsHelper-0.4.4/arequestsHelper.egg-info/requires.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-05-22 16:26:02.000000 arequestsHelper-0.4.4/arequestsHelper.egg-info/top_level.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-05-22 16:26:03.032681 arequestsHelper-0.4.4/setup.cfg
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1757 2023-05-22 15:54:43.000000 arequestsHelper-0.4.4/setup.py
```

### Comparing `arequestsHelper-0.4.3/LICENSE` & `arequestsHelper-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arequestsHelper-0.4.3/PKG-INFO` & `arequestsHelper-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.3
+Version: 0.4.4
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.4.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.3/arequestsHelper/arequestsHelper.py` & `arequestsHelper-0.4.4/arequestsHelper/arequestsHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,24 @@
     async def get_json_get(self,client: aiohttp.ClientSession, url: str,proxy,force_json = False) -> dict:
         if proxy == None: 
             async with client.request('GET', url,ssl=False,timeout=30) as response:
                 return await self.errors_catcher(response, force_json)
         else: 
             async with client.request('GET', url,proxy=proxy[0], proxy_auth=proxy[1],ssl=False,timeout=30) as response:
                 return await self.errors_catcher(response, force_json)
-        
+    
+    
+    async def get_json_patch(self,client: aiohttp.ClientSession, url: str,data, proxy,force_json = False) -> dict:
+        if proxy == None: 
+            async with client.request('patch', url, data = data, ssl=False) as response:
+                return await self.errors_catcher(response, force_json)
+        else: 
+            async with client.request('patch', url, data = data,proxy=proxy[0], proxy_auth=proxy[1], ssl=False) as response:
+                return await self.errors_catcher(response, force_json)
+            
 
     async def errors_catcher(self,response, force_json = False): 
         content_type = response.headers['Content-Type']
         # print(response)
         try: 
             resp = await response.json(content_type=None)
         except:
```

### Comparing `arequestsHelper-0.4.3/arequestsHelper.egg-info/PKG-INFO` & `arequestsHelper-0.4.4/arequestsHelper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.3
+Version: 0.4.4
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.4.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.3/setup.py` & `arequestsHelper-0.4.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'arequestsHelper',         # How you named your package folder (MyLib)
   packages = ['arequestsHelper'],   # Chose the same as "name"
-  version = '0.4.3',      # Start with a small number and increase it with every change you make
+  version = '0.4.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "This pakage helps to work with aiohttp requests in many threads",   # Give a short description about your library
   author = 'Vitalii Haruk',                   # Type in your name
   author_email = "garuk1vitalik@gmail.com",      # Type in your E-Mail
   url = "https://github.com/Harukvitalii",   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip',    # I explain this later on
+  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.4.zip',    # I explain this later on
   keywords = ['aiohttp', 'requests', 'threads'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
           'aiohttp',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

