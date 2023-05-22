# Comparing `tmp/FastSession-0.1.1.tar.gz` & `tmp/fastsession-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastSession-0.1.1.tar", last modified: Mon May 15 08:20:08 2023, max compression
+gzip compressed data, was "fastsession-0.1.2.tar", last modified: Mon May 22 02:50:06 2023, max compression
```

## Comparing `FastSession-0.1.1.tar` & `fastsession-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.934772 FastSession-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.921948 FastSession-0.1.1/FastSession.egg-info/
--rw-rw-rw-   0        0        0     3272 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 08:20:08.000000 FastSession-0.1.1/FastSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 FastSession-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3272 2023-05-15 08:20:08.934772 FastSession-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-05-15 07:54:01.000000 FastSession-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.924456 FastSession-0.1.1/fastsession/
--rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 FastSession-0.1.1/fastsession/__init__.py
--rw-rw-rw-   0        0        0    10213 2023-05-15 07:50:50.000000 FastSession-0.1.1/fastsession/fast_session_middleware.py
--rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 FastSession-0.1.1/fastsession/memory_store.py
--rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 FastSession-0.1.1/fastsession/timed_signature_serializer.py
--rw-rw-rw-   0        0        0       42 2023-05-15 08:20:08.934772 FastSession-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-15 08:14:22.000000 FastSession-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:20:08.925454 FastSession-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 FastSession-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     8754 2023-05-15 07:00:42.000000 FastSession-0.1.1/tests/test_session_middleware.py
--rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 FastSession-0.1.1/tests/test_store_memory.py
--rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 FastSession-0.1.1/tests/test_timed_signature_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.779543 fastsession-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.684017 fastsession-0.1.2/FastSession.egg-info/
+-rw-rw-rw-   0        0        0     3272 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 fastsession-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3272 2023-05-22 02:50:06.775546 fastsession-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2557 2023-05-15 07:54:01.000000 fastsession-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.733013 fastsession-0.1.2/fastsession/
+-rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 fastsession-0.1.2/fastsession/__init__.py
+-rw-rw-rw-   0        0        0    10213 2023-05-15 07:50:50.000000 fastsession-0.1.2/fastsession/fast_session_middleware.py
+-rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 fastsession-0.1.2/fastsession/memory_store.py
+-rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 fastsession-0.1.2/fastsession/timed_signature_serializer.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 02:50:06.780546 fastsession-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-05-22 02:43:40.000000 fastsession-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.772542 fastsession-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 fastsession-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     8754 2023-05-15 07:00:42.000000 fastsession-0.1.2/tests/test_session_middleware.py
+-rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 fastsession-0.1.2/tests/test_store_memory.py
+-rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 fastsession-0.1.2/tests/test_timed_signature_serializer.py
```

### Comparing `FastSession-0.1.1/FastSession.egg-info/PKG-INFO` & `fastsession-0.1.2/FastSession.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FastSession
-Version: 0.1.1
+Name: fastsession
+Version: 0.1.2
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FastSession-0.1.1/LICENSE` & `fastsession-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/PKG-INFO` & `fastsession-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FastSession
-Version: 0.1.1
+Name: fastsession
+Version: 0.1.2
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FastSession-0.1.1/README.md` & `fastsession-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/fastsession/fast_session_middleware.py` & `fastsession-0.1.2/fastsession/fast_session_middleware.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/fastsession/memory_store.py` & `fastsession-0.1.2/fastsession/memory_store.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/fastsession/timed_signature_serializer.py` & `fastsession-0.1.2/fastsession/timed_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/setup.py` & `fastsession-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="FastSession",
-    version="0.1.1",
+    name="fastsession",
+    version="0.1.2",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="A session middleware for Starlette and FastAPI",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/FastSession",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
-    tests_require=["pytest","httpx"],
+    tests_require=["pytest", "httpx"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `FastSession-0.1.1/tests/test_session_middleware.py` & `fastsession-0.1.2/tests/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/tests/test_store_memory.py` & `fastsession-0.1.2/tests/test_store_memory.py`

 * *Files identical despite different names*

### Comparing `FastSession-0.1.1/tests/test_timed_signature_serializer.py` & `fastsession-0.1.2/tests/test_timed_signature_serializer.py`

 * *Files identical despite different names*

