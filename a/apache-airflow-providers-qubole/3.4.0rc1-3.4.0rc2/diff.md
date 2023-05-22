# Comparing `tmp/apache-airflow-providers-qubole-3.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-qubole-3.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-qubole-3.4.0rc1.tar", last modified: Tue May 16 15:55:00 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-qubole-3.4.0rc2.tar", last modified: Fri May 19 17:53:18 2023, max compression
```

## Comparing `apache-airflow-providers-qubole-3.4.0rc1.tar` & `apache-airflow-providers-qubole-3.4.0rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:59.000000 apache-airflow-providers-qubole-3.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13823 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12269 2023-05-16 15:54:59.000000 apache-airflow-providers-qubole-3.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-16 15:54:59.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11208 2023-04-13 08:25:21.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/qubole.py
--rw-r--r--   0 root         (0) root         (0)     4084 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12541 2023-05-04 19:17:30.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/qubole.py
--rw-r--r--   0 root         (0) root         (0)     8381 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/sensors/qubole.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13823 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-qubole-3.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-16 15:55:00.000000 apache-airflow-providers-qubole-3.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-16 15:54:59.000000 apache-airflow-providers-qubole-3.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14040 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:20:35.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11208 2023-04-13 08:25:21.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12541 2023-05-04 19:17:30.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     8381 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/qubole.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14040 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-qubole-3.4.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/setup.py
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/LICENSE` & `apache-airflow-providers-qubole-3.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/MANIFEST.in` & `apache-airflow-providers-qubole-3.4.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/PKG-INFO` & `apache-airflow-providers-qubole-3.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
@@ -148,14 +148,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/README.rst` & `apache-airflow-providers-qubole-3.4.0rc2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
@@ -114,14 +114,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/get_provider_info.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/__init__.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/qubole.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/hooks/qubole_check.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/__init__.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/qubole.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/operators/qubole_check.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/sensors/__init__.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/airflow/providers/qubole/sensors/qubole.py` & `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO` & `apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
@@ -148,14 +148,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt` & `apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/pyproject.toml` & `apache-airflow-providers-qubole-3.4.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/setup.cfg` & `apache-airflow-providers-qubole-3.4.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.qubole.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.qubole
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc1/setup.py` & `apache-airflow-providers-qubole-3.4.0rc2/setup.py`

 * *Files identical despite different names*

