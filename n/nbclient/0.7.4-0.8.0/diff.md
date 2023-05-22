# Comparing `tmp/nbclient-0.7.4.tar.gz` & `tmp/nbclient-0.8.0.tar.gz`

## Comparing `nbclient-0.7.4.tar` & `nbclient-0.8.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/__init__.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/_version.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/cli.py
--rw-r--r--   0        0        0    49505 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/client.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/exceptions.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/jsonutil.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/output_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/py.typed
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/__init__.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/base.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/conftest.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0    71162 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/test_client.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/test_util.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Autokill.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Check History in Memory.ipynb
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Clear Output.ipynb
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Disable Stdin.ipynb
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Empty Cell.ipynb
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Error.ipynb
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Factorials.ipynb
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Inline Image.ipynb
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Interrupt.ipynb
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/JupyterWidgets.ipynb
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Other Comms.ipynb
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Output.ipynb
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Parallel Execute A.ipynb
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Parallel Execute B.ipynb
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/SVG.ipynb
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Exceptions.ipynb
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Execution with Cell Tag.ipynb
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Sleep1s.ipynb
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Unicode.ipynb
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/UnicodePy3.ipynb
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/python.png
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/update-display-id.ipynb
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 nbclient-0.7.4/.gitignore
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nbclient-0.7.4/LICENSE
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 nbclient-0.7.4/README.md
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 nbclient-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 nbclient-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/__init__.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/_version.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/cli.py
+-rw-r--r--   0        0        0    49505 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/client.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/exceptions.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/jsonutil.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/output_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/py.typed
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/__init__.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/base.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/conftest.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0    71162 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/test_client.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/test_util.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Autokill.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Check History in Memory.ipynb
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Clear Output.ipynb
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Disable Stdin.ipynb
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Empty Cell.ipynb
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Error.ipynb
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Factorials.ipynb
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Inline Image.ipynb
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Interrupt.ipynb
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/JupyterWidgets.ipynb
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Other Comms.ipynb
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Output.ipynb
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Parallel Execute A.ipynb
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Parallel Execute B.ipynb
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/SVG.ipynb
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Skip Exceptions.ipynb
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Skip Execution with Cell Tag.ipynb
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Sleep1s.ipynb
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/Unicode.ipynb
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/UnicodePy3.ipynb
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/python.png
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 nbclient-0.8.0/nbclient/tests/files/update-display-id.ipynb
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 nbclient-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nbclient-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 nbclient-0.8.0/README.md
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 nbclient-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 nbclient-0.8.0/PKG-INFO
```

### Comparing `nbclient-0.7.4/nbclient/cli.py` & `nbclient-0.8.0/nbclient/cli.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/client.py` & `nbclient-0.8.0/nbclient/client.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/exceptions.py` & `nbclient-0.8.0/nbclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/jsonutil.py` & `nbclient-0.8.0/nbclient/jsonutil.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/output_widget.py` & `nbclient-0.8.0/nbclient/output_widget.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/base.py` & `nbclient-0.8.0/nbclient/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/fake_kernelmanager.py` & `nbclient-0.8.0/nbclient/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/test_client.py` & `nbclient-0.8.0/nbclient/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/test_util.py` & `nbclient-0.8.0/nbclient/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Autokill.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Autokill.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Clear Output.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Clear Output.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Empty Cell.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Empty Cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Error.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Error.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Factorials.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Factorials.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Inline Image.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Inline Image.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Interrupt.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Interrupt.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/JupyterWidgets.ipynb` & `nbclient-0.8.0/nbclient/tests/files/JupyterWidgets.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Other Comms.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Other Comms.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'cells'": '{0: {\'source\': [\'from comm import create_comm\']}, 1: {\'source\': ["comm = '*

 * *            'create_comm(\'this-comm-tests-a-missing-handler\', data={\'id\': \'foo\'})"]}}'}*

```diff
@@ -7,29 +7,29 @@
                 "ExecuteTime": {
                     "end_time": "2020-05-29T11:16:26.365338Z",
                     "start_time": "2020-05-29T11:16:26.362047Z"
                 }
             },
             "outputs": [],
             "source": [
-                "from ipykernel.comm import Comm"
+                "from comm import create_comm"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
                     "end_time": "2020-05-29T11:16:26.377700Z",
                     "start_time": "2020-05-29T11:16:26.371603Z"
                 }
             },
             "outputs": [],
             "source": [
-                "comm = Comm('this-comm-tests-a-missing-handler', data={'id': 'foo'})"
+                "comm = create_comm('this-comm-tests-a-missing-handler', data={'id': 'foo'})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
```

### Comparing `nbclient-0.7.4/nbclient/tests/files/Output.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Output.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Parallel Execute A.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Parallel Execute A.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Parallel Execute B.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Parallel Execute B.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/SVG.ipynb` & `nbclient-0.8.0/nbclient/tests/files/SVG.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Skip Exceptions.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Skip Exceptions.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/Sleep1s.ipynb` & `nbclient-0.8.0/nbclient/tests/files/Sleep1s.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/python.png` & `nbclient-0.8.0/nbclient/tests/files/python.png`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/nbclient/tests/files/update-display-id.ipynb` & `nbclient-0.8.0/nbclient/tests/files/update-display-id.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/.gitignore` & `nbclient-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/LICENSE` & `nbclient-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/README.md` & `nbclient-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.4/pyproject.toml` & `nbclient-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 name = "nbclient"
 dynamic = [
     "version",
 ]
 description = "A client library for executing notebooks. Formerly nbconvert's ExecutePreprocessor."
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7.0"
+requires-python = ">=3.8.0"
 authors = [
     { name = "Jupyter Development Team", email = "jupyter@googlegroups.com" },
 ]
 keywords = [
     "executor",
     "jupyter",
     "notebook",
@@ -25,31 +25,30 @@
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jupyter_client>=6.1.12",
     "jupyter_core>=4.12,!=5.0.*",
     "nbformat>=5.1",
-    "traitlets>=5.3",
+    "traitlets>=5.4",
 ]
 
 [project.optional-dependencies]
 test = [
     "flaky",
-    "ipykernel",
+    "ipykernel>=6.19.3",
     "ipython",
     "ipywidgets",
     "nbconvert>=7.0.0",
     "pytest-asyncio",
     "pytest-cov>=4.0",
     "pytest>=7.0",
     "testpath",
@@ -112,15 +111,15 @@
 test = "mypy --install-types --non-interactive {args:nbclient}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black[jupyter]==22.10.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.254"
+  "ruff==0.0.263"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
```

### Comparing `nbclient-0.7.4/PKG-INFO` & `nbclient-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbclient
-Version: 0.7.4
+Version: 0.8.0
 Summary: A client library for executing notebooks. Formerly nbconvert's ExecutePreprocessor.
 Project-URL: Documentation, https://nbclient.readthedocs.io
 Project-URL: Funding, https://numfocus.org/
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Source, https://github.com/jupyter/nbclient
 Project-URL: Tracker, https://github.com/jupyter/nbclient/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
@@ -42,38 +42,37 @@
 Keywords: executor,jupyter,notebook,pipeline
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Requires-Dist: jupyter-client>=6.1.12
 Requires-Dist: jupyter-core!=5.0.*,>=4.12
 Requires-Dist: nbformat>=5.1
-Requires-Dist: traitlets>=5.3
+Requires-Dist: traitlets>=5.4
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodoc-traits; extra == 'docs'
 Requires-Dist: mock; extra == 'docs'
 Requires-Dist: moto; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: nbclient[test]; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx>=1.7; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: flaky; extra == 'test'
-Requires-Dist: ipykernel; extra == 'test'
+Requires-Dist: ipykernel>=6.19.3; extra == 'test'
 Requires-Dist: ipython; extra == 'test'
 Requires-Dist: ipywidgets; extra == 'test'
 Requires-Dist: nbconvert>=7.0.0; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov>=4.0; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: testpath; extra == 'test'
```

