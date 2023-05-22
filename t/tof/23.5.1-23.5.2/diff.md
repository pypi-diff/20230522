# Comparing `tmp/tof-23.5.1.tar.gz` & `tmp/tof-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-23.5.1.tar", last modified: Sun May 14 07:53:46 2023, max compression
+gzip compressed data, was "tof-23.5.2.tar", last modified: Mon May 22 11:45:28 2023, max compression
```

## Comparing `tof-23.5.1.tar` & `tof-23.5.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.824364 tof-23.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-14 07:53:28.000000 tof-23.5.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.804363 tof-23.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-14 07:53:28.000000 tof-23.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-14 07:53:28.000000 tof-23.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-14 07:53:28.000000 tof-23.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-14 07:53:28.000000 tof-23.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 07:53:28.000000 tof-23.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-14 07:53:28.000000 tof-23.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-14 07:53:46.820363 tof-23.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-14 07:53:28.000000 tof-23.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-14 07:53:28.000000 tof-23.5.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.816363 tof-23.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.816363 tof-23.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/detector.png
--rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/model.png
--rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-05-14 07:53:28.000000 tof-23.5.1/docs/_static/pulse.png
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 07:53:28.000000 tof-23.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-14 07:53:28.000000 tof-23.5.1/docs/components.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-14 07:53:28.000000 tof-23.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-14 07:53:28.000000 tof-23.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-14 07:53:28.000000 tof-23.5.1/docs/pulses.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-14 07:53:28.000000 tof-23.5.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-14 07:53:28.000000 tof-23.5.1/docs/short-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 07:53:28.000000 tof-23.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.820363 tof-23.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 07:53:28.000000 tof-23.5.1/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:53:46.824364 tof-23.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.804363 tof-23.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/chopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof/facilities/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/facilities/ess_pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 07:53:28.000000 tof-23.5.1/src/tof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.812363 tof-23.5.1/src/tof.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-14 07:53:46.000000 tof-23.5.1/src/tof.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:53:46.820363 tof-23.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 07:53:28.000000 tof-23.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-14 07:53:28.000000 tof-23.5.1/tests/chopper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-14 07:53:28.000000 tof-23.5.1/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-14 07:53:28.000000 tof-23.5.1/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-14 07:53:28.000000 tof-23.5.1/tests/pulse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-14 07:53:28.000000 tof-23.5.1/tests/result_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 07:53:28.000000 tof-23.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-22 11:45:16.000000 tof-23.5.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.469793 tof-23.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-22 11:45:16.000000 tof-23.5.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-22 11:45:16.000000 tof-23.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 11:45:16.000000 tof-23.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 11:45:16.000000 tof-23.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 11:45:16.000000 tof-23.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-22 11:45:16.000000 tof-23.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-22 11:45:28.477793 tof-23.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-22 11:45:16.000000 tof-23.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-22 11:45:16.000000 tof-23.5.2/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/detector.png
+-rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    96012 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/model.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32531 2023-05-22 11:45:16.000000 tof-23.5.2/docs/_static/pulse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 11:45:16.000000 tof-23.5.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-22 11:45:16.000000 tof-23.5.2/docs/components.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-22 11:45:16.000000 tof-23.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 11:45:16.000000 tof-23.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-22 11:45:16.000000 tof-23.5.2/docs/multiple-pulses.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 11:45:16.000000 tof-23.5.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-22 11:45:16.000000 tof-23.5.2/docs/short-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-22 11:45:16.000000 tof-23.5.2/docs/sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 11:45:16.000000 tof-23.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 11:45:16.000000 tof-23.5.2/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:45:28.477793 tof-23.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.469793 tof-23.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof/facilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/facilities/ess_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-22 11:45:16.000000 tof-23.5.2/src/tof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.473793 tof-23.5.2/src/tof.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 11:45:28.000000 tof-23.5.2/src/tof.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:45:28.477793 tof-23.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 11:45:16.000000 tof-23.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-22 11:45:16.000000 tof-23.5.2/tests/chopper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 11:45:16.000000 tof-23.5.2/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-22 11:45:16.000000 tof-23.5.2/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-22 11:45:16.000000 tof-23.5.2/tests/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-22 11:45:16.000000 tof-23.5.2/tests/source_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-22 11:45:16.000000 tof-23.5.2/tox.ini
```

### Comparing `tof-23.5.1/.github/workflows/ci.yml` & `tof-23.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/.github/workflows/release.yml` & `tof-23.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/.pre-commit-config.yaml` & `tof-23.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/LICENSE` & `tof-23.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/PKG-INFO` & `tof-23.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.1
+Version: 23.5.2
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.5.1/README.md` & `tof-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/conda/meta.yaml` & `tof-23.5.2/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/_static/detector.png` & `tof-23.5.2/docs/_static/detector.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/_static/favicon.ico` & `tof-23.5.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/_static/logo.svg` & `tof-23.5.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/_static/model.png` & `tof-23.5.2/docs/_static/model.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/_static/pulse.png` & `tof-23.5.2/docs/_static/pulse.png`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/components.ipynb` & `tof-23.5.2/docs/components.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990162037037037%*

 * *Differences: {"'cells'": "{2: {'source': ['We begin by making a source pulse using the profile from ESS.']}, 3: "*

 * *            '{\'source\': ["source = tof.Source(facility=\'ess\', neutrons=1_000_000)\\n", '*

 * *            "'source.plot()']}, 5: {'source': {insert: [(3, 'model = tof.Model(source=source, "*

 * *            "detectors=[detector])\\n')], delete: [3]}}}"}*

```diff
@@ -28,26 +28,26 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0543c13d-847d-4642-8736-14a75ed5fd01",
             "metadata": {},
             "source": [
-                "We begin by making a pulse using the profile from ESS."
+                "We begin by making a source pulse using the profile from ESS."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "35b39244-c45b-4bdb-8138-7d0e56a40478",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse = tof.Pulse(facility='ess', neutrons=1_000_000)\n",
-                "pulse.plot()"
+                "source = tof.Source(facility='ess', neutrons=1_000_000)\n",
+                "source.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3c6ecb82-a47f-4f66-a067-9224e9d67be9",
             "metadata": {},
             "source": [
@@ -63,15 +63,15 @@
             "id": "e2ced2be-d642-4886-9281-37cd90102c31",
             "metadata": {},
             "outputs": [],
             "source": [
                 "detector = tof.Detector(distance=30.0 * meter)\n",
                 "\n",
                 "# Build the instrument model\n",
-                "model = tof.Model(pulse=pulse, detectors=[detector])\n",
+                "model = tof.Model(source=source, detectors=[detector])\n",
                 "model"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "75dd1359-d990-482c-b0d6-4a0ae094b0fc",
```

### Comparing `tof-23.5.1/docs/conf.py` & `tof-23.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/docs/index.rst` & `tof-23.5.2/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -28,11 +28,12 @@
    conda install -c conda-forge -c scipp tof
 
 .. toctree::
    :maxdepth: 2
    :hidden:
 
    short-example
-   pulses
+   sources
    components
+   multiple-pulses
    api
    Release notes <https://github.com/scipp/tof/releases>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 .. raw:: html
 [_static/logo.svg]
  .. role:: transparent :transparent:`Tof` ****************** A simple tool to
 create time-of-flight chopper cascade diagrams. Installation ============ You
 can install from ``pip`` using .. code-block:: sh pip install tof You can
 install from ``conda`` using .. code-block:: sh conda install -c conda-forge -
-c scipp tof .. toctree:: :maxdepth: 2 :hidden: short-example pulses components
-api Release notes
+c scipp tof .. toctree:: :maxdepth: 2 :hidden: short-example sources components
+multiple-pulses api Release notes
 github.com/scipp/tof/releases>
```

### Comparing `tof-23.5.1/docs/pulses.ipynb` & `tof-23.5.2/docs/sources.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9584880114326433%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Creating sources\\n'), (2, 'This notebook will "*

 * *            "illustrate how to create different kinds of neutron sources for the beamline.')], "*

 * *            'delete: [2, 0]}}, 1: {\'source\': {insert: [(4, "Hz = sc.Unit(\'Hz\')")], delete: [5, '*

 * *            "4]}}, 2: {'source': {insert: [(0, '## The ESS source\\n'), (2, 'Sources are "*

 * *            "characterized by five aspects:\\n'), (4, '- the number of neutrons in a pulse\\n'), "*

 * *            "(7, '- the pulse  […]*

```diff
@@ -1,78 +1,80 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "6b645603-12c0-4b3d-ab3c-529ad4f373e3",
             "metadata": {},
             "source": [
-                "# Creating pulses\n",
+                "# Creating sources\n",
                 "\n",
-                "This notebook will illustrate how to create different kinds of pulses for the beamline."
+                "This notebook will illustrate how to create different kinds of neutron sources for the beamline."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "899a245a-0ae7-45dd-b684-3b9d1c034cc6",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "import tof\n",
                 "\n",
-                "AA = sc.Unit('angstrom')\n",
-                "ms = sc.Unit('ms')"
+                "Hz = sc.Unit('Hz')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2294ac91-961b-4347-a1df-80662721fe49",
             "metadata": {},
             "source": [
-                "## The ESS pulse\n",
+                "## The ESS source\n",
                 "\n",
-                "Pulses are characterized by three aspects:\n",
+                "Sources are characterized by five aspects:\n",
                 "\n",
-                "- the number of neutrons in the pulse\n",
+                "- the number of neutrons in a pulse\n",
                 "- the time at which each neutron is born inside the pulse\n",
                 "- the wavelength of each neutron inside the pulse\n",
+                "- the pulse frequency (or repetition rate)\n",
+                "- the number of pulses\n",
                 "\n",
-                "The default way of creating pulses is to choose a facility name and a number of neutrons.\n",
-                "Each facility defines time and wavelength probability distributions for the neutrons."
+                "The default way of creating a source is to choose a facility name and a number of neutrons.\n",
+                "Each facility defines time and wavelength probability distributions for the neutrons, as well as a pulse frequency.\n",
+                "By default, a single pulse is generated."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1e356a02-0c4c-42b9-8115-6abe7741ad8d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse = tof.Pulse(facility='ess', neutrons=1_000_000)\n",
-                "pulse"
+                "source = tof.Source(facility='ess', neutrons=1_000_000)\n",
+                "source"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1bf9e593-fb94-4174-b4f1-7cab27b7cf49",
             "metadata": {},
             "source": [
-                "To inspect the data in the pulse, we can either look at its `birth_times` or `wavelengths` properties"
+                "To inspect the data in the pulse, we can either look at the source's `data` property"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "88514d20-4fcc-4b33-b428-708e5cb0b1a5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse.wavelengths"
+                "source.data"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "75969bc3-9d28-4aa0-9f0b-7a6eafb3ed93",
             "metadata": {},
             "source": [
@@ -82,51 +84,64 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "74b69926-a979-4f41-a4ad-128477a8eebf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse.plot()"
+                "source.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "78fc25ec-39f0-43fb-a324-b522e050485f",
             "metadata": {},
             "source": [
                 "## Specifying time and wavelength distributions\n",
                 "\n",
-                "It is also possible to create pulses with custom time and wavelength distributions.\n",
-                "For this, we need to use the `Pulse.from_distribution()` method.\n",
+                "It is also possible to create sources with custom time and wavelength distributions.\n",
+                "For this, we need to use the `Source.from_distribution()` method.\n",
                 "\n",
                 "### Flat distributions\n",
                 "\n",
-                "By default, the time and wavelength distributions of neutrons are both flat (uniform).\n",
-                "We then need to define a pulse duration (start and end times) and a wavelength range.\n",
+                "The `from_distribution` method require two arrays that define the time (`p_time`) and wavelength (`p_wav`) distributions for the neutrons in the pulse.\n",
+                "The array values represent the probabilities, while the associated coordinates represent the values to be sampled from.\n",
+                "\n",
+                "We first show how to create flat time and wavelength distributions.\n",
+                "\n",
                 "\n",
                 "To create a pulse with 1 million neutrons, uniformly distributed in the ranges of 1-3 ms for birth times,\n",
                 "and 1-10 \u00c5 for wavelengths, we write:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a2699065-309c-439c-bcda-bf15d20edd0b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse = tof.Pulse.from_distribution(\n",
+                "time = sc.array(dims=['time'], values=[1.0, 3.0], unit='ms')\n",
+                "p_time = sc.DataArray(\n",
+                "    data=sc.ones(sizes=time.sizes),\n",
+                "    coords={'time': time},\n",
+                ")\n",
+                "\n",
+                "wavelength = sc.array(dims=['wavelength'], values=[1.0, 10.0], unit='angstrom')\n",
+                "p_wav = sc.DataArray(\n",
+                "    data=sc.ones(sizes=wavelength.sizes),\n",
+                "    coords={'wavelength': wavelength},\n",
+                ")\n",
+                "\n",
+                "source = tof.Source.from_distribution(\n",
                 "    neutrons=1_000_000,\n",
-                "    tmin=1.0 * ms,\n",
-                "    tmax=3.0 * ms,\n",
-                "    wmin=1.0 * AA,\n",
-                "    wmax=10.0 * AA,\n",
+                "    p_time=p_time,\n",
+                "    p_wav=p_wav,\n",
                 ")\n",
-                "pulse.plot()"
+                "source.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "af4c567b-86bb-46a5-b8e5-7c8e829ce49d",
             "metadata": {},
             "source": [
@@ -156,21 +171,21 @@
                 "p_wav = sc.DataArray(\n",
                 "    data=sc.array(dims=['wavelength'], values=[1.0, 4.0]),\n",
                 "    coords={\n",
                 "        'wavelength': sc.array(dims=['wavelength'], values=[1.0, 4.0], unit='angstrom')\n",
                 "    },\n",
                 ")\n",
                 "\n",
-                "pulse = tof.Pulse.from_distribution(neutrons=200_000, p_time=p_time, p_wav=p_wav)\n",
-                "pulse.plot()"
+                "source = tof.Source.from_distribution(neutrons=200_000, p_time=p_time, p_wav=p_wav)\n",
+                "source.plot()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e735311e-f7a7-4f40-b6b8-73e6388d398e",
+            "id": "142ac37a-b456-4d97-9b8e-a27443de6d0a",
             "metadata": {},
             "source": [
                 "Note that the time and wavelength distributions are independent;\n",
                 "a neutron with a randomly selected birth time from `p_time` can adopt any wavelength in `p_wav`\n",
                 "(in other words, the two distributions are simply broadcast into a square 2D parameter space)."
             ]
         },
@@ -187,23 +202,83 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "43177e0c-652e-4665-a31c-1f7abf2897ee",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse = tof.Pulse.from_neutrons(\n",
-                "    birth_times=sc.array(\n",
-                "        dims=['event'],\n",
-                "        values=[0.0, 0.1, 0.2, 0.56],\n",
-                "        unit='s',\n",
-                "    ),\n",
-                "    wavelengths=sc.array(dims=['event'], values=[5.0, 8.0, 11.0, 7.1], unit='angstrom'),\n",
+                "birth_times = sc.array(\n",
+                "    dims=['event'],\n",
+                "    values=[0.0, 0.1, 0.2, 0.56],\n",
+                "    unit='ms',\n",
                 ")\n",
-                "pulse.plot()"
+                "wavelengths = sc.array(dims=['event'], values=[5.0, 8.0, 11.0, 7.1], unit='angstrom')\n",
+                "\n",
+                "source = tof.Source.from_neutrons(birth_times=birth_times, wavelengths=wavelengths)\n",
+                "source.plot()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8aece779-85f0-4662-97e2-9f64b8a2d562",
+            "metadata": {},
+            "source": [
+                "## Multiple pulses\n",
+                "\n",
+                "To make more than one pulse, use the `pulses` parameter:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "06baecce-dc05-4142-aed4-0c22b7d8a129",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tof.Source(facility='ess', neutrons=100_000, pulses=3).plot()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "560fb19b-4ead-4116-946c-c2ff682fe94c",
+            "metadata": {},
+            "source": [
+                "If a custom distribution is supplied, a frequency for the pulse repetition rate must be supplied:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "47610f5d-9cc3-46ab-a1ca-3b9961b44a7f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tof.Source.from_distribution(\n",
+                "    neutrons=200_000, p_time=p_time, p_wav=p_wav, pulses=2, frequency=100.0 * Hz\n",
+                ").plot()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "26e348c4-e053-46a6-aa5e-8d57bbbd0176",
+            "metadata": {},
+            "source": [
+                "If a source was created from individual neutrons, the same neutrons will be repeated in all the pulses:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "3b765974-fe8f-4694-b64f-cba13fae4c43",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "tof.Source.from_neutrons(\n",
+                "    birth_times=birth_times, wavelengths=wavelengths, pulses=3, frequency=500.0 * Hz\n",
+                ").plot()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `tof-23.5.1/docs/short-example.ipynb` & `tof-23.5.2/docs/short-example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959356398809524%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '## Create a source pulse\\n'), (2, 'We first create a "*

 * *            'source with one pulse containing 1 million neutrons whose distribution follows the '*

 * *            "ESS time and wavelength profiles (both thermal and cold neutrons are included).')], "*

 * *            'delete: [2, 0]}}, 3: {\'source\': ["source = tof.Source(facility=\'ess\', '*

 * *            'neutrons=1_000_000)\\n", \'source\']}, 4: {\'source\': [\'source.plot()\']}, 6: '*

 * *            "{'source': {insert: […]*

```diff
@@ -26,38 +26,38 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3890d24c-93ab-4faa-b653-c9208b5eba23",
             "metadata": {},
             "source": [
-                "## Create a pulse\n",
+                "## Create a source pulse\n",
                 "\n",
-                "We first create a pulse with 1M neutrons whose distribution follows the ESS time and wavelength profiles (both thermal and cold neutrons are included)."
+                "We first create a source with one pulse containing 1 million neutrons whose distribution follows the ESS time and wavelength profiles (both thermal and cold neutrons are included)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a2699065-309c-439c-bcda-bf15d20edd0b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse = tof.Pulse(facility='ess', neutrons=1_000_000)\n",
-                "pulse"
+                "source = tof.Source(facility='ess', neutrons=1_000_000)\n",
+                "source"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "49fec301-52a4-45a7-9438-b3f736e50b9f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pulse.plot()"
+                "source.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b5ffdab6-10cd-4719-8ff2-86e5e1d10571",
             "metadata": {},
             "source": [
@@ -140,20 +140,20 @@
                 "        distance=15.9 * meter,\n",
                 "        name=\"Frame-overlap 2\",\n",
                 "    ),\n",
                 "    tof.Chopper(\n",
                 "        frequency=7 * Hz,\n",
                 "        open=sc.array(\n",
                 "            dims=['cutout'],\n",
-                "            values=[30.],\n",
+                "            values=[30.0],\n",
                 "            unit='deg',\n",
                 "        ),\n",
                 "        close=sc.array(\n",
                 "            dims=['cutout'],\n",
-                "            values=[140.],\n",
+                "            values=[140.0],\n",
                 "            unit='deg',\n",
                 "        ),\n",
                 "        phase=0 * deg,\n",
                 "        distance=22 * meter,\n",
                 "        name=\"Pulse-overlap\",\n",
                 "    ),\n",
                 "]"
@@ -162,15 +162,15 @@
         {
             "cell_type": "markdown",
             "id": "bd6e1399-7f05-4d5c-83e3-7d249d9e0a61",
             "metadata": {},
             "source": [
                 "## Detector set-up\n",
                 "\n",
-                "We add a monitor 23m from the source, and a main detector 32m from the source."
+                "We add a monitor 26 meters from the source, and a main detector 32 meters from the source."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a377e75c-51a5-4994-af9c-92139d27bee3",
             "metadata": {},
@@ -185,26 +185,26 @@
         {
             "cell_type": "markdown",
             "id": "4c3b69b7-5ebe-4188-aa4b-2c6621ec8017",
             "metadata": {},
             "source": [
                 "## Run the model\n",
                 "\n",
-                "We combine the `pulse`, `choppers`, and `detectors` into our `model`,\n",
+                "We combine the `source`, `choppers`, and `detectors` into our `model`,\n",
                 "and then use the `.run()` method to execute the ray-tracing simulation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "05c191a2-81ef-41d3-8f64-343f72d7555d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "model = tof.Model(choppers=choppers, pulse=pulse, detectors=detectors)\n",
+                "model = tof.Model(source=source, choppers=choppers, detectors=detectors)\n",
                 "model"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9a2d019b-5c0d-4bf1-8b38-3ed18f6f687c",
@@ -262,15 +262,15 @@
             "cell_type": "markdown",
             "id": "3d2fbae9-1480-4a29-93ab-4d18a09dd64e",
             "metadata": {},
             "source": [
                 "### Data inspection\n",
                 "\n",
                 "Each component entry in the results objects holds all the information about the neutrons that reached that component.\n",
-                "The `.data` property of the object returns a data group"
+                "The `.data` property of the object returns a data array, which has one pulse of neutrons."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "72fce589-389d-4597-997c-9cde65a6f6be",
             "metadata": {},
@@ -319,25 +319,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "abc519bb-cb22-4169-97f2-2cc2be21ec48",
             "metadata": {},
             "source": [
-                "As these are Scipp data structures, they can be manipulated and plotted directly:"
+                "This is a data group that contains a single pulse.\n",
+                "\n",
+                "As these are Scipp data structures, they can be manipulated (e.g. histogrammed) and plotted directly."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "72e46653-6ea5-45aa-9ca9-cbdb7fa3c88c",
+            "id": "8009886a-b355-41f5-a3ae-2a997bc613cb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "res.choppers['WFM1'].wavelengths.data.hist(wavelength=300).plot()"
+                "res.choppers['WFM1'].wavelengths.visible.data.hist(wavelength=500).plot()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `tof-23.5.1/pyproject.toml` & `tof-23.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/requirements/ci.txt` & `tof-23.5.2/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/requirements/docs.txt` & `tof-23.5.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/requirements/static.txt` & `tof-23.5.2/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/src/tof/chopper.py` & `tof-23.5.2/src/tof/chopper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import uuid
 from dataclasses import dataclass
-from typing import Tuple
+from typing import Optional, Tuple
 
 import scipp as sc
 
 from .component import Component, ComponentData
 from .utils import two_pi
 
 
@@ -56,35 +56,39 @@
     def omega(self) -> sc.Variable:
         """
         The angular velocity of the chopper.
         """
         return two_pi * self.frequency
 
     def open_close_times(
-        self, time_limit: sc.Variable
+        self, time_limit: sc.Variable, unit: Optional[str] = None
     ) -> Tuple[sc.Variable, sc.Variable]:
         """
         The times at which the chopper opens and closes.
 
         Parameters
         ----------
         time_limit:
             Determines how many rotations the chopper needs to perform to reach the time
             limit.
+        unit:
+            The unit of the returned times. If not specified, the unit of `time_limit`
+            is used.
         """
-        time_limit = time_limit.to(unit='s')
-        nrot = max(int(sc.ceil(time_limit * self.frequency).value), 1)
+        if unit is None:
+            unit = time_limit.unit
+        nrot = max(int(sc.ceil((time_limit * self.frequency).to(unit='')).value), 1)
         phases = sc.arange(uuid.uuid4().hex, nrot) * two_pi + self.phase.to(unit='rad')
         # Note that the order is important here: we need (phases + open/close) to get
         # the correct dimension order when we flatten below.
         open_times = (phases + self.open.to(unit='rad', copy=False)) / self.omega
         close_times = (phases + self.close.to(unit='rad', copy=False)) / self.omega
         return (
-            open_times.flatten(to=self.open.dim),
-            close_times.flatten(to=self.close.dim),
+            open_times.flatten(to=self.open.dim).to(unit=unit, copy=False),
+            close_times.flatten(to=self.close.dim).to(unit=unit, copy=False),
         )
 
     def __repr__(self) -> str:
         return (
             f"Chopper(name={self.name}, distance={self.distance:c}, "
             f"frequency={self.frequency:c}, phase={self.phase:c}, "
             f"cutouts={len(self.open)})"
@@ -111,30 +115,27 @@
     name: str
     frequency: sc.Variable
     open: sc.Variable
     close: sc.Variable
     phase: sc.Variable
     open_times: sc.Variable
     close_times: sc.Variable
+    data: sc.DataArray
     tofs: ComponentData
     wavelengths: ComponentData
     birth_times: ComponentData
     speeds: ComponentData
 
     def __repr__(self) -> str:
         out = f"Chopper: '{self.name}'\n"
         out += f"  distance: {self.distance:c}\n"
         out += f"  frequency: {self.frequency:c}\n"
         out += f"  phase: {self.phase:c}\n"
         out += f"  cutouts: {len(self.open)}\n"
-        for key, dim in {
-            'tofs': 'tof',
-            'wavelengths': 'wavelength',
-            'birth_times': 'time',
-            'speeds': 'speed',
-        }.items():
-            coord = getattr(self, key).visible.data.coords[dim]
-            out += f"  {key}: [{coord.min():c} - {coord.max():c}]\n"
+        out += "\n".join(
+            f"  {key}: {getattr(self, key)}"
+            for key in ('tofs', 'wavelengths', 'birth_times', 'speeds')
+        )
         return out
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `tof-23.5.1/src/tof/component.py` & `tof-23.5.2/src/tof/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 from dataclasses import dataclass
-from typing import Dict, Optional, Tuple, Union
+from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import plopp as pp
 import scipp as sc
 
 from .utils import Plot
 
@@ -21,54 +21,80 @@
     ----------
     data:
         The data to hold.
     dim:
         The dimension label of the data.
     """
 
-    data: sc.DataArray
+    data: sc.DataGroup
     dim: str
 
-    @property
-    def shape(self) -> Tuple[int]:
+    def __len__(self) -> int:
         """
-        The shape of the data.
+        The number of pulses in the data.
         """
-        return self.data.shape
+        return len(self.data)
 
-    @property
-    def sizes(self) -> Dict[str, int]:
-        """
-        The sizes of the data.
+    def __getitem__(self, val: Union[int, slice]):
         """
-        return self.data.sizes
+        Get the data for a single pulse or a range of pulses.
 
-    def __len__(self) -> int:
-        """
-        The length of the data.
+        Parameters
+        ----------
+        val:
+            The index or slice of the pulse(s) to get.
         """
-        return len(self.data)
+        if isinstance(val, int):
+            val = slice(val, val + 1)
+        # Convert the slice to a list of indices, which can then be used to create
+        # DataGroup keys in the form 'pulse:0', 'pulse:1', etc.
+        inds = range(len(self))[val]
+        return self.__class__(
+            data=sc.DataGroup(
+                {f'pulse:{ind}': self.data[f'pulse:{ind}'] for ind in inds}
+            ),
+            dim=self.dim,
+        )
 
     def plot(self, bins: Union[int, sc.Variable] = 300, **kwargs):
         """
         Plot the neutrons that reach the component as a histogram.
 
         Parameters
         ----------
         bins:
             The bins to use for histogramming the neutrons.
         """
         return self.data.hist({self.dim: bins}).plot(**kwargs)
 
     def __repr__(self) -> str:
-        coord = self.data.coords[self.dim]
-        return (
-            f"Data(dim='{self.dim}', events={len(self)}, "
-            f"min={coord.min():c}, max={coord.max():c})"
-        )
+        out = f"Data(dim='{self.dim}')\n"
+        for name, da in self.data.items():
+            out += f"  {name}: events={len(da)}"
+            if len(da) > 0:
+                coord = da.coords[self.dim]
+                out += f", min={coord.min():c}, max={coord.max():c})"
+            out += "\n"
+        return out
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+
+def _field_to_string(field: Data) -> str:
+    if isinstance(field.data, sc.DataArray):
+        return str(len(field))
+    data = field.data
+    out = [str(len(data['pulse:0']))]
+    npulses = len(data)
+    if npulses > 2:
+        out.append('...')
+    if npulses > 1:
+        out.append(str(len(data[f'pulse:{npulses - 1}'])))
+    return '[' + ', '.join(out) + ']'
 
 
 @dataclass(frozen=True)
 class ComponentData:
     """
     A component data object contains the data (time-of-flight or wavelengths) for a
     component.
@@ -85,84 +111,98 @@
     blocking:
         A mask to apply to the data which will select the neutrons that are blocked by
         the component (this only defined in the case of a :class:`Chopper` component
         since a :class:`Detector` does not block any neutrons).
     """
 
     visible: Data
-    blocked: Optional[Data]
+    blocked: Optional[Data] = None
 
     @property
     def data(self) -> sc.DataGroup:
         """
         The neutrons that reach the component, split up into those that are blocked by
         the component and those that are not.
         """
         out = {'visible': self.visible.data}
         if self.blocked is not None:
             out['blocked'] = self.blocked.data
         return sc.DataGroup(out)
 
-    def __repr__(self) -> str:
-        return (
-            f"ComponentData(dim='{self.visible.dim}', visible={len(self.visible)}, "
-            f"blocked={len(self.blocked) if self.blocked is not None else None})"
+    def __getitem__(self, val):
+        return self.__class__(
+            visible=self.visible[val],
+            blocked=self.blocked[val] if self.blocked is not None else None,
         )
 
+    def _repr_string_body(self) -> str:
+        out = f"visible={_field_to_string(self.visible)}"
+        if self.blocked is not None:
+            out += f", blocked={_field_to_string(self.blocked)}"
+        return out
+
+    def __repr__(self) -> str:
+        return f"ComponentData(dim='{self.visible.dim}', {self._repr_string_body()})"
+
     def plot(self, bins: Union[int, sc.Variable] = 300, **kwargs):
         """
         Plot the data for the neutrons that reach the component, split up into those
         that are blocked by the component and those that are not.
 
         Parameters
         ----------
         bins:
             The bins to use for histogramming the neutrons.
         """
         if self.blocked is None:
             return self.visible.plot(bins=bins, **kwargs)
         visible = self.visible.data
         blocked = self.blocked.data
+        if isinstance(visible, sc.DataArray):
+            visible = sc.DataGroup({'onepulse': visible})
+            blocked = sc.DataGroup({'onepulse': blocked})
         dim = self.visible.dim
-        if isinstance(bins, int):
-            bins = sc.linspace(
-                dim=dim,
-                start=min(visible.coords[dim].min(), blocked.coords[dim].min()).value,
-                stop=max(visible.coords[dim].max(), blocked.coords[dim].max()).value,
-                num=bins,
-                unit=visible.coords[dim].unit,
+        to_plot = {}
+        colors = {}
+        edges = bins
+        for i, p in enumerate(visible):
+            if isinstance(bins, int):
+                edges = sc.linspace(
+                    dim=dim,
+                    start=min(
+                        visible[p].coords[dim].min(), blocked[p].coords[dim].min()
+                    ).value,
+                    stop=max(
+                        visible[p].coords[dim].max(), blocked[p].coords[dim].max()
+                    ).value,
+                    num=bins,
+                    unit=visible[p].coords[dim].unit,
+                )
+            vk = f'visible-{p}'
+            bk = f'blocked-{p}'
+            to_plot.update(
+                {vk: visible[p].hist({dim: edges}), bk: blocked[p].hist({dim: edges})}
             )
-        return pp.plot(
-            {
-                'visible': visible.hist({dim: bins}),
-                'blocked': blocked.hist({dim: bins}),
-            },
-            **{**{'color': {'blocked': 'gray'}}, **kwargs},
+            colors.update({vk: f'C{i}', bk: 'gray'})
+        out = pp.plot(
+            to_plot,
+            **{**{'color': colors}, **kwargs},
         )
+        # TODO: remove this once https://github.com/scipp/plopp/issues/206 is done.
+        out.ax.get_legend().remove()
+        return out
 
 
 class Component:
     """
     A component is placed in the beam path. After the model is run, the component
     will have a record of the arrival times and wavelengths of the neutrons that
     passed through it.
     """
 
-    @property
-    def data(self) -> sc.DataGroup:
-        """ """
-        return sc.DataGroup(
-            {
-                'tofs': self.tofs.data,
-                'wavelengths': self.wavelengths.data,
-                'birth_times': self.birth_times.data,
-                'speeds': self.speeds.data,
-            }
-        )
-
     def plot(self, bins: int = 300) -> Plot:
         """
         Plot both the tof and wavelength data side by side.
 
         Parameters
         ----------
         bins:
```

### Comparing `tof-23.5.1/src/tof/detector.py` & `tof-23.5.2/src/tof/detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,27 +36,24 @@
 class DetectorReading(Component):
     """
     Read-only container for the neutrons that reach the detector.
     """
 
     distance: sc.Variable
     name: str
+    data: sc.DataArray
     tofs: ComponentData
     wavelengths: ComponentData
     birth_times: ComponentData
     speeds: ComponentData
 
     def __repr__(self) -> str:
         out = f"Detector: '{self.name}'\n"
         out += f"  distance: {self.distance:c}\n"
-        for key, dim in {
-            'tofs': 'tof',
-            'wavelengths': 'wavelength',
-            'birth_times': 'time',
-            'speeds': 'speed',
-        }.items():
-            coord = getattr(self, key).visible.data.coords[dim]
-            out += f"  {key}: [{coord.min():c} - {coord.max():c}]\n"
+        out += "\n".join(
+            f"  {key}: {getattr(self, key)}"
+            for key in ('tofs', 'wavelengths', 'birth_times', 'speeds')
+        )
         return out
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `tof-23.5.1/src/tof/facilities/ess_pulse.py` & `tof-23.5.2/src/tof/facilities/ess_pulse.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,8 +636,9 @@
                     1.97044554e01,
                     1.99014851e01,
                 ],
                 unit='angstrom',
             )
         },
     ),
+    frequency=14.0 * sc.Unit('Hz'),
 )
```

### Comparing `tof-23.5.1/src/tof/model.py` & `tof-23.5.2/src/tof/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from itertools import chain
 from typing import Dict, List, Optional, Tuple, Union
 
 import scipp as sc
 
 from .chopper import Chopper
 from .detector import Detector
-from .pulse import Pulse
 from .result import Result
+from .source import Source
 
 ComponentType = Union[Chopper, Detector]
 
 
 def _input_to_dict(
     obj: Union[
         None,
@@ -39,37 +39,37 @@
             "or a list/tuple of Choppers or Detectors."
         )
 
 
 class Model:
     """
     A class that represents a neutron instrument.
-    It is defined by a list of choppers, a list of detectors, and a pulse.
+    It is defined by a list of choppers, a list of detectors, and a source.
 
     Parameters
     ----------
     choppers:
         A list of choppers.
     detectors:
         A list of detectors.
-    pulse:
-        A pulse of neutrons.
+    source:
+        A source of neutrons.
     """
 
     def __init__(
         self,
-        pulse: Pulse,
+        source: Source,
         choppers: Optional[Union[Chopper, List[Chopper], Tuple[Chopper, ...]]] = None,
         detectors: Optional[
             Union[Detector, List[Detector], Tuple[Detector, ...]]
         ] = None,
     ):
         self.choppers = _input_to_dict(choppers, kind=Chopper)
         self.detectors = _input_to_dict(detectors, kind=Detector)
-        self.pulse = pulse
+        self.source = source
 
     def add(self, component):
         """
         Add a component to the instrument.
         Component names must be unique across choppers and detectors.
 
         Parameters
@@ -116,70 +116,61 @@
         if name not in self:
             raise KeyError(f"No component with name {name} was found.")
         return self.choppers[name] if name in self.choppers else self.detectors[name]
 
     def __delitem__(self, name):
         self.remove(name)
 
-    def run(self, npulses: int = 1):
+    def run(self):
         """
         Run the simulation.
-
-        Parameters
-        ----------
-        npulses:
-            Number of pulses to simulate.
         """
-        # TODO: ray-trace multiple pulses
         components = sorted(
             chain(self.choppers.values(), self.detectors.values()),
             key=lambda c: c.distance.value,
         )
 
-        initial_mask = sc.ones(
-            sizes=self.pulse.birth_times.sizes, unit=None, dtype=bool
-        )
+        birth_time = self.source.data.coords['time']
+        speed = self.source.data.coords['speed']
+        initial_mask = sc.ones(sizes=birth_time.sizes, unit=None, dtype=bool)
 
         result_choppers = {}
         result_detectors = {}
         time_limit = (
-            self.pulse.birth_times + components[-1].distance / self.pulse.speeds
+            birth_time + (components[-1].distance / speed).to(unit=birth_time.unit)
         ).max()
         for c in components:
             container = result_detectors if isinstance(c, Detector) else result_choppers
             container[c.name] = c.as_dict()
-            container[c.name].update(
-                {
-                    'birth_times': self.pulse.birth_times,
-                    'speeds': self.pulse.speeds,
-                    'wavelengths': self.pulse.wavelengths,
-                }
-            )
-            t = self.pulse.birth_times + c.distance / self.pulse.speeds
-            container[c.name]['arrival_times'] = t.to(unit='us')
+            container[c.name]['data'] = self.source.data.copy(deep=False)
+            t = birth_time + (c.distance / speed).to(unit=birth_time.unit, copy=False)
+            container[c.name]['data'].coords['tof'] = t
             if isinstance(c, Detector):
                 container[c.name]['visible_mask'] = initial_mask
+                container[c.name]['data'].masks['blocked_by_others'] = ~initial_mask
                 continue
             m = sc.zeros(sizes=t.sizes, unit=None, dtype=bool)
             to, tc = c.open_close_times(time_limit=time_limit)
             container[c.name].update({'open_times': to, 'close_times': tc})
             for i in range(len(to)):
                 m |= (t > to[i]) & (t < tc[i])
             combined = initial_mask & m
             container[c.name].update(
                 {'visible_mask': combined, 'blocked_mask': ~m & initial_mask}
             )
+            container[c.name]['data'].masks['blocked_by_others'] = ~initial_mask
+            container[c.name]['data'].masks['blocked_by_me'] = ~m & initial_mask
             initial_mask = combined
 
         return Result(
-            pulse=self.pulse, choppers=result_choppers, detectors=result_detectors
+            source=self.source, choppers=result_choppers, detectors=result_detectors
         )
 
     def __repr__(self) -> str:
-        out = f"Model:\n  Pulse: {self.pulse}\n  Choppers:\n"
+        out = f"Model:\n  Source: {self.source}\n  Choppers:\n"
         for name, ch in self.choppers.items():
             out += f"    {name}: {ch}\n"
         out += "  Detectors:\n"
         for name, det in self.detectors.items():
             out += f"    {name}: {det}\n"
         return out
```

### Comparing `tof-23.5.1/src/tof/result.py` & `tof-23.5.2/src/tof/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
+from functools import reduce
 from itertools import chain
 from types import MappingProxyType
-from typing import Dict, Optional, Union
+from typing import Dict, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipp as sc
 from matplotlib.collections import LineCollection
 
 from .chopper import Chopper, ChopperReading
 from .component import ComponentData, Data
 from .detector import Detector, DetectorReading
-from .pulse import Pulse, PulseParameters
+from .source import Source, SourceParameters
 from .utils import Plot
 
 
-def _make_data(array, dim):
-    return Data(
-        data=sc.DataArray(
-            data=sc.ones(sizes=array.sizes, unit='counts'), coords={dim: array}
-        ),
-        dim=dim,
-    )
-
-
-def _make_component_data(component, key, dim, blocked=False):
+def _make_component_data(component, dim, is_chopper=False):
+    visible = {}
+    blocked = {} if is_chopper else None
+    keep_dim = (set(component.dims) - {'pulse'}).pop()
+    for name, da in sc.collapse(component, keep=keep_dim).items():
+        one_mask = ~reduce(lambda a, b: a | b, da.masks.values())
+        vsel = da[one_mask]
+        visible[name] = sc.DataArray(data=vsel.data, coords={dim: vsel.coords[dim]})
+        if is_chopper:
+            bsel = da[da.masks['blocked_by_me']]
+            blocked[name] = sc.DataArray(data=bsel.data, coords={dim: bsel.coords[dim]})
     return ComponentData(
-        visible=_make_data(component[key][component['visible_mask']], dim=dim),
-        blocked=_make_data(component[key][component['blocked_mask']], dim=dim)
-        if blocked
-        else None,
+        visible=Data(data=sc.DataGroup(visible), dim=dim),
+        blocked=Data(data=sc.DataGroup(blocked), dim=dim) if is_chopper else None,
     )
 
 
 def _add_rays(
     ax: plt.Axes,
     tofs: sc.Variable,
     birth_times: sc.Variable,
     distances: sc.Variable,
     cbar: bool = True,
     wavelengths: Optional[sc.Variable] = None,
     wmin: Optional[sc.Variable] = None,
     wmax: Optional[sc.Variable] = None,
 ):
-    x0 = birth_times.to(unit='us', copy=False).values.reshape(-1, 1)
-    x1 = tofs.to(unit='us', copy=False).values.reshape(-1, 1)
+    x0 = birth_times.values.reshape(-1, 1)
+    x1 = tofs.values.reshape(-1, 1)
     y0 = np.zeros(x0.size).reshape(-1, 1)
     y1 = distances.values.reshape(-1, 1)
     segments = np.concatenate(
         (
             np.concatenate((x0, y0), axis=1).reshape(-1, 1, 2),
             np.concatenate((x1, y1), axis=1).reshape(-1, 1, 2),
         ),
@@ -58,80 +58,82 @@
     )
     coll = LineCollection(segments)
     if wavelengths is not None:
         coll.set_cmap(plt.cm.gist_rainbow_r)
         coll.set_array(wavelengths.values)
         coll.set_norm(plt.Normalize(wmin.value, wmax.value))
         if cbar:
-            cb = plt.colorbar(coll)
+            cb = plt.colorbar(coll, ax=ax)
             cb.ax.yaxis.set_label_coords(-0.9, 0.5)
             cb.set_label('Wavelength (Å)')
     else:
         coll.set_color('lightgray')
     ax.add_collection(coll)
 
 
 class Result:
     """
     Result of a simulation.
 
     Parameters
     ----------
-    pulse:
-        The pulse of neutrons.
+    source:
+        The source of neutrons.
     choppers:
         The choppers in the model.
     detectors:
         The detectors in the model.
     """
 
     def __init__(
         self,
-        pulse: Pulse,
+        source: Source,
         choppers: Dict[str, Chopper],
         detectors: Dict[str, Detector],
     ):
-        self._pulse = pulse.as_readonly()
+        self._source = source.as_readonly()
         self._masks = {}
         self._arrival_times = {}
         self._choppers = {}
         fields = {
-            'tofs': ('arrival_times', 'tof'),
-            'wavelengths': ('wavelengths', 'wavelength'),
-            'birth_times': ('birth_times', 'time'),
-            'speeds': ('speeds', 'speed'),
+            'tofs': 'tof',
+            'wavelengths': 'wavelength',
+            'birth_times': 'time',
+            'speeds': 'speed',
         }
         for name, chopper in choppers.items():
             self._masks[name] = chopper['visible_mask']
-            self._arrival_times[name] = chopper['arrival_times']
+            self._arrival_times[name] = chopper['data'].coords['tof']
             self._choppers[name] = ChopperReading(
                 distance=chopper['distance'],
                 name=chopper['name'],
                 frequency=chopper['frequency'],
                 open=chopper['open'],
                 close=chopper['close'],
                 phase=chopper['phase'],
                 open_times=chopper['open_times'],
                 close_times=chopper['close_times'],
+                data=chopper['data'],
                 **{
-                    key: _make_component_data(chopper, field, dim, blocked=True)
-                    for key, (field, dim) in fields.items()
+                    key: _make_component_data(chopper['data'], dim=dim, is_chopper=True)
+                    for key, dim in fields.items()
                 },
             )
 
         self._detectors = {}
         for name, det in detectors.items():
             self._masks[name] = det['visible_mask']
-            self._arrival_times[name] = det['arrival_times']
+            self._arrival_times[name] = det['data'].coords['tof']
             self._detectors[name] = DetectorReading(
                 distance=det['distance'],
                 name=det['name'],
+                data=det['data'],
                 **{
-                    key: _make_component_data(det, field, dim)
-                    for key, (field, dim) in fields.items()
+                    key: _make_component_data(det['data'], dim=dim)
+                    for key, dim in fields.items()
                 },
             )
 
         self._choppers = MappingProxyType(self._choppers)
         self._detectors = MappingProxyType(self._detectors)
         self._masks = MappingProxyType(self._masks)
         self._arrival_times = MappingProxyType(self._arrival_times)
@@ -143,33 +145,126 @@
 
     @property
     def detectors(self) -> MappingProxyType[str, DetectorReading]:
         """The detectors in the model."""
         return self._detectors
 
     @property
-    def pulse(self) -> PulseParameters:
-        """The pulse of neutrons."""
-        return self._pulse
+    def source(self) -> SourceParameters:
+        """The source of neutrons."""
+        return self._source
 
     def __iter__(self):
         return chain(self._choppers, self._detectors)
 
     def __getitem__(self, name: str) -> Union[ChopperReading, DetectorReading]:
         if name not in self:
             raise KeyError(f"No component with name {name} was found.")
         return self._choppers[name] if name in self._choppers else self._detectors[name]
 
+    def _plot_visible_rays(
+        self,
+        max_rays: int,
+        pulse_index: int,
+        furthest_detector: DetectorReading,
+        ax: plt.Axes,
+        cbar: bool,
+        wmin: sc.Variable,
+        wmax: sc.Variable,
+    ):
+        if max_rays <= 0:
+            return
+        da = furthest_detector.data['pulse', pulse_index]
+        visible = da[~da.masks['blocked_by_others']]
+        tofs = visible.coords['tof']
+        if (max_rays is not None) and (len(tofs) > max_rays):
+            inds = np.random.choice(len(tofs), size=max_rays, replace=False)
+        else:
+            inds = slice(None)
+        birth_times = visible.coords['time'][inds]
+        wavelengths = visible.coords['wavelength'][inds]
+        distances = furthest_detector.distance.broadcast(sizes=birth_times.sizes)
+        _add_rays(
+            ax=ax,
+            tofs=tofs[inds],
+            birth_times=birth_times,
+            distances=distances,
+            cbar=cbar,
+            wavelengths=wavelengths,
+            wmin=wmin,
+            wmax=wmax,
+        )
+
+    def _plot_blocked_rays(
+        self,
+        blocked_rays: int,
+        pulse_index: int,
+        furthest_detector: DetectorReading,
+        ax: plt.Axes,
+    ):
+        if blocked_rays <= 0:
+            return
+        slc = ('pulse', pulse_index)
+        inv_mask = ~self._masks[furthest_detector.name][slc]
+        nrays = int(inv_mask.sum())
+        if nrays > blocked_rays:
+            inds = np.random.choice(nrays, size=blocked_rays, replace=False)
+        else:
+            inds = slice(None)
+        birth_times = self._source.data.coords['time'][slc][inv_mask][inds]
+
+        components = sorted(
+            chain(self._choppers.values(), [furthest_detector]),
+            key=lambda c: c.distance.value,
+        )
+        dim = 'component'
+        tofs = sc.concat(
+            [
+                self._arrival_times[comp.name][slc][inv_mask][inds]
+                for comp in components
+            ],
+            dim=dim,
+        )
+        distances = sc.concat(
+            [comp.distance.broadcast(sizes=birth_times.sizes) for comp in components],
+            dim=dim,
+        )
+        masks = sc.concat(
+            [sc.ones(sizes=birth_times.sizes, dtype=bool)]
+            + [self._masks[comp.name][slc][inv_mask][inds] for comp in components],
+            dim=dim,
+        )
+
+        diff = sc.abs(masks[dim, 1:].to(dtype=int) - masks[dim, :-1].to(dtype=int))
+        diff.unit = ''
+        _add_rays(
+            ax=ax,
+            tofs=(tofs * diff).max(dim=dim),
+            birth_times=birth_times,
+            distances=(distances * diff).max(dim=dim),
+        )
+
+    def _plot_pulse(self, pulse_index: int, ax: plt.Axes):
+        time_coord = self.source.data.coords['time']['pulse', pulse_index]
+        tmin = time_coord.min().value
+        ax.plot(
+            [tmin, time_coord.max().value],
+            [0, 0],
+            color="gray",
+            lw=3,
+        )
+        ax.text(tmin, 0, "Pulse", ha="left", va="top", color="gray")
+
     def plot(
         self,
         max_rays: int = 1000,
         blocked_rays: int = 0,
-        figsize=None,
-        ax=None,
-        cbar=True,
+        figsize: Optional[Tuple[float, float]] = None,
+        ax: Optional[plt.Axes] = None,
+        cbar: bool = True,
     ) -> Plot:
         """
         Plot the time-distance diagram for the instrument, including the rays of
         neutrons that make it to the furthest detector.
         As plotting many lines can be slow, the number of rays to plot can be
         limited by setting ``max_rays``.
         In addition, it is possible to also plot the rays that are blocked by
@@ -189,86 +284,49 @@
             Show a colorbar for the wavelength if ``True``.
         """
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = ax.get_figure()
         furthest_detector = max(self._detectors.values(), key=lambda d: d.distance)
-
-        if blocked_rays > 0:
-            inv_mask = ~self._masks[furthest_detector.name]
-            nrays = int(inv_mask.sum())
-            if nrays > blocked_rays:
-                inds = np.random.choice(nrays, size=blocked_rays, replace=False)
-            else:
-                inds = slice(None)
-            birth_times = self.pulse.birth_times[inv_mask][inds]
-
-            components = sorted(
-                chain(self._choppers.values(), [furthest_detector]),
-                key=lambda c: c.distance.value,
-            )
-            dim = 'component'
-            tofs = sc.concat(
-                [self._arrival_times[comp.name][inv_mask][inds] for comp in components],
-                dim=dim,
-            )
-            distances = sc.concat(
-                [
-                    comp.distance.broadcast(sizes=birth_times.sizes)
-                    for comp in components
-                ],
-                dim=dim,
-            )
-            masks = sc.concat(
-                [sc.ones(sizes=birth_times.sizes, dtype=bool)]
-                + [self._masks[comp.name][inv_mask][inds] for comp in components],
-                dim=dim,
-            )
-
-            diff = sc.abs(masks[dim, 1:].to(dtype=int) - masks[dim, :-1].to(dtype=int))
-            diff.unit = ''
-            _add_rays(
+        wavelengths = sc.DataArray(
+            data=furthest_detector.data.coords['wavelength'],
+            masks=furthest_detector.data.masks,
+        )
+        for i in range(self._source.data.sizes['pulse']):
+            self._plot_blocked_rays(
+                blocked_rays=blocked_rays,
+                pulse_index=i,
+                furthest_detector=furthest_detector,
                 ax=ax,
-                tofs=(tofs * diff).max(dim=dim),
-                birth_times=birth_times,
-                distances=(distances * diff).max(dim=dim),
             )
-
-        # Normal rays
-        if max_rays > 0:
-            tofs = furthest_detector.tofs.visible.data.coords['tof']
-            if (max_rays is not None) and (len(tofs) > max_rays):
-                inds = np.random.choice(len(tofs), size=max_rays, replace=False)
-            else:
-                inds = slice(None)
-            birth_times = furthest_detector.birth_times.visible.data.coords['time'][
-                inds
-            ]
-            wavelengths = furthest_detector.wavelengths.visible.data.coords[
-                'wavelength'
-            ][inds]
-            distances = furthest_detector.distance.broadcast(sizes=birth_times.sizes)
-            _add_rays(
+            self._plot_visible_rays(
+                max_rays=max_rays,
+                pulse_index=i,
+                furthest_detector=furthest_detector,
                 ax=ax,
-                tofs=tofs[inds],
-                birth_times=birth_times,
-                distances=distances,
-                cbar=cbar,
-                wavelengths=wavelengths,
-                wmin=self._pulse.wmin,
-                wmax=self._pulse.wmax,
-            )
-
-        tof_max = tofs.max().value
+                cbar=cbar and (i == 0),
+                wmin=wavelengths.min(),
+                wmax=wavelengths.max(),
+            )
+            self._plot_pulse(pulse_index=i, ax=ax)
+
+        det_data = furthest_detector.tofs.visible.data
+        if len(det_data) == 1:
+            tof_max = det_data['pulse:0'].coords['tof'].max().value
+        else:
+            tof_max = reduce(
+                lambda a, b: max(a.max(), b.max()),
+                [da.coords['tof'] for da in det_data.values()],
+            ).value
         dx = 0.05 * tof_max
         # Plot choppers
         for ch in self._choppers.values():
-            x0 = ch.open_times.to(unit='us').values
-            x1 = ch.close_times.to(unit='us').values
+            x0 = ch.open_times.values
+            x1 = ch.close_times.values
             x = np.empty(3 * x0.size, dtype=x0.dtype)
             x[0::3] = x0
             x[1::3] = 0.5 * (x0 + x1)
             x[2::3] = x1
             x = np.concatenate([[0], x] + ([[tof_max + dx]] if x[-1] < tof_max else []))
             y = np.full_like(x, ch.distance.value)
             y[2::3] = None
@@ -280,38 +338,37 @@
         # Plot detectors
         for det in self._detectors.values():
             ax.plot([0, tof_max], [det.distance.value] * 2, color="gray", lw=3)
             ax.text(
                 0, det.distance.value, det.name, ha="left", va="bottom", color="gray"
             )
 
-        # Plot pulse
-        tmin = self.pulse.tmin.to(unit='us').value
-        ax.plot(
-            [tmin, self.pulse.tmax.to(unit='us').value],
-            [0, 0],
-            color="gray",
-            lw=3,
-        )
-        ax.text(tmin, 0, "Pulse", ha="left", va="top", color="gray")
-
         ax.set_xlabel("Time-of-flight (us)")
         ax.set_ylabel("Distance (m)")
         ax.set_xlim(0 - dx, tof_max + dx)
+        if figsize is None:
+            inches = fig.get_size_inches()
+            fig.set_size_inches(
+                (
+                    min(inches[0] * furthest_detector.data.sizes['pulse'], 12.0),
+                    inches[1],
+                )
+            )
         fig.tight_layout()
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self) -> str:
-        out = f"Result:\n  Pulse: {self._pulse.neutrons} neutrons.\n  Choppers:\n"
+        source_sizes = self._source.data.sizes
+        other_dim = (set(source_sizes) - {'pulse'}).pop()
+        out = (
+            f"Result:\n  Source: {source_sizes['pulse']} pulses, "
+            f"{source_sizes[other_dim]} neutrons per pulse.\n  Choppers:\n"
+        )
         for name, ch in self._choppers.items():
-            tofs = ch.tofs
-            out += (
-                f"    {name}: visible={len(tofs.visible)}, "
-                f"blocked={len(tofs.blocked)}\n"
-            )
+            out += f"    {name}: {ch.tofs._repr_string_body()}\n"
         out += "  Detectors:\n"
         for name, det in self._detectors.items():
-            out += f"    {name}: visible={len(det.tofs.visible)}\n"
+            out += f"    {name}: {det.tofs._repr_string_body()}\n"
         return out
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `tof-23.5.1/src/tof/utils.py` & `tof-23.5.2/src/tof/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 
 from dataclasses import dataclass
 
 import matplotlib.pyplot as plt
 import scipp as sc
 import scipp.constants as const
 
-alpha = const.m_n / const.h
+m_over_h = const.m_n / const.h
 two_pi = sc.constants.pi * (2.0 * sc.units.rad)
 
 
 def speed_to_wavelength(x: sc.Variable, unit: str = 'angstrom') -> sc.Variable:
     """
     Convert neutron speeds to wavelengths.
 
     Parameters
     ----------
     x:
         Input speeds.
     unit:
         The unit of the output wavelengths.
     """
-    return (1.0 / (alpha * x)).to(unit=unit)
+    return (1.0 / (m_over_h * x)).to(unit=unit)
 
 
 def wavelength_to_speed(x: sc.Variable, unit: str = 'm/s') -> sc.Variable:
     """
     Convert neutron wavelengths to speeds.
 
     Parameters
     ----------
     x:
         Input wavelengths.
     unit:
         The unit of the output speeds.
     """
-    return (1.0 / (alpha * x)).to(unit=unit)
+    return (1.0 / (m_over_h * x)).to(unit=unit)
 
 
 def speed_to_energy(x: sc.Variable, unit='meV') -> sc.Variable:
     """
     Convert neutron speeds to energies.
 
     Parameters
@@ -67,13 +67,14 @@
     return sc.sqrt(x / const.m_n).to(unit=unit)
 
 
 @dataclass(frozen=True)
 class FacilityPulse:
     time: sc.DataArray
     wavelength: sc.DataArray
+    frequency: sc.Variable
 
 
 @dataclass
 class Plot:
     ax: plt.Axes
     fig: plt.Figure
```

### Comparing `tof-23.5.1/src/tof.egg-info/PKG-INFO` & `tof-23.5.2/src/tof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 23.5.1
+Version: 23.5.2
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-23.5.1/src/tof.egg-info/SOURCES.txt` & `tof-23.5.2/src/tof.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 pyproject.toml
 tox.ini
 ./src/tof/__init__.py
 ./src/tof/chopper.py
 ./src/tof/component.py
 ./src/tof/detector.py
 ./src/tof/model.py
-./src/tof/pulse.py
 ./src/tof/result.py
+./src/tof/source.py
 ./src/tof/utils.py
 ./src/tof.egg-info/PKG-INFO
 ./src/tof.egg-info/SOURCES.txt
 ./src/tof.egg-info/dependency_links.txt
 ./src/tof.egg-info/requires.txt
 ./src/tof.egg-info/top_level.txt
 ./src/tof/facilities/__init__.py
@@ -24,17 +24,18 @@
 .github/workflows/ci.yml
 .github/workflows/release.yml
 conda/meta.yaml
 docs/api.rst
 docs/components.ipynb
 docs/conf.py
 docs/index.rst
-docs/pulses.ipynb
+docs/multiple-pulses.ipynb
 docs/requirements.txt
 docs/short-example.ipynb
+docs/sources.ipynb
 docs/_static/detector.png
 docs/_static/favicon.ico
 docs/_static/logo.svg
 docs/_static/model.png
 docs/_static/pulse.png
 requirements/ci.in
 requirements/ci.txt
@@ -47,18 +48,18 @@
 requirements/wheels.in
 requirements/wheels.txt
 src/tof/__init__.py
 src/tof/chopper.py
 src/tof/component.py
 src/tof/detector.py
 src/tof/model.py
-src/tof/pulse.py
 src/tof/result.py
+src/tof/source.py
 src/tof/utils.py
 src/tof/facilities/__init__.py
 src/tof/facilities/ess_pulse.py
 tests/__init__.py
 tests/chopper_test.py
 tests/common.py
 tests/model_test.py
-tests/pulse_test.py
-tests/result_test.py
+tests/result_test.py
+tests/source_test.py
```

### Comparing `tof-23.5.1/tests/chopper_test.py` & `tof-23.5.2/tests/chopper_test.py`

 * *Files identical despite different names*

### Comparing `tof-23.5.1/tests/model_test.py` & `tof-23.5.2/tests/model_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 
 import pytest
 import scipp as sc
 
 import tof
 
-from .common import dummy_chopper, dummy_detector, dummy_pulse, make_chopper, make_pulse
+from .common import (
+    dummy_chopper,
+    dummy_detector,
+    dummy_source,
+    make_chopper,
+    make_source,
+)
 
 Hz = sc.Unit('Hz')
 deg = sc.Unit('deg')
 meter = sc.Unit('m')
 ms = sc.Unit('ms')
 
 
@@ -26,39 +32,46 @@
         distance=10 * meter,
         name='chopper',
     )
     detector = tof.Detector(distance=20 * meter, name='detector')
 
     # Make a pulse with 3 neutrons with one neutron going through the chopper opening
     # and the other two neutrons on either side of the opening.
-    pulse = make_pulse(
+    source = make_source(
         arrival_times=sc.concat(
             [0.9 * topen, 0.5 * (topen + tclose), 1.1 * tclose], dim='event'
         ),
         distance=chopper.distance,
     )
 
-    model = tof.Model(pulse=pulse, choppers=[chopper], detectors=[detector])
+    model = tof.Model(source=source, choppers=[chopper], detectors=[detector])
     res = model.run()
 
-    visible = res.choppers['chopper'].tofs.visible
-    blocked = res.choppers['chopper'].tofs.blocked
+    key = 'pulse:0'
+    visible = res.choppers['chopper'].tofs.visible.data[key]
+    blocked = res.choppers['chopper'].tofs.blocked.data[key]
 
     assert len(visible) == 1
     assert len(blocked) == 2
     assert sc.isclose(
-        visible.data.coords['tof'][0],
+        visible.coords['tof'][0],
         (0.5 * (topen + tclose)).to(unit='us'),
     )
-    assert sc.isclose(blocked.data.coords['tof'][0], (0.9 * topen).to(unit='us'))
-    assert sc.isclose(blocked.data.coords['tof'][1], (1.1 * tclose).to(unit='us'))
-    assert len(res.detectors['detector'].tofs.visible) == 1
+    assert sc.isclose(blocked.coords['tof'][0], (0.9 * topen).to(unit='us'))
+    assert sc.isclose(blocked.coords['tof'][1], (1.1 * tclose).to(unit='us'))
+
+    det = res.detectors['detector'].tofs.visible.data[key]
+    assert len(det) == 1
     assert sc.isclose(
-        res.detectors['detector'].tofs.visible.data.coords['tof'][0],
-        (pulse.wavelengths[1] * detector.distance * tof.utils.alpha).to(unit='us'),
+        det.coords['tof'][0],
+        (
+            source.data.coords['wavelength']['pulse', 0][1]
+            * detector.distance
+            * tof.utils.m_over_h
+        ).to(unit='us'),
     )
 
 
 def test_two_choppers_one_opening():
     # Make a first chopper open from 5-16 ms. Assume zero phase.
     topen = 5.0 * ms
     tclose = 16.0 * ms
@@ -81,54 +94,59 @@
         name='chopper2',
     )
 
     detector = tof.Detector(distance=20 * meter, name='detector')
 
     # Make a pulse with 3 neutrons with 2 neutrons going through the first chopper
     # opening and only one making it through the second chopper.
-    pulse = make_pulse(
+    source = make_source(
         arrival_times=sc.concat(
             [1.5 * topen, 0.5 * (topen + tclose), 1.1 * tclose], dim='event'
         ),
         distance=chopper1.distance,
     )
 
-    model = tof.Model(pulse=pulse, choppers=[chopper1, chopper2], detectors=[detector])
+    model = tof.Model(
+        source=source, choppers=[chopper1, chopper2], detectors=[detector]
+    )
     res = model.run()
 
-    ch1_tofs = res.choppers['chopper1'].tofs
-    ch2_tofs = res.choppers['chopper2'].tofs
+    key = 'pulse:0'
+    ch1_tofs = res.choppers['chopper1'].tofs.data
+    ch2_tofs = res.choppers['chopper2'].tofs.data
+    wavs = source.data.coords['wavelength']['pulse', 0]
+    det = res.detectors['detector'].tofs.visible.data[key]
 
-    assert len(ch1_tofs.visible) == 2
-    assert len(ch1_tofs.blocked) == 1
+    assert len(ch1_tofs['visible'][key]) == 2
+    assert len(ch1_tofs['blocked'][key]) == 1
     assert sc.isclose(
-        ch1_tofs.visible.data.coords['tof'][0], (1.5 * topen).to(unit='us')
+        ch1_tofs['visible'][key].coords['tof'][0], (1.5 * topen).to(unit='us')
     )
     assert sc.isclose(
-        ch1_tofs.visible.data.coords['tof'][1],
+        ch1_tofs['visible'][key].coords['tof'][1],
         (0.5 * (topen + tclose)).to(unit='us'),
     )
     assert sc.isclose(
-        ch1_tofs.blocked.data.coords['tof'][0], (1.1 * tclose).to(unit='us')
+        ch1_tofs['blocked'][key].coords['tof'][0], (1.1 * tclose).to(unit='us')
     )
-    assert len(ch2_tofs.visible) == 1
+    assert len(ch2_tofs['visible'][key]) == 1
     # Blocks only one neutron, the other is blocked by chopper1
-    assert len(ch2_tofs.blocked) == 1
+    assert len(ch2_tofs['blocked'][key]) == 1
     assert sc.isclose(
-        ch2_tofs.visible.data.coords['tof'][0],
-        (pulse.wavelengths[1] * chopper2.distance * tof.utils.alpha).to(unit='us'),
+        ch2_tofs['visible'][key].coords['tof'][0],
+        (wavs[1] * chopper2.distance * tof.utils.m_over_h).to(unit='us'),
     )
     assert sc.isclose(
-        ch2_tofs.blocked.data.coords['tof'][0],
-        (pulse.wavelengths[0] * chopper2.distance * tof.utils.alpha).to(unit='us'),
+        ch2_tofs['blocked'][key].coords['tof'][0],
+        (wavs[0] * chopper2.distance * tof.utils.m_over_h).to(unit='us'),
     )
-    assert len(res.detectors['detector'].tofs.visible) == 1
+    assert len(det) == 1
     assert sc.isclose(
-        res.detectors['detector'].tofs.visible.data.coords['tof'][0],
-        (pulse.wavelengths[1] * detector.distance * tof.utils.alpha).to(unit='us'),
+        det.coords['tof'][0],
+        (wavs[1] * detector.distance * tof.utils.m_over_h).to(unit='us'),
     )
 
 
 def test_two_choppers_one_and_two_openings():
     topen = 5.0 * ms
     tclose = 16.0 * ms
     chopper1 = make_chopper(
@@ -151,15 +169,15 @@
 
     detector = tof.Detector(distance=20 * meter, name='detector')
 
     # Make a pulse with 7 neutrons:
     # - 2 neutrons blocked by chopper1
     # - 3 neutrons blocked by chopper2
     # - 2 neutrons detected (one through each of chopper2's openings)
-    pulse = make_pulse(
+    source = make_source(
         arrival_times=sc.concat(
             [
                 0.9 * topen,
                 1.01 * topen,
                 1.3 * topen,
                 1.8 * topen,
                 0.5 * (topen + tclose),
@@ -167,27 +185,30 @@
                 1.1 * tclose,
             ],
             dim='event',
         ),
         distance=chopper1.distance,
     )
 
-    model = tof.Model(pulse=pulse, choppers=[chopper1, chopper2], detectors=[detector])
+    model = tof.Model(
+        source=source, choppers=[chopper1, chopper2], detectors=[detector]
+    )
     res = model.run()
 
-    assert len(res.choppers['chopper1'].tofs.visible) == 5
-    assert len(res.choppers['chopper1'].tofs.blocked) == 2
-    assert len(res.choppers['chopper2'].tofs.visible) == 2
-    assert len(res.choppers['chopper2'].tofs.blocked) == 3
-    assert len(res.detectors['detector'].tofs.visible) == 2
+    key = 'pulse:0'
+    assert len(res.choppers['chopper1'].tofs.visible.data[key]) == 5
+    assert len(res.choppers['chopper1'].tofs.blocked.data[key]) == 2
+    assert len(res.choppers['chopper2'].tofs.visible.data[key]) == 2
+    assert len(res.choppers['chopper2'].tofs.blocked.data[key]) == 3
+    assert len(res.detectors['detector'].tofs.visible.data[key]) == 2
 
 
 def test_neutron_conservation():
     N = 100_000
-    pulse = tof.Pulse(facility='ess', neutrons=N)
+    source = tof.Source(facility='ess', neutrons=N)
 
     chopper1 = make_chopper(
         topen=[5.0 * ms],
         tclose=[16.0 * ms],
         f=10.0 * Hz,
         phase=0.0 * deg,
         distance=10 * meter,
@@ -199,46 +220,48 @@
         f=15.0 * Hz,
         phase=0.0 * deg,
         distance=15 * meter,
         name='chopper2',
     )
 
     detector = tof.Detector(distance=20 * meter, name='detector')
-    model = tof.Model(pulse=pulse, choppers=[chopper1, chopper2], detectors=[detector])
+    model = tof.Model(
+        source=source, choppers=[chopper1, chopper2], detectors=[detector]
+    )
     res = model.run()
 
-    assert (
-        res.choppers['chopper1'].tofs.visible.data.sum()
-        + res.choppers['chopper1'].tofs.blocked.data.sum()
-    ).value == N
+    key = 'pulse:0'
+    ch1 = res.choppers['chopper1'].tofs.data
+    ch2 = res.choppers['chopper2'].tofs.data
+
+    assert (ch1['visible'][key].sum() + ch1['blocked'][key].sum()).value == N
     assert sc.identical(
-        res.choppers['chopper2'].tofs.visible.data.sum()
-        + res.choppers['chopper2'].tofs.blocked.data.sum(),
-        res.choppers['chopper1'].tofs.visible.data.sum(),
+        ch2['visible'][key].sum() + ch2['blocked'][key].sum(),
+        ch1['visible'][key].sum(),
     )
     assert sc.identical(
-        res.detectors['detector'].tofs.visible.data.sum(),
-        res.choppers['chopper2'].tofs.visible.data.sum(),
+        res.detectors['detector'].tofs.data['visible'][key].sum(),
+        ch2['visible'][key].sum(),
     )
 
 
 def test_add_chopper_and_detector():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse())
+    model = tof.Model(source=dummy_source())
     model.add(chopper)
     assert 'dummy_chopper' in model.choppers
     model.add(detector)
     assert 'dummy_detector' in model.detectors
 
 
 def test_add_components_with_same_name_raises():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse())
+    model = tof.Model(source=dummy_source())
     model.add(chopper)
     with pytest.raises(
         KeyError, match='Component with name dummy_chopper already exists'
     ):
         model.add(chopper)
     model.add(detector)
     with pytest.raises(
@@ -251,58 +274,84 @@
     ):
         model.add(detector2)
 
 
 def test_iter():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse())
+    model = tof.Model(source=dummy_source())
     model.add(chopper)
     assert 'dummy_chopper' in model.choppers
     model.add(detector)
     assert 'dummy_detector' in model.detectors
 
 
 def test_remove():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse(), choppers=[chopper], detectors=[detector])
+    model = tof.Model(source=dummy_source(), choppers=[chopper], detectors=[detector])
     del model['dummy_chopper']
     assert 'dummy_chopper' not in model
     assert 'dummy_detector' in model
     del model['dummy_detector']
     assert 'dummy_detector' not in model
 
 
 def test_getitem():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse(), choppers=[chopper], detectors=[detector])
+    model = tof.Model(source=dummy_source(), choppers=[chopper], detectors=[detector])
     assert model['dummy_chopper'] is chopper
     assert model['dummy_detector'] is detector
     with pytest.raises(KeyError, match='No component with name foo'):
         model['foo']
 
 
 def test_input_can_be_single_component():
     chopper = dummy_chopper()
     detector = dummy_detector()
-    model = tof.Model(pulse=dummy_pulse(), choppers=chopper, detectors=detector)
+    model = tof.Model(source=dummy_source(), choppers=chopper, detectors=detector)
     assert 'dummy_chopper' in model.choppers
     assert 'dummy_detector' in model.detectors
 
 
 def test_bad_input_type_raises():
     chopper = dummy_chopper()
     detector = dummy_detector()
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), choppers='bad chopper')
+        _ = tof.Model(source=dummy_source(), choppers='bad chopper')
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), choppers=[chopper], detectors='abc')
+        _ = tof.Model(source=dummy_source(), choppers=[chopper], detectors='abc')
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), choppers=[chopper, 'bad chopper'])
+        _ = tof.Model(source=dummy_source(), choppers=[chopper, 'bad chopper'])
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), detectors=(1234, detector))
+        _ = tof.Model(source=dummy_source(), detectors=(1234, detector))
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), choppers=[detector])
+        _ = tof.Model(source=dummy_source(), choppers=[detector])
     with pytest.raises(TypeError, match='Invalid input type'):
-        _ = tof.Model(pulse=dummy_pulse(), detectors=[chopper])
+        _ = tof.Model(source=dummy_source(), detectors=[chopper])
+
+
+def test_model_repr_does_not_raise():
+    N = 10_000
+    source = tof.Source(facility='ess', neutrons=N)
+    chopper1 = make_chopper(
+        topen=[5.0 * ms],
+        tclose=[16.0 * ms],
+        f=10.0 * Hz,
+        phase=0.0 * deg,
+        distance=10 * meter,
+        name='chopper1',
+    )
+    chopper2 = make_chopper(
+        topen=[9.0 * ms, 15.0 * ms],
+        tclose=[15.0 * ms, 20.0 * ms],
+        f=15.0 * Hz,
+        phase=0.0 * deg,
+        distance=15 * meter,
+        name='chopper2',
+    )
+    detector = tof.Detector(distance=20 * meter, name='detector')
+    model = tof.Model(
+        source=source, choppers=[chopper1, chopper2], detectors=[detector]
+    )
+    assert repr(model) is not None
```

### Comparing `tof-23.5.1/tox.ini` & `tof-23.5.2/tox.ini`

 * *Files identical despite different names*

