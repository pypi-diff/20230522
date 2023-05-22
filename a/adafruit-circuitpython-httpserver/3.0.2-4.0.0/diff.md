# Comparing `tmp/adafruit-circuitpython-httpserver-3.0.2.tar.gz` & `tmp/adafruit-circuitpython-httpserver-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-3.0.2.tar", last modified: Tue Apr 25 22:26:54 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-4.0.0.tar", last modified: Mon May 22 20:39:01 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-3.0.2.tar` & `adafruit-circuitpython-httpserver-4.0.0.tar`

### file list

```diff
@@ -1,63 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.247208 adafruit-circuitpython-httpserver-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.235208 adafruit-circuitpython-httpserver-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.239208 adafruit-circuitpython-httpserver-3.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.239208 adafruit-circuitpython-httpserver-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.239208 adafruit-circuitpython-httpserver-3.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-25 22:26:54.247208 adafruit-circuitpython-httpserver-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.239208 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-25 22:26:54.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-25 22:26:54.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 22:26:54.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 22:26:54.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 22:26:54.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.243208 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.243208 adafruit-circuitpython-httpserver-3.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.247208 adafruit-circuitpython-httpserver-3.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 22:26:54.247208 adafruit-circuitpython-httpserver-3.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_simple_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-25 22:26:44.000000 adafruit-circuitpython-httpserver-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 22:26:32.000000 adafruit-circuitpython-httpserver-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 22:26:54.247208 adafruit-circuitpython-httpserver-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.863796 adafruit-circuitpython-httpserver-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.851795 adafruit-circuitpython-httpserver-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.855795 adafruit-circuitpython-httpserver-4.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.855795 adafruit-circuitpython-httpserver-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.855795 adafruit-circuitpython-httpserver-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-22 20:39:01.863796 adafruit-circuitpython-httpserver-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.855795 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-22 20:39:01.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 20:39:01.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:39:01.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 20:39:01.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 20:39:01.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.859795 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.859795 adafruit-circuitpython-httpserver-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.859795 adafruit-circuitpython-httpserver-4.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:39:01.863796 adafruit-circuitpython-httpserver-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_simpletest_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_simpletest_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-22 20:38:52.000000 adafruit-circuitpython-httpserver-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 20:38:39.000000 adafruit-circuitpython-httpserver-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:39:01.863796 adafruit-circuitpython-httpserver-4.0.0/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-4.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/.gitignore` & `adafruit-circuitpython-httpserver-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-4.0.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/.pylintrc` & `adafruit-circuitpython-httpserver-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-4.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/LICENSE` & `adafruit-circuitpython-httpserver-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-4.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-4.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-4.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/PKG-INFO` & `adafruit-circuitpython-httpserver-4.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 3.0.2
+Version: 4.0.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -44,14 +44,15 @@
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, body and client's address, the one from which the request came.
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
+- Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -109,14 +110,21 @@
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
 
+Security
+========
+
+The HTTP server implementation in this package is not robust and should only be deployed on trusted networks.
+For instance, there are trivial denial of service attacks against adafruit_httpserver.
+Pull requests that improve the server's security and robustness are of course welcome.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/README.rst` & `adafruit-circuitpython-httpserver-4.0.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, body and client's address, the one from which the request came.
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
+- Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -91,14 +92,21 @@
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
 
+Security
+========
+
+The HTTP server implementation in this package is not robust and should only be deployed on trusted networks.
+For instance, there are trivial denial of service attacks against adafruit_httpserver.
+Pull requests that improve the server's security and robustness are of course welcome.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 3.0.2
+Version: 4.0.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -44,14 +44,15 @@
 - Supports `socketpool` or `socket` as a source of sockets; can be used in CPython.
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, body and client's address, the one from which the request came.
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
+- Supports HTTP Basic and Bearer Authentication on both server and route per level.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -109,14 +110,21 @@
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
 
+Security
+========
+
+The HTTP server implementation in this package is not robust and should only be deployed on trusted networks.
+For instance, there are trivial denial of service attacks against adafruit_httpserver.
+Pull requests that improve the server's security and robustness are of course welcome.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-4.0.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 LICENSES/Unlicense.txt
 adafruit_circuitpython_httpserver.egg-info/PKG-INFO
 adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
 adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
 adafruit_circuitpython_httpserver.egg-info/requires.txt
 adafruit_circuitpython_httpserver.egg-info/top_level.txt
 adafruit_httpserver/__init__.py
+adafruit_httpserver/authentication.py
 adafruit_httpserver/exceptions.py
 adafruit_httpserver/headers.py
 adafruit_httpserver/methods.py
-adafruit_httpserver/mime_type.py
+adafruit_httpserver/mime_types.py
 adafruit_httpserver/request.py
 adafruit_httpserver/response.py
 adafruit_httpserver/route.py
 adafruit_httpserver/server.py
 adafruit_httpserver/status.py
 docs/api.rst
 docs/api.rst.license
@@ -38,14 +39,24 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/home.html
+examples/httpserver_authentication_handlers.py
+examples/httpserver_authentication_server.py
 examples/httpserver_chunked.py
 examples/httpserver_cpu_information.py
+examples/httpserver_handler_serves_file.py
 examples/httpserver_mdns.py
+examples/httpserver_methods.py
+examples/httpserver_multiple_servers.py
 examples/httpserver_neopixel.py
-examples/httpserver_simple_poll.py
-examples/httpserver_simpletest.py
-examples/httpserver_url_parameters.py
+examples/httpserver_redirects.py
+examples/httpserver_simpletest_auto.py
+examples/httpserver_simpletest_manual.py
+examples/httpserver_start_and_poll.py
+examples/httpserver_static_files_serving.py
+examples/httpserver_url_parameters.py
+examples/settings.toml
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 """
-`adafruit_httpserver.headers.HTTPHeaders`
+`adafruit_httpserver.headers`
 ====================================================
 * Author(s): Michał Pokusa
 """
 
 try:
     from typing import Dict, Tuple
 except ImportError:
     pass
 
 
-class HTTPHeaders:
+class Headers:
     """
     A dict-like class for storing HTTP headers.
 
     Allows access to headers using **case insensitive** names.
 
     Does **not** implement all dict methods.
 
     Examples::
 
-        headers = HTTPHeaders({"Content-Type": "text/html", "Content-Length": "1024"})
+        headers = Headers({"Content-Type": "text/html", "Content-Length": "1024"})
 
         len(headers)
         # 2
 
         headers.setdefault("Access-Control-Allow-Origin", "*")
         headers["Access-Control-Allow-Origin"]
         # '*'
@@ -44,15 +44,14 @@
         "CONTENT-TYPE" in headers
         # True
     """
 
     _storage: Dict[str, Tuple[str, str]]
 
     def __init__(self, headers: Dict[str, str] = None) -> None:
-
         headers = headers or {}
 
         self._storage = {key.lower(): [key, value] for key, value in headers.items()}
 
     def get(self, name: str, default: str = None):
         """Returns the value for the given header name, or default if not found."""
         return self._storage.get(name.lower(), [None, default])[1]
@@ -77,15 +76,15 @@
         """Updates the headers with the given dict."""
         return self._storage.update(
             {key.lower(): [key, value] for key, value in headers.items()}
         )
 
     def copy(self):
         """Returns a copy of the headers."""
-        return HTTPHeaders(dict(self._storage.values()))
+        return Headers(dict(self._storage.values()))
 
     def __getitem__(self, name: str):
         return self._storage[name.lower()][1]
 
     def __setitem__(self, name: str, value: str):
         self._storage[name.lower()] = [name, value]
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 # SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 """
-`adafruit_httpserver.request.HTTPRequest`
+`adafruit_httpserver.request`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
 
 try:
-    from typing import Dict, Tuple, Union
+    from typing import Dict, Tuple, Union, TYPE_CHECKING
     from socket import socket
     from socketpool import SocketPool
+
+    if TYPE_CHECKING:
+        from .server import Server
 except ImportError:
     pass
 
-from .headers import HTTPHeaders
+import json
+
+from .headers import Headers
 
 
-class HTTPRequest:
+class Request:
     """
     Incoming request, constructed from raw incoming bytes.
-    It is passed as first argument to route handlers.
+    It is passed as first argument to all route handlers.
+    """
+
+    server: "Server"
+    """
+    Server object that received the request.
     """
 
     connection: Union["SocketPool.Socket", "socket.socket"]
     """
-    Socket object usable to send and receive data on the connection.
+    Socket object used to send and receive data on the connection.
     """
 
     client_address: Tuple[str, int]
     """
     Address and port bound to the socket on the other end of the connection.
 
     Example::
@@ -38,56 +48,58 @@
             # ('192.168.137.1', 40684)
     """
 
     method: str
     """Request method e.g. "GET" or "POST"."""
 
     path: str
-    """Path of the request."""
+    """Path of the request, e.g. ``"/foo/bar"``."""
 
     query_params: Dict[str, str]
     """
     Query/GET parameters in the request.
 
     Example::
 
-            request  = HTTPRequest(raw_request=b"GET /?foo=bar HTTP/1.1...")
+            request  = Request(raw_request=b"GET /?foo=bar HTTP/1.1...")
             request.query_params
             # {"foo": "bar"}
     """
 
     http_version: str
-    """HTTP version, e.g. "HTTP/1.1"."""
+    """HTTP version, e.g. ``"HTTP/1.1"``."""
 
-    headers: HTTPHeaders
+    headers: Headers
     """
     Headers from the request.
     """
 
     raw_request: bytes
     """
-    Raw 'bytes' passed to the constructor and body 'bytes' received later.
+    Raw 'bytes' that were received from the client.
 
     Should **not** be modified directly.
     """
 
     def __init__(
         self,
+        server: "Server",
         connection: Union["SocketPool.Socket", "socket.socket"],
         client_address: Tuple[str, int],
         raw_request: bytes = None,
     ) -> None:
+        self.server = server
         self.connection = connection
         self.client_address = client_address
         self.raw_request = raw_request
 
         if raw_request is None:
             raise ValueError("raw_request cannot be None")
 
-        header_bytes = self.header_body_bytes[0]
+        header_bytes = self._raw_header_bytes
 
         try:
             (
                 self.method,
                 self.path,
                 self.query_params,
                 self.http_version,
@@ -95,29 +107,37 @@
             self.headers = self._parse_headers(header_bytes)
         except Exception as error:
             raise ValueError("Unparseable raw_request: ", raw_request) from error
 
     @property
     def body(self) -> bytes:
         """Body of the request, as bytes."""
-        return self.header_body_bytes[1]
+        return self._raw_body_bytes
 
     @body.setter
     def body(self, body: bytes) -> None:
-        self.raw_request = self.header_body_bytes[0] + b"\r\n\r\n" + body
+        self.raw_request = self._raw_header_bytes + b"\r\n\r\n" + body
+
+    def json(self) -> Union[dict, None]:
+        """Body of the request, as a JSON-decoded dictionary."""
+        return json.loads(self.body) if self.body else None
 
     @property
-    def header_body_bytes(self) -> Tuple[bytes, bytes]:
-        """Return tuple of header and body bytes."""
+    def _raw_header_bytes(self) -> bytes:
+        """Returns headers bytes."""
+        empty_line_index = self.raw_request.find(b"\r\n\r\n")
 
+        return self.raw_request[:empty_line_index]
+
+    @property
+    def _raw_body_bytes(self) -> bytes:
+        """Returns body bytes."""
         empty_line_index = self.raw_request.find(b"\r\n\r\n")
-        header_bytes = self.raw_request[:empty_line_index]
-        body_bytes = self.raw_request[empty_line_index + 4 :]
 
-        return header_bytes, body_bytes
+        return self.raw_request[empty_line_index + 4 :]
 
     @staticmethod
     def _parse_start_line(header_bytes: bytes) -> Tuple[str, str, Dict[str, str], str]:
         """Parse HTTP Start line to method, path, query_params and http_version."""
 
         start_line = header_bytes.decode("utf8").splitlines()[0]
 
@@ -135,18 +155,18 @@
                 query_params[key] = value
             elif query_param:
                 query_params[query_param] = ""
 
         return method, path, query_params, http_version
 
     @staticmethod
-    def _parse_headers(header_bytes: bytes) -> HTTPHeaders:
+    def _parse_headers(header_bytes: bytes) -> Headers:
         """Parse HTTP headers from raw request."""
         header_lines = header_bytes.decode("utf8").splitlines()[1:]
 
-        return HTTPHeaders(
+        return Headers(
             {
                 name: value
                 for header_line in header_lines
                 for name, value in [header_line.split(": ", 1)]
             }
         )
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-4.0.0/adafruit_httpserver/status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 # SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 """
-`adafruit_httpserver.status.HTTPStatus`
+`adafruit_httpserver.status`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
 
 
-class HTTPStatus:  # pylint: disable=too-few-public-methods
-    """HTTP status codes."""
+class Status:  # pylint: disable=too-few-public-methods
+    """HTTP status code."""
 
     def __init__(self, code: int, text: str):
-        """Define a status code.
+        """
+        Define a status code.
 
         :param int code: Numeric value: 200, 404, etc.
         :param str text: Short phrase: "OK", "Not Found', etc.
         """
         self.code = code
         self.text = text
 
     def __repr__(self):
-        return f'HTTPStatus({self.code}, "{self.text}")'
+        return f'Status({self.code}, "{self.text}")'
 
     def __str__(self):
         return f"{self.code} {self.text}"
 
-    def __eq__(self, other: "HTTPStatus"):
+    def __eq__(self, other: "Status"):
         return self.code == other.code and self.text == other.text
 
 
-class CommonHTTPStatus(HTTPStatus):  # pylint: disable=too-few-public-methods
-    """Common HTTP status codes."""
+OK_200 = Status(200, "OK")
+
+CREATED_201 = Status(201, "Created")
+
+ACCEPTED_202 = Status(202, "Accepted")
+
+NO_CONTENT_204 = Status(204, "No Content")
+
+PARTIAL_CONTENT_206 = Status(206, "Partial Content")
+
+TEMPORARY_REDIRECT_307 = Status(307, "Temporary Redirect")
+
+PERMANENT_REDIRECT_308 = Status(308, "Permanent Redirect")
+
+BAD_REQUEST_400 = Status(400, "Bad Request")
+
+UNAUTHORIZED_401 = Status(401, "Unauthorized")
+
+FORBIDDEN_403 = Status(403, "Forbidden")
+
+NOT_FOUND_404 = Status(404, "Not Found")
 
-    OK_200 = HTTPStatus(200, "OK")
-    """200 OK"""
+METHOD_NOT_ALLOWED_405 = Status(405, "Method Not Allowed")
 
-    BAD_REQUEST_400 = HTTPStatus(400, "Bad Request")
-    """400 Bad Request"""
+TOO_MANY_REQUESTS_429 = Status(429, "Too Many Requests")
 
-    FORBIDDEN_403 = HTTPStatus(403, "Forbidden")
-    """403 Forbidden"""
+INTERNAL_SERVER_ERROR_500 = Status(500, "Internal Server Error")
 
-    NOT_FOUND_404 = HTTPStatus(404, "Not Found")
-    """404 Not Found"""
+NOT_IMPLEMENTED_501 = Status(501, "Not Implemented")
 
-    INTERNAL_SERVER_ERROR_500 = HTTPStatus(500, "Internal Server Error")
-    """500 Internal Server Error"""
+SERVICE_UNAVAILABLE_503 = Status(503, "Service Unavailable")
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-4.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/docs/api.rst` & `adafruit-circuitpython-httpserver-4.0.0/docs/api.rst`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,12 @@
 
 .. automodule:: adafruit_httpserver.headers
     :members:
 
 .. automodule:: adafruit_httpserver.status
     :members:
 
-.. automodule:: adafruit_httpserver.methods
-    :members:
-
-.. automodule:: adafruit_httpserver.mime_type
+.. automodule:: adafruit_httpserver.mime_types
     :members:
 
 .. automodule:: adafruit_httpserver.exceptions
     :members:
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/docs/conf.py` & `adafruit-circuitpython-httpserver-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/docs/index.rst` & `adafruit-circuitpython-httpserver-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_mdns.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 # SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
-import os
-
 import mdns
 import socketpool
 import wifi
 
-from adafruit_httpserver.mime_type import MIMEType
-from adafruit_httpserver.request import HTTPRequest
-from adafruit_httpserver.response import HTTPResponse
-from adafruit_httpserver.server import HTTPServer
-
+from adafruit_httpserver import Server, Request, FileResponse
 
-ssid = os.getenv("WIFI_SSID")
-password = os.getenv("WIFI_PASSWORD")
-
-print("Connecting to", ssid)
-wifi.radio.connect(ssid, password)
-print("Connected to", ssid)
 
 mdns_server = mdns.Server(wifi.radio)
 mdns_server.hostname = "custom-mdns-hostname"
 mdns_server.advertise_service(service_type="_http", protocol="_tcp", port=80)
 
 pool = socketpool.SocketPool(wifi.radio)
-server = HTTPServer(pool, "/static")
+server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
-def base(request: HTTPRequest):
+def base(request: Request):
     """
     Serve the default index.html file.
     """
-    with HTTPResponse(request, content_type=MIMEType.TYPE_HTML) as response:
-        response.send_file("index.html")
+
+    return FileResponse(request, "index.html", "/www")
 
 
-print(f"Listening on http://{wifi.radio.ipv4_address}:80")
 server.serve_forever(str(wifi.radio.ipv4_address))
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_simple_poll.py` & `adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_start_and_poll.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 # SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
-import os
-
 import socketpool
 import wifi
 
-from adafruit_httpserver.mime_type import MIMEType
-from adafruit_httpserver.request import HTTPRequest
-from adafruit_httpserver.response import HTTPResponse
-from adafruit_httpserver.server import HTTPServer
-
+from adafruit_httpserver import Server, Request, FileResponse
 
-ssid = os.getenv("WIFI_SSID")
-password = os.getenv("WIFI_PASSWORD")
-
-print("Connecting to", ssid)
-wifi.radio.connect(ssid, password)
-print("Connected to", ssid)
 
 pool = socketpool.SocketPool(wifi.radio)
-server = HTTPServer(pool, "/static")
+server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
-def base(request: HTTPRequest):
+def base(request: Request):
     """
     Serve the default index.html file.
     """
-    with HTTPResponse(request, content_type=MIMEType.TYPE_HTML) as response:
-        response.send_file("index.html")
+    return FileResponse(request, "index.html")
 
 
-print(f"Listening on http://{wifi.radio.ipv4_address}:80")
-
 # Start the server.
 server.start(str(wifi.radio.ipv4_address))
 
 while True:
     try:
         # Do something useful in this section,
         # for example read a sensor and capture an average,
         # or a running total of the last 10 samples
 
         # Process any waiting requests
         server.poll()
+
+        # If you want you can stop the server by calling server.stop() anywhere in your code
     except OSError as error:
         print(error)
         continue
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/examples/httpserver_simpletest.py` & `adafruit-circuitpython-httpserver-4.0.0/examples/httpserver_simpletest_manual.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,36 +3,29 @@
 # SPDX-License-Identifier: Unlicense
 
 import os
 
 import socketpool
 import wifi
 
-from adafruit_httpserver.mime_type import MIMEType
-from adafruit_httpserver.request import HTTPRequest
-from adafruit_httpserver.response import HTTPResponse
-from adafruit_httpserver.server import HTTPServer
-
+from adafruit_httpserver import Server, Request, Response
 
 ssid = os.getenv("WIFI_SSID")
 password = os.getenv("WIFI_PASSWORD")
 
 print("Connecting to", ssid)
 wifi.radio.connect(ssid, password)
 print("Connected to", ssid)
 
 pool = socketpool.SocketPool(wifi.radio)
-server = HTTPServer(pool, "/static")
+server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
-def base(request: HTTPRequest):
+def base(request: Request):
     """
     Serve a default static plain text message.
     """
-    with HTTPResponse(request, content_type=MIMEType.TYPE_TXT) as response:
-        message = "Hello from the CircuitPython HTTPServer!"
-        response.send(message)
+    return Response(request, "Hello from the CircuitPython HTTP Server!")
 
 
-print(f"Listening on http://{wifi.radio.ipv4_address}:80")
 server.serve_forever(str(wifi.radio.ipv4_address))
```

### Comparing `adafruit-circuitpython-httpserver-3.0.2/pyproject.toml` & `adafruit-circuitpython-httpserver-4.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "3.0.2"
+version = "4.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

