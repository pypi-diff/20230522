# Comparing `tmp/asad-14-json-generator-0.1.2.tar.gz` & `tmp/asad-14-json-generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asad-14-json-generator-0.1.2.tar", last modified: Mon May 22 12:03:35 2023, max compression
+gzip compressed data, was "asad-14-json-generator-0.2.0.tar", last modified: Mon May 22 12:07:13 2023, max compression
```

## Comparing `asad-14-json-generator-0.1.2.tar` & `asad-14-json-generator-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.403913 asad-14-json-generator-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-22 12:03:35.403913 asad-14-json-generator-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3182 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.371913 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-22 12:03:35.000000 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1157 2023-05-22 12:03:35.000000 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:03:35.000000 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 12:03:35.000000 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-22 12:03:35.000000 asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.378913 asad-14-json-generator-0.1.2/jsonvaluetester/
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/__init__.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.381913 asad-14-json-generator-0.1.2/jsonvaluetester/controllers/
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12985 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/controllers/json_obj_controller.py
--rw-r--r--   0 root         (0) root         (0)    12952 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/controllers/json_val_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.383913 asad-14-json-generator-0.1.2/jsonvaluetester/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.393913 asad-14-json-generator-0.1.2/jsonvaluetester/http/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1879 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/http/http_response.py
--rw-r--r--   0 root         (0) root         (0)     2293 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/jsonvaluetester_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.401913 asad-14-json-generator-0.1.2/jsonvaluetester/models/
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/models/content_type.py
--rw-r--r--   0 root         (0) root         (0)     3135 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/models/schema_container.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/models/server_response.py
--rw-r--r--   0 root         (0) root         (0)     3102 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/models/value_container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:03:35.402912 asad-14-json-generator-0.1.2/jsonvaluetester/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/jsonvaluetester/utilities/file_wrapper.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-22 12:03:01.000000 asad-14-json-generator-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 12:03:35.404913 asad-14-json-generator-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.683333 asad-14-json-generator-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-22 12:07:13.683333 asad-14-json-generator-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.664333 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-22 12:07:13.000000 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-22 12:07:13.000000 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:07:13.000000 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-22 12:07:13.000000 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-22 12:07:13.000000 asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.667333 asad-14-json-generator-0.2.0/jsonvaluetester/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.671333 asad-14-json-generator-0.2.0/jsonvaluetester/controllers/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12985 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/controllers/json_obj_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12952 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/controllers/json_val_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.673333 asad-14-json-generator-0.2.0/jsonvaluetester/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.677333 asad-14-json-generator-0.2.0/jsonvaluetester/http/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/http/http_response.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/jsonvaluetester_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.681333 asad-14-json-generator-0.2.0/jsonvaluetester/models/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/models/content_type.py
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/models/schema_container.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/models/server_response.py
+-rw-r--r--   0 root         (0) root         (0)     3102 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/models/value_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:13.683333 asad-14-json-generator-0.2.0/jsonvaluetester/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/jsonvaluetester/utilities/file_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-22 12:06:47.000000 asad-14-json-generator-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-22 12:07:13.684333 asad-14-json-generator-0.2.0/setup.cfg
```

### Comparing `asad-14-json-generator-0.1.2/LICENSE` & `asad-14-json-generator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/README.md` & `asad-14-json-generator-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install asad-14-json-generator==0.1.2
+pip install asad-14-json-generator==0.2.0
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/asad-14-json-generator/0.1.2
+https://pypi.python.org/pypi/asad-14-json-generator/0.2.0
 
 ## Test the SDK
 
 You can test the generated SDK and the server with test cases. `unittest` is used as the testing framework and `pytest` is used as the test runner. You can run the tests as follows:
 
 Navigate to the root directory of the SDK and run the following commands
 
 ```
 pip install -r test-requirements.txt
 pytest
 ```
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.TESTING`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -64,16 +64,16 @@
 | Name | Description |
 |  --- | --- |
 | production | - |
 | testing | **Default** |
 
 ## List of APIs
 
-* [Json Obj](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/controllers/json-obj.md)
-* [Json Val](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/controllers/json-val.md)
+* [Json Obj](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/controllers/json-obj.md)
+* [Json Val](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/controllers/json-val.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/http-response.md)
-* [HttpRequest](https://www.github.com/asadali-14/python-json-generator/tree/0.1.2/doc/http-request.md)
+* [Utility Classes](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/http-response.md)
+* [HttpRequest](https://www.github.com/asadali-14/python-json-generator/tree/0.2.0/doc/http-request.md)
```

### Comparing `asad-14-json-generator-0.1.2/asad_14_json_generator.egg-info/SOURCES.txt` & `asad-14-json-generator-0.2.0/asad_14_json_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/api_helper.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/api_helper.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/configuration.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/configuration.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/controllers/base_controller.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/controllers/json_obj_controller.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/controllers/json_obj_controller.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/controllers/json_val_controller.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/controllers/json_val_controller.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/exceptions/api_exception.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/http/http_request.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/http/http_request.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/http/http_response.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/http/http_response.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/jsonvaluetester_client.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/jsonvaluetester_client.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/models/schema_container.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/models/schema_container.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/models/server_response.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/models/server_response.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/jsonvaluetester/models/value_container.py` & `asad-14-json-generator-0.2.0/jsonvaluetester/models/value_container.py`

 * *Files identical despite different names*

### Comparing `asad-14-json-generator-0.1.2/pyproject.toml` & `asad-14-json-generator-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "asad-14-json-generator"
 description = "Testing Special JsonValue feature"
-version = "0.1.2"
+version = "0.2.0"
 requires-python = ">=3.7"
 keywords = ["Json"]
 authors = []
 urls = {}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
 [project.optional-dependencies]
```

