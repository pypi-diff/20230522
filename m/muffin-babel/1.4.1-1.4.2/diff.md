# Comparing `tmp/muffin_babel-1.4.1.tar.gz` & `tmp/muffin_babel-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_babel-1.4.1.tar", max compression
+gzip compressed data, was "muffin_babel-1.4.2.tar", max compression
```

## Comparing `muffin_babel-1.4.1.tar` & `muffin_babel-1.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4396 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/README.rst
--rw-r--r--   0        0        0    10310 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/muffin_babel/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/muffin_babel/py.typed
--rw-r--r--   0        0        0     2030 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 muffin_babel-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4396 2023-05-22 11:58:56.785161 muffin_babel-1.4.2/README.rst
+-rw-r--r--   0        0        0    10443 2023-05-22 11:58:56.785161 muffin_babel-1.4.2/muffin_babel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:58:56.785161 muffin_babel-1.4.2/muffin_babel/py.typed
+-rw-r--r--   0        0        0     2030 2023-05-22 11:58:56.785161 muffin_babel-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 muffin_babel-1.4.2/PKG-INFO
```

### Comparing `muffin_babel-1.4.1/README.rst` & `muffin_babel-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_babel-1.4.1/muffin_babel/__init__.py` & `muffin_babel-1.4.2/muffin_babel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, Optional, Tuple, TypeVar
 
 from asgi_babel import current_locale, select_locale_by_request
-from babel import Locale, support
+from babel import Locale, UnknownLocaleError, support
 from babel.messages.catalog import Catalog
 from babel.messages.extract import extract_from_dir
 from babel.messages.mofile import write_mo
 from babel.messages.pofile import read_po, write_po
 from muffin import Application, Request
 from muffin.plugins import BasePlugin
 
@@ -192,15 +192,19 @@
             locale = Locale.parse(self.cfg.default_locale, sep="-")
             current_locale.set(locale)
         return locale
 
     @current_locale.setter
     def current_locale(self, lang: str):
         """Set current locale."""
-        return current_locale.set(Locale.parse(lang, sep="-"))
+        try:
+            locale = Locale.parse(lang, sep="-")
+            return current_locale.set(locale)
+        except (UnknownLocaleError, ValueError):
+            return
 
     @contextmanager
     def locale_ctx(self, lang: str):
         """Update current locale as context manager."""
         old_locale = current_locale.get()
         self.current_locale = lang  # type: ignore[assignment]
         yield self
```

### Comparing `muffin_babel-1.4.1/pyproject.toml` & `muffin_babel-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-babel"
-version = "1.4.1"
+version = "1.4.2"
 description = "Localization support for the Muffin Framework"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["localization", "internationalization", "muffin", "babel", "asyncio", "trio", "asgi"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin_babel-1.4.1/PKG-INFO` & `muffin_babel-1.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-babel
-Version: 1.4.1
+Version: 1.4.2
 Summary: Localization support for the Muffin Framework
 Home-page: https://github.com/klen/muffin-babel
 License: MIT
 Keywords: localization,internationalization,muffin,babel,asyncio,trio,asgi
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: asgi-babel (>=0,<1)
 Requires-Dist: muffin (>=0,<1)
 Project-URL: Repository, https://github.com/klen/muffin-babel
 Description-Content-Type: text/x-rst
 
 Muffin-Babel
```

