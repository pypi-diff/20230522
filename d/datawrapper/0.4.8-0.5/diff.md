# Comparing `tmp/datawrapper-0.4.8.tar.gz` & `tmp/datawrapper-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawrapper-0.4.8.tar", max compression
+gzip compressed data, was "datawrapper-0.5.tar", last modified: Mon May 22 17:33:01 2023, max compression
```

## Comparing `datawrapper-0.4.8.tar` & `datawrapper-0.5.tar`

### file list

```diff
@@ -1,7 +1,57 @@
--rw-r--r--   0        0        0     1093 2023-04-06 18:22:11.305264 datawrapper-0.4.8/LICENSE
--rw-r--r--   0        0        0    10131 2023-04-06 18:22:11.309264 datawrapper-0.4.8/README.md
--rw-r--r--   0        0        0      540 2023-04-06 18:22:11.309264 datawrapper-0.4.8/datawrapper/__init__.py
--rw-r--r--   0        0        0    22985 2023-04-06 18:22:11.309264 datawrapper-0.4.8/datawrapper/__main__.py
--rw-r--r--   0        0        0      362 2023-04-06 18:22:11.309264 datawrapper-0.4.8/datawrapper/example.py
--rw-r--r--   0        0        0     3538 2023-04-06 18:22:11.313264 datawrapper-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    11309 1970-01-01 00:00:00.000000 datawrapper-0.4.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 17:32:44.000000 datawrapper-0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/.stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-22 17:32:44.000000 datawrapper-0.5/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-22 17:32:44.000000 datawrapper-0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 17:32:44.000000 datawrapper-0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-22 17:32:44.000000 datawrapper-0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-22 17:32:44.000000 datawrapper-0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-22 17:32:44.000000 datawrapper-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-22 17:33:01.102587 datawrapper-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 17:32:44.000000 datawrapper-0.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    66724 2023-05-22 17:32:44.000000 datawrapper-0.5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-22 17:32:44.000000 datawrapper-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-22 17:32:44.000000 datawrapper-0.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23015 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 17:32:44.000000 datawrapper-0.5/datawrapper/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.098587 datawrapper-0.5/datawrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:33:01.000000 datawrapper-0.5/datawrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/_templates/class.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/about/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21532 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/static/datawrapper_logo_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/static/datawrapper_logo_light_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/user-guide/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   117469 2023-05-22 17:32:44.000000 datawrapper-0.5/docs/user-guide/usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:33:01.102587 datawrapper-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-22 17:32:44.000000 datawrapper-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.094586 datawrapper-0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:33:01.102587 datawrapper-0.5/tests/test_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 17:32:44.000000 datawrapper-0.5/tests/test_example/test_hello.py
```

### Comparing `datawrapper-0.4.8/LICENSE` & `datawrapper-0.5/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
  The MIT License (MIT)
  Copyright (c) 2021 chekos
- 
+
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
- 
+
  The above copyright notice and this permission notice shall be included in all
  copies or substantial portions of the Software.
- 
+
  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
  EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
  OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `datawrapper-0.4.8/datawrapper/__init__.py` & `datawrapper-0.5/datawrapper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# type: ignore[attr-defined]
 """A light-weight python wrapper for the Datawrapper API (v3). While it is not developed by Datawrapper officially, you can use it with your API credentials from datawrapper.de"""
 
 try:
-    from importlib.metadata import PackageNotFoundError, version
+    from importlib.metadata import PackageNotFoundError, version  # type: ignore
 except ImportError:  # pragma: no cover
-    from importlib_metadata import PackageNotFoundError, version
+    from importlib_metadata import PackageNotFoundError, version  # type: ignore
 
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 
 from .__main__ import Datawrapper
+
+__all__ = ["Datawrapper"]
```

### Comparing `datawrapper-0.4.8/datawrapper/__main__.py` & `datawrapper-0.5/datawrapper/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 
         Typical usage example:
 
         dw = Datawrapper(access_token = <YOUR_ACCESS_TOKEN_HERE>)
 
         dw.account_info()
 """
-from typing import Any, Dict, Iterable, List, Optional, Union
-
 import json
 import logging
 import os
 from pathlib import Path
+from typing import Any, Dict, Iterable, List, Optional, Union
 
 import IPython
 import pandas as pd
 import requests as r
 from IPython.display import HTML, Image
 
 logger = logging.getLogger(__name__)
@@ -41,14 +40,15 @@
     _PUBLISH_URL = _BASE_URL + "/charts"
     _FOLDERS_URL = _BASE_URL + "/folders"
 
     _ACCESS_TOKEN = os.getenv("DATAWRAPPER_ACCESS_TOKEN")
 
     def __init__(self, access_token=_ACCESS_TOKEN):
         """To create a token head to app.datawrapper.de/account/api-tokens.
+
         By default this will look for DATAWRAPPER_ACCESS_TOKEN environment variable.
 
         Parameters
         ----------
         access_token : [type], optional
             [description], by default _ACCESS_TOKEN
         """
@@ -128,15 +128,17 @@
         title: str = "New Chart",
         chart_type: str = "d3-bars-stacked",
         data: Union[pd.DataFrame, None] = None,
         folder_id: str = "",
         metadata: Optional[Dict[Any, Any]] = None,
     ) -> Union[Dict[Any, Any], None, Any]:
         """Creates a new Datawrapper chart, table or map.
+
         You can pass a pandas DataFrame as a `data` argument to upload data.
+
         Returns the created chart's information.
 
         Parameters
         ----------
         title : str, optional
             Title for new chart, table or map, by default "New Chart"
         chart_type : str, optional
@@ -321,14 +323,15 @@
             )
             return None
 
     def update_metadata(
         self, chart_id: str, properties: Dict[Any, Any]
     ) -> Union[Any, None]:
         """Update a chart, table, or map's metadata.
+
         Example: https://developer.datawrapper.de/docs/creating-a-chart-new#edit-colors
 
         Parameters
         ----------
         chart_id : str
             ID of chart, table, or map.
         properties : dict
@@ -532,14 +535,15 @@
         if export_chart_response.status_code == 200:
             with open(_filepath, "wb") as response:
                 response.write(export_chart_response.content)
             if display:
                 return Image(_filepath)
             else:
                 logger.debug(f"File exported at {_filepath}")
+                return None
         elif export_chart_response.status_code == 403:
             msg = "You don't have access to the requested chart."
             logger.error(msg)
             raise Exception(msg)
         elif export_chart_response.status_code == 401:
             msg = "You couldn't be authenticated."
             logger.error(msg)
@@ -597,15 +601,14 @@
         else:
             logger.error("Chart could not be moved at the moment.")
         return None
 
     def delete_chart(self, chart_id: str) -> r.Response.content:  # type: ignore
         """Deletes a specified chart, table or map.
 
-
         Parameters
         ----------
         chart_id : str
             ID of chart, table, or map.
 
         Returns
         -------
```

