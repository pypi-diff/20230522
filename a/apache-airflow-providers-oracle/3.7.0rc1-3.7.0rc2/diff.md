# Comparing `tmp/apache-airflow-providers-oracle-3.7.0rc1.tar.gz` & `tmp/apache-airflow-providers-oracle-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-oracle-3.7.0rc1.tar", last modified: Tue May 16 15:54:49 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-oracle-3.7.0rc2.tar", last modified: Fri May 19 17:53:07 2023, max compression
```

## Comparing `apache-airflow-providers-oracle-3.7.0rc1.tar` & `apache-airflow-providers-oracle-3.7.0rc2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13402 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11826 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/example_oracle.py
--rw-r--r--   0 root         (0) root         (0)     2950 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17534 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13402 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-oracle-3.7.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:06.000000 apache-airflow-providers-oracle-3.7.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-05-19 17:53:06.000000 apache-airflow-providers-oracle-3.7.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:18:45.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-05-19 17:53:06.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17534 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/hooks/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/operators/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/transfers/oracle_to_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13619 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-oracle-3.7.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-19 17:53:07.000000 apache-airflow-providers-oracle-3.7.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-19 17:53:06.000000 apache-airflow-providers-oracle-3.7.0rc2/setup.py
```

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/LICENSE` & `apache-airflow-providers-oracle-3.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/MANIFEST.in` & `apache-airflow-providers-oracle-3.7.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/PKG-INFO` & `apache-airflow-providers-oracle-3.7.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
@@ -150,14 +150,17 @@
 * ``Fix deprecated import in Oracle example (#31166)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
```

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/README.rst` & `apache-airflow-providers-oracle-3.7.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
@@ -115,14 +115,17 @@
 * ``Fix deprecated import in Oracle example (#31166)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
```

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/example_oracle.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/example_dags/example_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/get_provider_info.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/oracle.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/oracle.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/operators/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache-airflow-providers-oracle-3.7.0rc2/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO` & `apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
@@ -150,14 +150,17 @@
 * ``Fix deprecated import in Oracle example (#31166)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
```

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt` & `apache-airflow-providers-oracle-3.7.0rc2/apache_airflow_providers_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/pyproject.toml` & `apache-airflow-providers-oracle-3.7.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/setup.cfg` & `apache-airflow-providers-oracle-3.7.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.oracle.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.oracle
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-oracle-3.7.0rc1/setup.py` & `apache-airflow-providers-oracle-3.7.0rc2/setup.py`

 * *Files identical despite different names*

