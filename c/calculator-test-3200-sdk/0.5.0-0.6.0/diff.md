# Comparing `tmp/calculator-test-3200-sdk-0.5.0.tar.gz` & `tmp/calculator-test-3200-sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator-test-3200-sdk-0.5.0.tar", last modified: Mon May 22 03:13:35 2023, max compression
+gzip compressed data, was "calculator-test-3200-sdk-0.6.0.tar", last modified: Mon May 22 04:08:07 2023, max compression
```

## Comparing `calculator-test-3200-sdk-0.5.0.tar` & `calculator-test-3200-sdk-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.670244 calculator-test-3200-sdk-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-22 03:13:35.670244 calculator-test-3200-sdk-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2897 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.658244 calculator-test-3200-sdk-0.5.0/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.660243 calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.661244 calculator-test-3200-sdk-0.5.0/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.665243 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.667244 calculator-test-3200-sdk-0.5.0/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.668244 calculator-test-3200-sdk-0.5.0/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/apimaticcalculator/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 03:13:35.670244 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-22 03:13:35.000000 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1062 2023-05-22 03:13:35.000000 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 03:13:35.000000 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 03:13:35.000000 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 03:13:35.000000 calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      532 2023-05-22 03:13:09.000000 calculator-test-3200-sdk-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 03:13:35.671244 calculator-test-3200-sdk-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.355433 calculator-test-3200-sdk-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-22 04:08:07.355433 calculator-test-3200-sdk-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.331433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.333433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.336433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.340433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.342433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.346433 calculator-test-3200-sdk-0.6.0/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/apimaticcalculator/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 04:08:07.355433 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-22 04:08:07.000000 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-05-22 04:08:07.000000 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 04:08:07.000000 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 04:08:07.000000 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 04:08:07.000000 calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-22 04:07:38.000000 calculator-test-3200-sdk-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 04:08:07.358433 calculator-test-3200-sdk-0.6.0/setup.cfg
```

### Comparing `calculator-test-3200-sdk-0.5.0/LICENSE` & `calculator-test-3200-sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/README.md` & `calculator-test-3200-sdk-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install calculator-test-3200-sdk==0.5.0
+pip install calculator-test-3200-sdk==0.6.0
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/calculator-test-3200-sdk/0.5.0
+https://pypi.python.org/pypi/calculator-test-3200-sdk/0.6.0
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.5.0/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.6.0/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -53,15 +53,15 @@
 from apimaticcalculator.configuration import Environment
 
 client = ApimaticcalculatorClient()
 ```
 
 ## List of APIs
 
-* [Simple Calculator](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.5.0/doc/controllers/simple-calculator.md)
+* [Simple Calculator](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.6.0/doc/controllers/simple-calculator.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.5.0/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.5.0/doc/http-response.md)
-* [HttpRequest](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.5.0/doc/http-request.md)
+* [Utility Classes](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.6.0/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.6.0/doc/http-response.md)
+* [HttpRequest](https://www.github.com/thehappybug/calc-test-3200-python/tree/0.6.0/doc/http-request.md)
```

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/api_helper.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/apimaticcalculator_client.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/configuration.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/base_controller.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/controllers/simple_calculator_controller.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/exceptions/api_exception.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_request.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/http/http_response.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/apimaticcalculator/models/operation_type_enum.py` & `calculator-test-3200-sdk-0.6.0/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/calculator_test_3200_sdk.egg-info/SOURCES.txt` & `calculator-test-3200-sdk-0.6.0/calculator_test_3200_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calculator-test-3200-sdk-0.5.0/pyproject.toml` & `calculator-test-3200-sdk-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "calculator-test-3200-sdk"
 description = "Simple calculator API hosted on APIMATIC"
-version = "0.5.0"
+version = "0.6.0"
 requires-python = ">=3.7"
 keywords = []
 authors = []
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
```

