# Comparing `tmp/pytest_integration_mark-0.1.0.tar.gz` & `tmp/pytest_integration_mark-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_integration_mark-0.1.0.tar", max compression
+gzip compressed data, was "pytest_integration_mark-0.2.0.tar", max compression
```

## Comparing `pytest_integration_mark-0.1.0.tar` & `pytest_integration_mark-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2021-07-19 10:00:14.651570 pytest_integration_mark-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2122 2021-07-19 10:00:14.651570 pytest_integration_mark-0.1.0/README.md
--rwxr-xr-x   0        0        0      862 2021-07-19 10:00:14.651570 pytest_integration_mark-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2021-07-19 10:00:14.651570 pytest_integration_mark-0.1.0/pytest_integration_mark/__init__.py
--rwxr-xr-x   0        0        0     2340 2021-07-19 10:00:14.651570 pytest_integration_mark-0.1.0/pytest_integration_mark/hooks.py
--rw-r--r--   0        0        0     3083 2021-07-19 10:00:22.237233 pytest_integration_mark-0.1.0/setup.py
--rw-r--r--   0        0        0     3032 2021-07-19 10:00:22.237559 pytest_integration_mark-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 09:54:31.117523 pytest_integration_mark-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     2122 2023-05-22 09:54:31.117523 pytest_integration_mark-0.2.0/README.md
+-rwxr-xr-x   0        0        0      851 2023-05-22 09:54:31.117523 pytest_integration_mark-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-22 09:54:31.117523 pytest_integration_mark-0.2.0/pytest_integration_mark/__init__.py
+-rwxr-xr-x   0        0        0     2340 2023-05-22 09:54:31.117523 pytest_integration_mark-0.2.0/pytest_integration_mark/hooks.py
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 pytest_integration_mark-0.2.0/PKG-INFO
```

### Comparing `pytest_integration_mark-0.1.0/LICENSE` & `pytest_integration_mark-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_integration_mark-0.1.0/README.md` & `pytest_integration_mark-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_integration_mark-0.1.0/pyproject.toml` & `pytest_integration_mark-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_integration_mark"
-version = "0.1.0"
+version = "0.2.0"
 description = "Automatic integration test marking and excluding plugin for pytest"
 
 authors = ["Saulius Beinorius <saulius.beinorius@gmail.com>"]
 maintainers = ["Saulius Beinorius <saulius.beinorius@gmail.com>"]
 
 license = "Apache-2.0"
 readme = "README.md"
@@ -13,18 +13,18 @@
 repository = "https://github.com/Barbora-Data-Science/pytest-integration-mark"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pytest = ">=5.2,<7.0"
+pytest = ">=5.2"
 
 [tool.poetry.dev-dependencies]
-black = "^21.7b0"
+black = "*"
 
 [tool.poetry.plugins.pytest11]
 pytest_integration_mark = "pytest_integration_mark.hooks"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_integration_mark-0.1.0/pytest_integration_mark/hooks.py` & `pytest_integration_mark-0.2.0/pytest_integration_mark/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_integration_mark-0.1.0/setup.py` & `pytest_integration_mark-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,70 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-integration-mark
+Version: 0.2.0
+Summary: Automatic integration test marking and excluding plugin for pytest
+Home-page: https://github.com/Barbora-Data-Science/pytest-integration-mark
+License: Apache-2.0
+Author: Saulius Beinorius
+Author-email: saulius.beinorius@gmail.com
+Maintainer: Saulius Beinorius
+Maintainer-email: saulius.beinorius@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pytest (>=5.2)
+Project-URL: Repository, https://github.com/Barbora-Data-Science/pytest-integration-mark
+Description-Content-Type: text/markdown
+
+[![Formatter](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI version](https://badge.fury.io/py/pytest-integration-mark.svg)](https://pypi.org/project/pytest-integration-mark/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-integration-mark)](https://pypi.org/project/pytest-integration-mark/)
+
+
+# Description
+Provides a pytest marker `integration` for integration tests. 
+This marker automatically applies to all tests in a specified integration test folder.
+Integration tests will not run by default, which is useful for cases where an external dependency
+needs to be set up first (such as a database service).
+
+# Installation
+
+This is a pure python package, so it can be installed with `pip install pytest-integration-mark` 
+or any other dependency manager.
+
+# Usage
+
+After installation:
+
+Running `pytest` as usual:
+- Tests marked with `@pytest.mark.integration` will be skipped
+- Tests in `./tests/integration/...` will be skipped
+
+Running `pytest --with-integration`:
+- Tests marked with `@pytest.mark.integration` will run
+- Tests in `./tests/integration/...` will run
+
+Running `pytest --with-integration --integration-tests-folder integration`:
+- Tests marked with `@pytest.mark.integration` will run
+- Tests in `./integration/...` will run
+
+# Development
+
+This library uses the [poetry](https://python-poetry.org/) package manager, which has to be installed before installing
+other dependencies. Afterwards, run `poetry install` to create a virtualenv and install all dependencies.
+To then activate that environment, use `poetry shell`. To run a command in the environment without activating it,
+use `poetry run <command>`.
 
-packages = \
-['pytest_integration_mark']
+[Black](https://github.com/psf/black) is used (and enforced via workflows) to format all code. Poetry will install it
+automatically, but running it is up to the user. To format the entire project, run `black .` inside the virtualenv.
 
-package_data = \
-{'': ['*']}
+# Contributing
 
-install_requires = \
-['pytest>=5.2,<7.0']
-
-entry_points = \
-{'pytest11': ['pytest_integration_mark = pytest_integration_mark.hooks']}
-
-setup_kwargs = {
-    'name': 'pytest-integration-mark',
-    'version': '0.1.0',
-    'description': 'Automatic integration test marking and excluding plugin for pytest',
-    'long_description': '[![Formatter](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/pytest-integration-mark.svg)](https://pypi.org/project/pytest-integration-mark/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-integration-mark)](https://pypi.org/project/pytest-integration-mark/)\n\n\n# Description\nProvides a pytest marker `integration` for integration tests. \nThis marker automatically applies to all tests in a specified integration test folder.\nIntegration tests will not run by default, which is useful for cases where an external dependency\nneeds to be set up first (such as a database service).\n\n# Installation\n\nThis is a pure python package, so it can be installed with `pip install pytest-integration-mark` \nor any other dependency manager.\n\n# Usage\n\nAfter installation:\n\nRunning `pytest` as usual:\n- Tests marked with `@pytest.mark.integration` will be skipped\n- Tests in `./tests/integration/...` will be skipped\n\nRunning `pytest --with-integration`:\n- Tests marked with `@pytest.mark.integration` will run\n- Tests in `./tests/integration/...` will run\n\nRunning `pytest --with-integration --integration-tests-folder integration`:\n- Tests marked with `@pytest.mark.integration` will run\n- Tests in `./integration/...` will run\n\n# Development\n\nThis library uses the [poetry](https://python-poetry.org/) package manager, which has to be installed before installing\nother dependencies. Afterwards, run `poetry install` to create a virtualenv and install all dependencies.\nTo then activate that environment, use `poetry shell`. To run a command in the environment without activating it,\nuse `poetry run <command>`.\n\n[Black](https://github.com/psf/black) is used (and enforced via workflows) to format all code. Poetry will install it\nautomatically, but running it is up to the user. To format the entire project, run `black .` inside the virtualenv.\n\n# Contributing\n\nThis project uses the Apache 2.0 license and is maintained by the data science team @ Barbora. All contribution are \nwelcome in the form of PRs or raised issues.\n',
-    'author': 'Saulius Beinorius',
-    'author_email': 'saulius.beinorius@gmail.com',
-    'maintainer': 'Saulius Beinorius',
-    'maintainer_email': 'saulius.beinorius@gmail.com',
-    'url': 'https://github.com/Barbora-Data-Science/pytest-integration-mark',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+This project uses the Apache 2.0 license and is maintained by the data science team @ Barbora. All contribution are 
+welcome in the form of PRs or raised issues.
 
-
-setup(**setup_kwargs)
```

