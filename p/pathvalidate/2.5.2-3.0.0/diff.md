# Comparing `tmp/pathvalidate-2.5.2.tar.gz` & `tmp/pathvalidate-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathvalidate-2.5.2.tar", last modified: Sat Aug 20 16:29:46 2022, max compression
+gzip compressed data, was "pathvalidate-3.0.0.tar", last modified: Mon May 22 14:16:00 2023, max compression
```

## Comparing `pathvalidate-2.5.2.tar` & `pathvalidate-3.0.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.676245 pathvalidate-2.5.2/
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    11143 2022-08-20 16:29:46.676245 pathvalidate-2.5.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     9397 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)       97 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/pathvalidate/
--rw-r--r--   0 toor      (1000) toor      (1000)     1854 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4212 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3716 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)      266 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11876 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_filename.py
--rw-r--r--   0 toor      (1000) toor      (1000)    15074 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_filepath.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1271 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_ltsv.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3043 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/_symbol.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1622 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/argparse.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1673 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/click.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4175 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)      432 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/handler.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pathvalidate/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/pathvalidate.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    11143 2022-08-20 16:29:46.000000 pathvalidate-2.5.2/pathvalidate.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      888 2022-08-20 16:29:46.000000 pathvalidate-2.5.2/pathvalidate.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-08-20 16:29:46.000000 pathvalidate-2.5.2/pathvalidate.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       92 2022-08-20 16:29:46.000000 pathvalidate-2.5.2/pathvalidate.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2022-08-20 16:29:46.000000 pathvalidate-2.5.2/pathvalidate.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1292 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.666245 pathvalidate-2.5.2/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       84 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-08-20 16:29:46.676245 pathvalidate-2.5.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2861 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:46.676245 pathvalidate-2.5.2/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1875 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3944 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_argparse.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2325 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_click.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1490 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)    19670 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_filename.py
--rw-r--r--   0 toor      (1000) toor      (1000)    27906 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_filepath.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2441 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_ltsv.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4268 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/test/test_symbol.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1526 2022-08-20 16:29:01.000000 pathvalidate-2.5.2/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    11160 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     9413 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)       97 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/docs/pages/introduction/summary.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/pathvalidate/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1926 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6041 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3351 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      523 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14841 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_filename.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16234 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_filepath.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1203 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_ltsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2326 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_symbol.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      180 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/_types.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      970 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/argparse.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      960 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/click.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5313 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      441 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/handler.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pathvalidate/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/pathvalidate.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    11160 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      965 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:27.000000 pathvalidate-3.0.0/pathvalidate.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      136 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-05-22 14:15:59.000000 pathvalidate-3.0.0/pathvalidate.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1251 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       39 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2894 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-22 14:16:00.026778 pathvalidate-3.0.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1875 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4270 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_argparse.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2325 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_click.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1569 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      297 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    22640 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_filename.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    30287 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_filepath.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2500 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_ltsv.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4342 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/test/test_symbol.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1505 2023-05-22 14:15:18.000000 pathvalidate-3.0.0/tox.ini
```

### Comparing `pathvalidate-2.5.2/LICENSE` & `pathvalidate-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathvalidate-2.5.2/PKG-INFO` & `pathvalidate-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pathvalidate
-Version: 2.5.2
+Version: 3.0.0
 Summary: pathvalidate is a Python library to sanitize/validate a string such as filenames/file-paths/etc.
 Home-page: https://github.com/thombashi/pathvalidate
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://pathvalidate.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pathvalidate
 Project-URL: Tracker, https://github.com/thombashi/pathvalidate/issues
-Project-URL: Changes, https://github.com/thombashi/pathvalidate/releases
+Project-URL: Changlog, https://github.com/thombashi/pathvalidate/releases
 Keywords: file,path,validation,validator,sanitization,sanitizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -63,16 +63,16 @@
     :target: https://github.com/thombashi/pathvalidate/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/pathvalidate/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pathvalidate?branch=master
     :alt: Test coverage: coveralls
 
-.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
```

### Comparing `pathvalidate-2.5.2/README.rst` & `pathvalidate-3.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     :target: https://github.com/thombashi/pathvalidate/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/pathvalidate/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pathvalidate?branch=master
     :alt: Test coverage: coveralls
 
-.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
```

### Comparing `pathvalidate-2.5.2/pathvalidate/__init__.py` & `pathvalidate-3.0.0/pathvalidate/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 from .__version__ import __author__, __copyright__, __email__, __license__, __version__
 from ._base import AbstractSanitizer, AbstractValidator
 from ._common import (
-    Platform,
     ascii_symbols,
     normalize_platform,
     replace_ansi_escape,
     replace_unprintable_char,
     unprintable_ascii_chars,
-    validate_null_string,
     validate_pathtype,
+    validate_unprintable_char,
+)
+from ._const import Platform
+from ._filename import (
+    FileNameSanitizer,
+    FileNameValidator,
+    is_valid_filename,
+    sanitize_filename,
+    validate_filename,
 )
-from ._filename import FileNameSanitizer, is_valid_filename, sanitize_filename, validate_filename
 from ._filepath import (
     FilePathSanitizer,
+    FilePathValidator,
     is_valid_filepath,
-    sanitize_file_path,
     sanitize_filepath,
-    validate_file_path,
     validate_filepath,
 )
 from ._ltsv import sanitize_ltsv_label, validate_ltsv_label
 from ._symbol import replace_symbol, validate_symbol
 from .error import (
     ErrorReason,
     InvalidCharError,
-    InvalidLengthError,
     InvalidReservedNameError,
     NullNameError,
     ReservedNameError,
     ValidationError,
     ValidReservedNameError,
 )
 
@@ -48,28 +52,30 @@
     "Platform",
     "ascii_symbols",
     "normalize_platform",
     "replace_ansi_escape",
     "replace_unprintable_char",
     "unprintable_ascii_chars",
     "validate_pathtype",
+    "validate_unprintable_char",
     "FileNameSanitizer",
+    "FileNameValidator",
     "is_valid_filename",
     "sanitize_filename",
     "validate_filename",
     "FilePathSanitizer",
+    "FilePathValidator",
     "is_valid_filepath",
     "sanitize_filepath",
     "validate_filepath",
     "sanitize_ltsv_label",
     "validate_ltsv_label",
     "replace_symbol",
     "validate_symbol",
     "ErrorReason",
     "InvalidCharError",
-    "InvalidLengthError",
     "InvalidReservedNameError",
     "NullNameError",
     "ReservedNameError",
     "ValidationError",
     "ValidReservedNameError",
 )
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_base.py` & `pathvalidate-3.0.0/pathvalidate/_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import abc
 import os
-from typing import Optional, Tuple, cast
+import sys
+from typing import ClassVar, Optional, Tuple
 
-from ._common import PathType, Platform, PlatformType, normalize_platform, unprintable_ascii_chars
+from ._common import normalize_platform, unprintable_ascii_chars
+from ._const import DEFAULT_MIN_LEN, Platform
+from ._types import PathType, PlatformType
 from .error import ReservedNameError, ValidationError
-from .handler import Handler, return_null_string
-
-
-DEFAULT_MIN_LEN = 1
+from .handler import NullValueHandler, return_null_string
 
 
 class BaseFile:
-    _INVALID_PATH_CHARS = "".join(unprintable_ascii_chars)
-    _INVALID_FILENAME_CHARS = _INVALID_PATH_CHARS + "/"
-    _INVALID_WIN_PATH_CHARS = _INVALID_PATH_CHARS + ':*?"<>|\t\n\r\x0b\x0c'
-    _INVALID_WIN_FILENAME_CHARS = _INVALID_FILENAME_CHARS + _INVALID_WIN_PATH_CHARS + "\\"
-
-    _ERROR_MSG_TEMPLATE = "invalid char found: invalids=({invalid}), value={value}"
+    _INVALID_PATH_CHARS: ClassVar[str] = "".join(unprintable_ascii_chars)
+    _INVALID_FILENAME_CHARS: ClassVar[str] = _INVALID_PATH_CHARS + "/"
+    _INVALID_WIN_PATH_CHARS: ClassVar[str] = _INVALID_PATH_CHARS + ':*?"<>|\t\n\r\x0b\x0c'
+    _INVALID_WIN_FILENAME_CHARS: ClassVar[str] = (
+        _INVALID_FILENAME_CHARS + _INVALID_WIN_PATH_CHARS + "\\"
+    )
 
     @property
     def platform(self) -> Platform:
         return self.__platform
 
     @property
     def reserved_keywords(self) -> Tuple[str, ...]:
         return tuple()
 
     @property
-    def min_len(self) -> int:
-        return self._min_len
-
-    @property
     def max_len(self) -> int:
         return self._max_len
 
     def __init__(
         self,
-        min_len: int,
         max_len: int,
+        fs_encoding: Optional[str],
         check_reserved: bool,
-        null_value_handler: Optional[Handler] = None,
         platform_max_len: Optional[int] = None,
-        platform: PlatformType = None,
+        platform: Optional[PlatformType] = None,
     ) -> None:
         self.__platform = normalize_platform(platform)
         self._check_reserved = check_reserved
 
-        if null_value_handler is None:
-            null_value_handler = return_null_string
-        self._null_value_handler = null_value_handler
-
-        if min_len <= 0:
-            min_len = DEFAULT_MIN_LEN
-        self._min_len = max(min_len, 1)
-
         if platform_max_len is None:
             platform_max_len = self._get_default_max_path_len()
 
         if max_len <= 0:
             self._max_len = platform_max_len
         else:
-            self._max_len = cast(int, max_len)
+            self._max_len = max_len
 
         self._max_len = min(self._max_len, platform_max_len)
-        self._validate_max_len()
+
+        if fs_encoding:
+            self._fs_encoding = fs_encoding
+        else:
+            self._fs_encoding = sys.getfilesystemencoding()
 
     def _is_posix(self) -> bool:
         return self.platform == Platform.POSIX
 
     def _is_universal(self) -> bool:
         return self.platform == Platform.UNIVERSAL
 
-    def _is_linux(self) -> bool:
+    def _is_linux(self, include_universal: bool = False) -> bool:
+        if include_universal:
+            return self.platform in (Platform.UNIVERSAL, Platform.LINUX)
+
         return self.platform == Platform.LINUX
 
-    def _is_windows(self) -> bool:
-        return self.platform == Platform.WINDOWS
+    def _is_windows(self, include_universal: bool = False) -> bool:
+        if include_universal:
+            return self.platform in (Platform.UNIVERSAL, Platform.WINDOWS)
 
-    def _is_macos(self) -> bool:
-        return self.platform == Platform.MACOS
+        return self.platform == Platform.WINDOWS
 
-    def _validate_max_len(self) -> None:
-        if self.max_len < 1:
-            raise ValueError("max_len must be greater or equals to one")
+    def _is_macos(self, include_universal: bool = False) -> bool:
+        if include_universal:
+            return self.platform in (Platform.UNIVERSAL, Platform.MACOS)
 
-        if self.min_len > self.max_len:
-            raise ValueError("min_len must be lower than max_len")
+        return self.platform == Platform.MACOS
 
     def _get_default_max_path_len(self) -> int:
         if self._is_linux():
             return 4096
 
         if self._is_windows():
             return 260
@@ -101,14 +94,18 @@
         if self._is_posix() or self._is_macos():
             return 1024
 
         return 260  # universal
 
 
 class AbstractValidator(BaseFile, metaclass=abc.ABCMeta):
+    @abc.abstractproperty
+    def min_len(self) -> int:  # pragma: no cover
+        pass
+
     @abc.abstractmethod
     def validate(self, value: PathType) -> None:  # pragma: no cover
         pass
 
     def is_valid(self, value: PathType) -> bool:
         try:
             self.validate(value)
@@ -118,29 +115,90 @@
         return True
 
     def _is_reserved_keyword(self, value: str) -> bool:
         return value in self.reserved_keywords
 
 
 class AbstractSanitizer(BaseFile, metaclass=abc.ABCMeta):
+    def __init__(
+        self,
+        validator: AbstractValidator,
+        max_len: int,
+        fs_encoding: Optional[str],
+        check_reserved: bool,
+        validate_after_sanitize: bool,
+        null_value_handler: Optional[NullValueHandler] = None,
+        platform_max_len: Optional[int] = None,
+        platform: Optional[PlatformType] = None,
+    ) -> None:
+        super().__init__(
+            max_len=max_len,
+            fs_encoding=fs_encoding,
+            check_reserved=check_reserved,
+            platform_max_len=platform_max_len,
+            platform=platform,
+        )
+
+        if null_value_handler is None:
+            null_value_handler = return_null_string
+        self._null_value_handler = null_value_handler
+
+        self._validate_after_sanitize = validate_after_sanitize
+
+        self._validator = validator
+
     @abc.abstractmethod
     def sanitize(self, value: PathType, replacement_text: str = "") -> PathType:  # pragma: no cover
         pass
 
 
 class BaseValidator(AbstractValidator):
+    @property
+    def min_len(self) -> int:
+        return self._min_len
+
+    def __init__(
+        self,
+        min_len: int,
+        max_len: int,
+        fs_encoding: Optional[str],
+        check_reserved: bool,
+        platform_max_len: Optional[int] = None,
+        platform: Optional[PlatformType] = None,
+    ) -> None:
+        if min_len <= 0:
+            min_len = DEFAULT_MIN_LEN
+        self._min_len = max(min_len, 1)
+
+        super().__init__(
+            max_len=max_len,
+            fs_encoding=fs_encoding,
+            check_reserved=check_reserved,
+            platform_max_len=platform_max_len,
+            platform=platform,
+        )
+
+        self._validate_max_len()
+
     def _validate_reserved_keywords(self, name: str) -> None:
         if not self._check_reserved:
             return
 
         root_name = self.__extract_root_name(name)
         if self._is_reserved_keyword(root_name.upper()):
             raise ReservedNameError(
                 f"'{root_name}' is a reserved name",
                 reusable_name=False,
                 reserved_name=root_name,
                 platform=self.platform,
             )
 
+    def _validate_max_len(self) -> None:
+        if self.max_len < 1:
+            raise ValueError("max_len must be greater or equal to one")
+
+        if self.min_len > self.max_len:
+            raise ValueError("min_len must be lower than max_len")
+
     @staticmethod
     def __extract_root_name(path: str) -> str:
         return os.path.splitext(os.path.basename(path))[0]
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_common.py` & `pathvalidate-3.0.0/pathvalidate/_common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,46 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-import enum
 import platform
 import re
 import string
-import warnings
 from pathlib import Path
-from typing import Any, List, Optional, Union, cast
+from typing import Any, List, Optional
 
+from ._const import Platform
+from ._types import PathType, PlatformType
 
-_re_whitespaces = re.compile(r"^[\s]+$")
-
-
-@enum.unique
-class Platform(enum.Enum):
-    POSIX = "POSIX"
-    UNIVERSAL = "universal"
-
-    LINUX = "Linux"
-    WINDOWS = "Windows"
-    MACOS = "macOS"
 
-
-PathType = Union[str, Path]
-PlatformType = Union[str, Platform, None]
-
-
-def is_pathlike_obj(value: PathType) -> bool:
-    return isinstance(value, Path)
+_re_whitespaces = re.compile(r"^[\s]+$")
 
 
 def validate_pathtype(
     text: PathType, allow_whitespaces: bool = False, error_msg: Optional[str] = None
 ) -> None:
     from .error import ErrorReason, ValidationError
 
-    if _is_not_null_string(text) or is_pathlike_obj(text):
+    if _is_not_null_string(text) or isinstance(text, Path):
         return
 
     if allow_whitespaces and _re_whitespaces.search(str(text)):
         return
 
     if is_null_string(text):
-        if not error_msg:
-            error_msg = "the value must be a not empty"
-
-        raise ValidationError(
-            description=error_msg,
-            reason=ErrorReason.NULL_NAME,
-        )
+        raise ValidationError(reason=ErrorReason.NULL_NAME)
 
     raise TypeError(f"text must be a string: actual={type(text)}")
 
 
-def validate_null_string(text: PathType, error_msg: Optional[str] = None) -> None:
-    warnings.warn("'validate_null_string' has moved to 'validate_pathtype'", DeprecationWarning)
-
-    validate_pathtype(text, False, error_msg)
-
-
-def preprocess(name: PathType) -> str:
-    if is_pathlike_obj(name):
-        name = str(name)
+def to_str(name: PathType) -> str:
+    if isinstance(name, Path):
+        return str(name)
 
-    return cast(str, name)
+    return name
 
 
 def is_null_string(value: Any) -> bool:
     if value is None:
         return True
 
     try:
@@ -112,34 +83,44 @@
     "[{}]".format(re.escape("".join(unprintable_ascii_chars))), re.UNICODE
 )
 __RE_ANSI_ESCAPE = re.compile(
     r"(?:\x1B[@-Z\\-_]|[\x80-\x9A\x9C-\x9F]|(?:\x1B\[|\x9B)[0-?]*[ -/]*[@-~])"
 )
 
 
+def validate_unprintable_char(text: str) -> None:
+    from .error import InvalidCharError
+
+    match_list = __RE_UNPRINTABLE_CHARS.findall(to_str(text))
+    if match_list:
+        raise InvalidCharError(f"unprintable character found: {match_list}")
+
+
 def replace_unprintable_char(text: str, replacement_text: str = "") -> str:
     try:
         return __RE_UNPRINTABLE_CHARS.sub(replacement_text, text)
     except (TypeError, AttributeError):
         raise TypeError("text must be a string")
 
 
 def replace_ansi_escape(text: str, replacement_text: str = "") -> str:
     try:
         return __RE_ANSI_ESCAPE.sub(replacement_text, text)
     except (TypeError, AttributeError):
         raise TypeError("text must be a string")
 
 
-def normalize_platform(name: PlatformType) -> Platform:
+def normalize_platform(name: Optional[PlatformType]) -> Platform:
     if isinstance(name, Platform):
         return name
 
-    if name:
-        name = name.strip().casefold()
+    if not name:
+        return Platform.UNIVERSAL
+
+    name = name.strip().casefold()
 
     if name == "posix":
         return Platform.POSIX
 
     if name == "auto":
         name = platform.system().casefold()
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_filename.py` & `pathvalidate-3.0.0/pathvalidate/_filename.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,95 +5,115 @@
 import itertools
 import ntpath
 import posixpath
 import re
 from pathlib import Path
 from typing import Optional, Pattern, Tuple
 
-from ._base import DEFAULT_MIN_LEN, AbstractSanitizer, BaseFile, BaseValidator
-from ._common import (
-    PathType,
-    Platform,
-    PlatformType,
-    findall_to_str,
-    is_pathlike_obj,
-    preprocess,
-    validate_pathtype,
-)
-from .error import ErrorReason, InvalidCharError, InvalidLengthError, ValidationError
-from .handler import Handler
+from ._base import AbstractSanitizer, AbstractValidator, BaseFile, BaseValidator
+from ._common import findall_to_str, to_str, validate_pathtype
+from ._const import DEFAULT_MIN_LEN, INVALID_CHAR_ERR_MSG_TMPL, Platform
+from ._types import PathType, PlatformType
+from .error import ErrorReason, InvalidCharError, ValidationError
+from .handler import NullValueHandler
 
 
 _DEFAULT_MAX_FILENAME_LEN = 255
 _RE_INVALID_FILENAME = re.compile(f"[{re.escape(BaseFile._INVALID_FILENAME_CHARS):s}]", re.UNICODE)
 _RE_INVALID_WIN_FILENAME = re.compile(
     f"[{re.escape(BaseFile._INVALID_WIN_FILENAME_CHARS):s}]", re.UNICODE
 )
 
 
 class FileNameSanitizer(AbstractSanitizer):
     def __init__(
         self,
-        min_len: int = DEFAULT_MIN_LEN,
         max_len: int = _DEFAULT_MAX_FILENAME_LEN,
-        platform: PlatformType = None,
+        fs_encoding: Optional[str] = None,
+        platform: Optional[PlatformType] = None,
         check_reserved: bool = True,
-        null_value_handler: Optional[Handler] = None,
+        null_value_handler: Optional[NullValueHandler] = None,
+        validate_after_sanitize: bool = False,
+        validator: Optional[AbstractValidator] = None,
     ) -> None:
+        if validator:
+            fname_validator = validator
+        else:
+            fname_validator = FileNameValidator(
+                min_len=DEFAULT_MIN_LEN,
+                max_len=max_len,
+                fs_encoding=fs_encoding,
+                check_reserved=check_reserved,
+                platform=platform,
+            )
+
         super().__init__(
-            min_len=min_len,
             max_len=max_len,
+            fs_encoding=fs_encoding,
             check_reserved=check_reserved,
             null_value_handler=null_value_handler,
             platform_max_len=_DEFAULT_MAX_FILENAME_LEN,
             platform=platform,
+            validate_after_sanitize=validate_after_sanitize,
+            validator=fname_validator,
         )
 
         self._sanitize_regexp = self._get_sanitize_regexp()
-        self.__validator = FileNameValidator(
-            min_len=self.min_len,
-            max_len=self.max_len,
-            check_reserved=check_reserved,
-            platform=self.platform,
-        )
 
     def sanitize(self, value: PathType, replacement_text: str = "") -> PathType:
         try:
-            validate_pathtype(value, allow_whitespaces=False if self._is_windows() else True)
+            validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
+                if isinstance(value, Path):
+                    raise
+
                 return self._null_value_handler(e)
             raise
 
         sanitized_filename = self._sanitize_regexp.sub(replacement_text, str(value))
         sanitized_filename = sanitized_filename[: self.max_len]
 
         try:
-            self.__validator.validate(sanitized_filename)
+            self._validator.validate(sanitized_filename)
         except ValidationError as e:
             if e.reason == ErrorReason.RESERVED_NAME and e.reusable_name is False:
                 sanitized_filename = re.sub(
                     re.escape(e.reserved_name), f"{e.reserved_name}_", sanitized_filename
                 )
-            elif e.reason == ErrorReason.INVALID_CHARACTER:
-                if self.platform in [Platform.UNIVERSAL, Platform.WINDOWS]:
-                    # Do not end a file or directory name with a space or a period
+            elif e.reason == ErrorReason.INVALID_CHARACTER and self._is_windows(
+                include_universal=True
+            ):
+                # Do not start a file or directory name with a space
+                sanitized_filename = sanitized_filename.lstrip(" ")
+
+                # Do not end a file or directory name with a space or a period
+                sanitized_filename = sanitized_filename.rstrip(" ")
+                if sanitized_filename not in (".", ".."):
                     sanitized_filename = sanitized_filename.rstrip(" .")
             elif e.reason == ErrorReason.NULL_NAME:
-                return self._null_value_handler(e)
-            else:
-                raise
+                sanitized_filename = self._null_value_handler(e)
+
+        if self._validate_after_sanitize:
+            try:
+                self._validator.validate(sanitized_filename)
+            except ValidationError as e:
+                raise ValidationError(
+                    description=str(e),
+                    reason=ErrorReason.INVALID_AFTER_SANITIZE,
+                    platform=self.platform,
+                )
 
-        if is_pathlike_obj(value):
+        if isinstance(value, Path):
             return Path(sanitized_filename)
 
         return sanitized_filename
 
-    def _get_sanitize_regexp(self) -> Pattern:
-        if self.platform in [Platform.UNIVERSAL, Platform.WINDOWS]:
+    def _get_sanitize_regexp(self) -> Pattern[str]:
+        if self._is_windows(include_universal=True):
             return _RE_INVALID_WIN_FILENAME
 
         return _RE_INVALID_FILENAME
 
 
 class FileNameValidator(BaseValidator):
     _WINDOWS_RESERVED_FILE_NAMES = ("CON", "PRN", "AUX", "CLOCK$", "NUL") + tuple(
@@ -120,138 +140,165 @@
 
         return common_keywords
 
     def __init__(
         self,
         min_len: int = DEFAULT_MIN_LEN,
         max_len: int = _DEFAULT_MAX_FILENAME_LEN,
-        platform: PlatformType = None,
+        fs_encoding: Optional[str] = None,
+        platform: Optional[PlatformType] = None,
         check_reserved: bool = True,
     ) -> None:
         super().__init__(
             min_len=min_len,
             max_len=max_len,
+            fs_encoding=fs_encoding,
             check_reserved=check_reserved,
             platform_max_len=_DEFAULT_MAX_FILENAME_LEN,
             platform=platform,
         )
 
     def validate(self, value: PathType) -> None:
-        validate_pathtype(
-            value,
-            allow_whitespaces=False
-            if self.platform in [Platform.UNIVERSAL, Platform.WINDOWS]
-            else True,
-        )
+        validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
 
-        unicode_filename = preprocess(value)
-        value_len = len(unicode_filename)
+        unicode_filename = to_str(value)
+        byte_ct = len(unicode_filename.encode(self._fs_encoding))
 
         self.validate_abspath(unicode_filename)
 
-        if value_len > self.max_len:
-            raise InvalidLengthError(
-                f"filename is too long: expected<={self.max_len:d}, actual={value_len:d}"
+        err_kwargs = {
+            "reason": ErrorReason.INVALID_LENGTH,
+            "platform": self.platform,
+            "fs_encoding": self._fs_encoding,
+        }
+        if byte_ct > self.max_len:
+            raise ValidationError(
+                [
+                    f"filename is too long: expected<={self.max_len:d} bytes, actual={byte_ct:d} bytes"
+                ],
+                **err_kwargs,
             )
-        if value_len < self.min_len:
-            raise InvalidLengthError(
-                f"filename is too short: expected>={self.min_len:d}, actual={value_len:d}"
+        if byte_ct < self.min_len:
+            raise ValidationError(
+                [
+                    f"filename is too short: expected>={self.min_len:d} bytes, actual={byte_ct:d} bytes"
+                ],
+                **err_kwargs,
             )
 
         self._validate_reserved_keywords(unicode_filename)
 
-        if self._is_universal() or self._is_windows():
+        if self._is_windows(include_universal=True):
             self.__validate_win_filename(unicode_filename)
         else:
             self.__validate_unix_filename(unicode_filename)
 
     def validate_abspath(self, value: str) -> None:
         err = ValidationError(
             description=f"found an absolute path ({value}), expected a filename",
             platform=self.platform,
             reason=ErrorReason.FOUND_ABS_PATH,
         )
 
-        if self._is_universal() or self._is_windows():
+        if self._is_windows(include_universal=True):
             if ntpath.isabs(value):
                 raise err
 
         if posixpath.isabs(value):
             raise err
 
     def __validate_unix_filename(self, unicode_filename: str) -> None:
         match = _RE_INVALID_FILENAME.findall(unicode_filename)
         if match:
             raise InvalidCharError(
-                self._ERROR_MSG_TEMPLATE.format(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=findall_to_str(match), value=repr(unicode_filename)
                 )
             )
 
     def __validate_win_filename(self, unicode_filename: str) -> None:
         match = _RE_INVALID_WIN_FILENAME.findall(unicode_filename)
         if match:
             raise InvalidCharError(
-                self._ERROR_MSG_TEMPLATE.format(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=findall_to_str(match), value=repr(unicode_filename)
                 ),
                 platform=Platform.WINDOWS,
             )
 
         if unicode_filename in (".", ".."):
             return
 
+        KB2829981_err_tmpl = "{}. Refer: https://learn.microsoft.com/en-us/troubleshoot/windows-client/shell-experience/file-folder-name-whitespace-characters"  # noqa: E501
+
         if unicode_filename[-1] in (" ", "."):
             raise InvalidCharError(
-                self._ERROR_MSG_TEMPLATE.format(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=re.escape(unicode_filename[-1]), value=repr(unicode_filename)
                 ),
                 platform=Platform.WINDOWS,
-                description="Do not end a file or directory name with a space or a period",
+                description=KB2829981_err_tmpl.format(
+                    "Do not end a file or directory name with a space or a period"
+                ),
+            )
+
+        if unicode_filename[0] in (" "):
+            raise InvalidCharError(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
+                    invalid=re.escape(unicode_filename[0]), value=repr(unicode_filename)
+                ),
+                platform=Platform.WINDOWS,
+                description=KB2829981_err_tmpl.format(
+                    "Do not start a file or directory name with a space"
+                ),
             )
 
 
 def validate_filename(
     filename: PathType,
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     min_len: int = DEFAULT_MIN_LEN,
     max_len: int = _DEFAULT_MAX_FILENAME_LEN,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
 ) -> None:
     """Verifying whether the ``filename`` is a valid file name or not.
 
     Args:
         filename:
             Filename to validate.
         platform:
             Target platform name of the filename.
 
             .. include:: platform.txt
         min_len:
-            Minimum length of the ``filename``. The value must be greater or equal to one.
+            Minimum byte length of the ``filename``. The value must be greater or equal to one.
             Defaults to ``1``.
         max_len:
-            Maximum length of the ``filename``. The value must be lower than:
+            Maximum byte length of the ``filename``. The value must be lower than:
 
                 - ``Linux``: 4096
                 - ``macOS``: 1024
                 - ``Windows``: 260
                 - ``universal``: 260
 
             Defaults to ``255``.
+        fs_encoding:
+            Filesystem encoding that used to calculate the byte length of the filename.
+            If |None|, get the value from the execution environment.
         check_reserved:
             If |True|, check reserved names of the ``platform``.
 
     Raises:
         ValidationError (ErrorReason.INVALID_LENGTH):
             If the ``filename`` is longer than ``max_len`` characters.
         ValidationError (ErrorReason.INVALID_CHARACTER):
             If the ``filename`` includes invalid character(s) for a filename:
             |invalid_filename_chars|.
-            The following characters are also invalid for Windows platform:
+            The following characters are also invalid for Windows platforms:
             |invalid_win_filename_chars|.
         ValidationError (ErrorReason.RESERVED_NAME):
             If the ``filename`` equals reserved name by OS.
             Windows reserved name is as follows:
             ``"CON"``, ``"PRN"``, ``"AUX"``, ``"NUL"``, ``"COM[1-9]"``, ``"LPT[1-9]"``.
 
     Example:
@@ -259,23 +306,28 @@
 
     See Also:
         `Naming Files, Paths, and Namespaces - Win32 apps | Microsoft Docs
         <https://docs.microsoft.com/en-us/windows/win32/fileio/naming-a-file>`__
     """
 
     FileNameValidator(
-        platform=platform, min_len=min_len, max_len=max_len, check_reserved=check_reserved
+        platform=platform,
+        min_len=min_len,
+        max_len=max_len,
+        fs_encoding=fs_encoding,
+        check_reserved=check_reserved,
     ).validate(filename)
 
 
 def is_valid_filename(
     filename: PathType,
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     min_len: int = DEFAULT_MIN_LEN,
     max_len: Optional[int] = None,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
 ) -> bool:
     """Check whether the ``filename`` is a valid name or not.
 
     Args:
         filename:
             A filename to be checked.
@@ -287,58 +339,67 @@
         :py:func:`.validate_filename()`
     """
 
     return FileNameValidator(
         platform=platform,
         min_len=min_len,
         max_len=-1 if max_len is None else max_len,
+        fs_encoding=fs_encoding,
         check_reserved=check_reserved,
     ).is_valid(filename)
 
 
 def sanitize_filename(
     filename: PathType,
     replacement_text: str = "",
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     max_len: Optional[int] = _DEFAULT_MAX_FILENAME_LEN,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
-    null_value_handler: Optional[Handler] = None,
+    null_value_handler: Optional[NullValueHandler] = None,
+    validate_after_sanitize: bool = False,
 ) -> PathType:
     """Make a valid filename from a string.
 
-    To make a valid filename the function does:
+    To make a valid filename, the function does the following:
 
         - Replace invalid characters as file names included in the ``filename``
           with the ``replacement_text``. Invalid characters are:
 
             - unprintable characters
             - |invalid_filename_chars|
             - for Windows (or universal) only: |invalid_win_filename_chars|
 
-        - Append underscore (``"_"``) at the tail of the name if sanitized name
+        - Append underscore (``"_"``) at the tail of the return value if a sanitized name
           is one of the reserved names by operating systems
           (only when ``check_reserved`` is |True|).
 
     Args:
         filename: Filename to sanitize.
         replacement_text:
             Replacement text for invalid characters. Defaults to ``""``.
         platform:
             Target platform name of the filename.
 
             .. include:: platform.txt
         max_len:
-            Maximum length of the ``filename`` length. Truncate the name length if
-            the ``filename`` length exceeds this value.
+            Maximum byte length of the ``filename``.
+            Truncate the name length if the ``filename`` length exceeds this value.
             Defaults to ``255``.
+        fs_encoding:
+            Filesystem encoding that used to calculate the byte length of the filename.
+            If |None|, get the value from the execution environment.
         check_reserved:
             If |True|, sanitize reserved names of the ``platform``.
         null_value_handler:
             Function called when a value after sanitization is an empty string.
-            Defaults to ``pathvalidate.handler.return_null_string()`` that just return ``""``.
+            Defaults to ``pathvalidate.handler.return_null_string()`` function that
+            return an empty string.
+        validate_after_sanitize:
+            Execute validation after sanitization to the file name.
 
     Returns:
         Same type as the ``filename`` (str or PathLike object):
             Sanitized filename.
 
     Raises:
         ValueError:
@@ -347,10 +408,12 @@
     Example:
         :ref:`example-sanitize-filename`
     """
 
     return FileNameSanitizer(
         platform=platform,
         max_len=-1 if max_len is None else max_len,
+        fs_encoding=fs_encoding,
         check_reserved=check_reserved,
         null_value_handler=null_value_handler,
+        validate_after_sanitize=validate_after_sanitize,
     ).sanitize(filename, replacement_text)
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_filepath.py` & `pathvalidate-3.0.0/pathvalidate/_filepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,141 +2,142 @@
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import ntpath
 import os.path
 import posixpath
 import re
-import warnings
 from pathlib import Path
 from typing import List, Optional, Pattern, Tuple
 
-from ._base import DEFAULT_MIN_LEN, AbstractSanitizer, BaseFile, BaseValidator
-from ._common import (
-    PathType,
-    Platform,
-    PlatformType,
-    findall_to_str,
-    is_pathlike_obj,
-    preprocess,
-    validate_pathtype,
-)
-from ._const import _NTFS_RESERVED_FILE_NAMES
+from ._base import AbstractSanitizer, AbstractValidator, BaseFile, BaseValidator
+from ._common import findall_to_str, to_str, validate_pathtype
+from ._const import _NTFS_RESERVED_FILE_NAMES, DEFAULT_MIN_LEN, INVALID_CHAR_ERR_MSG_TMPL, Platform
 from ._filename import FileNameSanitizer, FileNameValidator
-from .error import (
-    ErrorReason,
-    InvalidCharError,
-    InvalidLengthError,
-    ReservedNameError,
-    ValidationError,
-)
-from .handler import Handler
+from ._types import PathType, PlatformType
+from .error import ErrorReason, InvalidCharError, ReservedNameError, ValidationError
+from .handler import NullValueHandler
 
 
 _RE_INVALID_PATH = re.compile(f"[{re.escape(BaseFile._INVALID_PATH_CHARS):s}]", re.UNICODE)
 _RE_INVALID_WIN_PATH = re.compile(f"[{re.escape(BaseFile._INVALID_WIN_PATH_CHARS):s}]", re.UNICODE)
 
 
 class FilePathSanitizer(AbstractSanitizer):
     def __init__(
         self,
-        min_len: int = DEFAULT_MIN_LEN,
         max_len: int = -1,
-        platform: PlatformType = None,
+        fs_encoding: Optional[str] = None,
+        platform: Optional[PlatformType] = None,
         check_reserved: bool = True,
-        null_value_handler: Optional[Handler] = None,
+        null_value_handler: Optional[NullValueHandler] = None,
         normalize: bool = True,
+        validate_after_sanitize: bool = False,
+        validator: Optional[AbstractValidator] = None,
     ) -> None:
+        if validator:
+            fpath_validator = validator
+        else:
+            fpath_validator = FilePathValidator(
+                min_len=DEFAULT_MIN_LEN,
+                max_len=max_len,
+                fs_encoding=fs_encoding,
+                check_reserved=check_reserved,
+                platform=platform,
+            )
         super().__init__(
-            min_len=min_len,
             max_len=max_len,
+            fs_encoding=fs_encoding,
             check_reserved=check_reserved,
+            validator=fpath_validator,
             null_value_handler=null_value_handler,
             platform=platform,
+            validate_after_sanitize=validate_after_sanitize,
         )
 
         self._sanitize_regexp = self._get_sanitize_regexp()
-        self.__fpath_validator = FilePathValidator(
-            min_len=self.min_len,
-            max_len=self.max_len,
-            check_reserved=check_reserved,
-            platform=self.platform,
-        )
         self.__fname_sanitizer = FileNameSanitizer(
-            min_len=self.min_len,
             max_len=self.max_len,
+            fs_encoding=fs_encoding,
             check_reserved=check_reserved,
+            null_value_handler=null_value_handler,
             platform=self.platform,
+            validate_after_sanitize=validate_after_sanitize,
         )
         self.__normalize = normalize
 
-        if self._is_universal() or self._is_windows():
+        if self._is_windows(include_universal=True):
             self.__split_drive = ntpath.splitdrive
         else:
             self.__split_drive = posixpath.splitdrive
 
     def sanitize(self, value: PathType, replacement_text: str = "") -> PathType:
         try:
-            validate_pathtype(value, allow_whitespaces=False if self._is_windows() else True)
+            validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
+                if isinstance(value, Path):
+                    raise
+
                 return self._null_value_handler(e)
             raise
 
-        self.__fpath_validator.validate_abspath(value)
-
-        unicode_filepath = preprocess(value)
+        unicode_filepath = to_str(value)
 
         drive, unicode_filepath = self.__split_drive(unicode_filepath)
         unicode_filepath = self._sanitize_regexp.sub(replacement_text, unicode_filepath)
         if self.__normalize and unicode_filepath:
             unicode_filepath = os.path.normpath(unicode_filepath)
         sanitized_path = unicode_filepath
 
-        if self._is_windows():
-            path_separator = "\\"
-        else:
-            path_separator = "/"
-
         sanitized_entries: List[str] = []
         if drive:
             sanitized_entries.append(drive)
         for entry in sanitized_path.replace("\\", "/").split("/"):
             if entry in _NTFS_RESERVED_FILE_NAMES:
                 sanitized_entries.append(f"{entry}_")
                 continue
 
-            sanitized_entry = str(self.__fname_sanitizer.sanitize(entry))
+            sanitized_entry = str(
+                self.__fname_sanitizer.sanitize(entry, replacement_text=replacement_text)
+            )
             if not sanitized_entry:
                 if not sanitized_entries:
                     sanitized_entries.append("")
                 continue
 
             sanitized_entries.append(sanitized_entry)
 
-        sanitized_path = path_separator.join(sanitized_entries)
+        sanitized_path = self.__get_path_separator().join(sanitized_entries)
         try:
-            self.__fpath_validator.validate(sanitized_path)
+            self._validator.validate(sanitized_path)
         except ValidationError as e:
             if e.reason == ErrorReason.NULL_NAME:
-                return self._null_value_handler(e)
+                sanitized_path = self._null_value_handler(e)
 
-            raise
+        if self._validate_after_sanitize:
+            self._validator.validate(sanitized_path)
 
-        if is_pathlike_obj(value):
+        if isinstance(value, Path):
             return Path(sanitized_path)
 
         return sanitized_path
 
-    def _get_sanitize_regexp(self) -> Pattern:
-        if self.platform in [Platform.UNIVERSAL, Platform.WINDOWS]:
+    def _get_sanitize_regexp(self) -> Pattern[str]:
+        if self._is_windows(include_universal=True):
             return _RE_INVALID_WIN_PATH
 
         return _RE_INVALID_PATH
 
+    def __get_path_separator(self) -> str:
+        if self._is_windows():
+            return "\\"
+
+        return "/"
+
 
 class FilePathValidator(BaseValidator):
     _RE_NTFS_RESERVED = re.compile(
         "|".join(f"^/{re.escape(pattern)}$" for pattern in _NTFS_RESERVED_FILE_NAMES),
         re.IGNORECASE,
     )
     _MACOS_RESERVED_FILE_PATHS = ("/", ":")
@@ -153,126 +154,130 @@
 
         return common_keywords
 
     def __init__(
         self,
         min_len: int = DEFAULT_MIN_LEN,
         max_len: int = -1,
-        platform: PlatformType = None,
+        fs_encoding: Optional[str] = None,
+        platform: Optional[PlatformType] = None,
         check_reserved: bool = True,
     ) -> None:
         super().__init__(
             min_len=min_len,
             max_len=max_len,
+            fs_encoding=fs_encoding,
             check_reserved=check_reserved,
             platform=platform,
         )
 
         self.__fname_validator = FileNameValidator(
             min_len=min_len, max_len=max_len, check_reserved=check_reserved, platform=platform
         )
 
-        if self._is_universal() or self._is_windows():
+        if self._is_windows(include_universal=True):
             self.__split_drive = ntpath.splitdrive
         else:
             self.__split_drive = posixpath.splitdrive
 
     def validate(self, value: PathType) -> None:
-        validate_pathtype(
-            value,
-            allow_whitespaces=False
-            if self.platform in [Platform.UNIVERSAL, Platform.WINDOWS]
-            else True,
-        )
+        validate_pathtype(value, allow_whitespaces=not self._is_windows(include_universal=True))
         self.validate_abspath(value)
 
-        _drive, value = self.__split_drive(str(value))
-        if not value:
+        _drive, tail = self.__split_drive(value)
+        if not tail:
             return
 
-        unicode_filepath = preprocess(value)
-        value_len = len(unicode_filepath)
-
-        if value_len > self.max_len:
-            raise InvalidLengthError(
-                f"file path is too long: expected<={self.max_len:d}, actual={value_len:d}"
+        unicode_filepath = to_str(tail)
+        byte_ct = len(unicode_filepath.encode(self._fs_encoding))
+        err_kwargs = {
+            "reason": ErrorReason.INVALID_LENGTH,
+            "platform": self.platform,
+            "fs_encoding": self._fs_encoding,
+        }
+
+        if byte_ct > self.max_len:
+            raise ValidationError(
+                [
+                    f"file path is too long: expected<={self.max_len:d} bytes, actual={byte_ct:d} bytes"
+                ],
+                **err_kwargs,
             )
-        if value_len < self.min_len:
-            raise InvalidLengthError(
-                "file path is too short: expected>={:d}, actual={:d}".format(
-                    self.min_len, value_len
-                )
+        if byte_ct < self.min_len:
+            raise ValidationError(
+                [
+                    "file path is too short: expected>={:d} bytes, actual={:d} bytes".format(
+                        self.min_len, byte_ct
+                    )
+                ],
+                **err_kwargs,
             )
 
         self._validate_reserved_keywords(unicode_filepath)
         unicode_filepath = unicode_filepath.replace("\\", "/")
         for entry in unicode_filepath.split("/"):
             if not entry or entry in (".", ".."):
                 continue
 
             self.__fname_validator._validate_reserved_keywords(entry)
 
-        if self._is_universal() or self._is_windows():
+        if self._is_windows(include_universal=True):
             self.__validate_win_filepath(unicode_filepath)
         else:
             self.__validate_unix_filepath(unicode_filepath)
 
     def validate_abspath(self, value: PathType) -> None:
-        value = str(value)
         is_posix_abs = posixpath.isabs(value)
         is_nt_abs = ntpath.isabs(value)
         err_object = ValidationError(
             description=(
                 "an invalid absolute file path ({}) for the platform ({}).".format(
                     value, self.platform.value
                 )
-                + " to avoid the error, specify an appropriate platform correspond"
-                + " with the path format, or 'auto'."
+                + " to avoid the error, specify an appropriate platform corresponding to"
+                + " the path format or 'auto'."
             ),
             platform=self.platform,
             reason=ErrorReason.MALFORMED_ABS_PATH,
         )
 
         if any([self._is_windows() and is_nt_abs, self._is_linux() and is_posix_abs]):
             return
 
         if self._is_universal() and any([is_posix_abs, is_nt_abs]):
             ValidationError(
                 description=(
-                    "{}. expected a platform independent file path".format(
-                        "POSIX absolute file path found"
-                        if is_posix_abs
-                        else "NT absolute file path found"
-                    )
+                    ("POSIX style" if is_posix_abs else "NT style")
+                    + " absolute file path found. expected a platform-independent file path."
                 ),
                 platform=self.platform,
                 reason=ErrorReason.MALFORMED_ABS_PATH,
             )
 
-        if any([self._is_windows(), self._is_universal()]) and is_posix_abs:
+        if self._is_windows(include_universal=True) and is_posix_abs:
             raise err_object
 
         drive, _tail = ntpath.splitdrive(value)
         if not self._is_windows() and drive and is_nt_abs:
             raise err_object
 
     def __validate_unix_filepath(self, unicode_filepath: str) -> None:
         match = _RE_INVALID_PATH.findall(unicode_filepath)
         if match:
             raise InvalidCharError(
-                self._ERROR_MSG_TEMPLATE.format(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=findall_to_str(match), value=repr(unicode_filepath)
                 )
             )
 
     def __validate_win_filepath(self, unicode_filepath: str) -> None:
         match = _RE_INVALID_WIN_PATH.findall(unicode_filepath)
         if match:
             raise InvalidCharError(
-                self._ERROR_MSG_TEMPLATE.format(
+                INVALID_CHAR_ERR_MSG_TMPL.format(
                     invalid=findall_to_str(match), value=repr(unicode_filepath)
                 ),
                 platform=Platform.WINDOWS,
             )
 
         _drive, value = self.__split_drive(unicode_filepath)
         if value:
@@ -285,47 +290,51 @@
                     reserved_name=reserved_name,
                     platform=self.platform,
                 )
 
 
 def validate_filepath(
     file_path: PathType,
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     min_len: int = DEFAULT_MIN_LEN,
     max_len: Optional[int] = None,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
 ) -> None:
     """Verifying whether the ``file_path`` is a valid file path or not.
 
     Args:
         file_path:
             File path to validate.
         platform:
             Target platform name of the file path.
 
             .. include:: platform.txt
         min_len:
-            Minimum length of the ``file_path``. The value must be greater or equal to one.
+            Minimum byte length of the ``file_path``. The value must be greater or equal to one.
             Defaults to ``1``.
         max_len:
-            Maximum length of the ``file_path`` length. If the value is |None| or minus,
+            Maximum byte length of the ``file_path``. If the value is |None| or minus,
             automatically determined by the ``platform``:
 
                 - ``Linux``: 4096
                 - ``macOS``: 1024
                 - ``Windows``: 260
                 - ``universal``: 260
+        fs_encoding:
+            Filesystem encoding that used to calculate the byte length of the file path.
+            If |None|, get the value from the execution environment.
         check_reserved:
             If |True|, check reserved names of the ``platform``.
 
     Raises:
         ValidationError (ErrorReason.INVALID_CHARACTER):
             If the ``file_path`` includes invalid char(s):
             |invalid_file_path_chars|.
-            The following characters are also invalid for Windows platform:
+            The following characters are also invalid for Windows platforms:
             |invalid_win_file_path_chars|
         ValidationError (ErrorReason.INVALID_LENGTH):
             If the ``file_path`` is longer than ``max_len`` characters.
         ValidationError:
             If ``file_path`` include invalid values.
 
     Example:
@@ -336,29 +345,25 @@
         <https://docs.microsoft.com/en-us/windows/win32/fileio/naming-a-file>`__
     """
 
     FilePathValidator(
         platform=platform,
         min_len=min_len,
         max_len=-1 if max_len is None else max_len,
+        fs_encoding=fs_encoding,
         check_reserved=check_reserved,
     ).validate(file_path)
 
 
-def validate_file_path(file_path, platform=None, max_path_len=None):
-    warnings.warn("'validate_file_path' has moved to 'validate_filepath'", DeprecationWarning)
-
-    validate_filepath(file_path, platform, max_path_len)
-
-
 def is_valid_filepath(
     file_path: PathType,
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     min_len: int = DEFAULT_MIN_LEN,
     max_len: Optional[int] = None,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
 ) -> bool:
     """Check whether the ``file_path`` is a valid name or not.
 
     Args:
         file_path:
             A filepath to be checked.
@@ -370,30 +375,33 @@
         :py:func:`.validate_filepath()`
     """
 
     return FilePathValidator(
         platform=platform,
         min_len=min_len,
         max_len=-1 if max_len is None else max_len,
+        fs_encoding=fs_encoding,
         check_reserved=check_reserved,
     ).is_valid(file_path)
 
 
 def sanitize_filepath(
     file_path: PathType,
     replacement_text: str = "",
-    platform: Optional[str] = None,
+    platform: Optional[PlatformType] = None,
     max_len: Optional[int] = None,
+    fs_encoding: Optional[str] = None,
     check_reserved: bool = True,
-    null_value_handler: Optional[Handler] = None,
+    null_value_handler: Optional[NullValueHandler] = None,
     normalize: bool = True,
+    validate_after_sanitize: bool = False,
 ) -> PathType:
     """Make a valid file path from a string.
 
-    To make a valid file path the function does:
+    To make a valid file path, the function does the following:
 
         - replace invalid characters for a file path within the ``file_path``
           with the ``replacement_text``. Invalid characters are as follows:
 
             - unprintable characters
             - |invalid_file_path_chars|
             - for Windows (or universal) only: |invalid_win_file_path_chars|
@@ -409,29 +417,34 @@
             Replacement text for invalid characters.
             Defaults to ``""``.
         platform:
             Target platform name of the file path.
 
             .. include:: platform.txt
         max_len:
-            Maximum length of the ``file_path`` length. Truncate the name if the ``file_path``
-            length exceedd this value. If the value is |None| or minus,
-            ``max_len`` will automatically determined by the ``platform``:
+            Maximum byte length of the file path.
+            Truncate the path if the value length exceeds the `max_len`.
+            If the value is |None| or minus, ``max_len`` will automatically determined by the ``platform``:
 
                 - ``Linux``: 4096
                 - ``macOS``: 1024
                 - ``Windows``: 260
                 - ``universal``: 260
+        fs_encoding:
+            Filesystem encoding that used to calculate the byte length of the file path.
+            If |None|, get the value from the execution environment.
         check_reserved:
             If |True|, sanitize reserved names of the ``platform``.
         null_value_handler:
             Function called when a value after sanitization is an empty string.
             Defaults to ``pathvalidate.handler.return_null_string()`` that just return ``""``.
         normalize:
             If |True|, normalize the the file path.
+        validate_after_sanitize:
+            Execute validation after sanitization to the file path.
 
     Returns:
         Same type as the argument (str or PathLike object):
             Sanitized filepath.
 
     Raises:
         ValueError:
@@ -440,17 +453,13 @@
     Example:
         :ref:`example-sanitize-file-path`
     """
 
     return FilePathSanitizer(
         platform=platform,
         max_len=-1 if max_len is None else max_len,
+        fs_encoding=fs_encoding,
         check_reserved=check_reserved,
         normalize=normalize,
         null_value_handler=null_value_handler,
+        validate_after_sanitize=validate_after_sanitize,
     ).sanitize(file_path, replacement_text)
-
-
-def sanitize_file_path(file_path, replacement_text="", platform=None, max_path_len=None):
-    warnings.warn("'sanitize_file_path' has moved to 'sanitize_filepath'", DeprecationWarning)
-
-    return sanitize_filepath(file_path, platform, max_path_len)
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_ltsv.py` & `pathvalidate-3.0.0/pathvalidate/_ltsv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import re
 
-from ._common import preprocess, validate_pathtype
+from ._common import to_str, validate_pathtype
 from .error import InvalidCharError
 
 
 __RE_INVALID_LTSV_LABEL = re.compile("[^0-9A-Za-z_.-]", re.UNICODE)
 
 
 def validate_ltsv_label(label: str) -> None:
@@ -17,27 +17,27 @@
     `Labeled Tab-separated Values (LTSV) <http://ltsv.org/>`__ label or not.
 
     :param label: Label to validate.
     :raises pathvalidate.ValidationError:
         If invalid character(s) found in the ``label`` for a LTSV format label.
     """
 
-    validate_pathtype(label, allow_whitespaces=False, error_msg="label is empty")
+    validate_pathtype(label, allow_whitespaces=False)
 
-    match_list = __RE_INVALID_LTSV_LABEL.findall(preprocess(label))
+    match_list = __RE_INVALID_LTSV_LABEL.findall(to_str(label))
     if match_list:
         raise InvalidCharError(f"invalid character found for a LTSV format label: {match_list}")
 
 
 def sanitize_ltsv_label(label: str, replacement_text: str = "") -> str:
     """
     Replace all of the symbols in text.
 
     :param label: Input text.
     :param replacement_text: Replacement text.
     :return: A replacement string.
     :rtype: str
     """
 
-    validate_pathtype(label, allow_whitespaces=False, error_msg="label is empty")
+    validate_pathtype(label, allow_whitespaces=False)
 
-    return __RE_INVALID_LTSV_LABEL.sub(replacement_text, preprocess(label))
+    return __RE_INVALID_LTSV_LABEL.sub(replacement_text, to_str(label))
```

### Comparing `pathvalidate-2.5.2/pathvalidate/_symbol.py` & `pathvalidate-3.0.0/pathvalidate/_symbol.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,37 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import re
-import warnings
 from typing import Sequence
 
-from ._common import ascii_symbols, preprocess, unprintable_ascii_chars
+from ._common import ascii_symbols, to_str, unprintable_ascii_chars
 from .error import InvalidCharError
 
 
-__RE_UNPRINTABLE = re.compile(
-    "[{}]".format(re.escape("".join(unprintable_ascii_chars))), re.UNICODE
-)
 __RE_SYMBOL = re.compile(
     "[{}]".format(re.escape("".join(ascii_symbols + unprintable_ascii_chars))), re.UNICODE
 )
 
 
-def validate_unprintable(text: str) -> None:
-    # deprecated
-    match_list = __RE_UNPRINTABLE.findall(preprocess(text))
-    if match_list:
-        raise InvalidCharError(f"unprintable character found: {match_list}")
-
-
-def replace_unprintable(text: str, replacement_text: str = "") -> str:
-    warnings.warn(
-        "'replace_unprintable' has moved to 'replace_unprintable_char'", DeprecationWarning
-    )
-
-    try:
-        return __RE_UNPRINTABLE.sub(replacement_text, preprocess(text))
-    except (TypeError, AttributeError):
-        raise TypeError("text must be a string")
-
-
 def validate_symbol(text: str) -> None:
     """
     Verifying whether symbol(s) included in the ``text`` or not.
 
     Args:
         text:
             Input text to validate.
 
     Raises:
         ValidationError (ErrorReason.INVALID_CHARACTER):
             If symbol(s) included in the ``text``.
     """
 
-    match_list = __RE_SYMBOL.findall(preprocess(text))
+    match_list = __RE_SYMBOL.findall(to_str(text))
     if match_list:
         raise InvalidCharError(f"invalid symbols found: {match_list}")
 
 
 def replace_symbol(
     text: str,
     replacement_text: str = "",
@@ -94,15 +72,15 @@
             ),
             re.UNICODE,
         )
     else:
         regexp = __RE_SYMBOL
 
     try:
-        new_text = regexp.sub(replacement_text, preprocess(text))
+        new_text = regexp.sub(replacement_text, to_str(text))
     except TypeError:
         raise TypeError("text must be a string")
 
     if not replacement_text:
         return new_text
 
     if is_replace_consecutive_chars:
```

### Comparing `pathvalidate-2.5.2/pathvalidate/click.py` & `pathvalidate-3.0.0/pathvalidate/click.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
-import warnings
-
 import click
 
-from ._common import PathType
 from ._filename import sanitize_filename, validate_filename
 from ._filepath import sanitize_filepath, validate_filepath
 from .error import ValidationError
 
 
 def validate_filename_arg(ctx, param, value) -> str:
     if not value:
@@ -32,47 +29,19 @@
         validate_filepath(value)
     except ValidationError as e:
         raise click.BadParameter(str(e))
 
     return value
 
 
-def sanitize_filename_arg(ctx, param, value) -> PathType:
+def sanitize_filename_arg(ctx, param, value: str) -> str:
     if not value:
         return ""
 
     return sanitize_filename(value)
 
 
-def sanitize_filepath_arg(ctx, param, value) -> PathType:
+def sanitize_filepath_arg(ctx, param, value: str) -> str:
     if not value:
         return ""
 
     return sanitize_filepath(value)
-
-
-def filename(ctx, param, value):  # pragma: no cover
-    warnings.warn("'filename' has moved to 'validate_filename'", DeprecationWarning)
-
-    if not value:
-        return None
-
-    try:
-        validate_filename(value)
-    except ValidationError as e:
-        raise click.BadParameter(str(e))
-
-    return sanitize_filename(value)
-
-
-def filepath(ctx, param, value):  # pragma: no cover
-    warnings.warn("'filepath' has moved to 'validate_filepath'", DeprecationWarning)
-
-    if not value:
-        return None
-
-    try:
-        validate_filepath(value)
-    except ValidationError as e:
-        raise click.BadParameter(str(e))
-
-    return sanitize_filepath(value)
```

### Comparing `pathvalidate-2.5.2/pathvalidate.egg-info/PKG-INFO` & `pathvalidate-3.0.0/pathvalidate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pathvalidate
-Version: 2.5.2
+Version: 3.0.0
 Summary: pathvalidate is a Python library to sanitize/validate a string such as filenames/file-paths/etc.
 Home-page: https://github.com/thombashi/pathvalidate
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://pathvalidate.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/pathvalidate
 Project-URL: Tracker, https://github.com/thombashi/pathvalidate/issues
-Project-URL: Changes, https://github.com/thombashi/pathvalidate/releases
+Project-URL: Changlog, https://github.com/thombashi/pathvalidate/releases
 Keywords: file,path,validation,validator,sanitization,sanitizer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -63,16 +63,16 @@
     :target: https://github.com/thombashi/pathvalidate/actions?query=workflow%3ATests
     :alt: Linux/macOS/Windows CI status
 
 .. image:: https://coveralls.io/repos/github/thombashi/pathvalidate/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pathvalidate?branch=master
     :alt: Test coverage: coveralls
 
-.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/pathvalidate/actions/workflows/codeql-analysis.yml
+.. image:: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pathvalidate/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Features
 ---------
 - Sanitize/Validate a string as a:
     - file name
     - file path
```

### Comparing `pathvalidate-2.5.2/pathvalidate.egg-info/SOURCES.txt` & `pathvalidate-3.0.0/pathvalidate.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 pathvalidate/_base.py
 pathvalidate/_common.py
 pathvalidate/_const.py
 pathvalidate/_filename.py
 pathvalidate/_filepath.py
 pathvalidate/_ltsv.py
 pathvalidate/_symbol.py
+pathvalidate/_types.py
 pathvalidate/argparse.py
 pathvalidate/click.py
 pathvalidate/error.py
 pathvalidate/handler.py
 pathvalidate/py.typed
 pathvalidate.egg-info/PKG-INFO
 pathvalidate.egg-info/SOURCES.txt
 pathvalidate.egg-info/dependency_links.txt
+pathvalidate.egg-info/not-zip-safe
 pathvalidate.egg-info/requires.txt
 pathvalidate.egg-info/top_level.txt
 requirements/docs_requirements.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 test/__init__.py
 test/_common.py
 test/test_argparse.py
 test/test_click.py
 test/test_common.py
+test/test_error.py
 test/test_filename.py
 test/test_filepath.py
 test/test_ltsv.py
 test/test_symbol.py
```

### Comparing `pathvalidate-2.5.2/pyproject.toml` & `pathvalidate-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -57,20 +57,18 @@
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = 3.6
 
 pretty = true
-strict = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
-warn_unused_ignores = true
 
 [tool.pytest.ini_options]
 testpaths = [
     "test",
 ]
 
 md_report = true
```

### Comparing `pathvalidate-2.5.2/setup.py` & `pathvalidate-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "pathvalidate"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -51,15 +51,15 @@
     include_package_data=True,
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
-        "Changes": f"{REPOSITORY_URL:s}/releases",
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
     },
     python_requires=">=3.6",
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
@@ -76,9 +76,10 @@
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: System :: Filesystems",
         "Topic :: Text Processing",
     ],
+    zip_safe=False,
     cmdclass=get_release_command_class(),
 )
```

### Comparing `pathvalidate-2.5.2/test/_common.py` & `pathvalidate-3.0.0/test/_common.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-2.5.2/test/test_argparse.py` & `pathvalidate-3.0.0/test/test_argparse.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,57 +8,90 @@
     sanitize_filepath_arg,
     validate_filename_arg,
     validate_filepath_arg,
 )
 
 
 class Test_validate_filename_arg:
-    @pytest.mark.parametrize(["value"], [["abc"], ["abc.txt"], [""]])
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            ["abc"],
+            ["abc.txt"],
+            [""],
+        ],
+    )
     def test_normal(self, value):
         parser = ArgumentParser()
         parser.add_argument("filename", type=validate_filename_arg)
 
         assert parser.parse_args([value]).filename == value
 
-    @pytest.mark.parametrize(["value"], [["foo/abc"], ["a?c"], ["COM1"], ["a" * 8000]])
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            ["foo/abc"],
+            ["a?c"],
+            ["COM1"],
+            ["a" * 8000],
+        ],
+    )
     def test_exception(self, value):
         parser = ArgumentParser()
         parser.add_argument("filename", type=validate_filename_arg)
 
         try:
             parser.parse_args([value])
         except SystemExit as e:
             assert isinstance(e.__context__, ArgumentError)
         else:
             raise RuntimeError()
 
 
 class Test_validate_filepath_arg:
-    @pytest.mark.parametrize(["value"], [["foo/abc"], ["foo/abc.txt"], [""]])
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            ["foo/abc"],
+            ["foo/abc.txt"],
+            [""],
+        ],
+    )
     def test_normal(self, value):
         parser = ArgumentParser()
         parser.add_argument("filepath", type=validate_filepath_arg)
 
         assert parser.parse_args([value]).filepath == value
 
     @pytest.mark.skipif(platform.system() == "Windows", reason="platform dependent tests")
-    @pytest.mark.parametrize(["value"], [["a" * 8000]])
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            ["a" * 8000],
+        ],
+    )
     def test_exception_posix(self, value):
         parser = ArgumentParser()
         parser.add_argument("filepath", type=validate_filepath_arg)
 
         try:
             parser.parse_args([value])
         except SystemExit as e:
             assert isinstance(e.__context__, ArgumentError)
         else:
             raise RuntimeError()
 
     @pytest.mark.skipif(platform.system() != "Windows", reason="platform dependent tests")
-    @pytest.mark.parametrize(["value"], [["foo/a?c"], ["COM1"]])
+    @pytest.mark.parametrize(
+        ["value"],
+        [
+            ["foo/a?c"],
+            ["COM1"],
+        ],
+    )
     def test_exception_windows(self, value):
         parser = ArgumentParser()
         parser.add_argument("filepath", type=validate_filepath_arg)
 
         try:
             parser.parse_args([value])
         except SystemExit as e:
```

### Comparing `pathvalidate-2.5.2/test/test_click.py` & `pathvalidate-3.0.0/test/test_click.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-2.5.2/test/test_common.py` & `pathvalidate-3.0.0/test/test_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,21 +28,28 @@
             ["A" + c + "B", rep, "A" + rep + "B"]
             for c, rep in itertools.product(TARGET_CHARS, REPLACE_TEXT_LIST)
         ]
         + [
             ["A" + c + "B", rep, "A" + c + "B"]
             for c, rep in itertools.product(NOT_TARGET_CHARS, REPLACE_TEXT_LIST)
         ]
-        + [["", "", ""]],
+        + [
+            ["", "", ""],
+        ],
     )
     def test_normal(self, value, replace_text, expected):
         assert replace_unprintable_char(value, replace_text) == expected
 
     @pytest.mark.parametrize(
-        ["value", "expected"], [[None, TypeError], [1, TypeError], [True, TypeError]]
+        ["value", "expected"],
+        [
+            [None, TypeError],
+            [1, TypeError],
+            [True, TypeError],
+        ],
     )
     def test_abnormal(self, value, expected):
         with pytest.raises(expected):
             replace_unprintable_char(value)
 
 
 class Test_replace_ansi_escape:
```

### Comparing `pathvalidate-2.5.2/test/test_filename.py` & `pathvalidate-3.0.0/test/test_filename.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import platform as m_platform
 import random
+import sys
 from collections import OrderedDict
 from itertools import chain, product
 from pathlib import Path
 
 import pytest
 from allpairspy import AllPairs
 
@@ -15,15 +16,15 @@
     ErrorReason,
     Platform,
     ValidationError,
     is_valid_filename,
     sanitize_filename,
     validate_filename,
 )
-from pathvalidate._common import is_pathlike_obj, unprintable_ascii_chars
+from pathvalidate._common import unprintable_ascii_chars
 from pathvalidate._filename import FileNameSanitizer, FileNameValidator
 from pathvalidate.handler import raise_error, return_null_string, return_timestamp
 
 from ._common import (
     INVALID_FILENAME_CHARS,
     INVALID_PATH_CHARS,
     INVALID_WIN_FILENAME_CHARS,
@@ -44,15 +45,19 @@
 
 VALID_MULTIBYTE_NAMES = ["新しいテキスト ドキュメント.txt", "新規 Microsoft Excel Worksheet.xlsx"]
 
 
 class Test_FileSanitizer:
     @pytest.mark.parametrize(
         ["test_platform", "expected"],
-        [["windows", Platform.WINDOWS], ["linux", Platform.LINUX], ["macos", Platform.MACOS]],
+        [
+            ["windows", Platform.WINDOWS],
+            ["linux", Platform.LINUX],
+            ["macos", Platform.MACOS],
+        ],
     )
     def test_normal_platform_auto(self, monkeypatch, test_platform, expected):
         if test_platform == "windows":
             patch = lambda: "windows"
         elif test_platform == "linux":
             patch = lambda: "linux"
         elif test_platform == "macos":
@@ -60,14 +65,16 @@
         else:
             raise ValueError(f"unexpected test platform: {test_platform}")
 
         monkeypatch.setattr(m_platform, "system", patch)
 
         assert FileNameSanitizer(255, platform="auto").platform == expected
 
+
+class Test_FileNameValidator:
     @pytest.mark.parametrize(
         ["test_platform", "expected"],
         [
             [
                 "windows",
                 (
                     "CON",
@@ -127,24 +134,31 @@
     )
     def test_normal(self, value, platform):
         validate_filename(value, platform)
         assert is_valid_filename(value, platform=platform)
 
     @pytest.mark.parametrize(
         ["platform"],
-        [["linux"], ["macos"], ["posix"]],
+        [
+            ["linux"],
+            ["macos"],
+            ["posix"],
+        ],
     )
     def test_normal_only_whitespaces(self, platform):
         value = "  "
         validate_filename(value, platform)
         assert is_valid_filename(value, platform=platform)
 
     @pytest.mark.parametrize(
         ["platform"],
-        [["windows"], ["universal"]],
+        [
+            ["windows"],
+            ["universal"],
+        ],
     )
     def test_abnormal_only_whitespaces(self, platform):
         value = "  "
         with pytest.raises(ValidationError) as e:
             validate_filename(value, platform=platform)
             assert e.value.reason == ErrorReason.NULL
         assert not is_valid_filename(value, platform)
@@ -196,14 +210,39 @@
             return
 
         with pytest.raises(ValidationError) as e:
             validate_filename(value, platform=platform, max_len=max_len)
         assert e.value.reason == expected
 
     @pytest.mark.parametrize(
+        ["value", "platform", "fs_encoding", "max_len", "expected"],
+        [
+            ["あ" * 85, "universal", "utf-8", 255, None],
+            ["あ" * 86, "universal", "utf-8", 255, ErrorReason.INVALID_LENGTH],
+            ["あ" * 126, "universal", "utf-16", 255, None],
+            ["あ" * 127, "universal", "utf-16", 255, ErrorReason.INVALID_LENGTH],
+        ],
+    )
+    def test_max_len_fs_encoding(self, value, platform, fs_encoding, max_len, expected):
+        kwargs = {
+            "platform": platform,
+            "max_len": max_len,
+            "fs_encoding": fs_encoding,
+        }
+
+        if expected is None:
+            validate_filename(value, **kwargs)
+            assert is_valid_filename(value, **kwargs)
+            return
+
+        with pytest.raises(ValidationError) as e:
+            validate_filename(value, **kwargs)
+        assert e.value.reason == expected
+
+    @pytest.mark.parametrize(
         ["value", "min_len", "max_len", "expected"],
         [
             ["minux max_len", 1, -1, None],
             ["zero max_len", 1, 0, None],
             ["valid length", 1, 255, None],
             ["eq min max", 10, 10, None],
             ["inversion", 100, 1, ValueError],
@@ -351,16 +390,16 @@
     def test_exception_escape_err_msg(self, value, platform, expected):
         with pytest.raises(ValidationError) as e:
             print(platform, repr(value))
             validate_filename(value, platform=platform)
 
         assert e.value.reason == ErrorReason.INVALID_CHARACTER
         assert str(e.value) == (
-            r"invalid char found: invalids=('\r'), value='asdf\rsdf', "
-            "reason=INVALID_CHARACTER, target-platform=Windows"
+            r"[PV1100] invalid characters found: invalids=('\r'), value='asdf\rsdf', "
+            "target-platform=Windows"
         )  # noqa
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             [None, ValueError],
             ["", ValidationError],
@@ -405,27 +444,41 @@
             for c, rep in product(NOT_SANITIZE_CHARS, REPLACE_TEXT_LIST)
         ]
         + [
             [pair.platform, "A" + pair.c + "B", pair.repl, "A" + pair.repl + "B"]
             for pair in AllPairs(
                 OrderedDict(
                     {
-                        "platform": ["posix", "linux", "macos"],
+                        "platform": [
+                            "posix",
+                            "linux",
+                            "macos",
+                            Platform.POSIX,
+                            Platform.LINUX,
+                            Platform.MACOS,
+                        ],
                         "c": INVALID_PATH_CHARS + unprintable_ascii_chars,
                         "repl": REPLACE_TEXT_LIST,
                     }
                 )
             )
         ]
         + [
             [pair.platform, "A" + pair.c + "B", pair.repl, "A" + pair.c + "B"]
             for pair in AllPairs(
                 OrderedDict(
                     {
-                        "platform": ["posix", "linux", "macos"],
+                        "platform": [
+                            "posix",
+                            "linux",
+                            "macos",
+                            Platform.POSIX,
+                            Platform.LINUX,
+                            Platform.MACOS,
+                        ],
                         "c": [":", "*", "?", '"', "<", ">", "|"],
                         "repl": REPLACE_TEXT_LIST,
                     }
                 )
             )
         ],
     )
@@ -446,15 +499,15 @@
             [Path("A" + c + "B"), rep, Path("A" + c + "B")]
             for c, rep in product(NOT_SANITIZE_CHARS, REPLACE_TEXT_LIST)
         ],
     )
     def test_normal_pathlike(self, value, replace_text, expected):
         sanitized_name = sanitize_filename(value, replace_text)
         assert sanitized_name == expected
-        assert is_pathlike_obj(sanitized_name)
+        assert isinstance(sanitized_name, Path)
 
         validate_filename(sanitized_name)
         assert is_valid_filename(sanitized_name)
 
     @pytest.mark.parametrize(
         ["value"],
         [
@@ -528,36 +581,80 @@
         ["value", "check_reserved", "expected"],
         [
             ["CON", True, "CON_"],
             ["CON", False, "CON"],
         ],
     )
     def test_normal_check_reserved(self, value, check_reserved, expected):
-        assert (
-            sanitize_filename(value, platform="windows", check_reserved=check_reserved) == expected
-        )
+        for platform in ["windows", "universal"]:
+            assert (
+                sanitize_filename(value, platform=platform, check_reserved=check_reserved)
+                == expected
+            )
 
     @pytest.mark.parametrize(
         ["platform", "value", "expected"],
         [
             ["windows", "period.", "period"],
             ["windows", "space ", "space"],
+            ["windows", " space ", "space"],
             ["windows", "space_and_period .", "space_and_period"],
             ["windows", "space_and_period. ", "space_and_period"],
+            ["windows", " .space_and_period", ".space_and_period"],
+            ["windows", ". space_and_period", ". space_and_period"],
+            ["windows", ". ", "."],
+            ["windows", " .", "."],
+            ["windows", " . ", "."],
+            ["windows", ".. ", ".."],
             ["linux", "period.", "period."],
             ["linux", "space ", "space "],
             ["linux", "space_and_period. ", "space_and_period. "],
             ["universal", "period.", "period"],
             ["universal", "space ", "space"],
             ["universal", "space_and_period .", "space_and_period"],
+            ["universal", ". ", "."],
+            ["universal", " .", "."],
+            ["universal", " . ", "."],
+            ["universal", ".. ", ".."],
         ],
     )
     def test_normal_space_or_period_at_tail(self, platform, value, expected):
         filename = sanitize_filename(value, platform=platform)
         assert filename == expected
         assert is_valid_filename(filename, platform=platform)
 
-    @pytest.mark.parametrize(["value", "expected"], [[1, TypeError], [True, TypeError]])
+    @pytest.mark.parametrize(
+        ["platform", "value"],
+        [
+            [platform, value]
+            for platform, value in product(
+                ["windows", "universal"],
+                [
+                    "\a\r",
+                ],
+            )
+        ],
+    )
+    def test_exception_invalid_after_sanitize(self, platform, value):
+        kwargs = {
+            "platform": platform,
+            "replacement_text": "",
+            "validate_after_sanitize": False,
+        }
+        print("'{}'".format(sanitize_filename(value, **kwargs)), file=sys.stderr)
+        kwargs["validate_after_sanitize"] = True
+
+        with pytest.raises(ValidationError) as e:
+            sanitize_filename(value, **kwargs)
+        assert e.value.reason == ErrorReason.INVALID_AFTER_SANITIZE
+
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            [1, TypeError],
+            [True, TypeError],
+        ],
+    )
     def test_exception_type(self, value, expected):
         with pytest.raises(expected):
             sanitize_filename(value)
         assert not is_valid_filename(value)
```

### Comparing `pathvalidate-2.5.2/test/test_filepath.py` & `pathvalidate-3.0.0/test/test_filepath.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ErrorReason,
     Platform,
     ValidationError,
     is_valid_filepath,
     sanitize_filepath,
     validate_filepath,
 )
-from pathvalidate._common import is_pathlike_obj, unprintable_ascii_chars
+from pathvalidate._common import unprintable_ascii_chars
 from pathvalidate._filepath import FilePathSanitizer, FilePathValidator
 from pathvalidate.handler import raise_error, return_null_string, return_timestamp
 
 from ._common import (
     INVALID_PATH_CHARS,
     INVALID_WIN_PATH_CHARS,
     NTFS_RESERVED_FILE_NAMES,
@@ -40,15 +40,19 @@
 
 random.seed(0)
 
 
 class Test_FileSanitizer:
     @pytest.mark.parametrize(
         ["test_platform", "expected"],
-        [["windows", Platform.WINDOWS], ["linux", Platform.LINUX], ["macos", Platform.MACOS]],
+        [
+            ["windows", Platform.WINDOWS],
+            ["linux", Platform.LINUX],
+            ["macos", Platform.MACOS],
+        ],
     )
     def test_normal_platform_auto(self, monkeypatch, test_platform, expected):
         if test_platform == "windows":
             patch = lambda: "windows"
         elif test_platform == "linux":
             patch = lambda: "linux"
         elif test_platform == "macos":
@@ -107,24 +111,31 @@
     )
     def test_normal(self, value, platform):
         validate_filepath(value, platform)
         assert is_valid_filepath(value, platform=platform)
 
     @pytest.mark.parametrize(
         ["platform"],
-        [["linux"], ["macos"], ["posix"]],
+        [
+            ["linux"],
+            ["macos"],
+            ["posix"],
+        ],
     )
     def test_normal_only_whitespaces(self, platform):
         value = "  "
         validate_filepath(value, platform)
         assert is_valid_filepath(value, platform=platform)
 
     @pytest.mark.parametrize(
         ["platform"],
-        [["windows"], ["universal"]],
+        [
+            ["windows"],
+            ["universal"],
+        ],
     )
     def test_abnormal_only_whitespaces(self, platform):
         value = "  "
         with pytest.raises(ValidationError) as e:
             validate_filepath(value, platform=platform)
             assert e.value.reason == ErrorReason.NULL
         assert not is_valid_filepath(value, platform)
@@ -183,42 +194,77 @@
             ["a" * 260, "universal", None, None],
             ["a" * 261, "universal", None, ErrorReason.INVALID_LENGTH],
             ["a" * 300, "universal", 1024, ErrorReason.INVALID_LENGTH],
             ["a" * 261, Platform.UNIVERSAL, None, ErrorReason.INVALID_LENGTH],
         ],
     )
     def test_normal_max_len(self, value, platform, max_len, expected):
+        kwargs = {
+            "platform": platform,
+            "max_len": max_len,
+        }
+
         if expected is None:
-            validate_filepath(value, platform=platform, max_len=max_len)
-            assert is_valid_filepath(value, platform=platform, max_len=max_len)
+            validate_filepath(value, **kwargs)
+            assert is_valid_filepath(value, **kwargs)
             return
 
         with pytest.raises(ValidationError) as e:
-            validate_filepath(value, platform=platform, max_len=max_len)
+            validate_filepath(value, **kwargs)
         assert e.value.reason == ErrorReason.INVALID_LENGTH
 
     @pytest.mark.parametrize(
+        ["value", "platform", "fs_encoding", "max_len", "expected"],
+        [
+            ["/tmp/" + "あ" * 83, "linux", "utf-8", 255, None],
+            ["/tmp/" + "あ" * 84, "linux", "utf-8", 255, ErrorReason.INVALID_LENGTH],
+            ["/tmp/" + "あ" * 121, "linux", "utf-16", 255, None],
+            ["/tmp/" + "あ" * 122, "linux", "utf-16", 255, ErrorReason.INVALID_LENGTH],
+        ],
+    )
+    def test_max_len_fs_encoding(self, value, platform, fs_encoding, max_len, expected):
+        kwargs = {
+            "platform": platform,
+            "max_len": max_len,
+            "fs_encoding": fs_encoding,
+        }
+
+        if expected is None:
+            validate_filepath(value, **kwargs)
+            assert is_valid_filepath(value, **kwargs)
+            return
+
+        with pytest.raises(ValidationError) as e:
+            validate_filepath(value, **kwargs)
+        assert e.value.reason == expected
+
+    @pytest.mark.parametrize(
         ["value", "min_len", "max_len", "expected"],
         [
             ["valid length", 1, 255, None],
             ["minus min_len", -2, 100, None],
             ["minus max_len", -3, -2, None],
             ["zero max_len", -2, 0, None],
             ["eq min max", 10, 10, None],
             ["inversion", 100, 1, ValueError],
         ],
     )
     def test_minmax_len(self, value, min_len, max_len, expected):
+        kwargs = {
+            "min_len": min_len,
+            "max_len": max_len,
+        }
+
         if expected is None:
-            validate_filepath(value, min_len=min_len, max_len=max_len)
-            assert is_valid_filepath(value, min_len=min_len, max_len=max_len)
+            validate_filepath(value, **kwargs)
+            assert is_valid_filepath(value, **kwargs)
             return
 
         with pytest.raises(expected):
-            validate_filepath(value, min_len=min_len, max_len=max_len)
+            validate_filepath(value, **kwargs)
 
     @pytest.mark.parametrize(
         ["test_platform", "value", "expected"],
         [
             ["linux", "/a/b/c.txt", None],
             ["linux", "C:\\a\\b\\c.txt", ValidationError],
             ["windows", "/a/b/c.txt", None],
@@ -423,16 +469,16 @@
     def test_exception_escape_err_msg(self, value, platform, expected):
         with pytest.raises(ValidationError) as e:
             print(platform, repr(value))
             validate_filepath(value, platform=platform)
 
         assert e.value.reason == expected
         assert str(e.value) == (
-            r"invalid char found: invalids=('\r'), value='asdf\rsdf', "
-            "reason=INVALID_CHARACTER, target-platform=Windows"
+            r"[PV1100] invalid characters found: invalids=('\r'), value='asdf\rsdf', "
+            "target-platform=Windows"
         )  # noqa
 
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             [None, ValueError],
             ["", ValidationError],
@@ -503,27 +549,41 @@
             for c, rep in product(NOT_SANITIZE_CHARS, REPLACE_TEXTS)
         ]
         + [
             [pair.platform, "A" + pair.c + "B", pair.repl, "A" + pair.repl + "B"]
             for pair in AllPairs(
                 OrderedDict(
                     {
-                        "platform": ["posix", "linux", "macos"],
+                        "platform": [
+                            "posix",
+                            "linux",
+                            "macos",
+                            Platform.POSIX,
+                            Platform.LINUX,
+                            Platform.MACOS,
+                        ],
                         "c": INVALID_PATH_CHARS + unprintable_ascii_chars,
                         "repl": REPLACE_TEXTS,
                     }
                 )
             )
         ]
         + [
             [pair.platform, "A" + pair.c + "B", pair.repl, "A" + pair.c + "B"]
             for pair in AllPairs(
                 OrderedDict(
                     {
-                        "platform": ["posix", "linux", "macos"],
+                        "platform": [
+                            "posix",
+                            "linux",
+                            "macos",
+                            Platform.POSIX,
+                            Platform.LINUX,
+                            Platform.MACOS,
+                        ],
                         "c": [":", "*", "?", '"', "<", ">", "|"],
                         "repl": REPLACE_TEXTS,
                     }
                 )
             )
         ],
     )
@@ -614,15 +674,15 @@
             [Path("あ" + c + "い"), rep, Path("あ" + c + "い")]
             for c, rep in product(NOT_SANITIZE_CHARS, REPLACE_TEXTS)
         ],
     )
     def test_normal_pathlike(self, value, replace_text, expected):
         sanitized_name = sanitize_filepath(value, replace_text)
         assert sanitized_name == expected
-        assert is_pathlike_obj(sanitized_name)
+        assert isinstance(sanitized_name, Path)
 
         validate_filepath(sanitized_name)
         assert is_valid_filepath(sanitized_name)
 
     @pytest.mark.parametrize(
         ["test_platform", "value", "expected"],
         [
@@ -730,23 +790,52 @@
     @pytest.mark.parametrize(
         ["value", "expected"],
         [
             ["C:\\a\\b\\c.txt", ValidationError],
         ],
     )
     def test_auto_platform_linux(self, value, expected):
+        kwargs = {
+            "platform": "auto",
+            "validate_after_sanitize": True,
+        }
+
         if isinstance(expected, str):
-            sanitized = sanitize_filepath(value, platform="auto")
+            sanitized = sanitize_filepath(value, **kwargs)
             assert is_valid_filepath(sanitized, platform="auto")
-        else:
-            with pytest.raises(expected):
-                sanitize_filepath(value, platform="auto")
+            return
+
+        with pytest.raises(expected) as e:
+            sanitize_filepath(value, **kwargs)
+        assert e.value.reason == ErrorReason.MALFORMED_ABS_PATH
+
+    @pytest.mark.parametrize(
+        ["platform", "value"],
+        [
+            ["windows", "CON \r"],
+        ],
+    )
+    def test_exception_invalid_after_sanitize(self, platform, value):
+        print(
+            "'{}'".format(
+                sanitize_filepath(value, platform=platform, validate_after_sanitize=False)
+            ),
+            file=sys.stderr,
+        )
+        with pytest.raises(ValidationError) as e:
+            sanitize_filepath(value, platform=platform, validate_after_sanitize=True)
+        assert e.value.reason == ErrorReason.INVALID_AFTER_SANITIZE
 
     @pytest.mark.skipif(sys.version_info < (3, 6), reason="requires python3.6 or higher")
     @pytest.mark.parametrize(
         ["value", "expected"],
-        [[1, TypeError], [True, TypeError], [nan, TypeError], [inf, TypeError]],
+        [
+            [1, TypeError],
+            [True, TypeError],
+            [nan, TypeError],
+            [inf, TypeError],
+        ],
     )
     def test_exception_type(self, value, expected):
         with pytest.raises(expected):
             sanitize_filepath(value)
         assert not is_valid_filepath(value)
```

### Comparing `pathvalidate-2.5.2/test/test_ltsv.py` & `pathvalidate-3.0.0/test/test_ltsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,12 +85,17 @@
 
     @pytest.mark.parametrize(["value", "expected"], [["aあいbうえcお", "abc"]])
     def test_normal_multibyte(self, value, expected):
         sanitize_ltsv_label(value)
 
     @pytest.mark.parametrize(
         ["value", "expected"],
-        [["", ValidationError], [None, ValidationError], [1, TypeError], [True, TypeError]],
+        [
+            ["", ValidationError],
+            [None, ValidationError],
+            [1, TypeError],
+            [True, TypeError],
+        ],
     )
     def test_abnormal(self, value, expected):
         with pytest.raises(expected):
             sanitize_ltsv_label(value)
```

### Comparing `pathvalidate-2.5.2/test/test_symbol.py` & `pathvalidate-3.0.0/test/test_symbol.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import itertools
 
 import pytest
 
-from pathvalidate import ascii_symbols, replace_symbol, unprintable_ascii_chars, validate_symbol
-from pathvalidate._symbol import validate_unprintable
+from pathvalidate import (
+    ascii_symbols,
+    replace_symbol,
+    unprintable_ascii_chars,
+    validate_symbol,
+    validate_unprintable_char,
+)
 from pathvalidate.error import ErrorReason, ValidationError
 
 from ._common import alphanum_chars
 
 
 class Test_validate_symbol:
     VALID_CHARS = alphanum_chars
@@ -92,41 +97,46 @@
                 is_replace_consecutive_chars=is_replace_consecutive_chars,
                 is_strip=is_strip,
             )
             == expected
         )
 
     @pytest.mark.parametrize(
-        ["value", "expected"], [[None, TypeError], [1, TypeError], [True, TypeError]]
+        ["value", "expected"],
+        [
+            [None, TypeError],
+            [1, TypeError],
+            [True, TypeError],
+        ],
     )
     def test_abnormal(self, value, expected):
         with pytest.raises(expected):
             replace_symbol(value)
 
 
-class Test_validate_unprintable:
+class Test_validate_unprintable_char:
     VALID_CHARS = alphanum_chars
     INVALID_CHARS = unprintable_ascii_chars
 
     @pytest.mark.parametrize(
         ["value"], [["abc" + valid_char + "hoge123"] for valid_char in VALID_CHARS]
     )
     def test_normal(self, value):
-        validate_unprintable(value)
+        validate_unprintable_char(value)
 
     @pytest.mark.parametrize(["value"], [["あいうえお"], ["シート"]])
     def test_normal_multibyte(self, value):
         pytest.skip("TODO")
 
-        validate_unprintable(value)
+        validate_unprintable_char(value)
 
     @pytest.mark.parametrize(
         ["value"],
         [
             ["abc" + invalid_char + "hoge123"]
             for invalid_char in INVALID_CHARS + unprintable_ascii_chars
         ],
     )
     def test_exception_invalid_char(self, value):
         with pytest.raises(ValidationError) as e:
-            validate_unprintable(value)
+            validate_unprintable_char(value)
         assert e.value.reason == ErrorReason.INVALID_CHARACTER
```

### Comparing `pathvalidate-2.5.2/tox.ini` & `pathvalidate-3.0.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,26 @@
     test
 allowlist_externals =
     pytest
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
     twine
     wheel
 commands =
     python setup.py sdist bdist_wheel
     twine check dist/*.whl dist/*.tar.gz
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.3.1
+    cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
 extras =
     test
 deps =
@@ -50,28 +49,28 @@
     -r{toxinidir}/requirements/docs_requirements.txt
 commands =
     python setup.py build_sphinx --source-dir=docs/ --build-dir=docs/_build --all-files
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
-    black>=22.6
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports --exclude ".pytype" .
     isort .
     black setup.py test pathvalidate
 
 [testenv:lint]
 skip_install = true
 deps =
-    codespell
-    mypy>=0.971
-    pylama
+    codespell>=2
+    mypy>=1
+    pylama>=8.4.1
     types-click
 commands =
     python setup.py check
     mypy pathvalidate setup.py
     codespell pathvalidate docs/pages examples test -q2 --check-filenames
     pylama pathvalidate test setup.py
```

