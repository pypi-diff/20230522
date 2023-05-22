# Comparing `tmp/cg_pytest_reporter-2023.5.19.1522.tar.gz` & `tmp/cg_pytest_reporter-2023.5.22.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2023.5.19.1522.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2023.5.22.933.tar", max compression
```

## Comparing `cg_pytest_reporter-2023.5.19.1522.tar` & `cg_pytest_reporter-2023.5.22.933.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     5581 2023-05-19 13:12:41.748033 cg_pytest_reporter-2023.5.19.1522/README.md
--rw-r--r--   0        0        0      472 2023-05-19 13:14:08.291891 cg_pytest_reporter-2023.5.19.1522/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    19080 2023-05-19 12:02:18.735299 cg_pytest_reporter-2023.5.19.1522/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1831 2023-05-19 13:21:22.650887 cg_pytest_reporter-2023.5.19.1522/pyproject.toml
--rw-r--r--   0        0        0     6568 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.19.1522/setup.py
--rw-r--r--   0        0        0     6065 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.19.1522/PKG-INFO
+-rw-r--r--   0        0        0     6290 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/README.md
+-rw-r--r--   0        0        0      605 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    19123 2023-05-22 09:33:21.362713 cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1831 2023-05-22 09:33:41.047090 cg_pytest_reporter-2023.5.22.933/pyproject.toml
+-rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 cg_pytest_reporter-2023.5.22.933/PKG-INFO
```

### Comparing `cg_pytest_reporter-2023.5.19.1522/README.md` & `cg_pytest_reporter-2023.5.22.933/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 Use the `suite_weight` decorator to change the weight of an entire suite
 relative to other suites in your test run.
 
 ```python
 from cg_pytest_reporter import suite_weight
 
 
-@suite_weight('My Test Suite')
+@suite_weight(2)
 class TestSuite:
     def test_function():
         assert True
 ```
 
 Similar to the suite name, you can set the weight of the module-level suite with
 the `__cg_suite_weight__` variable.
@@ -231,7 +231,45 @@
     def test_failure():
         print('Hello World!', file=sys.stderr)
         assert False
 
     def test_ok():
         print('Hello World!', file=sys.stderr)
 ```
+
+#### `hide_output`
+
+A combined version of `hide_stdout` and `hide_stderr`.
+
+```python
+import sys
+
+from cg_pytest_reporter import hide_output
+
+
+# The string "Hello World!" that was printed to `stdout` or `stderr` will not be
+# sent along with the results.
+@hide_output
+def test_failure():
+    print('Hello World!')
+    print('Hello World!', file=sys.stderr)
+    assert False
+```
+
+This decorator can also be applied to a test class to hide the output of each
+test case within it.
+
+```python
+import sys
+
+from cg_pytest_reporter import hide_output
+
+
+@hide_output
+class TestClass:
+    def test_failure():
+        print('Hello World!', file=sys.stderr)
+        assert False
+
+    def test_ok():
+        print('Hello World!')
+```
```

### Comparing `cg_pytest_reporter-2023.5.19.1522/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2023.5.22.933/cg_pytest_reporter/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 class MessageTooLargeException(Exception):
     """This exception is raised when the required fields of the message combined
     are too large.
     """
 
 
-# The message size limit for SQS messages is 256KB, but we are also going to
-# send the structured output over websocket connections, where the limit is
-# 128KB. We set it a little bit less here than 128KB to leave enough space for
-# the wrapping message.
-MESSAGE_SIZE_LIMIT = 120_000
+# The message size limit for SQS messages is 256KB. We set it a little bit less
+# here than 256KB to leave enough space for the wrapping message. Large
+# structured output messages are stored on S3 so we don't have to stay with the
+# WebSocket server message size limit of 128KB for these messages.
+MESSAGE_SIZE_LIMIT = 250_000
 
 PyTestCaseStatus = t.Literal['passed', 'failed', 'skipped']
 CgTestCaseStatus = t.Literal['success', 'failure', 'skipped']
 
 # Mapping from the status used by pytest to the status used by CodeGrade.
 STATUS_NAME_MAP: t.Mapping[PyTestCaseStatus, CgTestCaseStatus] = {
     'passed': 'success',
@@ -102,15 +102,15 @@
     #: Message tag.
     tag: t.Literal['unit-test']
     #: The test results.
     results: t.List[TestSuiteResult]
 
 
 @dataclasses.dataclass
-class CgMarks:
+class CGMarks:
     """Marks set on each test case by the `cg-pytest-reporter` plugin used when
     generating the report.
     """
     #: The name of the test suite.
     suite_name: t.Optional[str]
     #: The weight of the test suite.
     suite_weight: t.Optional[Numeric]
@@ -125,21 +125,21 @@
     reason: t.Optional[str]
     #: The stdout produced while running the test.
     hide_stdout: bool
     #: The stderr produced while running the test.
     hide_stderr: bool
 
     @classmethod
-    def from_item(cls, item: pytest.Item) -> 'CgMarks':
+    def from_item(cls, item: pytest.Item) -> 'CGMarks':
         """Get the CodeGrade marks from the given item.
 
         :param item: The item to get the marks from.
-        :returns: A new `CgMarks` instance.
+        :returns: A new `CGMarks` instance.
         """
-        return CgMarks(
+        return CGMarks(
             suite_name=cls._as_str(
                 cls._get_suite_mark_value(item, 'cg_suite_name')
             ),
             suite_weight=cls._as_num(
                 cls._get_suite_mark_value(item, 'cg_suite_weight')
             ),
             name=cls._as_str(cls._get_mark_value(item, 'cg_name')),
@@ -249,15 +249,15 @@
         :returns: A report for the test that was run, including an extra
             `_cg_marks` attribute to make it possible to retrieve the mark
             values in the `pytest_runtest_logreport` hook.
         """
         report = pytest.TestReport.from_item_and_call(item, call)
         # `TestReport` has no property `_cg_marks`...
         # pylint: disable=protected-access
-        report._cg_marks = CgMarks.from_item(item)  # type: ignore
+        report._cg_marks = CGMarks.from_item(item)  # type: ignore
         return report
 
     def pytest_runtest_logreport(self, report: pytest.TestReport) -> None:
         """Write the report to the given file descriptor.
 
         :param report: The report to write.
         :returns: Nothing.
@@ -295,15 +295,15 @@
         test_suite: TestSuiteResult = {
             'id': suite_name,
             'name': suite_name,
             'testCases': [self._mk_test_case(case_name, report)],
         }
 
         # pylint: disable=protected-access
-        marks = t.cast(CgMarks, report._cg_marks)
+        marks = t.cast(CGMarks, report._cg_marks)
 
         if marks.suite_name is not None:
             test_suite['id'] = test_suite['name'] = marks.suite_name
         if marks.suite_weight is not None:
             test_suite['weight'] = float(marks.suite_weight)
 
         return test_suite
@@ -314,15 +314,15 @@
 
         test_case: TestCaseResult = {
             'name': name,
             'status': status,
         }
 
         # pylint: disable=protected-access
-        marks = t.cast(CgMarks, report._cg_marks)
+        marks = t.cast(CGMarks, report._cg_marks)
 
         if marks.name is not None:
             test_case['name'] = marks.name
         if marks.description is not None:
             test_case['description'] = marks.description
         if marks.weight is not None:
             test_case['weight'] = float(marks.weight)
@@ -350,15 +350,15 @@
         return test_case
 
     def _update_score(self, report: pytest.TestReport) -> None:
         if report.outcome == 'skipped':
             return
 
         # pylint: disable=protected-access
-        marks = t.cast(CgMarks, report._cg_marks)
+        marks = t.cast(CGMarks, report._cg_marks)
         weight = Fraction(1, 1)
 
         if marks.weight is not None:
             weight *= Fraction(marks.weight)
         if marks.suite_weight is not None:
             weight *= Fraction(marks.suite_weight)
```

### Comparing `cg_pytest_reporter-2023.5.19.1522/pyproject.toml` & `cg_pytest_reporter-2023.5.22.933/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2023.05.19.1522"
+version = "2023.05.22.0933"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{include = "cg_pytest_reporter"}]
 
 [tool.poetry.plugins.pytest11]
 cg_pytest_reporter = "cg_pytest_reporter.plugin"
```

### Comparing `cg_pytest_reporter-2023.5.19.1522/PKG-INFO` & `cg_pytest_reporter-2023.5.22.933/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-pytest-reporter
-Version: 2023.5.19.1522
+Version: 2023.5.22.933
 Summary: 
 Author: CodeGrade
 Author-email: info@codegrade.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -66,15 +66,15 @@
 Use the `suite_weight` decorator to change the weight of an entire suite
 relative to other suites in your test run.
 
 ```python
 from cg_pytest_reporter import suite_weight
 
 
-@suite_weight('My Test Suite')
+@suite_weight(2)
 class TestSuite:
     def test_function():
         assert True
 ```
 
 Similar to the suite name, you can set the weight of the module-level suite with
 the `__cg_suite_weight__` variable.
@@ -247,7 +247,45 @@
         print('Hello World!', file=sys.stderr)
         assert False
 
     def test_ok():
         print('Hello World!', file=sys.stderr)
 ```
 
+#### `hide_output`
+
+A combined version of `hide_stdout` and `hide_stderr`.
+
+```python
+import sys
+
+from cg_pytest_reporter import hide_output
+
+
+# The string "Hello World!" that was printed to `stdout` or `stderr` will not be
+# sent along with the results.
+@hide_output
+def test_failure():
+    print('Hello World!')
+    print('Hello World!', file=sys.stderr)
+    assert False
+```
+
+This decorator can also be applied to a test class to hide the output of each
+test case within it.
+
+```python
+import sys
+
+from cg_pytest_reporter import hide_output
+
+
+@hide_output
+class TestClass:
+    def test_failure():
+        print('Hello World!', file=sys.stderr)
+        assert False
+
+    def test_ok():
+        print('Hello World!')
+```
+
```

