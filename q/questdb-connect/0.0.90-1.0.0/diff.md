# Comparing `tmp/questdb-connect-0.0.90.tar.gz` & `tmp/questdb-connect-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.90.tar", last modified: Mon May 22 13:03:43 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.0.tar", last modified: Mon May 22 11:00:37 2023, max compression
```

## Comparing `questdb-connect-0.0.90.tar` & `questdb-connect-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.454105 questdb-connect-0.0.90/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.90/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4488 2023-05-22 13:03:43.453973 questdb-connect-0.0.90/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3781 2023-05-22 11:44:31.000000 questdb-connect-0.0.90/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2580 2023-05-22 13:01:48.000000 questdb-connect-0.0.90/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:03:43.454140 questdb-connect-0.0.90/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.447981 questdb-connect-0.0.90/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.450525 questdb-connect-0.0.90/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.90/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.90/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.90/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.90/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.90/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.90/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.451591 questdb-connect-0.0.90/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.90/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-0.0.90/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.90/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-0.0.90/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.452424 questdb-connect-0.0.90/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4488 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:03:43.000000 questdb-connect-0.0.90/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.452536 questdb-connect-0.0.90/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-0.0.90/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.452988 questdb-connect-0.0.90/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-0.0.90/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12181 2023-05-22 13:01:48.000000 questdb-connect-0.0.90/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:03:43.453702 questdb-connect-0.0.90/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.90/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-0.0.90/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.90/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.366616 questdb-connect-1.0.0/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.0/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4434 2023-05-22 11:00:37.366481 questdb-connect-1.0.0/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3728 2023-05-22 10:59:42.000000 questdb-connect-1.0.0/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2574 2023-05-22 10:58:49.000000 questdb-connect-1.0.0/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 11:00:37.366658 questdb-connect-1.0.0/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.359512 questdb-connect-1.0.0/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.362189 questdb-connect-1.0.0/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.0/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.0/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.0/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.0/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.0/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.0/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.364154 questdb-connect-1.0.0/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-1.0.0/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.0/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.0/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13673 2023-05-22 09:37:13.000000 questdb-connect-1.0.0/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.0/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.365272 questdb-connect-1.0.0/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4434 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-22 11:00:37.000000 questdb-connect-1.0.0/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 11:00:37.366109 questdb-connect-1.0.0/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.0/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-1.0.0/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.0/tests/test_types.py
```

### Comparing `questdb-connect-0.0.90/LICENSE` & `questdb-connect-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/PKG-INFO` & `questdb-connect-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.90
+Version: 1.0.0
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -108,15 +108,15 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<img alt="QuestDB Logo" src="docs/superset.png"/>
 
 Follow the instructions available here
 [https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
```

### Comparing `questdb-connect-0.0.90/README.md` & `questdb-connect-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<img alt="QuestDB Logo" src="docs/superset.png"/>
 
 Follow the instructions available here
 [https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
```

### Comparing `questdb-connect-0.0.90/pyproject.toml` & `questdb-connect-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.90'
+version = '1.0.0'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -42,15 +42,15 @@
 'Homepage' = "https://github.com/questdb/questdb-connect/"
 'Bug Tracker' = "https://github.com/questdb/questdb-connect/issues/"
 
 [project.entry-points.'sqlalchemy.dialects']
 questdb = 'questdb_connect.dialect:QuestDBDialect'
 
 [project.entry-points.'superset.db_engine_specs']
-questdb = 'superset_ext.db_engine_specs.questdb:QDBEngineSpec'
+questdb = 'questdb_connect.superset_engine:QDBEngineSpec'
 
 [project.optional-dependencies]
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
```

### Comparing `questdb-connect-0.0.90/src/examples/__init__.py` & `questdb-connect-1.0.0/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/examples/hello_world.py` & `questdb-connect-1.0.0/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.0/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/examples/server_utilisation.py` & `questdb-connect-1.0.0/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.0/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.0/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/questdb_connect/__init__.py` & `questdb-connect-1.0.0/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/questdb_connect/dialect.py` & `questdb-connect-1.0.0/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/questdb_connect/function_names.py` & `questdb-connect-1.0.0/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/questdb_connect/types.py` & `questdb-connect-1.0.0/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.0/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.90
+Version: 1.0.0
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -108,15 +108,15 @@
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Superset Installation
 
-<img alt="QuestDB Logo" src="https://github.com/questdb/questdb-connect/blob/main/docs/superset.png"/>
+<img alt="QuestDB Logo" src="docs/superset.png"/>
 
 Follow the instructions available here
 [https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
```

### Comparing `questdb-connect-0.0.90/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.0/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 src/examples/psycopg2_connect.py
 src/examples/server_utilisation.py
 src/examples/sqlalchemy_orm.py
 src/examples/sqlalchemy_raw.py
 src/questdb_connect/__init__.py
 src/questdb_connect/dialect.py
 src/questdb_connect/function_names.py
+src/questdb_connect/superset_engine.py
 src/questdb_connect/types.py
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
-src/superset_ext/__init__.py
-src/superset_ext/db_engine_specs/__init__.py
-src/superset_ext/db_engine_specs/questdb.py
 tests/test_dialect.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.90/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.0/src/questdb_connect/superset_engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,18 +36,17 @@
     BasicParametersType,
     TimeGrain,
     builtin_time_grains,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-from questdb_connect import remove_public_schema, types as questdb_types
-from questdb_connect.dialect import connection_uri
-from questdb_connect.function_names import FUNCTION_NAMES
-
+from . import remove_public_schema, types
+from .dialect import connection_uri
+from .function_names import FUNCTION_NAMES
 
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # https://preset.io/blog/building-database-connector/
 # https://preset.io/blog/improving-apache-superset-integration-database-sqlalchemy/
 
 
@@ -95,31 +94,32 @@
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
         if duration:
             name = builtin_time_grains[duration]
             ret_list.append(TimeGrain(name, _(name), func, duration))
     _engine_time_grains = tuple(ret_list)
-    column_type_mappings = (
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
+    _default_column_type_mappings = (
+        (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
+        (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
+        (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
+        (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
+        (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
+        (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
+        (re.compile("^FLOAT", re.IGNORECASE), types.Float, GenericDataType.NUMERIC),
+        (re.compile("^DOUBLE'", re.IGNORECASE), types.Double, GenericDataType.NUMERIC),
+        (re.compile("^SYMBOL", re.IGNORECASE), types.Symbol, GenericDataType.STRING),
+        (re.compile("^STRING", re.IGNORECASE), types.String, GenericDataType.STRING),
+        (re.compile("^UUID", re.IGNORECASE), types.UUID, GenericDataType.STRING),
+        (re.compile("^CHAR", re.IGNORECASE), types.Char, GenericDataType.STRING),
+        (re.compile("^TIMESTAMP", re.IGNORECASE), types.Timestamp, GenericDataType.TEMPORAL),
+        (re.compile("^DATE", re.IGNORECASE), types.Date, GenericDataType.TEMPORAL),
+        (re.compile(r"^GEOHASH\(\d+[b|c]\)", re.IGNORECASE), types.GeohashLong, GenericDataType.STRING)
     )
+    column_type_mappings = _default_column_type_mappings
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
@@ -141,14 +141,23 @@
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
         return text(remove_public_schema(clause))
 
     @classmethod
+    def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
+        """Return a dict of all supported time grains including any
+        potential added grains but excluding any potentially disabled
+        grains in the config file.
+        :return: All time grain expressions supported by the engine
+        """
+        return cls._time_grain_expressions
+
+    @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return '{col} * 1000000'
@@ -173,27 +182,57 @@
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
         return type_code.upper() if type_code and isinstance(type_code, str) else str(type_code)
 
     @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        return cls._engine_time_grains
+
+    @classmethod
+    def get_column_types(
+            cls,
+            column_type: Optional[str],
+    ) -> Optional[Tuple[TypeEngine, GenericDataType]]:
+        """Return a sqlalchemy native column type and generic data type that
+        corresponds to the column type defined in the data source (return None
+        to use default type inferred by SQLAlchemy). Override `column_type_mappings`
+        for specific needs (see MSSQL for example of NCHAR/NVARCHAR handling).
+        :param column_type: Column type returned by inspector
+        :return: SQLAlchemy and generic Superset column types
+        """
+        if not column_type:
+            return None
+        for regex, sqla_type, generic_type in cls._default_column_type_mappings:
+            matching_name = regex.search(column_type)
+            if matching_name:
+                return (
+                    types.resolve_type_from_name(sqla_type.__visit_name__).impl,
+                    generic_type
+                )
+        return None
+
+    @classmethod
     def get_column_spec(
             cls,
             native_type: Optional[str],
             db_extra: Optional[Dict[str, Any]] = None,
             source: utils.ColumnTypeSource = utils.ColumnTypeSource.GET_TABLE,
     ) -> Optional[utils.ColumnSpec]:
         """Get generic type related specs regarding a native column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
-        sqla_type = questdb_types.resolve_type_from_name(native_type)
+        sqla_type = types.resolve_type_from_name(native_type)
         if not sqla_type:
             return BaseEngineSpec.get_column_spec(native_type, db_extra, source)
         name_u = sqla_type.__visit_name__
         generic_type = None
         if name_u == 'BOOLEAN':
             generic_type = GenericDataType.BOOLEAN
         elif name_u in ('BYTE', 'SHORT', 'INT', 'LONG', 'FLOAT', 'DOUBLE'):
@@ -215,15 +254,15 @@
     ) -> Optional[TypeEngine]:
         """Converts native database type to sqlalchemy column type.
         :param native_type: Native database type
         :param db_extra: The database extra object
         :param source: Type coming from the database table or cursor description
         :return: ColumnSpec object
         """
-        return questdb_types.resolve_type_from_name(native_type).impl
+        return types.resolve_type_from_name(native_type).impl
 
     @classmethod
     def column_datatype_to_string(cls, sqla_column_type: TypeEngine, dialect: Dialect) -> str:
         """Convert sqlalchemy column type to string representation.
         By default, removes collation and character encoding info to avoid
         unnecessarily long datatypes.
         :param sqla_column_type: SqlAlchemy column type
```

### Comparing `questdb-connect-0.0.90/tests/test_dialect.py` & `questdb-connect-1.0.0/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.90/tests/test_types.py` & `questdb-connect-1.0.0/tests/test_types.py`

 * *Files identical despite different names*

