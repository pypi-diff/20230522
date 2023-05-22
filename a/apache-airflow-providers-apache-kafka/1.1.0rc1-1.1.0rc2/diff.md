# Comparing `tmp/apache-airflow-providers-apache-kafka-1.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-kafka-1.1.0rc1.tar", last modified: Tue May 16 15:53:07 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-kafka-1.1.0rc2.tar", last modified: Fri May 19 17:51:44 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1.tar` & `apache-airflow-providers-apache-kafka-1.1.0rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4937 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3392 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4937 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1897 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3609 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:01:36.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -122,12 +122,15 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/README.rst` & `apache-airflow-providers-apache-kafka-1.1.0rc2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -89,12 +89,15 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/__init__.py`

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
+__version__ = "1.1.0"
 
-version = "1.1.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-apache-kafka:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-apache-kafka:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -122,12 +122,15 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.0rc2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kafka.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.kafka
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc1/setup.py` & `apache-airflow-providers-apache-kafka-1.1.0rc2/setup.py`

 * *Files identical despite different names*

