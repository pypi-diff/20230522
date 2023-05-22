# Comparing `tmp/hyper_requests-0.0.6.tar.gz` & `tmp/hyper_requests-0.0.7.tar.gz`

## Comparing `hyper_requests-0.0.6.tar` & `hyper_requests-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/MANIFEST.in
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/setup.cfg
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/request_builder.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/threader.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/performance/test_performance.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_check_request_params.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_threader.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_threader_setup.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/LICENSE
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/setup.cfg
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/request_builder.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/hyper_requests/threader.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/performance/test_performance.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_check_request_params.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_threader.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/test/unit/test_threader_setup.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 hyper_requests-0.0.7/PKG-INFO
```

### Comparing `hyper_requests-0.0.6/.pre-commit-config.yaml` & `hyper_requests-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/.github/workflows/python-package-conda.yml` & `hyper_requests-0.0.7/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/hyper_requests/request_builder.py` & `hyper_requests-0.0.7/hyper_requests/request_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 from requests.models import Request
 
 
 def check_request_params(
     request_parameters: list[dict[str, str]]
 ) -> list[dict[str, str]]:
+    """
+    Checks the validity of request parameters and ensures they match the attributes of the Request class.
+
+    :param request_parameters: List of dictionaries containing request parameters.
+    :return: Validated list of request parameters.
+    :raises ValueError: If the request parameters are invalid.
+    """
 
     # Get the attribute names of the Request class
     request_attributes = inspect.getfullargspec(Request.__init__).args
 
     # Iterate over each dictionary in the request_parameters list
     for request_dict in request_parameters:
         # Get the keys of the dictionary
@@ -17,13 +24,13 @@
 
         # Check if any key in the dictionary is also a valid attribute name of the Request class
         if not any(key in request_attributes for key in request_keys):
             raise ValueError(
                 "Invalid request parameters. No matching keys found in Request class attributes."
             )
 
-        # Check a url request string is present  in the dictionary
+        # Check if a URL request string is present in the dictionary
         if "url" not in request_keys:
             raise ValueError("Invalid request parameters. No url key present")
 
     # If all dictionaries have at least one matching key, return the request_parameters list
     return request_parameters
```

### Comparing `hyper_requests-0.0.6/test/performance/test_performance.py` & `hyper_requests-0.0.7/test/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/test/unit/test_check_request_params.py` & `hyper_requests-0.0.7/test/unit/test_check_request_params.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/test/unit/test_threader.py` & `hyper_requests-0.0.7/test/unit/test_threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/test/unit/test_threader_setup.py` & `hyper_requests-0.0.7/test/unit/test_threader_setup.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/.gitignore` & `hyper_requests-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/LICENSE` & `hyper_requests-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.6/README.md` & `hyper_requests-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 ### Installation
 Install hyper-requests using pip:
 ```bash
 pip install hyper-requests
 ```
 ### Example
 ```python
-from hyper_requests.threader import AsyncRequests
+import hyper_requests
 
 # Define the request parameters
 params = [
     {'url': 'http://httpbin.org/get' , 'data': 'value1'},
     {'url': 'http://httpbin.org/get' , 'data': 'value3'},
     {'url': 'http://httpbin.org/get' , 'data': 'value5'},
     {'url': 'http://httpbin.org/get' , 'data': 'value7'},
     {'url': 'http://httpbin.org/get' , 'data': 'value9'}
 ]
 
 # Create an instance of AsyncRequests and execute the requests
-returned_data = AsyncRequests(request_params=params, workers=10).run_threads()
+returned_data = hyper_requests.get(request_params=params, workers=10)
 
 # Process the returned data
 for response in returned_data:
     print(response)
 ```
 This example demonstrates the usage of hyper-requests to perform asynchronous HTTP requests.
```

### Comparing `hyper_requests-0.0.6/PKG-INFO` & `hyper_requests-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-requests
-Version: 0.0.6
+Version: 0.0.7
 Summary: Concurrent request HTTP execution library
 Project-URL: Homepage, https://github.com/edjones84/hyper-requests
 Project-URL: Bug Tracker, https://github.com/edjones84/hyper-requests/issues
 Author-email: Ed Jones <ejones84@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,27 +24,27 @@
 ### Installation
 Install hyper-requests using pip:
 ```bash
 pip install hyper-requests
 ```
 ### Example
 ```python
-from hyper_requests.threader import AsyncRequests
+import hyper_requests
 
 # Define the request parameters
 params = [
     {'url': 'http://httpbin.org/get' , 'data': 'value1'},
     {'url': 'http://httpbin.org/get' , 'data': 'value3'},
     {'url': 'http://httpbin.org/get' , 'data': 'value5'},
     {'url': 'http://httpbin.org/get' , 'data': 'value7'},
     {'url': 'http://httpbin.org/get' , 'data': 'value9'}
 ]
 
 # Create an instance of AsyncRequests and execute the requests
-returned_data = AsyncRequests(request_params=params, workers=10).run_threads()
+returned_data = hyper_requests.get(request_params=params, workers=10)
 
 # Process the returned data
 for response in returned_data:
     print(response)
 ```
 This example demonstrates the usage of hyper-requests to perform asynchronous HTTP requests.
```

