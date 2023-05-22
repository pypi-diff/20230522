# Comparing `tmp/tranquilo-0.0.3.tar.gz` & `tmp/tranquilo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tranquilo-0.0.3.tar", last modified: Sat May 20 10:06:50 2023, max compression
+gzip compressed data, was "tranquilo-0.0.4.tar", last modified: Mon May 22 08:33:36 2023, max compression
```

## Comparing `tranquilo-0.0.3.tar` & `tranquilo-0.0.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.515989 tranquilo-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.507990 tranquilo-0.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.507990 tranquilo-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-20 10:06:37.000000 tranquilo-0.0.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-20 10:06:37.000000 tranquilo-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-20 10:06:37.000000 tranquilo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 10:06:37.000000 tranquilo-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 10:06:50.515989 tranquilo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-20 10:06:37.000000 tranquilo-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-20 10:06:37.000000 tranquilo-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-20 10:06:50.515989 tranquilo-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-20 10:06:37.000000 tranquilo-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/acceptance_decision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/acceptance_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/adjust_n_evals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/adjust_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/aggregate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/estimate_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/exploration_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/filter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/get_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/handle_infinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/poisedness.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/process_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/rho_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/solve_subproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo/subsolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/bntr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/bntr_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/linear_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/wrapped_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/tranquilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/wrap_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.048448 tranquilo-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.040448 tranquilo-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.044448 tranquilo-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.044448 tranquilo-0.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.044448 tranquilo-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-22 08:33:26.000000 tranquilo-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-22 08:33:26.000000 tranquilo-0.0.4/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-22 08:33:26.000000 tranquilo-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-22 08:33:26.000000 tranquilo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-22 08:33:26.000000 tranquilo-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-22 08:33:36.048448 tranquilo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 08:33:26.000000 tranquilo-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 08:33:26.000000 tranquilo-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-22 08:33:36.048448 tranquilo-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 08:33:26.000000 tranquilo-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.040448 tranquilo-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.048448 tranquilo-0.0.4/src/tranquilo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 08:33:35.000000 tranquilo-0.0.4/src/tranquilo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/acceptance_decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/acceptance_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/adjust_n_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/adjust_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/aggregate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/estimate_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/exploration_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/filter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/fit_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/get_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/handle_infinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/poisedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/process_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/rho_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/sample_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/solve_subproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.048448 tranquilo-0.0.4/src/tranquilo/subsolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_steihaug_toint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_steihaug_toint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_trsbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/_trsbox_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/bntr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/bntr_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/gqtpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/gqtpar_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/linear_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/subsolvers/wrapped_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/tranquilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-22 08:33:26.000000 tranquilo-0.0.4/src/tranquilo/wrap_criterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:33:36.048448 tranquilo-0.0.4/src/tranquilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-22 08:33:36.000000 tranquilo-0.0.4/src/tranquilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 08:33:36.000000 tranquilo-0.0.4/src/tranquilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:33:36.000000 tranquilo-0.0.4/src/tranquilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:33:35.000000 tranquilo-0.0.4/src/tranquilo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 08:33:36.000000 tranquilo-0.0.4/src/tranquilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 08:33:36.000000 tranquilo-0.0.4/src/tranquilo.egg-info/top_level.txt
```

### Comparing `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md` & `tranquilo-0.0.4/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md` & `tranquilo-0.0.4/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `tranquilo-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/.github/workflows/main.yml` & `tranquilo-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/.github/workflows/publish-to-pypi.yml` & `tranquilo-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/.gitignore` & `tranquilo-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/CODE_OF_CONDUCT.md` & `tranquilo-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/LICENSE` & `tranquilo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/MANIFEST.in` & `tranquilo-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/PKG-INFO` & `tranquilo-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tranquilo-0.0.3/README.md` & `tranquilo-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/pyproject.toml` & `tranquilo-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 [tool.nbqa.mutate]
 black = 1
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:delta_grad == 0.0",  # UserWarning in test_poisedness.py
     "ignore:Jupyter is migrating",  # DeprecationWarning from jupyter client
+    "ignore:Noisy scalar functions are experimental",
 ]
 markers = [
     "wip: Tests that are work-in-progress.",
     "slow: Tests that take a long time to run and are skipped in continuous integration.",
 ]
 norecursedirs = ["docs", ".envs"]
```

### Comparing `tranquilo-0.0.3/setup.cfg` & `tranquilo-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/acceptance_decision.py` & `tranquilo-0.0.4/src/tranquilo/acceptance_decision.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/acceptance_sample_size.py` & `tranquilo-0.0.4/src/tranquilo/acceptance_sample_size.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/adjust_n_evals.py` & `tranquilo-0.0.4/src/tranquilo/adjust_n_evals.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/adjust_radius.py` & `tranquilo-0.0.4/src/tranquilo/adjust_radius.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/aggregate_models.py` & `tranquilo-0.0.4/src/tranquilo/aggregate_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/bounds.py` & `tranquilo-0.0.4/src/tranquilo/bounds.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/clustering.py` & `tranquilo-0.0.4/src/tranquilo/clustering.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/config.py` & `tranquilo-0.0.4/src/tranquilo/config.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/estimate_variance.py` & `tranquilo-0.0.4/src/tranquilo/estimate_variance.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/exploration_sample.py` & `tranquilo-0.0.4/src/tranquilo/exploration_sample.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/filter_points.py` & `tranquilo-0.0.4/src/tranquilo/filter_points.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/fit_models.py` & `tranquilo-0.0.4/src/tranquilo/fit_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/geometry.py` & `tranquilo-0.0.4/src/tranquilo/geometry.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/get_component.py` & `tranquilo-0.0.4/src/tranquilo/get_component.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/handle_infinity.py` & `tranquilo-0.0.4/src/tranquilo/handle_infinity.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/history.py` & `tranquilo-0.0.4/src/tranquilo/history.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/models.py` & `tranquilo-0.0.4/src/tranquilo/models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/options.py` & `tranquilo-0.0.4/src/tranquilo/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     strictness: float = 1e-10
     shape: str = "sphere"
 
 
 class SamplerOptions(NamedTuple):
     distribution: str = None
     hardness: float = 1
-    algorithm: str = "scipy_lbfgsb"
+    algorithm: str = "L-BFGS-B"
     algo_options: dict = None
     criterion: str = None
     n_points_randomsearch: int = 1
     return_info: bool = False
 
 
 class NoiseAdaptationOptions(NamedTuple):
```

### Comparing `tranquilo-0.0.3/src/tranquilo/poisedness.py` & `tranquilo-0.0.4/src/tranquilo/poisedness.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/process_arguments.py` & `tranquilo-0.0.4/src/tranquilo/process_arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import numpy as np
 
-from estimagic.optimization.algo_options import (
-    CONVERGENCE_RELATIVE_CRITERION_TOLERANCE,
-    CONVERGENCE_RELATIVE_GRADIENT_TOLERANCE,
-)
 from tranquilo.acceptance_decision import get_acceptance_decider
 from tranquilo.aggregate_models import get_aggregator
 from tranquilo.bounds import Bounds
 from tranquilo.estimate_variance import get_variance_estimator
 from tranquilo.filter_points import get_sample_filter
 from tranquilo.fit_models import get_fitter
 from tranquilo.history import History
@@ -29,14 +25,15 @@
     update_option_bundle,
     NoiseAdaptationOptions,
 )
 from tranquilo.region import Region
 from tranquilo.sample_points import get_sampler
 from tranquilo.solve_subproblem import get_subsolver
 from tranquilo.wrap_criterion import get_wrapped_criterion
+import warnings
 
 
 def process_arguments(
     # functype, will be partialled out
     functype,
     # problem description
     criterion,
@@ -47,16 +44,16 @@
     # basic options
     noisy=False,
     # convergence options
     disable_convergence=False,
     convergence_absolute_criterion_tolerance=0.0,
     convergence_absolute_gradient_tolerance=0.0,
     convergence_absolute_params_tolerance=0.0,
-    convergence_relative_criterion_tolerance=CONVERGENCE_RELATIVE_CRITERION_TOLERANCE,
-    convergence_relative_gradient_tolerance=CONVERGENCE_RELATIVE_GRADIENT_TOLERANCE,
+    convergence_relative_criterion_tolerance=2e-9,
+    convergence_relative_gradient_tolerance=1e-8,
     convergence_relative_params_tolerance=1e-8,
     convergence_min_trust_region_radius=0.0,
     # stopping options
     stopping_max_criterion_evaluations=2_000,
     stopping_max_iterations=200,
     stopping_max_time=np.inf,
     # single advanced options
@@ -86,14 +83,34 @@
     acceptance_decider=None,
     acceptance_decider_options=None,
     variance_estimator="classic",
     variance_estimator_options=None,
     infinity_handler="relative",
     residualize=None,
 ):
+    # warning for things that do not work well yet
+    if noisy and functype == "scalar":
+        msg = (
+            "Noisy scalar functions are experimental and likely to give very "
+            "suboptimal results."
+        )
+        warnings.warn(msg)
+    if noisy and n_cores > 1:
+        msg = (
+            "Parallelization together with noisy functions is experimental and likely "
+            "to give very suboptimal results."
+        )
+        warnings.warn(msg)
+    if n_cores > 1 and functype == "scalar":
+        msg = (
+            "Parallelization together with scalar functions is experimental and likely "
+            "to give very suboptimal results."
+        )
+        warnings.warn(msg)
+
     # process convergence options
     conv_options = ConvOptions(
         disable=bool(disable_convergence),
         ftol_abs=float(convergence_absolute_criterion_tolerance),
         gtol_abs=float(convergence_absolute_gradient_tolerance),
         xtol_abs=float(convergence_absolute_params_tolerance),
         ftol_rel=float(convergence_relative_criterion_tolerance),
```

### Comparing `tranquilo-0.0.3/src/tranquilo/region.py` & `tranquilo-0.0.4/src/tranquilo/region.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/rho_noise.py` & `tranquilo-0.0.4/src/tranquilo/rho_noise.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/sample_points.py` & `tranquilo-0.0.4/src/tranquilo/sample_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from functools import partial
 
 import numpy as np
 from scipy.spatial.distance import pdist
 from scipy.special import gammainc, logsumexp
 
-import estimagic as em
+from scipy.optimize import minimize, Bounds
 from tranquilo.get_component import get_component
 from tranquilo.options import SamplerOptions
+import functools
 
 
 def get_sampler(sampler, user_options=None):
     """Get sampling function partialled options.
 
     Args:
         sampler (str or callable): Name of a sampling method or sampling function.
@@ -237,16 +238,16 @@
     if n_points <= 0:
         return np.array([])
 
     if criterion is None:
         criterion = "determinant" if n_points == 1 else "distance"
 
     algo_options = {} if algo_options is None else algo_options
-    if "stopping_max_iterations" not in algo_options:
-        algo_options["stopping_max_iterations"] = 2 * n_params + 5
+    if "maxiter" not in algo_options:
+        algo_options["maxiter"] = 2 * n_params + 5
 
     if existing_xs is not None:
         # map existing points into unit space for easier optimization
 
         existing_xs_unit = trustregion.map_to_unit(existing_xs)
 
         if criterion == "distance":
@@ -298,23 +299,22 @@
     x0 = x0.flatten()  # flatten so that em.maximize uses fast path
 
     # This would raise an error because there are zero pairs to calculate the
     # pairwise distance
     if existing_xs_unit is None and n_points == 1:
         opt_params = x0
     else:
-        res = em.maximize(
-            criterion=func_dict[criterion],
-            params=x0,
-            algorithm=algorithm,
-            lower_bounds=-np.ones_like(x0),
-            upper_bounds=np.ones_like(x0),
-            algo_options=algo_options,
+        res = minimize(
+            switch_sign(func_dict[criterion]),
+            x0,
+            method=algorithm,
+            bounds=Bounds(-np.ones_like(x0), np.ones_like(x0)),
+            options=algo_options,
         )
-        opt_params = res.params
+        opt_params = res.x
 
     # Make sure the optimal sampling is actually better than the initial one with
     # respect to the fekete criterion. This could be violated if the surrogate
     # criterion is not a good approximation or if the optimization fails.
     start_fekete = func_dict["determinant"](x0)
     end_fekete = func_dict["determinant"](opt_params)
 
@@ -460,7 +460,15 @@
         np.ndarray: The projected points.
 
     """
     order = 2 if trustregion_shape == "sphere" else np.inf
     norm = np.linalg.norm(x, axis=1, ord=order).reshape(-1, 1)
     projected = x / norm
     return projected
+
+
+def switch_sign(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return -func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `tranquilo-0.0.3/src/tranquilo/solve_subproblem.py` & `tranquilo-0.0.4/src/tranquilo/solve_subproblem.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient_fast.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_conjugate_gradient_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_steihaug_toint.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint_fast.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_steihaug_toint_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_trsbox.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox_fast.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/_trsbox_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/bntr.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/bntr.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/bntr_fast.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/bntr_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/gqtpar.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar_fast.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/gqtpar_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/linear_subsolvers.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/linear_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/subsolvers/wrapped_subsolvers.py` & `tranquilo-0.0.4/src/tranquilo/subsolvers/wrapped_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/tranquilo.py` & `tranquilo-0.0.4/src/tranquilo/tranquilo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import functools
-from functools import partial
 from typing import NamedTuple
 
 import numpy as np
 
-from estimagic.decorators import mark_minimizer
 from tranquilo.adjust_radius import adjust_radius
 from tranquilo.filter_points import (
     drop_worst_points,
 )
 from tranquilo.models import (
     ScalarModel,
     VectorModel,
@@ -509,33 +507,14 @@
     else:
         converged = False
         msg = None
 
     return converged, msg
 
 
-tranquilo = mark_minimizer(
-    func=partial(_tranquilo, functype="scalar"),
-    name="tranquilo",
-    primary_criterion_entry="value",
-    needs_scaling=True,
-    is_available=True,
-    is_global=False,
-)
-
-tranquilo_ls = mark_minimizer(
-    func=partial(_tranquilo, functype="least_squares"),
-    primary_criterion_entry="root_contributions",
-    name="tranquilo_ls",
-    needs_scaling=True,
-    is_available=True,
-    is_global=False,
-)
-
-
 def _concatenate_indices(first, second):
     first = np.atleast_1d(first).astype(int)
     second = np.atleast_1d(second).astype(int)
     return np.hstack((first, second))
 
 
 def _get_additional_eval_info(model_indices, history, n_evals_per_point):
```

### Comparing `tranquilo-0.0.3/src/tranquilo/utilities.py` & `tranquilo-0.0.4/src/tranquilo/utilities.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/visualize.py` & `tranquilo-0.0.4/src/tranquilo/visualize.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/volume.py` & `tranquilo-0.0.4/src/tranquilo/volume.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/weighting.py` & `tranquilo-0.0.4/src/tranquilo/weighting.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.3/src/tranquilo/wrap_criterion.py` & `tranquilo-0.0.4/src/tranquilo/wrap_criterion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import functools
 
 import numpy as np
 
-from estimagic.batch_evaluators import process_batch_evaluator
-
 
 def get_wrapped_criterion(criterion, batch_evaluator, n_cores, history):
     """Wrap the criterion function to do get parallelization and history handling.
 
     Notes
     -----
 
@@ -62,7 +60,28 @@
 
         history.add_evals(
             x_indices=np.repeat(x_indices, repetitions),
             evals=clipped_evals,
         )
 
     return wrapper_criterion
+
+
+def process_batch_evaluator(batch_evaluator="joblib"):
+    batch_evaluator = "joblib" if batch_evaluator is None else batch_evaluator
+
+    if callable(batch_evaluator):
+        out = batch_evaluator
+    elif isinstance(batch_evaluator, str):
+        if batch_evaluator == "joblib":
+            from estimagic.batch_evaluators import joblib_batch_evaluator as out
+        elif batch_evaluator == "pathos":
+            from estimagic.batch_evaluators import pathos_mp_batch_evaluator as out
+        else:
+            raise ValueError(
+                "Invalid batch evaluator requested. Currently only 'pathos' and "
+                "'joblib' are supported."
+            )
+    else:
+        raise TypeError("batch_evaluator must be a callable or string.")
+
+    return out
```

### Comparing `tranquilo-0.0.3/src/tranquilo.egg-info/PKG-INFO` & `tranquilo-0.0.4/src/tranquilo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tranquilo-0.0.3/src/tranquilo.egg-info/SOURCES.txt` & `tranquilo-0.0.4/src/tranquilo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

