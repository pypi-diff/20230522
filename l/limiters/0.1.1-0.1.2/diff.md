# Comparing `tmp/limiters-0.1.1.tar.gz` & `tmp/limiters-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limiters-0.1.1.tar", max compression
+gzip compressed data, was "limiters-0.1.2.tar", max compression
```

## Comparing `limiters-0.1.1.tar` & `limiters-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1652 2023-05-22 11:19:10.587764 limiters-0.1.1/LICENSE
--rw-r--r--   0        0        0     3528 2023-05-22 11:19:10.587764 limiters-0.1.1/README.md
--rw-r--r--   0        0        0      294 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/__init__.py
--rw-r--r--   0        0        0      727 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/base.py
--rw-r--r--   0        0        0      143 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/py.typed
--rw-r--r--   0        0        0     1544 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/semaphore.lua
--rw-r--r--   0        0        0     5180 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/semaphore.py
--rw-r--r--   0        0        0     2349 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/token_bucket.lua
--rw-r--r--   0        0        0     3523 2023-05-22 11:19:10.587764 limiters-0.1.1/limiters/token_bucket.py
--rw-r--r--   0        0        0     2695 2023-05-22 11:19:10.591764 limiters-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 limiters-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1652 2023-05-22 08:31:26.765266 limiters-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3528 2023-05-22 09:53:05.163953 limiters-0.1.2/README.md
+-rw-r--r--   0        0        0      294 2023-05-22 08:31:26.769266 limiters-0.1.2/limiters/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-22 08:31:26.769266 limiters-0.1.2/limiters/base.py
+-rw-r--r--   0        0        0      143 2023-05-22 08:31:26.769266 limiters-0.1.2/limiters/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:31:26.769266 limiters-0.1.2/limiters/py.typed
+-rw-r--r--   0        0        0     1544 2023-05-22 10:44:36.373118 limiters-0.1.2/limiters/semaphore.lua
+-rw-r--r--   0        0        0     5180 2023-05-22 10:35:56.364509 limiters-0.1.2/limiters/semaphore.py
+-rw-r--r--   0        0        0     2349 2023-05-22 08:31:26.769266 limiters-0.1.2/limiters/token_bucket.lua
+-rw-r--r--   0        0        0     3523 2023-05-22 10:35:19.525032 limiters-0.1.2/limiters/token_bucket.py
+-rw-r--r--   0        0        0     2755 2023-05-22 11:09:17.143122 limiters-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 limiters-0.1.2/PKG-INFO
```

### Comparing `limiters-0.1.1/LICENSE` & `limiters-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/README.md` & `limiters-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/limiters/base.py` & `limiters-0.1.2/limiters/base.py`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/limiters/semaphore.lua` & `limiters-0.1.2/limiters/semaphore.lua`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/limiters/semaphore.py` & `limiters-0.1.2/limiters/semaphore.py`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/limiters/token_bucket.lua` & `limiters-0.1.2/limiters/token_bucket.lua`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/limiters/token_bucket.py` & `limiters-0.1.2/limiters/token_bucket.py`

 * *Files identical despite different names*

### Comparing `limiters-0.1.1/pyproject.toml` & `limiters-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "limiters"
-version = "0.1.1"
+version = "0.1.2"
 description = "Distributed rate limiters"
 license = "BSD-4-Clause"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 readme = "README.md"
 homepage = "https://github.com/otovo/limiters"
 repository = "https://github.com/otovo/limiters"
 keywords = [
@@ -46,14 +46,19 @@
 coverage = "^7"
 pytest = "^7"
 pytest-asyncio = "*"
 pytest-mock = "*"
 pytest-randomly = "*"
 pytest-socket = "*"
 
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
```

### Comparing `limiters-0.1.1/PKG-INFO` & `limiters-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limiters
-Version: 0.1.1
+Version: 0.1.2
 Summary: Distributed rate limiters
 Home-page: https://github.com/otovo/limiters
 License: BSD-4-Clause
 Keywords: async,sync,rate,limiting,limiters
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.11,<4.0
```

