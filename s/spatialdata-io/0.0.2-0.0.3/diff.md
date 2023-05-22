# Comparing `tmp/spatialdata_io-0.0.2.tar.gz` & `tmp/spatialdata_io-0.0.3.tar.gz`

## Comparing `spatialdata_io-0.0.2.tar` & `spatialdata_io-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.codecov.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.mypy.ini
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/_version.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/Makefile
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/changelog.md
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/contributing.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/references.md
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/extensions/.gitkeep
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/_constants/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/_constants/_constants.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/_constants/_enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/__init__.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/cosmx.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/mcmicro.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/metaspace.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/resolve.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/steinbock.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/visium.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/xenium.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/_utils/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/_utils/_read_10x_h5.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/src/spatialdata_io/readers/_utils/_utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/tests/test_basic.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/LICENSE
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 spatialdata_io-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.codecov.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.mypy.ini
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/_version.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/changelog.md
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/references.md
+-rw-r--r--   0        0        0    16386 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/extensions/.gitkeep
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/_constants.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/_constants/_enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/__init__.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/cosmx.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/mcmicro.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/metaspace.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/resolve.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/steinbock.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/visium.py
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/xenium.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_read_10x_h5.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/tests/test_basic.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 spatialdata_io-0.0.3/PKG-INFO
```

### Comparing `spatialdata_io-0.0.2/.flake8` & `spatialdata_io-0.0.3/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/.mypy.ini` & `spatialdata_io-0.0.3/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/.pre-commit-config.yaml` & `spatialdata_io-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/.github/workflows/build.yaml` & `spatialdata_io-0.0.3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/.github/workflows/test_and_deploy.yaml` & `spatialdata_io-0.0.3/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/Makefile` & `spatialdata_io-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/conf.py` & `spatialdata_io-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/contributing.md` & `spatialdata_io-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/make.bat` & `spatialdata_io-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/references.bib` & `spatialdata_io-0.0.3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/template_usage.md` & `spatialdata_io-0.0.3/docs/template_usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Using this template
+# Developer guide
 
 Welcome to the developer guidelines! This document is split into two parts:
 
 1.  The [repository setup](#setting-up-the-repository). This section is relevant primarily for the repository maintainer and shows how to connect
     continuous integration services and documents initial set-up of the repository.
 2.  The [contributor guide](contributing.md#contributing-guide). It contains information relevant to all developers who want to make a contribution.
```

### Comparing `spatialdata_io-0.0.2/docs/_templates/autosummary/class.rst` & `spatialdata_io-0.0.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/docs/extensions/typed_returns.py` & `spatialdata_io-0.0.3/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/_docs.py` & `spatialdata_io-0.0.3/src/spatialdata_io/_docs.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/_constants/_constants.py` & `spatialdata_io-0.0.3/src/spatialdata_io/_constants/_constants.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/_constants/_enum.py` & `spatialdata_io-0.0.3/src/spatialdata_io/_constants/_enum.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/cosmx.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/cosmx.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/mcmicro.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/mcmicro.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/steinbock.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/steinbock.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/visium.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/visium.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/xenium.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/xenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         geo_df.index = idx
     scale = Scale([1.0 / specs["pixel_size"], 1.0 / specs["pixel_size"]], axes=("x", "y"))
     return ShapesModel.parse(geo_df, transformations={"global": scale})
 
 
 def _get_points(path: Path, specs: dict[str, Any]) -> Table:
     table = read_parquet(path / XeniumKeys.TRANSCRIPTS_FILE)
+    table["feature_name"] = table["feature_name"].apply(lambda x: x.decode("utf-8"), meta=("feature_name", "object"))
 
     transform = Scale([1.0 / specs["pixel_size"], 1.0 / specs["pixel_size"]], axes=("x", "y"))
     points = PointsModel.parse(
         table,
         coordinates={"x": XeniumKeys.TRANSCRIPTS_X, "y": XeniumKeys.TRANSCRIPTS_Y, "z": XeniumKeys.TRANSCRIPTS_Y},
         feature_key=XeniumKeys.FEATURE_NAME,
         instance_key=XeniumKeys.CELL_ID,
```

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/_utils/_read_10x_h5.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_read_10x_h5.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/src/spatialdata_io/readers/_utils/_utils.py` & `spatialdata_io-0.0.3/src/spatialdata_io/readers/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/LICENSE` & `spatialdata_io-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/pyproject.toml` & `spatialdata_io-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata_io-0.0.2/PKG-INFO` & `spatialdata_io-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata-io
-Version: 0.0.2
+Version: 0.0.3
 Summary: SpatialData IO for common techs
 Project-URL: Documentation, https://spatialdata-io.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-io
 Project-URL: Home-page, https://github.com/scverse/spatialdata-io
 Author: scverse
 Maintainer-email: scverse <scverse@scverse.scverse>
 License: BSD 3-Clause License
@@ -58,63 +58,65 @@
 Requires-Dist: sphinx>=4.5; extra == 'doc'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
-# spatialdata-io
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# spatialdata-io: convenient readers for loading common formats into SpatialData
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 
-[badge-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test.yaml/badge.svg
-[link-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test.yaml
+[badge-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml/badge.svg
+[link-tests]: https://github.com/scverse/spatialdata-io/actions/workflows/test_and_deploy.yaml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-io
 
-SpatialData IO for common technologies.
+This package contains reader functions to load common spatial omics formats into SpatialData. Currently, we provide support for:
+
+-   NanoString CosMx
+-   MCMICRO
+-   Steinbock
+-   10x Genomics Visium
+-   10x Genomics Xenium
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular, the
 
 -   [API documentation][link-api].
 
 ## Installation
 
 You need to have Python 3.8 or newer installed on your system. If you don't have
 Python installed, we recommend installing [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 
 There are several alternative options to install spatialdata-io:
 
-<!--
-1) Install the latest release of `spatialdata-io` from `PyPI <https://pypi.org/project/spatialdata-io/>`_:
+1. Install the latest release of `spatialdata-io` from [PyPI](https://pypi.org/project/spatialdata-io/):
 
 ```bash
 pip install spatialdata-io
 ```
--->
 
-1. Install the latest development version:
+2. Install the latest development version:
 
 ```bash
 pip install git+https://github.com/scverse/spatialdata-io.git@main
 ```
 
-## Release notes
-
-See the [changelog][changelog].
-
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+[L Marconato*, G Palla*, KA Yamauchi*, I Virshup*, E Heidari, T Treis, M Toth, R Shrestha, H Vöhringer, W Huber, M Gerstung, J Moore, FJ Theis, O Stegle, bioRxiv, 2023](https://www.biorxiv.org/content/10.1101/2023.05.05.539647v1). \* = equal contribution
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata-io/issues
 [changelog]: https://spatialdata-io.readthedocs.io/latest/changelog.html
 [link-docs]: https://spatialdata-io.readthedocs.io
 [link-api]: https://spatialdata-io.readthedocs.io/latest/api.html
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

