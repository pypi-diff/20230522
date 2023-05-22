# Comparing `tmp/py_volley-1.1.0.tar.gz` & `tmp/py_volley-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_volley-1.1.0.tar", max compression
+gzip compressed data, was "py_volley-1.1.1.tar", max compression
```

## Comparing `py_volley-1.1.0.tar` & `py_volley-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2023-05-18 15:46:30.487841 py_volley-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     8734 2023-05-18 15:46:30.487841 py_volley-1.1.0/README.md
--rw-r--r--   0        0        0     2751 2023-05-18 15:46:30.491842 py_volley-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      132 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/concurrency.py
--rw-r--r--   0        0        0     4897 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/config.py
--rw-r--r--   0        0        0        0 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/base.py
--rw-r--r--   0        0        0    16383 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/confluent.py
--rw-r--r--   0        0        0     7372 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/rsmq.py
--rw-r--r--   0        0        0     3018 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/connectors/zmq.py
--rw-r--r--   0        0        0      393 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/data_models.py
--rw-r--r--   0        0        0    12250 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/engine.py
--rw-r--r--   0        0        0     3150 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/global.yml
--rw-r--r--   0        0        0       53 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/logging.py
--rw-r--r--   0        0        0     1686 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/metrics.py
--rw-r--r--   0        0        0      253 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/__init__.py
--rw-r--r--   0        0        0     4858 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/base.py
--rw-r--r--   0        0        0     2113 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/models/pydantic_model.py
--rw-r--r--   0        0        0     4271 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/profiles.py
--rw-r--r--   0        0        0     4078 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/queues.py
--rw-r--r--   0        0        0      285 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/__init__.py
--rw-r--r--   0        0        0      537 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/base.py
--rw-r--r--   0        0        0      453 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/json_serializer.py
--rw-r--r--   0        0        0      439 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/msgpack_serializer.py
--rw-r--r--   0        0        0      475 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/serializers/orjson_serializer.py
--rw-r--r--   0        0        0     4663 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/transport.py
--rw-r--r--   0        0        0     1742 2023-05-18 15:46:30.503843 py_volley-1.1.0/volley/util.py
--rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 py_volley-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-22 16:30:29.590656 py_volley-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     8734 2023-05-22 16:30:29.590656 py_volley-1.1.1/README.md
+-rw-r--r--   0        0        0     2728 2023-05-22 16:30:29.594656 py_volley-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/concurrency.py
+-rw-r--r--   0        0        0     4897 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/base.py
+-rw-r--r--   0        0        0    16383 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/confluent.py
+-rw-r--r--   0        0        0     7372 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/rsmq.py
+-rw-r--r--   0        0        0     3018 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/connectors/zmq.py
+-rw-r--r--   0        0        0      393 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/data_models.py
+-rw-r--r--   0        0        0    12250 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/engine.py
+-rw-r--r--   0        0        0     3150 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/global.yml
+-rw-r--r--   0        0        0       53 2023-05-22 16:30:29.594656 py_volley-1.1.1/volley/logging.py
+-rw-r--r--   0        0        0     1686 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/metrics.py
+-rw-r--r--   0        0        0      253 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/__init__.py
+-rw-r--r--   0        0        0     4858 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/base.py
+-rw-r--r--   0        0        0     2113 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/models/pydantic_model.py
+-rw-r--r--   0        0        0     4279 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/profiles.py
+-rw-r--r--   0        0        0     4078 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/queues.py
+-rw-r--r--   0        0        0      285 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/__init__.py
+-rw-r--r--   0        0        0      537 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/base.py
+-rw-r--r--   0        0        0      453 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/json_serializer.py
+-rw-r--r--   0        0        0      439 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/msgpack_serializer.py
+-rw-r--r--   0        0        0      475 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/serializers/orjson_serializer.py
+-rw-r--r--   0        0        0     4663 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/transport.py
+-rw-r--r--   0        0        0     1742 2023-05-22 16:30:29.598657 py_volley-1.1.1/volley/util.py
+-rw-r--r--   0        0        0    10074 1970-01-01 00:00:00.000000 py_volley-1.1.1/PKG-INFO
```

### Comparing `py_volley-1.1.0/LICENSE.md` & `py_volley-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/README.md` & `py_volley-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/pyproject.toml` & `py_volley-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 [tool.poetry]
 name = "py_volley"
-version = "1.1.0"
+version = "1.1.1"
 description = "Pluggable message queueing for Python"
 authors = ["ask-machine-learning <shipt@shipt.com>"]
 readme = "README.md"
 
 packages = [
     { include = "volley" },
 ]
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/shipt/py-volley"
 "Repository" = "https://github.com/shipt/py-volley"
 "Documentation" = "https://shipt.github.io/py-volley/"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <4"
-prometheus-client = ">=0.11.0, <1"
-pydantic = ">=1.8.2, <2"
-PyYAML = ">=5.4.1, <6.1"
-orjson = ">=3.6.4, <4.0"
-msgpack = "^1.0.3, <2"
-starlette = "<1"
-uvicorn = "<1"
+python = "^3.8.1"
+prometheus-client = "^0"
+pydantic = "^1.8.2"
+PyYAML = "^6.0.0"
+orjson = "^3.6.4"
+msgpack = "^1.0.3"
+starlette = "^0"
+uvicorn = "^0"
 
 confluent-kafka = {version ="^2.0.0", optional = true}
 PyRSMQ = {version ="^0.4.5", optional = true}
 hiredis = {version ="^2.0", optional = true}
 tenacity = {version ="^8.0.1", optional = true}
 pyzmq = {version =">=22.3.0", optional = true}
 
 [tool.poetry.extras]
 all = ["confluent-kafka", "PyRSMQ", "hiredis", "tenacity", "pyzmq"]
 rsmq = ["PyRSMQ", "hiredis", "tenacity"]
 kafka = ["confluent-kafka"]
 zmq = ["pyzmq"]
 
 [tool.poetry.dev-dependencies]
-flake8 = "^3.9.2"
-mypy = "^0.910"
+flake8 = "^6.0.0"
+mypy = "^1.0.0"
+# TODo(@damon): Remove coverage
 coverage = "^6.0"
 black = "^22.3.0"
 pytest = "^7.2"
 isort = "^5.9.3"
-pydantic = "^1.8.2"
 debugpy = "^1.5.0"
 pytest-cov = "^3.0.0"
 types-requests = "^2.25.11"
 types-pytz = "^2021.3.0"
 mkdocs = "^1.2.3"
 mkdocs-material = "^7.3.6"
 mdx-include = "^1.4.1"
@@ -81,14 +81,15 @@
 [tool.black]
 line-length = 120
 target-version = ['py310', 'py39', 'py38']
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
+
 markers = [
     "integration: mark a test as an integration test"
 ]
 
 [tool.pylint.master]
 ignore="example"
```

### Comparing `py_volley-1.1.0/volley/concurrency.py` & `py_volley-1.1.1/volley/concurrency.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import contextvars
 import functools
-from typing import Any, Awaitable, Callable
+from typing import Any, Callable, Coroutine
 
 from prometheus_client import Counter
 
 from volley.util import FuncEnvelope
 
 APP_STATUS = Counter("volley_app_completions", "Application cycle status", ["app_name", "status"])  # success/failure
 
@@ -49,12 +49,12 @@
     except Exception:
         APP_STATUS.labels(app_name=app_name, status="failure").inc()
         raise
     APP_STATUS.labels(app_name=app_name, status="success").inc()
     return fun_result
 
 
-def run_async(func: Callable[..., Awaitable[Any]]) -> Callable[..., None]:
+def run_async(func: Callable[..., Coroutine[Any, Any, Any]]) -> Callable[..., None]:
     def wrapper() -> None:
         asyncio.run(func())
 
     return wrapper
```

### Comparing `py_volley-1.1.0/volley/config.py` & `py_volley-1.1.1/volley/config.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/connectors/base.py` & `py_volley-1.1.1/volley/connectors/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, Optional
 
 from volley.data_models import QueueMessage
 
 
-@dataclass  # type: ignore
+@dataclass
 class BaseConsumer(ABC):
     """Base class for implementing a consumer"""
 
     queue_name: str
     host: Optional[str] = None
     config: Dict[str, Any] = field(default_factory=dict)
 
@@ -36,15 +36,15 @@
     @abstractmethod
     def shutdown(self) -> None:
         """perform some action when shutting down the application.
         For example, close a connection or leave a consumer group
         """
 
 
-@dataclass  # type: ignore
+@dataclass
 class BaseProducer(ABC):
     """Base class for implementing a producer"""
 
     queue_name: str
     host: Optional[str] = None
     config: Dict[str, Any] = field(default_factory=dict)
```

### Comparing `py_volley-1.1.0/volley/connectors/confluent.py` & `py_volley-1.1.1/volley/connectors/confluent.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/connectors/rsmq.py` & `py_volley-1.1.1/volley/connectors/rsmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/connectors/zmq.py` & `py_volley-1.1.1/volley/connectors/zmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/engine.py` & `py_volley-1.1.1/volley/engine.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/global.yml` & `py_volley-1.1.1/volley/global.yml`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/metrics.py` & `py_volley-1.1.1/volley/metrics.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/models/base.py` & `py_volley-1.1.1/volley/models/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/models/pydantic_model.py` & `py_volley-1.1.1/volley/models/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/profiles.py` & `py_volley-1.1.1/volley/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,10 +97,10 @@
             # and is validated in Profile()
             this_profile = deepcopy(q_cfg)
         else:
             raise ValueError(
                 f"`{profile_requested}` is not a valid profile name. "
                 f"Available profiles: `{list(supported_profiles.keys())}`"
             )
-        constructed_profiles[q_name] = Profile(**this_profile)
+        constructed_profiles[q_name] = Profile.parse_obj(this_profile)
 
     return constructed_profiles
```

### Comparing `py_volley-1.1.0/volley/queues.py` & `py_volley-1.1.1/volley/queues.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/serializers/base.py` & `py_volley-1.1.1/volley/serializers/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/transport.py` & `py_volley-1.1.1/volley/transport.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/volley/util.py` & `py_volley-1.1.1/volley/util.py`

 * *Files identical despite different names*

### Comparing `py_volley-1.1.0/PKG-INFO` & `py_volley-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: py-volley
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pluggable message queueing for Python
 Author: ask-machine-learning
 Author-email: shipt@shipt.com
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: kafka
 Provides-Extra: rsmq
 Provides-Extra: zmq
 Requires-Dist: PyRSMQ (>=0.4.5,<0.5.0) ; extra == "all" or extra == "rsmq"
-Requires-Dist: PyYAML (>=5.4.1,<6.1)
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: confluent-kafka (>=2.0.0,<3.0.0) ; extra == "all" or extra == "kafka"
 Requires-Dist: hiredis (>=2.0,<3.0) ; extra == "all" or extra == "rsmq"
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
-Requires-Dist: orjson (>=3.6.4,<4.0)
-Requires-Dist: prometheus-client (>=0.11.0,<1)
-Requires-Dist: pydantic (>=1.8.2,<2)
+Requires-Dist: orjson (>=3.6.4,<4.0.0)
+Requires-Dist: prometheus-client (>=0,<1)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyzmq (>=22.3.0) ; extra == "all" or extra == "zmq"
-Requires-Dist: starlette (<1)
+Requires-Dist: starlette (>=0,<1)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0) ; extra == "all" or extra == "rsmq"
-Requires-Dist: uvicorn (<1)
+Requires-Dist: uvicorn (>=0,<1)
 Project-URL: Documentation, https://shipt.github.io/py-volley/
 Project-URL: Homepage, https://github.com/shipt/py-volley
 Project-URL: Repository, https://github.com/shipt/py-volley
 Description-Content-Type: text/markdown
 
 ![VolleyFull-Horizontal](https://user-images.githubusercontent.com/81711984/149005139-f0441dcf-c76e-4112-baf1-998d0a6abdbb.png)
```

