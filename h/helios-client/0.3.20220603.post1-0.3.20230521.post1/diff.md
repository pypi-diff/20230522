# Comparing `tmp/helios-client-0.3.20220603.post1.tar.gz` & `tmp/helios-client-0.3.20230521.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-client-0.3.20220603.post1.tar", last modified: Sat Jun  4 00:58:15 2022, max compression
+gzip compressed data, was "helios-client-0.3.20230521.post1.tar", last modified: Mon May 22 01:23:07 2023, max compression
```

## Comparing `helios-client-0.3.20220603.post1.tar` & `helios-client-0.3.20230521.post1.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2022-06-04 00:58:15.802761 helios-client-0.3.20220603.post1/
--rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.3.20220603.post1/Copying
--rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.3.20220603.post1/MANIFEST.in
--rw-rw-r--   0 kip       (1000) kip       (1000)     5660 2022-06-04 00:58:15.802761 helios-client-0.3.20220603.post1/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)     4165 2022-06-03 01:42:25.000000 helios-client-0.3.20220603.post1/README.md
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2022-06-04 00:58:15.798761 helios-client-0.3.20220603.post1/Source/
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2022-06-04 00:58:15.798761 helios-client-0.3.20220603.post1/Source/helios/
--rwxrwxr-x   0 kip       (1000) kip       (1000)      336 2022-06-03 01:40:00.000000 helios-client-0.3.20220603.post1/Source/helios/__init__.py
--rw-------   0 kip       (1000) kip       (1000)      221 2022-06-04 00:56:41.000000 helios-client-0.3.20220603.post1/Source/helios/__version__.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2022-06-03 01:39:49.000000 helios-client-0.3.20220603.post1/Source/helios/chunked_upload.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)    30510 2022-06-03 01:39:54.000000 helios-client-0.3.20220603.post1/Source/helios/client.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2022-06-03 01:39:58.000000 helios-client-0.3.20220603.post1/Source/helios/exceptions.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3804 2022-06-03 01:40:05.000000 helios-client-0.3.20220603.post1/Source/helios/requests.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     9378 2022-06-03 01:40:14.000000 helios-client-0.3.20220603.post1/Source/helios/responses.py
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2022-06-04 00:58:15.802761 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/
--rw-rw-r--   0 kip       (1000) kip       (1000)     5660 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)      498 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/SOURCES.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/dependency_links.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)       65 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/requires.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        7 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/top_level.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2022-06-04 00:58:15.000000 helios-client-0.3.20220603.post1/Source/helios_client.egg-info/zip-safe
--rw-rw-r--   0 kip       (1000) kip       (1000)       38 2022-06-04 00:58:15.802761 helios-client-0.3.20220603.post1/setup.cfg
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3215 2022-06-03 04:50:33.000000 helios-client-0.3.20220603.post1/setup.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.295567 helios-client-0.3.20230521.post1/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.3.20230521.post1/Copying
+-rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.3.20230521.post1/MANIFEST.in
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5660 2023-05-22 01:23:07.319567 helios-client-0.3.20230521.post1/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)     4165 2022-06-03 01:42:25.000000 helios-client-0.3.20230521.post1/README.md
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.279567 helios-client-0.3.20230521.post1/Source/
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.299567 helios-client-0.3.20230521.post1/Source/helios/
+-rwxrwxr-x   0 kip       (1000) kip       (1000)      336 2022-06-03 01:40:00.000000 helios-client-0.3.20230521.post1/Source/helios/__init__.py
+-rw-------   0 kip       (1000) kip       (1000)      221 2023-05-22 00:59:00.000000 helios-client-0.3.20230521.post1/Source/helios/__version__.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2022-06-03 01:39:49.000000 helios-client-0.3.20230521.post1/Source/helios/chunked_upload.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)    30510 2022-06-03 01:39:54.000000 helios-client-0.3.20230521.post1/Source/helios/client.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2022-06-03 01:39:58.000000 helios-client-0.3.20230521.post1/Source/helios/exceptions.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3804 2022-06-03 01:40:05.000000 helios-client-0.3.20230521.post1/Source/helios/requests.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     9511 2023-05-22 00:55:53.000000 helios-client-0.3.20230521.post1/Source/helios/responses.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.299567 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5660 2023-05-22 01:23:06.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)      727 2023-05-22 01:23:07.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2023-05-22 01:23:06.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)       65 2023-05-22 01:23:06.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/requires.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        7 2023-05-22 01:23:06.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/top_level.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2023-05-22 01:23:06.000000 helios-client-0.3.20230521.post1/Source/helios_client.egg-info/zip-safe
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.299567 helios-client-0.3.20230521.post1/debian/
+-rw-rw-r--   0 kip       (1000) kip       (1000)      188 2023-05-22 00:59:37.000000 helios-client-0.3.20230521.post1/debian/changelog
+-rw-rw-r--   0 kip       (1000) kip       (1000)     1087 2022-06-03 04:49:46.000000 helios-client-0.3.20230521.post1/debian/control
+-rw-rw-r--   0 kip       (1000) kip       (1000)      385 2022-06-03 01:44:11.000000 helios-client-0.3.20230521.post1/debian/copyright
+-rw-rw-r--   0 kip       (1000) kip       (1000)       11 2019-05-15 03:31:30.000000 helios-client-0.3.20230521.post1/debian/docs
+-rwxr-xr-x   0 kip       (1000) kip       (1000)     3238 2022-06-03 01:41:05.000000 helios-client-0.3.20230521.post1/debian/rules
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.307567 helios-client-0.3.20230521.post1/debian/source/
+-rw-rw-r--   0 kip       (1000) kip       (1000)       12 2015-01-02 04:54:06.000000 helios-client-0.3.20230521.post1/debian/source/format
+-rw-rw-r--   0 kip       (1000) kip       (1000)       63 2019-09-16 23:53:59.000000 helios-client-0.3.20230521.post1/debian/source/options
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2023-05-22 01:23:07.319567 helios-client-0.3.20230521.post1/debian/tests/
+-rw-------   0 kip       (1000) kip       (1000)      834 2022-06-03 01:41:11.000000 helios-client-0.3.20230521.post1/debian/tests/control
+-rwx--x--x   0 kip       (1000) kip       (1000)      417 2022-06-03 01:43:41.000000 helios-client-0.3.20230521.post1/debian/tests/test-import-module.py
+-rwx--x--x   0 kip       (1000) kip       (1000)     3388 2022-06-03 01:41:17.000000 helios-client-0.3.20230521.post1/debian/tests/test-module-usage.py
+-rw-rw-r--   0 kip       (1000) kip       (1000)      213 2019-05-22 05:29:11.000000 helios-client-0.3.20230521.post1/debian/watch
+-rw-rw-r--   0 kip       (1000) kip       (1000)       38 2023-05-22 01:23:07.319567 helios-client-0.3.20230521.post1/setup.cfg
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3215 2022-06-03 04:50:33.000000 helios-client-0.3.20230521.post1/setup.py
```

### Comparing `helios-client-0.3.20220603.post1/Copying` & `helios-client-0.3.20230521.post1/Copying`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/PKG-INFO` & `helios-client-0.3.20230521.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.3.20220603.post1
+Version: 0.3.20230521.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: info@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
```

### Comparing `helios-client-0.3.20220603.post1/README.md` & `helios-client-0.3.20230521.post1/README.md`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/Source/helios/chunked_upload.py` & `helios-client-0.3.20230521.post1/Source/helios/chunked_upload.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/Source/helios/client.py` & `helios-client-0.3.20230521.post1/Source/helios/client.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/Source/helios/exceptions.py` & `helios-client-0.3.20230521.post1/Source/helios/exceptions.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/Source/helios/requests.py` & `helios-client-0.3.20230521.post1/Source/helios/requests.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.3.20220603.post1/Source/helios/responses.py` & `helios-client-0.3.20230521.post1/Source/helios/responses.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @attr.s
 class StoredSong:
     album               = attr.ib(validator=attr.validators.instance_of(str))
     algorithm_age       = attr.ib(validator=attr.validators.instance_of(int))
     artist              = attr.ib(validator=attr.validators.instance_of(str))
     beats_per_minute    = attr.ib(validator=attr.validators.instance_of(float))
     duration            = attr.ib(validator=attr.validators.instance_of(int))
+    fingerprint         = attr.ib(validator=attr.validators.instance_of(str))
     genre               = attr.ib(validator=attr.validators.instance_of(str))
     id                  = attr.ib(validator=attr.validators.instance_of(int))
     isrc                = attr.ib(validator=attr.validators.instance_of(str))
     location            = attr.ib(validator=attr.validators.instance_of(str))
     reference           = attr.ib(validator=attr.validators.instance_of(str))
     title               = attr.ib(validator=attr.validators.instance_of(str))
     year                = attr.ib(validator=attr.validators.instance_of(int))
@@ -38,14 +39,15 @@
 
     # Fields...
     album               = fields.String(required=True)
     algorithm_age       = fields.Integer(required=True)
     artist              = fields.String(required=True)
     beats_per_minute    = fields.Float(required=True)
     duration            = fields.Integer(required=True)
+    fingerprint         = fields.String(required=True)
     genre               = fields.String(required=True)
     id                  = fields.Integer(required=True)
     isrc                = fields.String(required=True)
     location            = fields.String(required=True)
     reference           = fields.String(required=True)
     title               = fields.String(required=True)
     year                = fields.Integer(required=True)
```

### Comparing `helios-client-0.3.20220603.post1/Source/helios_client.egg-info/PKG-INFO` & `helios-client-0.3.20230521.post1/Source/helios_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.3.20220603.post1
+Version: 0.3.20230521.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: info@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
```

### Comparing `helios-client-0.3.20220603.post1/setup.py` & `helios-client-0.3.20230521.post1/setup.py`

 * *Files identical despite different names*

