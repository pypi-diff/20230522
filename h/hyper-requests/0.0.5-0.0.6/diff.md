# Comparing `tmp/hyper_requests-0.0.5.tar.gz` & `tmp/hyper_requests-0.0.6.tar.gz`

## Comparing `hyper_requests-0.0.5.tar` & `hyper_requests-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/MANIFEST.in
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/requirements.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/setup.cfg
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.github/workflows/python-package-conda.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/request_builder.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/hyper_requests/threader.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/performance/test_performance.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_check_request_params.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_threader.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/test/unit/test_threader_setup.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/LICENSE
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/README.md
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 hyper_requests-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/MANIFEST.in
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/setup.cfg
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.github/workflows/python-package-conda.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/request_builder.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/hyper_requests/threader.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/performance/test_performance.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_check_request_params.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_threader.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/test/unit/test_threader_setup.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 hyper_requests-0.0.6/PKG-INFO
```

### Comparing `hyper_requests-0.0.5/.pre-commit-config.yaml` & `hyper_requests-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/hyper_requests/request_builder.py` & `hyper_requests-0.0.6/hyper_requests/request_builder.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/hyper_requests/threader.py` & `hyper_requests-0.0.6/hyper_requests/threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/test/performance/test_performance.py` & `hyper_requests-0.0.6/test/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/test/unit/test_check_request_params.py` & `hyper_requests-0.0.6/test/unit/test_check_request_params.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/test/unit/test_threader.py` & `hyper_requests-0.0.6/test/unit/test_threader.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/test/unit/test_threader_setup.py` & `hyper_requests-0.0.6/test/unit/test_threader_setup.py`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/.gitignore` & `hyper_requests-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/LICENSE` & `hyper_requests-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_requests-0.0.5/README.md` & `hyper_requests-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ![coollogo_com-289063340](https://github.com/edjones84/hyper-requests/assets/78102381/8d7fd889-d655-432a-b048-8cbb03fe7cce)<br>
 ---
 *Concurrent request HTTP execution library*
 [![Python Package using Conda](https://github.com/edjones84/hyper-requests/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/edjones84/hyper-requests/actions/workflows/python-package-conda.yml)
 ## What is it?
-hyper-requests is a Python library that enables multithreading of API calls using asyncio. It takes a list of URLs and a list of parameters as input and then uses the requests library to make these calls asynchronously (https://pypi.org/project/requests/).
+hyper-requests is a Python library, enabling multithreading of API calls using asyncio. It takes a list of URLs and a list of parameters as input and then uses the requests library to make these calls asynchronously (https://pypi.org/project/requests/).
 ## Usage
 ### Installation
 Install hyper-requests using pip:
 ```bash
 pip install hyper-requests
 ```
 ### Example
@@ -44,15 +44,15 @@
 
 Finally, process the returned data as desired. In this example, each response is printed, but you can perform further operations based on your specific needs.
 ## Performance
 It is hyper fast!
 
 Within the `test/performance` directory there is a performance test that makes 20 API calls to the random joke generator api: https://official-joke-api.appspot.com/random_joke.
 
-Using hyper requests the time taken to make these calls is ~2 second, using syncronous api calls takes ~16 seconds.
+Using hyper requests the time taken to make these calls is ~2 second, using synchronous api calls takes ~16 seconds.
 
 ```bash
 ============================= test session starts ==============================
 collecting ... collected 1 item
 
 test_performance.py::PerformanceTest::test_api_performance
```

### Comparing `hyper_requests-0.0.5/pyproject.toml` & `hyper_requests-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "hyper-requests"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ed Jones", email="ejones84@icloud.com" },
 ]
 description = "Concurrent request HTTP execution library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hyper_requests-0.0.5/PKG-INFO` & `hyper_requests-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-requests
-Version: 0.0.5
+Version: 0.0.6
 Summary: Concurrent request HTTP execution library
 Project-URL: Homepage, https://github.com/edjones84/hyper-requests
 Project-URL: Bug Tracker, https://github.com/edjones84/hyper-requests/issues
 Author-email: Ed Jones <ejones84@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 
 ![coollogo_com-289063340](https://github.com/edjones84/hyper-requests/assets/78102381/8d7fd889-d655-432a-b048-8cbb03fe7cce)<br>
 ---
 *Concurrent request HTTP execution library*
 [![Python Package using Conda](https://github.com/edjones84/hyper-requests/actions/workflows/python-package-conda.yml/badge.svg)](https://github.com/edjones84/hyper-requests/actions/workflows/python-package-conda.yml)
 ## What is it?
-hyper-requests is a Python library that enables multithreading of API calls using asyncio. It takes a list of URLs and a list of parameters as input and then uses the requests library to make these calls asynchronously (https://pypi.org/project/requests/).
+hyper-requests is a Python library, enabling multithreading of API calls using asyncio. It takes a list of URLs and a list of parameters as input and then uses the requests library to make these calls asynchronously (https://pypi.org/project/requests/).
 ## Usage
 ### Installation
 Install hyper-requests using pip:
 ```bash
 pip install hyper-requests
 ```
 ### Example
@@ -60,15 +60,15 @@
 
 Finally, process the returned data as desired. In this example, each response is printed, but you can perform further operations based on your specific needs.
 ## Performance
 It is hyper fast!
 
 Within the `test/performance` directory there is a performance test that makes 20 API calls to the random joke generator api: https://official-joke-api.appspot.com/random_joke.
 
-Using hyper requests the time taken to make these calls is ~2 second, using syncronous api calls takes ~16 seconds.
+Using hyper requests the time taken to make these calls is ~2 second, using synchronous api calls takes ~16 seconds.
 
 ```bash
 ============================= test session starts ==============================
 collecting ... collected 1 item
 
 test_performance.py::PerformanceTest::test_api_performance
```

