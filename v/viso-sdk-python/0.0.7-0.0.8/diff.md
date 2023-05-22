# Comparing `tmp/viso-sdk-python-0.0.7.tar.gz` & `tmp/viso-sdk-python-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viso-sdk-python-0.0.7.tar", last modified: Tue May  2 19:25:58 2023, max compression
+gzip compressed data, was "viso-sdk-python-0.0.8.tar", last modified: Mon May 22 20:11:16 2023, max compression
```

## Comparing `viso-sdk-python-0.0.7.tar` & `viso-sdk-python-0.0.8.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.244015 viso-sdk-python-0.0.7/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-02 19:25:58.244015 viso-sdk-python-0.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.221097 viso-sdk-python-0.0.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7128 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.222014 viso-sdk-python-0.0.7/docs/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/ext/docstrings.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/ext/manager_tmpl.j2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/docs/viso.rst
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements-docker.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements-docs.txt
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements-lint.txt
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-02 19:25:58.244932 viso-sdk-python-0.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2580 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.222931 viso-sdk-python-0.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.222931 viso-sdk-python-0.0.7/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/fixtures/flow.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.224764 viso-sdk-python-0.0.7/tests/meta/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/meta/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/meta/test_ensure_type_hints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.224764 viso-sdk-python-0.0.7/tests/smoke/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/smoke/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/smoke/test_dists.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/test_flow.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tests/test_status.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.226598 viso-sdk-python-0.0.7/viso_sdk/
--rw-r--r--   0 root         (0) root         (0)   128282 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138995 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/_version.c
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.229348 viso-sdk-python-0.0.7/viso_sdk/constants/
--rw-r--r--   0 root         (0) root         (0)   134253 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/constants/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/constants/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168423 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/constants/constants.c
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/constants/constants.py
--rw-r--r--   0 root         (0) root         (0)   122038 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/constants/modules.c
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/constants/modules.py
--rw-r--r--   0 root         (0) root         (0)   219738 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/constants/variables.c
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/constants/variables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.231181 viso-sdk-python-0.0.7/viso_sdk/edge/
--rw-r--r--   0 root         (0) root         (0)   108989 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/edge/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/edge/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312878 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/edge/common.c
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/edge/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.233015 viso-sdk-python-0.0.7/viso_sdk/logging/
--rw-r--r--   0 root         (0) root         (0)   114597 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/logging/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)   275645 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/logging/logger.c
--rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/logging/logger.py
--rw-r--r--   0 root         (0) root         (0)   356104 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/logging/status_logger.c
--rw-rw-rw-   0 root         (0) root         (0)     4603 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/logging/status_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.235765 viso-sdk-python-0.0.7/viso_sdk/mqtt/
--rw-r--r--   0 root         (0) root         (0)   113135 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/mqtt/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)   353758 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/mqtt/mqtt_wrapper.c
--rw-rw-rw-   0 root         (0) root         (0)     3802 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/mqtt/mqtt_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.237598 viso-sdk-python-0.0.7/viso_sdk/nodered/
--rw-r--r--   0 root         (0) root         (0)   113205 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/nodered/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/nodered/__init__.py
--rw-r--r--   0 root         (0) root         (0)   377549 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/nodered/flow.c
--rw-rw-rw-   0 root         (0) root         (0)     5613 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/nodered/flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.239432 viso-sdk-python-0.0.7/viso_sdk/redis/
--rw-r--r--   0 root         (0) root         (0)   113197 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/redis/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387846 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/redis/redis_wrapper.c
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/redis/redis_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.242182 viso-sdk-python-0.0.7/viso_sdk/visualize/
--rw-r--r--   0 root         (0) root         (0)   113212 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/__init__.c
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/__init__.py
--rw-r--r--   0 root         (0) root         (0)   244344 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/custom_font.c
--rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/custom_font.py
--rw-r--r--   0 root         (0) root         (0)   378258 2023-05-02 19:25:57.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/palette.c
--rw-rw-rw-   0 root         (0) root         (0)     2400 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/palette.py
--rw-r--r--   0 root         (0) root         (0)   472190 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/visualization.c
--rw-rw-rw-   0 root         (0) root         (0)     7621 2023-05-02 19:25:43.000000 viso-sdk-python-0.0.7/viso_sdk/visualize/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:25:58.244015 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-02 19:25:58.000000 viso-sdk-python-0.0.7/viso_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.521395 viso-sdk-python-0.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-22 20:11:16.521395 viso-sdk-python-0.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.507395 viso-sdk-python-0.0.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.507395 viso-sdk-python-0.0.8/docs/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/ext/docstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/ext/manager_tmpl.j2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/docs/viso.rst
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements-docker.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements-docs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements-lint.txt
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-22 20:11:16.521395 viso-sdk-python-0.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2580 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.508395 viso-sdk-python-0.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.508395 viso-sdk-python-0.0.8/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/fixtures/flow.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.508395 viso-sdk-python-0.0.8/tests/meta/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/meta/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/meta/test_ensure_type_hints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.509395 viso-sdk-python-0.0.8/tests/smoke/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/smoke/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/smoke/test_dists.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/test_flow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tests/test_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.510395 viso-sdk-python-0.0.8/viso_sdk/
+-rw-r--r--   0 root         (0) root         (0)   128282 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138995 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/_version.c
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.512395 viso-sdk-python-0.0.8/viso_sdk/constants/
+-rw-r--r--   0 root         (0) root         (0)   134253 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/constants/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/constants/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168423 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/constants/constants.c
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/constants/constants.py
+-rw-r--r--   0 root         (0) root         (0)   122038 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/constants/modules.c
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/constants/modules.py
+-rw-r--r--   0 root         (0) root         (0)   195895 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/constants/variables.c
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/constants/variables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.513395 viso-sdk-python-0.0.8/viso_sdk/edge/
+-rw-r--r--   0 root         (0) root         (0)   108989 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/edge/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/edge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312878 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/edge/common.c
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/edge/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.514395 viso-sdk-python-0.0.8/viso_sdk/logging/
+-rw-r--r--   0 root         (0) root         (0)   114597 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/logging/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   275645 2023-05-22 20:11:15.000000 viso-sdk-python-0.0.8/viso_sdk/logging/logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/logging/logger.py
+-rw-r--r--   0 root         (0) root         (0)   356104 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/logging/status_logger.c
+-rw-rw-rw-   0 root         (0) root         (0)     4603 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/logging/status_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.515395 viso-sdk-python-0.0.8/viso_sdk/mqtt/
+-rw-r--r--   0 root         (0) root         (0)   113135 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/mqtt/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   353758 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/mqtt/mqtt_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     3802 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/mqtt/mqtt_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.516395 viso-sdk-python-0.0.8/viso_sdk/nodered/
+-rw-r--r--   0 root         (0) root         (0)   113205 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/nodered/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/nodered/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   377549 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/nodered/flow.c
+-rw-rw-rw-   0 root         (0) root         (0)     5613 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/nodered/flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.518395 viso-sdk-python-0.0.8/viso_sdk/redis/
+-rw-r--r--   0 root         (0) root         (0)   113197 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/redis/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387846 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/redis/redis_wrapper.c
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/redis/redis_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.520395 viso-sdk-python-0.0.8/viso_sdk/visualize/
+-rw-r--r--   0 root         (0) root         (0)   113212 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/__init__.c
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   244344 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/custom_font.c
+-rw-rw-rw-   0 root         (0) root         (0)     2861 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/custom_font.py
+-rw-r--r--   0 root         (0) root         (0)   378258 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/palette.c
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/palette.py
+-rw-r--r--   0 root         (0) root         (0)   472190 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/visualization.c
+-rw-rw-rw-   0 root         (0) root         (0)     7621 2023-05-22 20:11:05.000000 viso-sdk-python-0.0.8/viso_sdk/visualize/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 20:11:16.521395 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 20:11:16.000000 viso-sdk-python-0.0.8/viso_sdk_python.egg-info/top_level.txt
```

### Comparing `viso-sdk-python-0.0.7/COPYING` & `viso-sdk-python-0.0.8/COPYING`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/PKG-INFO` & `viso-sdk-python-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `viso-sdk-python-0.0.7/docs/Makefile` & `viso-sdk-python-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/docs/conf.py` & `viso-sdk-python-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/docs/ext/docstrings.py` & `viso-sdk-python-0.0.8/docs/ext/docstrings.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/docs/ext/manager_tmpl.j2` & `viso-sdk-python-0.0.8/docs/ext/manager_tmpl.j2`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/docs/make.bat` & `viso-sdk-python-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/docs/viso.rst` & `viso-sdk-python-0.0.8/docs/viso.rst`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/setup.py` & `viso-sdk-python-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tests/fixtures/flow.json` & `viso-sdk-python-0.0.8/tests/fixtures/flow.json`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tests/meta/test_ensure_type_hints.py` & `viso-sdk-python-0.0.8/tests/meta/test_ensure_type_hints.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tests/smoke/test_dists.py` & `viso-sdk-python-0.0.8/tests/smoke/test_dists.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tests/test_flow.py` & `viso-sdk-python-0.0.8/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tests/test_status.py` & `viso-sdk-python-0.0.8/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/tox.ini` & `viso-sdk-python-0.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/__init__.py` & `viso-sdk-python-0.0.8/viso_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/_version.c` & `viso-sdk-python-0.0.8/viso_sdk/_version.c`

 * *Files 0% similar despite different names*

```diff
@@ -1289,15 +1289,15 @@
 static const char __pyx_k_now[] = "now";
 static const char __pyx_k_file[] = "__file__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_year[] = "year";
-static const char __pyx_k_0_0_7[] = "0.0.7";
+static const char __pyx_k_0_0_8[] = "0.0.8";
 static const char __pyx_k_LGPL3[] = "LGPL3";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_title[] = "__title__";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_abspath[] = "abspath";
 static const char __pyx_k_cur_dir[] = "_cur_dir";
@@ -1309,15 +1309,15 @@
 static const char __pyx_k_Viso_ai_team[] = "Viso.ai team";
 static const char __pyx_k_Constant_file[] = "\n    Constant file\n";
 static const char __pyx_k_Copyright_2020[] = "Copyright 2020-";
 static const char __pyx_k_viso_sdk_python[] = "viso-sdk-python";
 static const char __pyx_k_s_carlyon_viso_ai[] = "s.carlyon@viso.ai";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_viso_ai_AG_info_viso_ai[] = " viso.ai AG <info@viso.ai>";
-static PyObject *__pyx_kp_u_0_0_7;
+static PyObject *__pyx_kp_u_0_0_8;
 static PyObject *__pyx_kp_u_Copyright_2020;
 static PyObject *__pyx_n_u_LGPL3;
 static PyObject *__pyx_kp_u_Viso_ai_team;
 static PyObject *__pyx_n_s_abspath;
 static PyObject *__pyx_n_s_author;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_copyright;
@@ -1384,15 +1384,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_0_7, __pyx_k_0_0_7, sizeof(__pyx_k_0_0_7), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_0_8, __pyx_k_0_0_8, sizeof(__pyx_k_0_0_8), 0, 1, 0, 0},
   {&__pyx_kp_u_Copyright_2020, __pyx_k_Copyright_2020, sizeof(__pyx_k_Copyright_2020), 0, 1, 0, 0},
   {&__pyx_n_u_LGPL3, __pyx_k_LGPL3, sizeof(__pyx_k_LGPL3), 0, 1, 0, 1},
   {&__pyx_kp_u_Viso_ai_team, __pyx_k_Viso_ai_team, sizeof(__pyx_k_Viso_ai_team), 0, 1, 0, 0},
   {&__pyx_n_s_abspath, __pyx_k_abspath, sizeof(__pyx_k_abspath), 0, 0, 1, 1},
   {&__pyx_n_s_author, __pyx_k_author, sizeof(__pyx_k_author), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_copyright, __pyx_k_copyright, sizeof(__pyx_k_copyright), 0, 0, 1, 1},
@@ -1870,24 +1870,24 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_license, __pyx_n_u_LGPL3) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":15
  * __email__ = "s.carlyon@viso.ai"
  * __license__ = "LGPL3"
  * __title__ = "viso-sdk-python"             # <<<<<<<<<<<<<<
  * 
- * __version__ = "0.0.7"
+ * __version__ = "0.0.8"
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_kp_u_viso_sdk_python) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":17
  * __title__ = "viso-sdk-python"
  * 
- * __version__ = "0.0.7"             # <<<<<<<<<<<<<<
+ * __version__ = "0.0.8"             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_7) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_0_8) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "viso_sdk/_version.py":1
  * """             # <<<<<<<<<<<<<<
  *     Constant file
  * """
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `viso-sdk-python-0.0.7/viso_sdk/constants/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/constants/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/constants/constants.c` & `viso-sdk-python-0.0.8/viso_sdk/constants/constants.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/constants/constants.py` & `viso-sdk-python-0.0.8/viso_sdk/constants/constants.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/constants/modules.c` & `viso-sdk-python-0.0.8/viso_sdk/constants/modules.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/constants/variables.c` & `viso-sdk-python-0.0.8/viso_sdk/constants/variables.c`

 * *Files 6% similar despite different names*

```diff
@@ -1129,40 +1129,14 @@
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
 #endif
 
-/* PyObjectLookupSpecial.proto */
-#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name) {
-    PyObject *res;
-    PyTypeObject *tp = Py_TYPE(obj);
-#if PY_MAJOR_VERSION < 3
-    if (unlikely(PyInstance_Check(obj)))
-        return __Pyx_PyObject_GetAttrStr(obj, attr_name);
-#endif
-    res = _PyType_Lookup(tp, attr_name);
-    if (likely(res)) {
-        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
-        if (!f) {
-            Py_INCREF(res);
-        } else {
-            res = f(res, obj, (PyObject *)tp);
-        }
-    } else {
-        PyErr_SetObject(PyExc_AttributeError, attr_name);
-    }
-    return res;
-}
-#else
-#define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
-#endif
-
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -1170,77 +1144,14 @@
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* None.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
-
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -1328,14 +1239,50 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -1394,130 +1341,96 @@
 
 /* Module declarations from 'viso_sdk.constants.variables' */
 #define __Pyx_MODULE_NAME "viso_sdk.constants.variables"
 extern int __pyx_module_is_main_viso_sdk__constants__variables;
 int __pyx_module_is_main_viso_sdk__constants__variables = 0;
 
 /* Implementation of 'viso_sdk.constants.variables' */
-static PyObject *__pyx_builtin_open;
 static const char __pyx_k_[] = "";
-static const char __pyx_k_r[] = "r";
-static const char __pyx_k__4[] = "\n";
-static const char __pyx_k__7[] = "_";
+static const char __pyx_k__4[] = "_";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_get[] = "get";
-static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_logs[] = "logs";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
-static const char __pyx_k_open[] = "open";
 static const char __pyx_k_path[] = "path";
-static const char __pyx_k_read[] = "read";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_viso[] = "/viso";
-static const char __pyx_k_enter[] = "__enter__";
-static const char __pyx_k_token[] = ".token";
-static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_NODE_ID[] = "NODE_ID";
 static const char __pyx_k_environ[] = "environ";
 static const char __pyx_k_log_dir[] = "log_dir";
-static const char __pyx_k_replace[] = "replace";
 static const char __pyx_k_unknown[] = "unknown";
 static const char __pyx_k_VISO_DIR[] = "VISO_DIR";
-static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_exist_ok[] = "exist_ok";
 static const char __pyx_k_makedirs[] = "makedirs";
 static const char __pyx_k_NODE_TYPE[] = "NODE_TYPE";
-static const char __pyx_k_TOKEN_FILE[] = "TOKEN_FILE";
 static const char __pyx_k_get_log_dir[] = "get_log_dir";
 static const char __pyx_k_get_node_id[] = "get_node_id";
-static const char __pyx_k_device_token[] = "device_token";
-static const char __pyx_k_file_pointer[] = "file_pointer";
 static const char __pyx_k_get_viso_dir[] = "get_viso_dir";
 static const char __pyx_k_container_dir[] = "container_dir";
 static const char __pyx_k_get_node_type[] = "get_node_type";
 static const char __pyx_k_SLIM_SIMULATION[] = "SLIM_SIMULATION";
-static const char __pyx_k_get_device_token[] = "get_device_token";
 static const char __pyx_k_get_container_dir[] = "get_container_dir";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_viso_sdk_constants_variables[] = "viso_sdk.constants.variables";
 static const char __pyx_k_Environment_Values_Note_that_NO[] = "\nEnvironment Values\n\nNote that NODE_ID and NODE_TYPE environment variables are passed from the SolutionManager.\n\nUse these constant values in your containers to make your code simple!\n\n";
 static const char __pyx_k_viso_sdk_constants_variables_py[] = "viso_sdk/constants/variables.py";
 static PyObject *__pyx_kp_u_;
 static PyObject *__pyx_n_s_NODE_ID;
 static PyObject *__pyx_n_u_NODE_ID;
 static PyObject *__pyx_n_s_NODE_TYPE;
 static PyObject *__pyx_n_u_NODE_TYPE;
 static PyObject *__pyx_n_u_SLIM_SIMULATION;
-static PyObject *__pyx_n_s_TOKEN_FILE;
 static PyObject *__pyx_n_s_VISO_DIR;
-static PyObject *__pyx_kp_u__4;
-static PyObject *__pyx_n_u__7;
+static PyObject *__pyx_n_u__4;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_container_dir;
-static PyObject *__pyx_n_s_device_token;
-static PyObject *__pyx_n_s_encoding;
-static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_environ;
 static PyObject *__pyx_n_s_exist_ok;
-static PyObject *__pyx_n_s_exit;
-static PyObject *__pyx_n_s_file_pointer;
 static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_get_container_dir;
-static PyObject *__pyx_n_s_get_device_token;
 static PyObject *__pyx_n_s_get_log_dir;
 static PyObject *__pyx_n_s_get_node_id;
 static PyObject *__pyx_n_s_get_node_type;
 static PyObject *__pyx_n_s_get_viso_dir;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_log_dir;
 static PyObject *__pyx_n_u_logs;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_makedirs;
 static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_n_s_path;
-static PyObject *__pyx_n_u_r;
-static PyObject *__pyx_n_s_read;
-static PyObject *__pyx_n_s_replace;
 static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_kp_u_token;
 static PyObject *__pyx_n_u_unknown;
-static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_kp_u_viso;
 static PyObject *__pyx_n_s_viso_sdk_constants_variables;
 static PyObject *__pyx_kp_s_viso_sdk_constants_variables_py;
 static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_get_node_id(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_2get_node_type(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_4get_device_token(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_6get_container_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_8get_viso_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_10get_log_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_4get_container_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_6get_viso_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_8get_log_dir(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__17;
-static PyObject *__pyx_codeobj__9;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__16;
-static PyObject *__pyx_codeobj__18;
 /* Late includes */
 
-/* "viso_sdk/constants/variables.py":20
+/* "viso_sdk/constants/variables.py":17
  * 
  * 
  * def get_node_id():             # <<<<<<<<<<<<<<
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  */
 
@@ -1546,38 +1459,38 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_node_id", 0);
 
-  /* "viso_sdk/constants/variables.py":23
+  /* "viso_sdk/constants/variables.py":20
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  *     NODE_ID: str = os.environ.get("SLIM_SIMULATION", os.environ.get("NODE_ID", ""))             # <<<<<<<<<<<<<<
  *     return NODE_ID
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_environ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_environ); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_environ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -1587,63 +1500,63 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_n_u_SLIM_SIMULATION, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_n_u_SLIM_SIMULATION, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_SLIM_SIMULATION);
     __Pyx_GIVEREF(__pyx_n_u_SLIM_SIMULATION);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_n_u_SLIM_SIMULATION);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 20, __pyx_L1_error)
   __pyx_v_NODE_ID = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":24
+  /* "viso_sdk/constants/variables.py":21
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  *     NODE_ID: str = os.environ.get("SLIM_SIMULATION", os.environ.get("NODE_ID", ""))
  *     return NODE_ID             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_NODE_ID);
   __pyx_r = __pyx_v_NODE_ID;
   goto __pyx_L0;
 
-  /* "viso_sdk/constants/variables.py":20
+  /* "viso_sdk/constants/variables.py":17
  * 
  * 
  * def get_node_id():             # <<<<<<<<<<<<<<
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  */
 
@@ -1659,15 +1572,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_NODE_ID);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/constants/variables.py":27
+/* "viso_sdk/constants/variables.py":24
  * 
  * 
  * def get_node_type():             # <<<<<<<<<<<<<<
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")
  */
 
@@ -1692,49 +1605,49 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_node_type", 0);
 
-  /* "viso_sdk/constants/variables.py":29
+  /* "viso_sdk/constants/variables.py":26
  * def get_node_type():
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")             # <<<<<<<<<<<<<<
  *     return NODE_TYPE
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_environ); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_environ); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_2)->tp_name), 0))) __PYX_ERR(0, 26, __pyx_L1_error)
   __pyx_v_NODE_TYPE = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "viso_sdk/constants/variables.py":30
+  /* "viso_sdk/constants/variables.py":27
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")
  *     return NODE_TYPE             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_NODE_TYPE);
   __pyx_r = __pyx_v_NODE_TYPE;
   goto __pyx_L0;
 
-  /* "viso_sdk/constants/variables.py":27
+  /* "viso_sdk/constants/variables.py":24
  * 
  * 
  * def get_node_type():             # <<<<<<<<<<<<<<
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")
  */
 
@@ -1747,291 +1660,37 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_NODE_TYPE);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/constants/variables.py":33
- * 
- * 
- * def get_device_token():             # <<<<<<<<<<<<<<
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_5get_device_token(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_8viso_sdk_9constants_9variables_4get_device_token[] = "Read device token from a file";
-static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_5get_device_token = {"get_device_token", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_5get_device_token, METH_NOARGS, __pyx_doc_8viso_sdk_9constants_9variables_4get_device_token};
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_5get_device_token(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_device_token (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_4get_device_token(__pyx_self);
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_4get_device_token(CYTHON_UNUSED PyObject *__pyx_self) {
-  PyObject *__pyx_v_file_pointer = NULL;
-  PyObject *__pyx_v_device_token = NULL;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
-  int __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_device_token", 0);
-
-  /* "viso_sdk/constants/variables.py":35
- * def get_device_token():
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:             # <<<<<<<<<<<<<<
- *         device_token = file_pointer.read().replace("\n", "")
- *     return device_token
- */
-  /*with:*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TOKEN_FILE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-    __Pyx_INCREF(__pyx_n_u_r);
-    __Pyx_GIVEREF(__pyx_n_u_r);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_r);
-    __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 35, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 35, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_LookupSpecial(__pyx_t_3, __pyx_n_s_enter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L3_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
-      }
-    }
-    __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L3_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __pyx_t_1;
-    __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    /*try:*/ {
-      {
-        __Pyx_PyThreadState_declare
-        __Pyx_PyThreadState_assign
-        __Pyx_ExceptionSave(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8);
-        __Pyx_XGOTREF(__pyx_t_6);
-        __Pyx_XGOTREF(__pyx_t_7);
-        __Pyx_XGOTREF(__pyx_t_8);
-        /*try:*/ {
-          __pyx_v_file_pointer = __pyx_t_2;
-          __pyx_t_2 = 0;
-
-          /* "viso_sdk/constants/variables.py":36
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- *         device_token = file_pointer.read().replace("\n", "")             # <<<<<<<<<<<<<<
- *     return device_token
- * 
- */
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_file_pointer, __pyx_n_s_read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_1 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-            __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
-            if (likely(__pyx_t_1)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-              __Pyx_INCREF(__pyx_t_1);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_3, function);
-            }
-          }
-          __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_replace); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 36, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L7_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_v_device_token = __pyx_t_2;
-          __pyx_t_2 = 0;
-
-          /* "viso_sdk/constants/variables.py":35
- * def get_device_token():
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:             # <<<<<<<<<<<<<<
- *         device_token = file_pointer.read().replace("\n", "")
- *     return device_token
- */
-        }
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        goto __pyx_L12_try_end;
-        __pyx_L7_error:;
-        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-        /*except:*/ {
-          __Pyx_AddTraceback("viso_sdk.constants.variables.get_device_token", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_1) < 0) __PYX_ERR(0, 35, __pyx_L9_except_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L9_except_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L9_except_error)
-          __Pyx_GOTREF(__pyx_t_9);
-          __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_9);
-          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          if (__pyx_t_10 < 0) __PYX_ERR(0, 35, __pyx_L9_except_error)
-          __pyx_t_11 = ((!(__pyx_t_10 != 0)) != 0);
-          if (__pyx_t_11) {
-            __Pyx_GIVEREF(__pyx_t_2);
-            __Pyx_GIVEREF(__pyx_t_3);
-            __Pyx_XGIVEREF(__pyx_t_1);
-            __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_3, __pyx_t_1);
-            __pyx_t_2 = 0; __pyx_t_3 = 0; __pyx_t_1 = 0; 
-            __PYX_ERR(0, 35, __pyx_L9_except_error)
-          }
-          __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-          goto __pyx_L8_exception_handled;
-        }
-        __pyx_L9_except_error:;
-        __Pyx_XGIVEREF(__pyx_t_6);
-        __Pyx_XGIVEREF(__pyx_t_7);
-        __Pyx_XGIVEREF(__pyx_t_8);
-        __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
-        goto __pyx_L1_error;
-        __pyx_L8_exception_handled:;
-        __Pyx_XGIVEREF(__pyx_t_6);
-        __Pyx_XGIVEREF(__pyx_t_7);
-        __Pyx_XGIVEREF(__pyx_t_8);
-        __Pyx_ExceptionReset(__pyx_t_6, __pyx_t_7, __pyx_t_8);
-        __pyx_L12_try_end:;
-      }
-    }
-    /*finally:*/ {
-      /*normal exit:*/{
-        if (__pyx_t_4) {
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__6, NULL);
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 35, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        }
-        goto __pyx_L6;
-      }
-      __pyx_L6:;
-    }
-    goto __pyx_L16;
-    __pyx_L3_error:;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    goto __pyx_L1_error;
-    __pyx_L16:;
-  }
-
-  /* "viso_sdk/constants/variables.py":37
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- *         device_token = file_pointer.read().replace("\n", "")
- *     return device_token             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_device_token)) { __Pyx_RaiseUnboundLocalError("device_token"); __PYX_ERR(0, 37, __pyx_L1_error) }
-  __Pyx_INCREF(__pyx_v_device_token);
-  __pyx_r = __pyx_v_device_token;
-  goto __pyx_L0;
-
-  /* "viso_sdk/constants/variables.py":33
- * 
- * 
- * def get_device_token():             # <<<<<<<<<<<<<<
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("viso_sdk.constants.variables.get_device_token", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_file_pointer);
-  __Pyx_XDECREF(__pyx_v_device_token);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "viso_sdk/constants/variables.py":40
+/* "viso_sdk/constants/variables.py":30
  * 
  * 
  * def get_container_dir():             # <<<<<<<<<<<<<<
  *     NODE_ID = get_node_id()
  *     NODE_TYPE = get_node_type()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_7get_container_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_7get_container_dir = {"get_container_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_7get_container_dir, METH_NOARGS, 0};
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_7get_container_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_5get_container_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_5get_container_dir = {"get_container_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_5get_container_dir, METH_NOARGS, 0};
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_5get_container_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_container_dir (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_6get_container_dir(__pyx_self);
+  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_4get_container_dir(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_6get_container_dir(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_4get_container_dir(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_v_NODE_ID = NULL;
   PyObject *__pyx_v_NODE_TYPE = NULL;
   PyObject *__pyx_v_container_dir = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -2043,108 +1702,108 @@
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_container_dir", 0);
 
-  /* "viso_sdk/constants/variables.py":41
+  /* "viso_sdk/constants/variables.py":31
  * 
  * def get_container_dir():
  *     NODE_ID = get_node_id()             # <<<<<<<<<<<<<<
  *     NODE_TYPE = get_node_type()
  *     # Root directory where all log files, model files, etc are located.
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_node_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_node_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_NODE_ID = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":42
+  /* "viso_sdk/constants/variables.py":32
  * def get_container_dir():
  *     NODE_ID = get_node_id()
  *     NODE_TYPE = get_node_type()             # <<<<<<<<<<<<<<
  *     # Root directory where all log files, model files, etc are located.
  *     container_dir: str = os.path.join(VISO_DIR, f"{NODE_TYPE}_{NODE_ID}")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_node_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_node_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_NODE_TYPE = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":44
+  /* "viso_sdk/constants/variables.py":34
  *     NODE_TYPE = get_node_type()
  *     # Root directory where all log files, model files, etc are located.
  *     container_dir: str = os.path.join(VISO_DIR, f"{NODE_TYPE}_{NODE_ID}")             # <<<<<<<<<<<<<<
  *     os.makedirs(container_dir, exist_ok=True)
  *     return container_dir
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VISO_DIR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_VISO_DIR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = 0;
   __pyx_t_6 = 127;
-  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_NODE_TYPE, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_NODE_TYPE, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
   __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
   __pyx_t_7 = 0;
-  __Pyx_INCREF(__pyx_n_u__7);
+  __Pyx_INCREF(__pyx_n_u__4);
   __pyx_t_5 += 1;
-  __Pyx_GIVEREF(__pyx_n_u__7);
-  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u__7);
-  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_NODE_ID, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_n_u__4);
+  PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u__4);
+  __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_NODE_ID, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
   __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_7);
   __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
@@ -2154,92 +1813,92 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_7);
     __pyx_t_3 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 34, __pyx_L1_error)
   __pyx_v_container_dir = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":45
+  /* "viso_sdk/constants/variables.py":35
  *     # Root directory where all log files, model files, etc are located.
  *     container_dir: str = os.path.join(VISO_DIR, f"{NODE_TYPE}_{NODE_ID}")
  *     os.makedirs(container_dir, exist_ok=True)             # <<<<<<<<<<<<<<
  *     return container_dir
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_container_dir);
   __Pyx_GIVEREF(__pyx_v_container_dir);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_container_dir);
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_exist_ok, Py_True) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_exist_ok, Py_True) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "viso_sdk/constants/variables.py":46
+  /* "viso_sdk/constants/variables.py":36
  *     container_dir: str = os.path.join(VISO_DIR, f"{NODE_TYPE}_{NODE_ID}")
  *     os.makedirs(container_dir, exist_ok=True)
  *     return container_dir             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_container_dir);
   __pyx_r = __pyx_v_container_dir;
   goto __pyx_L0;
 
-  /* "viso_sdk/constants/variables.py":40
+  /* "viso_sdk/constants/variables.py":30
  * 
  * 
  * def get_container_dir():             # <<<<<<<<<<<<<<
  *     NODE_ID = get_node_id()
  *     NODE_TYPE = get_node_type()
  */
 
@@ -2258,60 +1917,60 @@
   __Pyx_XDECREF(__pyx_v_NODE_TYPE);
   __Pyx_XDECREF(__pyx_v_container_dir);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/constants/variables.py":49
+/* "viso_sdk/constants/variables.py":39
  * 
  * 
  * def get_viso_dir():             # <<<<<<<<<<<<<<
  *     return VISO_DIR
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_9get_viso_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_9get_viso_dir = {"get_viso_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_9get_viso_dir, METH_NOARGS, 0};
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_9get_viso_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_7get_viso_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_7get_viso_dir = {"get_viso_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_7get_viso_dir, METH_NOARGS, 0};
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_7get_viso_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_viso_dir (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_8get_viso_dir(__pyx_self);
+  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_6get_viso_dir(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_8get_viso_dir(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_6get_viso_dir(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_viso_dir", 0);
 
-  /* "viso_sdk/constants/variables.py":50
+  /* "viso_sdk/constants/variables.py":40
  * 
  * def get_viso_dir():
  *     return VISO_DIR             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_VISO_DIR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_VISO_DIR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "viso_sdk/constants/variables.py":49
+  /* "viso_sdk/constants/variables.py":39
  * 
  * 
  * def get_viso_dir():             # <<<<<<<<<<<<<<
  *     return VISO_DIR
  * 
  */
 
@@ -2322,91 +1981,91 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viso_sdk/constants/variables.py":53
+/* "viso_sdk/constants/variables.py":43
  * 
  * 
  * def get_log_dir():             # <<<<<<<<<<<<<<
  *     # Log file directory
  *     container_dir = get_container_dir()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_11get_log_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_11get_log_dir = {"get_log_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_11get_log_dir, METH_NOARGS, 0};
-static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_11get_log_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_9get_log_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_8viso_sdk_9constants_9variables_9get_log_dir = {"get_log_dir", (PyCFunction)__pyx_pw_8viso_sdk_9constants_9variables_9get_log_dir, METH_NOARGS, 0};
+static PyObject *__pyx_pw_8viso_sdk_9constants_9variables_9get_log_dir(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_log_dir (wrapper)", 0);
-  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_10get_log_dir(__pyx_self);
+  __pyx_r = __pyx_pf_8viso_sdk_9constants_9variables_8get_log_dir(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_10get_log_dir(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8viso_sdk_9constants_9variables_8get_log_dir(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_v_container_dir = NULL;
   PyObject *__pyx_v_log_dir = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_log_dir", 0);
 
-  /* "viso_sdk/constants/variables.py":55
+  /* "viso_sdk/constants/variables.py":45
  * def get_log_dir():
  *     # Log file directory
  *     container_dir = get_container_dir()             # <<<<<<<<<<<<<<
  *     log_dir: str = os.path.join(container_dir, "logs")
  *     os.makedirs(log_dir, exist_ok=True)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_container_dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_container_dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_container_dir = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":56
+  /* "viso_sdk/constants/variables.py":46
  *     # Log file directory
  *     container_dir = get_container_dir()
  *     log_dir: str = os.path.join(container_dir, "logs")             # <<<<<<<<<<<<<<
  *     os.makedirs(log_dir, exist_ok=True)
  *     return log_dir
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_join); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -2416,85 +2075,85 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_container_dir, __pyx_n_u_logs};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_container_dir, __pyx_n_u_logs};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_container_dir);
     __Pyx_GIVEREF(__pyx_v_container_dir);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_container_dir);
     __Pyx_INCREF(__pyx_n_u_logs);
     __Pyx_GIVEREF(__pyx_n_u_logs);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_n_u_logs);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 56, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_v_log_dir = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":57
+  /* "viso_sdk/constants/variables.py":47
  *     container_dir = get_container_dir()
  *     log_dir: str = os.path.join(container_dir, "logs")
  *     os.makedirs(log_dir, exist_ok=True)             # <<<<<<<<<<<<<<
  *     return log_dir
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_makedirs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_log_dir);
   __Pyx_GIVEREF(__pyx_v_log_dir);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_log_dir);
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_exist_ok, Py_True) < 0) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_exist_ok, Py_True) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viso_sdk/constants/variables.py":58
+  /* "viso_sdk/constants/variables.py":48
  *     log_dir: str = os.path.join(container_dir, "logs")
  *     os.makedirs(log_dir, exist_ok=True)
  *     return log_dir             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_log_dir);
   __pyx_r = __pyx_v_log_dir;
   goto __pyx_L0;
 
-  /* "viso_sdk/constants/variables.py":53
+  /* "viso_sdk/constants/variables.py":43
  * 
  * 
  * def get_log_dir():             # <<<<<<<<<<<<<<
  *     # Log file directory
  *     container_dir = get_container_dir()
  */
 
@@ -2562,179 +2221,128 @@
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
   {&__pyx_n_s_NODE_ID, __pyx_k_NODE_ID, sizeof(__pyx_k_NODE_ID), 0, 0, 1, 1},
   {&__pyx_n_u_NODE_ID, __pyx_k_NODE_ID, sizeof(__pyx_k_NODE_ID), 0, 1, 0, 1},
   {&__pyx_n_s_NODE_TYPE, __pyx_k_NODE_TYPE, sizeof(__pyx_k_NODE_TYPE), 0, 0, 1, 1},
   {&__pyx_n_u_NODE_TYPE, __pyx_k_NODE_TYPE, sizeof(__pyx_k_NODE_TYPE), 0, 1, 0, 1},
   {&__pyx_n_u_SLIM_SIMULATION, __pyx_k_SLIM_SIMULATION, sizeof(__pyx_k_SLIM_SIMULATION), 0, 1, 0, 1},
-  {&__pyx_n_s_TOKEN_FILE, __pyx_k_TOKEN_FILE, sizeof(__pyx_k_TOKEN_FILE), 0, 0, 1, 1},
   {&__pyx_n_s_VISO_DIR, __pyx_k_VISO_DIR, sizeof(__pyx_k_VISO_DIR), 0, 0, 1, 1},
-  {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-  {&__pyx_n_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 1},
+  {&__pyx_n_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_container_dir, __pyx_k_container_dir, sizeof(__pyx_k_container_dir), 0, 0, 1, 1},
-  {&__pyx_n_s_device_token, __pyx_k_device_token, sizeof(__pyx_k_device_token), 0, 0, 1, 1},
-  {&__pyx_n_s_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 0, 1, 1},
-  {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_environ, __pyx_k_environ, sizeof(__pyx_k_environ), 0, 0, 1, 1},
   {&__pyx_n_s_exist_ok, __pyx_k_exist_ok, sizeof(__pyx_k_exist_ok), 0, 0, 1, 1},
-  {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
-  {&__pyx_n_s_file_pointer, __pyx_k_file_pointer, sizeof(__pyx_k_file_pointer), 0, 0, 1, 1},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_get_container_dir, __pyx_k_get_container_dir, sizeof(__pyx_k_get_container_dir), 0, 0, 1, 1},
-  {&__pyx_n_s_get_device_token, __pyx_k_get_device_token, sizeof(__pyx_k_get_device_token), 0, 0, 1, 1},
   {&__pyx_n_s_get_log_dir, __pyx_k_get_log_dir, sizeof(__pyx_k_get_log_dir), 0, 0, 1, 1},
   {&__pyx_n_s_get_node_id, __pyx_k_get_node_id, sizeof(__pyx_k_get_node_id), 0, 0, 1, 1},
   {&__pyx_n_s_get_node_type, __pyx_k_get_node_type, sizeof(__pyx_k_get_node_type), 0, 0, 1, 1},
   {&__pyx_n_s_get_viso_dir, __pyx_k_get_viso_dir, sizeof(__pyx_k_get_viso_dir), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_log_dir, __pyx_k_log_dir, sizeof(__pyx_k_log_dir), 0, 0, 1, 1},
   {&__pyx_n_u_logs, __pyx_k_logs, sizeof(__pyx_k_logs), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_makedirs, __pyx_k_makedirs, sizeof(__pyx_k_makedirs), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
-  {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
-  {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
-  {&__pyx_n_s_replace, __pyx_k_replace, sizeof(__pyx_k_replace), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_kp_u_token, __pyx_k_token, sizeof(__pyx_k_token), 0, 1, 0, 0},
   {&__pyx_n_u_unknown, __pyx_k_unknown, sizeof(__pyx_k_unknown), 0, 1, 0, 1},
-  {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_kp_u_viso, __pyx_k_viso, sizeof(__pyx_k_viso), 0, 1, 0, 0},
   {&__pyx_n_s_viso_sdk_constants_variables, __pyx_k_viso_sdk_constants_variables, sizeof(__pyx_k_viso_sdk_constants_variables), 0, 0, 1, 1},
   {&__pyx_kp_s_viso_sdk_constants_variables_py, __pyx_k_viso_sdk_constants_variables_py, sizeof(__pyx_k_viso_sdk_constants_variables_py), 0, 0, 1, 0},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 35, __pyx_L1_error)
   return 0;
-  __pyx_L1_error:;
-  return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "viso_sdk/constants/variables.py":23
+  /* "viso_sdk/constants/variables.py":20
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  *     NODE_ID: str = os.environ.get("SLIM_SIMULATION", os.environ.get("NODE_ID", ""))             # <<<<<<<<<<<<<<
  *     return NODE_ID
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_NODE_ID, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(2, __pyx_n_u_NODE_ID, __pyx_kp_u_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "viso_sdk/constants/variables.py":29
+  /* "viso_sdk/constants/variables.py":26
  * def get_node_type():
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")             # <<<<<<<<<<<<<<
  *     return NODE_TYPE
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_NODE_TYPE, __pyx_n_u_unknown); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_n_u_NODE_TYPE, __pyx_n_u_unknown); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "viso_sdk/constants/variables.py":36
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- *         device_token = file_pointer.read().replace("\n", "")             # <<<<<<<<<<<<<<
- *     return device_token
- * 
- */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_u__4, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 36, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-
-  /* "viso_sdk/constants/variables.py":35
- * def get_device_token():
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:             # <<<<<<<<<<<<<<
- *         device_token = file_pointer.read().replace("\n", "")
- *     return device_token
- */
-  __pyx_tuple__6 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-
-  /* "viso_sdk/constants/variables.py":20
+  /* "viso_sdk/constants/variables.py":17
  * 
  * 
  * def get_node_id():             # <<<<<<<<<<<<<<
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_n_s_NODE_ID); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_node_id, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_NODE_ID); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_node_id, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 17, __pyx_L1_error)
 
-  /* "viso_sdk/constants/variables.py":27
+  /* "viso_sdk/constants/variables.py":24
  * 
  * 
  * def get_node_type():             # <<<<<<<<<<<<<<
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_n_s_NODE_TYPE); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_node_type, 27, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_n_s_NODE_TYPE); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_node_type, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "viso_sdk/constants/variables.py":33
- * 
- * 
- * def get_device_token():             # <<<<<<<<<<<<<<
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_file_pointer, __pyx_n_s_device_token); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 33, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_device_token, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 33, __pyx_L1_error)
-
-  /* "viso_sdk/constants/variables.py":40
+  /* "viso_sdk/constants/variables.py":30
  * 
  * 
  * def get_container_dir():             # <<<<<<<<<<<<<<
  *     NODE_ID = get_node_id()
  *     NODE_TYPE = get_node_type()
  */
-  __pyx_tuple__14 = PyTuple_Pack(3, __pyx_n_s_NODE_ID, __pyx_n_s_NODE_TYPE, __pyx_n_s_container_dir); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_container_dir, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_n_s_NODE_ID, __pyx_n_s_NODE_TYPE, __pyx_n_s_container_dir); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_container_dir, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "viso_sdk/constants/variables.py":49
+  /* "viso_sdk/constants/variables.py":39
  * 
  * 
  * def get_viso_dir():             # <<<<<<<<<<<<<<
  *     return VISO_DIR
  * 
  */
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_viso_dir, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_viso_dir, 39, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 39, __pyx_L1_error)
 
-  /* "viso_sdk/constants/variables.py":53
+  /* "viso_sdk/constants/variables.py":43
  * 
  * 
  * def get_log_dir():             # <<<<<<<<<<<<<<
  *     # Log file directory
  *     container_dir = get_container_dir()
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_container_dir, __pyx_n_s_log_dir); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_log_dir, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_container_dir, __pyx_n_s_log_dir); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_viso_sdk_constants_variables_py, __pyx_n_s_get_log_dir, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2900,16 +2508,14 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_variables(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -3024,140 +2630,94 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "viso_sdk/constants/variables.py":14
  * 
  * # Viso directory where all Viso containers are using.
  * VISO_DIR: str = "/viso"             # <<<<<<<<<<<<<<
  * 
- * # Token file that can be used for Viso API Calls.
+ * 
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_VISO_DIR, __pyx_kp_u_viso) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
 
   /* "viso_sdk/constants/variables.py":17
  * 
- * # Token file that can be used for Viso API Calls.
- * TOKEN_FILE: str = os.path.join(VISO_DIR, ".token")             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_join); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_VISO_DIR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
-  __Pyx_INCREF(__pyx_kp_u_token);
-  __Pyx_GIVEREF(__pyx_kp_u_token);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_kp_u_token);
-  __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TOKEN_FILE, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "viso_sdk/constants/variables.py":20
- * 
  * 
  * def get_node_id():             # <<<<<<<<<<<<<<
  *     # Node ID in the flow.
  *     # Use `SLIM_SIMULATION` value if set, otherwise, use correct value
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_1get_node_id, 0, __pyx_n_s_get_node_id, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_node_id, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_1get_node_id, 0, __pyx_n_s_get_node_id, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_node_id, __pyx_t_1) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":27
+  /* "viso_sdk/constants/variables.py":24
  * 
  * 
  * def get_node_type():             # <<<<<<<<<<<<<<
  *     # Node type in the flow
  *     NODE_TYPE: str = os.environ.get("NODE_TYPE", "unknown")
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_3get_node_type, 0, __pyx_n_s_get_node_type, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_node_type, __pyx_t_2) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "viso_sdk/constants/variables.py":33
- * 
- * 
- * def get_device_token():             # <<<<<<<<<<<<<<
- *     """Read device token from a file"""
- *     with open(TOKEN_FILE, "r", encoding="utf-8") as file_pointer:
- */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_5get_device_token, 0, __pyx_n_s_get_device_token, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_device_token, __pyx_t_2) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_3get_node_type, 0, __pyx_n_s_get_node_type, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_node_type, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":40
+  /* "viso_sdk/constants/variables.py":30
  * 
  * 
  * def get_container_dir():             # <<<<<<<<<<<<<<
  *     NODE_ID = get_node_id()
  *     NODE_TYPE = get_node_type()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_7get_container_dir, 0, __pyx_n_s_get_container_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_container_dir, __pyx_t_2) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_5get_container_dir, 0, __pyx_n_s_get_container_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_container_dir, __pyx_t_1) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":49
+  /* "viso_sdk/constants/variables.py":39
  * 
  * 
  * def get_viso_dir():             # <<<<<<<<<<<<<<
  *     return VISO_DIR
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_9get_viso_dir, 0, __pyx_n_s_get_viso_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_viso_dir, __pyx_t_2) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_7get_viso_dir, 0, __pyx_n_s_get_viso_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_viso_dir, __pyx_t_1) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viso_sdk/constants/variables.py":53
+  /* "viso_sdk/constants/variables.py":43
  * 
  * 
  * def get_log_dir():             # <<<<<<<<<<<<<<
  *     # Log file directory
  *     container_dir = get_container_dir()
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_11get_log_dir, 0, __pyx_n_s_get_log_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_log_dir, __pyx_t_2) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8viso_sdk_9constants_9variables_9get_log_dir, 0, __pyx_n_s_get_log_dir, NULL, __pyx_n_s_viso_sdk_constants_variables, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_log_dir, __pyx_t_1) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "viso_sdk/constants/variables.py":2
  * 
  * """             # <<<<<<<<<<<<<<
  * Environment Values
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init viso_sdk.constants.variables", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init viso_sdk.constants.variables");
@@ -3520,173 +3080,14 @@
     if (unlikely(!args)) return NULL;
     result = __Pyx_PyObject_Call(func, args, NULL);
     Py_DECREF(args);
     return result;
 }
 #endif
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* None */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
-}
-
 /* JoinPyUnicode */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       CYTHON_UNUSED Py_UCS4 max_char) {
 #if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     PyObject *result_uval;
     int result_ukind;
     Py_ssize_t i, char_pos;
@@ -4474,14 +3875,38 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
```

### Comparing `viso-sdk-python-0.0.7/viso_sdk/edge/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/edge/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/edge/common.c` & `viso-sdk-python-0.0.8/viso_sdk/edge/common.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/edge/common.py` & `viso-sdk-python-0.0.8/viso_sdk/edge/common.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/logging/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/logging/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/logging/logger.c` & `viso-sdk-python-0.0.8/viso_sdk/logging/logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/logging/logger.py` & `viso-sdk-python-0.0.8/viso_sdk/logging/logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/logging/status_logger.c` & `viso-sdk-python-0.0.8/viso_sdk/logging/status_logger.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/logging/status_logger.py` & `viso-sdk-python-0.0.8/viso_sdk/logging/status_logger.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/mqtt/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/mqtt/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/mqtt/mqtt_wrapper.c` & `viso-sdk-python-0.0.8/viso_sdk/mqtt/mqtt_wrapper.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/mqtt/mqtt_wrapper.py` & `viso-sdk-python-0.0.8/viso_sdk/mqtt/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/nodered/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/nodered/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/nodered/flow.c` & `viso-sdk-python-0.0.8/viso_sdk/nodered/flow.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/nodered/flow.py` & `viso-sdk-python-0.0.8/viso_sdk/nodered/flow.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/redis/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/redis/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/redis/redis_wrapper.c` & `viso-sdk-python-0.0.8/viso_sdk/redis/redis_wrapper.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/redis/redis_wrapper.py` & `viso-sdk-python-0.0.8/viso_sdk/redis/redis_wrapper.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/__init__.c` & `viso-sdk-python-0.0.8/viso_sdk/visualize/__init__.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/custom_font.c` & `viso-sdk-python-0.0.8/viso_sdk/visualize/custom_font.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/custom_font.py` & `viso-sdk-python-0.0.8/viso_sdk/visualize/custom_font.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/palette.c` & `viso-sdk-python-0.0.8/viso_sdk/visualize/palette.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/palette.py` & `viso-sdk-python-0.0.8/viso_sdk/visualize/palette.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/visualization.c` & `viso-sdk-python-0.0.8/viso_sdk/visualize/visualization.c`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk/visualize/visualization.py` & `viso-sdk-python-0.0.8/viso_sdk/visualize/visualization.py`

 * *Files identical despite different names*

### Comparing `viso-sdk-python-0.0.7/viso_sdk_python.egg-info/PKG-INFO` & `viso-sdk-python-0.0.8/viso_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viso-sdk-python
-Version: 0.0.7
+Version: 0.0.8
 Summary: VisoSDK: A Python SDK for use in Viso containers
 Home-page: https://gitlab.com/TopKamera/03_edge/Base/viso-sdk-python-public.git
 Author: support@viso.ai
 Author-email: support@viso.ai
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `viso-sdk-python-0.0.7/viso_sdk_python.egg-info/SOURCES.txt` & `viso-sdk-python-0.0.8/viso_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

