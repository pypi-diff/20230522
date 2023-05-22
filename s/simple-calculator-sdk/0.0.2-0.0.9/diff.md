# Comparing `tmp/simple-calculator-sdk-0.0.2.tar.gz` & `tmp/simple-calculator-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-calculator-sdk-0.0.2.tar", last modified: Mon May 22 11:45:34 2023, max compression
+gzip compressed data, was "simple-calculator-sdk-0.0.9.tar", last modified: Mon May 22 12:08:54 2023, max compression
```

## Comparing `simple-calculator-sdk-0.0.2.tar` & `simple-calculator-sdk-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.156797 simple-calculator-sdk-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 11:45:34.157797 simple-calculator-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2931 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.133797 simple-calculator-sdk-0.0.2/apimaticcalculator/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/apimaticcalculator_client.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.136797 simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/simple_calculator_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.137797 simple-calculator-sdk-0.0.2/apimaticcalculator/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.146797 simple-calculator-sdk-0.0.2/apimaticcalculator/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.149797 simple-calculator-sdk-0.0.2/apimaticcalculator/models/
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/models/operation_type_enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.150797 simple-calculator-sdk-0.0.2/apimaticcalculator/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/apimaticcalculator/utilities/file_wrapper.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-22 11:45:06.000000 simple-calculator-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 11:45:34.158797 simple-calculator-sdk-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:34.156797 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 11:45:34.000000 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-22 11:45:34.000000 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:45:34.000000 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 11:45:34.000000 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 11:45:34.000000 simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.559046 simple-calculator-sdk-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 12:08:54.559046 simple-calculator-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.538046 simple-calculator-sdk-0.0.9/apimaticcalculator/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/apimaticcalculator_client.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.542046 simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/simple_calculator_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.544046 simple-calculator-sdk-0.0.9/apimaticcalculator/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.547046 simple-calculator-sdk-0.0.9/apimaticcalculator/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.549046 simple-calculator-sdk-0.0.9/apimaticcalculator/models/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/models/operation_type_enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.550046 simple-calculator-sdk-0.0.9/apimaticcalculator/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/apimaticcalculator/utilities/file_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-22 12:08:22.000000 simple-calculator-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 12:08:54.560046 simple-calculator-sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:08:54.558046 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-22 12:08:54.000000 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-22 12:08:54.000000 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:08:54.000000 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 12:08:54.000000 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 12:08:54.000000 simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/top_level.txt
```

### Comparing `simple-calculator-sdk-0.0.2/LICENSE` & `simple-calculator-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/README.md` & `simple-calculator-sdk-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install simple-calculator-sdk==0.0.2
+pip install simple-calculator-sdk==0.0.9
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/simple-calculator-sdk/0.0.2
+https://pypi.python.org/pypi/simple-calculator-sdk/0.0.9
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.2/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.9/doc/client.md)
 
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
 
-* [Simple Calculator](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.2/doc/controllers/simple-calculator.md)
+* [Simple Calculator](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.9/doc/controllers/simple-calculator.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.2/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.2/doc/http-response.md)
-* [HttpRequest](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.2/doc/http-request.md)
+* [Utility Classes](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/bismapervaiz/simple-calculator-python-sdk/tree/0.0.9/doc/http-request.md)
```

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/api_helper.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/api_helper.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/apimaticcalculator_client.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/apimaticcalculator_client.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/configuration.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/configuration.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/base_controller.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/controllers/simple_calculator_controller.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/controllers/simple_calculator_controller.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/exceptions/api_exception.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_request.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_request.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/http/http_response.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/http/http_response.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/apimaticcalculator/models/operation_type_enum.py` & `simple-calculator-sdk-0.0.9/apimaticcalculator/models/operation_type_enum.py`

 * *Files identical despite different names*

### Comparing `simple-calculator-sdk-0.0.2/pyproject.toml` & `simple-calculator-sdk-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "simple-calculator-sdk"
 description = "Simple Calculations"
-version = "0.0.2"
+version = "0.0.9"
 requires-python = ">=3.7"
 keywords = []
 authors = [{name = "Bisma", email = "bismapervaiz@gmail.com.com"}]
 urls = {Documentation = "https://www.apimatic.io/apidocs/apimatic-calculator"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
```

### Comparing `simple-calculator-sdk-0.0.2/simple_calculator_sdk.egg-info/SOURCES.txt` & `simple-calculator-sdk-0.0.9/simple_calculator_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

