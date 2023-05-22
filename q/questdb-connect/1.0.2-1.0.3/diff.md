# Comparing `tmp/questdb-connect-1.0.2.tar.gz` & `tmp/questdb-connect-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-1.0.2.tar", last modified: Mon May 22 13:26:29 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.3.tar", last modified: Mon May 22 14:23:31 2023, max compression
```

## Comparing `questdb-connect-1.0.2.tar` & `questdb-connect-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.515423 questdb-connect-1.0.2/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.2/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4485 2023-05-22 13:26:29.515284 questdb-connect-1.0.2/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3781 2023-05-22 11:44:31.000000 questdb-connect-1.0.2/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 13:25:54.000000 questdb-connect-1.0.2/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:26:29.515464 questdb-connect-1.0.2/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.509406 questdb-connect-1.0.2/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.511512 questdb-connect-1.0.2/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.2/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.2/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.2/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.2/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.2/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.2/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.512388 questdb-connect-1.0.2/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-1.0.2/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.2/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.2/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.2/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.513476 questdb-connect-1.0.2/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4485 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 13:26:29.000000 questdb-connect-1.0.2/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.513596 questdb-connect-1.0.2/src/superset_ext/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.2/src/superset_ext/__init__.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.514207 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/
--rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12810 2023-05-22 13:25:10.000000 questdb-connect-1.0.2/src/superset_ext/db_engine_specs/questdb.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 13:26:29.514986 questdb-connect-1.0.2/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.2/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.2/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.2/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.912086 questdb-connect-1.0.3/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-1.0.3/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 14:23:31.911922 questdb-connect-1.0.3/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3789 2023-05-22 13:37:39.000000 questdb-connect-1.0.3/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2577 2023-05-22 14:23:15.000000 questdb-connect-1.0.3/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 14:23:31.912175 questdb-connect-1.0.3/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.905616 questdb-connect-1.0.3/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.907825 questdb-connect-1.0.3/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-1.0.3/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-1.0.3/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-1.0.3/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-1.0.3/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-1.0.3/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-1.0.3/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.908838 questdb-connect-1.0.3/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-22 14:22:42.000000 questdb-connect-1.0.3/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-1.0.3/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-1.0.3/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-1.0.3/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.909680 questdb-connect-1.0.3/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4493 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      788 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      160 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 14:23:31.000000 questdb-connect-1.0.3/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.909793 questdb-connect-1.0.3/src/superset_ext/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.3/src/superset_ext/__init__.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.910362 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/
+-rw-r--r--   0 marregui   (501) staff       (20)      843 2023-05-22 12:59:39.000000 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12810 2023-05-22 13:25:10.000000 questdb-connect-1.0.3/src/superset_ext/db_engine_specs/questdb.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 14:23:31.911585 questdb-connect-1.0.3/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-1.0.3/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2844 2023-05-22 13:02:28.000000 questdb-connect-1.0.3/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-1.0.3/tests/test_types.py
```

### Comparing `questdb-connect-1.0.2/LICENSE` & `questdb-connect-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/PKG-INFO` & `questdb-connect-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.2
+Version: 1.0.3
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -32,14 +32,15 @@
 
 The Python module is available here:
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
+<p></p>
 
 _Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
 It provides a comprehensive set of features for interacting with the PostgreSQL database system.
 
 _SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
 communicating with relational databases, including schema creation and modification, an SQL expression
 language, and database connection management. The ORM layer abstracts away the complexities of the
```

### Comparing `questdb-connect-1.0.2/README.md` & `questdb-connect-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 The Python module is available here:
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
+<p></p>
 
 _Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
 It provides a comprehensive set of features for interacting with the PostgreSQL database system.
 
 _SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
 communicating with relational databases, including schema creation and modification, an SQL expression
 language, and database connection management. The ORM layer abstracts away the complexities of the
```

### Comparing `questdb-connect-1.0.2/pyproject.toml` & `questdb-connect-1.0.3/pyproject.toml`

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
-version = '1.0.2'
+version = '1.0.3'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset library."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-1.0.2/src/examples/__init__.py` & `questdb-connect-1.0.3/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/examples/hello_world.py` & `questdb-connect-1.0.3/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.3/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/examples/server_utilisation.py` & `questdb-connect-1.0.3/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.3/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.3/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/questdb_connect/dialect.py` & `questdb-connect-1.0.3/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/questdb_connect/function_names.py` & `questdb-connect-1.0.3/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/questdb_connect/types.py` & `questdb-connect-1.0.3/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-1.0.3/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 1.0.2
+Version: 1.0.3
 Summary: SqlAlchemy/Superset library.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -32,14 +32,15 @@
 
 The Python module is available here:
 
 <a href="https://pypi.org/project/questdb-connect/">
     <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
     https://pypi.org/project/questdb-connect/
 </a>
+<p></p>
 
 _Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
 It provides a comprehensive set of features for interacting with the PostgreSQL database system.
 
 _SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
 communicating with relational databases, including schema creation and modification, an SQL expression
 language, and database connection management. The ORM layer abstracts away the complexities of the
```

### Comparing `questdb-connect-1.0.2/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.3/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/superset_ext/__init__.py` & `questdb-connect-1.0.3/src/superset_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/superset_ext/db_engine_specs/__init__.py` & `questdb-connect-1.0.3/src/superset_ext/db_engine_specs/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/src/superset_ext/db_engine_specs/questdb.py` & `questdb-connect-1.0.3/src/superset_ext/db_engine_specs/questdb.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/tests/test_dialect.py` & `questdb-connect-1.0.3/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/tests/test_superset.py` & `questdb-connect-1.0.3/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-1.0.2/tests/test_types.py` & `questdb-connect-1.0.3/tests/test_types.py`

 * *Files identical despite different names*

