# Comparing `tmp/questdb-connect-0.0.84.tar.gz` & `tmp/questdb-connect-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.84.tar", last modified: Mon May 22 09:38:06 2023, max compression
+gzip compressed data, was "questdb-connect-1.0.0.tar", last modified: Mon May 22 11:00:37 2023, max compression
```

## Comparing `questdb-connect-0.0.84.tar` & `questdb-connect-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.447566 questdb-connect-0.0.84/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.84/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-22 09:38:06.447422 questdb-connect-0.0.84/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.84/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2575 2023-05-22 09:37:34.000000 questdb-connect-0.0.84/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-22 09:38:06.447604 questdb-connect-0.0.84/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.441684 questdb-connect-0.0.84/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.443878 questdb-connect-0.0.84/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.84/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.84/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.84/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.84/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.84/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.84/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.445326 questdb-connect-0.0.84/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.84/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11809 2023-05-22 09:15:51.000000 questdb-connect-0.0.84/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.84/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    13673 2023-05-22 09:37:13.000000 questdb-connect-0.0.84/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5780 2023-05-22 09:34:56.000000 questdb-connect-0.0.84/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.446481 questdb-connect-0.0.84/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      155 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-22 09:38:06.000000 questdb-connect-0.0.84/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-22 09:38:06.447106 questdb-connect-0.0.84/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-18 13:56:07.000000 questdb-connect-0.0.84/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4270 2023-05-18 15:00:19.000000 questdb-connect-0.0.84/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-05-18 17:16:30.000000 questdb-connect-0.0.84/tests/test_types.py
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

### Comparing `questdb-connect-0.0.84/LICENSE` & `questdb-connect-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/PKG-INFO` & `questdb-connect-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-Metadata-Version: 2.1
-Name: questdb-connect
-Version: 0.0.84
-Summary: SqlAlchemy/Superset libraries.
-Author-email: "questdb.io" <miguel@questdb.io>
-Project-URL: Homepage, https://github.com/questdb/questdb-connect/
-Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
+<a href="https://questdb.io/docs/" target="blank">
+    <img alt="QuestDB Logo" src="https://questdb.io/img/questdb-logo-themed.svg" width="305px"/>
+</a>
+<p></p>
+<a href="https://slack.questdb.io">
+    <img src="https://slack.questdb.io/badge.svg" alt="QuestDB community Slack channel"/>
+</a>
 
 ## QuestDB Connect
 
-This module offers an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/), 
-as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using 
+This repository contains an implementation of QuestDB's dialect for [SQLAlchemy](https://www.sqlalchemy.org/),
+as well as an engine specification for [Apache Superset](https://github.com/apache/superset/), using
 [psycopg2](https://www.psycopg.org/) for database connectivity.
 
-Psycopg2 is a widely used and trusted Python module for connecting to and working with PostgreSQL databases. 
+The Python module is available here:
+
+<a href="https://pypi.org/project/questdb-connect/">
+    <img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi"/>
+    https://pypi.org/project/questdb-connect/
+</a>
+
+_Psycopg2_ is a widely used and trusted Python module for connecting to and working with PostgreSQL databases.
 It provides a comprehensive set of features for interacting with the PostgreSQL database system.
 
-SQLAlchemy is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for 
-communicating with relational databases, including schema creation and modification, an SQL expression 
-language, and database connection management. The ORM layer abstracts away the complexities of the 
+_SQLAlchemy_ is an open-source SQL toolkit and ORM library for Python. It provides a high-level API for
+communicating with relational databases, including schema creation and modification, an SQL expression
+language, and database connection management. The ORM layer abstracts away the complexities of the
 database, allowing developers to work with Python objects instead of raw SQL statements.
 
-Apache Superset is a popular open-source business intelligence web application that enables users to 
-visualize and explore data through customizable dashboards and reports. It provides a rich set of data 
+_Apache Superset_ is a popular open-source business intelligence web application that enables users to
+visualize and explore data through customizable dashboards and reports. It provides a rich set of data
 visualizations, including charts, tables, and maps.
 
 ## Requirements
 
-* Python from 3.8.x to 3.10.x
-* Psycopg2
-* SQLAlchemy
+* **Python from 3.8.x to 3.10.x** (superset itself use version _3.9.x_)
+* **Psycopg2** `('psycopg2-binary~=2.9.6')`
+* **SQLAlchemy** `('SQLAlchemy<=1.4.47')`
+
+You need to install these packages because questdb-connect depends on them.
 
 ## Installation
 
 You can install this package using pip:
 
 ```shell
 pip install questdb-connect
 ```
 
-## Sample Usage
+## SQLALchemy Sample Usage
 
-Use the QuestDB dialect by specifying it in your SQLAlchemy connection string, 
+Use the QuestDB dialect by specifying it in your SQLAlchemy connection string,
 from that point on use SQLAlchemy:
 
 ```python
 import datetime
 import os
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
@@ -64,15 +63,15 @@
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base(metadata=MetaData())
 
 
 class Signal(Base):
     __tablename__ = 'signal'
-    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True), )
+    __table_args__ = (qdbc.QDBTableEngine('signal', 'ts', qdbc.PartitionBy.HOUR, is_wal=True),)
     source = Column(qdbc.Symbol)
     value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
     engine = create_engine('questdb://localhost:8812/main')
@@ -89,12 +88,19 @@
             engine.dispose()
 
 
 if __name__ == '__main__':
     main()
 ```
 
+## Superset Installation
+
+<img alt="QuestDB Logo" src="docs/superset.png"/>
+
+Follow the instructions available here
+[https://superset.apache.org/docs/installation/installing-superset-from-scratch/](https://superset.apache.org/docs/installation/installing-superset-from-scratch/).
+
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
 please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md)
 if you would like to push a PR.
```

### Comparing `questdb-connect-0.0.84/pyproject.toml` & `questdb-connect-1.0.0/pyproject.toml`

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
-version = '0.0.84'
+version = '1.0.0'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.84/src/examples/__init__.py` & `questdb-connect-1.0.0/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/examples/hello_world.py` & `questdb-connect-1.0.0/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/examples/psycopg2_connect.py` & `questdb-connect-1.0.0/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/examples/server_utilisation.py` & `questdb-connect-1.0.0/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/examples/sqlalchemy_orm.py` & `questdb-connect-1.0.0/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/examples/sqlalchemy_raw.py` & `questdb-connect-1.0.0/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect/__init__.py` & `questdb-connect-1.0.0/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect/dialect.py` & `questdb-connect-1.0.0/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect/function_names.py` & `questdb-connect-1.0.0/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect/superset_engine.py` & `questdb-connect-1.0.0/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect/types.py` & `questdb-connect-1.0.0/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-1.0.0/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/tests/test_dialect.py` & `questdb-connect-1.0.0/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/tests/test_superset.py` & `questdb-connect-1.0.0/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.84/tests/test_types.py` & `questdb-connect-1.0.0/tests/test_types.py`

 * *Files identical despite different names*

