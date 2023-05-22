# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-hive-6.1.0rc1.tar", last modified: Tue May 16 15:53:04 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-hive-6.1.0rc2.tar", last modified: Fri May 19 17:51:41 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.0rc1.tar` & `apache-airflow-providers-apache-hive-6.1.0rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18741 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17026 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1394 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5601 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42315 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7383 2023-04-13 08:25:21.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7454 2023-04-30 16:55:11.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5671 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11742 2023-05-04 19:17:30.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5548 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18741 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-hive-6.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-16 15:53:02.000000 apache-airflow-providers-apache-hive-6.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    18958 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17243 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 12:01:05.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42315 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7383 2023-04-13 08:25:21.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2023-04-30 16:55:11.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5279 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11742 2023-05-04 19:17:30.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18958 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-hive-6.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hive-6.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/LICENSE` & `apache-airflow-providers-apache-hive-6.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.0rc1
+Version: 6.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
@@ -55,15 +55,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc1``
+Release: ``6.1.0rc2``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -165,14 +165,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/README.rst` & `apache-airflow-providers-apache-hive-6.1.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc1``
+Release: ``6.1.0rc2``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -125,14 +125,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/__init__.py`

 * *Files 10% similar despite different names*

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
+__version__ = "6.1.0"
 
-version = "6.1.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-apache-hive:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-apache-hive:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.0rc1
+Version: 6.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
@@ -55,15 +55,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc1``
+Release: ``6.1.0rc2``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -165,14 +165,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -60,10 +60,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc1/setup.py` & `apache-airflow-providers-apache-hive-6.1.0rc2/setup.py`

 * *Files identical despite different names*

