# Comparing `tmp/scienceio-2.0.2.tar.gz` & `tmp/scienceio-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scienceio-2.0.2.tar", last modified: Fri Feb 24 20:12:09 2023, max compression
+gzip compressed data, was "scienceio-2.1.0.tar", last modified: Mon May 22 20:14:26 2023, max compression
```

## Comparing `scienceio-2.0.2.tar` & `scienceio-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      148 2023-02-24 20:11:54.865112 scienceio-2.0.2/.flake8
--rw-r--r--   0        0        0        2 2023-02-24 20:11:54.865112 scienceio-2.0.2/.fourmat
--rw-r--r--   0        0        0      107 2023-02-24 20:11:54.869112 scienceio-2.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      226 2023-02-24 20:11:54.869112 scienceio-2.0.2/.github/pull_request_template.md
--rw-r--r--   0        0        0     1773 2023-02-24 20:11:54.869112 scienceio-2.0.2/.github/workflows/deploy_staging.yml
--rw-r--r--   0        0        0     1485 2023-02-24 20:11:54.869112 scienceio-2.0.2/.github/workflows/pull_request.yml
--rw-r--r--   0        0        0     1728 2023-02-24 20:11:54.869112 scienceio-2.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2371 2023-02-24 20:11:54.869112 scienceio-2.0.2/.gitignore
--rw-r--r--   0        0        0      234 2023-02-24 20:11:54.869112 scienceio-2.0.2/CODEOWNERS
--rw-r--r--   0        0        0     2588 2023-02-24 20:11:54.869112 scienceio-2.0.2/PUBLISHING.md
--rw-r--r--   0        0        0      336 2023-02-24 20:11:54.869112 scienceio-2.0.2/Pipfile
--rw-r--r--   0        0        0    36713 2023-02-24 20:11:54.869112 scienceio-2.0.2/Pipfile.lock
--rw-r--r--   0        0        0     1366 2023-02-24 20:11:54.869112 scienceio-2.0.2/README.md
--rw-r--r--   0        0        0     3083 2023-02-24 20:11:54.869112 scienceio-2.0.2/examples/analytics.py
--rw-r--r--   0        0        0     2591 2023-02-24 20:11:54.869112 scienceio-2.0.2/examples/convert_data_model.py
--rw-r--r--   0        0        0    10051 2023-02-24 20:11:54.869112 scienceio-2.0.2/examples/example-analytics-1.ipynb
--rw-r--r--   0        0        0    46436 2023-02-24 20:11:54.873112 scienceio-2.0.2/examples/example-analytics-2.ipynb
--rw-r--r--   0        0        0    12058 2023-02-24 20:11:54.873112 scienceio-2.0.2/examples/example-annotate-onboarding-text.ipynb
--rw-r--r--   0        0        0     9677 2023-02-24 20:11:54.873112 scienceio-2.0.2/examples/example-onboarding.ipynb
--rw-r--r--   0        0        0      877 2023-02-24 20:11:54.877112 scienceio-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      165 2023-02-24 20:11:54.877112 scienceio-2.0.2/src/scienceio/__init__.py
--rw-r--r--   0        0        0     9636 2023-02-24 20:11:54.877112 scienceio-2.0.2/src/scienceio/scienceio.py
--rwxr-xr-x   0        0        0       47 2023-02-24 20:11:54.877112 scienceio-2.0.2/test.sh
--rw-r--r--   0        0        0        0 2023-02-24 20:11:54.877112 scienceio-2.0.2/tests/__init__.py
--rw-r--r--   0        0        0    13798 2023-02-24 20:11:54.877112 scienceio-2.0.2/tests/__snapshots__/test_scienceio.ambr
--rw-r--r--   0        0        0     4839 2023-02-24 20:11:54.877112 scienceio-2.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2634 2023-02-24 20:11:54.877112 scienceio-2.0.2/tests/test_scienceio.py
--rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-05-22 20:14:09.208550 scienceio-2.1.0/.flake8
+-rw-r--r--   0        0        0        2 2023-05-22 20:14:09.208550 scienceio-2.1.0/.fourmat
+-rw-r--r--   0        0        0      107 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      226 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1773 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/deploy_staging.yml
+-rw-r--r--   0        0        0     1485 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/pull_request.yml
+-rw-r--r--   0        0        0     1728 2023-05-22 20:14:09.208550 scienceio-2.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2371 2023-05-22 20:14:09.208550 scienceio-2.1.0/.gitignore
+-rw-r--r--   0        0        0      234 2023-05-22 20:14:09.208550 scienceio-2.1.0/CODEOWNERS
+-rw-r--r--   0        0        0     2588 2023-05-22 20:14:09.212550 scienceio-2.1.0/PUBLISHING.md
+-rw-r--r--   0        0        0      336 2023-05-22 20:14:09.212550 scienceio-2.1.0/Pipfile
+-rw-r--r--   0        0        0    36713 2023-05-22 20:14:09.212550 scienceio-2.1.0/Pipfile.lock
+-rw-r--r--   0        0        0     1366 2023-05-22 20:14:09.212550 scienceio-2.1.0/README.md
+-rw-r--r--   0        0        0     3083 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/analytics.py
+-rw-r--r--   0        0        0     2591 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/convert_data_model.py
+-rw-r--r--   0        0        0    10051 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-analytics-1.ipynb
+-rw-r--r--   0        0        0    46436 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-analytics-2.ipynb
+-rw-r--r--   0        0        0    12058 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-annotate-onboarding-text.ipynb
+-rw-r--r--   0        0        0     9677 2023-05-22 20:14:09.212550 scienceio-2.1.0/examples/example-onboarding.ipynb
+-rw-r--r--   0        0        0      877 2023-05-22 20:14:09.212550 scienceio-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-05-22 20:14:09.212550 scienceio-2.1.0/src/scienceio/__init__.py
+-rw-r--r--   0        0        0    10571 2023-05-22 20:14:09.212550 scienceio-2.1.0/src/scienceio/scienceio.py
+-rwxr-xr-x   0        0        0       47 2023-05-22 20:14:09.212550 scienceio-2.1.0/test.sh
+-rw-r--r--   0        0        0        0 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    13798 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/__snapshots__/test_scienceio.ambr
+-rw-r--r--   0        0        0     4839 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2634 2023-05-22 20:14:09.212550 scienceio-2.1.0/tests/test_scienceio.py
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 scienceio-2.1.0/PKG-INFO
```

### Comparing `scienceio-2.0.2/.github/workflows/deploy_staging.yml` & `scienceio-2.1.0/.github/workflows/deploy_staging.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/.github/workflows/pull_request.yml` & `scienceio-2.1.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/.github/workflows/release.yml` & `scienceio-2.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/.gitignore` & `scienceio-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/PUBLISHING.md` & `scienceio-2.1.0/PUBLISHING.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/Pipfile.lock` & `scienceio-2.1.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/README.md` & `scienceio-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/analytics.py` & `scienceio-2.1.0/examples/analytics.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/convert_data_model.py` & `scienceio-2.1.0/examples/convert_data_model.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/example-analytics-1.ipynb` & `scienceio-2.1.0/examples/example-analytics-1.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/example-analytics-2.ipynb` & `scienceio-2.1.0/examples/example-analytics-2.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/example-annotate-onboarding-text.ipynb` & `scienceio-2.1.0/examples/example-annotate-onboarding-text.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/examples/example-onboarding.ipynb` & `scienceio-2.1.0/examples/example-onboarding.ipynb`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/pyproject.toml` & `scienceio-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/src/scienceio/scienceio.py` & `scienceio-2.1.0/src/scienceio/scienceio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import configparser
 import enum
 import json
 import os
 import requests
 import time
 
+from http import HTTPStatus
 from pathlib import Path
 from typing import Optional
 
 API_URL: str = "https://api.aws.science.io/v2"
 HELP_EMAIL: str = "api_support@science.io"
 SETTINGS_DIR: Path = Path.home() / ".scienceio"
 BASE_DELAY_SEC: float = 1
 BACKOFF_FACTOR: float = 2
 MAX_RETRY_ATTEMPTS: int = 8
 DEFAULT_ERROR_MESSAGE = f"An error occured, please email {HELP_EMAIL} for assistance."
+RETRY_AFTER_HEADER = "retry-after"
 
 
 class Model(str, enum.Enum):
     STRUCTURE = "structure"
     IDENTIFY_PHI = "identify-phi"
     REDACT_PHI = "redact-phi"
 
@@ -33,38 +35,40 @@
 class ScienceIOError(Exception):
     """Base class for all exceptions that are raised by the ScienceIO SDK."""
 
 
 class HTTPError(ScienceIOError):
     """Raised when an HTTP error occurs when using the ScienceIO SDK."""
 
-    def __init__(self, status_code: int, message: str):
+    def __init__(self, status_code: int, message: str, headers: dict):
         super().__init__(message)
         self.status_code = status_code
+        self.headers = headers
 
 
 class TimeoutError(ScienceIOError):
     """Raised when a call to the ScienceIO API times out."""
 
     def __init__(self, msg):
         self.msg = msg
 
 
 class ScienceIO(object):
-    def __init__(self):
+    def __init__(self, enable_rate_limit_retry: bool = True):
         """Initializer for the ScienceIO client. The client will attempt to
         configure itself by trying to read from environment variables, if set.
         If unable to, the config values will be read from the ScienceIO config
         file.
         """
 
         # Create a persistent session across requests.
         # https://docs.python-requests.org/en/master/user/advanced/
         self.session = requests.Session()
         self.session.params = {}
+        self._enable_rate_limit_retry = enable_rate_limit_retry
 
         # Lazy loading of configuration (no need to try and load the settings if user specifies
         # their own API ID and secret). Also, this prevents breakage when in envs with no
         # settings file, such as test environments or hosted Jupyter notebooks.
         config = None
 
         def get_config_value(key: str) -> str:
@@ -162,45 +166,63 @@
 
         response = self.session.post(
             submit_url,
             json={key_name: text},
             headers=self.headers,
         )
 
+        if (
+            self._enable_rate_limit_retry
+            and response.status_code == HTTPStatus.TOO_MANY_REQUESTS
+        ):
+            retry_after = int(response.headers.get(RETRY_AFTER_HEADER, 0))
+            time.sleep(retry_after)
+            return self._submit_request(text, model)
+
         payload = _response_handler(response)
 
         request_id = payload["request_id"]
 
         return request_id
 
     def _poll_response(self, request_id: str, model: Model) -> Optional[dict]:
         poll_url = self._construct_poll_url(request_id=request_id, model=model)
 
         response = self.session.get(
             poll_url,
             headers=self.headers,
         )
 
+        if (
+            self._enable_rate_limit_retry
+            and response.status_code == HTTPStatus.TOO_MANY_REQUESTS
+        ):
+            retry_after = int(response.headers.get(RETRY_AFTER_HEADER, 0))
+            time.sleep(retry_after)
+            return self._poll_response(request_id, model)
+
         payload = _response_handler(response)
 
         return _poll_payload_handler(payload)
 
 
 def _response_handler(response: requests.Response) -> dict:
     status_code = response.status_code
     payload = response.json()
 
     if 400 <= status_code <= 599:
         error_payload = payload.get("detail", DEFAULT_ERROR_MESSAGE)
 
+        if status_code == HTTPStatus.TOO_MANY_REQUESTS:
+            error_payload = payload.get("error")
+
         error_json_str = json.dumps(error_payload)
 
         raise HTTPError(
-            status_code=status_code,
-            message=error_json_str,
+            status_code=status_code, message=error_json_str, headers=response.headers
         )
 
     return payload
 
 
 def _poll_payload_handler(payload: dict) -> Optional[dict]:
     status = payload["inference_status"]
```

### Comparing `scienceio-2.0.2/tests/__snapshots__/test_scienceio.ambr` & `scienceio-2.1.0/tests/__snapshots__/test_scienceio.ambr`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/tests/conftest.py` & `scienceio-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/tests/test_scienceio.py` & `scienceio-2.1.0/tests/test_scienceio.py`

 * *Files identical despite different names*

### Comparing `scienceio-2.0.2/PKG-INFO` & `scienceio-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scienceio
-Version: 2.0.2
+Version: 2.1.0
 Summary: ScienceIO Python SDK
 Author-email: ScienceIO <info@science.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Dist: requests >=2.26
```

