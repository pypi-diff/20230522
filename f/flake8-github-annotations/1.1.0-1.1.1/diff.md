# Comparing `tmp/flake8_github_annotations-1.1.0.tar.gz` & `tmp/flake8_github_annotations-1.1.1.tar.gz`

## Comparing `flake8_github_annotations-1.1.0.tar` & `flake8_github_annotations-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/.flake8
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/assets/example_annotation.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/src/flake8_github_annotations/__about__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/src/flake8_github_annotations/__init__.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/src/flake8_github_annotations/formatter.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/tests/test_entrypoint.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/tests/integration/test_cli_output.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/README.md
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/.flake8
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/assets/example_annotation.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/src/flake8_github_annotations/__about__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/src/flake8_github_annotations/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/src/flake8_github_annotations/formatter.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/tests/test_entrypoint.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/tests/integration/test_cli_output.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/README.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 flake8_github_annotations-1.1.1/PKG-INFO
```

### Comparing `flake8_github_annotations-1.1.0/.github/workflows/ci.yml` & `flake8_github_annotations-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `flake8_github_annotations-1.1.0/assets/example_annotation.png` & `flake8_github_annotations-1.1.1/assets/example_annotation.png`

 * *Files identical despite different names*

### Comparing `flake8_github_annotations-1.1.0/src/flake8_github_annotations/formatter.py` & `flake8_github_annotations-1.1.1/src/flake8_github_annotations/formatter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from pathlib import Path
 from typing import Optional
 
 from flake8.formatting.base import BaseFormatter
-from flake8.options.manager import OptionManager
-from flake8.violation import Violation
 
 
 class GithubAnnotationsFormatter(BaseFormatter):
-    def format(self, error: Violation) -> Optional[str]:
+    name = "GithubAnnotationsFormatter"
+
+    def format(self, error) -> Optional[str]:
         return (
             f"::error file={self.path_prefix / error.filename},line={error.line_number}"
             f",col={error.column_number},title={error.code}::{error.text}"
         )
 
     @classmethod
-    def add_options(cls, option_manager: OptionManager) -> None:
+    def add_options(cls, option_manager) -> None:
         option_manager.add_option(
             "--github-annotation-path-prefix",
             default="",
             parse_from_config=True,
             help=(
                 "Path prefix to add to prepend to filenames"
                 "when using --format github"
             ),
         )
 
     @classmethod
-    def parse_options(cls, option_manager: OptionManager) -> None:
+    def parse_options(cls, option_manager) -> None:
         cls.path_prefix = Path(option_manager.github_annotation_path_prefix)
```

### Comparing `flake8_github_annotations-1.1.0/tests/integration/test_cli_output.py` & `flake8_github_annotations-1.1.1/tests/integration/test_cli_output.py`

 * *Files identical despite different names*

### Comparing `flake8_github_annotations-1.1.0/LICENSE.txt` & `flake8_github_annotations-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flake8_github_annotations-1.1.0/README.md` & `flake8_github_annotations-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8_github_annotations-1.1.0/pyproject.toml` & `flake8_github_annotations-1.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-  "flake8 >= 3.0.0"
+  "flake8 >= 4.0.0"
 ]
 dynamic = ["version"]
 
 [project.entry-points]
 "flake8.report" = { github = "flake8_github_annotations:GithubAnnotationsFormatter" }
 
 
@@ -43,30 +43,47 @@
   "hatch run test:test",
   "hatch run types:check",
   "hatch run style:check",
 ]
 
 [tool.hatch.envs.test]
 # Environment used to run tests
+matrix-name-format = "{variable}={value}"
 dependencies = [
   "pytest",
   "importlib_metadata; python_version < '3.10'",
+  "flake8=={matrix:flake8:6.0.0}"
 ]
 
 [tool.hatch.envs.test.scripts]
 test = 'pytest'
 
 [[tool.hatch.envs.test.matrix]]
 python = [
   "3.7",
   "3.8",
   "3.9",
   "3.10",
   "3.11",
 ]
+flake8 = [
+  "4.0.0",
+]
+[[tool.hatch.envs.test.matrix]]
+# flake8 6.0.0 does not support python 3.7
+python = [
+  "3.8",
+  "3.9",
+  "3.10",
+  "3.11",
+]
+flake8 = [
+  "6.0.0",
+]
+
 
 [tool.hatch.envs.types]
 # Environment used to type check
 dependencies = [
   "mypy",
   "pytest",
   "importlib_metadata; python_version < '3.10'",
```

### Comparing `flake8_github_annotations-1.1.0/PKG-INFO` & `flake8_github_annotations-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flake8-github-annotations
-Version: 1.1.0
+Version: 1.1.1
 Summary: A flake8 formatter that turns output into Github Annotations
 Project-URL: Documentation, https://github.com/gustavgransbo/flake8-github-annotations#readme
 Project-URL: Issues, https://github.com/gustavgransbo/flake8-github-annotations/issues
 Project-URL: Source, https://github.com/gustavgransbo/flake8-github-annotations
 Author-email: Gustav Gränsbo <gustav.gransbo@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: flake8>=3.0.0
+Requires-Dist: flake8>=4.0.0
 Description-Content-Type: text/markdown
 
 # flake8-github-annotations
 
 [![PyPI - Version](https://img.shields.io/pypi/v/flake8-github-annotations.svg)](https://pypi.org/project/flake8-github-annotations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flake8-github-annotations.svg)](https://pypi.org/project/flake8-github-annotations)
 [![CI](https://github.com/gustavgransbo/flake8-github-annotations/actions/workflows/ci.yml/badge.svg)](https://github.com/gustavgransbo/flake8-github-annotations/actions/workflows/ci.yml)
```

