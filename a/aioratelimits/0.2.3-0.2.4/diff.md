# Comparing `tmp/aioratelimits-0.2.3.tar.gz` & `tmp/aioratelimits-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioratelimits-0.2.3.tar", max compression
+gzip compressed data, was "aioratelimits-0.2.4.tar", max compression
```

## Comparing `aioratelimits-0.2.3.tar` & `aioratelimits-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.3/README.md
--rw-r--r--   0        0        0     1346 2023-05-21 18:02:57.139940 aioratelimits-0.2.3/aioratelimits.py
--rw-r--r--   0        0        0      475 2023-05-21 18:02:50.699930 aioratelimits-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1384 2023-05-21 18:03:43.994243 aioratelimits-0.2.3/setup.py
--rw-r--r--   0        0        0     1422 2023-05-21 18:03:43.994496 aioratelimits-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      868 2022-08-21 06:32:22.351981 aioratelimits-0.2.4/README.md
+-rw-r--r--   0        0        0     1362 2023-05-21 18:28:33.784928 aioratelimits-0.2.4/aioratelimits.py
+-rw-r--r--   0        0        0      475 2023-05-21 18:30:40.777539 aioratelimits-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1384 2023-05-21 18:31:04.969449 aioratelimits-0.2.4/setup.py
+-rw-r--r--   0        0        0     1422 2023-05-21 18:31:04.969747 aioratelimits-0.2.4/PKG-INFO
```

### Comparing `aioratelimits-0.2.3/README.md` & `aioratelimits-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `aioratelimits-0.2.3/aioratelimits.py` & `aioratelimits-0.2.4/aioratelimits.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,11 @@
                 result = await coro
                 future.set_result(result)
             except Exception as exc:
                 future.set_exception(exc)
 
             await asyncio.sleep(self.delay)
 
-    def run(self, coro: Coroutine) -> asyncio.Future:
+    def run(self, coro: Coroutine[Any, Any, T]) -> asyncio.Future[T]:
         future = asyncio.get_running_loop().create_future()
         self.call_queue.put_nowait((coro, future))
         return future
```

### Comparing `aioratelimits-0.2.3/setup.py` & `aioratelimits-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['aioratelimits']
 setup_kwargs = {
     'name': 'aioratelimits',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': '',
     'long_description': "# aioratelimits\n\nClient rate limiter. It enqueues function calls and run them as leaky bucket to\nensure specified rates.\n\n## Implementation\n\nLeaky bucket. We have one queue for requests and `count` number of workers.\nEach worker can handle one request per `delay` seconds\n\n## Install\n\n```\npip install aioratelimits\n```\n\n## Use\n\nThe following code prints not more than 2 lines per second.\n\n```python\nimport asyncio\nfrom aioratelimits import RateLimiter\n\n\nasync def critical_resource(i: int):\n    print('request:', i)\n\n\nasync def main():\n    async with RateLimiter(count=2, delay=1) as limiter:\n        await asyncio.gather(*(\n            limiter.run(critical_resource(i))\n            for i in range(10)\n        ))\n\n\nasyncio.run(main())\n```\n\nArguments to `RateLimiter`:\n- `count` - how many calls can we do in the specified interval\n- `delay` - the interval in seconds \n",
     'author': 'Dmitry Kostromin',
     'author_email': 'kupec-k@ya.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kupec/aioratelimits',
```

### Comparing `aioratelimits-0.2.3/PKG-INFO` & `aioratelimits-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioratelimits
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Home-page: https://github.com/kupec/aioratelimits
 Keywords: rates,ratelimit,ratelimiter,leaky,bucket
 Author: Dmitry Kostromin
 Author-email: kupec-k@ya.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

