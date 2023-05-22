# Comparing `tmp/psycopg_infdate-1.0.1.tar.gz` & `tmp/psycopg_infdate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg_infdate-1.0.1.tar", last modified: Sat Apr 29 22:57:15 2023, max compression
+gzip compressed data, was "psycopg_infdate-1.0.2.tar", last modified: Mon May 22 17:59:50 2023, max compression
```

## Comparing `psycopg_infdate-1.0.1.tar` & `psycopg_infdate-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-04-29 22:57:15.411215 psycopg_infdate-1.0.1/
--rw-r--r--   0 pjb1008    (501) staff       (20)     7652 2023-04-29 22:38:10.000000 psycopg_infdate-1.0.1/LICENSE
--rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-04-29 22:57:15.411094 psycopg_infdate-1.0.1/PKG-INFO
--rw-r--r--   0 pjb1008    (501) staff       (20)     4262 2023-04-29 22:03:05.000000 psycopg_infdate-1.0.1/README.md
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-04-29 22:57:15.410164 psycopg_infdate-1.0.1/psycopg_infdate/
--rw-r--r--   0 pjb1008    (501) staff       (20)     8282 2023-04-29 22:03:05.000000 psycopg_infdate-1.0.1/psycopg_infdate/__init__.py
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-04-29 22:57:15.410949 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/
--rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-04-29 22:57:15.000000 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/PKG-INFO
--rw-r--r--   0 pjb1008    (501) staff       (20)      254 2023-04-29 22:57:15.000000 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/SOURCES.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)        1 2023-04-29 22:57:15.000000 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/dependency_links.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)       11 2023-04-29 22:57:15.000000 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/requires.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)       16 2023-04-29 22:57:15.000000 psycopg_infdate-1.0.1/psycopg_infdate.egg-info/top_level.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)      782 2023-04-29 22:42:37.000000 psycopg_infdate-1.0.1/pyproject.toml
--rw-r--r--   0 pjb1008    (501) staff       (20)       38 2023-04-29 22:57:15.411246 psycopg_infdate-1.0.1/setup.cfg
+drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.142082 psycopg_infdate-1.0.2/
+-rw-r--r--   0 pjb1008    (501) staff       (20)     7652 2023-04-29 22:38:10.000000 psycopg_infdate-1.0.2/LICENSE
+-rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-05-22 17:59:50.141969 psycopg_infdate-1.0.2/PKG-INFO
+-rw-r--r--   0 pjb1008    (501) staff       (20)     4262 2023-04-29 22:03:05.000000 psycopg_infdate-1.0.2/README.md
+drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.140870 psycopg_infdate-1.0.2/psycopg_infdate/
+-rw-r--r--   0 pjb1008    (501) staff       (20)     8689 2023-05-22 17:54:06.000000 psycopg_infdate-1.0.2/psycopg_infdate/__init__.py
+drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.141827 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/
+-rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/PKG-INFO
+-rw-r--r--   0 pjb1008    (501) staff       (20)      254 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/SOURCES.txt
+-rw-r--r--   0 pjb1008    (501) staff       (20)        1 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/dependency_links.txt
+-rw-r--r--   0 pjb1008    (501) staff       (20)       11 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/requires.txt
+-rw-r--r--   0 pjb1008    (501) staff       (20)       16 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/top_level.txt
+-rw-r--r--   0 pjb1008    (501) staff       (20)      782 2023-05-22 17:59:25.000000 psycopg_infdate-1.0.2/pyproject.toml
+-rw-r--r--   0 pjb1008    (501) staff       (20)       38 2023-05-22 17:59:50.142117 psycopg_infdate-1.0.2/setup.cfg
```

### Comparing `psycopg_infdate-1.0.1/LICENSE` & `psycopg_infdate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psycopg_infdate-1.0.1/PKG-INFO` & `psycopg_infdate-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg_infdate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support postgresql 'infinity'::DATE in psycopg3
 Author-email: Peter Benie <pjb1008@cam.ac.uk>
 Project-URL: Homepage, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psycopg_infdate-1.0.1/README.md` & `psycopg_infdate-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `psycopg_infdate-1.0.1/psycopg_infdate/__init__.py` & `psycopg_infdate-1.0.2/psycopg_infdate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 __all__ = ('register_inf_date_handler',
            'date_plus_infinity', 'PlusInfDate',
            'date_minus_infinity', 'MinusInfDate',
            'datetime_plus_infinity', 'PlusInfDatetimeNoTz',
            'datetime_minus_infinity', 'MinusInfDatetimeNoTz',
            'datetime_tz_plus_infinity', 'PlusInfDatetime',
-           'datetime_tz_minus_infinity', 'MinusInfDatetime')
+           'datetime_tz_minus_infinity', 'MinusInfDatetime',
+           'PGDate', 'PGDateTime')
 
 
 class _BaseInfDate:
     _inf_str: str
     _inf_text: bytes
     _inf_binary: bytes
     _inf_oid: int
@@ -94,16 +95,21 @@
         return NotImplemented
 
     def __eq__(self, other):
         if isinstance(other, _BasePlusInfDate):
             return True
         if isinstance(other, (dt.date, dt.datetime, _BaseMinusInfDate)):
             return False
+        if isinstance(other, str) and other == 'infinity':
+            return True
         return NotImplemented
 
+    def __hash__(self):
+        return hash('pginfinity')
+
 
 class _BaseMinusInfDate(_BaseInfDate):
     _inf_str = '-infinity'
     _inf_text = b'-infinity'
     __slots__ = ()
 
     def __lt__(self, other):
@@ -119,16 +125,21 @@
         return NotImplemented
 
     def __eq__(self, other):
         if isinstance(other, _BasePlusInfDate):
             return True
         if isinstance(other, (dt.date, dt.datetime, _BaseMinusInfDate)):
             return False
+        if isinstance(other, str) and other == '-infinity':
+            return True
         return NotImplemented
 
+    def __hash__(self):
+        return hash('-pginfinity')
+
 
 class PlusInfDate(_BasePlusInfDate):
     _inf_binary = b'\x7f\xff\xff\xff'
     _inf_oid = postgres.types["date"].oid
     __slots__ = ()
 
 
@@ -230,7 +241,11 @@
                                                             datetime_plus_infinity, datetime_minus_infinity))
     obj.adapters.register_loader("timestamptz", text_loader(TimestamptzLoader,
                                                             PlusInfDatetime, MinusInfDatetime,
                                                             datetime_tz_plus_infinity, datetime_tz_minus_infinity))
     obj.adapters.register_loader("timestamptz", binary_loader(TimestamptzBinaryLoader,
                                                               PlusInfDatetime, MinusInfDatetime,
                                                               datetime_tz_plus_infinity, datetime_tz_minus_infinity))
+
+
+PGDate = Union[dt.date, _BaseInfDate]
+PGDateTime = Union[dt.datetime, _BaseInfDate]
```

### Comparing `psycopg_infdate-1.0.1/psycopg_infdate.egg-info/PKG-INFO` & `psycopg_infdate-1.0.2/psycopg_infdate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psycopg-infdate
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support postgresql 'infinity'::DATE in psycopg3
 Author-email: Peter Benie <pjb1008@cam.ac.uk>
 Project-URL: Homepage, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psycopg_infdate-1.0.1/pyproject.toml` & `psycopg_infdate-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psycopg_infdate"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Peter Benie", email="pjb1008@cam.ac.uk" },
 ]
 description = "Support postgresql 'infinity'::DATE in psycopg3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

