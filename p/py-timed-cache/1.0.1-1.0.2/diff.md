# Comparing `tmp/py-timed-cache-1.0.1.tar.gz` & `tmp/py-timed-cache-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-timed-cache-1.0.1.tar", last modified: Wed May 10 14:44:19 2023, max compression
+gzip compressed data, was "py-timed-cache-1.0.2.tar", last modified: Mon May 22 08:23:23 2023, max compression
```

## Comparing `py-timed-cache-1.0.1.tar` & `py-timed-cache-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453976 py-timed-cache-1.0.1/
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1067 2023-05-10 13:54:04.000000 py-timed-cache-1.0.1/LICENSE
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-10 14:44:19.453818 py-timed-cache-1.0.1/PKG-INFO
--rw-r--r--   0 nadrian  (546264773) staff       (20)      962 2023-05-10 14:43:21.000000 py-timed-cache-1.0.1/README.md
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.452480 py-timed-cache-1.0.1/py_timed_cache.egg-info/
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/PKG-INFO
--rw-r--r--   0 nadrian  (546264773) staff       (20)      286 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)        1 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)       17 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/top_level.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)       38 2023-05-10 14:44:19.454024 py-timed-cache-1.0.1/setup.cfg
--rw-r--r--   0 nadrian  (546264773) staff       (20)      532 2023-05-10 14:44:15.000000 py-timed-cache-1.0.1/setup.py
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453082 py-timed-cache-1.0.1/tests/
--rw-r--r--   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:00:38.000000 py-timed-cache-1.0.1/tests/__init__.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)      148 2023-05-10 14:19:10.000000 py-timed-cache-1.0.1/tests/context.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1091 2023-05-10 14:35:21.000000 py-timed-cache-1.0.1/tests/test.timedcache.py
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453564 py-timed-cache-1.0.1/timedcache/
--rw-r--r--   0 nadrian  (546264773) staff       (20)       59 2023-05-10 14:17:28.000000 py-timed-cache-1.0.1/timedcache/__init__.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)     2230 2023-05-10 14:18:36.000000 py-timed-cache-1.0.1/timedcache/timedcache.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-22 08:23:23.465126 py-timed-cache-1.0.2/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1067 2023-05-10 13:54:04.000000 py-timed-cache-1.0.2/LICENSE
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-22 08:23:23.464990 py-timed-cache-1.0.2/PKG-INFO
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      962 2023-05-10 14:43:21.000000 py-timed-cache-1.0.2/README.md
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-22 08:23:23.464036 py-timed-cache-1.0.2/py_timed_cache.egg-info/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-22 08:23:23.000000 py-timed-cache-1.0.2/py_timed_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      286 2023-05-22 08:23:23.000000 py-timed-cache-1.0.2/py_timed_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)        1 2023-05-22 08:23:23.000000 py-timed-cache-1.0.2/py_timed_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       17 2023-05-22 08:23:23.000000 py-timed-cache-1.0.2/py_timed_cache.egg-info/top_level.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       38 2023-05-22 08:23:23.465175 py-timed-cache-1.0.2/setup.cfg
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      532 2023-05-22 08:20:54.000000 py-timed-cache-1.0.2/setup.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-22 08:23:23.464433 py-timed-cache-1.0.2/tests/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:00:38.000000 py-timed-cache-1.0.2/tests/__init__.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      148 2023-05-10 14:19:10.000000 py-timed-cache-1.0.2/tests/context.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1562 2023-05-22 08:19:06.000000 py-timed-cache-1.0.2/tests/test_timedcache.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-22 08:23:23.464770 py-timed-cache-1.0.2/timedcache/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       59 2023-05-10 14:17:28.000000 py-timed-cache-1.0.2/timedcache/__init__.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     2230 2023-05-10 14:18:36.000000 py-timed-cache-1.0.2/timedcache/timedcache.py
```

### Comparing `py-timed-cache-1.0.1/LICENSE` & `py-timed-cache-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-timed-cache-1.0.1/PKG-INFO` & `py-timed-cache-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-timed-cache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure Python timed-cache
 Home-page: https://github.com/NicoAdrian/timed-cache
 Author: Nicolas Adrian
 Author-email: nicolasadrian3@gmail.com
 License: MIT
 Keywords: cache,timed-cache,timedcache
 Description-Content-Type: text/markdown
```

### Comparing `py-timed-cache-1.0.1/README.md` & `py-timed-cache-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-timed-cache-1.0.1/py_timed_cache.egg-info/PKG-INFO` & `py-timed-cache-1.0.2/py_timed_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-timed-cache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure Python timed-cache
 Home-page: https://github.com/NicoAdrian/timed-cache
 Author: Nicolas Adrian
 Author-email: nicolasadrian3@gmail.com
 License: MIT
 Keywords: cache,timed-cache,timedcache
 Description-Content-Type: text/markdown
```

### Comparing `py-timed-cache-1.0.1/setup.py` & `py-timed-cache-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as fd:
     readme = fd.read()
 
 setup(
     name="py-timed-cache",
-    version="1.0.1",
+    version="1.0.2",
     description="Pure Python timed-cache",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Nicolas Adrian",
     author_email="nicolasadrian3@gmail.com",
     url="https://github.com/NicoAdrian/timed-cache",
     license="MIT",
```

### Comparing `py-timed-cache-1.0.1/tests/test.timedcache.py` & `py-timed-cache-1.0.2/tests/test_timedcache.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,13 +37,30 @@
         result = foo(*numbers)
         self.assertEqual(result, sum(numbers))
         self.assertEqual(len(l), 1)
         result2 = foo(*numbers)
         self.assertEqual(result2, sum(numbers))
         self.assertEqual(len(l), 1)
 
+    @async_test
+    async def test_cache_async_function(self):
+        l = []
+
+        @timedcache.TimedCache(1)
+        async def foo(*args):
+            l.append(None)
+            return sum(args)
+
+        numbers = [1, 2, 3]
+        result = await foo(*numbers)
+        self.assertEqual(result, sum(numbers))
+        self.assertEqual(len(l), 1)
+        result2 = await foo(*numbers)
+        self.assertEqual(result2, sum(numbers))
+        self.assertEqual(len(l), 1)
+
 
 if __name__ == "__main__":
     try:
         unittest.main()
     except KeyboardInterrupt:
         pass
```

### Comparing `py-timed-cache-1.0.1/timedcache/timedcache.py` & `py-timed-cache-1.0.2/timedcache/timedcache.py`

 * *Files identical despite different names*

