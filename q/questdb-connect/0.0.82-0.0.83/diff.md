# Comparing `tmp/questdb-connect-0.0.82.tar.gz` & `tmp/questdb-connect-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.82.tar", last modified: Fri May 19 10:00:32 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.83.tar", last modified: Mon May 22 09:18:36 2023, max compression
```

## Comparing `questdb-connect-0.0.82.tar` & `questdb-connect-0.0.83.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.545717 questdb-connect-0.0.82/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.82/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 10:00:32.545580 questdb-connect-0.0.82/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.82/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-19 10:00:05.000000 questdb-connect-0.0.82/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-19 10:00:32.545754 questdb-connect-0.0.82/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.540279 questdb-connect-0.0.82/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.542677 questdb-connect-0.0.82/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.82/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.82/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.82/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.82/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.82/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.82/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.543876 questdb-connect-0.0.82/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.82/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11778 2023-05-19 09:49:25.000000 questdb-connect-0.0.82/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.82/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    13615 2023-05-19 09:49:31.000000 questdb-connect-0.0.82/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5865 2023-05-19 08:53:49.000000 questdb-connect-0.0.82/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.544719 questdb-connect-0.0.82/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-19 10:00:32.000000 questdb-connect-0.0.82/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-19 10:00:32.545313 questdb-connect-0.0.82/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.82/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.82/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.82/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.044484 questdb-connect-0.0.83/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.83/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-22 09:18:36.044358 questdb-connect-0.0.83/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.83/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-22 09:16:05.000000 questdb-connect-0.0.83/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 09:18:36.044522 questdb-connect-0.0.83/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.039110 questdb-connect-0.0.83/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.041263 questdb-connect-0.0.83/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.83/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.83/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.83/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.83/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.83/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.83/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.042436 questdb-connect-0.0.83/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.83/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-0.0.83/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.83/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13618 2023-05-22 09:15:51.000000 questdb-connect-0.0.83/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5865 2023-05-19 08:53:49.000000 questdb-connect-0.0.83/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.043364 questdb-connect-0.0.83/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-22 09:18:36.000000 questdb-connect-0.0.83/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:18:36.044001 questdb-connect-0.0.83/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.83/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.83/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.83/tests/test_types.py
```

### Comparing `questdb-connect-0.0.82/LICENSE` & `questdb-connect-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/PKG-INFO` & `questdb-connect-0.0.83/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.82
+Version: 0.0.83
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.82/README.md` & `questdb-connect-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/pyproject.toml` & `questdb-connect-0.0.83/pyproject.toml`

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
-version = '0.0.82'
+version = '0.0.83'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -50,15 +50,15 @@
 
 [project.optional-dependencies]
 test = [
     'psycopg2-binary~=2.9.6',
     'SQLAlchemy<=1.4.47',
     'apache-superset>=2.1.0',
     'sqlparse==0.4.3',
-    'ruff~=0.0.261',
+    'ruff~=0.0.269',
     'pytest~=7.3.0',
 ]
 
 [tool.ruff]
 # https://github.com/charliermarsh/ruff#configuration
 select = ["PL", "RUF", "TCH", "TID", "PT", "C4", "B", "S", "I"]
 line-length = 120
```

### Comparing `questdb-connect-0.0.82/src/examples/__init__.py` & `questdb-connect-0.0.83/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/examples/hello_world.py` & `questdb-connect-0.0.83/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.83/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/examples/server_utilisation.py` & `questdb-connect-0.0.83/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.83/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.83/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/questdb_connect/__init__.py` & `questdb-connect-0.0.83/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/questdb_connect/dialect.py` & `questdb-connect-0.0.83/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,14 +267,15 @@
     supports_multivalues_insert = True
     supports_comments = True
     inline_comments = False
     postfetch_lastrowid = False
     non_native_boolean_check_constraint = False
     max_identifier_length = 255
     _user_defined_max_identifier_length = 255
+    _has_native_hstore = False
     supports_is_distinct_from = False
 
     @classmethod
     def dbapi(cls):
         import questdb_connect as dbapi
         return dbapi
```

### Comparing `questdb-connect-0.0.82/src/questdb_connect/function_names.py` & `questdb-connect-0.0.83/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.83/src/questdb_connect/superset_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 
 
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
-    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname"
+    sqlalchemy_uri_placeholder = "questdb://user:password@host:port/database"
     parameters_schema = QDBParametersSchema()
-    time_groupby_inline = True
+    time_groupby_inline = False
     allows_hidden_cc_in_orderby = True
     time_secondary_columns = True
     try_remove_schema_from_table_name = True
     max_column_name_length = 120
     supports_dynamic_schema = False
     top_keywords = {}
     # https://en.wikipedia.org/wiki/ISO_8601#Durations
```

### Comparing `questdb-connect-0.0.82/src/questdb_connect/types.py` & `questdb-connect-0.0.83/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.83/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.82
+Version: 0.0.83
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.82/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.83/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/tests/test_dialect.py` & `questdb-connect-0.0.83/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/tests/test_superset.py` & `questdb-connect-0.0.83/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.82/tests/test_types.py` & `questdb-connect-0.0.83/tests/test_types.py`

 * *Files identical despite different names*

