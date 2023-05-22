# Comparing `tmp/loopmon-1.0.0.tar.gz` & `tmp/loopmon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopmon-1.0.0.tar", max compression
+gzip compressed data, was "loopmon-1.0.1.tar", max compression
```

## Comparing `loopmon-1.0.0.tar` & `loopmon-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1071 2022-02-24 15:45:18.752100 loopmon-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     4176 2022-02-24 15:45:18.752100 loopmon-1.0.0/README.md
--rw-r--r--   0        0        0     2296 2022-02-24 15:45:18.752100 loopmon-1.0.0/loopmon/__init__.py
--rw-r--r--   0        0        0     7123 2022-02-24 15:45:18.752100 loopmon-1.0.0/loopmon/monitor.py
--rw-r--r--   0        0        0        0 2022-02-24 15:45:18.752100 loopmon-1.0.0/loopmon/py.typed
--rw-r--r--   0        0        0     2855 2022-02-24 15:45:18.752100 loopmon-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4944 2022-02-24 15:45:28.489793 loopmon-1.0.0/setup.py
--rw-r--r--   0        0        0     5773 2022-02-24 15:45:28.490213 loopmon-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-22 16:06:05.651411 loopmon-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4195 2023-05-22 16:06:05.651411 loopmon-1.0.1/README.md
+-rw-r--r--   0        0        0     2485 2023-05-22 16:06:05.651411 loopmon-1.0.1/loopmon/__init__.py
+-rw-r--r--   0        0        0     7101 2023-05-22 16:06:05.651411 loopmon-1.0.1/loopmon/monitor.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:06:05.651411 loopmon-1.0.1/loopmon/py.typed
+-rw-r--r--   0        0        0     2961 2023-05-22 16:06:05.651411 loopmon-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5792 1970-01-01 00:00:00.000000 loopmon-1.0.1/PKG-INFO
```

### Comparing `loopmon-1.0.0/LICENSE.txt` & `loopmon-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loopmon-1.0.0/README.md` & `loopmon-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [![Codecov](https://img.shields.io/codecov/c/gh/isac322/loopmon?style=flat-square&logo=codecov)](https://app.codecov.io/gh/isac322/loopmon)
 [![Dependabot Status](https://flat.badgen.net/github/dependabot/isac322/loopmon?icon=github)](https://github.com/isac322/loopmon/network/dependencies)
 [![PyPI](https://img.shields.io/pypi/v/loopmon?label=pypi&logo=pypi&style=flat-square)](https://pypi.org/project/loopmon/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/loopmon?style=flat-square&logo=pypi)](https://pypi.org/project/loopmon/)
 [![Python Version](https://img.shields.io/pypi/pyversions/loopmon.svg?style=flat-square&logo=python)](https://pypi.org/project/loopmon/)
 [![GitHub last commit (branch)](https://img.shields.io/github/last-commit/isac322/loopmon/master?logo=github&style=flat-square)](https://github.com/isac322/loopmon/commits/master)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/isac322/loopmon/CI/master?logo=github&style=flat-square)](https://github.com/isac322/loopmon/actions)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/isac322/loopmon/ci.yml?branch=master&logo=github&style=flat-square)](https://github.com/isac322/loopmon/actions)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 loopmon is a lightweight library that can detect throttling of event loops.
 For example, you can detect long-running coroutine or whether the blocking function is invoked inside the event loop.
 
 
 ## Usage
```

### Comparing `loopmon-1.0.0/loopmon/__init__.py` & `loopmon-1.0.1/loopmon/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Any, Optional, Type, TypeVar, cast, overload
+from collections.abc import Callable, Iterable
+from typing import Optional, TypeVar, overload
+
+from typing_extensions import ParamSpec
 
 from loopmon.monitor import Callback, EventLoopMonitor, SleepEventLoopMonitor
 
 _MT = TypeVar('_MT', bound=EventLoopMonitor)
+_MonCon = ParamSpec('_MonCon')
 
 __all__ = (
     'Callback',
     'EventLoopMonitor',
     'SleepEventLoopMonitor',
     'create',
 )
 
 
 @overload
 def create(
     loop: Optional[asyncio.AbstractEventLoop] = None,
-    monitor_cls: Type[SleepEventLoopMonitor] = SleepEventLoopMonitor,
-    *args: Any,
-    **kwargs: Any,
+    interval: float = ...,
+    callbacks: Iterable[Callback] = ...,
+    name: Optional[str] = ...,
 ) -> SleepEventLoopMonitor:
     pass
 
 
 @overload
 def create(
-    loop: Optional[asyncio.AbstractEventLoop],
-    monitor_cls: Type[_MT],
-    *args: Any,
-    **kwargs: Any,
+    loop: Optional[asyncio.AbstractEventLoop] = None,
+    monitor_cls: Callable[_MonCon, _MT] = ...,
+    *args: _MonCon.args,
+    **kwargs: _MonCon.kwargs,
 ) -> _MT:
     pass
 
 
 # https://github.com/python/mypy/issues/3737#issuecomment-465355737
-def create(  # type: ignore[no-untyped-def]
+def create(  # type: ignore[misc]
     loop: Optional[asyncio.AbstractEventLoop] = None,
-    monitor_cls=SleepEventLoopMonitor,
-    *args: Any,
-    **kwargs: Any,
+    monitor_cls: Callable[_MonCon, _MT] = SleepEventLoopMonitor,  # type: ignore[assignment]
+    *args: _MonCon.args,
+    **kwargs: _MonCon.kwargs,
 ) -> _MT:
     """
     Creates a monitor object that can monitor an event loop, installs it in a given event loop, and starts monitoring.
     This function just commands the installation and returns immediately. (doesn't block)
 
     If `monitor_cls` is not specified, `SleepEventLoopMonitor` is used,
     so parameters such as `interval` `callbacks` `name` can be specified as `kwargs`.
@@ -66,10 +70,10 @@
     If not specified, the currently running event loop is automatically selected.
     :param monitor_cls: The class of the monitor. If not specified, `SleepEventLoopMonitor` is used.
     :param args: Parameters to pass to the `monitor_cls` constructor
     :param kwargs: Parameters to pass to the `monitor_cls` constructor
     :return:
     """
 
-    mon = cast(Type[_MT], monitor_cls)(*args, **kwargs)
+    mon = monitor_cls(*args, **kwargs)
     mon.install_to_loop(loop)
     return mon
```

### Comparing `loopmon-1.0.0/loopmon/monitor.py` & `loopmon-1.0.1/loopmon/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import sys
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable
 from datetime import datetime, timezone
-from typing import NoReturn, Optional, Tuple
+from typing import Optional, Tuple
 
 from typing_extensions import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class Callback(Protocol):
     async def __call__(self, lag: float, tasks: int, data_at: datetime) -> None:
@@ -91,15 +91,15 @@
         """
         The Task name to use when installing the monitor into the event loop.
         Only supported on Python 3.8+.
         """
         return self._name
 
     @abstractmethod
-    async def start(self) -> NoReturn:
+    async def start(self) -> None:
         """
         A coroutine function to start monitoring.
         Since it is an infinite loop, it is generally not recommended to `await'.
         In general, it is recommended to use `install_to_loop`.
 
         If you want to run a monitor in the currently running event loop without `install_to_loop`,
         just add `asyncio.create_task(monitor.start())`.
@@ -157,24 +157,24 @@
 
         self._started = False
 
     @property
     def running(self) -> bool:
         return self._started
 
-    async def start(self) -> NoReturn:
+    async def start(self) -> None:
         if self.running:
             raise ValueError('This monitor already installed into (the given or other) loop')
 
         try:
             await self._start()
         except asyncio.CancelledError:
             await self.stop()
 
-    async def _start(self) -> NoReturn:
+    async def _start(self) -> None:
         self._started = True
         loop = asyncio.get_running_loop()
 
         while self.running:
             before = await asyncio.sleep(self.interval, result=loop.time())
             lag = loop.time() - before - self.interval
             tasks = len(asyncio.all_tasks(loop))
```

### Comparing `loopmon-1.0.0/pyproject.toml` & `loopmon-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loopmon"
-version = "1.0.0"
+version = "1.0.1"
 description = "Lightewight monitor library for asyncio.EventLoop"
 authors = ["Byeonghoon Yoo <bh322yoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["asyncio", "monitoring", "eventloop", "lag", "delay"]
 repository = "https://github.com/isac322/loopmon"
 classifiers = [
@@ -33,32 +33,33 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = ">=3.8"
 
-[tool.poetry.dev-dependencies]
-flake8-black = "^0.2.4"
-black = "^22.1.0"
-flake8 = "^4.0.1"
-pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
-mypy = "^0.931"
-pytest-mock = "^3.7.0"
-flake8-isort = "^4.1.1"
+[tool.poetry.group.dev.dependencies]
+flake8-black = "^0.3.6"
+black = "^23.3.0"
+flake8 = "^5.0.4"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+mypy = "^1.3.0"
+pytest-mock = "^3.10.0"
+flake8-isort = "^6.0.0"
 asyncmock = {version = "^0.4.2", python = "<3.8"}
+flake8-pyproject = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
-python_version = "3.10"
+python_version = "3.11"
 allow_redefinition = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_decorators = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 no_implicit_reexport = true
@@ -80,15 +81,15 @@
     "tests.*",
 ]
 ignore_errors = true
 
 
 [tool.black]
 line-length = 120
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 skip-string-normalization = true
 
 
 [tool.coverage.run]
 omit = ['*/__init__.py',]
 
 [tool.coverage.report]
@@ -107,7 +108,11 @@
 
 
 [tool.pytest.ini_options]
 python_files = 'test_*.py'
 
 [tool.isort]
 profile = 'black'
+
+[tool.flake8]
+max-line-length = 120
+extend-ignore = ['E203']
```

### Comparing `loopmon-1.0.0/PKG-INFO` & `loopmon-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopmon
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lightewight monitor library for asyncio.EventLoop
 Home-page: https://github.com/isac322/loopmon
 License: MIT
 Keywords: asyncio,monitoring,eventloop,lag,delay
 Author: Byeonghoon Yoo
 Author-email: bh322yoo@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -13,20 +13,20 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System
@@ -41,15 +41,15 @@
 
 [![Codecov](https://img.shields.io/codecov/c/gh/isac322/loopmon?style=flat-square&logo=codecov)](https://app.codecov.io/gh/isac322/loopmon)
 [![Dependabot Status](https://flat.badgen.net/github/dependabot/isac322/loopmon?icon=github)](https://github.com/isac322/loopmon/network/dependencies)
 [![PyPI](https://img.shields.io/pypi/v/loopmon?label=pypi&logo=pypi&style=flat-square)](https://pypi.org/project/loopmon/)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/loopmon?style=flat-square&logo=pypi)](https://pypi.org/project/loopmon/)
 [![Python Version](https://img.shields.io/pypi/pyversions/loopmon.svg?style=flat-square&logo=python)](https://pypi.org/project/loopmon/)
 [![GitHub last commit (branch)](https://img.shields.io/github/last-commit/isac322/loopmon/master?logo=github&style=flat-square)](https://github.com/isac322/loopmon/commits/master)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/isac322/loopmon/CI/master?logo=github&style=flat-square)](https://github.com/isac322/loopmon/actions)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/isac322/loopmon/ci.yml?branch=master&logo=github&style=flat-square)](https://github.com/isac322/loopmon/actions)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 loopmon is a lightweight library that can detect throttling of event loops.
 For example, you can detect long-running coroutine or whether the blocking function is invoked inside the event loop.
 
 
 ## Usage
```

