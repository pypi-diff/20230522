# Comparing `tmp/mojo_waiting-1.0.1.tar.gz` & `tmp/mojo_waiting-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_waiting-1.0.1.tar", max compression
+gzip compressed data, was "mojo_waiting-1.0.2.tar", max compression
```

## Comparing `mojo_waiting-1.0.1.tar` & `mojo_waiting-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1083 2023-03-17 03:56:33.147303 mojo_waiting-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4304 2023-04-29 15:22:19.117740 mojo_waiting-1.0.1/README.rst
--rw-r--r--   0        0        0      669 2023-04-29 15:37:19.904649 mojo_waiting-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-17 04:03:03.850169 mojo_waiting-1.0.1/source/packages/mojo/waiting/__init__.py
--rw-r--r--   0        0        0      779 2023-03-17 03:56:33.151303 mojo_waiting-1.0.1/source/packages/mojo/waiting/constants.py
--rw-r--r--   0        0        0     3080 2023-03-17 04:24:58.948898 mojo_waiting-1.0.1/source/packages/mojo/waiting/waitfunction.py
--rw-r--r--   0        0        0    11582 2023-03-17 04:29:41.595852 mojo_waiting-1.0.1/source/packages/mojo/waiting/waitmodel.py
--rw-r--r--   0        0        0     5000 1970-01-01 00:00:00.000000 mojo_waiting-1.0.1/setup.py
--rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 mojo_waiting-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-17 03:56:33.147303 mojo_waiting-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4441 2023-05-20 15:42:40.989830 mojo_waiting-1.0.2/README.rst
+-rw-r--r--   0        0        0      816 2023-05-21 03:46:53.383403 mojo_waiting-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-17 04:03:03.850169 mojo_waiting-1.0.2/source/packages/mojo/waiting/__init__.py
+-rw-r--r--   0        0        0      779 2023-03-17 03:56:33.151303 mojo_waiting-1.0.2/source/packages/mojo/waiting/constants.py
+-rw-r--r--   0        0        0     3080 2023-03-17 04:24:58.948898 mojo_waiting-1.0.2/source/packages/mojo/waiting/waitfunction.py
+-rw-r--r--   0        0        0    11582 2023-03-17 04:29:41.595852 mojo_waiting-1.0.2/source/packages/mojo/waiting/waitmodel.py
+-rw-r--r--   0        0        0     5190 1970-01-01 00:00:00.000000 mojo_waiting-1.0.2/setup.py
+-rw-r--r--   0        0        0     5245 1970-01-01 00:00:00.000000 mojo_waiting-1.0.2/PKG-INFO
```

### Comparing `mojo_waiting-1.0.1/LICENSE.txt` & `mojo_waiting-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.0.1/README.rst` & `mojo_waiting-1.0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -83,8 +83,14 @@
         """
         ...
 
 The `wait_for_it` function must be passed a method that follows the `WaitCallback` protocol.  The function
 can have variable arguments and keyword arguements but the first parameter to the `WaitCallback` method
 must be a `WaitContext` object.
 
+==========
+References
+==========
+
+- `User Guide <userguide/userguide.rst>`_
+- `Coding Standards <userguide/10-00-coding-standards.rst>`_
```

### Comparing `mojo_waiting-1.0.1/pyproject.toml` & `mojo_waiting-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "mojo-waiting"
 description = "Automation Mojo Waiting Module"
-version = "1.0.1"
-authors = []
+version = "1.0.2"
+authors = [
+    "Myron Walker <myron.walker@gmail.com>"
+]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{ include="mojo", from = "source/packages" }]
 
+homepage = "http://automationmojo.com"
+repository = "https://github.com/automationmojo/mojo-waiting"
+
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
```

### Comparing `mojo_waiting-1.0.1/source/packages/mojo/waiting/constants.py` & `mojo_waiting-1.0.2/source/packages/mojo/waiting/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.0.1/source/packages/mojo/waiting/waitfunction.py` & `mojo_waiting-1.0.2/source/packages/mojo/waiting/waitfunction.py`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.0.1/source/packages/mojo/waiting/waitmodel.py` & `mojo_waiting-1.0.2/source/packages/mojo/waiting/waitmodel.py`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.0.1/setup.py` & `mojo_waiting-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 ['mojo', 'mojo.waiting']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-waiting',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Automation Mojo Waiting Module',
-    'long_description': '\n=============================================\nAutomation Mojo Waiting Module - mojo-waiting\n=============================================\n\nThis package provides support for enhanced context based waiting.  The waiting code\npatterns used are designed to present the best results in test stacktraces presented\nwhen a wait fails.  This makes the `mojo.waiting` module perfect for use with\ntest frameworks such as `pytest` and `testplus` that show code context in the error\nreport stack traces.\n\nAnother important aspect of the `mojo.waiting` module is that it uses `datetime`\ntimestamps and `timespan` for lengths of time so timeouts in error reporting are easier\nto interpret.\n\n.. code::\n\n    Traceback (most recent call last):\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 97, in test_basic_wait_for_it_timeout\n        future.result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 451, in result\n        return self.__get_result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 403, in __get_result\n        raise self._exception\n    File "/usr/lib/python3.10/concurrent/futures/thread.py", line 58, in run\n        result = self.fn(*self.args, **self.kwargs)\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 88, in wait_task\n        ctxwait.wait_for_it(wait_helper, interval=.5, timeout=2)\n    File "/home/myron/repos/mojo.waiting/source/packages/ctxwait/waiting.py", line 103, in wait_for_it\n        raise toerr\n    TimeoutError: Timeout waiting for \'wait_helper\':\n        timeout=2 start_time=2023-03-13 14:57:29.860302, end_time=2023-03-13 14:57:31.860302 now_time=2023-03-13 14:57:31.863681 time_diff=0:00:02.003379\n\n\nThe following is an example of how the `mojo.waiting` module is used.\n\n.. code:: python\n\n    from ctxwait import WaitContext, wait_for_it\n\n    def some_wait_helper(wctx: WaitContext):\n        finished = False\n\n        // TODO: Check if something is finished, the code and variables used\n        //       here will show up in any tracebacks from pytest or testplus\n        //       because the timeout is being raised in the appropriate scope.\n\n        if not finished and wctx.final_attempt:\n            whatfor = "Test timeout"\n            toerr = wctx.create_timeout(whatfor)\n            raise toerr\n\n        return finished\n\n    wait_for_it(some_wait_helper)\n\n\nThe `wait_for_it` method has many different parameters that can be used to override the\nbehavior of the wait loop.\n\n.. code:: python\n\n    def wait_for_it(looper: WaitCallback, *largs, what_for: Optional[str]=None, delay: float=DEFAULT_WAIT_DELAY,\n                interval: float=DEFAULT_WAIT_INTERVAL, timeout: float=DEFAULT_WAIT_TIMEOUT,\n                lkwargs: Dict[Any, Any]={}, wctx: Optional[WaitContext]=None):\n        """\n            Provides for convenient mechanism to wait for criteria to be met before proceeding.\n\n            :param looper: A callback method that is repeatedly called while it returns `False` up-to\n                        the end of a timeout period, and that will return `True` if a waited on\n                        condition is met prior to a timeout condition being met.\n            :param largs: Arguements to pass to the looper callback function.\n            :param what_for: A breif description of what is being waited for.\n            :param delay: An initial time delay to consume before beginning the waiting process.\n            :param interval: A period of time to delay between rechecks of the wait conditon\n            :param timeout: The maximum period of time in seconds that should be waited before timing out.\n            :param lkwargs: Additional keyword arguments to pass to the looper function\n\n            :raises TimeoutError: A timeout error with details around the wait condition.\n\n            ..note: The \'delay\', \'interval\' and \'timeout\' parameters will be ignored if the \'wctx\' parameter\n                    is passed as the wctx (WaitContext) parameter includes these values with it.\n        """\n        ...\n\nThe `wait_for_it` function must be passed a method that follows the `WaitCallback` protocol.  The function\ncan have variable arguments and keyword arguements but the first parameter to the `WaitCallback` method\nmust be a `WaitContext` object.\n\n\n',
-    'author': 'None',
-    'author_email': 'None',
+    'long_description': '\n=============================================\nAutomation Mojo Waiting Module - mojo-waiting\n=============================================\n\nThis package provides support for enhanced context based waiting.  The waiting code\npatterns used are designed to present the best results in test stacktraces presented\nwhen a wait fails.  This makes the `mojo.waiting` module perfect for use with\ntest frameworks such as `pytest` and `testplus` that show code context in the error\nreport stack traces.\n\nAnother important aspect of the `mojo.waiting` module is that it uses `datetime`\ntimestamps and `timespan` for lengths of time so timeouts in error reporting are easier\nto interpret.\n\n.. code::\n\n    Traceback (most recent call last):\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 97, in test_basic_wait_for_it_timeout\n        future.result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 451, in result\n        return self.__get_result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 403, in __get_result\n        raise self._exception\n    File "/usr/lib/python3.10/concurrent/futures/thread.py", line 58, in run\n        result = self.fn(*self.args, **self.kwargs)\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 88, in wait_task\n        ctxwait.wait_for_it(wait_helper, interval=.5, timeout=2)\n    File "/home/myron/repos/mojo.waiting/source/packages/ctxwait/waiting.py", line 103, in wait_for_it\n        raise toerr\n    TimeoutError: Timeout waiting for \'wait_helper\':\n        timeout=2 start_time=2023-03-13 14:57:29.860302, end_time=2023-03-13 14:57:31.860302 now_time=2023-03-13 14:57:31.863681 time_diff=0:00:02.003379\n\n\nThe following is an example of how the `mojo.waiting` module is used.\n\n.. code:: python\n\n    from ctxwait import WaitContext, wait_for_it\n\n    def some_wait_helper(wctx: WaitContext):\n        finished = False\n\n        // TODO: Check if something is finished, the code and variables used\n        //       here will show up in any tracebacks from pytest or testplus\n        //       because the timeout is being raised in the appropriate scope.\n\n        if not finished and wctx.final_attempt:\n            whatfor = "Test timeout"\n            toerr = wctx.create_timeout(whatfor)\n            raise toerr\n\n        return finished\n\n    wait_for_it(some_wait_helper)\n\n\nThe `wait_for_it` method has many different parameters that can be used to override the\nbehavior of the wait loop.\n\n.. code:: python\n\n    def wait_for_it(looper: WaitCallback, *largs, what_for: Optional[str]=None, delay: float=DEFAULT_WAIT_DELAY,\n                interval: float=DEFAULT_WAIT_INTERVAL, timeout: float=DEFAULT_WAIT_TIMEOUT,\n                lkwargs: Dict[Any, Any]={}, wctx: Optional[WaitContext]=None):\n        """\n            Provides for convenient mechanism to wait for criteria to be met before proceeding.\n\n            :param looper: A callback method that is repeatedly called while it returns `False` up-to\n                        the end of a timeout period, and that will return `True` if a waited on\n                        condition is met prior to a timeout condition being met.\n            :param largs: Arguements to pass to the looper callback function.\n            :param what_for: A breif description of what is being waited for.\n            :param delay: An initial time delay to consume before beginning the waiting process.\n            :param interval: A period of time to delay between rechecks of the wait conditon\n            :param timeout: The maximum period of time in seconds that should be waited before timing out.\n            :param lkwargs: Additional keyword arguments to pass to the looper function\n\n            :raises TimeoutError: A timeout error with details around the wait condition.\n\n            ..note: The \'delay\', \'interval\' and \'timeout\' parameters will be ignored if the \'wctx\' parameter\n                    is passed as the wctx (WaitContext) parameter includes these values with it.\n        """\n        ...\n\nThe `wait_for_it` function must be passed a method that follows the `WaitCallback` protocol.  The function\ncan have variable arguments and keyword arguements but the first parameter to the `WaitCallback` method\nmust be a `WaitContext` object.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`_\n- `Coding Standards <userguide/10-00-coding-standards.rst>`_\n\n',
+    'author': 'Myron Walker',
+    'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'http://automationmojo.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `mojo_waiting-1.0.1/PKG-INFO` & `mojo_waiting-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: mojo-waiting
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automation Mojo Waiting Module
+Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
+Author: Myron Walker
+Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Project-URL: Repository, https://github.com/automationmojo/mojo-waiting
 Description-Content-Type: text/x-rst
 
 
 =============================================
 Automation Mojo Waiting Module - mojo-waiting
 =============================================
 
@@ -101,9 +105,15 @@
         """
         ...
 
 The `wait_for_it` function must be passed a method that follows the `WaitCallback` protocol.  The function
 can have variable arguments and keyword arguements but the first parameter to the `WaitCallback` method
 must be a `WaitContext` object.
 
+==========
+References
+==========
+
+- `User Guide <userguide/userguide.rst>`_
+- `Coding Standards <userguide/10-00-coding-standards.rst>`_
```

