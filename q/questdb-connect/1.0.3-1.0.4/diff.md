# Comparing `tmp/questdb-connect-1.0.3.tar.gz` & `tmp/questdb-connect-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-1.0.3.tar", last modified: Mon May 22 14:23:31 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.4.tar", last modified: Mon May 22 16:16:19 2023, max compression
```

## Comparing `questdb-connect-1.0.3.tar` & `questdb-connect-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.912086 questdb-connect-1.0.3/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.3/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 14:23:31.911922 questdb-connect-1.0.3/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.3/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 14:23:15.000000 questdb-connect-1.0.3/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 14:23:31.912175 questdb-connect-1.0.3/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.905616 questdb-connect-1.0.3/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.907825 questdb-connect-1.0.3/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.3/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.3/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.3/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.3/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.3/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.3/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.908838 questdb-connect-1.0.3/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.3/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.3/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.3/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.3/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.909680 questdb-connect-1.0.3/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.909793 questdb-connect-1.0.3/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.3/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.910362 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12810 2023-05-22 13:25:10.000000 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.911585 questdb-connect-1.0.3/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.3/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.3/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.3/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.662469 questdb-connect-1.0.4/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.4/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 16:16:19.662322 questdb-connect-1.0.4/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.4/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 16:15:43.000000 questdb-connect-1.0.4/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 16:16:19.662510 questdb-connect-1.0.4/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.656192 questdb-connect-1.0.4/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.658533 questdb-connect-1.0.4/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.4/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.4/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.4/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.4/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.4/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.4/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.659616 questdb-connect-1.0.4/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.4/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.4/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.4/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.4/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.660562 questdb-connect-1.0.4/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 16:16:19.000000 questdb-connect-1.0.4/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.660685 questdb-connect-1.0.4/src/superset_ext/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.4/src/superset_ext/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.661307 questdb-connect-1.0.4/src/superset_ext/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.4/src/superset_ext/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12388 2023-05-22 16:15:24.000000 questdb-connect-1.0.4/src/superset_ext/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 16:16:19.662039 questdb-connect-1.0.4/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.4/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.4/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.4/tests/test_types.py
```

### Comparing `questdb-connect-1.0.3/LICENSE` & `questdb-connect-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/PKG-INFO` & `questdb-connect-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.3
+Version: 1.0.4
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-1.0.3/README.md` & `questdb-connect-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/pyproject.toml` & `questdb-connect-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '1.0.3'
+version = '1.0.4'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-1.0.3/src/examples/__init__.py` & `questdb-connect-1.0.4/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/examples/hello_world.py` & `questdb-connect-1.0.4/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.4/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/examples/server_utilisation.py` & `questdb-connect-1.0.4/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.4/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.4/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/questdb_connect/__init__.py` & `questdb-connect-1.0.4/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/questdb_connect/dialect.py` & `questdb-connect-1.0.4/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/questdb_connect/function_names.py` & `questdb-connect-1.0.4/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/questdb_connect/types.py` & `questdb-connect-1.0.4/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.4/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.3
+Version: 1.0.4
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-1.0.3/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.4/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/superset_ext/__init__.py` & `questdb-connect-1.0.4/src/superset_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/superset_ext/db_engine_specs/__init__.py` & `questdb-connect-1.0.4/src/superset_ext/db_engine_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.4/src/superset_ext/db_engine_specs/questdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,23 +71,16 @@
     supports_dynamic_schema = False
     top_keywords = {}
     # https://en.wikipedia.org/wiki/ISO_8601#Durations
     # https://questdb.io/docs/reference/function/date-time/#date_trunc
     _time_grain_expressions = {
         None: '{col}',
         "PT1S": "date_trunc('second', {col})",
-        "PT5S": "date_trunc('second', {col}) + 5000000L",
-        "PT30S": "date_trunc('second', {col}) + 30000000L",
         "PT1M": "date_trunc('minute', {col})",
-        "PT5M": "date_trunc('minute', {col}) + 300000000L",
-        "PT10M": "date_trunc('minute', {col}) + 600000000L",
-        "PT15M": "date_trunc('minute', {col}) + 900000000L",
-        "PT30M": "date_trunc('minute', {col}) + 1800000000L",
         "PT1H": "date_trunc('hour', {col})",
-        "PT6H": "date_trunc('hour', {col}) + 21600000000L",
         "P1D": "date_trunc('day', {col})",
         "P1W": "date_trunc('week', {col})",
         "P1M": "date_trunc('month', {col})",
         "P1Y": "date_trunc('year', {col})",
         "P3M": "date_trunc('quarter', {col})",
     }
     column_type_mappings = (
```

### Comparing `questdb-connect-1.0.3/tests/test_dialect.py` & `questdb-connect-1.0.4/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/tests/test_superset.py` & `questdb-connect-1.0.4/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.3/tests/test_types.py` & `questdb-connect-1.0.4/tests/test_types.py`

 * *Files identical despite different names*

