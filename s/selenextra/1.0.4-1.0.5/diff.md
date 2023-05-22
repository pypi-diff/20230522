# Comparing `tmp/selenextra-1.0.4.tar.gz` & `tmp/selenextra-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-1.0.4.tar", last modified: Sun May 14 05:07:44 2023, max compression
+gzip compressed data, was "selenextra-1.0.5.tar", last modified: Mon May 22 06:05:06 2023, max compression
```

## Comparing `selenextra-1.0.4.tar` & `selenextra-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.561365 selenextra-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-14 05:05:34.000000 selenextra-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      627 2023-05-14 05:07:44.560364 selenextra-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-14 05:05:34.000000 selenextra-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.554380 selenextra-1.0.4/selenextra/
--rw-rw-rw-   0        0        0     4757 2023-05-14 05:06:55.000000 selenextra-1.0.4/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-05-14 05:05:34.000000 selenextra-1.0.4/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1030 2023-05-14 05:05:34.000000 selenextra-1.0.4/selenextra/patcher.py
-drwxrwxrwx   0        0        0        0 2023-05-14 05:07:44.560364 selenextra-1.0.4/selenextra.egg-info/
--rw-rw-rw-   0        0        0      627 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 05:07:44.000000 selenextra-1.0.4/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 05:07:44.561365 selenextra-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      782 2023-05-14 05:06:14.000000 selenextra-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.458127 selenextra-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-22 04:32:59.000000 selenextra-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:05:06.458127 selenextra-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-22 04:32:59.000000 selenextra-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.453140 selenextra-1.0.5/selenextra/
+-rw-rw-rw-   0        0        0     3967 2023-05-22 05:56:55.000000 selenextra-1.0.5/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-22 05:56:18.000000 selenextra-1.0.5/selenextra/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:05:06.457130 selenextra-1.0.5/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       74 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 06:05:06.000000 selenextra-1.0.5/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:05:06.458127 selenextra-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-05-22 06:04:51.000000 selenextra-1.0.5/setup.py
```

### Comparing `selenextra-1.0.4/LICENSE` & `selenextra-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-1.0.4/PKG-INFO` & `selenextra-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
```

### Comparing `selenextra-1.0.4/selenextra/__init__.py` & `selenextra-1.0.5/selenextra/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,29 @@
 from urllib.parse import urlparse
 from undetected_chromedriver import ChromeOptions
 from seleniumwire.undetected_chromedriver import Chrome
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
 from typing import Union, Callable, Any, List, Tuple
-from .patcher import CustomPatcher
 from .exceptions import *
 
 import json
 import re
 import random as rnd
 import time
 
 
 class ChromeDriver(Chrome):
     CONNECTION_TIMEOUT = 30
 
-    def __init__(self, user_multi_procs: bool = True, **kwargs) -> None:
-        self.custom_patcher = CustomPatcher(
-            executable_path=kwargs.get('driver_executable_path', None),
-            force=kwargs.get('patcher_force_close', False),
-            version_main=kwargs.get('version_main', None),
-            user_multi_procs=user_multi_procs
-        )
-
-        self.custom_patcher.auto()
-
-        release = self.custom_patcher.fetch_release_number()
-        version = release.version[0]
-
-        kwargs['driver_executable_path'] = self.custom_patcher.executable_path
+    def __init__(self, **kwargs) -> None:
         kwargs['seleniumwire_options'] = kwargs.get('seleniumwire_options', {})
         kwargs['seleniumwire_options']['mitm_http2'] = False
 
-        super().__init__(
-            version_main=version,
-            user_multi_procs=user_multi_procs,
-            **kwargs
-        )
+        super().__init__(**kwargs)
 
     def get_user_agent(self) -> str:
         return self.execute_script('return navigator.userAgent')
 
     def get_cookie_string(self) -> str:
         cookies = self.get_cookies()
         cookies = [f'{item["name"]}={item["value"]}' for item in cookies]
@@ -55,31 +37,30 @@
             self.get(url)
             
             request = self.wait_for_request('/ip')
             body = request.response.body.decode('utf-8')
             data = json.loads(body)
             ip = data['origin']
         except:
-            raise RequestException(f"Error retrieving IP address from {url}")
+            raise UnableToFetchIP
         
         return ip
 
     def callback_with_timeout(self, callback: Callable[[Tuple], Any], params: tuple, timeout: Union[int, float] = 30) -> Any:
         end_time = time.time() + timeout
 
         while time.time() < end_time:
             result = callback(*params)
 
             if not result:
                 continue
 
             return result
 
-        raise TimeoutException(
-            f'Callback execution timed out: {callback.__name__}')
+        raise TimeoutException(f'Callback execution timed out: {callback.__name__}')
 
     def _process_requests(self, callback: Callable[[Request, Response], Any]) -> Any:
         for request in self.requests:
             if not request.response:
                 continue
 
             response = request.response
@@ -131,9 +112,8 @@
         self.proxy = {
             'http': http_proxy,
             'https': proxy,
             'no_proxy': 'localhost,127.0.0.1'
         }
 
     def quit(self) -> None:
-        super().quit()
-        self.custom_patcher = None
+        super().quit()
```

### Comparing `selenextra-1.0.4/selenextra.egg-info/PKG-INFO` & `selenextra-1.0.5/selenextra.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: selenextra
-Version: 1.0.4
+Version: 1.0.5
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
```

