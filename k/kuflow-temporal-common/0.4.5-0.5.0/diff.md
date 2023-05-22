# Comparing `tmp/kuflow_temporal_common-0.4.5.tar.gz` & `tmp/kuflow_temporal_common-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_common-0.4.5.tar", max compression
+gzip compressed data, was "kuflow_temporal_common-0.5.0.tar", max compression
```

## Comparing `kuflow_temporal_common-0.4.5.tar` & `kuflow_temporal_common-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      789 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/README.md
--rw-r--r--   0        0        0        6 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/VERSION
--rw-r--r--   0        0        0     1182 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/kuflow_temporal_common/__init__.py
--rw-r--r--   0        0        0     1346 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/kuflow_temporal_common/activity_utils.py
--rw-r--r--   0        0        0     4006 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/kuflow_temporal_common/authentication.py
--rw-r--r--   0        0        0      777 2023-05-15 11:39:40.707021 kuflow_temporal_common-0.4.5/kuflow_temporal_common/exceptions.py
--rw-r--r--   0        0        0      832 2023-05-15 11:41:10.590851 kuflow_temporal_common-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1562 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.5/setup.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      789 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/README.md
+-rw-r--r--   0        0        0        6 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/VERSION
+-rw-r--r--   0        0        0     1182 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/kuflow_temporal_common/__init__.py
+-rw-r--r--   0        0        0     2467 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/kuflow_temporal_common/activity_utils.py
+-rw-r--r--   0        0        0     5197 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/kuflow_temporal_common/authentication.py
+-rw-r--r--   0        0        0     1849 2023-05-22 09:05:44.095853 kuflow_temporal_common-0.5.0/kuflow_temporal_common/exceptions.py
+-rw-r--r--   0        0        0     1030 2023-05-22 09:07:37.338466 kuflow_temporal_common-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.5.0/setup.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 kuflow_temporal_common-0.5.0/PKG-INFO
```

### Comparing `kuflow_temporal_common-0.4.5/README.md` & `kuflow_temporal_common-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_common-0.4.5/kuflow_temporal_common/__init__.py` & `kuflow_temporal_common-0.5.0/kuflow_temporal_common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 # __all__ = ["KuFlowPayloadConverter"]
-__version__ = "0.4.5"
+__version__ = "0.5.0"
```

### Comparing `kuflow_temporal_common-0.4.5/setup.py` & `kuflow_temporal_common-0.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['kuflow_temporal_common']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['azure-core>=1.26.3,<2.0.0',
+['azure-core>=1.26.4,<2.0.0',
  'isodate>=0.6.1,<0.7.0',
- 'kuflow-rest>=0.4.5,<0.5.0',
- 'temporalio>=1.1.0,<2.0.0']
+ 'kuflow-rest>=0.5.0,<0.6.0',
+ 'temporalio==1.2.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-common',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': 'KuFlow utilities to use Temporal.io',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)\n\n# KuFlow Temporal Common\n\nTODO\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_common-0.4.5/PKG-INFO` & `kuflow_temporal_common-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-common
-Version: 0.4.5
+Version: 0.5.0
 Summary: KuFlow utilities to use Temporal.io
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: azure-core (>=1.26.3,<2.0.0)
+Requires-Dist: azure-core (>=1.26.4,<2.0.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
-Requires-Dist: kuflow-rest (>=0.4.5,<0.5.0)
-Requires-Dist: temporalio (>=1.1.0,<2.0.0)
+Requires-Dist: kuflow-rest (>=0.5.0,<0.6.0)
+Requires-Dist: temporalio (==1.2.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-common.svg)](https://pypi.org/project/kuflow-temporal-common)
```

