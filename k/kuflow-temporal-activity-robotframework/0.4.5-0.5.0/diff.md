# Comparing `tmp/kuflow_temporal_activity_robotframework-0.4.5.tar.gz` & `tmp/kuflow_temporal_activity_robotframework-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_robotframework-0.4.5.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_robotframework-0.5.0.tar", max compression
```

## Comparing `kuflow_temporal_activity_robotframework-0.4.5.tar` & `kuflow_temporal_activity_robotframework-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      921 2023-05-15 11:39:40.707021 kuflow_temporal_activity_robotframework-0.4.5/README.md
--rw-r--r--   0        0        0        6 2023-05-15 11:39:40.707021 kuflow_temporal_activity_robotframework-0.4.5/VERSION
--rw-r--r--   0        0        0     1249 2023-05-15 11:39:40.707021 kuflow_temporal_activity_robotframework-0.4.5/kuflow_temporal_activity_robotframework/__init__.py
--rw-r--r--   0        0        0     3964 2023-05-15 11:39:40.707021 kuflow_temporal_activity_robotframework-0.4.5/kuflow_temporal_activity_robotframework/robot_framework_activities.py
--rw-r--r--   0        0        0      905 2023-05-15 11:41:12.579024 kuflow_temporal_activity_robotframework-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.4.5/setup.py
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      921 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/README.md
+-rw-r--r--   0        0        0        6 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/VERSION
+-rw-r--r--   0        0        0     1249 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/__init__.py
+-rw-r--r--   0        0        0     5329 2023-05-22 09:05:44.095853 kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py
+-rw-r--r--   0        0        0     1104 2023-05-22 09:07:40.150431 kuflow_temporal_activity_robotframework-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.5.0/setup.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 kuflow_temporal_activity_robotframework-0.5.0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/README.md` & `kuflow_temporal_activity_robotframework-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/kuflow_temporal_activity_robotframework/__init__.py` & `kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .robot_framework_activities import RobotFrameworkActivities
 
 __all__ = ["RobotFrameworkActivities"]
 
-__version__ = "0.4.5"
+__version__ = "0.5.0"
```

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/kuflow_temporal_activity_robotframework/robot_framework_activities.py` & `kuflow_temporal_activity_robotframework-0.5.0/kuflow_temporal_activity_robotframework/robot_framework_activities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,34 @@
+# coding=utf-8
+#
+# MIT License
+#
+# Copyright (c) 2022 KuFlow
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import Callable, List, Optional, Sequence
 import robot
 
 from temporalio import activity
 from temporalio.exceptions import ApplicationError
 from kuflow_temporal_common.activity_utils import auto_heartbeater
 
 from kuflow_temporal_common.exceptions import KuFlowFailureType
@@ -17,56 +42,64 @@
     return {}
 
 
 @dataclass
 class ExecuteRobotRequest:
     """Data class for execute robot activity.
 
-    :param tests: Paths to test case files/directories to be executed similarly
-        as when running the ``robot`` command on the command line.
-    :param variables: Options to configure and control execution.
-        Take precedence over "variable" key in :param options. Values are merged.
-        Take precedence over default_variables in :class:`RobotFrameworkActivities`.
-        Values are merged.
-        Please see :func:`robot.run.run` docstring to more info
-    :param options: Options to configure and control execution. Please see
-        Take precedence over default_options in :class:`RobotFrameworkActivities`
-        Values are merged.
-        Please see :func:`robot.run.run` docstring to more info
+    Attributes:
+        tests: Paths to test case files/directories to be executed similarly
+            as when running the ``robot`` command on the command line.
+        variables: Options to configure and control execution.
+            Take precedence over "variable" key in :param options. Values are merged.
+            Take precedence over default_variables in :class:`RobotFrameworkActivities`.
+            Values are merged.
+            Please see :func:`robot.run.run` docstring to more info
+        options: Options to configure and control execution. Please see
+            Take precedence over default_options in :class:`RobotFrameworkActivities`
+            Values are merged.
+            Please see :func:`robot.run.run` docstring to more info
     """
 
     tests: str
 
     variables: List[str] = field(default_factory=_default_variables)
 
     options: dict = field(default_factory=_default_additional_options)
 
 
 class RobotFrameworkActivities:
     """
     Set of Temporal.io activities to manage Robot Framework activities
 
-       Args:
+    Arguments:
         default_variables (Optional[List[str]]): Variables to pass to the robot.
             Format: ["<key>:<value>"]. Example: ["key1:value1", "key2:000"]
             It is equivalent to setting the variables on the command line of 'robot'.
             Important. Take precedence over "variable" key in :arg default_options. Values are merged.
             We recommend avoiding the "variable" key in default_options and using the
             default_variables field for it.
             These variables can be overridden in activity invocations.
         default_options (Optional[dict]): Options to configure and control execution.
             These options can be overridden in activity invocations.
             Please see :func:`robot.run.run` docstring to more info.
     """
 
+    activities: Sequence[Callable]
+
     def __init__(
         self,
-        default_variables: Optional[List[str]] = [],
-        default_options: Optional[dict] = {},
+        default_variables: Optional[List[str]] = None,
+        default_options: Optional[dict] = None,
     ) -> None:
+        if default_options is None:
+            default_options = {}
+        if default_variables is None:
+            default_variables = []
+
         merge_variables = self._merge_variables(default_options.get("variable"), default_variables)
         options = {**default_options, **{"variable": merge_variables}}
 
         self._default_options = options
         self.activities = [self.execute_robot]
 
     @activity.defn
@@ -80,20 +113,23 @@
         options = {**self._default_options, **{"variable": merge_variables_in_default}}
 
         # Run
         robot_code = robot.run(request.tests, **options)
 
         if robot_code != 0:
             raise ApplicationError(
-                message=f"Robot finised with undesired status value of ${robot_code}",
+                f"Robot finished with undesired status value of ${robot_code}",
                 non_retryable=True,
                 type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
             )
 
-    def _merge_variables(self, variables=[], variables_overwrite=[]):
+    def _merge_variables(self, variables: List = None, variables_overwrite: List = None):
         # First variables defined take priority
-        variables = [] if variables is None else variables
-        variables_overwrite = [] if variables_overwrite is None else variables_overwrite
+        if variables_overwrite is None:
+            variables_overwrite = []
+        if variables is None:
+            variables = []
+
         merge_variables = variables_overwrite + variables
         unique_variables = list({s.split(":")[0]: s for s in merge_variables}.values())
 
         return unique_variables
```

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/pyproject.toml` & `kuflow_temporal_activity_robotframework-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-robotframework"
-version = "0.4.5"
+version = "0.5.0"
 description = "KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,20 +13,27 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.4.5"
+kuflow-temporal-common = "^0.5.0"
 robotframework = "^5.0.1"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "0.910"
-flake8 = "4.0.1"
-black = "^23.1.0"
-pytest = "^7.2.1"
+mypy = "^1.3.0"
+ipython = "^7.34.0"
+flake8 = "^5.0.4"
+black = "^23.3.0"
+pytest = "^7.3.1"
 robotframework-tidy = "^3.3.3"
 
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+python_files= "test_*.py"
+
 [tool.black]
 line-length = 120
 target-version = ["py38", "py39"]
```

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/setup.py` & `kuflow_temporal_activity_robotframework-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_robotframework']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.4.5,<0.5.0', 'robotframework>=5.0.1,<6.0.0']
+['kuflow-temporal-common>=0.5.0,<0.6.0', 'robotframework>=5.0.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-robotframework',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': 'KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)\n\n# KuFlow Temporal Activities Robot Framework\n\nTemporal.io activities to execute Robot Framework tasks, aka RPA\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_robotframework-0.4.5/PKG-INFO` & `kuflow_temporal_activity_robotframework-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-robotframework
-Version: 0.4.5
+Version: 0.5.0
 Summary: KuFlow SDK :: Temporal.io activities to execute Robot Frameworks tasks
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
-Requires-Dist: kuflow-temporal-common (>=0.4.5,<0.5.0)
+Requires-Dist: kuflow-temporal-common (>=0.5.0,<0.6.0)
 Requires-Dist: robotframework (>=5.0.1,<6.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-robotframework)
```

