# Comparing `tmp/pytest-reportlog-0.3.0.tar.gz` & `tmp/pytest-reportlog-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportlog-0.3.0.tar", last modified: Wed Apr 26 21:45:12 2023, max compression
+gzip compressed data, was "pytest-reportlog-0.4.0.tar", last modified: Mon May 22 14:35:22 2023, max compression
```

## Comparing `pytest-reportlog-0.3.0.tar` & `pytest-reportlog-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.205610 pytest-reportlog-0.3.0/src/pytest_reportlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/src/pytest_reportlog/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 21:45:12.000000 pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:45:12.209610 pytest-reportlog-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/tests/test_reportlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-26 21:44:44.000000 pytest-reportlog-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.747183 pytest-reportlog-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.739183 pytest-reportlog-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.743183 pytest-reportlog-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-22 14:35:22.747183 pytest-reportlog-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:35:22.747183 pytest-reportlog-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.739183 pytest-reportlog-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.743183 pytest-reportlog-0.4.0/src/pytest_reportlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/src/pytest_reportlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/src/pytest_reportlog/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.747183 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 14:35:22.000000 pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:35:22.747183 pytest-reportlog-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/tests/test_reportlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 14:35:01.000000 pytest-reportlog-0.4.0/tox.ini
```

### Comparing `pytest-reportlog-0.3.0/.github/workflows/test.yml` & `pytest-reportlog-0.4.0/.github/workflows/test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 name: test
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+      - master
+      - "test-me-*"
+
+  pull_request:
+    branches:
+      - "*"
 
 # Cancel running jobs for the same workflow and branch.
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
+  package:
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Build and Check Package
+      uses: hynek/build-and-inspect-python-package@v1.5
+
   test:
+    needs: [package]
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: false
       matrix:
         python: ["3.7", "3.8", "3.9", "3.10", "3.11"]
@@ -27,25 +43,28 @@
           - python: "3.10"
             tox_env: "py310"
           - python: "3.11"
             tox_env: "py311"
 
     steps:
     - uses: actions/checkout@v3
+
+    - name: Download Package
+      uses: actions/download-artifact@v3
+      with:
+        name: Packages
+        path: dist
+
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
+
     - name: Install tox
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade virtualenv tox
+        pip install tox
+
     - name: Test
+      shell: bash
       run: |
-        tox -e ${{ matrix.tox_env }}
-
-  check-package:
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v3
-    - name: Build and Check Package
-      uses: hynek/build-and-inspect-python-package@v1.5
+        tox run -e ${{ matrix.tox_env }} --installpkg `find dist/*.tar.gz`
```

### Comparing `pytest-reportlog-0.3.0/.gitignore` & `pytest-reportlog-0.4.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -100,7 +100,10 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 src/pytest_reportlog/_version.py
+
+# PyCharm
+.idea/
```

### Comparing `pytest-reportlog-0.3.0/.pre-commit-config.yaml` & `pytest-reportlog-0.4.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,20 @@
       - id: black
         args: [--safe, --quiet]
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
+
+  -  repo: https://github.com/pre-commit/mirrors-mypy
+     rev: 'v1.3.0'
+     hooks:
+     -   id: mypy
+
   - repo: local
     hooks:
       - id: rst
         name: rst
         entry: rst-lint --encoding utf-8
         files: ^(CHANGELOG.rst|README.rst|HOWTORELEASE.rst)$
         language: python
```

### Comparing `pytest-reportlog-0.3.0/LICENSE` & `pytest-reportlog-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.3.0/PKG-INFO` & `pytest-reportlog-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportlog
-Version: 0.3.0
+Version: 0.4.0
 Summary: Replacement for the --resultlog option, focused in simplicity and extensibility
 Home-page: https://github.com/pytest-dev/pytest-reportlog
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest
 Platform: any
@@ -55,25 +55,30 @@
     If you use ``--resultlog``, please try out ``--report-log`` and provide feedback.
 
 Usage
 =====
 
 Install ``pytest-reportlog`` as a test requirement in your test environment.
 
-The ``--report-log=FILE`` option writes *report logs* into a file as the test session executes.
+The ``--report-log=FILE`` option writes a file in `JSON lines <https://jsonlines.org/>`__ format as the test session executes.
 
 Each line of the report log contains a self contained JSON object corresponding to a testing event,
 such as a collection or a test result report. The file is guaranteed to be flushed after writing
 each line, so systems can read and process events in real-time.
 
 Each JSON object contains a special key ``$report_type``, which contains a unique identifier for
 that kind of report object. For future compatibility, consumers of the file should ignore reports
 they don't recognize, as well as ignore unknown properties/keys in JSON objects that they do know,
 as future pytest versions might enrich the objects with more properties/keys.
 
+Compression
+===========
+
+Common compression suffixes like `.gz`, `.bz2` and `.xz` will automatically use the requested compression format.
+The implementations from the python stdlib are used and must be enabled in the python builds.
 
 Example
 -------
 
 Consider this file:
 
 .. code-block:: python
@@ -87,32 +92,32 @@
 
     def test_fail():
         assert 4 + 4 == 1
 
 
 ::
 
-    $ pytest test_report_example.py -q --report-log=log.json
+    $ pytest test_report_example.py -q --report-log=log.jsonl
     .F                                                                   [100%]
     ================================= FAILURES =================================
     ________________________________ test_fail _________________________________
 
         def test_fail():
     >       assert 4 + 4 == 1
     E       assert (4 + 4) == 1
 
     test_report_example.py:8: AssertionError
-    ------------------- generated report log file: log.json --------------------
+    ------------------- generated report log file: log.jsonl --------------------
     1 failed, 1 passed in 0.12s
 
-The generated ``log.json`` will contain a JSON object per line:
+The generated ``log.jsonl`` will contain a JSON object per line:
 
 ::
 
-    $ cat log.json
+    $ cat log.jsonl
     {"pytest_version": "5.2.2", "$report_type": "SessionStart"}
     {"nodeid": "", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "call", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "teardown", "user_properties": [], "sections": [], "duration": 0.00099945068359375, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_fail", "location": ["test_report_example.py", 4, "test_fail"], "keywords": {"test_fail": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
@@ -136,15 +141,7 @@
 
 This information will be recorded in the report JSON objects under the ``user_properties`` key as follows::
 
     ..., "user_properties": [["price", 12.34], ["fruit", "banana"]], ...
 
 Note that this nested list construct is just the JSON representation
 of a list of tuples (name-value pairs).
-
-
-License
-=======
-
-Distributed under the terms of the `MIT`_ license.
-
-.. _MIT: https://github.com/pytest-dev/pytest-mock/blob/master/LICENSE
```

### Comparing `pytest-reportlog-0.3.0/README.rst` & `pytest-reportlog-0.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,30 @@
     If you use ``--resultlog``, please try out ``--report-log`` and provide feedback.
 
 Usage
 =====
 
 Install ``pytest-reportlog`` as a test requirement in your test environment.
 
-The ``--report-log=FILE`` option writes *report logs* into a file as the test session executes.
+The ``--report-log=FILE`` option writes a file in `JSON lines <https://jsonlines.org/>`__ format as the test session executes.
 
 Each line of the report log contains a self contained JSON object corresponding to a testing event,
 such as a collection or a test result report. The file is guaranteed to be flushed after writing
 each line, so systems can read and process events in real-time.
 
 Each JSON object contains a special key ``$report_type``, which contains a unique identifier for
 that kind of report object. For future compatibility, consumers of the file should ignore reports
 they don't recognize, as well as ignore unknown properties/keys in JSON objects that they do know,
 as future pytest versions might enrich the objects with more properties/keys.
 
+Compression
+===========
+
+Common compression suffixes like `.gz`, `.bz2` and `.xz` will automatically use the requested compression format.
+The implementations from the python stdlib are used and must be enabled in the python builds.
 
 Example
 -------
 
 Consider this file:
 
 .. code-block:: python
@@ -60,32 +65,32 @@
 
     def test_fail():
         assert 4 + 4 == 1
 
 
 ::
 
-    $ pytest test_report_example.py -q --report-log=log.json
+    $ pytest test_report_example.py -q --report-log=log.jsonl
     .F                                                                   [100%]
     ================================= FAILURES =================================
     ________________________________ test_fail _________________________________
 
         def test_fail():
     >       assert 4 + 4 == 1
     E       assert (4 + 4) == 1
 
     test_report_example.py:8: AssertionError
-    ------------------- generated report log file: log.json --------------------
+    ------------------- generated report log file: log.jsonl --------------------
     1 failed, 1 passed in 0.12s
 
-The generated ``log.json`` will contain a JSON object per line:
+The generated ``log.jsonl`` will contain a JSON object per line:
 
 ::
 
-    $ cat log.json
+    $ cat log.jsonl
     {"pytest_version": "5.2.2", "$report_type": "SessionStart"}
     {"nodeid": "", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "call", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "teardown", "user_properties": [], "sections": [], "duration": 0.00099945068359375, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_fail", "location": ["test_report_example.py", 4, "test_fail"], "keywords": {"test_fail": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
@@ -109,15 +114,7 @@
 
 This information will be recorded in the report JSON objects under the ``user_properties`` key as follows::
 
     ..., "user_properties": [["price", 12.34], ["fruit", "banana"]], ...
 
 Note that this nested list construct is just the JSON representation
 of a list of tuples (name-value pairs).
-
-
-License
-=======
-
-Distributed under the terms of the `MIT`_ license.
-
-.. _MIT: https://github.com/pytest-dev/pytest-mock/blob/master/LICENSE
```

### Comparing `pytest-reportlog-0.3.0/setup.py` & `pytest-reportlog-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-reportlog-0.3.0/src/pytest_reportlog/plugin.py` & `pytest-reportlog-0.4.0/src/pytest_reportlog/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Dict, Any
+from typing import Dict, Any, TextIO
 
 from _pytest.pathlib import Path
 
 import pytest
 
 
 def pytest_addoption(parser):
@@ -11,14 +11,20 @@
     group.addoption(
         "--report-log",
         action="store",
         metavar="path",
         default=None,
         help="Path to line-based json objects of test session events.",
     )
+    group.addoption(
+        "--report-log-exclude-logs-on-passed-tests",
+        action="store_true",
+        default=False,
+        help="Don't capture logs for passing tests",
+    )
 
 
 def pytest_configure(config):
     report_log = config.option.report_log
     if report_log and not hasattr(config, "workerinput"):
         config._report_log_plugin = ReportLogPlugin(config, Path(report_log))
         config.pluginmanager.register(config._report_log_plugin)
@@ -27,21 +33,39 @@
 def pytest_unconfigure(config):
     report_log_plugin = getattr(config, "_report_log_plugin", None)
     if report_log_plugin:
         report_log_plugin.close()
         del config._report_log_plugin
 
 
+def _open_filtered_writer(log_path: Path) -> TextIO:
+    if log_path.suffix == ".gz":
+        import gzip
+
+        return gzip.open(log_path, "wt", encoding="UTF-8")
+    elif log_path.suffix == ".bz2":
+        import bz2
+
+        return bz2.open(log_path, "wt", encoding="UTF-8")
+    elif log_path.suffix == ".xz":
+        import lzma
+
+        return lzma.open(log_path, "wt", encoding="UTF-8")
+    else:
+        # line buffer for text mode to ease tail -f
+        return log_path.open("wt", buffering=1, encoding="UTF-8")
+
+
 class ReportLogPlugin:
     def __init__(self, config, log_path: Path):
         self._config = config
         self._log_path = log_path
 
         log_path.parent.mkdir(parents=True, exist_ok=True)
-        self._file = log_path.open("w", buffering=1, encoding="UTF-8")
+        self._file = _open_filtered_writer(log_path)
 
     def close(self):
         if self._file is not None:
             self._file.close()
             self._file = None
 
     def _write_json_data(self, data):
@@ -61,14 +85,29 @@
         data = {"exitstatus": exitstatus, "$report_type": "SessionFinish"}
         self._write_json_data(data)
 
     def pytest_runtest_logreport(self, report):
         data = self._config.hook.pytest_report_to_serializable(
             config=self._config, report=report
         )
+        if (
+            self._config.option.report_log_exclude_logs_on_passed_tests
+            and data.get("outcome", "") == "passed"
+        ):
+            data["sections"] = [
+                s
+                for s in data["sections"]
+                if s[0]
+                not in [
+                    "Captured log setup",
+                    "Captured log call",
+                    "Captured log teardown",
+                ]
+            ]
+
         self._write_json_data(data)
 
     def pytest_warning_recorded(self, warning_message, when, nodeid, location):
         data = {
             "category": (
                 warning_message.category.__name__ if warning_message.category else None
             ),
```

### Comparing `pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/PKG-INFO` & `pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportlog
-Version: 0.3.0
+Version: 0.4.0
 Summary: Replacement for the --resultlog option, focused in simplicity and extensibility
 Home-page: https://github.com/pytest-dev/pytest-reportlog
 Author: Bruno Oliveira
 Author-email: nicoddemus@gmail.com
 License: MIT
 Keywords: pytest
 Platform: any
@@ -55,25 +55,30 @@
     If you use ``--resultlog``, please try out ``--report-log`` and provide feedback.
 
 Usage
 =====
 
 Install ``pytest-reportlog`` as a test requirement in your test environment.
 
-The ``--report-log=FILE`` option writes *report logs* into a file as the test session executes.
+The ``--report-log=FILE`` option writes a file in `JSON lines <https://jsonlines.org/>`__ format as the test session executes.
 
 Each line of the report log contains a self contained JSON object corresponding to a testing event,
 such as a collection or a test result report. The file is guaranteed to be flushed after writing
 each line, so systems can read and process events in real-time.
 
 Each JSON object contains a special key ``$report_type``, which contains a unique identifier for
 that kind of report object. For future compatibility, consumers of the file should ignore reports
 they don't recognize, as well as ignore unknown properties/keys in JSON objects that they do know,
 as future pytest versions might enrich the objects with more properties/keys.
 
+Compression
+===========
+
+Common compression suffixes like `.gz`, `.bz2` and `.xz` will automatically use the requested compression format.
+The implementations from the python stdlib are used and must be enabled in the python builds.
 
 Example
 -------
 
 Consider this file:
 
 .. code-block:: python
@@ -87,32 +92,32 @@
 
     def test_fail():
         assert 4 + 4 == 1
 
 
 ::
 
-    $ pytest test_report_example.py -q --report-log=log.json
+    $ pytest test_report_example.py -q --report-log=log.jsonl
     .F                                                                   [100%]
     ================================= FAILURES =================================
     ________________________________ test_fail _________________________________
 
         def test_fail():
     >       assert 4 + 4 == 1
     E       assert (4 + 4) == 1
 
     test_report_example.py:8: AssertionError
-    ------------------- generated report log file: log.json --------------------
+    ------------------- generated report log file: log.jsonl --------------------
     1 failed, 1 passed in 0.12s
 
-The generated ``log.json`` will contain a JSON object per line:
+The generated ``log.jsonl`` will contain a JSON object per line:
 
 ::
 
-    $ cat log.json
+    $ cat log.jsonl
     {"pytest_version": "5.2.2", "$report_type": "SessionStart"}
     {"nodeid": "", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py", "outcome": "passed", "longrepr": null, "result": null, "sections": [], "$report_type": "CollectReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "call", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_ok", "location": ["test_report_example.py", 0, "test_ok"], "keywords": {"test_ok": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "teardown", "user_properties": [], "sections": [], "duration": 0.00099945068359375, "$report_type": "TestReport"}
     {"nodeid": "test_report_example.py::test_fail", "location": ["test_report_example.py", 4, "test_fail"], "keywords": {"test_fail": 1, "pytest-reportlog": 1, "test_report_example.py": 1}, "outcome": "passed", "longrepr": null, "when": "setup", "user_properties": [], "sections": [], "duration": 0.0, "$report_type": "TestReport"}
@@ -136,15 +141,7 @@
 
 This information will be recorded in the report JSON objects under the ``user_properties`` key as follows::
 
     ..., "user_properties": [["price", 12.34], ["fruit", "banana"]], ...
 
 Note that this nested list construct is just the JSON representation
 of a list of tuples (name-value pairs).
-
-
-License
-=======
-
-Distributed under the terms of the `MIT`_ license.
-
-.. _MIT: https://github.com/pytest-dev/pytest-mock/blob/master/LICENSE
```

### Comparing `pytest-reportlog-0.3.0/src/pytest_reportlog.egg-info/SOURCES.txt` & `pytest-reportlog-0.4.0/src/pytest_reportlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

