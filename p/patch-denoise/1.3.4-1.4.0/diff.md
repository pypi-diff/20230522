# Comparing `tmp/patch-denoise-1.3.4.tar.gz` & `tmp/patch-denoise-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patch-denoise-1.3.4.tar", last modified: Wed Mar 15 13:28:54 2023, max compression
+gzip compressed data, was "patch-denoise-1.4.0.tar", last modified: Mon May 22 08:29:23 2023, max compression
```

## Comparing `patch-denoise-1.3.4.tar` & `patch-denoise-1.4.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.743160 patch-denoise-1.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.731160 patch-denoise-1.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.731160 patch-denoise-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-15 13:28:54.743160 patch-denoise-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.735160 patch-denoise-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.735160 patch-denoise-1.3.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/denoisers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.735160 patch-denoise-1.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/examples/example_experimental_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/examples/example_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 13:28:54.743160 patch-denoise-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.731160 patch-denoise-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.735160 patch-denoise-1.3.4/src/patch_denoise/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.739160 patch-denoise-1.3.4/src/patch_denoise/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/bindings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/bindings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/bindings/modopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/bindings/nipype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/bindings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/denoise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.739160 patch-denoise-1.3.4/src/patch_denoise/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/simulation/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/simulation/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/simulation/phantom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.739160 patch-denoise-1.3.4/src/patch_denoise/space_time/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/space_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/space_time/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/space_time/lowrank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/space_time/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.739160 patch-denoise-1.3.4/src/patch_denoise/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/viz/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/src/patch_denoise/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.739160 patch-denoise-1.3.4/src/patch_denoise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 13:28:54.000000 patch-denoise-1.3.4/src/patch_denoise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:54.743160 patch-denoise-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/test_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/test_spacetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-15 13:28:16.000000 patch-denoise-1.3.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/denoisers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/example_experimental_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/example_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/modopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/nipype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/denoise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/phantom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/space_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/lowrank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_spacetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_utils.py
```

### Comparing `patch-denoise-1.3.4/.github/workflows/master-cd.yml` & `patch-denoise-1.4.0/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/.github/workflows/tags-release.yml` & `patch-denoise-1.4.0/.github/workflows/tags-release.yml`

 * *Files 27% similar despite different names*

```diff
@@ -29,7 +29,17 @@
       run: |
         python -m build --sdist --wheel --outdir dist/ .
 
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_TOKEN_RESTRICTED }}
+    
+    - name: Create release
+      uses: actions/create-release@v1
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided by Actions, you do not need to create your own token
+      with:
+        tag_name: ${{ github.ref }}
+        release_name: Release ${{ github.ref }}
+        draft: true
+        prerelease: false
```

### Comparing `patch-denoise-1.3.4/.github/workflows/test-ci.yml` & `patch-denoise-1.4.0/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/LICENSE.txt` & `patch-denoise-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/PKG-INFO` & `patch-denoise-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-denoise
-Version: 1.3.4
+Version: 1.4.0
 Summary: Denoising method for sequence of images or volumes. Primarly targeting fMRI data.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -138,7 +138,18 @@
         MONTH = Apr,
         KEYWORDS = {functional MRI ; patch denoising ; singular value thresholding ; functional MRI patch denoising singular value thresholding},
         PDF = {https://hal.science/hal-03895194/file/isbi2023_denoise.pdf},
         HAL_ID = {hal-03895194},
         HAL_VERSION = {v1},
       }
 
+
+Related Packages
+================
+
+- https://github.com/paquiteau/retino-pypeline
+
+  For the application of the denoising in an fMRI pypeline using Nipype
+
+- https://github.com/CEA-COSMIC/ModOpt
+
+  For the integration of the patch-denoising in convex optimisation algorithms.
```

### Comparing `patch-denoise-1.3.4/README.rst` & `patch-denoise-1.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -89,7 +89,18 @@
         MONTH = Apr,
         KEYWORDS = {functional MRI ; patch denoising ; singular value thresholding ; functional MRI patch denoising singular value thresholding},
         PDF = {https://hal.science/hal-03895194/file/isbi2023_denoise.pdf},
         HAL_ID = {hal-03895194},
         HAL_VERSION = {v1},
       }
 
+
+Related Packages
+================
+
+- https://github.com/paquiteau/retino-pypeline
+
+  For the application of the denoising in an fMRI pypeline using Nipype
+
+- https://github.com/CEA-COSMIC/ModOpt
+
+  For the integration of the patch-denoising in convex optimisation algorithms.
```

### Comparing `patch-denoise-1.3.4/docs/Makefile` & `patch-denoise-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/docs/_templates/custom-class-template.rst` & `patch-denoise-1.4.0/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/docs/_templates/custom-module-template.rst` & `patch-denoise-1.4.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/docs/conf.py` & `patch-denoise-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/docs/denoisers.rst` & `patch-denoise-1.4.0/docs/denoisers.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/examples/conftest.py` & `patch-denoise-1.4.0/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/examples/example_experimental_data.py` & `patch-denoise-1.4.0/examples/example_experimental_data.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/examples/example_visualisation.py` & `patch-denoise-1.4.0/examples/example_visualisation.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/pyproject.toml` & `patch-denoise-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/__init__.py` & `patch-denoise-1.4.0/src/patch_denoise/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,8 +38,11 @@
     from ._version import version as __version__
 except ImportError:
     # -- Source mode --
     # use setuptools_scm to get the current version from src using git
     from setuptools_scm import get_version as _gv
     from os import path as _path
 
-    __version__ = _gv(_path.join(_path.dirname(__file__), _path.pardir))
+    try:
+        __version__ = _gv(_path.join(_path.dirname(__file__), _path.pardir))
+    except LookupError:
+        __version__ = "0.0.0+unknown"
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/_docs.py` & `patch-denoise-1.4.0/src/patch_denoise/_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     percentage of the path that has to be in the mask so that the patch is processed.
     if mask_threshold = -1, all the patch are processed, if mask_threshold=100, all
     the voxels of the patch needs to be in the mask""",
     denoise_return="""
 tuple
     numpy.ndarray: The denoised sequence of volume
     numpy.ndarray: The weight of each pixel after the processing.
-    numpy.ndarray: If possible, the noise variance distribution in the volume.""",
+    numpy.ndarray: If possible, the noise variance distribution in the volume
+    numpy.ndarray: If possible, the rank of each patch in the volume.""",
     input_config="""
 input_data: numpy.ndarray
     The input data to denoise. It should be a ND array, and the last
     dimension should a dynamically varying one (eg time).
 progbar: tqdm.tqdm Progress bar, optiononal
     An existing Progressbar, default (None) will create a new one.
     """,
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/bindings/cli.py` & `patch-denoise-1.4.0/src/patch_denoise/bindings/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,32 +124,36 @@
         affine_mask = None
     else:
         mask, affine_mask = load_as_array(args.mask)
     noise_map, affine_noise_map = load_as_array(args.noise_map)
 
     if affine is not None:
         if affine_mask is not None and np.allclose(affine, affine_mask):
-            warnings.warn("Affine matrix of input and mask does not match")
+            warnings.warn(
+                "Affine matrix of input and mask does not match", stacklevel=2
+            )
         if affine_noise_map is not None and np.allclose(affine, affine_noise_map):
-            warnings.warn("Affine matrix of input and noise map does not match")
+            warnings.warn(
+                "Affine matrix of input and noise map does not match", stacklevel=2
+            )
     d_par = DenoiseParameters.from_str(args.conf)
     print(d_par)
     denoise_func = DENOISER_MAP[d_par.method]
     extra_kwargs = dict()
 
     if d_par.method in [
         "nordic",
         "hybrid-pca",
         "adaptive-qut",
         "optimal-fro-noise",
     ]:
         extra_kwargs["noise_std"] = noise_map
         if noise_map is None:
             raise RuntimeError("A noise map must me specified for this method.")
-    denoised_data, _, noise_std_map = denoise_func(
+    denoised_data, patchs_weight, noise_std_map, rank_map = denoise_func(
         input_data,
         patch_shape=d_par.patch_shape,
         patch_overlap=d_par.patch_overlap,
         mask=mask,
         mask_threshold=d_par.mask_threshold,
         recombination=d_par.recombination,
         **extra_kwargs,
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/bindings/modopt.py` & `patch-denoise-1.4.0/src/patch_denoise/bindings/modopt.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     ):
         self._denoiser = DENOISER_MAP[denoiser]
         self._params = dict(
             patch_shape=patch_shape,
             patch_overlap=patch_overlap,
             mask=mask,
             mask_threshold=mask_threshold,
+            recombination=recombination,
             progbar=progbar,
             **kwargs,
         )
         self.op = self._op_method
         self.cost = lambda *args, **kw: np.NaN
         self.time_dimension = time_dimension
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/bindings/nipype.py` & `patch-denoise-1.4.0/src/patch_denoise/bindings/nipype.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 class PatchDenoiseOutputSpec(TraitedSpec):
     """OutputSpec for Denoising Interface."""
 
     denoised_file = File(desc="denoised file")
     noise_std_map = File(desc="a map of the noise variance.")
-    pass
+    rank_map = File(desc="a map of the rank of the patch.")
 
 
 class PatchDenoise(SimpleInterface):
     """Patch based denoising interface."""
 
     input_spec = PatchDenoiseInputSpec
     output_spec = PatchDenoiseOutputSpec
@@ -95,18 +95,18 @@
             for attr in PatchDenoise._denoise_attrs:
                 setattr(d_par, attr, getattr(self.inputs, attr))
 
         if isdefined(self.inputs.in_mag):
             data_mag_nii = nib.load(self.inputs.in_mag)
             data = data_mag_nii.get_fdata(dtype=np.float32)
             basename = self.inputs.in_mag
-            affine = data_mag_nii.affine
+            self._affine = data_mag_nii.affine
         else:
             data_real_nii = nib.load(self.inputs.in_real)
-            affine = data_real_nii.affine
+            self._affine = data_real_nii.affine
             data_real = data_real_nii.get_fdata(dtype=np.float32)
             data_imag = nib.load(self.inputs.in_imag).get_fdata(dtype=np.float32)
             data = 1j * data_imag
             data += data_real
             basename = self.inputs.in_real
 
         if isdefined(self.inputs.mask) and self.inputs.mask:
@@ -132,47 +132,49 @@
             "adaptive-qut",
             "optimal-fro-noise",
         ]:
             extra_kwargs["noise_std"] = nib.load(self.inputs.noise_std_map).get_fdata()
 
         if denoise_func is not None:
             # CORE CALL
-            denoised_data, _, noise_std_map = denoise_func(
+            denoised_data, _, noise_std_map, rank_map = denoise_func(
                 data,
                 patch_shape=d_par.patch_shape,
                 patch_overlap=d_par.patch_overlap,
                 mask=mask,
                 mask_threshold=d_par.mask_threshold,
                 recombination=d_par.recombination,
                 **extra_kwargs,
             )
         else:
             denoised_data = data
             noise_std_map = np.std(data, axis=-1, dtype=np.float32)
+            rank_map = np.zeros_like(noise_std_map)
         # OUTPUT
         if np.any(np.iscomplex(denoised_data)):
             denoised_data = np.abs(denoised_data, dtype=np.float32)
 
         _, base, _ = split_filename(basename)
         base = base.replace("_mag", "")
         base = base.replace("_real", "")
-        denoise_filename = f"{base}_d_{d_par.method}.nii"
-        noise_map_filename = f"{base}_noise_map.nii"
-
-        denoised_data_img = nib.Nifti1Image(denoised_data, affine=affine)
-        denoised_data_img.to_filename(denoise_filename)
-
-        noise_map_img = nib.Nifti1Image(noise_std_map, affine=affine)
-        noise_map_img.to_filename(noise_map_filename)
-
-        self._results["denoised_file"] = os.path.abspath(denoise_filename)
-        self._results["noise_std_map"] = os.path.abspath(noise_map_filename)
 
+        self._make_results_file("rank_map", f"{base}_rank_map.nii", rank_map)
+        self._make_results_file(
+            "denoised_file",
+            f"{base}_d_{d_par.method}.nii",
+            denoised_data,
+        )
+        self._make_results_file("noise_std_map", f"{base}_noise_map.nii", noise_std_map)
         return runtime
 
+    def _make_results_file(self, result_file, file_name, array):
+        """Add a new results file."""
+        self._results[result_file] = os.path.abspath(file_name)
+        nib.save(nib.Nifti1Image(array, self._affine), file_name)
+
 
 class NoiseStdMapInputSpec(BaseInterfaceInputSpec):
     """InputSpec for Noise Map Estimation."""
 
     noise_map_file = File(
         exists=True,
         mandatory=True,
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/bindings/utils.py` & `patch-denoise-1.4.0/src/patch_denoise/bindings/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,22 +52,45 @@
 
     method: str = None
     patch_shape: int = 11
     patch_overlap: int = 0
     recombination: str = "weighted"  # "center" is also available
     mask_threshold: int = 10
 
-    @classmethod
-    def from_str(self, config_str):
-        """Parse config string to create data structure.
+    @property
+    def pretty_name(self):
+        """Return a pretty name for the representation of parameters."""
+        if self.method:
+            name = self.method
+            for attr in [
+                "patch_shape",
+                "patch_overlap",
+                "recombination",
+                "mask_threshold",
+            ]:
+                if getattr(self, attr):
+                    name += f"_{getattr(self, attr)}"
+        else:
+            name = "noisy"
+        return name
 
-        The full format is ::
+    @property
+    def pretty_par(self):
+        """Get pretty representation of parameters."""
+        name = f"{self.patch_shape}_{self.patch_overlap}{self.recombination[0]}"
+        return name
 
-            <method>_<patch_shape>_<patch_overlap>_<recombination>_<mask_threshold>
-        """
+    @classmethod
+    def get_str(cls, **kwargs):
+        """Get full string representation from set of kwargs."""
+        return cls(**kwargs).pretty_name
+
+    @classmethod
+    def from_str(self, config_str):
+        """Create a DenoiseParameters from a string."""
         if "noisy" in config_str:
             return DenoiseParameters(
                 method=None,
                 patch_shape=None,
                 patch_overlap=None,
                 recombination=None,
                 mask_threshold=None,
@@ -79,29 +102,22 @@
                 d.method = conf.pop(0)
             if conf:
                 d.patch_shape = int(conf.pop(0))
             if conf:
                 d.patch_overlap = int(conf.pop(0))
             if conf:
                 c = conf.pop(0)
-                try:
-                    d.recombination = _RECOMBINATION[c]
-                except KeyError as exc:
-                    raise ValueError(f"unsupported  recombination key: {c}") from exc
+                d.recombination = c
             if conf:
                 d.mask_threshold = int(conf.pop(0))
             return d
 
     def __str__(self):
-        """Return string reprensation."""
-        ret_str = f"{self.method}_{self.patch_shape}_{self.patch_overlap}_"
-        ret_str += self.recombination[0]
-        if self.mask_threshold:
-            ret_str += f"_{self.mask_threshold}"
-        return ret_str
+        """Get string representation."""
+        return self.pretty_name
 
 
 def load_complex_nifti(mag_file, phase_file, filename=None):  # pragma: no cover
     """Load two nifti image (magnitude and phase) to create a complex valued array.
 
     Optionally, the result can be save as a .npy file
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/denoise.py` & `patch-denoise-1.4.0/src/patch_denoise/denoise.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/simulation/noise.py` & `patch-denoise-1.4.0/src/patch_denoise/simulation/noise.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/simulation/phantom.py` & `patch-denoise-1.4.0/src/patch_denoise/simulation/phantom.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/space_time/base.py` & `patch-denoise-1.4.0/src/patch_denoise/space_time/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base Structure for patch-based denoising on spatio-temporal dimension."""
 import abc
-
+import warnings
 import numpy as np
 from tqdm.auto import tqdm
 
 from .._docs import fill_doc
 
 from .utils import get_patch_locs
 
@@ -18,14 +18,20 @@
     ----------
     $patch_config
     """
 
     def __init__(self, patch_shape, patch_overlap, recombination="weighted"):
         self.p_shape = patch_shape
         self.p_ovl = patch_overlap
+
+        if recombination not in ["weighted", "average", "center"]:
+            raise ValueError(
+                "recombination must be one of 'weighted', 'average', 'center'"
+            )
+
         self.recombination = recombination
 
         self.input_denoising_kwargs = dict()
 
     @fill_doc
     def denoise(self, input_data, mask=None, mask_threshold=50, progbar=None):
         """Denoise the input_data, according to mask.
@@ -41,14 +47,15 @@
 
         Returns
         -------
         $denoise_return
         """
         data_shape = input_data.shape
         output_data = np.zeros_like(input_data)
+        rank_map = np.zeros(data_shape[:-1], dtype=np.int32)
         # Create Default mask
         if mask is None:
             process_mask = np.full(data_shape[:-1], True)
         else:
             process_mask = np.copy(mask)
 
         patch_shape, patch_overlap = self.__get_patch_param(data_shape)
@@ -90,45 +97,53 @@
             patch = np.reshape(input_data[patch_slice], (-1, input_data.shape[-1]))
 
             # Replace all nan by mean value of patch.
             # FIXME this behaviour should be documented
             # And ideally choosen by the user.
 
             patch[np.isnan(patch)] = np.mean(patch)
-            p_denoise, *extras = self._patch_processing(
+            p_denoise, maxidx, noise_var = self._patch_processing(
                 patch,
                 patch_slice=patch_slice,
                 **self.input_denoising_kwargs,
             )
 
             p_denoise = np.reshape(p_denoise, (*patch_shape, -1))
+            patch_center_img = tuple(
+                ptl + ps // 2 for ptl, ps in zip(patch_tl, patch_shape)
+            )
             if self.recombination == "center":
-                patch_center_img = tuple(
-                    ptl + ps // 2 for ptl, ps in zip(patch_tl, patch_shape)
-                )
                 output_data[patch_center_img] = p_denoise[patch_center]
-                patchs_weight[patch_center_img] += extras[0]
-                noise_std_estimate[patch_center_img] += extras[1]
-            else:
+                noise_std_estimate[patch_center_img] += noise_var
+            elif self.recombination == "weighted":
+                theta = 1 / (2 + maxidx)
+                output_data[patch_slice] += p_denoise * theta
+                patchs_weight[patch_slice] += theta
+            elif self.recombination == "average":
                 output_data[patch_slice] += p_denoise
-                if self.recombination == "weighted":
-                    patchs_weight[patch_slice] += extras[0]
-                elif self.recombination == "average":
-                    patchs_weight[patch_slice] += 1
-            if len(extras) > 1:
-                noise_std_estimate[patch_slice] += extras[1]
+                patchs_weight[patch_slice] += 1
+            else:
+                raise ValueError(
+                    "recombination must be one of 'weighted', 'average', 'center'"
+                )
+            if not np.isnan(noise_var):
+                noise_std_estimate[patch_slice] += noise_var
+            # the top left corner of the patch is used as id for the patch.
+            rank_map[patch_center_img] = maxidx
             if progbar:
                 progbar.update()
         # Averaging the overlapping pixels.
-        output_data /= patchs_weight[..., None]
-        noise_std_estimate /= patchs_weight
+        # this is only required for averaging recombinations.
+        if self.recombination in ["average", "weighted"]:
+            output_data /= patchs_weight[..., None]
+            noise_std_estimate /= patchs_weight
 
         output_data[~process_mask] = 0
 
-        return output_data, patchs_weight, noise_std_estimate
+        return output_data, patchs_weight, noise_std_estimate, rank_map
 
     @abc.abstractmethod
     def _patch_processing(self, patch, patch_slice=None, **kwargs):
         """Process a patch.
 
         Implemented by child classes.
         """
@@ -144,13 +159,14 @@
             p = getattr(self, attr)
             if isinstance(p, list):
                 p = tuple(p)
             elif isinstance(p, (int, np.integer)):
                 p = (p,) * (len(data_shape) - 1)
             pp[i] = p
         if np.prod(pp[0]) < data_shape[-1]:
-            raise ValueError(
+            warnings.warn(
                 f"the number of voxel in patch ({np.prod(pp[0])}) is smaller than the"
                 f" last dimension ({data_shape[-1]}), this makes an ill-conditioned"
-                "matrix for SVD."
+                "matrix for SVD.",
+                stacklevel=2,
             )
         return tuple(pp)
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/space_time/lowrank.py` & `patch-denoise-1.4.0/src/patch_denoise/space_time/lowrank.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Low Rank Denoising methods."""
+"""Low Rank  methods."""
 from types import MappingProxyType
 
 import numpy as np
 from scipy.linalg import svd
 from scipy.optimize import minimize
 
 from .base import BaseSpaceTimeDenoiser
@@ -54,19 +54,16 @@
 
         if maxidx == 0:
             patch_new = np.zeros_like(patch) + p_tmean
         else:
             patch_new = eig_synthesis(p_center, eig_vec, p_tmean, maxidx)
 
         # Equation (3) of Manjon 2013
-        weights = 1.0 / (1.0 + maxidx)
-        noise_map = var_noise * weights
-        patch_new *= weights
 
-        return patch_new, noise_map, weights
+        return patch_new, maxidx, var_noise
 
 
 @fill_doc
 class HybridPCADenoiser(BaseSpaceTimeDenoiser):
     """Denoising using the Hybrid-PCA thresholding method.
 
     Parameters
@@ -111,19 +108,16 @@
             maxidx += 1
             var_noise = np.mean(eig_vals[:-maxidx])
         if maxidx == 0:  # all eigen values are noise
             patch_new = np.zeros_like(patch) + p_tmean
         else:
             patch_new = eig_synthesis(p_center, eig_vec, p_tmean, maxidx)
         # Equation (3) of Manjon2013
-        weights = 1.0 / (1.0 + maxidx)
-        noise_map = var_noise * weights
-        patch_new *= weights
 
-        return patch_new, noise_map, weights
+        return patch_new, maxidx, var_noise
 
 
 @fill_doc
 class RawSVDDenoiser(BaseSpaceTimeDenoiser):
     """
     Classical Patch wise singular value thresholding denoiser.
 
@@ -179,19 +173,16 @@
         if maxidx == 0:
             p_new = np.zeros_like(patch) + p_tmean
         else:
             s_values[s_values < self._threshold] = 0
             p_new = svd_synthesis(u_vec, s_values, v_vec, p_tmean, maxidx)
 
         # Equation (3) in Manjon 2013
-        theta = 1.0 / (1.0 + maxidx)
-        p_new *= theta
-        weights = theta
 
-        return p_new, weights, np.NaN
+        return p_new, maxidx, np.NaN
 
 
 @fill_doc
 class NordicDenoiser(RawSVDDenoiser):
     """Denoising using the NORDIC method.
 
     Parameters
@@ -399,20 +390,15 @@
         if np.any(thresh_s_values):
             maxidx = np.max(np.nonzero(thresh_s_values)) + 1
             p_new = svd_synthesis(u_vec, thresh_s_values, v_vec, p_tmean, maxidx)
         else:
             maxidx = 0
             p_new = np.zeros_like(patch) + p_tmean
 
-        # Equation (3) in Manjon 2013
-        theta = 1.0 / (1.0 + maxidx)
-        p_new *= theta
-        weights = theta
-
-        return p_new, weights, np.NaN
+        return p_new, maxidx, np.NaN
 
 
 def _sure_atn_cost(X, method, sing_vals, gamma, sigma=None, tau=None):
     """
     Compute the SURE cost function.
 
     Parameters
@@ -629,13 +615,8 @@
         if np.any(thresh_s_values):
             maxidx = np.max(np.nonzero(thresh_s_values)) + 1
             p_new = svd_synthesis(u_vec, thresh_s_values, v_vec, p_tmean, maxidx)
         else:
             maxidx = 0
             p_new = np.zeros_like(patch) + p_tmean
 
-        # Equation (3) in Manjon 2013
-        theta = 1.0 / (1.0 + maxidx)
-        p_new *= theta
-        weights = theta
-
-        return p_new, weights, np.NaN
+        return p_new, maxidx, np.NaN
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise/space_time/utils.py` & `patch-denoise-1.4.0/src/patch_denoise/space_time/utils.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/viz/plots.py` & `patch-denoise-1.4.0/src/patch_denoise/viz/plots.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise/viz/utils.py` & `patch-denoise-1.4.0/src/patch_denoise/viz/utils.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/src/patch_denoise.egg-info/PKG-INFO` & `patch-denoise-1.4.0/src/patch_denoise.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-denoise
-Version: 1.3.4
+Version: 1.4.0
 Summary: Denoising method for sequence of images or volumes. Primarly targeting fMRI data.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -138,7 +138,18 @@
         MONTH = Apr,
         KEYWORDS = {functional MRI ; patch denoising ; singular value thresholding ; functional MRI patch denoising singular value thresholding},
         PDF = {https://hal.science/hal-03895194/file/isbi2023_denoise.pdf},
         HAL_ID = {hal-03895194},
         HAL_VERSION = {v1},
       }
 
+
+Related Packages
+================
+
+- https://github.com/paquiteau/retino-pypeline
+
+  For the application of the denoising in an fMRI pypeline using Nipype
+
+- https://github.com/CEA-COSMIC/ModOpt
+
+  For the integration of the patch-denoising in convex optimisation algorithms.
```

### Comparing `patch-denoise-1.3.4/src/patch_denoise.egg-info/SOURCES.txt` & `patch-denoise-1.4.0/src/patch_denoise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/tests/conftest.py` & `patch-denoise-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.3.4/tests/test_bindings.py` & `patch-denoise-1.4.0/tests/test_bindings.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,22 +21,21 @@
 from patch_denoise.bindings.nipype import PatchDenoise
 from patch_denoise.bindings.utils import DenoiseParameters
 from patch_denoise.denoise import mp_pca
 
 
 @pytest.fixture(scope="module")
 def denoised_ref(noisy_phantom):
-    denoised_func, _, _ = mp_pca(
+    return mp_pca(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         threshold_scale=2.3,
         recombination="weighted",
-    )
-    return denoised_func
+    )[0]
 
 
 @pytest.fixture
 def nifti_noisy_phantom(noisy_phantom, tmpdir_factory):
     tempdir = tmpdir_factory.mktemp("test")
     tempdir.chdir()
     nii_img = nib.Nifti1Image(noisy_phantom, affine=np.eye(4))
@@ -67,15 +66,15 @@
 
 def test_cli(nifti_noisy_phantom, tmpdir_factory, denoised_ref):
     tempdir = tmpdir_factory.mktemp("test")
     tempdir.chdir()
     outfile = "out.nii"
     print(nifti_noisy_phantom, tempdir)
     exit_status = os.system(
-        f"patch-denoise {nifti_noisy_phantom} {outfile} --conf mp-pca_6_5_w --extra threshold_scale=2.3"
+        f"patch-denoise {nifti_noisy_phantom} {outfile} --conf mp-pca_6_5_weighted --extra threshold_scale=2.3"
     )
     assert exit_status == 0
     npt.assert_allclose(nib.load(outfile).get_fdata(), denoised_ref)
 
 
 def test_denoise_param():
     """Test the Denoise parameter structure."""
@@ -85,26 +84,42 @@
 
 
 def test_nipype_mag(nifti_noisy_phantom, denoised_ref):
     """Test the Nipye Interfaces."""
 
     interface = PatchDenoise()
     interface.inputs.in_mag = nifti_noisy_phantom
-    interface.inputs.denoise_str = "mp-pca_6_5_w"
+    interface.inputs.denoise_str = "mp-pca_6_5_weighted"
     interface.inputs.extra_kwargs = {"threshold_scale": 2.3}
 
     output_file = interface.run().outputs.denoised_file
 
     output_data = nib.load(output_file).get_fdata()
     npt.assert_allclose(output_data, denoised_ref, rtol=1e-2)
 
 
 def test_nipype_cpx(nifti_noisy_phantom):
     """Test the Nipye Interfaces."""
 
     interface = PatchDenoise()
     interface.inputs.in_real = nifti_noisy_phantom
     interface.inputs.in_imag = nifti_noisy_phantom
-    interface.inputs.denoise_str = "mp-pca_6_5_w"
+    interface.inputs.denoise_str = "mp-pca_6_5_weighted"
     interface.inputs.extra_kwargs = {"threshold_scale": 2.3}
 
     output_file = interface.run().outputs.denoised_file
+
+
+def test_denoise_paramter_pretty_par():
+
+    pretty_par = DenoiseParameters("optimal-fro", 11, 10, "weighted", 10).pretty_par
+
+    assert pretty_par == "11_10w"
+
+
+def test_denoise_parameter_pretty():
+    """Test the pretty_name."""
+
+    pretty_string = "optimal-fro_11_10_weighted_10"
+    pretty_name = DenoiseParameters.from_str(pretty_string).pretty_name
+
+    assert pretty_name == pretty_string
```

### Comparing `patch-denoise-1.3.4/tests/test_denoiser.py` & `patch-denoise-1.4.0/tests/test_denoiser.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 
 from patch_denoise.simulation.phantom import g_factor_map
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 def test_mppca_denoiser(phantom, noisy_phantom, recombination):
     """Test the MP-PCA denoiser."""
-    denoised, weights, noise = mp_pca(
+    denoised, weights, noise, rank_map = mp_pca(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         threshold_scale=2.3,
         recombination=recombination,
     )
     noise_std_before = np.sqrt(np.nanmean(np.nanvar(noisy_phantom - phantom, axis=-1)))
     noise_std_after = np.sqrt(np.nanmean(np.nanvar(denoised - phantom, axis=-1)))
     assert noise_std_after < noise_std_before
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 def test_hybridpca_denoiser(phantom, noisy_phantom, recombination):
     """Test the Hybrid-PCA denoiser."""
-    denoised, weights, noise = hybrid_pca(
+    denoised, weights, noise, rank_map = hybrid_pca(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         noise_std=1.0,
         recombination=recombination,
     )
 
@@ -45,15 +45,15 @@
     noise_std_after = np.sqrt(np.nanmean(np.nanvar(denoised - phantom, axis=-1)))
     assert noise_std_after < noise_std_before
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 def test_nordic_denoiser(phantom, noisy_phantom, recombination):
     """Test the Hybrid-PCA denoiser."""
-    denoised, weights, noise = nordic(
+    denoised, weights, noise, rank_map = nordic(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         noise_std=1.0,
         recombination=recombination,
     )
 
@@ -61,15 +61,15 @@
     noise_std_after = np.sqrt(np.nanmean(np.nanvar(denoised - phantom, axis=-1)))
     assert noise_std_after < noise_std_before
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 def test_rawsvt_denoiser(phantom, noisy_phantom, recombination):
     """Test the Hybrid-PCA denoiser."""
-    denoised, weights, noise = raw_svt(
+    denoised, weights, noise, rank_map = raw_svt(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         threshold=10,
         recombination=recombination,
     )
 
@@ -78,15 +78,15 @@
     assert noise_std_after < noise_std_before
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 @pytest.mark.parametrize("loss", ["fro", "nuc", "ope"])
 def test_optimal_denoiser(phantom, noisy_phantom, recombination, loss):
     """Test the Optimal Thresholding denoiser."""
-    denoised, weights, noise = optimal_thresholding(
+    denoised, weights, noise, rank_map = optimal_thresholding(
         noisy_phantom,
         patch_shape=6,
         patch_overlap=5,
         recombination=recombination,
         loss=loss,
     )
 
@@ -95,15 +95,15 @@
     assert noise_std_after < noise_std_before
 
 
 @pytest.mark.parametrize("recombination", ["weighted", "average", "center"])
 @pytest.mark.parametrize("loss", ["fro", "nuc", "ope"])
 def test_optimal_denoiser2(phantom, noisy_phantom, recombination, loss):
     """Test the Optimal Thresholding denoiser with noise apriori provided."""
-    denoised, weights, noise = optimal_thresholding(
+    denoised, weights, noise, rank_map = optimal_thresholding(
         noisy_phantom,
         patch_shape=10,
         patch_overlap=9,
         noise_std=1.414 * g_factor_map(phantom.shape[:-1]),
         recombination=recombination,
         loss=loss,
     )
@@ -116,15 +116,15 @@
 @pytest.mark.parametrize("recombination", ["weighted", "average"])
 @pytest.mark.parametrize(
     "method, gamma",
     [("qut", None), ("gsure", np.linspace(1, 5, 10)), ("sure", np.linspace(1, 5, 10))],
 )
 def test_adaptive_denoiser(phantom, noisy_phantom, recombination, method, gamma):
     """Test the Adaptive Thresholding denoiser."""
-    denoised, weights, noise = adaptive_thresholding(
+    denoised, weights, noise, rank_map = adaptive_thresholding(
         noisy_phantom,
         patch_shape=10,
         patch_overlap=0,
         recombination=recombination,
         method=method,
         noise_std=2 * g_factor_map(phantom.shape[:-1]),
         gamma0=gamma,
```

### Comparing `patch-denoise-1.3.4/tests/test_spacetime_utils.py` & `patch-denoise-1.4.0/tests/test_spacetime_utils.py`

 * *Files identical despite different names*

