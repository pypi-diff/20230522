# Comparing `tmp/token_throttler-1.2.1.tar.gz` & `tmp/token_throttler-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_throttler-1.2.1.tar", max compression
+gzip compressed data, was "token_throttler-1.3.0.tar", max compression
```

## Comparing `token_throttler-1.2.1.tar` & `token_throttler-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1058 2022-03-30 22:46:19.422357 token_throttler-1.2.1/LICENSE
--rw-r--r--   0        0        0     4799 2022-10-28 20:06:32.855333 token_throttler-1.2.1/README.md
--rw-r--r--   0        0        0     2296 2022-10-28 20:06:32.855333 token_throttler-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      230 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/__init__.py
--rw-r--r--   0        0        0      238 2022-03-31 21:15:42.896315 token_throttler-1.2.1/src/token_throttler/exception.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 token_throttler-1.2.1/src/token_throttler/py.typed
--rw-r--r--   0        0        0      138 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/__init__.py
--rw-r--r--   0        0        0     1099 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/bucket_storage.py
--rw-r--r--   0        0        0     1160 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/bucket_storage_async.py
--rw-r--r--   0        0        0     1728 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/memory_storage.py
--rw-r--r--   0        0        0       91 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/redis/__init__.py
--rw-r--r--   0        0        0     3806 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/storage/redis/redis_storage.py
--rw-r--r--   0        0        0     4001 2022-10-28 20:06:32.855333 token_throttler-1.2.1/src/token_throttler/storage/redis/redis_storage_async.py
--rw-r--r--   0        0        0      794 2022-04-18 20:45:02.610504 token_throttler-1.2.1/src/token_throttler/throttler_config.py
--rw-r--r--   0        0        0      753 2022-04-13 19:09:46.862268 token_throttler-1.2.1/src/token_throttler/token_bucket.py
--rw-r--r--   0        0        0     3919 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/token_throttler.py
--rw-r--r--   0        0        0     3709 2022-10-18 11:35:18.519274 token_throttler-1.2.1/src/token_throttler/token_throttler_async.py
--rw-r--r--   0        0        0     1945 2022-10-01 22:11:29.780129 token_throttler-1.2.1/src/token_throttler/validate.py
--rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 token_throttler-1.2.1/setup.py
--rw-r--r--   0        0        0     6587 1970-01-01 00:00:00.000000 token_throttler-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-30 22:46:19.422357 token_throttler-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6505 2023-05-22 00:08:07.486464 token_throttler-1.3.0/README.md
+-rw-r--r--   0        0        0     2614 2023-05-22 00:08:07.489798 token_throttler-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      230 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/__init__.py
+-rw-r--r--   0        0        0      238 2022-03-31 21:15:42.896315 token_throttler-1.3.0/src/token_throttler/exception.py
+-rw-r--r--   0        0        0        0 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/ext/__init__.py
+-rw-r--r--   0        0        0      814 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2022-04-01 23:18:33.555504 token_throttler-1.3.0/src/token_throttler/py.typed
+-rw-r--r--   0        0        0      139 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/storage/__init__.py
+-rw-r--r--   0        0        0     1099 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/bucket_storage.py
+-rw-r--r--   0        0        0     1160 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/bucket_storage_async.py
+-rw-r--r--   0        0        0       91 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/redis/__init__.py
+-rw-r--r--   0        0        0     3806 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage.py
+-rw-r--r--   0        0        0     4001 2022-10-28 20:06:32.855333 token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage_async.py
+-rw-r--r--   0        0        0     1728 2023-05-22 00:08:07.489798 token_throttler-1.3.0/src/token_throttler/storage/runtime_storage.py
+-rw-r--r--   0        0        0      794 2022-04-18 20:45:02.610504 token_throttler-1.3.0/src/token_throttler/throttler_config.py
+-rw-r--r--   0        0        0      753 2022-04-13 19:09:46.862268 token_throttler-1.3.0/src/token_throttler/token_bucket.py
+-rw-r--r--   0        0        0     3919 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/token_throttler.py
+-rw-r--r--   0        0        0     3709 2022-10-18 11:35:18.519274 token_throttler-1.3.0/src/token_throttler/token_throttler_async.py
+-rw-r--r--   0        0        0     1945 2022-10-01 22:11:29.780129 token_throttler-1.3.0/src/token_throttler/validate.py
+-rw-r--r--   0        0        0     8377 1970-01-01 00:00:00.000000 token_throttler-1.3.0/PKG-INFO
```

### Comparing `token_throttler-1.2.1/LICENSE` & `token_throttler-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/pyproject.toml` & `token_throttler-1.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "token-throttler"
-version = "1.2.1"
+version = "1.3.0"
 description = "Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm"
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = [
         "Vojko Pribudić <dmanthing@gmail.com>",
         "Rino Dugonjić <dugonjic.rino@gmail.com>",
 ]
 repository = "https://gitlab.com/vojko.pribudic/token-throttler"
@@ -35,38 +35,51 @@
 
 [tool.poetry.urls]
 "Tracker" = "https://gitlab.com/vojko.pribudic/token-throttler/-/issues"
 "Changelog" = "https://gitlab.com/vojko.pribudic/token-throttler/-/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
-redis = { version = "^4.3.4", optional = true }
+redis = { version = "^4.4", optional = true }
+fastapi = { version = "^0.95.2", optional = true }
 
 [tool.poetry.extras]
 redis = ["redis"]
+fastapi = ["fastapi"]
 
 [tool.poetry.group.test.dependencies]
-fakeredis = "1.9.3"
-freezegun = "1.2.2"
-pytest-asyncio = "0.18.3"
-pytest-cov = "3.0.0"
-tox = "3.25.0"
+fakeredis = "^2.2"
+fastapi = "^0.95.2"
+freezegun = "^1.2"
+pytest = "^7.2"
+pytest-asyncio = "^0.20"
+pytest-cov = "^4.0"
+tox = "^4.4"
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["src"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+exclude_lines=[
+    "def __repr__",
+    "if 0:",
+    "if __name__ == .__main__.:",
+    "pass",
+    "pragma: no cover"
+  ]
+sort = "cover"
+precision = 3
 
 [tool.pytest.ini_options]
+addopts = "--cov-fail-under=100 --strict-markers"
 asyncio_mode = "auto"
 filterwarnings = "ignore::DeprecationWarning"
 
 [tool.isort]
 profile = "black"
 
 [tool.tox]
@@ -75,16 +88,19 @@
 isolated_build = True
 envlist = py37, py38, py39, py310, py311
 
 [testenv]
 commands =
   pytest --cov
 deps =
+  fastapi
   fakeredis
   freezegun
+  httpx
   pytest-asyncio
   pytest-cov
+  redis==4.5.4
 """
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `token_throttler-1.2.1/src/token_throttler/storage/bucket_storage.py` & `token_throttler-1.3.0/src/token_throttler/storage/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/storage/bucket_storage_async.py` & `token_throttler-1.3.0/src/token_throttler/storage/bucket_storage_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/storage/memory_storage.py` & `token_throttler-1.3.0/src/token_throttler/storage/runtime_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/storage/redis/redis_storage.py` & `token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/storage/redis/redis_storage_async.py` & `token_throttler-1.3.0/src/token_throttler/storage/redis/redis_storage_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/throttler_config.py` & `token_throttler-1.3.0/src/token_throttler/throttler_config.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/token_bucket.py` & `token_throttler-1.3.0/src/token_throttler/token_bucket.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/token_throttler.py` & `token_throttler-1.3.0/src/token_throttler/token_throttler.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/token_throttler_async.py` & `token_throttler-1.3.0/src/token_throttler/token_throttler_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/src/token_throttler/validate.py` & `token_throttler-1.3.0/src/token_throttler/validate.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.2.1/setup.py` & `token_throttler-1.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Token throttler
 
-package_dir = \
-{'': 'src'}
+![Coverage](https://img.shields.io/gitlab/coverage/vojko.pribudic/token-throttler/main?job_name=tests)
+![Version](https://img.shields.io/pypi/pyversions/token-throttler)
+![Downloads](https://pepy.tech/badge/token-throttler)
+![Formatter](https://img.shields.io/badge/code%20style-black-black)
+![License](https://img.shields.io/pypi/l/token-throttler)
 
-packages = \
-['token_throttler', 'token_throttler.storage', 'token_throttler.storage.redis']
+**Token throttler** is an extendable rate-limiting library somewhat based on a [token bucket algorithm](https://en.wikipedia.org/wiki/Token_bucket).
 
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'redis': ['redis>=4.3.4,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'token-throttler',
-    'version': '1.2.1',
-    'description': 'Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm',
-    'long_description': '# Token throttler\n\n![Coverage](https://img.shields.io/gitlab/coverage/vojko.pribudic/token-throttler/main?job_name=tests)\n![Version](https://img.shields.io/pypi/pyversions/token-throttler)\n![Downloads](https://pepy.tech/badge/token-throttler)\n![Formatter](https://img.shields.io/badge/code%20style-black-black)\n![License](https://img.shields.io/pypi/l/token-throttler)\n\n**Token throttler** is an extendable rate-limiting library somewhat based on a [token bucket algorithm](https://en.wikipedia.org/wiki/Token_bucket).\n\n## Table of contents\n\n1. [ Installation ](#installation)\n2. [ Features ](#features)\n3. [ Usage ](#usage)\n    1. [ Manual usage example ](#usage-manual)\n    2. [ Decorator usage example ](#usage-decorator)\n4. [ Storage ](#storage)\n5. [ Configuration ](#configuration)\n   1. [ Configuration usage ](#configuration-usage)\n\n<a name="installation"></a>\n## 1. Installation\n\nToken throttler is available on PyPI:\n```console \n$ python -m pip install token-throttler\n```\nToken throttler officially supports Python >= 3.7.\n\n*NOTE*: Depending on the storage engine you pick, you can install token throttler with extras:\n```console \n$ python -m pip install token-throttler[redis]\n```\n\n<a name="features"></a>\n## 2. Features\n\n- Blocking (TokenThrottler) and non-blocking (TokenThrottlerAsync)\n- Global throttler(s) configuration\n- Configurable token throttler cost and identifier\n- Multiple buckets per throttler per identifier\n- Buckets can be added/removed manually or by a `dict` configuration\n- Manual usage or usage via decorator\n- Decorator usage supports async code too\n- Custom decorator can be written\n- Extendable storage engine (eg. Redis)\n\n<a name="usage"></a>\n## 3. Usage\n\nToken throttler supports both manual usage and via decorator.\n\nDecorator usage supports both async and sync.\n\n<a name="usage-manual"></a>\n### 1) Manual usage example:\n\n```python\nfrom token_throttler import TokenBucket, TokenThrottler\nfrom token_throttler.storage import RuntimeStorage\n\nthrottler: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())\nthrottler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=10, max_tokens=10))\nthrottler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=30, max_tokens=20))\n\n\ndef hello_world() -> None:\n    print("Hello World")\n\n\nfor i in range(10):\n    throttler.consume(identifier="hello_world")\n    hello_world()\n\nif throttler.consume(identifier="hello_world"):\n    hello_world()\nelse:\n    print("bucket_one ran out of tokens")\n```\n\n<a name="usage-decorator"></a>\n### 2) Decorator usage example:\n\n```python\nfrom token_throttler import TokenBucket, TokenThrottler, TokenThrottlerException\nfrom token_throttler.storage import RuntimeStorage\n\nthrottler: TokenThrottler = TokenThrottler(1, RuntimeStorage())\nthrottler.add_bucket("hello_world", TokenBucket(10, 10))\nthrottler.add_bucket("hello_world", TokenBucket(30, 20))\n\n\n@throttler.enable("hello_world")\ndef hello_world() -> None:\n    print("Hello World")\n\n\nfor i in range(10):\n    hello_world()\n\ntry:\n    hello_world()\nexcept TokenThrottlerException:\n    print("bucket_one ran out of tokens")\n```\n\nFor other examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.\n\n<a name="storage"></a>\n## 4. Storage\n\n`TokenThrottler` supports `RuntimeStorage` and `RedisStorage`.\n`TokenThrottlerAsync` supports `RedisStorageAsync`\n\nIf you want your own storage engine, feel free to extend the `token_throttler.storage.BucketStorage` or `token_throttler.storage.BucketStorageAsync` classes.\n\nFor storage examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.\n\n<a name="configuration"></a>\n## 5. Configuration\n\nToken throttler supports global configuration by making use of `ThrottlerConfig` class.\n\nConfiguration params:\n- `IDENTIFIER_FAIL_SAFE` - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`\nis set to `True`, no `KeyError` exception will be raised and `consume` will act like a limitless bucket is being consumed.\n- `ENABLE_THREAD_LOCK` - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release\nthe lock once the `consume` is finished. This avoids various race conditions at a slight performance cost.\n\n<a name="configuration-usage"></a>\n### Configuration usage\n\n```python\nfrom token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler\nfrom token_throttler.storage import RuntimeStorage\n\nThrottlerConfig.set({\n   "ENABLE_THREAD_LOCK": False,\n   "IDENTIFIER_FAIL_SAFE": True,\n})\nthrottler: TokenThrottler = TokenThrottler(1, RuntimeStorage())\nthrottler.add_bucket("hello_world", TokenBucket(10, 10))\nthrottler.add_bucket("hello_world", TokenBucket(30, 20))\n...\n```\n',
-    'author': 'Vojko Pribudić',
-    'author_email': 'dmanthing@gmail.com',
-    'maintainer': 'Vojko Pribudić',
-    'maintainer_email': 'dmanthing@gmail.com',
-    'url': 'https://gitlab.com/vojko.pribudic/token-throttler',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+## Table of contents
 
+1. [ Installation ](#installation)
+2. [ Features ](#features)
+3. [ Usage ](#usage)
+    1. [ Manual usage example ](#usage-manual)
+    2. [ Decorator usage example ](#usage-decorator)
+    3. [ FastAPI usage example ](#usage-fastapi)
+4. [ Storage ](#storage)
+5. [ Configuration ](#configuration)
+   1. [ Configuration usage ](#configuration-usage)
 
-setup(**setup_kwargs)
+<a name="installation"></a>
+## 1. Installation
+
+Token throttler is available on PyPI:
+```console 
+$ python -m pip install token-throttler
+```
+Token throttler officially supports Python >= 3.7.
+
+*NOTE*: Depending on the storage engine you pick, you can install token throttler with extras:
+```console 
+$ python -m pip install token-throttler[redis]
+```
+
+<a name="features"></a>
+## 2. Features
+
+- Blocking (TokenThrottler) and non-blocking (TokenThrottlerAsync)
+- Global throttler(s) configuration
+- Configurable token throttler cost and identifier
+- Multiple buckets per throttler per identifier
+- Buckets can be added/removed manually or by a `dict` configuration
+- Manual usage or usage via decorator
+- Decorator usage supports async code too
+- Custom decorator can be written
+- Extendable storage engine (eg. Redis)
+
+<a name="usage"></a>
+## 3. Usage
+
+Token throttler supports both manual usage and via decorator.
+
+Decorator usage supports both async and sync.
+
+<a name="usage-manual"></a>
+### 1) Manual usage example:
+
+```python
+from token_throttler import TokenBucket, TokenThrottler
+from token_throttler.storage import RuntimeStorage
+
+throttler: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())
+throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=10, max_tokens=10))
+throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=30, max_tokens=20))
+
+
+def hello_world() -> None:
+    print("Hello World")
+
+
+for i in range(10):
+    throttler.consume(identifier="hello_world")
+    hello_world()
+
+if throttler.consume(identifier="hello_world"):
+    hello_world()
+else:
+    print("bucket_one ran out of tokens")
+```
+
+<a name="usage-decorator"></a>
+### 2) Decorator usage example:
+
+```python
+from token_throttler import TokenBucket, TokenThrottler, TokenThrottlerException
+from token_throttler.storage import RuntimeStorage
+
+throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
+
+
+@throttler.enable("hello_world")
+def hello_world() -> None:
+    print("Hello World")
+
+
+for i in range(10):
+    hello_world()
+
+try:
+    hello_world()
+except TokenThrottlerException:
+    print("bucket_one ran out of tokens")
+```
+
+<a name="usage-fastapi"></a>
+### 3) FastAPI usage example:
+
+```python
+from fastapi import Depends, FastAPI, Request
+from pydantic import BaseModel
+from token_throttler import TokenThrottler, TokenBucket
+from token_throttler.storage import RuntimeStorage
+from token_throttler.ext.fastapi import FastAPIThrottler
+
+app: FastAPI = FastAPI()
+ban_hammer: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())
+
+
+class User(BaseModel):
+    id: int
+    name: str
+
+
+u1: User = User(id=1, name="Test")
+users: list[User] = [u1]
+
+
+def create_buckets() -> None:
+    for user in users:
+        ban_hammer.add_bucket(
+            str(user.id), TokenBucket(replenish_time=10, max_tokens=10)
+        )
+
+
+# For example purposes only - feel free to load your users with the bucket(s) anywhere else
+app.add_event_handler("startup", create_buckets)
+
+
+# Add your auth logic here
+def get_auth_user() -> User:
+    return u1
+
+
+# Since this is a FastAPI dependency, you can have the `Request` object here too if needed (e.g. storing the JWT token in
+# a request lifecycle).
+# You can also use sub-dependencies like shown below - `auth_user`
+async def get_user_id(
+        request: Request, auth_user: User = Depends(get_auth_user)
+) -> str:
+    return str(auth_user.id)
+
+
+# You can configure the dependency per route, on a router level or on global application level.
+# Pass your unique user identifier (e.g. JWT subject, apikey or user's ID) as a callback parameter 
+# of the `enable` method.
+@app.get(
+    "/throttle", dependencies=[Depends(FastAPIThrottler(ban_hammer).enable(get_user_id))]
+)
+async def read_users():
+    return {"detail": "This is throttled URL"}
+```
+
+For other examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.
+
+<a name="storage"></a>
+## 4. Storage
+
+`TokenThrottler` supports `RuntimeStorage` and `RedisStorage`.
+`TokenThrottlerAsync` supports `RedisStorageAsync`
+
+If you want your own storage engine, feel free to extend the `token_throttler.storage.BucketStorage` or `token_throttler.storage.BucketStorageAsync` classes.
+
+For storage examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.
+
+<a name="configuration"></a>
+## 5. Configuration
+
+Token throttler supports global configuration by making use of `ThrottlerConfig` class.
+
+Configuration params:
+- `IDENTIFIER_FAIL_SAFE` - if invalid identifier is given as a param for the `consume` method and `IDENTIFIER_FAIL_SAFE`
+is set to `True`, no `KeyError` exception will be raised and `consume` will act like a limitless bucket is being consumed.
+- `ENABLE_THREAD_LOCK` - if set to `True`, throttler will acquire a thread lock upon calling `consume` method and release
+the lock once the `consume` is finished. This avoids various race conditions at a slight performance cost.
+
+<a name="configuration-usage"></a>
+### Configuration usage
+
+```python
+from token_throttler import ThrottlerConfig, TokenBucket, TokenThrottler
+from token_throttler.storage import RuntimeStorage
+
+ThrottlerConfig.set({
+   "ENABLE_THREAD_LOCK": False,
+   "IDENTIFIER_FAIL_SAFE": True,
+})
+throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
+...
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `token_throttler-1.2.1/PKG-INFO` & `token_throttler-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-throttler
-Version: 1.2.1
+Version: 1.3.0
 Summary: Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm
 Home-page: https://gitlab.com/vojko.pribudic/token-throttler
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -26,16 +26,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: fastapi
 Provides-Extra: redis
-Requires-Dist: redis (>=4.3.4,<5.0.0); extra == "redis"
+Requires-Dist: fastapi (>=0.95.2,<0.96.0) ; extra == "fastapi"
+Requires-Dist: redis (>=4.4,<5.0) ; extra == "redis"
 Project-URL: Changelog, https://gitlab.com/vojko.pribudic/token-throttler/-/releases
 Project-URL: Repository, https://gitlab.com/vojko.pribudic/token-throttler
 Project-URL: Tracker, https://gitlab.com/vojko.pribudic/token-throttler/-/issues
 Description-Content-Type: text/markdown
 
 # Token throttler
 
@@ -50,14 +52,15 @@
 ## Table of contents
 
 1. [ Installation ](#installation)
 2. [ Features ](#features)
 3. [ Usage ](#usage)
     1. [ Manual usage example ](#usage-manual)
     2. [ Decorator usage example ](#usage-decorator)
+    3. [ FastAPI usage example ](#usage-fastapi)
 4. [ Storage ](#storage)
 5. [ Configuration ](#configuration)
    1. [ Configuration usage ](#configuration-usage)
 
 <a name="installation"></a>
 ## 1. Installation
 
@@ -140,14 +143,72 @@
 
 try:
     hello_world()
 except TokenThrottlerException:
     print("bucket_one ran out of tokens")
 ```
 
+<a name="usage-fastapi"></a>
+### 3) FastAPI usage example:
+
+```python
+from fastapi import Depends, FastAPI, Request
+from pydantic import BaseModel
+from token_throttler import TokenThrottler, TokenBucket
+from token_throttler.storage import RuntimeStorage
+from token_throttler.ext.fastapi import FastAPIThrottler
+
+app: FastAPI = FastAPI()
+ban_hammer: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())
+
+
+class User(BaseModel):
+    id: int
+    name: str
+
+
+u1: User = User(id=1, name="Test")
+users: list[User] = [u1]
+
+
+def create_buckets() -> None:
+    for user in users:
+        ban_hammer.add_bucket(
+            str(user.id), TokenBucket(replenish_time=10, max_tokens=10)
+        )
+
+
+# For example purposes only - feel free to load your users with the bucket(s) anywhere else
+app.add_event_handler("startup", create_buckets)
+
+
+# Add your auth logic here
+def get_auth_user() -> User:
+    return u1
+
+
+# Since this is a FastAPI dependency, you can have the `Request` object here too if needed (e.g. storing the JWT token in
+# a request lifecycle).
+# You can also use sub-dependencies like shown below - `auth_user`
+async def get_user_id(
+        request: Request, auth_user: User = Depends(get_auth_user)
+) -> str:
+    return str(auth_user.id)
+
+
+# You can configure the dependency per route, on a router level or on global application level.
+# Pass your unique user identifier (e.g. JWT subject, apikey or user's ID) as a callback parameter 
+# of the `enable` method.
+@app.get(
+    "/throttle", dependencies=[Depends(FastAPIThrottler(ban_hammer).enable(get_user_id))]
+)
+async def read_users():
+    return {"detail": "This is throttled URL"}
+```
+
 For other examples see [**examples**](https://gitlab.com/vojko.pribudic/token-throttler/-/tree/main/examples) directory.
 
 <a name="storage"></a>
 ## 4. Storage
 
 `TokenThrottler` supports `RuntimeStorage` and `RedisStorage`.
 `TokenThrottlerAsync` supports `RedisStorageAsync`
```

