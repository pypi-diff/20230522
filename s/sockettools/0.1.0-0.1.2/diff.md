# Comparing `tmp/sockettools-0.1.0.tar.gz` & `tmp/sockettools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockettools-0.1.0.tar", last modified: Fri May 19 18:29:14 2023, max compression
+gzip compressed data, was "sockettools-0.1.2.tar", last modified: Mon May 22 17:54:23 2023, max compression
```

## Comparing `sockettools-0.1.0.tar` & `sockettools-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:29:14.483406 sockettools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35077 2023-05-19 18:29:00.000000 sockettools-0.1.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-19 18:29:14.483406 sockettools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-19 18:29:00.000000 sockettools-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-19 18:29:00.000000 sockettools-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:29:14.483406 sockettools-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:29:14.479406 sockettools-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:29:14.479406 sockettools-0.1.0/src/sockettools/
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-19 18:29:00.000000 sockettools-0.1.0/src/sockettools/network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:29:14.479406 sockettools-0.1.0/src/sockettools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-19 18:29:14.000000 sockettools-0.1.0/src/sockettools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-19 18:29:14.000000 sockettools-0.1.0/src/sockettools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:29:14.000000 sockettools-0.1.0/src/sockettools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 18:29:14.000000 sockettools-0.1.0/src/sockettools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:54:23.164775 sockettools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-22 17:54:09.000000 sockettools-0.1.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-22 17:54:23.164775 sockettools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-22 17:54:09.000000 sockettools-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 17:54:09.000000 sockettools-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:54:23.164775 sockettools-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:54:23.156774 sockettools-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:54:23.160775 sockettools-0.1.2/src/sockettools/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/clienthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 17:54:09.000000 sockettools-0.1.2/src/sockettools/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:54:23.160775 sockettools-0.1.2/src/sockettools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-22 17:54:23.000000 sockettools-0.1.2/src/sockettools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 17:54:23.000000 sockettools-0.1.2/src/sockettools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:54:23.000000 sockettools-0.1.2/src/sockettools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:54:23.000000 sockettools-0.1.2/src/sockettools.egg-info/top_level.txt
```

### Comparing `sockettools-0.1.0/PKG-INFO` & `sockettools-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockettools
-Version: 0.1.0
+Version: 0.1.2
 Summary: Wrapper around built-in python sockets library
 Author-email: Highghlow <highghlow@proton.me>
 Project-URL: Homepage, https://github.com/highghlow/SocketTools
 Project-URL: Bug Tracker, https://github.com/highghlow/SocketTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sockettools-0.1.0/README.md` & `sockettools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sockettools-0.1.0/pyproject.toml` & `sockettools-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "sockettools"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Highghlow", email="highghlow@proton.me" },
 ]
 description = "Wrapper around built-in python sockets library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sockettools-0.1.0/src/sockettools.egg-info/PKG-INFO` & `sockettools-0.1.2/src/sockettools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockettools
-Version: 0.1.0
+Version: 0.1.2
 Summary: Wrapper around built-in python sockets library
 Author-email: Highghlow <highghlow@proton.me>
 Project-URL: Homepage, https://github.com/highghlow/SocketTools
 Project-URL: Bug Tracker, https://github.com/highghlow/SocketTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

