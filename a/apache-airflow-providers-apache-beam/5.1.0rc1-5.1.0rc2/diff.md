# Comparing `tmp/apache-airflow-providers-apache-beam-5.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-beam-5.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.1.0rc1.tar", last modified: Tue May 16 15:52:53 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.1.0rc2.tar", last modified: Fri May 19 17:51:30 2023, max compression
```

## Comparing `apache-airflow-providers-apache-beam-5.1.0rc1.tar` & `apache-airflow-providers-apache-beam-5.1.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15241 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/
--rw-r--r--   0 root         (0) root         (0)     1394 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14199 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32492 2023-04-21 10:05:41.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15241 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-beam-5.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1879 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:29.000000 apache-airflow-providers-apache-beam-5.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15513 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13948 2023-05-19 17:51:29.000000 apache-airflow-providers-apache-beam-5.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 11:59:33.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-19 17:51:29.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14199 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/hooks/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-04-21 10:05:41.000000 apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/operators/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15513 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-beam-5.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-05-19 17:51:30.000000 apache-airflow-providers-apache-beam-5.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-05-19 17:51:28.000000 apache-airflow-providers-apache-beam-5.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/LICENSE` & `apache-airflow-providers-apache-beam-5.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-beam-5.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.1.0rc1
+Version: 5.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.0rc1``
+Release: ``5.1.0rc2``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
@@ -81,15 +81,15 @@
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
-``apache-beam``     ``>=2.33.0``
+``apache-beam``     ``>=2.47.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -140,18 +140,22 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
+* ``Update SDKs for google provider package (#30067)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/README.rst` & `apache-airflow-providers-apache-beam-5.1.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.0rc1``
+Release: ``5.1.0rc2``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
@@ -47,15 +47,15 @@
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
-``apache-beam``     ``>=2.33.0``
+``apache-beam``     ``>=2.47.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -106,18 +106,22 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
+* ``Update SDKs for google provider package (#30067)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/__init__.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/__init__.py`

 * *Files 11% similar despite different names*

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
+__version__ = "5.1.0"
 
-version = "5.1.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-apache-beam:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-apache-beam:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/get_provider_info.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "3.1.0",
             "3.0.1",
             "3.0.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.4.0", "apache-beam>=2.33.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-beam>=2.47.0"],
         "integrations": [
             {
                 "integration-name": "Apache Beam",
                 "external-doc-url": "https://beam.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-beam/operators.rst"],
                 "tags": ["apache"],
             }
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/__init__.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/beam.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/hooks/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/__init__.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/beam.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/airflow/providers/apache/beam/operators/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.1.0rc1
+Version: 5.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.0rc1``
+Release: ``5.1.0rc2``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
@@ -81,15 +81,15 @@
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
-``apache-beam``     ``>=2.33.0``
+``apache-beam``     ``>=2.47.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -140,18 +140,22 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
+* ``Update SDKs for google provider package (#30067)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-beam-5.1.0rc2/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/pyproject.toml` & `apache-airflow-providers-apache-beam-5.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/setup.cfg` & `apache-airflow-providers-apache-beam-5.1.0rc2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow>=2.4.0.dev0
-	apache-beam>=2.33.0
+	apache-beam>=2.47.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.beam.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.beam
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-beam-5.1.0rc1/setup.py` & `apache-airflow-providers-apache-beam-5.1.0rc2/setup.py`

 * *Files identical despite different names*

