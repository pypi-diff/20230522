# Comparing `tmp/asyncio_pool_ng-0.7.2.tar.gz` & `tmp/asyncio_pool_ng-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_pool_ng-0.7.2.tar", max compression
+gzip compressed data, was "asyncio_pool_ng-0.8.0.tar", max compression
```

## Comparing `asyncio_pool_ng-0.7.2.tar` & `asyncio_pool_ng-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1067 2022-11-27 01:25:31.260000 asyncio_pool_ng-0.7.2/LICENSE
--rw-r--r--   0        0        0     4043 2022-11-29 14:28:54.470000 asyncio_pool_ng-0.7.2/README.md
--rw-r--r--   0        0        0      202 2022-12-08 21:32:35.419004 asyncio_pool_ng-0.7.2/asyncio_pool/__init__.py
--rw-r--r--   0        0        0      167 2022-11-25 23:36:40.230000 asyncio_pool_ng-0.7.2/asyncio_pool/_anyio.py
--rw-r--r--   0        0        0     8381 2022-12-08 21:28:15.609004 asyncio_pool_ng-0.7.2/asyncio_pool/_pool.py
--rw-r--r--   0        0        0      217 2022-11-29 14:30:12.670000 asyncio_pool_ng-0.7.2/asyncio_pool/_typing.py
--rw-r--r--   0        0        0        0 2022-11-25 12:59:38.015375 asyncio_pool_ng-0.7.2/asyncio_pool/py.typed
--rw-r--r--   0        0        0     1569 2022-12-08 21:32:35.419004 asyncio_pool_ng-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4881 1970-01-01 00:00:00.000000 asyncio_pool_ng-0.7.2/setup.py
--rw-r--r--   0        0        0     4850 1970-01-01 00:00:00.000000 asyncio_pool_ng-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-11-27 01:25:31.000000 asyncio_pool_ng-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4002 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/README.md
+-rw-r--r--   0        0        0      202 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/__init__.py
+-rw-r--r--   0        0        0     9080 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/_pool.py
+-rw-r--r--   0        0        0      244 2023-05-22 14:00:42.724655 asyncio_pool_ng-0.8.0/asyncio_pool/_typing.py
+-rw-r--r--   0        0        0        0 2022-11-25 12:59:38.000000 asyncio_pool_ng-0.8.0/asyncio_pool/py.typed
+-rw-r--r--   0        0        0     3621 2023-05-22 14:00:42.734655 asyncio_pool_ng-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 asyncio_pool_ng-0.8.0/PKG-INFO
```

### Comparing `asyncio_pool_ng-0.7.2/LICENSE` & `asyncio_pool_ng-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio_pool_ng-0.7.2/README.md` & `asyncio_pool_ng-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/asyncio-pool-ng)](https://pypi.org/project/asyncio-pool-ng/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![](https://github.com/smithk86/asyncio-pool-ng/workflows/ci/badge.svg)](https://github.com/smithk86/asyncio-pool-ng/actions?query=workflow%3Aci)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## About
 
-**AsyncioPoolNG** takes the ideas used in [asyncio-pool](https://github.com/gistart/asyncio-pool) and wraps them around a [TaskGroup](https://anyio.readthedocs.io/en/stable/tasks.html) from [anyio](https://anyio.readthedocs.io/en/stable/index.html).
+**AsyncioPoolNG** takes the ideas used in [asyncio-pool](https://github.com/gistart/asyncio-pool) and wraps them around an [asyncio.TaskGroup](https://docs.python.org/3/library/asyncio-task.html#task-groups).
 
 `AsyncioPool` has three main functions `spawn`, `map`, and `itermap`.
 
 1. `spawn`: Schedule an async function on the pool and get a future back which will eventually have either the result or the exception from the function.
 2. `map`: Spawn an async function for each item in an iterable object, and return a set containing a future for each item.
 
 - `asyncio.wait()` can be used to wait for the set of futures to complete.
```

### Comparing `asyncio_pool_ng-0.7.2/setup.py` & `asyncio_pool_ng-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,105 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asyncio-pool-ng
+Version: 0.8.0
+Summary: A pool of coroutine functions.
+Home-page: https://github.com/smithk86/asyncio-pool-ng
+License: MIT
+Author: Kyle Smith
+Author-email: smithk86@smc3.com
+Requires-Python: >=3.11,<4
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Documentation, https://smithk86.github.io/asyncio-pool-ng
+Project-URL: Repository, https://github.com/smithk86/asyncio-pool-ng
+Description-Content-Type: text/markdown
 
-packages = \
-['asyncio_pool']
+# asyncio-pool-ng
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://img.shields.io/pypi/v/asyncio-pool-ng)](https://pypi.org/project/asyncio-pool-ng/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/asyncio-pool-ng)](https://pypi.org/project/asyncio-pool-ng/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![](https://github.com/smithk86/asyncio-pool-ng/workflows/ci/badge.svg)](https://github.com/smithk86/asyncio-pool-ng/actions?query=workflow%3Aci)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-install_requires = \
-['anyio>=3.6']
-
-entry_points = \
-{'console_scripts': ['pytest = pytest:main']}
-
-setup_kwargs = {
-    'name': 'asyncio-pool-ng',
-    'version': '0.7.2',
-    'description': 'A pool of coroutine functions.',
-    'long_description': '# asyncio-pool-ng\n\n[![PyPI version](https://img.shields.io/pypi/v/asyncio-pool-ng)](https://pypi.org/project/asyncio-pool-ng/)\n[![Python Versions](https://img.shields.io/pypi/pyversions/asyncio-pool-ng)](https://pypi.org/project/asyncio-pool-ng/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![](https://github.com/smithk86/asyncio-pool-ng/workflows/ci/badge.svg)](https://github.com/smithk86/asyncio-pool-ng/actions?query=workflow%3Aci)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## About\n\n**AsyncioPoolNG** takes the ideas used in [asyncio-pool](https://github.com/gistart/asyncio-pool) and wraps them around a [TaskGroup](https://anyio.readthedocs.io/en/stable/tasks.html) from [anyio](https://anyio.readthedocs.io/en/stable/index.html).\n\n`AsyncioPool` has three main functions `spawn`, `map`, and `itermap`.\n\n1. `spawn`: Schedule an async function on the pool and get a future back which will eventually have either the result or the exception from the function.\n2. `map`: Spawn an async function for each item in an iterable object, and return a set containing a future for each item.\n\n- `asyncio.wait()` can be used to wait for the set of futures to complete.\n- When the `AsyncioPool` closes, it will wait for all tasks to complete. All pending futures will be complete once it is closed.\n\n3. `itermap`: Works similarly to `map` but returns an [Async Generator](https://docs.python.org/3/library/typing.html#typing.AsyncGenerator "Async Generator") which yields each future as it completes.\n\n## Differences from asyncio-pool\n\n1. `asyncio-pool-ng` implements [Python typing](https://typing.readthedocs.io/en/latest/) and passes validation checks with [mypy](http://mypy-lang.org/)\'s strict mode. This helps IDEs and static type checkers know what type of result to expect when getting data from a completed future.\n2. `asyncio-pool` uses callbacks to process data before returning it; `asyncio-pool-ng` only returns [Future](https://docs.python.org/3.10/library/asyncio-future.html#asyncio.Future) instances directly. The future will contain either a result or an exception which can then be handled as needed.\n3. While `asyncio-pool` schedules [Coroutine](https://docs.python.org/3/library/typing.html#typing.Coroutine) instances directly, `asyncio-pool-ng` takes the callable and arguments, and creates the Coroutine instance at execution time.\n\n## Example\n\n```python title="example.py"\nimport asyncio\nimport logging\nfrom random import random\n\nfrom asyncio_pool import AsyncioPool\n\n\nlogging.basicConfig(level=logging.INFO)\n\n\nasync def worker(number: int) -> int:\n    await asyncio.sleep(random() / 2)\n    return number * 2\n\n\nasync def main() -> None:\n    result: int = 0\n    results: list[int] = []\n\n    async with AsyncioPool(2) as pool:\n        """spawn task and wait for the results"""\n        result = await pool.spawn(worker, 5)\n        assert result == 10\n        logging.info(f"results for pool.spawn(worker, 5): {result}")\n\n        """spawn task and get results later"""\n        future: asyncio.Future[int] = pool.spawn(worker, 5)\n\n        # do other stuff\n\n        result = await future\n        assert result == 10\n\n        """map an async function to a set of values"""\n        futures: set[asyncio.Future[int]] = pool.map(worker, range(10))\n        await asyncio.wait(futures)\n        results = [x.result() for x in futures]\n        logging.info(f"results for pool.map(worker, range(10)): {results}")\n        results.sort()\n        assert results == [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]\n\n        """iterate futures as they complete"""\n        logging.info("results for pool.itermap(worker, range(10)):")\n        results = []\n        async for future in pool.itermap(worker, range(10)):\n            results.append(future.result())\n            logging.info(f"> {future.result()}")\n\n        results.sort()\n        assert results == [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]\n\n\nasyncio.run(main())\n```\n',
-    'author': 'Kyle Smith',
-    'author_email': 'smithk86@smc3.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/smithk86/asyncio-pool-ng',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4',
-}
+## About
 
+**AsyncioPoolNG** takes the ideas used in [asyncio-pool](https://github.com/gistart/asyncio-pool) and wraps them around an [asyncio.TaskGroup](https://docs.python.org/3/library/asyncio-task.html#task-groups).
+
+`AsyncioPool` has three main functions `spawn`, `map`, and `itermap`.
+
+1. `spawn`: Schedule an async function on the pool and get a future back which will eventually have either the result or the exception from the function.
+2. `map`: Spawn an async function for each item in an iterable object, and return a set containing a future for each item.
+
+- `asyncio.wait()` can be used to wait for the set of futures to complete.
+- When the `AsyncioPool` closes, it will wait for all tasks to complete. All pending futures will be complete once it is closed.
+
+3. `itermap`: Works similarly to `map` but returns an [Async Generator](https://docs.python.org/3/library/typing.html#typing.AsyncGenerator "Async Generator") which yields each future as it completes.
+
+## Differences from asyncio-pool
+
+1. `asyncio-pool-ng` implements [Python typing](https://typing.readthedocs.io/en/latest/) and passes validation checks with [mypy](http://mypy-lang.org/)'s strict mode. This helps IDEs and static type checkers know what type of result to expect when getting data from a completed future.
+2. `asyncio-pool` uses callbacks to process data before returning it; `asyncio-pool-ng` only returns [Future](https://docs.python.org/3.10/library/asyncio-future.html#asyncio.Future) instances directly. The future will contain either a result or an exception which can then be handled as needed.
+3. While `asyncio-pool` schedules [Coroutine](https://docs.python.org/3/library/typing.html#typing.Coroutine) instances directly, `asyncio-pool-ng` takes the callable and arguments, and creates the Coroutine instance at execution time.
+
+## Example
+
+```python title="example.py"
+import asyncio
+import logging
+from random import random
+
+from asyncio_pool import AsyncioPool
+
+
+logging.basicConfig(level=logging.INFO)
+
+
+async def worker(number: int) -> int:
+    await asyncio.sleep(random() / 2)
+    return number * 2
+
+
+async def main() -> None:
+    result: int = 0
+    results: list[int] = []
+
+    async with AsyncioPool(2) as pool:
+        """spawn task and wait for the results"""
+        result = await pool.spawn(worker, 5)
+        assert result == 10
+        logging.info(f"results for pool.spawn(worker, 5): {result}")
+
+        """spawn task and get results later"""
+        future: asyncio.Future[int] = pool.spawn(worker, 5)
+
+        # do other stuff
+
+        result = await future
+        assert result == 10
+
+        """map an async function to a set of values"""
+        futures: set[asyncio.Future[int]] = pool.map(worker, range(10))
+        await asyncio.wait(futures)
+        results = [x.result() for x in futures]
+        logging.info(f"results for pool.map(worker, range(10)): {results}")
+        results.sort()
+        assert results == [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+
+        """iterate futures as they complete"""
+        logging.info("results for pool.itermap(worker, range(10)):")
+        results = []
+        async for future in pool.itermap(worker, range(10)):
+            results.append(future.result())
+            logging.info(f"> {future.result()}")
+
+        results.sort()
+        assert results == [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+
+
+asyncio.run(main())
+```
 
-setup(**setup_kwargs)
```

