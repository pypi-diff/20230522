# Comparing `tmp/jao-py-0.3.5.tar.gz` & `tmp/jao-py-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jao-py-0.3.5.tar", last modified: Wed Jan 18 22:07:09 2023, max compression
+gzip compressed data, was "jao-py-0.3.6.tar", last modified: Sun May 21 21:58:45 2023, max compression
```

## Comparing `jao-py-0.3.5.tar` & `jao-py-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:07:09.195683 jao-py-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-18 22:06:41.000000 jao-py-0.3.5/LICENSE.MD
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-18 22:07:09.195683 jao-py-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-18 22:06:41.000000 jao-py-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:07:09.195683 jao-py-0.3.5/jao/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:07:09.195683 jao-py-0.3.5/jao/CWE/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/CWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/CWE/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/CWE/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/CWE/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/CWE/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:07:09.195683 jao-py-0.3.5/jao/beta/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/beta/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/jao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-01-18 22:06:41.000000 jao-py-0.3.5/jao/webservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 22:07:09.195683 jao-py-0.3.5/jao_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-18 22:07:09.000000 jao-py-0.3.5/jao_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-18 22:07:09.000000 jao-py-0.3.5/jao_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 22:07:09.000000 jao-py-0.3.5/jao_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-18 22:07:09.000000 jao-py-0.3.5/jao_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-18 22:07:09.000000 jao-py-0.3.5/jao_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-18 22:07:09.199683 jao-py-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-18 22:06:41.000000 jao-py-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.848231 jao-py-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 21:58:34.000000 jao-py-0.3.6/LICENSE.MD
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 21:58:45.848231 jao-py-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-21 21:58:34.000000 jao-py-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/CWE/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/CWE/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.844231 jao-py-0.3.6/jao/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/beta/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/jao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-21 21:58:34.000000 jao-py-0.3.6/jao/webservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:58:45.848231 jao-py-0.3.6/jao_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 21:58:45.000000 jao-py-0.3.6/jao_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 21:58:45.848231 jao-py-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-21 21:58:34.000000 jao-py-0.3.6/setup.py
```

### Comparing `jao-py-0.3.5/LICENSE.MD` & `jao-py-0.3.6/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/PKG-INFO` & `jao-py-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.5/README.md` & `jao-py-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao/CWE/jao.py` & `jao-py-0.3.6/jao/CWE/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao/CWE/parsers.py` & `jao-py-0.3.6/jao/CWE/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao/beta/jao.py` & `jao-py-0.3.6/jao/beta/jao.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao/jao.py` & `jao-py-0.3.6/jao/jao.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import itertools
 from .exceptions import NoMatchingDataError
 from .parsers import parse_final_domain, parse_base_output
 from typing import List, Dict
 from .util import to_snake_case
 
 __title__ = "jao-py"
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 __author__ = "Frank Boerman"
 __license__ = "MIT"
 
 
 class JaoPublicationToolClient:
     BASEURL = "https://publicationtool.jao.eu/core/api/core/"
     BASEURL2 = "https://publicationtool.jao.eu/core/api/data/"
@@ -128,22 +128,30 @@
 
     def query_maxbex(self, day: pd.Timestamp) -> List[Dict]:
         return self._query_base(day, 'maxExchanges')
 
     def query_minmax_np(self, day: pd.Timestamp) -> List[Dict]:
         return self._query_base(day, 'maxNetPos')
 
+    def query_allocationconstraint(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> List[Dict]:
+        return self._query_base_fromto(d_from, d_to, 'allocationConstraint')
+
 
 class JaoPublicationToolPandasClient(JaoPublicationToolClient):
     def query_final_domain(self, mtu: pd.Timestamp, presolved: bool = None, cne: str = None,
                            co: str = None) -> pd.DataFrame:
         return parse_final_domain(
             super().query_final_domain(mtu=mtu, presolved=presolved, cne=cne, co=co)
         )
 
+    def query_allocationconstraint(self, d_from: pd.Timestamp, d_to: pd.Timestamp) -> pd.DataFrame:
+        return parse_base_output(
+            super().query_allocationconstraint(d_from=d_from, d_to=d_to)
+        ).rename(columns=lambda c: c.split('_')[1] + '_' + ('import' if 'Down' in c.split('_')[0] else 'export'))
+
     def query_net_position(self, day: pd.Timestamp) -> pd.DataFrame:
         return parse_base_output(
             super().query_net_position(day=day)
         ).rename(columns=lambda x: x.replace('hub_', '')) \
             .rename(columns={'DE': 'DE_LU'})
 
     def query_active_constraints(self, day: pd.Timestamp) -> pd.DataFrame:
```

### Comparing `jao-py-0.3.5/jao/parsers.py` & `jao-py-0.3.6/jao/parsers.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao/webservice.py` & `jao-py-0.3.6/jao/webservice.py`

 * *Files identical despite different names*

### Comparing `jao-py-0.3.5/jao_py.egg-info/PKG-INFO` & `jao-py-0.3.6/jao_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jao-py
-Version: 0.3.5
+Version: 0.3.6
 Summary: A python API wrapper for JAO.eu
 Home-page: https://github.com/fboerman/jao-py
 Author: Frank Boerman
 Author-email: frank@fboerman.nl
 License: MIT
 Keywords: JAO data api energy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jao-py-0.3.5/setup.py` & `jao-py-0.3.6/setup.py`

 * *Files identical despite different names*

