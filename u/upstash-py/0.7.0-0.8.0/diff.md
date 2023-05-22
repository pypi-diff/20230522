# Comparing `tmp/upstash_py-0.7.0.tar.gz` & `tmp/upstash_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_py-0.7.0.tar", max compression
+gzip compressed data, was "upstash_py-0.8.0.tar", max compression
```

## Comparing `upstash_py-0.7.0.tar` & `upstash_py-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      363 2023-05-19 12:33:50.766534 upstash_py-0.7.0/README.md
--rw-r--r--   0        0        0      379 2023-05-22 11:36:29.853072 upstash_py-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.7.0/upstash_py/__init__.py
--rw-r--r--   0        0        0    87423 2023-05-19 12:09:27.190405 upstash_py-0.7.0/upstash_py/client.py
--rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_py-0.7.0/upstash_py/config.py
--rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.7.0/upstash_py/exception.py
--rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.7.0/upstash_py/http/decode.py
--rw-r--r--   0        0        0     2584 2023-05-19 12:16:11.244880 upstash_py-0.7.0/upstash_py/http/execute.py
--rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.7.0/upstash_py/play.py
--rw-r--r--   0        0        0       61 2023-05-19 11:53:59.079435 upstash_py-0.7.0/upstash_py/play2.py
--rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.7.0/upstash_py/schema/commands/parameters.py
--rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.7.0/upstash_py/schema/commands/returns.py
--rw-r--r--   0        0        0      729 2023-05-19 12:15:03.869929 upstash_py-0.7.0/upstash_py/schema/http.py
--rw-r--r--   0        0        0      154 2023-05-19 11:45:14.791080 upstash_py-0.7.0/upstash_py/schema/telemetry.py
--rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.7.0/upstash_py/utils/base.py
--rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.7.0/upstash_py/utils/comparison.py
--rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.7.0/upstash_py/utils/exception.py
--rw-r--r--   0        0        0     4130 2023-05-19 13:48:26.411672 upstash_py-0.7.0/upstash_py/utils/format.py
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 upstash_py-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      363 2023-05-19 12:33:50.766534 upstash_py-0.8.0/README.md
+-rw-r--r--   0        0        0      379 2023-05-22 11:47:26.956631 upstash_py-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 11:23:56.540070 upstash_py-0.8.0/upstash_py/__init__.py
+-rw-r--r--   0        0        0    87423 2023-05-19 12:09:27.190405 upstash_py-0.8.0/upstash_py/client.py
+-rw-r--r--   0        0        0      308 2023-05-16 14:24:46.481207 upstash_py-0.8.0/upstash_py/config.py
+-rw-r--r--   0        0        0       44 2023-03-08 07:44:02.265644 upstash_py-0.8.0/upstash_py/exception.py
+-rw-r--r--   0        0        0      755 2023-05-04 15:53:00.952164 upstash_py-0.8.0/upstash_py/http/decode.py
+-rw-r--r--   0        0        0     2584 2023-05-19 12:16:11.244880 upstash_py-0.8.0/upstash_py/http/execute.py
+-rw-r--r--   0        0        0     1030 2023-05-04 15:39:39.039487 upstash_py-0.8.0/upstash_py/play.py
+-rw-r--r--   0        0        0       61 2023-05-19 11:53:59.079435 upstash_py-0.8.0/upstash_py/play2.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:36:04.331779 upstash_py-0.8.0/upstash_py/py.typed
+-rw-r--r--   0        0        0      409 2023-04-14 12:17:17.899972 upstash_py-0.8.0/upstash_py/schema/commands/parameters.py
+-rw-r--r--   0        0        0     1119 2023-05-13 16:00:21.639249 upstash_py-0.8.0/upstash_py/schema/commands/returns.py
+-rw-r--r--   0        0        0      729 2023-05-19 12:15:03.869929 upstash_py-0.8.0/upstash_py/schema/http.py
+-rw-r--r--   0        0        0      154 2023-05-19 11:45:14.791080 upstash_py-0.8.0/upstash_py/schema/telemetry.py
+-rw-r--r--   0        0        0      107 2023-04-13 16:18:51.335437 upstash_py-0.8.0/upstash_py/utils/base.py
+-rw-r--r--   0        0        0      242 2023-04-14 14:58:16.064260 upstash_py-0.8.0/upstash_py/utils/comparison.py
+-rw-r--r--   0        0        0     3333 2023-05-04 07:39:00.163434 upstash_py-0.8.0/upstash_py/utils/exception.py
+-rw-r--r--   0        0        0     4130 2023-05-19 13:48:26.411672 upstash_py-0.8.0/upstash_py/utils/format.py
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 upstash_py-0.8.0/PKG-INFO
```

### Comparing `upstash_py-0.7.0/upstash_py/client.py` & `upstash_py-0.8.0/upstash_py/client.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/http/decode.py` & `upstash_py-0.8.0/upstash_py/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/http/execute.py` & `upstash_py-0.8.0/upstash_py/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/play.py` & `upstash_py-0.8.0/upstash_py/play.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/schema/commands/returns.py` & `upstash_py-0.8.0/upstash_py/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/schema/http.py` & `upstash_py-0.8.0/upstash_py/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/utils/exception.py` & `upstash_py-0.8.0/upstash_py/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/upstash_py/utils/format.py` & `upstash_py-0.8.0/upstash_py/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_py-0.7.0/PKG-INFO` & `upstash_py-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

