# Comparing `tmp/questdb-connect-1.0.1.tar.gz` & `tmp/questdb-connect-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-1.0.1.tar", last modified: Mon May 22 13:16:34 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.2.tar", last modified: Mon May 22 13:26:29 2023, max compression
```

## Comparing `questdb-connect-1.0.1.tar` & `questdb-connect-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.196442 questdb-connect-1.0.1/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.1/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4487 2023-05-22 13:16:34.196322 questdb-connect-1.0.1/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3781 2023-05-22 11:44:31.000000 questdb-connect-1.0.1/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2579 2023-05-22 13:16:13.000000 questdb-connect-1.0.1/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:16:34.196480 questdb-connect-1.0.1/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.189591 questdb-connect-1.0.1/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.192042 questdb-connect-1.0.1/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.1/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.1/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.1/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.1/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.1/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.1/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.193290 questdb-connect-1.0.1/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-1.0.1/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.1/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.1/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.1/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.194227 questdb-connect-1.0.1/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4487 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:16:34.000000 questdb-connect-1.0.1/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.194340 questdb-connect-1.0.1/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.1/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.194882 questdb-connect-1.0.1/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.1/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12181 2023-05-22 13:01:48.000000 questdb-connect-1.0.1/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:16:34.195965 questdb-connect-1.0.1/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.1/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.1/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.1/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.515423 questdb-connect-1.0.2/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.2/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4485 2023-05-22 13:26:29.515284 questdb-connect-1.0.2/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3781 2023-05-22 11:44:31.000000 questdb-connect-1.0.2/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 13:25:54.000000 questdb-connect-1.0.2/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:26:29.515464 questdb-connect-1.0.2/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.509406 questdb-connect-1.0.2/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.511512 questdb-connect-1.0.2/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.2/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.2/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.2/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.2/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.2/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.2/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.512388 questdb-connect-1.0.2/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-1.0.2/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.2/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.2/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.2/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.513476 questdb-connect-1.0.2/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4485 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.513596 questdb-connect-1.0.2/src/superset_ext/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.2/src/superset_ext/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.514207 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12810 2023-05-22 13:25:10.000000 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.514986 questdb-connect-1.0.2/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.2/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.2/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.2/tests/test_types.py
```

### Comparing `questdb-connect-1.0.1/LICENSE` & `questdb-connect-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/PKG-INFO` & `questdb-connect-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.1
-Summary: SqlAlchemy/Superset libraries.
+Version: 1.0.2
+Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `questdb-connect-1.0.1/README.md` & `questdb-connect-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/pyproject.toml` & `questdb-connect-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '1.0.1'
+version = '1.0.2'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
-description = "SqlAlchemy/Superset libraries."
+description = "SqlAlchemy/Superset library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

### Comparing `questdb-connect-1.0.1/src/examples/__init__.py` & `questdb-connect-1.0.2/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/examples/hello_world.py` & `questdb-connect-1.0.2/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.2/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/examples/server_utilisation.py` & `questdb-connect-1.0.2/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.2/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.2/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/questdb_connect/__init__.py` & `questdb-connect-1.0.2/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/questdb_connect/dialect.py` & `questdb-connect-1.0.2/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/questdb_connect/function_names.py` & `questdb-connect-1.0.2/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/questdb_connect/types.py` & `questdb-connect-1.0.2/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.2/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.1
-Summary: SqlAlchemy/Superset libraries.
+Version: 1.0.2
+Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `questdb-connect-1.0.1/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.2/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/superset_ext/__init__.py` & `questdb-connect-1.0.2/src/superset_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/superset_ext/db_engine_specs/__init__.py` & `questdb-connect-1.0.2/src/superset_ext/db_engine_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.2/src/superset_ext/db_engine_specs/questdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,28 +18,25 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 from flask_babel import gettext as __
-from flask_babel import lazy_gettext as _
 from marshmallow import Schema, fields
 from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
-    TimeGrain,
-    builtin_time_grains,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 from questdb_connect import remove_public_schema, types as questdb_types
 from questdb_connect.dialect import connection_uri
 from questdb_connect.function_names import FUNCTION_NAMES
@@ -89,36 +86,89 @@
         "PT6H": "date_trunc('hour', {col}) + 21600000000L",
         "P1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
-    ret_list = []
-    for duration, func in _time_grain_expressions.items():
-        if duration:
-            name = builtin_time_grains[duration]
-            ret_list.append(TimeGrain(name, _(name), func, duration))
-    _engine_time_grains = tuple(ret_list)
     column_type_mappings = (
-        (re.compile("^LONG256", re.IGNORECASE), questdb_types.Long256, GenericDataType.STRING),
-        (re.compile("^BOOLEAN", re.IGNORECASE), questdb_types.Boolean, GenericDataType.BOOLEAN),
-        (re.compile("^BYTE", re.IGNORECASE), questdb_types.Byte, GenericDataType.BOOLEAN),
-        (re.compile("^SHORT", re.IGNORECASE), questdb_types.Short, GenericDataType.NUMERIC),
-        (re.compile("^INT", re.IGNORECASE), questdb_types.Int, GenericDataType.NUMERIC),
-        (re.compile("^LONG", re.IGNORECASE), questdb_types.Long, GenericDataType.NUMERIC),
-        (re.compile("^FLOAT", re.IGNORECASE), questdb_types.Float, GenericDataType.NUMERIC),
-        (re.compile("^DOUBLE'", re.IGNORECASE), questdb_types.Double, GenericDataType.NUMERIC),
-        (re.compile("^SYMBOL", re.IGNORECASE), questdb_types.Symbol, GenericDataType.STRING),
-        (re.compile("^STRING", re.IGNORECASE), questdb_types.String, GenericDataType.STRING),
-        (re.compile("^UUID", re.IGNORECASE), questdb_types.UUID, GenericDataType.STRING),
-        (re.compile("^CHAR", re.IGNORECASE), questdb_types.Char, GenericDataType.STRING),
-        (re.compile("^TIMESTAMP", re.IGNORECASE), questdb_types.Timestamp, GenericDataType.TEMPORAL),
-        (re.compile("^DATE", re.IGNORECASE), questdb_types.Date, GenericDataType.TEMPORAL),
-        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), questdb_types.GeohashLong, GenericDataType.STRING)
+        (
+            re.compile("^LONG256", re.IGNORECASE),
+            questdb_types.Long256,
+            GenericDataType.STRING
+        ),
+        (
+            re.compile("^BOOLEAN", re.IGNORECASE),
+            questdb_types.Boolean,
+            GenericDataType.BOOLEAN
+        ),
+        (
+            re.compile("^BYTE", re.IGNORECASE),
+            questdb_types.Byte,
+            GenericDataType.NUMERIC),
+        (
+            re.compile("^SHORT", re.IGNORECASE),
+            questdb_types.Short,
+            GenericDataType.NUMERIC
+        ),
+        (
+            re.compile("^INT", re.IGNORECASE),
+            questdb_types.Int,
+            GenericDataType.NUMERIC
+        ),
+        (
+            re.compile("^LONG", re.IGNORECASE),
+            questdb_types.Long,
+            GenericDataType.NUMERIC
+        ),
+        (
+            re.compile("^FLOAT", re.IGNORECASE),
+            questdb_types.Float,
+            GenericDataType.NUMERIC
+        ),
+        (
+            re.compile("^DOUBLE'", re.IGNORECASE),
+            questdb_types.Double,
+            GenericDataType.NUMERIC
+        ),
+        (
+            re.compile("^SYMBOL", re.IGNORECASE),
+            questdb_types.Symbol,
+            GenericDataType.STRING
+        ),
+        (
+            re.compile("^STRING", re.IGNORECASE),
+            questdb_types.String,
+            GenericDataType.STRING
+        ),
+        (
+            re.compile("^UUID", re.IGNORECASE),
+            questdb_types.UUID,
+            GenericDataType.STRING
+        ),
+        (
+            re.compile("^CHAR", re.IGNORECASE),
+            questdb_types.Char,
+            GenericDataType.STRING
+        ),
+        (
+            re.compile("^TIMESTAMP", re.IGNORECASE),
+            questdb_types.Timestamp,
+            GenericDataType.TEMPORAL
+        ),
+        (
+            re.compile("^DATE", re.IGNORECASE),
+            questdb_types.Date,
+            GenericDataType.TEMPORAL
+        ),
+        (
+            re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE),
+            questdb_types.GeohashLong,
+            GenericDataType.STRING
+        )
     )
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
@@ -142,23 +192,29 @@
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
         return text(remove_public_schema(clause))
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
-        """SQL expression that converts epoch (seconds) to datetime that can be used in a
-        query. The reference column should be denoted as `{col}` in the return
+        """SQL expression that converts epoch (seconds) to datetime that can be used
+        in a query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return '{col} * 1000000'
 
     @classmethod
-    def convert_dttm(cls, target_type: str, dttm: datetime, *_args, **_kwargs) -> Optional[str]:
+    def convert_dttm(
+            cls,
+            target_type: str,
+            dttm: datetime,
+            *_args,
+            **_kwargs
+    ) -> Optional[str]:
         """Convert a Python `datetime` object to a SQL expression.
         :param target_type: The target type of expression
         :param dttm: The datetime object
         :return: The SQL expression
         """
         type_u = target_type.upper()
         if type_u == 'DATE':
@@ -170,15 +226,17 @@
 
     @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
-        return type_code.upper() if type_code and isinstance(type_code, str) else str(type_code)
+        if type_code and isinstance(type_code, str):
+            return type_code.upper()
+        return str(type_code)
 
     @classmethod
     def get_column_spec(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
@@ -200,15 +258,19 @@
             generic_type = GenericDataType.NUMERIC
         elif name_u in ('SYMBOL', 'STRING', 'CHAR', 'LONG256', 'UUID'):
             generic_type = GenericDataType.STRING
         elif name_u in ('DATE', 'TIMESTAMP'):
             generic_type = GenericDataType.TEMPORAL
         elif 'GEOHASH' in name_u and '(' in name_u and ')' in name_u:
             generic_type = GenericDataType.STRING
-        return utils.ColumnSpec(sqla_type, generic_type, generic_type == GenericDataType.TEMPORAL)
+        return utils.ColumnSpec(
+            sqla_type,
+            generic_type,
+            generic_type == GenericDataType.TEMPORAL
+        )
 
     @classmethod
     def get_sqla_column_type(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
@@ -218,15 +280,19 @@
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
         return questdb_types.resolve_type_from_name(native_type).impl
 
     @classmethod
-    def column_datatype_to_string(cls, sqla_column_type: TypeEngine, dialect: Dialect) -> str:
+    def column_datatype_to_string(
+            cls,
+            sqla_column_type: TypeEngine,
+            dialect: Dialect,
+    ) -> str:
         """Convert sqlalchemy column type to string representation.
         By default, removes collation and character encoding info to avoid
         unnecessarily long datatypes.
         :param sqla_column_type: SqlAlchemy column type
         :param dialect: Sqlalchemy dialect
         :return: Compiled column type
         """
@@ -253,15 +319,25 @@
         :param limit: limit to impose on query
         :param show_cols: Show columns in query; otherwise use "*"
         :param indent: Add indentation to query
         :param latest_partition: Only query the latest partition
         :param cols: Columns to include in query
         :return: SQL query
         """
-        return super().select_star(database, table_name, engine, None, limit, show_cols, indent, latest_partition, cols)
+        return super().select_star(
+            database,
+            table_name,
+            engine,
+            None,
+            limit,
+            show_cols,
+            indent,
+            latest_partition,
+            cols
+        )
 
     @classmethod
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
```

### Comparing `questdb-connect-1.0.1/tests/test_dialect.py` & `questdb-connect-1.0.2/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/tests/test_superset.py` & `questdb-connect-1.0.2/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.1/tests/test_types.py` & `questdb-connect-1.0.2/tests/test_types.py`

 * *Files identical despite different names*

