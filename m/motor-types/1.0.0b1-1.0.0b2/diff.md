# Comparing `tmp/motor_types-1.0.0b1.tar.gz` & `tmp/motor_types-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motor_types-1.0.0b1.tar", max compression
+gzip compressed data, was "motor_types-1.0.0b2.tar", max compression
```

## Comparing `motor_types-1.0.0b1.tar` & `motor_types-1.0.0b2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1093 2022-12-21 07:54:32.629951 motor_types-1.0.0b1/LICENSE
--rw-r--r--   0        0        0      120 2023-01-29 08:30:26.441624 motor_types-1.0.0b1/motor-stubs/__init__.pyi
--rw-r--r--   0        0        0      113 2023-01-14 06:42:30.382805 motor_types-1.0.0b1/motor-stubs/aiohttp/__init__.pyi
--rw-r--r--   0        0        0    38673 2023-02-12 04:44:52.847585 motor_types-1.0.0b1/motor-stubs/core.pyi
--rw-r--r--   0        0        0     1050 2023-01-14 06:42:30.382805 motor_types-1.0.0b1/motor-stubs/docstrings.pyi
--rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b1/motor-stubs/frameworks/asyncio.pyi
--rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b1/motor-stubs/frameworks/tornado.pyi
--rw-r--r--   0        0        0     2584 2023-01-14 17:06:11.003894 motor_types-1.0.0b1/motor-stubs/metaprogramming.pyi
--rw-r--r--   0        0        0    14489 2023-02-12 04:44:52.892909 motor_types-1.0.0b1/motor-stubs/motor_asyncio.pyi
--rw-r--r--   0        0        0       75 2023-01-14 06:42:30.393216 motor_types-1.0.0b1/motor-stubs/motor_common.pyi
--rw-r--r--   0        0        0     6753 2023-02-12 04:45:50.680209 motor_types-1.0.0b1/motor-stubs/motor_gridfs.pyi
--rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b1/motor-stubs/motor_tornado.pyi
--rw-r--r--   0        0        0        0 2023-01-14 06:42:30.399448 motor_types-1.0.0b1/motor-stubs/web.pyi
--rw-r--r--   0        0        0     1830 2023-02-12 04:56:54.259851 motor_types-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3999 2023-01-29 11:15:43.353472 motor_types-1.0.0b1/README.md
--rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 motor_types-1.0.0b1/setup.py
--rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 motor_types-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-12-21 07:54:32.629951 motor_types-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0      120 2023-01-29 08:30:26.441624 motor_types-1.0.0b2/motor-stubs/__init__.pyi
+-rw-r--r--   0        0        0      113 2023-01-14 06:42:30.382805 motor_types-1.0.0b2/motor-stubs/aiohttp/__init__.pyi
+-rw-r--r--   0        0        0    38690 2023-02-23 08:51:03.335031 motor_types-1.0.0b2/motor-stubs/core.pyi
+-rw-r--r--   0        0        0     1050 2023-01-14 06:42:30.382805 motor_types-1.0.0b2/motor-stubs/docstrings.pyi
+-rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b2/motor-stubs/frameworks/asyncio.pyi
+-rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b2/motor-stubs/frameworks/tornado.pyi
+-rw-r--r--   0        0        0     2584 2023-01-14 17:06:11.003894 motor_types-1.0.0b2/motor-stubs/metaprogramming.pyi
+-rw-r--r--   0        0        0    14489 2023-02-12 04:44:52.892909 motor_types-1.0.0b2/motor-stubs/motor_asyncio.pyi
+-rw-r--r--   0        0        0       75 2023-01-14 06:42:30.393216 motor_types-1.0.0b2/motor-stubs/motor_common.pyi
+-rw-r--r--   0        0        0     6766 2023-05-22 18:58:36.326032 motor_types-1.0.0b2/motor-stubs/motor_gridfs.pyi
+-rw-r--r--   0        0        0        0 2023-01-14 06:42:30.393216 motor_types-1.0.0b2/motor-stubs/motor_tornado.pyi
+-rw-r--r--   0        0        0        0 2023-01-14 06:42:30.399448 motor_types-1.0.0b2/motor-stubs/web.pyi
+-rw-r--r--   0        0        0     1829 2023-05-22 19:01:31.556443 motor_types-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3999 2023-01-29 11:15:43.353472 motor_types-1.0.0b2/README.md
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 motor_types-1.0.0b2/PKG-INFO
```

### Comparing `motor_types-1.0.0b1/LICENSE` & `motor_types-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `motor_types-1.0.0b1/motor-stubs/core.pyi` & `motor_types-1.0.0b2/motor-stubs/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -727,15 +727,15 @@
         callback: typing.Callable[
             [typing.Optional[_Document], typing.Optional[Exception]], typing.Any
         ] = None,
     ) -> None: ...
     def get_io_loop(self) -> _IO_Loop: ...
     async def next(self) -> _Document: ...
     def next_object(self) -> _Document: ...
-    async def to_list(self, length: int) -> typing.List[_Document]: ...
+    async def to_list(self, length: typing.Optional[int]) -> typing.List[_Document]: ...
 
 class AgnosticCursor(AgnosticBaseCursor):
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, memodict: typing.Optional[typing.Dict] = None) -> Self: ...
     async def _Cursor__die(self, synchronous=False) -> None: ...
     def _data(self) -> _deque: ...
     def _killed(self) -> bool: ...
```

### Comparing `motor_types-1.0.0b1/motor-stubs/docstrings.pyi` & `motor_types-1.0.0b2/motor-stubs/docstrings.pyi`

 * *Files identical despite different names*

### Comparing `motor_types-1.0.0b1/motor-stubs/metaprogramming.pyi` & `motor_types-1.0.0b2/motor-stubs/metaprogramming.pyi`

 * *Files identical despite different names*

### Comparing `motor_types-1.0.0b1/motor-stubs/motor_asyncio.pyi` & `motor_types-1.0.0b2/motor-stubs/motor_asyncio.pyi`

 * *Files identical despite different names*

### Comparing `motor_types-1.0.0b1/motor-stubs/motor_gridfs.pyi` & `motor_types-1.0.0b2/motor-stubs/motor_gridfs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,18 +59,18 @@
     async def __aiter__(self) -> Self: ...
     async def __anext__(self) -> bytes: ...
     def __getattr__(self, name: str) -> Any: ...
     async def _ensure_file(self) -> None: ...
     async def close(self) -> None: ...
     def get_io_loop(self) -> _IO_Loop: ...
     async def open(self) -> Self: ...
-    def read(self, size: int = -1) -> bytes: ...
+    async def read(self, size: int = -1) -> bytes: ...
     def readable(self) -> Literal[True]: ...
     async def readchunk(self) -> bytes: ...
-    def readline(self, size: int = -1) -> bytes: ...
+    async def readline(self, size: int = -1) -> bytes: ...
     def seek(self, pos: int, whence: int = _SEEK_SET) -> int: ...
     def tell(self) -> int: ...
     def seekable(self) -> Literal[True]: ...
     async def write(self, data: Any) -> None: ...
     async def stream_to_handler(self, request_handler: _Handler) -> None: ...
 
 class AgnosticGridIn(object):
@@ -185,12 +185,12 @@
         metadata: Optional[Mapping[str, Any]] = None,
         session: Optional[_Session] = None,
     ) -> ObjectId: ...
     async def upload_from_stream_with_id(
         self,
         file_id: Any,
         filename: str,
-        source: IO,
+        source: Any,
         chunk_size_bytes: Optional[int] = None,
         metadata: Optional[Mapping[str, Any]] = None,
         session: Optional[_Session] = None,
     ) -> None: ...
```

### Comparing `motor_types-1.0.0b1/pyproject.toml` & `motor_types-1.0.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motor-types"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "Python stubs for Motor, a Non-Blocking MongoDB driver for Python's Tornado and AsyncIO based applications."
 authors = ["L0RD-ZER0 <ackerhon@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "motor-stubs"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -21,15 +21,15 @@
     "Topic :: Text Editors",
     "Topic :: Utilities",
     "Typing :: Stubs Only",
 ]
 homepage = "https://github.com/L0RD-ZER0/Motor-Types"
 repository = "https://github.com/L0RD-ZER0/Motor-Types"
 
-[tools.poetry.urls]
+[tool.poetry.urls]
 "Bug Tracker" = "https://github.com/L0RD-ZER0/Motor-Types/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 pymongo = { version = ">=4.3.0" }
 motor = { version = ">=3.0.0", optional = true }
 typing-extensions = { version = ">=4.0.0" }
```

### Comparing `motor_types-1.0.0b1/README.md` & `motor_types-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `motor_types-1.0.0b1/setup.py` & `motor_types-1.0.0b2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['motor-stubs']
-
-package_data = \
-{'': ['*'], 'motor-stubs': ['aiohttp/*', 'frameworks/*']}
-
-install_requires = \
-['pymongo>=4.3.0', 'typing-extensions>=4.0.0']
-
-extras_require = \
-{'motor': ['motor>=3.0.0', 'dnspython>=2.3.0']}
-
-setup_kwargs = {
-    'name': 'motor-types',
-    'version': '1.0.0b1',
-    'description': "Python stubs for Motor, a Non-Blocking MongoDB driver for Python's Tornado and AsyncIO based applications.",
-    'long_description': 'Motor-Types\n===========\nPython stubs for [Motor], a Non-Blocking [MongoDB] driver for [Python]\'s [Tornado] and [AsyncIO] based applications.\n\nAbout\n------\nStubs for [Motor] (version 3.0.0+) for substituting the missing type-hints. These stubs are meant to be used along with\npycharm and mypy to facilitate static type-checking. Installing this package adds these `.pyi` files to\n`libs/site-packages/motor`. Currently, only the stubs for [AsyncIO] are supported. You can contribute to stubs for\n[Tornado] by opening a pull request for the same.\n\n**Note:** This project is currently under development and is in no way affiliated with MongoDB. This is an unofficial\nstub package.\n\nHow to use?\n-----------\n\nYou can either install from [PyPI] using [pip] or add files to your project directories manually.\n\n### Installing Using [pip]:\n```commandline\npip install motor-types\n```\n\n### To install [Motor] (and [Dnspython]) alongside the package:\n```commandline\npip install motor-types[motor]\n```\n\n### To add files to the project manually:\nUse this command to clone the repository:\n```commandline\ngit clone "https://github.com/L0RD-ZER0/Motor-Types"\n```\n\nAfterwards, you can do either of the following to use stubs:\n* Copy the stubs manually to either ``libs/site-packages/motor`` or ``libs/site-packages/motor-stubs``, ideally the latter.\n* Add these stubs manually to project directories.\n  * [For MyPy][MyPy-Stubs].\n  * [For PyCharm][PyCharm-Stubs].\n  * For other static type-checking tools, consider referring to their corresponding documentation regarding stubs.\n\nExamples:\n---------\n### Auto-Complete Example\n**Without Stubs:**\n\n![ACNS]\n\n**With Stubs:**\n\n![ACWS]\n\n### Type-Checking Example\n**Without Stubs:**\n\n![TCNS]\n\n**With Stubs:**\n\n![TCWS]\n\nDependencies\n------------\nThis package uses following dependencies:\n* [Poetry] (For Packaging and Publishing)\n* [PyMongo] (For PyMongo related types)\n* [Motor] (For Referencing and for motor installation extra)\n* [Dnspython] (For motor installation extra)\n* [Pre-Commit] (For maintaining code quality)\n* [Typing-Extensions] (For using the latest typing features)\n\nHow to Contribute?\n------------------\nThe simplest contribution you can make is by opening a [GitHub Issue][GH-Issues] or by forking the repository and making\na pull request on the [GitHub Repository][GH-Repo] for the same. The changes can be as simple as improving the\ndocumentation or as big as completing any incomplete section of the typings.\n\n**Note:** All issues and pull-requests are subjected to a preliminary inspection.\n\nLicense\n-------\nThis repository is licensed under MIT License. The [license][License] can be found within the repository.\n\n\n[Motor]: https://github.com/mongodb/motor\n[MongoDB]: https://www.mongodb.com\n[PyMongo]: https://github.com/mongodb/mongo-python-driver\n[Poetry]: https://github.com/python-poetry/poetry\n[pip]: https://pypi.org/project/pip/\n[Dnspython]: https://www.dnspython.org/\n[Pre-Commit]: https://pre-commit.com\n[Typing-Extensions]: https://github.com/python/typing_extensions\n[Python]: https://python.org\n[Tornado]: https://www.tornadoweb.org/\n[Asyncio]: https://docs.python.org/3/library/asyncio.html\n[PyPI]: https://pypi.org/\n[MyPy-Stubs]: https://mypy.readthedocs.io/en/stable/stubs.html#stub-files\n[PyCharm-Stubs]: https://www.jetbrains.com/help/pycharm/stubs.html\n[GH-Repo]: https://github.com/L0RD-ZER0/Motor-Types\n[GH-Issues]: https://github.com/L0RD-ZER0/Motor-Types/issues\n[License]: https://github.com/L0RD-ZER0/Motor-Types/blob/master/LICENSE\n[ACNS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/auto-complete-example-ns.png\n[ACWS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/auto-complete-example-ws.png\n[TCNS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/type-checking-example-ns.png\n[TCWS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/type-checking-example-ws.png',
-    'author': 'L0RD-ZER0',
-    'author_email': 'ackerhon@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/L0RD-ZER0/Motor-Types',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8.0,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: motor-types
+Version: 1.0.0b2
+Summary: Python stubs for Motor, a Non-Blocking MongoDB driver for Python's Tornado and AsyncIO based applications.
+Home-page: https://github.com/L0RD-ZER0/Motor-Types
+License: MIT
+Author: L0RD-ZER0
+Author-email: ackerhon@gmail.com
+Requires-Python: >=3.8.0,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Text Editors
+Classifier: Topic :: Utilities
+Classifier: Typing :: Stubs Only
+Provides-Extra: motor
+Requires-Dist: dnspython (>=2.3.0) ; extra == "motor"
+Requires-Dist: motor (>=3.0.0) ; extra == "motor"
+Requires-Dist: pymongo (>=4.3.0)
+Requires-Dist: typing-extensions (>=4.0.0)
+Project-URL: Bug Tracker, https://github.com/L0RD-ZER0/Motor-Types/issues
+Project-URL: Repository, https://github.com/L0RD-ZER0/Motor-Types
+Description-Content-Type: text/markdown
+
+Motor-Types
+===========
+Python stubs for [Motor], a Non-Blocking [MongoDB] driver for [Python]'s [Tornado] and [AsyncIO] based applications.
+
+About
+------
+Stubs for [Motor] (version 3.0.0+) for substituting the missing type-hints. These stubs are meant to be used along with
+pycharm and mypy to facilitate static type-checking. Installing this package adds these `.pyi` files to
+`libs/site-packages/motor`. Currently, only the stubs for [AsyncIO] are supported. You can contribute to stubs for
+[Tornado] by opening a pull request for the same.
+
+**Note:** This project is currently under development and is in no way affiliated with MongoDB. This is an unofficial
+stub package.
+
+How to use?
+-----------
+
+You can either install from [PyPI] using [pip] or add files to your project directories manually.
+
+### Installing Using [pip]:
+```commandline
+pip install motor-types
+```
+
+### To install [Motor] (and [Dnspython]) alongside the package:
+```commandline
+pip install motor-types[motor]
+```
+
+### To add files to the project manually:
+Use this command to clone the repository:
+```commandline
+git clone "https://github.com/L0RD-ZER0/Motor-Types"
+```
+
+Afterwards, you can do either of the following to use stubs:
+* Copy the stubs manually to either ``libs/site-packages/motor`` or ``libs/site-packages/motor-stubs``, ideally the latter.
+* Add these stubs manually to project directories.
+  * [For MyPy][MyPy-Stubs].
+  * [For PyCharm][PyCharm-Stubs].
+  * For other static type-checking tools, consider referring to their corresponding documentation regarding stubs.
+
+Examples:
+---------
+### Auto-Complete Example
+**Without Stubs:**
+
+![ACNS]
+
+**With Stubs:**
+
+![ACWS]
+
+### Type-Checking Example
+**Without Stubs:**
+
+![TCNS]
+
+**With Stubs:**
+
+![TCWS]
+
+Dependencies
+------------
+This package uses following dependencies:
+* [Poetry] (For Packaging and Publishing)
+* [PyMongo] (For PyMongo related types)
+* [Motor] (For Referencing and for motor installation extra)
+* [Dnspython] (For motor installation extra)
+* [Pre-Commit] (For maintaining code quality)
+* [Typing-Extensions] (For using the latest typing features)
+
+How to Contribute?
+------------------
+The simplest contribution you can make is by opening a [GitHub Issue][GH-Issues] or by forking the repository and making
+a pull request on the [GitHub Repository][GH-Repo] for the same. The changes can be as simple as improving the
+documentation or as big as completing any incomplete section of the typings.
+
+**Note:** All issues and pull-requests are subjected to a preliminary inspection.
+
+License
+-------
+This repository is licensed under MIT License. The [license][License] can be found within the repository.
+
+
+[Motor]: https://github.com/mongodb/motor
+[MongoDB]: https://www.mongodb.com
+[PyMongo]: https://github.com/mongodb/mongo-python-driver
+[Poetry]: https://github.com/python-poetry/poetry
+[pip]: https://pypi.org/project/pip/
+[Dnspython]: https://www.dnspython.org/
+[Pre-Commit]: https://pre-commit.com
+[Typing-Extensions]: https://github.com/python/typing_extensions
+[Python]: https://python.org
+[Tornado]: https://www.tornadoweb.org/
+[Asyncio]: https://docs.python.org/3/library/asyncio.html
+[PyPI]: https://pypi.org/
+[MyPy-Stubs]: https://mypy.readthedocs.io/en/stable/stubs.html#stub-files
+[PyCharm-Stubs]: https://www.jetbrains.com/help/pycharm/stubs.html
+[GH-Repo]: https://github.com/L0RD-ZER0/Motor-Types
+[GH-Issues]: https://github.com/L0RD-ZER0/Motor-Types/issues
+[License]: https://github.com/L0RD-ZER0/Motor-Types/blob/master/LICENSE
+[ACNS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/auto-complete-example-ns.png
+[ACWS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/auto-complete-example-ws.png
+[TCNS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/type-checking-example-ns.png
+[TCWS]: https://github.com/L0RD-ZER0/Motor-Types/raw/master/examples/type-checking-example-ws.png
```

