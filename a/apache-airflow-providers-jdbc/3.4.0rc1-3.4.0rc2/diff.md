# Comparing `tmp/apache-airflow-providers-jdbc-3.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-jdbc-3.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-jdbc-3.4.0rc1.tar", last modified: Tue May 16 15:54:27 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-jdbc-3.4.0rc2.tar", last modified: Fri May 19 17:52:45 2023, max compression
```

## Comparing `apache-airflow-providers-jdbc-3.4.0rc1.tar` & `apache-airflow-providers-jdbc-3.4.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12794 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11246 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/
--rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/hooks/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-03 19:47:07.000000 apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/operators/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12794 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1884 2023-05-16 15:54:27.000000 apache-airflow-providers-jdbc-3.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-16 15:54:26.000000 apache-airflow-providers-jdbc-3.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13011 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11463 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:12:57.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2811 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-05-03 19:47:07.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13011 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-jdbc-3.4.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/setup.py
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/LICENSE` & `apache-airflow-providers-jdbc-3.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/MANIFEST.in` & `apache-airflow-providers-jdbc-3.4.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/PKG-INFO` & `apache-airflow-providers-jdbc-3.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
@@ -147,14 +147,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/README.rst` & `apache-airflow-providers-jdbc-3.4.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
@@ -113,14 +113,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/__init__.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-import airflow
+__all__ = ["__version__"]
 
-__all__ = ["version"]
+__version__ = "3.4.0"
 
-version = "3.4.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-jdbc:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-jdbc:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/get_provider_info.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/hooks/__init__.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/hooks/jdbc.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/operators/__init__.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/airflow/providers/jdbc/operators/jdbc.py` & `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO` & `apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
@@ -147,14 +147,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt` & `apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/pyproject.toml` & `apache-airflow-providers-jdbc-3.4.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
+    # "D400", WIP: see #31135
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/setup.cfg` & `apache-airflow-providers-jdbc-3.4.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.jdbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jdbc
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc1/setup.py` & `apache-airflow-providers-jdbc-3.4.0rc2/setup.py`

 * *Files identical despite different names*

