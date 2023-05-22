# Comparing `tmp/geneagrapher_core-0.1.0.tar.gz` & `tmp/geneagrapher_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneagrapher_core-0.1.0.tar", max compression
+gzip compressed data, was "geneagrapher_core-0.1.1.tar", max compression
```

## Comparing `geneagrapher_core-0.1.0.tar` & `geneagrapher_core-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-02-21 09:11:38.849157 geneagrapher_core-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     2223 2023-02-19 20:15:31.788168 geneagrapher_core-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-28 06:21:14.741358 geneagrapher_core-0.1.0/geneagrapher_core/__init__.py
--rw-r--r--   0        0        0        0 2023-02-15 21:52:31.275363 geneagrapher_core-0.1.0/geneagrapher_core/py.typed
--rw-r--r--   0        0        0     6596 2023-03-02 07:18:55.082251 geneagrapher_core-0.1.0/geneagrapher_core/record.py
--rw-r--r--   0        0        0     8962 2023-04-07 08:37:20.426689 geneagrapher_core-0.1.0/geneagrapher_core/traverse.py
--rw-r--r--   0        0        0     1061 2023-04-07 23:25:32.581626 geneagrapher_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 geneagrapher_core-0.1.0/setup.py
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 geneagrapher_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-21 09:11:38.849157 geneagrapher_core-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2223 2023-02-19 20:15:31.788168 geneagrapher_core-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-01-28 06:21:14.741358 geneagrapher_core-0.1.1/geneagrapher_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-15 21:52:31.275363 geneagrapher_core-0.1.1/geneagrapher_core/py.typed
+-rw-r--r--   0        0        0     6789 2023-05-22 17:55:02.989239 geneagrapher_core-0.1.1/geneagrapher_core/record.py
+-rw-r--r--   0        0        0     8962 2023-04-07 08:37:20.426689 geneagrapher_core-0.1.1/geneagrapher_core/traverse.py
+-rw-r--r--   0        0        0     1061 2023-05-22 17:55:02.989863 geneagrapher_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 geneagrapher_core-0.1.1/setup.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 geneagrapher_core-0.1.1/PKG-INFO
```

### Comparing `geneagrapher_core-0.1.0/LICENSE.md` & `geneagrapher_core-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geneagrapher_core-0.1.0/README.md` & `geneagrapher_core-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geneagrapher_core-0.1.0/geneagrapher_core/record.py` & `geneagrapher_core-0.1.1/geneagrapher_core/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,16 +196,20 @@
     else:
         return []
 
 
 def get_advisors(soup: BeautifulSoup) -> List[int]:
     """Return the set of advisors.
 
-    Rarely, a record has multiple groups of advisors (e.g.,
-    https://www.mathgenealogy.org/id.php?id=17864). In this case,
-    capture all of the advisors from all groups..
+    Rarely:
+      - A record has multiple groups of advisors (e.g.,
+        https://www.mathgenealogy.org/id.php?id=17864). In this case,
+        capture all of the advisors from all groups.
+      - A record has promotors and co-promotors (e.g.,
+        https://www.mathgenealogy.org/id.php?id=51506). Capture
+        promotors and co-promotors as advisors.
     """
     return [
         extract_id(info.find_next())
-        for info in soup.find_all(string=re.compile("Advisor"))
+        for info in soup.find_all(string=re.compile("(Advisor|Promotor)"))
         if "Advisor: Unknown" not in info
     ]
```

### Comparing `geneagrapher_core-0.1.0/geneagrapher_core/traverse.py` & `geneagrapher_core-0.1.1/geneagrapher_core/traverse.py`

 * *Files identical despite different names*

### Comparing `geneagrapher_core-0.1.0/pyproject.toml` & `geneagrapher_core-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneagrapher-core"
-version = "0.1.0"
+version = "0.1.1"
 description = "Functions for getting records and building graphs from the Math Genealogy Project."
 license = "MIT"
 authors = ["David Alber <alber.david@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/davidalber/geneagrapher-core"
 packages = [{include = "geneagrapher_core"}]
```

### Comparing `geneagrapher_core-0.1.0/setup.py` & `geneagrapher_core-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['aiodns>=3.0.0,<4.0.0',
  'aiohttp>=3.8.3,<4.0.0',
  'beautifulsoup4>=4.11.1,<5.0.0',
  'types-beautifulsoup4>=4.11.6.4,<5.0.0.0']
 
 setup_kwargs = {
     'name': 'geneagrapher-core',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Functions for getting records and building graphs from the Math Genealogy Project.',
     'long_description': "# geneagrapher-core [![Continuous Integration Status](https://github.com/davidalber/geneagrapher-core/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/davidalber/geneagrapher-core/actions/workflows/ci.yaml/badge.svg?branch=main) [![Live Tests Status](https://github.com/davidalber/geneagrapher-core/actions/workflows/live-tests.yaml/badge.svg?branch=main)](https://github.com/davidalber/geneagrapher-core/actions/workflows/live-tests.yaml/badge.svg?branch=main) [![Documentation Status](https://readthedocs.org/projects/geneagrapher-core/badge/?version=latest)](https://geneagrapher-core.readthedocs.io/en/latest/?badge=latest)\n\n## Overview\nGeneagrapher is a tool for extracting information from the\n[Mathematics Genealogy Project](https://www.mathgenealogy.org/) to\nform a math family tree, where connections are between advisors and\ntheir students.\n\nThis package contains the core data-grabbing and manipulation\nfunctions needed to build a math family tree. The functionality here\nis low level and intended to support the development of other\ntools. If you just want to build a geneagraph, take a look at\n[Geneagrapher](https://github.com/davidalber/geneagrapher). If you\nwant to get mathematician records and use them in code, then this\nproject may be useful to you.\n\n## Documentation\nDocumentation about how to call into this package's functions can be\nfound at http://geneagrapher-core.readthedocs.io/.\n\n## Development\nDependencies in this package are managed by\n[Poetry](https://python-poetry.org/). Thus, your Python environment\nwill need Poetry installed. Install all dependencies with:\n\n```sh\n$ poetry install\n```\n\nSeveral development commands are runnable with `make`:\n- `make fmt` (also `make black` and `make format`) formats code using\n  black\n- `make format-check` runs black and reports if the code passes\n  formatting checks without making changes\n- `make lint` (also `make flake8` and `make flake`) does linting\n- `make mypy` (also `make types`) checks the code for typing violations\n- `make test` runs automated tests\n- `make check` does code formatting (checking, not modifying),\n  linting, type checking, and testing in one command; if this command\n  does not pass, CI will not pass\n",
     'author': 'David Alber',
     'author_email': 'alber.david@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/davidalber/geneagrapher-core',
```

### Comparing `geneagrapher_core-0.1.0/PKG-INFO` & `geneagrapher_core-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneagrapher-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions for getting records and building graphs from the Math Genealogy Project.
 Home-page: https://github.com/davidalber/geneagrapher-core
 License: MIT
 Author: David Alber
 Author-email: alber.david@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

