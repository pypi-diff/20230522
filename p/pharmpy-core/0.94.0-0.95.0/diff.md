# Comparing `tmp/pharmpy-core-0.94.0.tar.gz` & `tmp/pharmpy-core-0.95.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.94.0.tar", last modified: Wed Apr 26 11:35:39 2023, max compression
+gzip compressed data, was "pharmpy-core-0.95.0.tar", last modified: Mon May 22 08:31:02 2023, max compression
```

## Comparing `pharmpy-core-0.94.0.tar` & `pharmpy-core-0.95.0.tar`

### file list

```diff
@@ -1,1182 +1,1185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44894 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.324879 pharmpy-core-0.94.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.328879 pharmpy-core-0.94.0/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80309 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.332879 pharmpy-core-0.94.0/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.284879 pharmpy-core-0.94.0/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.336879 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.340879 pharmpy-core-0.94.0/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.344879 pharmpy-core-0.94.0/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.344879 pharmpy-core-0.94.0/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    68113 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.356879 pharmpy-core-0.94.0/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    33875 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    45291 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    71026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iov.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/update_inits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.364879 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.368879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    64128 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.372879 pharmpy-core-0.94.0/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.376879 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38407 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.380879 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.384879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.388879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.388879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.392879 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/simfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.396879 pharmpy-core-0.94.0/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.400879 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46809 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46649 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:29:03.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 11:35:39.000000 pharmpy-core-0.94.0/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.404879 pharmpy-core-0.94.0/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/integration/test_ruvsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.408879 pharmpy-core-0.94.0/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.412879 pharmpy-core-0.94.0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27417 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.416879 pharmpy-core-0.94.0/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_add_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_has_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)   100500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_remove_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.420879 pharmpy-core-0.94.0/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.420879 pharmpy-core-0.94.0/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35906 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/plugins/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/plugins/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.424879 pharmpy-core-0.94.0/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.436879 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.448880 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.452880 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.456879 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.456879 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.460880 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.460880 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.464880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.468880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.468880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.296879 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.484880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.484880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.488880 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.488880 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.496880 pharmpy-core-0.94.0/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.504880 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.504880 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.508880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.512880 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.512880 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.516880 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.524880 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.524880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.528880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.532880 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.532880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.536880 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.548880 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   263999 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.552880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.304879 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:30:47.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.556880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.560880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.560880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.564880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.568880 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.572880 pharmpy-core-0.94.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    27814 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_modelfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:35:39.576880 pharmpy-core-0.94.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-26 11:27:38.000000 pharmpy-core-0.94.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45578 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47493 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80455 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.320743 pharmpy-core-0.95.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.360744 pharmpy-core-0.95.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.360744 pharmpy-core-0.95.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72906 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.364744 pharmpy-core-0.95.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34265 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    45326 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70916 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/update_inits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28145 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.376744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22581 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64435 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.404744 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.404744 pharmpy-core-0.95.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47493 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46762 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:24:01.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_ruvsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.420745 pharmpy-core-0.95.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.424745 pharmpy-core-0.95.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_add_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_has_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_remove_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_rxode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.432745 pharmpy-core-0.95.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.432745 pharmpy-core-0.95.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.436745 pharmpy-core-0.95.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.440745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.440745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.452745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/failed_run.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.464745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.464745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.472746 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.472746 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.476745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.476745 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.488746 pharmpy-core-0.95.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_conc.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.492746 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.504746 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.512746 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.516746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.516746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.524746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.540746 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:00.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.560747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.560747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_modelfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tox.ini
```

### Comparing `pharmpy-core-0.94.0/AUTHORS.rst` & `pharmpy-core-0.95.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/CHANGELOG.rst` & `pharmpy-core-0.95.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+0.95.0 (2023-05-22)
+-------------------
+
+Changes
+=======
+
+* ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
+
+Bugfixes
+========
+
+* Fix bug causing changes in FIX from model1 to model4 to crash frem
+* Fix bug causing individual parameters in $ERROR to crash frem
+* create_report now does not assume that results.json already exists
+* ~ for $HOME is now supported in write_model and create_report
+* Fix bug where LLOQ value did not override column in dataset in ``transform_blq``
+* Correct BLQ indicator column condition in ``transform_blq``
+* Fix bug where modelfit results were not connected to model after a fit
+
 0.94.0 (2023-04-26)
 -------------------
 
 New features
 ============
 
 * Support parsing assignments other than DADT in $DES in NONMEM
```

### Comparing `pharmpy-core-0.94.0/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.95.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/LICENSE` & `pharmpy-core-0.95.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/LICENSE.LESSER` & `pharmpy-core-0.95.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/MANIFEST.in` & `pharmpy-core-0.95.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/PKG-INFO` & `pharmpy-core-0.95.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.94.0
+Version: 0.95.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.95.0 (2023-05-22)
+-------------------
+
+Changes
+=======
+
+* ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
+
+Bugfixes
+========
+
+* Fix bug causing changes in FIX from model1 to model4 to crash frem
+* Fix bug causing individual parameters in $ERROR to crash frem
+* create_report now does not assume that results.json already exists
+* ~ for $HOME is now supported in write_model and create_report
+* Fix bug where LLOQ value did not override column in dataset in ``transform_blq``
+* Correct BLQ indicator column condition in ``transform_blq``
+* Fix bug where modelfit results were not connected to model after a fit
+
 0.94.0 (2023-04-26)
 -------------------
 
 New features
 ============
 
 * Support parsing assignments other than DADT in $DES in NONMEM
```

### Comparing `pharmpy-core-0.94.0/README.rst` & `pharmpy-core-0.95.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/NONMEM.rst` & `pharmpy-core-0.95.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/Pharmpy_logo.svg` & `pharmpy-core-0.95.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.95.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/_ext/conversion.py` & `pharmpy-core-0.95.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.95.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/allometry.rst` & `pharmpy-core-0.95.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/amd.rst` & `pharmpy-core-0.95.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/api.rst` & `pharmpy-core-0.95.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/bootstrap.rst` & `pharmpy-core-0.95.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/cdd.rst` & `pharmpy-core-0.95.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/cli.rst` & `pharmpy-core-0.95.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/conf.py` & `pharmpy-core-0.95.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.94.0'
+version = release = '0.95.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.94.0/docs/configuration.rst` & `pharmpy-core-0.95.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/contribute.rst` & `pharmpy-core-0.95.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/covsearch.rst` & `pharmpy-core-0.95.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/crossval.rst` & `pharmpy-core-0.95.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/custom.css` & `pharmpy-core-0.95.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/data.rst` & `pharmpy-core-0.95.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/design.rst` & `pharmpy-core-0.95.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/estmethod.rst` & `pharmpy-core-0.95.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/frem.rst` & `pharmpy-core-0.95.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/getting_started.rst` & `pharmpy-core-0.95.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/help_functions.py` & `pharmpy-core-0.95.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/iivsearch.rst` & `pharmpy-core-0.95.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.95.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/images/tools.png` & `pharmpy-core-0.95.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/index.rst` & `pharmpy-core-0.95.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/iovsearch.rst` & `pharmpy-core-0.95.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/license.rst` & `pharmpy-core-0.95.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/linearize.rst` & `pharmpy-core-0.95.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/model.rst` & `pharmpy-core-0.95.0/docs/model.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/modelfit.rst` & `pharmpy-core-0.95.0/docs/modelfit.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/modeling.rst` & `pharmpy-core-0.95.0/docs/modeling.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/modelsearch.rst` & `pharmpy-core-0.95.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/nonmem_plugin.rst` & `pharmpy-core-0.95.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/pharmr_logo.svg` & `pharmpy-core-0.95.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/plots.rst` & `pharmpy-core-0.95.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/plugins.rst` & `pharmpy-core-0.95.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/projects.rst` & `pharmpy-core-0.95.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/qa.rst` & `pharmpy-core-0.95.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/ruvsearch.rst` & `pharmpy-core-0.95.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/scm.rst` & `pharmpy-core-0.95.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/simeval.rst` & `pharmpy-core-0.95.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/tools.rst` & `pharmpy-core-0.95.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/docs/using_r.rst` & `pharmpy-core-0.95.0/docs/using_r.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/requirements.txt` & `pharmpy-core-0.95.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 appdirs==1.4.4
 asttokens==2.2.1
 attrs==23.1.0
 Babel==2.12.1
 backcall==0.2.0
 beautifulsoup4==4.12.2
 bleach==6.0.0
-certifi==2022.12.7
+certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
 cloudpickle==2.2.1
 comm==0.1.3
 commonmark==0.9.1
 csscompressor==0.9.5
-dask==2023.4.0
+dask==2023.5.0
 debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
-distributed==2023.4.0
-docutils==0.19.0
+distributed==2023.5.0
+docutils==0.20.1
 entrypoints==0.4
 executing==1.2.0
-fastjsonschema==2.16.3
-fsspec==2023.4.0
+fastjsonschema==2.17.0
+fsspec==2023.5.0
 HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
 importlib_metadata==6.6.0
-ipykernel==6.22.0
-ipython==8.12.0
+ipykernel==6.23.1
+ipython==8.13.2
 ipywidgets==8.0.6
 jedi==0.18.2
 Jinja2==3.1.2
 jsonschema==4.17.3
 jupyter-client==8.2.0
 jupyter-core==5.3.0
 jupyter-sphinx==0.4.0
@@ -44,69 +44,66 @@
 lxml==4.9.2
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
 nbclient==0.7.4
-nbconvert==7.3.1
+nbconvert==7.4.0
 nbformat==5.8.0
 nest-asyncio==1.5.6
 networkx==3.1
 numexpr==2.8.4
 numpy==1.24.3
 packaging==23.1
 pandas==1.5.3
 pandocfilters==1.5.0
 parso==0.8.3
 partd==1.4.0
 pexpect==4.8.0
 pickleshare==0.7.5
-platformdirs==3.3.0
+platformdirs==3.5.1
 prompt-toolkit==3.0.38
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 Pygments==2.15.1
 pyreadr==0.4.7
 pyrsistent==0.19.3
 python-dateutil==2.8.2
 pytz==2023.3
 pywin32>=302,!=304; sys_platform == 'win32' and platform_python_implementation != 'PyPy'
 PyYAML==6.0
-requests==2.28.2
+requests==2.30.0
 pyzmq==25.0.2
-rich==13.3.4
+rich==13.3.5
 scipy==1.10.1
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 soupsieve==2.4.1
-Sphinx==6.2.1
+Sphinx==7.0.1
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxcontrib.applehelp==1.0.4
 stack-data==0.6.2
 symengine==0.10.0
-sympy==1.11.1
+sympy==1.12
 tblib==1.7.0
 tinycss2==1.2.1
 toolz==0.12.0
-tornado==6.3.1
+tornado==6.3.2
 traitlets==5.9.0
-urllib3==1.26.15
+urllib3==2.0.2
 wcwidth==0.2.6
 webencodings==0.5.1
 widgetsnbextension==4.0.7
 zict==3.0.0
 zipp==3.15.0
-tflite-runtime==2.11.0; sys_platform == 'linux' and python_version == '3.8'
-tflite-runtime==2.11.0; sys_platform == 'linux' and python_version == '3.9'
-tflite-runtime==2.5.0; sys_platform == 'darwin' and python_version == '3.8'
+tflite-runtime==2.12.0; sys_platform == 'linux' and python_version == '3.9'
 tflite_runtime @ https://github.com/hjonnala/snippets/raw/main/wheels/python3.10/tflite_runtime-2.5.0.post1-cp310-cp310-linux_x86_64.whl ; sys_platform == 'linux' and python_version == '3.10'
 --extra-index-url https://google-coral.github.io/py-repo/
 tflite_runtime==2.5.0.post1; sys_platform == 'darwin' and python_version == '3.9'
-tflite_runtime==2.5.0.post1; sys_platform == 'win32' and python_version == '3.8'
 tflite_runtime==2.5.0.post1; sys_platform == 'win32' and python_version == '3.9'
```

### Comparing `pharmpy-core-0.94.0/setup.cfg` & `pharmpy-core-0.95.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/setup.py` & `pharmpy-core-0.95.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.94.0',
+    version='0.95.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/cli.py` & `pharmpy-core-0.95.0/src/pharmpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,21 +246,21 @@
     run_amd(
         args.input_path,
         modeltype=args.modeltype,
         cl_init=args.cl_init,
         vc_init=args.vc_init,
         mat_init=args.mat_init,
         search_space=args.search_space,
-        lloq=args.lloq,
+        lloq_method=args.lloq_method,
+        lloq_limit=args.lloq_limit,
         order=args.order,
-        categorical=args.categorical,
-        continuous=args.continuous,
         allometric_variable=args.allometric_variable,
         occasion=args.occasion,
         path=args.path,
+        resume=args.resume,
     )
 
 
 def data_write(args):
     """Subcommand to write a dataset."""
     try:
         from pharmpy.modeling import write_csv
@@ -1339,36 +1339,32 @@
                             {
                                 'name': '--search_space',
                                 'type': str,
                                 'default': None,
                                 'help': 'MFL for search space for structural model',
                             },
                             {
-                                'name': '--lloq',
-                                'type': float,
-                                'default': None,
-                                'help': 'Lower limit of quantification. LOQ data will be removed.',
-                            },
-                            {
-                                'name': '--order',
-                                'type': comma_list,
+                                'name': '--lloq_method',
+                                'type': str,
                                 'default': None,
-                                'help': 'Runorder of components',
+                                'help': 'Method for how to remove LOQ data. See '
+                                '`transform_blq` for list of available methods',
                             },
                             {
-                                'name': '--categorical',
-                                'type': comma_list,
+                                'name': '--lloq_limit',
+                                'type': float,
                                 'default': None,
-                                'help': 'List of categorical covariates',
+                                'help': 'Lower limit of quantification. If None LLOQ column '
+                                'from dataset will be used',
                             },
                             {
-                                'name': '--continuous',
+                                'name': '--order',
                                 'type': comma_list,
                                 'default': None,
-                                'help': 'List of continuous covariates',
+                                'help': 'Runorder of components',
                             },
                             {
                                 'name': '--allometric_variable',
                                 'type': str,
                                 'default': None,
                                 'help': 'Variable to use for allometry',
                             },
@@ -1380,14 +1376,20 @@
                             },
                             {
                                 'name': '--path',
                                 'type': str,
                                 'default': None,
                                 'help': 'Path to run AMD in',
                             },
+                            {
+                                'name': '--resume',
+                                'type': bool,
+                                'default': True,
+                                'help': 'Whether to allow resuming previous run',
+                            },
                         ],
                     }
                 },
             ],
             'help': 'Run a tool',
             'title': 'Pharmpy commands for running tools',
             'metavar': 'TOOL',
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/config.py` & `pharmpy-core-0.95.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/deps/altair.py` & `pharmpy-core-0.95.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/df.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/fn/type.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/fs/tmp.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/math.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/ignored.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.95.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/data.py` & `pharmpy-core-0.95.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.95.0/src/pharmpy/model/datainfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import Optional, Tuple, Union, cast, overload
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.units import parse as parse_units
 from pharmpy.internals.fs.path import path_absolute, path_relative_to
-from pharmpy.internals.immutable import Immutable
+from pharmpy.internals.immutable import Immutable, frozenmapping
 
 
 class ColumnInfo(Immutable):
     """Information about one data column
 
     Parameters
     ----------
@@ -25,16 +25,16 @@
         Type (see the "type" attribute)
     unit : str
         Unit (see the "unit" attribute)
     scale : str
         Scale of measurement (see the "scale" attribute)
     continuous : bool
         True if continuous or False if discrete
-    categories : list
-        List of all possible categories
+    categories : Optional[Union[Tuple, Dict]]
+        Tuple of all possible categories or dict from value to label for each category
     drop : bool
         Should column be dropped (i.e. barred from being used)
     datatype : str
         Pandas datatype or special Pharmpy datatype (see the "dtype" attribute)
     descriptor : str
         Descriptor (kind) of data
     """
@@ -82,14 +82,16 @@
         'body weight',
         'lean body mass',
         'fat free mass',
         'time after dose',
         'plasma concentration',
         'subject identifier',
         'observation identifier',
+        'pk measurement',
+        'pd measurement',
     )
 
     @staticmethod
     def convert_pd_dtype_to_datatype(dtype):
         """Convert pandas dtype to Pharmpy datatype
 
         Parameters
@@ -155,14 +157,29 @@
         self._scale = scale
         self._continuous = continuous
         self._categories = categories
         self._drop = drop
         self._datatype = datatype
         self._descriptor = descriptor
 
+    @staticmethod
+    def _canonicalize_categories(categories):
+        if isinstance(categories, dict):
+            return frozenmapping(categories)
+        elif isinstance(categories, frozenmapping):
+            return categories
+        elif isinstance(categories, list):
+            return tuple(categories)
+        elif isinstance(categories, tuple):
+            return categories
+        elif categories is None:
+            return categories
+        else:
+            raise TypeError("categories must be None, list-like or dict-like")
+
     @classmethod
     def create(
         cls,
         name,
         type='unknown',
         unit=None,
         scale='ratio',
@@ -190,14 +207,16 @@
         unit = sympy.Integer(1) if unit is None else parse_units(unit)
         if datatype not in ColumnInfo._all_dtypes:
             raise ValueError(
                 f"{datatype} is not a valid datatype. Valid datatypes are {ColumnInfo._all_dtypes}"
             )
         if descriptor not in ColumnInfo._all_descriptors:
             raise TypeError(f"Unknown column descriptor {descriptor}")
+        categories = ColumnInfo._canonicalize_categories(categories)
+
         return cls(
             name=name,
             type=type,
             unit=unit,
             scale=scale,
             continuous=continuous,
             categories=categories,
@@ -222,14 +241,57 @@
             and self._scale == other._scale
             and self._continuous == other._continuous
             and self._categories == other._categories
             and self._drop == other._drop
             and self._datatype == other._datatype
         )
 
+    def __hash__(self):
+        return hash(
+            (
+                self._name,
+                self._type,
+                self._unit,
+                self._scale,
+                self._continuous,
+                # FIXME: What are categories really?
+                # self._categories,
+                self._drop,
+                self._datatype,
+                self._descriptor,
+            )
+        )
+
+    def to_dict(self):
+        return {
+            'name': self._name,
+            'type': self._type,
+            'unit': sympy.srepr(self._unit),
+            'scale': self._scale,
+            'continuous': self._continuous,
+            'categories': self._categories,
+            'drop': self._drop,
+            'datatype': self._datatype,
+            'descriptor': self._descriptor,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            name=d['name'],
+            type=d['type'],
+            unit=sympy.parse_expr(d['unit']),
+            scale=d['scale'],
+            continuous=d['continuous'],
+            categories=d['categories'],
+            drop=d['drop'],
+            datatype=d['datatype'],
+            descriptor=d['descriptor'],
+        )
+
     @property
     def name(self):
         """Column name"""
         return self._name
 
     @property
     def type(self):
@@ -271,14 +333,16 @@
         body weight            Human body weight
         lean body mass         Lean body mass
         fat free mass          Fat free mass
         time after dose        Time after dose
         plasma concentration   Concentration of substance in blood plasma
         subject identifier     Unique integer identifier for a subject
         observation identifier Unique integer identifier for an observation
+        pk measurement         Any kind of PK measurement
+        pd measurement         Any kind of PD measurement
         ====================== ============================================
         """
         return self._descriptor
 
     @property
     def unit(self):
         """Unit of the column data
@@ -304,15 +368,15 @@
         True for continuous data and False for discrete. Note that nominal and ordinal data have to
         be discrete.
         """
         return self._continuous
 
     @property
     def categories(self):
-        """List of allowed categories"""
+        """List or dict of allowed categories"""
         return self._categories
 
     @property
     def drop(self):
         """Should this column be dropped"""
         return self._drop
 
@@ -421,14 +485,21 @@
             'int64',
             'uint8',
             'uint16',
             'uint32',
             'uint64',
         ]
 
+    def get_all_categories(self):
+        """Get a list of all categories"""
+        if isinstance(self._categories, tuple):
+            return list(self._categories)
+        else:
+            return list(self._categories.keys())
+
     def __repr__(self):
         ser = pd.Series(
             [
                 self._type,
                 self._scale,
                 self._continuous,
                 self._categories,
@@ -465,16 +536,16 @@
         Path to dataset file
     separator : str
         Character or regexp separator for dataset
     """
 
     def __init__(
         self,
-        columns: Optional[Union[Sequence[ColumnInfo], Sequence[str]]] = (),
-        path: Optional[Union[str, Path]] = None,
+        columns: tuple[ColumnInfo, ...] = (),
+        path: Optional[Path] = None,
         separator: str = ',',
         force_absolute_path: bool = True,
     ):
         self._columns = columns
         self._path = path
         self._separator = separator
         self._force_absolute_path = force_absolute_path
@@ -495,16 +566,25 @@
             columns = cast(Tuple[ColumnInfo, ...], tuple(columns))
         if path is not None:
             path = Path(path)
         assert not force_absolute_path or path is None or path.is_absolute()
         return cls(columns=columns, path=path, separator=separator)
 
     def replace(self, **kwargs):
-        columns = kwargs.get('columns', self._columns)
-        path = kwargs.get('path', self._path)
+        if 'columns' in kwargs:
+            columns = tuple(kwargs['columns'])
+        else:
+            columns = self._columns
+        if 'path' in kwargs:
+            if kwargs['path'] is not None:
+                path = Path(kwargs['path'])
+            else:
+                path = None
+        else:
+            path = self._path
         separator = kwargs.get('separator', self._separator)
         return DataInfo.create(columns=columns, path=path, separator=separator)
 
     def __add__(self, other):
         if isinstance(other, DataInfo):
             return DataInfo.create(
                 columns=self._columns + other._columns, path=self.path, separator=self.separator
@@ -534,14 +614,17 @@
         if len(self) != len(other):
             return False
         for col1, col2 in zip(self, other):
             if col1 != col2:
                 return False
         return True
 
+    def __hash__(self):
+        return hash(self._columns)
+
     def __len__(self):
         return len(self._columns)
 
     def _getindex(self, i):
         if isinstance(i, str):
             for n, col in enumerate(self._columns):
                 if col.name == i:
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.95.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.95.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,32 @@
 
     def __len__(self):
         return 1
 
     def __hash__(self):
         return hash((self._name, self._level, self._mean, self._variance))
 
+    def to_dict(self):
+        return {
+            'class': self.__class__.__name__,
+            'name': self._name,
+            'level': self._level,
+            'mean': sympy.srepr(self._mean),
+            'variance': sympy.srepr(self._variance),
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            name=d['name'],
+            level=d['level'],
+            mean=sympy.parse_expr(d['mean']),
+            variance=sympy.parse_expr(d['variance']),
+        )
+
     def __repr__(self):
         return (
             f'{sympy.pretty(sympy.Symbol(self._name), wrap_line=False, use_unicode=True)}'
             f' ~ {unicode.mathematical_script_capital_n}'
             f'({sympy.pretty(self._mean, wrap_line=False, use_unicode=True)}, '
             f'{sympy.pretty(self._variance, wrap_line=False, use_unicode=True)})'
         )
@@ -460,14 +478,32 @@
 
     def __len__(self):
         return len(self._names)
 
     def __hash__(self):
         return hash((self._names, self._level, self._mean, self._variance))
 
+    def to_dict(self):
+        return {
+            'class': self.__class__.__name__,
+            'names': self._names,
+            'level': self._level,
+            'mean': sympy.srepr(self._mean),
+            'variance': sympy.srepr(self._variance),
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            names=d['names'],
+            level=d['level'],
+            mean=sympy.parse_expr(d['mean']),
+            variance=sympy.parse_expr(d['variance']),
+        )
+
     def __repr__(self):
         name_vector = sympy.Matrix(self._names)
         name_strings = sympy.pretty(name_vector, wrap_line=False, use_unicode=True).split('\n')
         mu_strings = sympy.pretty(self._mean, wrap_line=False, use_unicode=True).split('\n')
         sigma_strings = sympy.pretty(self._variance, wrap_line=False, use_unicode=True).split('\n')
         mu_height = len(mu_strings)
         sigma_height = len(sigma_strings)
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/estimation.py` & `pharmpy-core-0.95.0/src/pharmpy/model/estimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,14 +270,56 @@
             and self.keep_every_nth_iter == other.keep_every_nth_iter
             and self.solver == other.solver
             and self.solver_rtol == other.solver_rtol
             and self.solver_atol == other.solver_atol
             and self.tool_options == other.tool_options
         )
 
+    def __hash__(self):
+        return hash(
+            (
+                self._method,
+                self._interaction,
+                self._cov,
+                self._evaluation,
+                self._maximum_evaluations,
+                self._laplace,
+                self._isample,
+                self._niter,
+                self._auto,
+                self._keep_every_nth_iter,
+                self._solver,
+                self._solver_rtol,
+                self._solver_atol,
+                self._tool_options,
+            )
+        )
+
+    def to_dict(self):
+        return {
+            'method': self._method,
+            'interaction': self._interaction,
+            'cov': self._cov,
+            'evaluation': self._evaluation,
+            'maximum_evaluations': self._maximum_evaluations,
+            'laplace': self._laplace,
+            'isample': self._isample,
+            'niter': self._niter,
+            'auto': self._auto,
+            'keep_every_nth_iter': self._keep_every_nth_iter,
+            'solver': self._solver,
+            'solver_rtol': self._solver_rtol,
+            'solver_atol': self._solver_atol,
+            'tool_options': self._tool_options,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(**d)
+
     def __repr__(self):
         return (
             f'EstimationStep("{self.method}", interaction={self.interaction}, '
             f'cov={self.cov}, evaluation={self.evaluation}, '
             f'maximum_evaluations={self.maximum_evaluations}, laplace={self.laplace}, '
             f'isample={self.isample}, niter={self.niter}, auto={self.auto}, '
             f'keep_every_nth_iter={self.keep_every_nth_iter}, solver={self.solver}, '
@@ -344,14 +386,24 @@
         if len(self) != len(other):
             return False
         for s1, s2 in zip(self, other):
             if s1 != s2:
                 return False
         return True
 
+    def __hash__(self):
+        return hash(self._steps)
+
+    def to_dict(self):
+        return {'steps': tuple(step.to_dict() for step in self._steps)}
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(steps=tuple(EstimationStep.from_dict(s) for s in d['steps']))
+
     def to_dataframe(self):
         """Convert to DataFrame
 
         Use this to create an overview of all estimation steps
 
         Returns
         -------
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/model.py` & `pharmpy-core-0.95.0/src/pharmpy/model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 import warnings
 from io import IOBase
 from pathlib import Path
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
-from pharmpy.internals.immutable import Immutable
+from pharmpy.internals.immutable import Immutable, frozenmapping
 from pharmpy.plugins.utils import detect_model
 
 from .datainfo import ColumnInfo, DataInfo
 from .estimation import EstimationSteps
 from .parameters import Parameters
 from .random_variables import RandomVariables
-from .statements import Statements
+from .statements import ODESystem, Statements
 
 
 class ModelError(Exception):
     """Exception for errors in model object"""
 
     pass
 
@@ -74,19 +74,23 @@
         )
         self._name = name
         self._datainfo = datainfo
         self._dataset = dataset
         self._random_variables = random_variables
         self._parameters = parameters
         self._statements = statements
-        self._dependent_variables = actual_dependent_variables
+        # FIXME: Only do this conversion in the future Model.create
+        self._dependent_variables = frozenmapping(actual_dependent_variables)
         if observation_transformation is None:
-            self._observation_transformation = {dv: dv for dv in actual_dependent_variables.keys()}
+            self._observation_transformation = frozenmapping(
+                {dv: dv for dv in actual_dependent_variables.keys()}
+            )
         else:
-            self._observation_transformation = observation_transformation
+            # FIXME: Only do this conversion in the future Model.create
+            self._observation_transformation = frozenmapping(observation_transformation)
         self._estimation_steps = estimation_steps
         self._modelfit_results = modelfit_results
         self._parent_model = parent_model
         self._initial_individual_estimates = initial_individual_estimates
         self._filename_extension = filename_extension
         self._value_type = value_type
         self._description = description
@@ -121,40 +125,70 @@
 
     @staticmethod
     def _canonicalize_random_variables(rvs):
         if not isinstance(rvs, RandomVariables):
             raise TypeError("model.random_variables must be of RandomVariables type")
 
     @staticmethod
-    def _canonicalize_statements(statements):
+    def _canonicalize_statements(statements, params, rvs, datainfo):
         if not isinstance(statements, Statements):
             raise TypeError("model.statements must be of Statements type")
+        colnames = {sympy.Symbol(colname) for colname in datainfo.names}
+        symbs_all = rvs.free_symbols.union(params.symbols).union(colnames)
+        sset_prev = []
+        for i, statement in enumerate(statements):
+            if isinstance(statement, ODESystem):
+                continue
+
+            symbs = statement.expression.free_symbols
+            if not symbs.issubset(symbs_all):
+                # E.g. after solve_ode_system
+                if isinstance(statement.symbol, sympy.Function):
+                    symbs_all.add(sympy.Symbol(statement.symbol.func.__name__))
+                    continue
+
+                for symb in symbs:
+                    if symb in symbs_all:
+                        continue
+                    if str(symb) == 'NaN':
+                        continue
+                    if statements.find_assignment(symb) is None:
+                        if statements.ode_system and symb in statements.ode_system.amounts:
+                            continue
+                        raise ValueError(f'Symbol {symb} is not defined')
+                    if Statements(sset_prev).find_assignment_index(symb) is None:
+                        raise ValueError(f'Symbol {symb} defined after being used')
+
+            sset_prev += statement
 
     def replace(self, **kwargs):
         name = kwargs.get('name', self.name)
         if not isinstance(name, str):
             raise TypeError("Name of a model has to be of string type")
 
-        dependent_variables = kwargs.get('dependent_variables', self.dependent_variables)
+        if 'dependent_variables' in kwargs:
+            dependent_variables = frozenmapping(kwargs['dependent_variables'])
+        else:
+            dependent_variables = self.dependent_variables
+
+        if 'observation_transformation' in kwargs:
+            observation_transformation = frozenmapping(kwargs['observation_transformation'])
+        else:
+            observation_transformation = self.observation_transformation
+
         parameters = kwargs.get('parameters', self.parameters)
 
         if 'random_variables' in kwargs:
             random_variables = kwargs['random_variables']
             Model._canonicalize_random_variables(random_variables)
         else:
             random_variables = self.random_variables
 
         parameters = Model._canonicalize_parameter_estimates(parameters, random_variables)
 
-        if 'statements' in kwargs:
-            statements = kwargs['statements']
-            Model._canonicalize_statements(statements)
-        else:
-            statements = self.statements
-
         if 'dataset' in kwargs:
             dataset = kwargs['dataset']
             new_dataset = True
         else:
             dataset = self._dataset
             new_dataset = False
 
@@ -164,14 +198,21 @@
                 raise TypeError("model.datainfo must be of DataInfo type")
         else:
             datainfo = self._datainfo
 
         if new_dataset:
             datainfo = update_datainfo(datainfo, dataset)
 
+        # Has to be checked after datainfo is updated since it looks for symbols in datainfo as well
+        if 'statements' in kwargs:
+            statements = kwargs['statements']
+            Model._canonicalize_statements(statements, parameters, random_variables, datainfo)
+        else:
+            statements = self.statements
+
         estimation_steps = kwargs.get('estimation_steps', self.estimation_steps)
         if not isinstance(estimation_steps, EstimationSteps):
             raise TypeError("model.estimation_steps must be of EstimationSteps type")
         modelfit_results = kwargs.get('modelfit_results', self.modelfit_results)
         parent_model = kwargs.get('parent_model', self.parent_model)
         initial_individual_estimates = kwargs.get(
             'initial_individual_estimates', self.initial_individual_estimates
@@ -180,17 +221,14 @@
         if not isinstance(filename_extension, str):
             raise TypeError("Filename extension has to be of string type")
         if 'value_type' in kwargs:
             value_type = self._canonicalize_value_type(kwargs['value_type'])
         else:
             value_type = self.value_type
         description = kwargs.get('description', self.description)
-        observation_transformation = kwargs.get(
-            'observation_transformation', self.observation_transformation
-        )
         internals = kwargs.get('internals', self._internals)
         return self.__class__(
             name=name,
             dependent_variables=dependent_variables,
             parameters=parameters,
             random_variables=random_variables,
             statements=statements,
@@ -264,14 +302,29 @@
         if self.datainfo != other.datainfo:
             return False
         if self.value_type != other.value_type:
             return False
 
         return True
 
+    def __hash__(self):
+        return hash(
+            (
+                self._parameters,
+                self._random_variables,
+                self._statements,
+                self._dependent_variables,
+                self._observation_transformation,
+                self._estimation_steps,
+                self._initial_individual_estimates,
+                self._datainfo,
+                self._value_type,
+            )
+        )
+
     def __repr__(self):
         return f'<Pharmpy model object {self.name}>'
 
     def _repr_html_(self):
         stat = self.statements._repr_html_()
         rvs = self.random_variables._repr_latex_()
         return f'<hr>{stat}<hr>${rvs}$<hr>{self.parameters._repr_html_()}<hr>'
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/parameters.py` & `pharmpy-core-0.95.0/src/pharmpy/model/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,28 @@
 
     @property
     def init(self):
         """Initial parameter estimate or value"""
         return self._init
 
     def __hash__(self):
-        return hash(self.name)
+        return hash((self.name, self.init, self.lower, self.upper, self.fix))
+
+    def to_dict(self):
+        return {
+            'name': self.name,
+            'init': self.init,
+            'lower': self.lower,
+            'upper': self.upper,
+            'fix': self.fix,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(**d)
 
     def __eq__(self, other):
         """Two parameters are equal if they have the same name, init and constraints"""
         return (
             isinstance(other, Parameter)
             and self._init == other._init
             and self._lower == other._lower
@@ -386,14 +399,26 @@
         if len(self) != len(other):
             return False
         for p1, p2 in zip(self, other):
             if p1 != p2:
                 return False
         return True
 
+    def __hash__(self):
+        return hash(self._params)
+
+    def to_dict(self):
+        params = tuple(p.to_dict() for p in self._params)
+        return {'parameters': params}
+
+    @classmethod
+    def from_dict(cls, d):
+        params = tuple(Parameter.from_dict(p) for p in d['parameters'])
+        return cls(parameters=params)
+
     def __repr__(self):
         if len(self) == 0:
             return "Parameters()"
         return (
             self.to_dataframe().replace(float("inf"), "∞").replace(-float("inf"), "-∞").to_string()
         )
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.95.0/src/pharmpy/model/random_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,24 @@
         return (
             isinstance(other, VariabilityLevel)
             and self._name == other._name
             and self._reference == other._reference
             and self._group == other._group
         )
 
+    def __hash__(self):
+        return hash((self._name, self._reference, self._group))
+
+    def to_dict(self):
+        return {'name': self._name, 'reference': self._reference, 'group': self._group}
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(**d)
+
     @property
     def name(self) -> str:
         """Name of the variability level"""
         return self._name
 
     @property
     def reference(self) -> bool:
@@ -121,14 +131,26 @@
             return False
         else:
             for l1, l2 in zip(self._levels, other._levels):
                 if l1 != l2:
                     return False
             return True
 
+    def __hash__(self):
+        return hash(self._levels)
+
+    def to_dict(self):
+        levels = tuple(level.to_dict() for level in self._levels)
+        return {'levels': levels}
+
+    @classmethod
+    def from_dict(cls, d):
+        levels = tuple(VariabilityLevel.from_dict(vl) for vl in d['levels'])
+        return cls(levels=levels)
+
     def _lookup(self, ind: Union[int, str, VariabilityLevel]) -> VariabilityLevel:
         # Lookup one index
         if isinstance(ind, int):
             # Index on numeric level for ints
             i = self._find_reference()
             return self._levels[ind - i]
         elif isinstance(ind, str):
@@ -351,14 +373,38 @@
                     return False
             return (
                 self._eta_levels == other._eta_levels
                 and self._epsilon_levels == other._epsilon_levels
             )
         return False
 
+    def __hash__(self):
+        return hash((self._dists, self._eta_levels, self._epsilon_levels))
+
+    def to_dict(self):
+        dists = tuple(d.to_dict() for d in self._dists)
+        return {
+            'dists': dists,
+            'eta_levels': self._eta_levels.to_dict(),
+            'epsilon_levels': self._epsilon_levels.to_dict(),
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        eta_levels = VariabilityHierarchy.from_dict(d['eta_levels'])
+        epsilon_levels = VariabilityHierarchy.from_dict(d['epsilon_levels'])
+        dists = []
+        for dist_dict in d['dists']:
+            if dist_dict['class'] == 'NormalDistribution':
+                dist = NormalDistribution.from_dict(dist_dict)
+            else:
+                dist = JointNormalDistribution.from_dict(dist_dict)
+            dists.append(dist)
+        return cls(dists=tuple(dists), eta_levels=eta_levels, epsilon_levels=epsilon_levels)
+
     def _lookup_rv(self, ind):
         if isinstance(ind, sympy.Symbol):
             ind = ind.name
         if isinstance(ind, str):
             for i, dist in enumerate(self._dists):
                 if ind in dist.names:
                     return i, dist
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/results.py` & `pharmpy-core-0.95.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/model/statements.py` & `pharmpy-core-0.95.0/src/pharmpy/model/statements.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,30 @@
     def __eq__(self, other):
         return (
             isinstance(other, Assignment)
             and self.symbol == other.symbol
             and self.expression == other.expression
         )
 
+    def __hash__(self):
+        return hash((self.symbol, self.expression))
+
+    def to_dict(self):
+        return {
+            'class': 'Assignment',
+            'symbol': sympy.srepr(self.symbol),
+            'expression': sympy.srepr(self.expression),
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            symbol=sympy.parse_expr(d['symbol']), expression=sympy.parse_expr(d['expression'])
+        )
+
     def __repr__(self):
         expression = sympy.pretty(self.expression)
         lines = [line.rstrip() for line in expression.split('\n')]
         definition = f'{sympy.pretty(self.symbol)} = '
         s = ''
         for line in lines:
             if line == lines[-1]:
@@ -190,14 +206,21 @@
 
     def __repr__(self):
         return "Output()"
 
     def __hash__(self):
         return 5267
 
+    def to_dict(self):
+        return {'class': 'Output'}
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls.instance
+
     def __eq__(self, other):
         return self is other
 
 
 output = Output()
 
 
@@ -387,14 +410,19 @@
             The new updated compartment
         """
         new_comp = compartment.replace(input=input)
         mapping = {compartment: new_comp}
         nx.relabel_nodes(self._g, mapping, copy=False)
         return new_comp
 
+    def find_compartment(self, name):
+        for comp in self._g.nodes:
+            if not isinstance(comp, Output) and comp.name == name:
+                return comp
+
 
 def _is_positive(expr: sympy.Expr) -> bool:
     return sympy.ask(
         sympy.Q.positive(expr), assume_all(sympy.Q.positive, free_images_and_symbols(expr))
     )
 
 
@@ -645,14 +673,55 @@
         return (
             isinstance(other, CompartmentalSystem)
             and self._t == other._t
             and nx.to_dict_of_dicts(self._g) == nx.to_dict_of_dicts(other._g)
             and self.dosing_compartment.dose == other.dosing_compartment.dose
         )
 
+    def __hash__(self):
+        return hash((self._t, self._g))
+
+    def to_dict(self):
+        comps = [comp for comp in self._g.nodes]
+        comps_dicts = tuple(comp.to_dict() for comp in comps)
+
+        edges = []
+        for from_comp, to_comp, rate in self._g.edges.data('rate'):
+            from_n = comps.index(from_comp)
+            to_n = comps.index(to_comp)
+            edge = (from_n, to_n, sympy.srepr(rate))
+            edges.append(edge)
+
+        d = {
+            'class': 'CompartmentalSystem',
+            'compartments': comps_dicts,
+            'rates': edges,
+            't': sympy.srepr(self._t),
+        }
+        return d
+
+    @classmethod
+    def from_dict(cls, d):
+        cb = CompartmentalSystemBuilder()
+        comps = []
+        for comp_dict in d['compartments']:
+            if comp_dict['class'] == 'Output':
+                compartment = output
+            else:
+                compartment = Compartment.from_dict(comp_dict)
+                cb.add_compartment(compartment)
+            comps.append(compartment)
+
+        for from_n, to_n, rate in d['rates']:
+            from_comp = comps[from_n]
+            to_comp = comps[to_n]
+            cb.add_flow(from_comp, to_comp, sympy.parse_expr(rate))
+
+        return cls(cb, t=sympy.parse_expr(d['t']))
+
     def get_flow(self, source, destination):
         """Get the rate of flow between two compartments
 
         Parameters
         ----------
         source : Compartment
             Source compartment
@@ -1366,23 +1435,65 @@
             lag_time=subs(self._lag_time, substitutions),
             bioavailability=subs(self._bioavailability, substitutions),
         )
 
     def __eq__(self, other):
         return (
             isinstance(other, Compartment)
-            and self.name == other.name
-            and self.amount == other.amount
-            and self.dose == other.dose
-            and self.input == other.input
-            and self.lag_time == other.lag_time
+            and self._name == other._name
+            and self._amount == other._amount
+            and self._dose == other._dose
+            and self._input == other._input
+            and self._lag_time == other._lag_time
+            and self._bioavailability == other._bioavailability
         )
 
     def __hash__(self):
-        return hash(self.name)
+        return hash(
+            (
+                self._name,
+                self._amount,
+                self._dose,
+                self._input,
+                self._lag_time,
+                self._bioavailability,
+            )
+        )
+
+    def to_dict(self):
+        if self._dose is None:
+            dose = None
+        else:
+            dose = self._dose.to_dict()
+        return {
+            'class': 'Compartment',
+            'name': self._name,
+            'amount': sympy.srepr(self._amount),
+            'dose': dose,
+            'input': sympy.srepr(self._input),
+            'lag_time': sympy.srepr(self._lag_time),
+            'bioavailability': sympy.srepr(self._bioavailability),
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        if d['dose'] is None:
+            dose = None
+        elif d['dose']['class'] == 'Bolus':
+            dose = Bolus.from_dict(d['dose'])
+        else:
+            dose = Infusion.from_dict(d['dose'])
+        return cls(
+            name=d['name'],
+            amount=sympy.parse_expr(d['amount']),
+            dose=dose,
+            input=sympy.parse_expr(d['input']),
+            lag_time=sympy.parse_expr(d['lag_time']),
+            bioavailability=sympy.parse_expr(d['bioavailability']),
+        )
 
     def __repr__(self):
         lag = '' if self.lag_time == 0 else f', lag_time={self._lag_time}'
         dose = '' if self.dose is None else f', dose={self._dose}'
         input = '' if self.input == 0 else f', input={self._input}'
         bioavailability = (
             '' if self.bioavailability == 1 else f', bioavailability={self._bioavailability}'
@@ -1477,14 +1588,24 @@
     def __eq__(self, other):
         return (
             isinstance(other, Bolus)
             and self._amount == other._amount
             and self._admid == other._admid
         )
 
+    def __hash__(self):
+        return hash((self._amount, self._admid))
+
+    def to_dict(self):
+        return {'class': 'Bolus', 'amount': sympy.srepr(self._amount), 'admid': self._admid}
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(amount=sympy.parse_expr(d['amount']), admid=d['admid'])
+
     def __repr__(self):
         return f'Bolus({self.amount}, admid={self._admid})'
 
 
 class Infusion(Dose):
     """An infusion dose
 
@@ -1608,14 +1729,35 @@
             isinstance(other, Infusion)
             and self._admid == other._admid
             and self._rate == other._rate
             and self._duration == other._duration
             and self._amount == other._amount
         )
 
+    def __hash__(self):
+        return hash((self._admid, self._rate, self._duration, self._amount))
+
+    def to_dict(self):
+        return {
+            'class': 'Infusion',
+            'amount': sympy.srepr(self._amount),
+            'rate': sympy.srepr(self._rate),
+            'duration': sympy.srepr(self._duration),
+            'admid': self._admid,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            amount=sympy.parse_expr(d['amount']),
+            admid=d['admid'],
+            rate=sympy.parse_expr(d['rate']),
+            duration=sympy.parse_expr(d['duration']),
+        )
+
     def __repr__(self):
         if self.rate is not None:
             arg = f'rate={self.rate}'
         else:
             arg = f'duration={self.duration}'
         return f'Infusion({self.amount}, admid={self._admid}, {arg})'
 
@@ -2097,14 +2239,32 @@
             return False
         else:
             for first, second in zip(self, other):
                 if first != second:
                     return False
         return True
 
+    def __hash__(self):
+        return hash(self._statements)
+
+    def to_dict(self):
+        stats = tuple(s.to_dict() for s in self)
+        return {'statements': stats}
+
+    @classmethod
+    def from_dict(cls, d):
+        statements = []
+        for sdict in d['statements']:
+            if sdict['class'] == 'Assignment':
+                s = Assignment.from_dict(sdict)
+            else:
+                s = CompartmentalSystem.from_dict(sdict)
+            statements.append(s)
+        return cls(tuple(statements))
+
     def __repr__(self):
         return '\n'.join([repr(statement) for statement in self])
 
     def _repr_html_(self):
         html = r'\begin{align*}'
         for statement in self:
             if hasattr(statement, '_repr_html_'):
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
 from .plots import (
     plot_individual_predictions,
     plot_iofv_vs_iofv,
     plot_transformed_eta_distributions,
 )
 from .remove_iiv import remove_iiv
 from .remove_iov import remove_iov
-from .reporting import create_report
 from .results import (
     calculate_aic,
     calculate_bic,
     calculate_eta_shrinkage,
     calculate_individual_parameter_statistics,
     calculate_individual_shrinkage,
     calculate_pk_parameters_statistics,
@@ -238,15 +237,14 @@
     'check_high_correlations',
     'check_parameters_near_bounds',
     'cleanup_model',
     'convert_model',
     'create_basic_pk_model',
     'create_config_template',
     'create_joint_distribution',
-    'create_report',
     'create_rng',
     'create_symbol',
     'deidentify_data',
     'display_odes',
     'drop_columns',
     'drop_dropped_columns',
     'evaluate_epsilon_gradient',
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/allometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import List, Optional, Union
 
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.parse import parse as parse_expr
 from pharmpy.model import Assignment, Model, Parameter, Parameters
 
-from .expressions import create_symbol
+from .expressions import _create_symbol
 from .odes import find_clearance_parameters, find_volume_parameters
 
 
 def add_allometry(
     model: Model,
     allometric_variable: Union[str, sympy.Expr] = 'WT',
     reference_value: Union[str, int, float, sympy.Expr] = 70,
@@ -110,23 +110,24 @@
     if lower_bounds is None:
         lower_bounds = [0.0] * len(parsed_parameters)
     if upper_bounds is None:
         upper_bounds = [2.0] * len(parsed_parameters)
 
     if not (len(parsed_parameters) == len(initials) == len(lower_bounds) == len(upper_bounds)):
         raise ValueError("The number of parameters, initials and bounds must be the same")
-
+    sset = model.statements
     params = list(model.parameters)
     for p, init, lower, upper in zip(parsed_parameters, initials, lower_bounds, upper_bounds):
-        symb = create_symbol(model, f'ALLO_{p.name}')
+        symb = _create_symbol(
+            sset, params, model.random_variables, model.datainfo, f'ALLO_{p.name}', False
+        )
         param = Parameter(symb.name, init=init, lower=lower, upper=upper, fix=fixed)
         params.append(param)
         expr = p * (variable / reference) ** param.symbol
         new_ass = Assignment(p, expr)
-        ind = model.statements.find_assignment_index(p)
-        statements = model.statements[0 : ind + 1] + new_ass + model.statements[ind + 1 :]
-        model = model.replace(statements=statements)
+        ind = sset.find_assignment_index(p)
+        sset = sset[0 : ind + 1] + new_ass + sset[ind + 1 :]
     parameters = Parameters.create(params)
-    model = model.replace(parameters=parameters)
+    model = model.replace(statements=sset, parameters=parameters)
     model = model.update_source()
 
     return model
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/basic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     pop_cl = Parameter('POP_CL', cl_init, lower=0)
     pop_vc = Parameter('POP_VC', vc_init, lower=0)
     iiv_cl = Parameter('IIV_CL', 0.1)
     iiv_vc = Parameter('IIV_VC', 0.1)
 
     params = Parameters((pop_cl, pop_vc, iiv_cl, iiv_vc))
 
-    eta_cl_name = 'eta_cl'
+    eta_cl_name = 'ETA_CL'
     eta_cl = NormalDistribution.create(eta_cl_name, 'iiv', 0, iiv_cl.symbol)
-    eta_vc_name = 'eta_vc'
+    eta_vc_name = 'ETA_VC'
     eta_vc = NormalDistribution.create(eta_vc_name, 'iiv', 0, iiv_vc.symbol)
     rvs = RandomVariables.create([eta_cl, eta_vc])
 
     CL = sympy.Symbol('CL')
     VC = sympy.Symbol('VC')
     cl_ass = Assignment(CL, pop_cl.symbol * sympy.exp(sympy.Symbol(eta_cl_name)))
     vc_ass = Assignment(VC, pop_vc.symbol * sympy.exp(sympy.Symbol(eta_vc_name)))
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/block_rvs.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/blq.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,27 +85,29 @@
     model = model.replace(estimation_steps=est_steps_new)
 
     # FIXME: handle other DVs?
     y_symb = list(model.dependent_variables.keys())[0]
     y = sset.find_assignment(y_symb)
     ipred = y.expression.subs({rv: 0 for rv in model.random_variables.epsilons.names})
 
-    blq_symb, blq_type = get_blq_symb_and_type(model)
     if isinstance(lloq, float):
-        blq_symb = create_symbol(model, blq_symb)
+        blq_symb = create_symbol(model, 'LLOQ')
+        blq_type = 'lloq'
+    else:
+        blq_symb, blq_type = get_blq_symb_and_type(model)
 
     sd = _get_sd(model, y)
     symb_dv = sympy.Symbol(model.datainfo.dv_column.name)
     symb_fflag = create_symbol(model, 'F_FLAG')
     symb_cumd = create_symbol(model, 'CUMD')
 
     if blq_type == 'lloq':
         is_above_lloq = sympy.GreaterThan(symb_dv, blq_symb)
     else:
-        is_above_lloq = sympy.Equality(blq_symb, 1)
+        is_above_lloq = sympy.Equality(blq_symb, 0)
 
     assignments = [sd]
 
     if isinstance(lloq, float):
         lloq = Assignment(blq_symb, sympy.Float(lloq))
         assignments.append(lloq)
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/common.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -584,47 +584,54 @@
         Pharmpy model object
 
     Returns
     -------
     Model
         Pharmpy model object
     """
-    symbols = model.statements.free_symbols
+    new_rvs, new_params = _get_unused_parameters_and_rvs(
+        model.statements, model.parameters, model.random_variables
+    )
+    model = model.replace(random_variables=new_rvs, parameters=new_params)
+    return model.update_source()
+
+
+def _get_unused_parameters_and_rvs(statements, parameters, random_variables):
+    symbols = statements.free_symbols
 
     # Find unused rvs needing unjoining
     to_unjoin = []
-    for dist in model.random_variables:
+    for dist in random_variables:
         if isinstance(dist, JointNormalDistribution):
             names = dist.names
             for i, name in enumerate(names):
                 params = dist.variance[i, :].free_symbols
                 symb = sympy.Symbol(name)
                 if symb not in symbols and symbols.isdisjoint(params):
                     to_unjoin.append(name)
 
-    rvs = model.random_variables.unjoin(to_unjoin)
+    rvs = random_variables.unjoin(to_unjoin)
 
     new_dists = []
     for dist in rvs:
         if isinstance(dist, NormalDistribution):
             if not symbols.isdisjoint(dist.free_symbols):
                 new_dists.append(dist)
         else:
             new_dists.append(dist)
 
     new_rvs = RandomVariables(tuple(new_dists), rvs._eta_levels, rvs._epsilon_levels)
 
     new_params = []
-    for p in model.parameters:
+    for p in parameters:
         symb = p.symbol
         if symb in symbols or symb in new_rvs.free_symbols or (p.fix and p.init == 0):
             new_params.append(p)
 
-    model = model.replace(random_variables=new_rvs, parameters=Parameters.create(new_params))
-    return model.update_source()
+    return new_rvs, Parameters.create(new_params)
 
 
 def rename_symbols(
     model: Model, new_names: Dict[Union[str, sympy.Symbol], Union[str, sympy.Symbol]]
 ):
     """Rename symbols in the model
 
@@ -638,15 +645,20 @@
         From old name or symbol to new name or symbol
 
     Returns
     -------
     Model
         Pharmpy model object
     """
-    d = {sympy.Symbol(key): sympy.Symbol(val) for key, val in new_names.items()}
+    d = {
+        (sympy.Symbol(key) if isinstance(key, str) else key): (
+            sympy.Symbol(val) if isinstance(val, str) else val
+        )
+        for key, val in new_names.items()
+    }
 
     new = []
     for p in model.parameters:
         if p.symbol in d:
             newparam = Parameter(
                 name=d[p.symbol].name, init=p.init, lower=p.lower, upper=p.upper, fix=p.fix
             )
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/data.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/error.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from typing import List, Optional, Union
 
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.parse import parse as parse_expr
 from pharmpy.internals.expr.subs import subs
 from pharmpy.model import Assignment, Model, NormalDistribution, Parameter, Parameters, Statements
 
-from .common import remove_unused_parameters_and_rvs
+from .common import _get_unused_parameters_and_rvs, remove_unused_parameters_and_rvs
 from .data import get_observations
-from .expressions import create_symbol, get_dv_symbol
+from .expressions import _create_symbol, create_symbol, get_dv_symbol
 from .help_functions import _format_input_list, _get_epsilons
 from .parameters import add_population_parameter, fix_parameters, set_initial_estimates
 
 
-def _preparations(model):
+def _preparations(model, y=None):
     stats = model.statements
     # FIXME: handle other DVs?
-    y = list(model.dependent_variables.keys())[0]
+    if y is None:
+        y = list(model.dependent_variables.keys())[0]
     f = subs(
         model.statements.find_assignment(y.name).expression,
         {sympy.Symbol(eps): 0 for eps in model.random_variables.epsilons.names},
         simultaneous=True,
     )
     return stats, y, f
 
@@ -138,31 +139,35 @@
     set_proportional_error_model : Proportional error model
     set_combined_error_model : Combined error model
 
     """
     dv = get_dv_symbol(model, dv)
     if has_additive_error_model(model, dv):
         return model
-    stats, y, f = _preparations(model)
+    stats, y, f = _preparations(model, dv)
     ruv = create_symbol(model, 'epsilon_a')
 
     data_trans = _canonicalize_data_transformation(model, data_trans, dv)
     expr = f + ruv
 
     if data_trans != dv:
         expr = subs(data_trans, {dv: expr}, simultaneous=True).series(ruv, n=series_terms).removeO()
 
-    model = model.replace(statements=stats.reassign(y, expr))
-    model = remove_unused_parameters_and_rvs(model)
-
     sigma = create_symbol(model, 'sigma')
     model = add_population_parameter(model, sigma.name, _get_prop_init(model))
 
     eps = NormalDistribution.create(ruv.name, 'RUV', 0, sigma)
-    model = model.replace(random_variables=model.random_variables + eps)
+
+    rvs_new, params_new = _get_unused_parameters_and_rvs(
+        stats.reassign(y, expr), model.parameters, model.random_variables + eps
+    )
+
+    model = model.replace(
+        statements=stats.reassign(y, expr), random_variables=rvs_new, parameters=params_new
+    )
     return model.update_source()
 
 
 def _get_prop_init(model):
     dv_min = get_observations(model).min()
     if dv_min == 0:
         return 0.01
@@ -252,15 +257,15 @@
     set_combined_error_model : Combined error model
 
     """
     dv = get_dv_symbol(model, dv)
     if has_proportional_error_model(model, dv):
         return model
 
-    stats, y, f = _preparations(model)
+    stats, y, f = _preparations(model, dv)
     ruv = create_symbol(model, 'epsilon_p')
 
     data_trans = _canonicalize_data_transformation(model, data_trans, dv)
     ipred = create_symbol(model, 'IPREDADJ') if zero_protection else f
 
     if data_trans == sympy.log(dv):
         expr = sympy.log(ipred) + ruv
@@ -272,24 +277,28 @@
     statements = model.statements
     if zero_protection:
         guard_expr = sympy.Piecewise((2.225e-16, sympy.Eq(f, 0)), (f, True))
         guard_assignment = Assignment(ipred, guard_expr)
         ind = stats.find_assignment_index(y)
         statements = statements[0:ind] + guard_assignment + statements[ind:]
 
-    model = model.replace(statements=statements.reassign(y, expr))
-    model = remove_unused_parameters_and_rvs(model)
-
     sigma = create_symbol(model, 'sigma')
     model = add_population_parameter(model, sigma.name, 0.09)
 
     eps = NormalDistribution.create(ruv.name, 'RUV', 0, sigma)
-    model = model.replace(random_variables=model.random_variables + eps)
-    model = model.update_source()
-    return model
+
+    rvs_new, params_new = _get_unused_parameters_and_rvs(
+        stats.reassign(y, expr), model.parameters, model.random_variables + eps
+    )
+
+    model = model.replace(
+        statements=statements.reassign(y, expr), random_variables=rvs_new, parameters=params_new
+    )
+
+    return model.update_source()
 
 
 def set_combined_error_model(
     model: Model,
     dv: Union[sympy.Symbol, str, int, None] = None,
     data_trans: Optional[Union[str, sympy.Expr]] = None,
 ):
@@ -342,15 +351,15 @@
     set_additive_error_model : Additive error model
     set_proportional_error_model: Proportional error model
 
     """
     dv = get_dv_symbol(model, dv)
     if has_combined_error_model(model, dv):
         return model
-    stats, y, f = _preparations(model)
+    stats, y, f = _preparations(model, dv)
 
     expr = stats.find_assignment(y.name).expression
 
     ruv_prop = create_symbol(model, 'epsilon_p')
     ruv_add = create_symbol(model, 'epsilon_a')
 
     eta_ruv = sympy.Symbol('ETA_RV1')
@@ -393,25 +402,29 @@
         ):
             expr_combined = f + f * ruv_prop * sympy.exp(eta_ruv) + ruv_add * sympy.exp(eta_ruv)
         else:
             expr_combined = f + f * ruv_prop + ruv_add
     else:
         raise ValueError(f"Not supported data transformation {data_trans}")
 
-    model = model.replace(statements=stats.reassign(y, expr_combined))
-    model = remove_unused_parameters_and_rvs(model)
+    stats_new = stats.reassign(y, expr_combined)
 
     sigma_prop = create_symbol(model, 'sigma_prop')
     model = add_population_parameter(model, sigma_prop.name, 0.09)
     sigma_add = create_symbol(model, 'sigma_add')
     model = add_population_parameter(model, sigma_add.name, _get_prop_init(model))
 
     eps_prop = NormalDistribution.create(ruv_prop.name, 'RUV', 0, sigma_prop)
     eps_add = NormalDistribution.create(ruv_add.name, 'RUV', 0, sigma_add)
-    model = model.replace(random_variables=model.random_variables + [eps_prop, eps_add])
+
+    rvs_new, params_new = _get_unused_parameters_and_rvs(
+        stats_new, model.parameters, model.random_variables + [eps_prop, eps_add]
+    )
+    model = model.replace(statements=stats_new, random_variables=rvs_new, parameters=params_new)
+
     return model.update_source()
 
 
 def has_additive_error_model(model: Model, dv: Union[sympy.Symbol, str, int, None] = None):
     """Check if a model has an additive error model
 
     Multiple dependent variables are supported. By default the only (in case of one) or the
@@ -768,16 +781,17 @@
         + ipredass
         + stats[i + 1 : yexpr_ind]
         + yexpr
         + stats[yexpr_ind + 1 :]
     )
 
     obs = model.observation_transformation
-    obs[y] = sympy.Piecewise(
-        (sympy.log(y), sympy.Eq(lam, 0)), ((y**lam - 1) / lam, sympy.Ne(lam, 0))
+    obs = obs.replace(
+        y,
+        sympy.Piecewise((sympy.log(y), sympy.Eq(lam, 0)), ((y**lam - 1) / lam, sympy.Ne(lam, 0))),
     )
     model = model.replace(observation_transformation=obs, statements=statements)
 
     return model.update_source()
 
 
 def set_time_varying_error_model(model: Model, cutoff: float, idv: str = 'TIME'):
@@ -819,16 +833,17 @@
                 {sympy.Symbol(e): sympy.Symbol(e) * theta for e in eps.names},
                 simultaneous=True,
             ),
             idv < cutoff,
         ),
         (y.expression, True),
     )
-    model = model.replace(statements=model.statements.reassign(y.symbol, expr))
     model = add_population_parameter(model, theta.name, 0.1)
+    model = model.replace(statements=model.statements.reassign(y.symbol, expr))
+
     return model.update_source()
 
 
 def set_power_on_ruv(
     model: Model,
     list_of_eps: Optional[Union[str, list]] = None,
     lower_limit: Optional[float] = 0.01,
@@ -901,27 +916,30 @@
                 ind = sset.find_assignment_index('Y')
                 sset = sset[0:ind] + guard_assignment + sset[ind:]
             break
     else:
         alternative = None
 
     for e in eps.names:
-        theta_name = str(create_symbol(model, stem='power', force_numbering=True))
+        theta_name = str(
+            _create_symbol(
+                sset, pset, model.random_variables, model.datainfo, 'power', force_numbering=True
+            )
+        )
         if lower_limit is None:
             theta = Parameter(theta_name, theta_init)
         else:
             theta = Parameter(theta_name, theta_init, lower=lower_limit)
         pset.append(theta)
         sset = sset.subs(
             {sympy.Symbol(e) * ipred: sympy.Symbol(e)}
         )  # To avoid getting F*EPS*F**THETA
         if alternative:  # To avoid getting W*EPS*F**THETA
             sset = sset.subs({sympy.Symbol(e) * alternative: sympy.Symbol(e)})
         sset = sset.subs({sympy.Symbol(e): ipred ** sympy.Symbol(theta.name) * sympy.Symbol(e)})
-        model = model.replace(statements=sset)
 
     model = model.replace(parameters=Parameters.create(pset), statements=sset)
 
     return model.update_source()
 
 
 def get_ipred(model):
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/eta_additions.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/eta_transformations.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/evaluation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,23 +225,31 @@
     >>> create_symbol(model, "TEMP")
     TEMP
     >>> create_symbol(model, "TEMP", force_numbering=True)
     TEMP1
     >>> create_symbol(model, "CL")
     CL1
     """
-    symbols = [str(symbol) for symbol in model.statements.free_symbols]
-    params = [param.name for param in model.parameters]
-    rvs = model.random_variables.names
-    dataset_col = model.datainfo.names
-    # FIXME: handle other DVs
-    dv = list(model.dependent_variables.keys())[0]
-    misc = [dv]
+    return _create_symbol(
+        model.statements,
+        model.parameters,
+        model.random_variables,
+        model.datainfo,
+        stem,
+        force_numbering,
+    )
+
+
+def _create_symbol(statements, parameters, random_variables, datainfo, stem, force_numbering):
+    symbols = [str(symbol) for symbol in statements.free_symbols]
+    params = [param.name for param in parameters]
+    rvs = random_variables.names
+    dataset_col = datainfo.names
 
-    all_names = symbols + params + rvs + dataset_col + misc
+    all_names = symbols + params + rvs + dataset_col
 
     if str(stem) not in all_names and not force_numbering:
         return sympy.Symbol(str(stem))
 
     i = 1
     while True:
         candidate = f'{stem}{i}'
@@ -352,20 +360,18 @@
     -------
     Expression
         Simplified expression
 
     Example
     -------
     >>> from pharmpy.plugins.nonmem import conf
-    >>> conf.parameter_names = ['comment', 'basic']
     >>> from pharmpy.modeling import load_example_model, simplify_expression
     >>> model = load_example_model("pheno")
     >>> simplify_expression(model, "Abs(PTVCL)")
     PTVCL
-    >>> conf.parameter_names = ['basic']
     """
     expr = parse_expr(expr)
     d = {}
     for p in model.parameters:
         if p.fix:
             s = sympy.Float(p.init)
         elif p.upper < 0:
@@ -701,17 +707,18 @@
             subs[elt] = sympy.Symbol(f"sigma_{subscript}")
     for i, eta in enumerate(model.random_variables.etas.names, start=1):
         subscript = get_subscript(eta, i, named_subscripts)
         subs[sympy.Symbol(eta)] = sympy.Symbol(f"eta_{subscript}")
     for i, epsilon in enumerate(model.random_variables.epsilons.names, start=1):
         subscript = get_subscript(epsilon, i, named_subscripts)
         subs[sympy.Symbol(epsilon)] = sympy.Symbol(f"epsilon_{subscript}")
-    statements = model.statements.subs(subs)
-    model = model.replace(statements=statements)
-    return model.update_source()
+    from pharmpy.modeling import rename_symbols
+
+    model = rename_symbols(model, subs)
+    return model
 
 
 def get_individual_parameters(model: Model, level: str = 'all') -> List[str]:
     """Retrieves all parameters with IIV or IOV in :class:`pharmpy.model`.
 
     Parameters
     ----------
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/math.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/metabolite.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     Compartment,
     CompartmentalSystem,
     CompartmentalSystemBuilder,
     Model,
     output,
 )
 
-from .odes import add_individual_parameter
+from .error import set_proportional_error_model
+from .odes import _find_noncov_theta, add_individual_parameter
+from .parameters import set_initial_estimates
 
 
 def add_metabolite(model: Model, drug_dvid: int = 1):
     """Adds a metabolite compartment to a model
 
     The flow from the central compartment to the metabolite compartment
     will be unidirectional.
@@ -35,42 +37,49 @@
     Examples
     --------
     >>> from pharmpy.modeling import *
     >>> model = load_example_model("pheno")
     >>> model = add_metabolite(model)
 
     """
-    qm1 = sympy.Symbol('QM1')
-    model = add_individual_parameter(model, qm1.name)
-    clm1 = sympy.Symbol('CLM1')
-    model = add_individual_parameter(model, clm1.name)
-    vm1 = sympy.Symbol('VM1')
-    model = add_individual_parameter(model, vm1.name)
+    clm = sympy.Symbol('CLM')
+    model = add_individual_parameter(model, clm.name)
+    vm = sympy.Symbol('VM')
+    model = add_individual_parameter(model, vm.name)
 
     odes = model.statements.ode_system
     central = odes.central_compartment
     ke = odes.get_flow(central, output)
     cl, vc = ke.as_numer_denom()
+
+    if vc != 1:
+        pop_cl = _find_noncov_theta(model, cl)
+        pop_vc = _find_noncov_theta(model, vc)
+        pop_clm_init = model.parameters[pop_cl].init * 2.0
+        pop_vm_init = model.parameters[pop_vc].init * 0.5
+        model = set_initial_estimates(model, {'POP_CLM': pop_clm_init, 'POP_VM': pop_vm_init})
+
     cb = CompartmentalSystemBuilder(odes)
     metacomp = Compartment.create(name="METABOLITE")
     cb.add_compartment(metacomp)
-    cb.add_flow(central, metacomp, qm1 / vc)
-    cb.add_flow(metacomp, output, clm1 / vm1)
+    cb.add_flow(central, metacomp, ke)
+    cb.add_flow(metacomp, output, clm / vm)
+    cb.remove_flow(central, output)
     cs = CompartmentalSystem(cb)
 
     # dvid_col = model.datainfo.typeix['dvid'][0]
     # dvids = dvid_col.categories
 
-    conc = Assignment(sympy.Symbol('CONC_M1'), metacomp.amount / vm1)
-    y_m1 = sympy.Symbol('Y_M1')
-    y = Assignment(y_m1, conc.symbol + sympy.Symbol(model.random_variables.epsilons.names[0]))
+    conc = Assignment(sympy.Symbol('CONC_M'), metacomp.amount / vm)
+    y_m = sympy.Symbol('Y_M')
+    y = Assignment(y_m, conc.symbol)
     original_y = next(iter(model.dependent_variables))
     ind = model.statements.after_odes.find_assignment_index(original_y)
     old_after = model.statements.after_odes
     new_after = old_after[: ind + 1] + y + old_after[ind + 1 :]
     error = conc + new_after
 
-    dvs = model.dependent_variables.copy()
-    dvs[y_m1] = 2  # FIXME: Should be next DVID in categories
+    dvs = model.dependent_variables.replace(y_m, 2)  # FIXME: Should be next DVID in categories
     statements = model.statements.before_odes + cs + error
     model = model.replace(statements=statements, dependent_variables=dvs)
-    return model.update_source()
+    model = set_proportional_error_model(model, dv=2, zero_protection=False)
+    return model
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/odes.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,56 @@
         symb.name
         for symb in statements.before_odes.full_expression(sympy.Symbol(symbol_name)).free_symbols
     }
     theta_name = terms.intersection(pset.names).pop()
     return pset[theta_name]
 
 
+def _find_noncov_theta(model, paramsymb, full=False):
+    # Deterministic function to find the main theta in the expression for parasymb
+    # Set full to True if already providing a full expression
+    # Find subexpression with as few thetas and covariates as possible
+    # Stop if one theta found with no covs.
+    if full:
+        start_expr = paramsymb
+    else:
+        start_expr = model.statements.before_odes.full_expression(paramsymb)
+
+    exprs = [start_expr]
+    all_popparams = set(model.parameters.symbols)
+    all_covs = set(sympy.Symbol(name) for name in model.datainfo.names)
+
+    while exprs:
+        nthetas = float("Inf")
+        ncovs = float("Inf")
+        next_expr = None
+        for expr in exprs:
+            symbs = expr.free_symbols
+            curthetas = symbs & all_popparams
+            ncurthetas = len(curthetas)
+            curcovs = symbs & all_covs
+            ncurcovs = len(curcovs)
+            if ncurthetas != 0 and (
+                ncurthetas < nthetas or (ncurthetas == nthetas and ncurcovs < ncovs)
+            ):
+                next_expr = expr
+                thetas = curthetas
+                nthetas = ncurthetas
+                ncovs = ncurcovs
+
+        if next_expr is None:
+            break
+        else:
+            if nthetas == 1 and ncovs == 0:
+                return next(iter(thetas))
+            else:
+                exprs = next_expr.args
+    raise ValueError(f"Could not find theta connected to {paramsymb}")
+
+
 def add_individual_parameter(model: Model, name: str):
     """Add an individual or pk parameter to a model
 
     Parameters
     ----------
     model : Model
         Pharmpy model
@@ -1469,37 +1511,31 @@
             cb.add_flow(peripheral, central, kpc)
         else:
             # Heurstic to handle the Mixed MM-FO case
             if cl.is_Add:
                 cl1 = cl.args[0]
                 if cl1.is_Mul:
                     cl = cl1.args[0]
-            full_cl = statements.before_odes.full_expression(cl)
-            full_vc = statements.before_odes.full_expression(vc)
-            pop_cl_candidates = full_cl.free_symbols & set(model.parameters.symbols)
-            pop_cl = pop_cl_candidates.pop()
-            pop_vc_candidates = full_vc.free_symbols & set(model.parameters.symbols)
-            pop_vc = pop_vc_candidates.pop()
+            pop_cl = _find_noncov_theta(model, cl)
+            pop_vc = _find_noncov_theta(model, vc)
             pop_cl_init = model.parameters[pop_cl].init
             pop_vc_init = model.parameters[pop_vc].init
             qp_init = pop_cl_init
             vp_init = pop_vc_init * 0.05
     elif n == 2:
         per1 = per[0]
         from_rate = odes.get_flow(per1, central)
         assert from_rate is not None
         qp1, vp1 = from_rate.as_numer_denom()
         full_qp1 = statements.before_odes.full_expression(qp1)
         full_vp1 = statements.before_odes.full_expression(vp1)
         if full_vp1 == 1:
             full_qp1, full_vp1 = full_qp1.as_numer_denom()
-        pop_qp1_candidates = full_qp1.free_symbols & set(model.parameters.symbols)
-        pop_qp1 = pop_qp1_candidates.pop()
-        pop_vp1_candidates = full_vp1.free_symbols & set(model.parameters.symbols)
-        pop_vp1 = pop_vp1_candidates.pop()
+        pop_qp1 = _find_noncov_theta(model, full_qp1, full=True)
+        pop_vp1 = _find_noncov_theta(model, full_vp1, full=True)
         pop_qp1_init = model.parameters[pop_qp1].init
         pop_vp1_init = model.parameters[pop_vp1].init
         model = set_initial_estimates(model, {pop_qp1.name: pop_qp1_init * 0.10})
         qp_init = pop_qp1_init * 0.90
         vp_init = pop_vp1_init
 
     if vc != 1:
@@ -1579,52 +1615,36 @@
         if len(peripherals) == 1:
             elimination_rate = odes.get_flow(central, output)
             assert elimination_rate is not None
             cl, vc = elimination_rate.as_numer_denom()
             from_rate = odes.get_flow(last_peripheral, central)
             assert from_rate is not None
             qp1, vp1 = from_rate.as_numer_denom()
-            full_cl = statements.before_odes.full_expression(cl)
-            full_vc = statements.before_odes.full_expression(vc)
-            full_qp1 = statements.before_odes.full_expression(qp1)
-            full_vp1 = statements.before_odes.full_expression(vp1)
-            pop_cl_candidates = full_cl.free_symbols & set(model.parameters.symbols)
-            pop_cl = pop_cl_candidates.pop()
-            pop_vc_candidates = full_vc.free_symbols & set(model.parameters.symbols)
-            pop_vc = pop_vc_candidates.pop()
-            pop_qp1_candidates = full_qp1.free_symbols & set(model.parameters.symbols)
-            pop_qp1 = pop_qp1_candidates.pop()
-            pop_vp1_candidates = full_vp1.free_symbols & set(model.parameters.symbols)
-            pop_vp1 = pop_vp1_candidates.pop()
+            pop_cl = _find_noncov_theta(model, cl)
+            pop_vc = _find_noncov_theta(model, vc)
+            pop_qp1 = _find_noncov_theta(model, qp1)
+            pop_vp1 = _find_noncov_theta(model, vp1)
             pop_vc_init = model.parameters[pop_vc].init
             pop_cl_init = model.parameters[pop_cl].init
             pop_qp1_init = model.parameters[pop_qp1].init
             pop_vp1_init = model.parameters[pop_vp1].init
             new_vc_init = pop_vc_init + pop_qp1_init / pop_cl_init * pop_vp1_init
             model = set_initial_estimates(model, {pop_vc.name: new_vc_init})
         elif len(peripherals) == 2:
             first_peripheral = peripherals[0]
             from1_rate = odes.get_flow(first_peripheral, central)
             assert from1_rate is not None
             qp1, vp1 = from1_rate.as_numer_denom()
             from2_rate = odes.get_flow(last_peripheral, central)
             assert from2_rate is not None
             qp2, vp2 = from2_rate.as_numer_denom()
-            full_qp2 = statements.before_odes.full_expression(qp2)
-            full_vp2 = statements.before_odes.full_expression(vp2)
-            full_qp1 = statements.before_odes.full_expression(qp1)
-            full_vp1 = statements.before_odes.full_expression(vp1)
-            pop_qp2_candidates = full_qp2.free_symbols & set(model.parameters.symbols)
-            pop_qp2 = pop_qp2_candidates.pop()
-            pop_vp2_candidates = full_vp2.free_symbols & set(model.parameters.symbols)
-            pop_vp2 = pop_vp2_candidates.pop()
-            pop_qp1_candidates = full_qp1.free_symbols & set(model.parameters.symbols)
-            pop_qp1 = pop_qp1_candidates.pop()
-            pop_vp1_candidates = full_vp1.free_symbols & set(model.parameters.symbols)
-            pop_vp1 = pop_vp1_candidates.pop()
+            pop_qp2 = _find_noncov_theta(model, qp2)
+            pop_vp2 = _find_noncov_theta(model, vp2)
+            pop_qp1 = _find_noncov_theta(model, qp1)
+            pop_vp1 = _find_noncov_theta(model, vp1)
             pop_qp2_init = model.parameters[pop_qp2].init
             pop_vp2_init = model.parameters[pop_vp2].init
             pop_qp1_init = model.parameters[pop_qp1].init
             pop_vp1_init = model.parameters[pop_vp1].init
             new_qp1_init = (pop_qp1_init + pop_qp2_init) / 2
             new_vp1_init = pop_vp1_init + pop_vp2_init
             model = set_initial_estimates(
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iiv.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iiv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/remove_iov.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iov.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/results.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/tmdd.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/units.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/update_inits.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/update_inits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.95.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/fcon/model.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 
 import pharmpy.config as config
 
-from .model import Model, convert_model, parse_modelfit_results
+from .model import Model, convert_model, execute_model, parse_modelfit_results, verification
 
 r"""
 .. list-table:: Options for the nlmixr plugin
    :widths: 25 25 50 150
    :header-rows: 1
 
    * - Option name
@@ -27,8 +27,8 @@
         'Path to R installation directory',
         cls=pathlib.Path,
     )
 
 
 conf = NLMIXRConfiguration()
 
-__all__ = ('Model', 'convert_model', 'parse_modelfit_results')
+__all__ = ('Model', 'convert_model', 'parse_modelfit_results', 'verification', 'execute_model')
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/error_model.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/error_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,24 @@
         terms = sympy.Add.make_args(self.expr)
         # Assert that it follows the above set of format rules
         assert len(terms) <= 3
 
         errors = []
         for term in terms:
             error_term = False
+            full_term = full_expression(term, self.model)
             for factor in sympy.Mul.make_args(term):
-                full_term = full_expression(factor, self.model)
-                all_symbols = full_term.free_symbols.union(factor.free_symbols)
+                full_factor = full_expression(factor, self.model)
+                all_symbols = full_factor.free_symbols.union(factor.free_symbols)
                 for symbol in all_symbols:
                     if str(symbol) in self.model.random_variables.epsilons.names:
                         sigma = convert_eps_to_sigma(symbol, self.model)
                         if self.model.parameters[str(sigma)].init == 1.0:
                             if self.model.parameters[str(sigma)].fix:
-                                term.subs(factor, 1)
+                                term = term.subs(factor, 1)
                         if factor != symbol:
                             sigma_alias = factor
                         else:
                             sigma_alias = None
                         error_term = True
 
             if error_term:
@@ -79,30 +80,29 @@
             else:
                 if self.res is None:
                     self.res = term
                     self.create_res_alias()
                 else:
                     # FIXME : Should this be allowed??
                     self.res += term
+                    self.create_res_alias()
 
         if self.res is None:
             print("No resulting term found")
             exit
         elif len(errors) > 2:
             print("Too many error terms found")
             exit
 
-        prop = False
-
         for t in errors:
             prop = False
             term = t["term"]
             full_term = t["full_term"]
-            for symbol in full_term.free_symbols:
-                for ali in find_aliases(symbol, self.model).union(term.free_symbols):
+            for symbol in full_term.free_symbols.union(term.free_symbols):
+                for ali in find_aliases(symbol, self.model):
                     if ali in self.res_alias:
                         prop = True
                         # Remove the resulting symbol from the error term
                         term = convert_eps_to_sigma(term, self.model)
                         term = term.subs(ali, 1)
                         self.prop = error(
                             self.model, term, t["sigma"], sigma_alias=t["sigma_alias"], prop=True
@@ -156,18 +156,32 @@
             return False
 
     def check_dependecies(self):
         if self.model is not None and self.expr is not None:
             accepted_symbols = set([self.sigma, self.sigma_alias])
             thetas = get_thetas(self.model).symbols
             accepted_symbols.update(thetas)
+            etas = [sympy.Symbol(i) for i in self.model.random_variables.etas.names]
+            accepted_symbols.update(etas)
             for symbol in self.expr.free_symbols:
-                if symbol not in accepted_symbols:
-                    # TODO : also aid  aliases for all dependencies
-                    self.dependencies.add(symbol)
+                if not any([i in accepted_symbols for i in find_aliases(symbol, self.model)]):
+                    if is_number(symbol, self.model):
+                        accepted_symbols.update([symbol])
+                    else:
+                        self.dependencies.add(symbol)
+
+
+def is_number(symbol: sympy.Expr, model: pharmpy.model.Model) -> bool:
+    alias = find_aliases(symbol, model)
+    for a in alias:
+        if a not in model.random_variables.free_symbols:
+            a_assign = model.statements.find_assignment(a)
+            if a_assign.expression.is_number:
+                return True
+    return False
 
 
 def full_expression(expression: sympy.Expr, model: pharmpy.model.Model) -> sympy.Expr:
     """
     Return the full expression of an expression (used for model statements)
 
     Parameters
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/ini.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/ini.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Parameters
     ----------
     model : pharmpy.model.Model
         Pharmpy model object.
     cg : CodeGenerator
         Code generator to add code upon.
     """
+    cg.add("# --- THETAS ---")
     thetas = [p for p in model.parameters if p.symbol not in model.random_variables.free_symbols]
     for theta in thetas:
         if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
             add_ini_parameter(cg, theta, boundary=True)
         else:
             add_ini_parameter(cg, theta)
 
@@ -33,56 +34,78 @@
     model : pharmpy.model.Model
         Pharmpy model object.
     cg : CodeGenerator
         Code generator to add code upon.
     as_list : bool
         Add with separation character ","
     """
+    cg.add("")
+    cg.add("# --- ETAS ---")
     for dist in model.random_variables.etas:
         omega = dist.variance
         if len(dist.names) == 1:
             init = model.parameters[omega.name].init
             code_line = f'{name_mangle(dist.names[0])} ~ {init}'
             if as_list and dist != model.random_variables.etas[-1]:
                 code_line += ","
             cg.add(code_line)
         else:
+            cg.add(f'{" + ".join([name_mangle(name) for name in dist.names])} ~ c(')
             inits = []
             for row in range(omega.rows):
                 for col in range(row + 1):
-                    inits.append(model.parameters[omega[row, col].name].init)
-            cg.add(
-                f'{" + ".join([name_mangle(name) for name in dist.names])} ~ c({", ".join([str(x) for x in inits])})'
-            )
+                    if col == 0 and row != 0:
+                        cg.add(f'{", ".join([str(x) for x in inits])},')
+                        inits = []
+                        inits.append(f'{model.parameters[omega[row, col].name].init}')
+                    else:
+                        inits.append(model.parameters[omega[row, col].name].init)
+            cg.add(f'{", ".join([str(x) for x in inits])}')
+            if as_list and dist != model.random_variables.etas[-1]:
+                cg.add("),")
+            else:
+                cg.add(")")
 
 
 def add_sigma(model: pharmpy.model.Model, cg: CodeGenerator) -> None:
     """
     Add SIGMAs to code generator when converting a model.
 
     Parameters
     ----------
     model : pharmpy.model.Model
         Pharmpy model object.
     cg : CodeGenerator
         Code generator to add code upon.
     """
+    cg.add("")
+    cg.add("# --- EPSILONS ---")
     for dist in model.random_variables.epsilons:
         sigma = dist.variance
         if len(dist.names) == 1:
             sigma_param = model.parameters[sigma]
-            if sigma_param.init != 1 and not sigma_param.fix:
+            if sigma_param.init != 1:
+                if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
+                    add_ini_parameter(cg, sigma_param, boundary=True)
+                else:
+                    add_ini_parameter(cg, sigma_param)
+            elif not sigma_param.fix:
                 if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
                     add_ini_parameter(cg, sigma_param, boundary=True)
                 else:
                     add_ini_parameter(cg, sigma_param)
         else:
             for row, col in zip(range(sigma.rows), range(sigma.rows + 1)):
                 sigma_param = model.parameters[sigma[row, col]]
-                if sigma_param.init != 1 and not sigma_param.fix:
+                if sigma_param.init != 1:
+                    if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
+                        add_ini_parameter(cg, sigma_param, boundary=True)
+                    else:
+                        add_ini_parameter(cg, sigma_param)
+                elif not sigma_param.fix:
                     if model.estimation_steps[0].method not in ["SAEM", "NLME"]:
                         add_ini_parameter(cg, sigma_param, boundary=True)
                     else:
                         add_ini_parameter(cg, sigma_param)
 
 
 def add_ini_parameter(cg: CodeGenerator, parameter: sympy.Symbol, boundary: bool = False) -> None:
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,20 +23,23 @@
 )
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import fit
 from pharmpy.workflows.log import Log
 
 from .error_model import res_error_term
 from .ini import add_eta, add_sigma, add_theta
-from .model_block import add_ode, add_statements
+from .model_block import add_bioavailability, add_lag_times, add_ode, add_statements
 from .sanity_checks import check_model
 
 
 def convert_model(
-    model: pharmpy.model.Model, keep_etas: bool = False, skip_check: bool = False
+    model: pharmpy.model.Model,
+    keep_etas: bool = False,
+    skip_check: bool = False,
+    updated_estimates: bool = False,
 ) -> pharmpy.model.Model:
     """
     Convert a NONMEM model into an nlmixr model
 
     Parameters
     ----------
     model : pharmpy.model.Model
@@ -52,14 +55,17 @@
         A model converted to nlmixr format.
 
     """
 
     if isinstance(model, Model):
         return model
 
+    if updated_estimates:
+        model = update_inits(model, model.modelfit_results.parameter_estimates)
+
     nlmixr_model = Model(
         internals=NLMIXRModelInternals(),
         parameters=model.parameters,
         random_variables=model.random_variables,
         statements=model.statements,
         dependent_variables=model.dependent_variables,
         estimation_steps=model.estimation_steps,
@@ -74,14 +80,16 @@
     if model.dataset is not None:
         if keep_etas is True:
             nlmixr_model = nlmixr_model.replace(
                 modelfit_results=ModelfitResults(
                     individual_estimates=model.modelfit_results.individual_estimates
                 )
             )
+            nlmixr_model = fixate_eta(nlmixr_model)
+
         nlmixr_model = translate_nmtran_time(nlmixr_model)
         # FIXME: dropping columns runs update source which becomes redundant.
         # drop_dropped_columns(nlmixr_model)
         if all(x in nlmixr_model.dataset.columns for x in ["RATE", "DUR"]):
             nlmixr_model = drop_columns(nlmixr_model, ["DUR"])
         nlmixr_model = nlmixr_model.replace(
             datainfo=nlmixr_model.datainfo.replace(path=None),
@@ -162,16 +170,19 @@
 
     # Add statements before ODEs
     cg.indent()
     if len(model.statements.after_odes) != 0:
         add_statements(model, cg, model.statements.before_odes)
 
     # Add the ODEs
+    cg.add("")
+    cg.add("# --- DIFF EQUATIONS ---")
     if model.statements.ode_system:
         add_ode(model, cg)
+    cg.add("")
 
     # Find what kind of error model we are looking at
     dv = list(model.dependent_variables.keys())[0]
     dv_statement = model.statements.find_assignment(dv)
 
     only_piecewise = False
     if dv_statement.expression.is_Piecewise:
@@ -196,14 +207,19 @@
                     res_alias.update(dv_term.res_alias)
     else:
         dv_term = res_error_term(model, dv_statement.expression)
         dependencies = dv_term.dependencies()
         dv_term.create_res_alias()
         res_alias = dv_term.res_alias
 
+    # Add bioavailability statements
+    if model.statements.ode_system is not None:
+        add_bioavailability(model, cg)
+        add_lag_times(model, cg)
+
     # Add statements after ODEs
     if len(model.statements.after_odes) == 0:
         statements = model.statements
     else:
         statements = model.statements.after_odes
     add_statements(
         model, cg, statements, only_piecewise, dependencies=dependencies, res_alias=res_alias
@@ -295,17 +311,14 @@
         cg.empty_line()
         create_fit(cg, self)
         # Create lowercase id, time and amount symbols for nlmixr to be able
         # to run
         self.internals.src = str(cg).replace("AMT", "amt").replace("TIME", "time")
         self.internals.path = None
         code = str(cg).replace("AMT", "amt").replace("TIME", "time")
-        # Replace all instances of EPS with sigma instead
-        for eps in self.random_variables.epsilons:
-            code = code.replace(eps.names[0], eps.variance.name)
         internals = replace(self.internals, src=code)
         model = self.replace(internals=internals)
         return model
 
     @property
     def model_code(self):
         model = self.update_source()
@@ -368,15 +381,15 @@
     pe = {}
     for param in model.parameters:
         if param.fix:
             continue
         elif param.name in omegas_sigmas:
             pe[param.name] = omegas_sigmas[param.name]
         else:
-            pe[param.name] = rdata['thetas']['fit$theta'][thetas_index]
+            pe[param.name] = rdata['thetas']['fit$theta'][param.name]
             thetas_index += 1
 
     name = model.name
     description = model.description
     pe = pd.Series(pe)
     predictions = rdata['pred'].set_index(["ID", "TIME"])
     predictions.index = predictions.index.set_levels(
@@ -391,15 +404,15 @@
         parameter_estimates=pe,
         predictions=predictions,
         log=Log(),
     )
     return res
 
 
-def execute_model(model: pharmpy.model.Model, db: str) -> pharmpy.model.Model:
+def execute_model(model: pharmpy.model.Model, db: str, evaluate=False) -> pharmpy.model.Model:
     """
     Executes a model using nlmixr2 estimation.
 
     Parameters
     ----------
     model : pharmpy.model.Model
         An pharmpy model object.
@@ -408,21 +421,27 @@
 
     Returns
     -------
     model : pharmpy.model.Model
         Model with accompanied results.
 
     """
+    if evaluate:
+        if [s.evaluation for s in model.estimation_steps._steps][0] is False:
+            model = set_evaluation_step(model)
+
     db = pharmpy.workflows.LocalDirectoryToolDatabase(db)
     database = db.model_database
     model = convert_model(model)
     path = Path.cwd() / f'nlmixr_run_{model.name}-{uuid.uuid1()}'
     model.internals.path = path
     meta = path / '.pharmpy'
     meta.mkdir(parents=True, exist_ok=True)
+    if model.datainfo.path is not None:
+        model = model.replace(datainfo=model.datainfo.replace(path=None))
     write_csv(model, path=path)
     model = model.replace(datainfo=model.datainfo.replace(path=path))
 
     dataname = f'{model.name}.csv'
     pre = f'library(nlmixr2)\n\ndataset <- read.csv("{path / dataname}")\n'
 
     if "fix_eta" in model.estimation_steps[0].tool_options:
@@ -509,161 +528,249 @@
 
 def verification(
     model: pharmpy.model.Model,
     db_name: str,
     error: float = 10**-3,
     return_comp: bool = False,
     fix_eta: bool = True,
-    ipred_diff: bool = False,
+    force_ipred: bool = False,
+    force_pred: bool = False,
+    ignore_print=False,
 ) -> Union[bool, pd.DataFrame]:
     """
     Verify that a model inputet in NONMEM format can be correctly translated to
     nlmixr as well as verify that the predictions of the two models are the same
     given a user specified error margin (defailt is 0.001).
 
     Comparison will be done on PRED values as default unless only IPRED values
-    are present or if ipred_diff is set to True.
+    are present or if force_ipred is set to True. Can also force to use pred values
+    which will cause an error if only ipred values are present.
 
     Parameters
     ----------
     model : pharmpy.model.Model
         pharmpy Model object in NONMEM format.
     db_name : str
         a string with given name of database folder for created files.
     error : float, optional
         Allowed error margins for predictions. The default is 10**-3.
     return_comp : bool, optional
         Choose to return table of predictions. The default is False.
     fix_eta : bool, optional
         Decide if NONMEM estimated ETAs are to be used. The default is True.
-    ipred_diff : bool, optional
+    force_ipred : bool, optional
         Force to use IPRED for calculating differences instead of PRED. The default is False.
+    force_pred : bool, optional
+        Force to use PRED for calculating differences. The default is False.
 
     Returns
     -------
     Union[bool, pd.Dataframe]
         If return_comp = True, return a table of comparisons and differences in
         predictions instead of a boolean indicating if they are the same or not
 
     """
 
     nonmem_model = model
 
     # Save results from the nonmem model
     if nonmem_model.modelfit_results is None:
-        print_step("Calculating NONMEM predictions... (this might take a while)")
+        if not ignore_print:
+            print_step("Calculating NONMEM predictions... (this might take a while)")
         nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-        nonmem_results = nonmem_model.modelfit_results.predictions.copy()
     else:
         if nonmem_model.modelfit_results.predictions is None:
-            print_step("Calculating NONMEM predictions... (this might take a while)")
+            if not ignore_print:
+                print_step("Calculating NONMEM predictions... (this might take a while)")
             nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-            nonmem_results = nonmem_model.modelfit_results.predictions.copy()
-        else:
-            nonmem_results = nonmem_model.modelfit_results.predictions.copy()
 
     # Set a tool option to fix theta values when running nlmixr
     if fix_eta:
         nonmem_model = fixate_eta(nonmem_model)
 
     # Check that evaluation step is set to True
     if [s.evaluation for s in nonmem_model.estimation_steps._steps][0] is False:
         nonmem_model = set_evaluation_step(nonmem_model)
 
     # Update the nonmem model with new estimates
     # and convert to nlmixr
-    print_step("Converting NONMEM model to nlmixr2...")
+    if not ignore_print:
+        print_step("Converting NONMEM model to nlmixr2...")
     if fix_eta is True:
         nlmixr_model = convert_model(
             update_inits(nonmem_model, nonmem_model.modelfit_results.parameter_estimates),
             keep_etas=True,
         )
     else:
         nlmixr_model = convert_model(
             update_inits(nonmem_model, nonmem_model.modelfit_results.parameter_estimates)
         )
 
     # Execute the nlmixr model
-    print_step("Executing nlmixr2 model... (this might take a while)")
+    if not ignore_print:
+        print_step("Executing nlmixr2 model... (this might take a while)")
 
     nlmixr_model = execute_model(nlmixr_model, db_name)
-    nlmixr_results = nlmixr_model.modelfit_results.predictions
+
+    # Combine the two based on ID and time
+    if not ignore_print:
+        print_step("Creating result comparison table...")
+    combined_result = compare_models(
+        nonmem_model,
+        nlmixr_model,
+        error=error,
+        force_ipred=force_ipred,
+        force_pred=force_pred,
+        ignore_print=ignore_print,
+    )
+
+    if not ignore_print:
+        print_step("DONE")
+    if return_comp is True:
+        return combined_result
+    else:
+        if all(combined_result["PASS/FAIL"] == "PASS"):
+            return True
+        else:
+            return False
+
+
+def compare_models(
+    model_1, model_2, error=10**-3, force_ipred=False, force_pred=False, ignore_print=False
+):
+    assert model_1.modelfit_results.predictions is not None
+    assert model_2.modelfit_results.predictions is not None
+
+    mod1 = model_1
+    mod1_type = str(type(mod1)).split(".")[2]
+    mod2 = model_2
+    mod2_type = str(type(mod2)).split(".")[2]
+
+    nm_to_r = False
+    if (
+        mod1_type == "nonmem"
+        and mod2_type != "nonmem"
+        or mod2_type == "nonmem"
+        and mod1_type != "nonmem"
+    ):
+        nm_to_r = True
+
+    mod1 = mod1.replace(dataset=mod1.dataset.reset_index())
+    mod2 = mod2.replace(dataset=mod2.dataset.reset_index())
+
+    for mod in [mod1, mod2]:
+        if "EVID" not in mod.dataset.columns:
+            mod = add_evid(mod)
+
+    if nm_to_r:
+        if mod1_type == "nonmem":
+            predictions = mod1.modelfit_results.predictions.reset_index()
+            predictions = predictions.drop(
+                mod1.dataset[~mod1.dataset["EVID"].isin([0, 2])].index.to_list()
+            )
+            predictions = predictions.set_index(["ID", "TIME"])
+            mod1 = mod1.replace(modelfit_results=ModelfitResults(predictions=predictions))
+        if mod2_type == "nonmem":
+            predictions = mod2.modelfit_results.predictions.reset_index()
+            predictions = predictions.drop(
+                mod2.dataset[~mod2.dataset["EVID"].isin([0, 2])].index.to_list()
+            )
+            predictions = predictions.set_index(["ID", "TIME"])
+            mod2 = mod2.replace(modelfit_results=ModelfitResults(predictions=predictions))
+
+    mod1_results = mod1.modelfit_results.predictions.copy()
+
+    mod2_results = mod2.modelfit_results.predictions.copy()
 
     pred = False
     ipred = False
-    for p in nonmem_model.modelfit_results.predictions.columns:
-        if p == "PRED":
+    # ---
+    if force_pred:
+        if "PRED" in mod1_results.columns:
             pred = True
-            nonmem_results.rename(columns={p: 'PRED_NONMEM'}, inplace=True)
-            nlmixr_results.rename(columns={p: 'PRED_NLMIXR'}, inplace=True)
-        elif p == "IPRED" or p == "CIPREDI":
+            p = "PRED"
+            assert p in mod2_results.columns
+            mod1_results.rename(columns={p: f'PRED_{mod1_type}'}, inplace=True)
+            mod2_results.rename(columns={p: f'PRED_{mod2_type}'}, inplace=True)
+    elif force_ipred:
+        if "IPRED" in mod1_results.columns:
+            p = "IPRED"
             ipred = True
-            nonmem_results.rename(columns={p: 'IPRED_NONMEM'}, inplace=True)
-            if p == "CIPREDI":
-                p = "IPRED"
-            nlmixr_results.rename(columns={p: 'IPRED_NLMIXR'}, inplace=True)
-        else:
-            print(
-                f"Unknown prediction value {p}. Currently only 'PRED' and 'IPRED' are supported and this is ignored"
-            )
+            assert p in mod2_results.columns
+            mod1_results.rename(columns={p: f'{p}_{mod1_type}'}, inplace=True)
+            mod2_results.rename(columns={p: f'IPRED_{mod2_type}'}, inplace=True)
+        elif "CIPREDI" in mod1_results.columns:
+            p = "CIPREDI"
+            ipred = True
+            assert p in mod2_results.columns
+            mod1_results.rename(columns={p: f'{p}_{mod1_type}'}, inplace=True)
+            mod2_results.rename(columns={p: f'IPRED_{mod2_type}'}, inplace=True)
+    else:
+        for p in mod1_results.columns:
+            if p == "PRED":
+                pred = True
+                assert p in mod2_results.columns
+                mod1_results.rename(columns={p: f'PRED_{mod1_type}'}, inplace=True)
+                mod2_results.rename(columns={p: f'PRED_{mod2_type}'}, inplace=True)
+            elif (p == "IPRED" or p == "CIPREDI") and "PRED" not in mod1_results.columns:
+                ipred = True
+                assert "IPRED" in mod2_results.columns or "CIPREDI" in mod2_results.columns
+                mod1_results.rename(columns={p: f'{p}_{mod1_type}'}, inplace=True)
+                if "IPRED" in mod2_results.columns:
+                    mod2_results.rename(columns={p: f'IPRED_{mod2_type}'}, inplace=True)
+                else:
+                    mod2_results.rename(columns={p: f'CIPREDI_{mod2_type}'}, inplace=True)
+    # ---
 
     if not (pred or ipred):
-        print("No known prediction value was found. Please use 'PRED' or 'IPRED")
+        print("No comparable prediction value was found. Please use 'PRED' or 'IPRED")
         return False
 
-    # Combine the two based on ID and time
-    print_step("Creating result comparison table...")
-    nonmem_model = nonmem_model.replace(dataset=nonmem_model.dataset.reset_index())
-
-    if "EVID" not in nonmem_model.dataset.columns:
-        nonmem_model = add_evid(nonmem_model)
-    nonmem_results = nonmem_results.reset_index()
-    nonmem_results = nonmem_results.drop(
-        nonmem_model.dataset[nonmem_model.dataset["EVID"] != 0].index.to_list()
-    )
-    nonmem_results = nonmem_results.set_index(["ID", "TIME"])
-
-    combined_result = nonmem_results
+    combined_result = mod1_results
     if pred:
-        combined_result['PRED_NLMIXR'] = nlmixr_results['PRED_NLMIXR'].to_list()
+        combined_result[f'PRED_{mod2_type}'] = mod2_results[f'PRED_{mod2_type}'].to_list()
         # Add difference between the models
         combined_result['PRED_DIFF'] = abs(
-            combined_result['PRED_NONMEM'] - combined_result['PRED_NLMIXR']
+            combined_result[f'PRED_{mod1_type}'] - combined_result[f'PRED_{mod2_type}']
         )
     if ipred:
-        combined_result['IPRED_NLMIXR'] = nlmixr_results['IPRED_NLMIXR'].to_list()
+        combined_result[f'IPRED_{mod2_type}'] = mod2_results[f'IPRED_{mod2_type}'].to_list()
         combined_result['IPRED_DIFF'] = abs(
-            combined_result['IPRED_NONMEM'] - combined_result['IPRED_NLMIXR']
+            combined_result[f'IPRED_{mod1_type}'] - combined_result[f'IPRED_{mod2_type}']
         )
 
     combined_result["PASS/FAIL"] = "PASS"
-    print("Differences in population predicted values")
+    if not ignore_print:
+        print("Differences in population predicted values")
     if (pred and ipred) or (pred and not ipred):
-        if ipred_diff:
-            print("Using PRED values for final comparison")
+        if force_ipred:
+            if not ignore_print:
+                print("Using IPRED values for final comparison")
             final = "IPRED"
         else:
-            print("Using PRED values for final comparison")
+            if not ignore_print:
+                print("Using PRED values for final comparison")
             final = "PRED"
     elif ipred and not pred:
-        print("Using IPRED values for final comparison")
+        if force_ipred:
+            if not ignore_print:
+                print("Using IPRED values for final comparison")
+        else:
+            if not ignore_print:
+                print("Using IPRED values instead")
         final = "IPRED"
+
     combined_result.loc[combined_result[f'{final}_DIFF'] > error, "PASS/FAIL"] = "FAIL"
-    print(
-        combined_result[f'{final}_DIFF'].describe()[["mean", "75%", "max"]].to_string(), end="\n\n"
-    )
+    if not ignore_print:
+        print(
+            combined_result[f'{final}_DIFF'].describe()[["mean", "75%", "max"]].to_string(),
+            end="\n\n",
+        )
 
-    print_step("DONE")
-    if return_comp is True:
-        return combined_result
-    else:
-        if all(combined_result["PASS/FAIL"] == "PASS"):
-            return True
-        else:
-            return False
+    return combined_result
 
 
 def print_step(s: str) -> None:
     """
     Print step currently being performed. Used during verification
 
     Parameters
@@ -736,7 +843,43 @@
     path = path / filename
     if not force and path.exists():
         raise FileExistsError(f'File at {path} already exists.')
 
     path = path_absolute(path)
     model.modelfit_results.individual_estimates.to_csv(path, na_rep=data.conf.na_rep, index=False)
     return path
+
+
+def verify_param(model1, model2, est=False):
+    tol = 0.01
+
+    if est:
+        param1 = model1.modelfit_results.parameter_estimates
+        param2 = model2.modelfit_results.parameter_estimates
+
+        passed = []
+        failed = []
+        for p1 in param1.index:
+            if p1 in param2.index:
+                p1_value = param1[p1]
+                p2_value = param2[p1]
+                diff = p1_value - p2_value
+                if abs(diff) > tol:
+                    failed.append((p1, diff))
+                else:
+                    passed.append((p1, diff))
+
+    else:
+        param1 = model1.parameters
+        param2 = model2.parameters
+
+        passed = []
+        failed = []
+        for p1 in param1:
+            if p1.name in param2.names:
+                p2 = param2[p1.name]
+                diff = p1.init - p2.init
+                if abs(diff) > tol:
+                    failed.append((p1.name, diff))
+                else:
+                    passed.append((p1.name, diff))
+    return passed, failed
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/model_block.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from typing import Set, Union
 
 import pharmpy.model
 from pharmpy.deps import sympy, sympy_printing
 from pharmpy.internals.code_generator import CodeGenerator
 from pharmpy.model import Assignment
+from pharmpy.modeling import get_bioavailability, get_lag_times
 
 from .error_model import res_error_term
 from .name_mangle import name_mangle
 
 
 class ExpressionPrinter(sympy_printing.str.StrPrinter):
     def __init__(self, amounts):
@@ -82,31 +83,29 @@
                         cg.add(f'{s.symbol} <- {res}')
                         cg.add(f'{s.symbol} ~ add(add_error) + prop(prop_error)')
 
                         # TODO: Remove sigma here instead of in ini
                         # also remove aliases
 
                     else:
-                        cg.add(f'{s.symbol} <- {res}')
-                        e = ""
-                        first = True
-                        if dv_term.add.expr != 0:
-                            e += f'add({dv_term.add.expr})'
-                            first = False
-                        if dv_term.prop.expr != 0:
-                            if not first:
-                                e += " + "
-                            e += f'prop({dv_term.prop.expr})'
-                        cg.add(f'{s.symbol} ~ {e}')
+                        cg.add(f"{s.symbol} <- {res}")
+                        cg.add(f'add_error <- {dv_term.add.expr}')
+                        cg.add(f'prop_error <- {dv_term.prop.expr}')
+                        cg.add(f'{s.symbol} ~ add(add_error) + prop(prop_error)')
                 else:
                     dv_term = res_error_term(model, s.expression)
                     cg.add(f"res <- {dv_term.res}")
                     cg.add(f'add_error <- {dv_term.add.expr}')
                     cg.add(f'prop_error <- {dv_term.prop.expr}')
 
+            elif model.statements.ode_system is not None and (
+                s.symbol in get_bioavailability(model).values()
+                or s.symbol in get_lag_times(model).values()
+            ):
+                pass
             else:
                 expr = s.expression
                 if expr.is_Piecewise:
                     first = True
                     for value, cond in expr.args:
                         if cond is not sympy.S.true:
                             cond = convert_eq(cond)
@@ -193,34 +192,65 @@
             The symbol representing  the proportional error. Zero if none found
 
     """
     if isinstance(s, sympy.Symbol):
         terms = [s]
     elif isinstance(s, sympy.Pow):
         terms = sympy.Add.make_args(s.args[0])
+    elif isinstance(s, sympy.Mul):
+        terms = [s]
+    elif isinstance(s, sympy.Integer):
+        terms = [s]
+    elif isinstance(s, sympy.Float):
+        terms = [s]
     else:
         terms = sympy.Add.make_args(s.expression)
     assert len(terms) <= 2
 
+    r = r"sqrt\([a-zA-Z0-9_.-]*\*\*2\*[a-zA-Z0-9_.-]*\*\*2 \+ [a-zA-Z0-9_.-]*\*\*2\)"
+    if re.match(r, str(s)):
+        w = True
+    else:
+        w = False
+
     prop = 0
     add = 0
     prop_found = False
     for term in terms:
         for symbol in term.free_symbols:
             if symbol in res_alias:
                 if prop_found is False:
                     term = term.subs(symbol, 1)
-                    prop = list(term.free_symbols)[0]
+                    if w:
+                        prop = list(term.free_symbols)[0]
+                    else:
+                        add = term
                     prop_found = True
         if prop_found is False:
-            add = list(term.free_symbols)[0]
-
+            if w:
+                add = list(term.free_symbols)[0]
+            else:
+                add = term
     return add, prop
 
 
+def add_bioavailability(model: pharmpy.model.Model, cg: CodeGenerator):
+    bio = get_bioavailability(model)
+    for comp, symbol in bio.items():
+        symbol_value = model.statements.find_assignment(symbol).expression
+        cg.add(f'f(A_{comp}) <- {symbol_value}')
+
+
+def add_lag_times(model: pharmpy.model.Model, cg: CodeGenerator):
+    lag = get_lag_times(model)
+    for comp, symbol in lag.items():
+        symbol_value = model.statements.find_assignment(symbol).expression
+        cg.add(f'alag(A_{comp}) <- {symbol_value}')
+
+
 def add_piecewise(model: pharmpy.model.Model, cg: CodeGenerator, s):
     expr = s.expression
     first = True
     for value, cond in expr.args:
         if cond is not sympy.S.true:
             if cond.atoms(sympy.Eq):
                 cond = convert_eq(cond)
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nlmixr/sanity_checks.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/advan.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/advan.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,24 +293,25 @@
 
         sset = des.statements.subs(subs_dict)
 
         eqs = [sympy.Eq(s.symbol, s.expression) for s in sset if not s.symbol.is_Symbol]
 
         cs = to_compartmental_system(func_to_name, eqs)
         cb = CompartmentalSystemBuilder(cs)
-
         for i, comp_name in enumerate(comps, start=1):
             comp = cs.find_compartment(comp_name)
             if comp is None:  # Compartments can be in $MODEL but not used in $DES
                 continue
             if i == 1:
                 dose = dosing(di, dataset, 1)  # FIXME: Only one dose to 1st compartment
                 cb.set_dose(comp, dose)
+                comp = cb.find_compartment(comp_name)
             f = _get_bioavailability(control_stream, i)
             cb.set_bioavailability(comp, f)
+            comp = cb.find_compartment(comp_name)
             alag = _get_alag(control_stream, i)
             cb.set_lag_time(comp, alag)
 
         # Search for DEFOBSERVATION, default to first
         it = iter(rec_model.compartments())
         defobs = (next(it)[0], 1)
         for i, (name, opts) in enumerate(it, start=2):
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/config.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/dataset.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/model.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     parse_value_type,
 )
 from .results import _parse_modelfit_results
 from .update import (
     abbr_translation,
     create_name_map,
     update_ccontra,
-    update_dependent_variables,
     update_description,
     update_estimation,
     update_initial_individual_estimates,
     update_input,
     update_name_of_tables,
     update_random_variables,
     update_sizes,
@@ -196,15 +195,15 @@
             model, abbr_map = abbr_translation(model, rv_trans)
             trans = {key: value for key, value in trans.items() if key not in abbr_map.values()}
 
         trans = {sympy.Symbol(key): sympy.Symbol(value) for key, value in trans.items()}
         model, updated_dataset = update_statements(
             model, model.internals.old_statements, model._statements, trans
         )
-        model = update_dependent_variables(model, trans)
+        # model = update_dependent_variables(model, trans)
 
         cs = model.internals.control_stream
 
         if model.dataset is None:
             pass
         elif (
             updated_dataset
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/nmtran_parser.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/parsing.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/parsing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/code_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/code_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/data_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/factory.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/model_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/omega_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/omega_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import math
 import re
-import warnings
 from typing import cast
 
 from pharmpy.deps import numpy as np
 from pharmpy.internals.math import flattened_to_symmetric, triangular_root
 from pharmpy.internals.parse import AttrToken, AttrTree
 from pharmpy.internals.parse.generic import (
     eval_token,
@@ -98,29 +97,14 @@
                         label_index += 1
                 block = (names, inits, fix, False)
             else:
                 block = (None, None, None, True)
             blocks.append(block)
         return blocks
 
-    def _find_label(self, node, seen_labels):
-        """Find label from comment of omega parameter"""
-        # needed to avoid circular import with Python 3.6
-        import pharmpy.plugins.nonmem as nonmem
-
-        name = None
-        if 'comment' in nonmem.conf.parameter_names:
-            name = self._get_name(node)
-            if name in seen_labels:
-                warnings.warn(
-                    f'The parameter name {name} is duplicated. Falling back to basic NONMEM names.'
-                )
-                name = None
-        return name
-
     def _get_name(self, node):
         name = None
         found = False
         for subnode in self.root.tree_walk():
             if id(subnode) == id(node):
                 found = True
                 continue
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/option_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/parsers.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/problem_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/sizes_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/table_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/table_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/records/theta_record.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,27 +466,47 @@
         n = len(df)
         step += [i] * n
         iteration += list(df['ITERATION'])
         ofv += list(df['OBJ'])
         final_table = table
 
     assert isinstance(final_table, ExtTable)
-    final_ofv = final_table.final_ofv
+    if np.isnan(ofv[-1]):
+        final_ofv = ofv[-1]
+    else:
+        final_ofv = final_table.final_ofv
     ofv_iterations = create_ofv_iterations_series(ofv, step, iteration)
     return final_ofv, ofv_iterations
 
 
 def _get_iter_df(df):
     final_iter = -(10**9)
     iters = df['ITERATION']
     if 0 not in iters.values and final_iter in iters.values:
         df = df[iters == -(10**9)]
         df.at[0, 'ITERATION'] = 0
     else:
-        df = df[iters >= 0]
+        try:
+            final_iter_ofv = df[iters == final_iter].iloc[-1].loc['OBJ']
+        except IndexError:
+            final_iter_ofv = np.nan
+        last_iter_ofv = df[iters >= 0].iloc[-1].loc['OBJ']
+        if final_iter_ofv != last_iter_ofv:
+            new_iter_no = int(df[iters >= 0].iloc[-1].loc['ITERATION']) + 1
+            if final_iter in iters.values:
+                idx = df[iters == final_iter].index.values[0]
+                df.at[idx, 'ITERATION'] = new_iter_no
+                new_iter_no += 1
+            nan_row_dict = {
+                colname: (new_iter_no if colname == 'ITERATION' else np.nan)
+                for colname in df.columns
+            }
+            nan_row = pd.DataFrame(nan_row_dict, index=[len(df)])
+            df = pd.concat([df, nan_row])
+        df = df[df['ITERATION'] >= 0]
     return df
 
 
 def _calculate_relative_standard_errors(pe, se):
     if pe is None or se is None:
         ser = None
     else:
@@ -517,17 +537,20 @@
         df['step'] = i
         df = df.rename(columns=name_map)
         pe = pd.concat([pe, df])
         final_table = table
 
     assert fix is not None
     assert final_table is not None
-    final = final_table.final_parameter_estimates
-    final = final.drop(fixed_param_names)
-    final = final.rename(index=name_map)
+    if pe.iloc[-1].drop(['ITERATION', 'step']).isnull().all():
+        final = pe.iloc[-1].drop(['ITERATION', 'step']).rename('estimates')
+    else:
+        final = final_table.final_parameter_estimates
+        final = final.drop(fixed_param_names)
+        final = final.rename(index=name_map)
     pe = pe.rename(columns={'ITERATION': 'iteration'}).set_index(['step', 'iteration'])
 
     try:
         sdcorr = final_table.omega_sigma_stdcorr[~fix]
     except KeyError:
         sdcorr_ests = pd.Series(np.nan, index=pe.index)
     else:
@@ -585,35 +608,35 @@
     results = []
     for i in range(1, nsubs + 1):
         res = parse_modelfit_results(model, model_path, subproblem=i)
         results.append(res)
     return results
 
 
-def parse_ext(model, path, subproblem):
-    try:
-        ext_tables = NONMEMTableFile(path.with_suffix('.ext'))
-    except ValueError:
-        failed_pe = _create_failed_parameter_estimates(model.parameters)
-        n = len(model.estimation_steps)
-        df = pd.concat([failed_pe] * n, axis=1).T
-        df['step'] = range(1, n + 1)
-        df['iteration'] = 0
-        df = df.set_index(['step', 'iteration'])
-        return (
-            [],
-            np.nan,
-            _create_failed_ofv_iterations(len(model.estimation_steps)),
-            failed_pe,
-            failed_pe,
-            df,
-            None,
-            None,
-        )
-    return _parse_ext(model.internals.control_stream, ext_tables, subproblem, model.parameters)
+# def parse_ext(model, path, subproblem):
+#     try:
+#         ext_tables = NONMEMTableFile(path.with_suffix('.ext'))
+#     except ValueError:
+#         failed_pe = _create_failed_parameter_estimates(model.parameters)
+#         n = len(model.estimation_steps)
+#         df = pd.concat([failed_pe] * n, axis=1).T
+#         df['step'] = range(1, n + 1)
+#         df['iteration'] = 0
+#         df = df.set_index(['step', 'iteration'])
+#         return (
+#             [],
+#             np.nan,
+#             _create_failed_ofv_iterations(len(model.estimation_steps)),
+#             failed_pe,
+#             failed_pe,
+#             df,
+#             None,
+#             None,
+#         )
+#     return _parse_ext(model.internals.control_stream, ext_tables, subproblem, model.parameters)
 
 
 def parse_modelfit_results(
     model, path: Optional[Union[str, Path]], subproblem: Optional[int] = None
 ):
     name_map = create_name_map(model)
     name_map = {value: key for key, value in name_map.items()}
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/results_file.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/run.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/table.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/nonmem/update.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,38 +550,41 @@
             return Statements(new)
 
     return statements
 
 
 def update_statements(model: Model, old: Statements, new: Statements, trans):
     trans['NaN'] = int(data.conf.na_rep)
-    main_statements = Statements()
-    error_statements = Statements()
 
     new_odes = new.ode_system
     updated_dataset = False
+
+    old_solver, new_solver = None, None
+    if len(model.estimation_steps) > 0:
+        new_solver = model.estimation_steps[0].solver
+    if len(model.internals.old_estimation_steps) > 0:
+        old_solver = model.internals.old_estimation_steps[0].solver
+
+    if old == new and old_solver == new_solver:
+        return model, updated_dataset
+
     if new_odes is not None:
         old_odes = old.ode_system
         if new_odes != old_odes:
             colnames, drop, _, _ = parse_column_info(model.internals.control_stream)
             col_dropped = dict(zip(colnames, drop))
             if 'CMT' in col_dropped.keys() and not col_dropped['CMT']:
                 warnings.warn(
                     'Compartment structure has been updated, CMT-column '
                     'in dataset might not be relevant anymore. Check '
                     'CMT-column or drop column'
                 )
             model, updated_dataset = update_ode_system(model, old_odes, new_odes)
         else:
-            if len(model.estimation_steps) > 0:
-                new_solver = model.estimation_steps[0].solver
-            else:
-                new_solver = None
             if new_solver:
-                old_solver = model.internals.old_estimation_steps[0].solver
                 if new_solver != old_solver:
                     advan = solver_to_advan(new_solver)
                     subs = model.internals.control_stream.get_records('SUBROUTINES')[0]
                     newsubs = subs.set_advan(advan)
                     newcs = model.internals.control_stream.replace_records([subs], [newsubs])
                     model = model.replace(internals=model.internals.replace(control_stream=newcs))
                     model = update_model_record(model, advan)
@@ -616,14 +619,16 @@
         new_error = new_error.update_extra_nodes(model.dependent_variables)
         newcs = model.internals.control_stream.replace_records([error], [new_error])
         model = model.replace(internals=model.internals.replace(control_stream=newcs))
     return model, updated_dataset
 
 
 def update_dependent_variables(model: Model, trans):
+    # FIXME: This is currently not used.
+    # Does it conflict with code_record.update_extra_nodes ?
     old_dvs = model.internals.old_dependent_variables
     new_dvs = model.dependent_variables
     if old_dvs != new_dvs:
         # Will replace AST nodes (representing plain assignments) for all dvs
         # with new block IF structure. All statements are kept
         # FIXME: Assumes DVs added from 1
         # FIXME: Assumes DVID colname
@@ -903,14 +908,18 @@
     if len(odes) != 2:
         return False
     dosing = odes.dosing_compartment
     outflows = odes.get_compartment_outflows(dosing)
     if len(outflows) != 1:
         return False
     central = outflows[0][0]
+    central_rate = outflows[0][1]
+    if {sympy.Symbol('CL'), sympy.Symbol('V')} & central_rate.free_symbols:
+        # Cannot use reserved symbols
+        return False
     central_outflows = odes.get_compartment_outflows(central)
     if len(central_outflows) != 1:
         return False
     return True
 
 
 def match_advan3(odes):
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 
 import pharmpy.config as config
 
-# from .model import Model, convert_model, parse_modelfit_results
+from .model import Model, convert_model, execute_model, parse_modelfit_results, verification
 
 r"""
 .. list-table:: Options for the nlmixr plugin
    :widths: 25 25 50 150
    :header-rows: 1
 
    * - Option name
@@ -17,18 +17,18 @@
      - ````
      - str
      - Path to R installation directory
 """
 
 
 class RxODEConfiguration(config.Configuration):
-    module = 'pharmpy.plugins.nlmixr'
+    module = 'pharmpy.plugins.rxode'
     rpath = config.ConfigItem(
         pathlib.Path(''),
         'Path to R installation directory',
         cls=pathlib.Path,
     )
 
 
 conf = RxODEConfiguration()
 
-# __all__ = ('Model', 'convert_model', 'parse_modelfit_results')
+__all__ = ('Model', 'convert_model', 'parse_modelfit_results', 'verification', 'execute_model')
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/rxode/model.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,31 +9,37 @@
 
 import pharmpy.model
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.code_generator import CodeGenerator
 from pharmpy.modeling import (
     drop_columns,
+    get_bioavailability,
+    get_lag_times,
     get_omegas,
     get_sigmas,
     get_thetas,
     translate_nmtran_time,
     write_csv,
 )
 from pharmpy.plugins.nlmixr.error_model import convert_eps_to_sigma
 from pharmpy.plugins.nlmixr.model import add_evid
-from pharmpy.plugins.nlmixr.model_block import add_ode, convert_eq
+from pharmpy.plugins.nlmixr.model_block import (
+    add_bioavailability,
+    add_lag_times,
+    add_ode,
+    convert_eq,
+)
 from pharmpy.results import ModelfitResults
 
 
 @dataclass
 class RxODEModelInternals:
     src: Optional[str] = None
     path: Optional[Path] = None
-    DES: Optional = None
 
 
 class Model(pharmpy.model.Model):
     def __init__(self, **kwargs):
         super().__init__(
             **kwargs,
         )
@@ -88,14 +94,16 @@
     db = pharmpy.workflows.LocalDirectoryToolDatabase(db)
     database = db.model_database
     model = convert_model(model)
     path = Path.cwd() / f'rxode_run_{model.name}-{uuid.uuid1()}'
     model.internals.path = path
     meta = path / '.pharmpy'
     meta.mkdir(parents=True, exist_ok=True)
+    if model.datainfo.path is not None:
+        model = model.replace(datainfo=model.datainfo.replace(path=None))
     write_csv(model, path=path)
     model = model.replace(datainfo=model.datainfo.replace(path=path))
 
     dataname = f'{model.name}.csv'
     pre = f'library(rxode2)\n\nev <- read.csv("{path / dataname}")\n'
 
     pre += "\n"
@@ -208,126 +216,78 @@
 
 
 def verification(
     model: pharmpy.model.Model,
     db_name: str,
     error: float = 10**-3,
     return_comp: bool = False,
-    fix_eta: bool = True,
+    ignore_print=False,
 ) -> Union[bool, pd.DataFrame]:
     nonmem_model = model
 
     from pharmpy.modeling import update_inits
     from pharmpy.plugins.nlmixr.model import print_step
     from pharmpy.tools import fit
 
     # Save results from the nonmem model
     if nonmem_model.modelfit_results is None:
-        print_step("Calculating NONMEM predictions... (this might take a while)")
+        if not ignore_print:
+            print_step("Calculating NONMEM predictions... (this might take a while)")
         nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-        nonmem_results = nonmem_model.modelfit_results.predictions.copy()
     else:
         if nonmem_model.modelfit_results.predictions is None:
-            print_step("Calculating NONMEM predictions... (this might take a while)")
+            if not ignore_print:
+                print_step("Calculating NONMEM predictions... (this might take a while)")
             nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-            nonmem_results = nonmem_model.modelfit_results.predictions.copy()
-        else:
-            nonmem_results = nonmem_model.modelfit_results.predictions.copy()
 
     param_estimates = nonmem_model.modelfit_results.parameter_estimates
 
     omega_names = get_omegas(nonmem_model).names
     for name in omega_names:
         param_estimates[name] = 0
 
     sigma_names = get_sigmas(model).names
     for name in sigma_names:
         param_estimates[name] = 0
 
     # Update the nonmem model with new estimates
     # and convert to nlmixr
-    print_step("Converting NONMEM model to RxODE...")
+    if not ignore_print:
+        print_step("Converting NONMEM model to RxODE...")
     rxode_model = convert_model(update_inits(nonmem_model, param_estimates))
 
     # Execute the nlmixr model
-    print_step("Executing RxODE model... (this might take a while)")
+    if not ignore_print:
+        print_step("Executing RxODE model... (this might take a while)")
 
     rxode_model = execute_model(rxode_model, db_name)
-    rxode_results = rxode_model.modelfit_results.predictions
-
-    pred = False
-    ipred = False
-    for p in nonmem_model.modelfit_results.predictions.columns:
-        if p == "PRED":
-            pred = True
-            nonmem_results.rename(columns={p: 'PRED_NONMEM'}, inplace=True)
-            rxode_results.rename(columns={p: 'PRED_RXODE'}, inplace=True)
-        else:
-            print(
-                f"Unknown prediction value {p}. Currently only 'PRED' are supported and this is ignored"
-            )
-
-    if not (pred or ipred):
-        print("No known prediction value was found. Please use 'PRED' or 'IPRED")
-        return False
-
-    # Combine the two based on ID and time
-    print_step("Creating result comparison table...")
-    nonmem_model = nonmem_model.replace(dataset=nonmem_model.dataset.reset_index())
-
-    if "EVID" not in nonmem_model.dataset.columns:
-        nonmem_model = add_evid(nonmem_model)
-    nonmem_results = nonmem_results.reset_index()
-    nonmem_results = nonmem_results.drop(
-        nonmem_model.dataset[nonmem_model.dataset["EVID"] != 0].index.to_list()
-    )
-    nonmem_results = nonmem_results.set_index(["ID", "TIME"])
 
-    combined_result = nonmem_results
-    if pred:
-        combined_result['PRED_RXODE'] = rxode_results['PRED_RXODE'].to_list()
-        # Add difference between the models
-        combined_result['PRED_DIFF'] = abs(
-            combined_result['PRED_NONMEM'] - combined_result['PRED_RXODE']
-        )
+    from pharmpy.plugins.nlmixr.model import compare_models
 
-    combined_result["PASS/FAIL"] = "PASS"
-    print("Differences in population predicted values")
-    if (pred and ipred) or (pred and not ipred):
-        print("Using PRED values for final comparison")
-        final = "PRED"
-    elif ipred and not pred:
-        print("Using IPRED values for final comparison")
-        final = "IPRED"
-    combined_result.loc[combined_result[f'{final}_DIFF'] > error, "PASS/FAIL"] = "FAIL"
-    print(
-        combined_result[f'{final}_DIFF'].describe()[["mean", "75%", "max"]].to_string(), end="\n\n"
+    combined_result = compare_models(
+        nonmem_model, rxode_model, error=error, force_pred=True, ignore_print=ignore_print
     )
 
-    print_step("DONE")
+    if not ignore_print:
+        print_step("DONE")
     if return_comp is True:
         return combined_result
     else:
         if all(combined_result["PASS/FAIL"] == "PASS"):
             return True
         else:
             return False
 
 
-def convert_model(model):
+def convert_model(model, skip_check=False):
     if isinstance(model, Model):
         return model
 
-    if model.internals.control_stream.get_records("DES"):
-        des = model.internals.control_stream.get_records("DES")[0]
-    else:
-        des = None
-
     rxode_model = Model(
-        internals=RxODEModelInternals(DES=des),
+        internals=RxODEModelInternals(),
         parameters=model.parameters,
         random_variables=model.random_variables,
         statements=model.statements,
         dependent_variables=model.dependent_variables,
         estimation_steps=model.estimation_steps,
         filename_extension='.R',
         datainfo=model.datainfo,
@@ -349,38 +309,50 @@
 
         # Add evid
         rxode_model = add_evid(rxode_model)
 
     # Check model for warnings regarding data structure or model contents
     from pharmpy.plugins.nlmixr.sanity_checks import check_model
 
-    rxode_model = check_model(rxode_model)
+    rxode_model = check_model(rxode_model, skip_error_model_check=skip_check)
 
     rxode_model.update_source()
 
     return rxode_model
 
 
 def create_model(cg, model):
     add_true_statements(model, cg, model.statements.before_odes)
 
     if model.statements.ode_system:
         add_ode(model, cg)
 
+    # Add bioavailability statements
+    if model.statements.ode_system is not None:
+        add_bioavailability(model, cg)
+        add_lag_times(model, cg)
+
+    # Add statements after ODE
     add_true_statements(model, cg, model.statements.after_odes)
 
 
 def add_true_statements(model, cg, statements):
     for s in statements:
-        expr = s.expression
-        expr = convert_eps_to_sigma(expr, model)
-        if expr.is_Piecewise:
-            add_piecewise(model, cg, s)
+        if model.statements.ode_system is not None and (
+            s.symbol in get_bioavailability(model).values()
+            or s.symbol in get_lag_times(model).values()
+        ):
+            pass
         else:
-            cg.add(f'{s.symbol.name} <- {expr}')
+            expr = s.expression
+            expr = convert_eps_to_sigma(expr, model)
+            if expr.is_Piecewise:
+                add_piecewise(model, cg, s)
+            else:
+                cg.add(f'{s.symbol.name} <- {expr}')
 
 
 def add_piecewise(model: pharmpy.model.Model, cg: CodeGenerator, s):
     expr = s.expression
     first = True
     for value, cond in expr.args:
         if cond is not sympy.S.true:
@@ -434,18 +406,38 @@
     add_eta(model, cg, as_list=True)
     cg.add(")")
 
 
 def create_sigma(cg, model):
     cg.add("sigmas <-")
     cg.add("lotri(")
-    sigmas = get_sigmas(model)
-    for n, sigma in enumerate(sigmas):
-        if n != len(sigmas) - 1:
-            cg.add(f'{sigma.name} ~ {sigma.init}, ')
+    all_eps = model.random_variables.epsilons
+    for n, eps in enumerate(all_eps):
+        sigma = eps.variance
+        if len(eps.names) == 1:
+            name = model.parameters[sigma].name
+            init = model.parameters[sigma].init
+            if n != len(all_eps) - 1:
+                cg.add(f'{name} ~ {init},')
+            else:
+                cg.add(f'{name} ~ {init}')
         else:
-            cg.add(f'{sigma.name} ~ {sigma.init}')
+            cg.add(f'{" + ".join([name for name in eps.names])} ~ c(')
+            inits = []
+            for row in range(sigma.rows):
+                for col in range(row + 1):
+                    if col == 0 and row != 0:
+                        cg.add(f'{", ".join([str(x) for x in inits])},')
+                        inits = []
+                        inits.append(f'{model.parameters[sigma[row, col].name].init}')
+                    else:
+                        inits.append(model.parameters[sigma[row, col].name].init)
+            cg.add(f'{", ".join([str(x) for x in inits])}')
+            if eps != model.random_variables.epsilons[-1]:
+                cg.add("),")
+            else:
+                cg.add(")")
     cg.add(")")
 
 
 def create_fit(cg, model):
     cg.add(f'fit <- {model.name} %>% rxSolve(thetas, ev, omega = omegas, sigma = sigmas)')
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/plugins/utils.py` & `pharmpy-core-0.95.0/src/pharmpy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.95.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.95.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.95.0/src/pharmpy/reporting/reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 from csscompressor import compress
 from sphinx.application import Sphinx
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.internals.fs.tmp import TemporaryDirectory
 
 
-def generate_report(rst_path, results_path):
+def generate_report(rst_path, results_path, target_path):
     """Generate report from rst and results json"""
     results_path = Path(results_path)
     with TemporaryDirectory() as tmpdirname:
         tmp_path = Path(tmpdirname)
         source_path = tmp_path / 'source'
         source_path.mkdir()
         shutil.copy(rst_path, source_path / 'results.rst')
-        shutil.copy(results_path / 'results.json', source_path)
+        if results_path.is_dir():
+            results_path /= 'results.json'
+        shutil.copy(results_path, source_path)
 
         conf_path = Path(__file__).resolve().parent
 
         # Change directory for results.json to be found
         with chdir(source_path):
             with open(os.devnull, 'w') as devnull:
                 with warnings.catch_warnings():
@@ -87,15 +89,15 @@
     margin-top: 20px;
     width: 100%;
 }
 """
             )
         report_path = tmp_path / 'results.html'
         embed_css_and_js(tmp_path / 'results.html', report_path)
-        shutil.copy(report_path, results_path)
+        shutil.copy(report_path, target_path)
 
 
 def embed_css_and_js(html, target):
     """Embed all external css and javascript into an html"""
     with open(html, 'r', encoding='utf-8') as sh:
         soup = BeautifulSoup(sh, features='lxml')
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/results.py` & `pharmpy-core-0.95.0/src/pharmpy/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from threading import Lock
 
 __all__ = (
+    'create_report',  # pyright: ignore [reportUnsupportedDunderAll]
     'create_results',  # pyright: ignore [reportUnsupportedDunderAll]
     'fit',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_influential_individuals',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_influential_outliers',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_outliers',  # pyright: ignore [reportUnsupportedDunderAll]
     'print_fit_summary',  # pyright: ignore [reportUnsupportedDunderAll]
     'rank_models',  # pyright: ignore [reportUnsupportedDunderAll]
@@ -32,14 +33,15 @@
 )
 
 
 _allowed = set(__all__)
 
 _not_wrapped = {
     '.amd.run': ('run_amd',),
+    '.reporting': ('create_report',),
     '.run': (
         'create_results',
         'fit',
         'print_fit_summary',
         'rank_models',
         'read_modelfit_results',
         'read_results',
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/allometry/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/amd/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/amd/run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/cdd/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/common.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/crossval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/estmethod/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/frem/models.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/frem/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,18 +447,18 @@
         unexplained_variability_plot=plot_unexplained_variability(res),
     )
 
 
 def base_vs_frem_model(frem_model, model_1):
     base_ests = model_1.modelfit_results.parameter_estimates
     final_ests = frem_model.modelfit_results.parameter_estimates
-    ser = pd.Series(dtype=np.float64)
+    ser = pd.Series(dtype=np.float64, name='relative_change')
     for param in base_ests.keys():
-        ser[param] = (final_ests[param] - base_ests[param]) / abs(base_ests[param]) * 100
-    ser.name = 'relative_change'
+        if param in final_ests:
+            ser[param] = (final_ests[param] - base_ests[param]) / abs(base_ests[param]) * 100
     return ser
 
 
 def parameter_inits_and_estimates(frem_model, intermediate_models) -> pd.DataFrame:
     model_names = []
     df = pd.DataFrame()
 
@@ -813,21 +813,21 @@
         covariate_baselines=covariate_baselines,
         parameter_variability=parameter_variability,
     )
 
 
 def get_params(frem_model, rvs, npars):
     param_names = rvs[:npars]
-    sset = frem_model.statements.before_odes
+    sset = reversed(frem_model.statements.before_odes) + frem_model.statements.error
     symbs = []
 
     for p in param_names:
-        statement = [s for s in reversed(sset) if sympy.Symbol(p) in s.rhs_symbols][0]
+        statement = [s for s in sset if sympy.Symbol(p) in s.rhs_symbols][0]
         if str(statement.expression) == p:
-            statement = [s for s in reversed(sset) if statement.symbol in s.rhs_symbols][0]
+            statement = [s for s in sset if statement.symbol in s.rhs_symbols][0]
         symbs.append(statement.symbol.name)
 
     duplicates = set([e for e in symbs if symbs.count(e) > 1])
 
     for i, s in enumerate(symbs):
         if s in duplicates:
             symbs[i] = rename_duplicate(symbs, s)
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/frem/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/linearize/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/linearize/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/linearize/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
 def start_linearize(model):
     return model
 
 
 def create_linearized_model(model):
     linbase = pharmpy.model.Model(
-        parameters=model.parameters, random_variables=model.random_variables
+        parameters=model.parameters,
+        random_variables=model.random_variables,
+        datainfo=model.datainfo,
     )
 
     ms = []
     base_terms_sum = 0
     for i, eta in enumerate(model.random_variables.etas.names, start=1):
         deta = sympy.Symbol("D_ETA1")
         oeta = sympy.Symbol("OETA")
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/qa/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/run.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,23 @@
 def import_tool(name: str):
     return importlib.import_module(f'pharmpy.tools.{name}')
 
 
 def run_tool_with_name(
     name: str, tool, args: Sequence, kwargs: Mapping[str, Any]
 ) -> Union[Model, List[Model], Tuple[Model], Results]:
+    # FIXME: workaround until ModelfitResults is disentangled with
+    #  Model object
+    if 'model' in kwargs.keys() and 'results' in kwargs.keys():
+        model = kwargs['model']
+        res = kwargs['results']
+        if isinstance(model, Model) and isinstance(res, ModelfitResults):
+            model = model.replace(modelfit_results=res)
+            kwargs['model'] = model
+
     common_options, tool_options = split_common_options(kwargs)
 
     create_workflow = tool.create_workflow
 
     dispatcher, tool_database = _get_run_setup(common_options, name)
 
     tool_params = inspect.signature(create_workflow).parameters
@@ -656,14 +665,15 @@
     path : Path
         Path to results file
     lzma : bool
         True for lzma compression. Not applicable to csv file
     csv : bool
         Save as csv file
     """
+    path = normalize_user_given_path(path)
     if csv:
         results.to_csv(path)
     else:
         results.to_json(path, lzma=lzma)
 
 
 def summarize_errors(models: Union[Model, List[Model]]) -> pd.DataFrame:
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,14 @@
     model = remove_error_model(input_model)
     sset = model.statements
     s = sset[0]
     ruv_prop = create_symbol(model, 'epsilon_p')
     ruv_add = create_symbol(model, 'epsilon_a')
     ipred = sympy.Symbol('IPRED')
     s = Assignment(s.symbol, s.expression + ruv_prop + ruv_add / ipred)
-    model = model.replace(statements=s + sset[1:])
 
     prop_name = 'sigma_prop'
     model = add_population_parameter(model, prop_name, 1, lower=0)
     df = model.dataset.copy()
     df['IPRED'].replace(0, 2.225e-307, inplace=True)
     model = model.replace(dataset=df)
     ipred_min = model.dataset['IPRED'].min()
@@ -319,15 +318,18 @@
     add_name = 'sigma_add'
     model = add_population_parameter(model, add_name, sigma_add_init, lower=0)
 
     eps_prop = NormalDistribution.create(ruv_prop.name, 'ruv', 0, sympy.Symbol(prop_name))
     eps_add = NormalDistribution.create(ruv_add.name, 'ruv', 0, sympy.Symbol(add_name))
     name = f'combined_{current_iteration}'
     model = model.replace(
-        random_variables=model.random_variables + [eps_prop, eps_add], name=name, description=name
+        statements=s + sset[1:],
+        random_variables=model.random_variables + [eps_prop, eps_add],
+        name=name,
+        description=name,
     )
     return model
 
 
 def _create_dataset(input_model):
     residuals = input_model.modelfit_results.residuals
     cwres = residuals['CWRES'].reset_index(drop=True)
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/simeval/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/simfit/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.95.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/visualization.py` & `pharmpy-core-0.95.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/args.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/call.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     res: T = dispatcher.run(workflow)
 
     if isinstance(res, Results):
         if hasattr(res, 'tool_database'):
             res = replace(res, tool_database=database)
         database.store_results(res)
         if hasattr(res, 'rst_path'):
-            from pharmpy.modeling.reporting import create_report
+            from pharmpy.tools.reporting import create_report
 
             create_report(res, database.path)
     elif isinstance(res, Model):
         # original_input_models[0].modelfit_results = res.modelfit_results
         pass
     elif isinstance(res, list) or isinstance(res, tuple):
         # index = {model.name: model for model in res}
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/log.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/local_directory.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.95.0/src/pharmpy/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.95.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.94.0
+Version: 0.95.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,33 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.95.0 (2023-05-22)
+-------------------
+
+Changes
+=======
+
+* ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
+
+Bugfixes
+========
+
+* Fix bug causing changes in FIX from model1 to model4 to crash frem
+* Fix bug causing individual parameters in $ERROR to crash frem
+* create_report now does not assume that results.json already exists
+* ~ for $HOME is now supported in write_model and create_report
+* Fix bug where LLOQ value did not override column in dataset in ``transform_blq``
+* Correct BLQ indicator column condition in ``transform_blq``
+* Fix bug where modelfit results were not connected to model after a fit
+
 0.94.0 (2023-04-26)
 -------------------
 
 New features
 ============
 
 * Support parsing assignments other than DADT in $DES in NONMEM
```

### Comparing `pharmpy-core-0.94.0/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.95.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,14 @@
 src/pharmpy/modeling/metabolite.py
 src/pharmpy/modeling/odes.py
 src/pharmpy/modeling/parameter_sampling.py
 src/pharmpy/modeling/parameters.py
 src/pharmpy/modeling/plots.py
 src/pharmpy/modeling/remove_iiv.py
 src/pharmpy/modeling/remove_iov.py
-src/pharmpy/modeling/reporting.py
 src/pharmpy/modeling/results.py
 src/pharmpy/modeling/tmdd.py
 src/pharmpy/modeling/units.py
 src/pharmpy/modeling/update_inits.py
 src/pharmpy/modeling/write_csv.py
 src/pharmpy/modeling/example_models/moxo.csv
 src/pharmpy/modeling/example_models/moxo.mod
@@ -244,14 +243,15 @@
 src/pharmpy/reporting/conf.py
 src/pharmpy/reporting/custom.css
 src/pharmpy/reporting/reporting.py
 src/pharmpy/tools/__init__.py
 src/pharmpy/tools/common.py
 src/pharmpy/tools/psn_helpers.py
 src/pharmpy/tools/rankfuncs.py
+src/pharmpy/tools/reporting.py
 src/pharmpy/tools/run.py
 src/pharmpy/tools/wrap.py
 src/pharmpy/tools/allometry/__init__.py
 src/pharmpy/tools/allometry/tool.py
 src/pharmpy/tools/amd/__init__.py
 src/pharmpy/tools/amd/funcs.py
 src/pharmpy/tools/amd/results.py
@@ -449,14 +449,15 @@
 tests/nonmem/records/test_problem.py
 tests/nonmem/records/test_simulation.py
 tests/nonmem/records/test_sizes.py
 tests/nonmem/records/test_subroutines.py
 tests/nonmem/records/test_theta.py
 tests/plugins/test_nlmixr.py
 tests/plugins/test_plugins.py
+tests/plugins/test_rxode.py
 tests/testdata/pheno_data.csv
 tests/testdata/frem/results.json
 tests/testdata/nonmem/DDMODEL00000130
 tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
 tests/testdata/nonmem/file.csv
 tests/testdata/nonmem/minimal.mod
 tests/testdata/nonmem/pheno.datainfo
@@ -546,14 +547,15 @@
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
 tests/testdata/nonmem/errors/control_stream_error.lst
 tests/testdata/nonmem/errors/est_step_warning.lst
 tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+tests/testdata/nonmem/errors/failed_run.ext
 tests/testdata/nonmem/errors/no_header_error.ext
 tests/testdata/nonmem/errors/no_header_error.lst
 tests/testdata/nonmem/errors/rounding_error.lst
 tests/testdata/nonmem/errors/run_interrupted.ext
 tests/testdata/nonmem/errors/run_interrupted.mod
 tests/testdata/nonmem/errors/zero_gradient_error.lst
 tests/testdata/nonmem/fcon/FCON
@@ -683,14 +685,15 @@
 tests/testdata/nonmem/models/mytab_mox2
 tests/testdata/nonmem/models/pef.csv
 tests/testdata/nonmem/models/pef.mod
 tests/testdata/nonmem/models/pheno_advan3_trans1.ext
 tests/testdata/nonmem/models/pheno_advan3_trans1.lst
 tests/testdata/nonmem/models/pheno_advan3_trans1.mod
 tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+tests/testdata/nonmem/models/pheno_conc.mod
 tests/testdata/nonmem/models/pheno_dvid.csv
 tests/testdata/nonmem/models/pheno_dvid.mod
 tests/testdata/nonmem/models/pheno_noifs.coi
 tests/testdata/nonmem/models/pheno_noifs.cor
 tests/testdata/nonmem/models/pheno_noifs.cov
 tests/testdata/nonmem/models/pheno_noifs.ext
 tests/testdata/nonmem/models/pheno_noifs.lst
```

### Comparing `pharmpy-core-0.94.0/tests/cli/test_cli.py` & `pharmpy-core-0.95.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/conftest.py` & `pharmpy-core-0.95.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/conftest.py` & `pharmpy-core-0.95.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_allometry.py` & `pharmpy-core-0.95.0/tests/integration/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_amd.py` & `pharmpy-core-0.95.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_bootstrap.py` & `pharmpy-core-0.95.0/tests/integration/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_common.py` & `pharmpy-core-0.95.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_covsearch.py` & `pharmpy-core-0.95.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_estmethod.py` & `pharmpy-core-0.95.0/tests/integration/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_evaldesign.py` & `pharmpy-core-0.95.0/tests/integration/test_evaldesign.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_fit.py` & `pharmpy-core-0.95.0/tests/integration/test_fit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_iivsearch.py` & `pharmpy-core-0.95.0/tests/integration/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_iovsearch.py` & `pharmpy-core-0.95.0/tests/integration/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_modelsearch.py` & `pharmpy-core-0.95.0/tests/integration/test_modelsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,16 @@
             results=start_model.modelfit_results,
             model=start_model,
         )
 
         assert len(res.summary_tool) == 4
         assert len(res.summary_models) == 4
         assert len(res.models) == 3
-        assert all(
-            model.modelfit_results and not np.isnan(model.modelfit_results.ofv)
-            for model in res.models
-        )
+        assert all(model.modelfit_results for model in res.models)
+        assert not all(np.isnan(model.modelfit_results.ofv) for model in res.models)
         rundir = tmp_path / 'modelsearch_dir1'
         assert rundir.is_dir()
         assert model_count(rundir) == 3
         assert (rundir / 'results.json').exists()
         assert (rundir / 'results.csv').exists()
         assert (rundir / 'metadata.json').exists()
 
@@ -211,14 +209,15 @@
             'dofv_vs_parent',
             'predicted_dofv',
             'predicted_residual',
         )
         assert summary is not None
         assert tuple(summary.columns) == columns
         for column in columns:
+            # Cannot check that all are non-na because some model runs fail
             assert summary[column].notna().any()
         assert summary['dofv_vs_parent'].equals(
             summary.apply(
                 lambda row: summary.loc[(row['parent_model'], row.name[1])]['ofv'] - row['ofv'],
                 axis=1,
             )
         )
```

### Comparing `pharmpy-core-0.94.0/tests/integration/test_resume.py` & `pharmpy-core-0.95.0/tests/integration/test_resume.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.95.0/tests/integration/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/internals/fs/test_lock.py` & `pharmpy-core-0.95.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/internals/module/test_lazy.py` & `pharmpy-core-0.95.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/internals/test_math.py` & `pharmpy-core-0.95.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/internals/test_parse.py` & `pharmpy-core-0.95.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/model/test_datainfo.py` & `pharmpy-core-0.95.0/tests/model/test_datainfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,14 +72,20 @@
 drop            False
 datatype      float64
 descriptor       None
 Name: DUMMY"""
     assert repr(col) == correct
 
 
+def test_columninfo_hash():
+    col1 = ColumnInfo.create("DUMMY", scale='nominal')
+    col2 = ColumnInfo.create("DUMMY", scale='ratio')
+    assert hash(col1) != hash(col2)
+
+
 def test_init():
     di = DataInfo.create()
     assert len(di) == 0
 
 
 def test_eq():
     di1 = DataInfo.create()
@@ -299,7 +305,40 @@
     dtype = ColumnInfo.convert_datatype_to_pd_dtype("nmtran-date")
     assert dtype == "str"
     dtype = ColumnInfo.convert_datatype_to_pd_dtype("float64")
     assert dtype == "float64"
 
     datatype = ColumnInfo.convert_pd_dtype_to_datatype("float64")
     assert datatype == 'float64'
+
+
+def test_hash():
+    col1 = ColumnInfo.create("ID", type='id')
+    col2 = ColumnInfo.create("WGT", type='covariate', descriptor='body weight')
+    di1 = DataInfo.create([col1, col2])
+    di2 = DataInfo.create([col1])
+    assert hash(di1) != hash(di2)
+
+
+def test_dict():
+    col1 = ColumnInfo.create("ID", type='id')
+    d = col1.to_dict()
+    assert d == {
+        'name': 'ID',
+        'type': 'id',
+        'unit': 'Integer(1)',
+        'scale': 'ratio',
+        'continuous': True,
+        'categories': None,
+        'drop': False,
+        'datatype': 'float64',
+        'descriptor': None,
+    }
+    col2 = ColumnInfo.from_dict(d)
+    assert col1 == col2
+
+
+def test_get_all_categories():
+    col1 = ColumnInfo.create("SCORE", categories=[1, 2, 3])
+    assert col1.get_all_categories() == [1, 2, 3]
+    col2 = ColumnInfo.create("SCORE", categories={1: 'a', 2: 'b'})
+    assert col2.get_all_categories() == [1, 2]
```

### Comparing `pharmpy-core-0.94.0/tests/model/test_parameter.py` & `pharmpy-core-0.95.0/tests/model/test_parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,15 +221,46 @@
     pset1 = Parameters((p1, p2, p3))
     pset2 = pset1.replace(parameters=(p1, p2))
     assert len(pset2) == 2
 
 
 def test_hash():
     p1 = Parameter.create('Y', 9)
-    hash(p1)
+    p2 = Parameter.create('Y', 9, upper=23)
+    assert hash(p1) != hash(p2)
+    p3 = Parameter.create('X', 9)
+    p4 = Parameter.create('Z', 9)
+    pset1 = Parameters((p1, p3))
+    pset2 = Parameters((p1, p4))
+    assert hash(pset1) != hash(pset2)
+
+
+def test_dict():
+    p1 = Parameter.create('Y', 9)
+    d = p1.to_dict()
+    assert d == {
+        'name': 'Y',
+        'init': 9.0,
+        'lower': -float('inf'),
+        'upper': float('inf'),
+        'fix': False,
+    }
+    p2 = Parameter.from_dict(d)
+    assert p1 == p2
+    p3 = Parameter.create('Z', 0, lower=0, upper=22)
+    pset = Parameters((p1, p3))
+    d2 = pset.to_dict()
+    assert d2 == {
+        'parameters': (
+            {'name': 'Y', 'init': 9.0, 'lower': -float('inf'), 'upper': float('inf'), 'fix': False},
+            {'name': 'Z', 'init': 0.0, 'lower': 0.0, 'upper': 22.0, 'fix': False},
+        )
+    }
+    pset2 = Parameters.from_dict(d2)
+    assert pset == pset2
 
 
 def test_contains():
     p1 = Parameter.create('Y', 9)
     p2 = Parameter.create('X', 3)
     p3 = Parameter.create('Z', 1)
     pset1 = Parameters((p1, p2, p3))
```

### Comparing `pharmpy-core-0.94.0/tests/model/test_random_variables.py` & `pharmpy-core-0.95.0/tests/model/test_random_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     dist2 = NormalDistribution.create('ETA(2)', 'iiv', 0, 1)
     dist3 = NormalDistribution.create('ETA(3)', 'iiv', 0, 1)
     rvs = RandomVariables.create([dist1, dist2])
     rvs2 = RandomVariables.create([dist1])
     assert rvs != rvs2
     rvs3 = RandomVariables.create([dist1, dist3])
     assert rvs != rvs3
+    assert hash(rvs) != hash(rvs2)
 
 
 def test_add():
     dist1 = NormalDistribution.create('ETA(1)', 'iiv', 0, 1)
     dist2 = NormalDistribution.create('ETA(2)', 'iiv', 0, 0.1)
     dist3 = NormalDistribution.create('ETA(3)', 'center', 0, 0.1)
     rvs1 = RandomVariables.create([dist1])
@@ -404,14 +405,68 @@
     )
     dist4 = JointNormalDistribution.create(
         ['ETA(1)', 'ETA(3)'], 'iiv', [0, 0], [[1, 0.1], [0.1, 2]]
     )
     assert hash(dist3) != hash(dist4)
 
 
+def test_dict():
+    dist1 = NormalDistribution.create('ETA_3', 'iiv', 2, 1)
+    d = dist1.to_dict()
+    assert d == {
+        'class': 'NormalDistribution',
+        'name': 'ETA_3',
+        'level': 'IIV',
+        'mean': 'Integer(2)',
+        'variance': 'Integer(1)',
+    }
+    dist2 = NormalDistribution.from_dict(d)
+    assert dist1 == dist2
+
+    dist1 = NormalDistribution.create('ETA_1', 'iiv', 0, 1)
+    dist2 = JointNormalDistribution.create(
+        ['ETA_2', 'ETA_3'],
+        'iiv',
+        [0, 0],
+        [
+            [symbol('OMEGA11'), symbol('OMEGA21')],
+            [symbol('OMEGA21'), symbol('OMEGA22')],
+        ],
+    )
+    rvs = RandomVariables.create([dist1, dist2])
+    d = rvs.to_dict()
+    assert d == {
+        'dists': (
+            {
+                'class': 'NormalDistribution',
+                'name': 'ETA_1',
+                'level': 'IIV',
+                'mean': 'Integer(0)',
+                'variance': 'Integer(1)',
+            },
+            {
+                'class': 'JointNormalDistribution',
+                'names': ('ETA_2', 'ETA_3'),
+                'level': 'IIV',
+                'mean': 'ImmutableDenseMatrix([[Integer(0)], [Integer(0)]])',
+                'variance': "ImmutableDenseMatrix([[Symbol('OMEGA11'), Symbol('OMEGA21')], [Symbol('OMEGA21'), Symbol('OMEGA22')]])",  # noqa: E501
+            },
+        ),
+        'eta_levels': {
+            'levels': (
+                {'name': 'IIV', 'reference': True, 'group': 'ID'},
+                {'name': 'IOV', 'reference': False, 'group': 'OCC'},
+            )
+        },
+        'epsilon_levels': {'levels': ({'name': 'RUV', 'reference': True, 'group': None},)},
+    }
+    rvs2 = RandomVariables.from_dict(d)
+    assert rvs == rvs2
+
+
 def test_nearest_valid_parameters():
     values = {'x': 1, 'y': 0.1, 'z': 2}
     dist1 = JointNormalDistribution.create(
         ['ETA(1)', 'ETA(2)'],
         'iiv',
         [0, 0],
         [[symbol('x'), symbol('y')], [symbol('y'), symbol('z')]],
@@ -630,41 +685,58 @@
     assert level.reference is True
     assert level.group == 'ID'
 
     new = level.replace(group='L1')
     assert new.name == 'IIV'
     assert new.reference is True
     assert new.group == 'L1'
+    assert hash(level) != hash(new)
 
     new = level.replace(group='L1', reference=False)
     assert new.name == 'IIV'
     assert new.reference is False
     assert new.group == 'L1'
 
     assert repr(level) == "VariabilityLevel(IIV, reference=True, group=ID)"
 
+    d = level.to_dict()
+    assert d == {'name': 'IIV', 'reference': True, 'group': 'ID'}
+    level2 = VariabilityLevel.from_dict(d)
+    assert level == level2
+
 
 def test_variability_hierarchy():
     lev1 = VariabilityLevel('IIV', reference=True, group='ID')
     levs = VariabilityHierarchy((lev1,))
     assert levs[0].name == 'IIV'
     with pytest.raises(IndexError):
         levs[1].name
     lev2 = VariabilityLevel('CENTER', reference=False, group='CENTER')
     levs2 = VariabilityHierarchy((lev2, lev1))
+    assert hash(levs) != hash(levs2)
     assert len(levs2) == 2
     lev3 = VariabilityLevel('PLANET', reference=False, group='PLANET')
     levs3 = VariabilityHierarchy((lev3, lev2, lev1))
     assert len(levs3) == 3
 
     levs4 = levs + lev2
     assert len(levs4) == 2
     levs5 = lev2 + levs
     assert len(levs5) == 2
 
+    d = levs2.to_dict()
+    assert d == {
+        'levels': (
+            {'name': 'CENTER', 'group': 'CENTER', 'reference': False},
+            {'name': 'IIV', 'group': 'ID', 'reference': True},
+        )
+    }
+    levs6 = VariabilityHierarchy.from_dict(d)
+    assert levs2 == levs6
+
 
 def test_covariance_matrix():
     dist1 = NormalDistribution.create('ETA(1)', 'iiv', 0, symbol('OMEGA(1,1)'))
     dist2 = NormalDistribution.create('ETA(2)', 'iiv', 0, symbol('OMEGA(2,2)'))
     rvs = RandomVariables.create([dist1, dist2])
     assert len(rvs.covariance_matrix) == 4
```

### Comparing `pharmpy-core-0.94.0/tests/model/test_statements.py` & `pharmpy-core-0.95.0/tests/model/test_statements.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,123 @@
     s3 = Assignment(S('M'), sympy.Integer(2))
     s4 = Assignment(S('G'), sympy.Integer(3))
     s1 = Statements([s2, s1])
     s2 = Statements([s3, s4])
     assert s1 != s2
 
 
+def test_hash():
+    s1 = Assignment(S('KA'), S('X') + S('Y'))
+    s2 = Assignment(S('KA'), S('X') + S('Z'))
+    assert hash(s1) != hash(s2)
+
+    b1 = Bolus(S('AMT'))
+    b2 = Bolus(S('AMT'), admid=2)
+    assert hash(b1) != hash(b2)
+
+    i1 = Infusion("AMT", rate="R1")
+    i2 = Infusion("AMT", rate="R2")
+    assert hash(i1) != hash(i2)
+
+    c1 = Compartment.create("DEPOT", lag_time="ALAG")
+    c2 = Compartment.create("DEPOT")
+    assert hash(c1) != hash(c2)
+    assert hash(c1) != hash(output)
+
+    st1 = Statements((s1, s2))
+    st2 = Statements((s1,))
+    assert hash(st1) != hash(st2)
+
+
+def test_dict(load_model_for_test, testdata):
+    ass1 = Assignment(S('KA'), S('X') + S('Y'))
+    d = ass1.to_dict()
+    assert d == {
+        'class': 'Assignment',
+        'symbol': "Symbol('KA')",
+        'expression': "Add(Symbol('X'), Symbol('Y'))",
+    }
+    ass2 = Assignment.from_dict(d)
+    assert ass1 == ass2
+
+    dose1 = Bolus.create('AMT')
+    d = dose1.to_dict()
+    assert d == {'class': 'Bolus', 'amount': "Symbol('AMT')", 'admid': 1}
+    dose2 = Bolus.from_dict(d)
+    assert dose1 == dose2
+
+    inf1 = Infusion.create('AMT', rate='R1')
+    d = inf1.to_dict()
+    assert d == {
+        'class': 'Infusion',
+        'amount': "Symbol('AMT')",
+        'admid': 1,
+        'rate': "Symbol('R1')",
+        'duration': 'None',
+    }
+    inf2 = Infusion.from_dict(d)
+    assert inf1 == inf2
+
+    central = Compartment.create('CENTRAL', dose=dose1)
+    d = central.to_dict()
+    assert d == {
+        'class': 'Compartment',
+        'name': 'CENTRAL',
+        'amount': "Symbol('A_CENTRAL')",
+        'dose': {'class': 'Bolus', 'amount': "Symbol('AMT')", 'admid': 1},
+        'input': 'Integer(0)',
+        'lag_time': 'Integer(0)',
+        'bioavailability': 'Integer(1)',
+    }
+    central2 = Compartment.from_dict(d)
+    assert central == central2
+
+    d = output.to_dict()
+    assert d == {'class': 'Output'}
+    output2 = output.__class__.from_dict(d)
+    assert output == output2
+
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
+    odes = model.statements.ode_system
+    d = odes.to_dict()
+    assert d == {
+        'class': 'CompartmentalSystem',
+        'compartments': (
+            {'class': 'Output'},
+            {
+                'class': 'Compartment',
+                'name': 'CENTRAL',
+                'amount': "Symbol('A_CENTRAL')",
+                'dose': {'class': 'Bolus', 'amount': "Symbol('AMT')", 'admid': 1},
+                'input': 'Integer(0)',
+                'lag_time': 'Integer(0)',
+                'bioavailability': 'Integer(1)',
+            },
+        ),
+        'rates': [(1, 0, "Mul(Symbol('CL'), Pow(Symbol('V'), Integer(-1)))")],
+        't': "Symbol('t')",
+    }
+    odes2 = CompartmentalSystem.from_dict(d)
+    assert odes == odes2
+
+    model = load_model_for_test(testdata / 'nonmem' / 'minimal.mod')
+    d = model.statements.to_dict()
+    assert d == {
+        'statements': (
+            {
+                'class': 'Assignment',
+                'symbol': "Symbol('Y')",
+                'expression': "Add(Symbol('EPS_1'), Symbol('ETA_1'), Symbol('THETA_1'))",
+            },
+        )
+    }
+    stats2 = Statements.from_dict(d)
+    assert model.statements == stats2
+
+
 def test_add():
     s1 = Assignment(S('KA'), S('X') + S('Y'))
     s2 = Assignment(S('Z'), sympy.Integer(23) + S('M'))
     s3 = Assignment(S('M'), sympy.Integer(2))
     s = Statements([s1, s2])
     new = (s3,) + s
     assert len(new) == 3
@@ -248,15 +357,15 @@
 def test_repr_html():
     s1 = Assignment(S('KA'), S('X') + S('Y'))
     stats = Statements([s1])
     html = stats._repr_html_()
     assert 'X + Y' in html
 
     cb = CompartmentalSystemBuilder()
-    dose = Bolus('AMT')
+    dose = Bolus.create('AMT')
     central = Compartment.create('CENTRAL', dose=dose)
     cb.add_compartment(central)
     cb.add_compartment(output)
     cb.add_flow(central, output, S('K'))
     cs = CompartmentalSystem(cb)
     stats = Statements([cs])
     assert type(stats._repr_html_()) == str
@@ -313,25 +422,26 @@
     depot = Compartment.create('DEPOT')
     cb.add_compartment(depot)
     cb.add_flow(depot, central, S('KA'))
     cm = CompartmentalSystem(cb)
     assert cm.find_compartment('DEPOT').dose is None
     assert cm.central_compartment.dose == dose
     cb.move_dose(central, depot)
-    cm = CompartmentalSystem(cb)
-    assert cm.find_compartment('DEPOT').dose == dose
-    assert cm.central_compartment.dose is None
+    cm2 = CompartmentalSystem(cb)
+    assert cm2.find_compartment('DEPOT').dose == dose
+    assert cm2.central_compartment.dose is None
+    assert hash(cm) != hash(cm2)
 
 
 def test_infusion_repr():
-    inf = Infusion('AMT', rate='R1')
+    inf = Infusion.create('AMT', rate='R1')
     assert repr(inf) == 'Infusion(AMT, admid=1, rate=R1)'
-    inf = Infusion('AMT', duration='D1')
+    inf = Infusion.create('AMT', duration='D1')
     assert repr(inf) == 'Infusion(AMT, admid=1, duration=D1)'
-    inf = Infusion('AMT', admid=2, duration='D1')
+    inf = Infusion.create('AMT', admid=2, duration='D1')
     assert repr(inf) == 'Infusion(AMT, admid=2, duration=D1)'
 
 
 def test_infusion_create():
     inf = Infusion.create('AMT', rate='R1')
     assert inf.rate == S('R1')
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_add_covariate_effect.py` & `pharmpy-core-0.95.0/tests/modeling/test_add_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_allometry.py` & `pharmpy-core-0.95.0/tests/modeling/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_block_rvs.py` & `pharmpy-core-0.95.0/tests/modeling/test_block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_blq.py` & `pharmpy-core-0.95.0/tests/modeling/test_blq.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,24 +107,29 @@
     assert 'DV.GE.LLOQ' in model_float.model_code
 
     df_blq = model.dataset
     df_blq['BLQ'] = np.random.randint(0, 2, df_blq.shape[0])
     di_blq = update_datainfo(model.datainfo, df_blq)
     blq_col = di_blq['BLQ'].replace(type='blq')
     di_blq = di_blq.set_column(blq_col)
-    model_blq_col = model.replace(dataset=df_blq, datainfo=di_blq)
+    model_blq = model.replace(dataset=df_blq, datainfo=di_blq)
 
-    model_blq_col = transform_blq(model_blq_col)
+    model_blq_col = transform_blq(model_blq)
 
-    assert 'BLQ.EQ.1' in model_blq_col.model_code
+    assert 'BLQ.EQ.0' in model_blq_col.model_code
 
     df_lloq = model.dataset
     df_lloq['LLOQ'] = np.random.random(df_lloq.shape[0])
     di_lloq = update_datainfo(model.datainfo, df_lloq)
     lloq_col = di_lloq['LLOQ'].replace(type='lloq')
     di_lloq = di_lloq.set_column(lloq_col)
     model_lloq = model.replace(dataset=df_lloq, datainfo=di_lloq)
 
     model_lloq_col = transform_blq(model_lloq)
 
     assert 'DV.GE.LLOQ' in model_lloq_col.model_code
     assert 'LLOQ = ' not in model_lloq_col.model_code
+
+    model_float_with_blq_col = transform_blq(model_blq, lloq=0.1)
+
+    assert 'DV.GE.LLOQ' in model_float_with_blq_col.model_code
+    assert 'LLOQ = ' in model_float_with_blq_col.model_code
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_common.py` & `pharmpy-core-0.95.0/tests/modeling/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.95.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_data_funcs.py` & `pharmpy-core-0.95.0/tests/modeling/test_data_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
 
 def test_set_dvid(load_example_model_for_test):
     m = load_example_model_for_test('pheno')
     m = set_dvid(m, 'FA1')
     col = m.datainfo['FA1']
     assert col.type == 'dvid'
     assert col.scale == 'nominal'
-    assert col.categories == [0, 1]
+    assert col.categories == (0, 1)
     m = set_dvid(m, 'FA1')
     assert m.datainfo['FA1'].type == 'dvid'
     m = set_dvid(m, 'FA2')
     assert m.datainfo['FA1'].type == 'unknown'
     assert m.datainfo['FA2'].type == 'dvid'
     with pytest.raises(ValueError):
         set_dvid(m, 'WGT')
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_distribution.py` & `pharmpy-core-0.95.0/tests/modeling/test_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,40 +69,42 @@
 MAT=THETA(3)*EXP(ETA(3))
 V=VC
 KA=1/MAT
 $ERROR
 Y=F+F*EPS(1)
 $THETA (0,0.00469307) ; POP_CL
 $THETA (0,0.22) ; POP_VC
+$THETA (0,0.22) ; POP_MAT
 $OMEGA 0.0309626  ; IVCL
 $OMEGA 0.0309626  ; IVV
 $OMEGA 0.0309626  ; IVMAT
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION
 """
     model = create_model_for_test(code, dataset='pheno')
     model = add_peripheral_compartment(model)
     correct = """$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV FA1 FA2
 $SUBROUTINE ADVAN4 TRANS4
 $PK
-VP1 = THETA(4)
-QP1 = THETA(3)
+VP1 = THETA(5)
+QP1 = THETA(4)
 CL=THETA(1)*EXP(ETA(1))
 VC=THETA(2)*EXP(ETA(2))
 MAT=THETA(3)*EXP(ETA(3))
 V2 = VC
 KA=1/MAT
 Q = QP1
 V3 = VP1
 $ERROR
 Y=F+F*EPS(1)
 $THETA (0,0.00469307) ; POP_CL
 $THETA (0,0.22) ; POP_VC
+$THETA (0,0.22) ; POP_MAT
 $THETA  (0,0.00469307) ; POP_QP1
 $THETA  (0,0.011000000000000001) ; POP_VP1
 $OMEGA 0.0309626  ; IVCL
 $OMEGA 0.0309626  ; IVV
 $OMEGA 0.0309626  ; IVMAT
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION
@@ -121,40 +123,42 @@
 MAT=THETA(3)*EXP(ETA(3))
 KA=1/MAT
 K=CL/VC
 $ERROR
 Y=F+F*EPS(1)
 $THETA (0,0.00469307) ; POP_CL
 $THETA (0,0.22) ; POP_VC
+$THETA (0,0.22) ; POP_MAT
 $OMEGA 0.0309626  ; IVCL
 $OMEGA 0.0309626  ; IVV
 $OMEGA 0.0309626  ; IVMAT
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION
 """
     model = create_model_for_test(code, dataset='pheno')
     model = add_peripheral_compartment(model)
     correct = """$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno.dta IGNORE=@
 $INPUT ID TIME AMT WGT APGR DV FA1 FA2
 $SUBROUTINE ADVAN4 TRANS1
 $PK
-VP1 = THETA(4)
-QP1 = THETA(3)
+VP1 = THETA(5)
+QP1 = THETA(4)
 CL=THETA(1)*EXP(ETA(1))
 VC=THETA(2)*EXP(ETA(2))
 MAT=THETA(3)*EXP(ETA(3))
 KA=1/MAT
 K23 = QP1/VC
 K32 = QP1/VP1
 K=CL/VC
 $ERROR
 Y=F+F*EPS(1)
 $THETA (0,0.00469307) ; POP_CL
 $THETA (0,0.22) ; POP_VC
+$THETA (0,0.22) ; POP_MAT
 $THETA  (0,0.00469307) ; POP_QP1
 $THETA  (0,0.011000000000000001) ; POP_VP1
 $OMEGA 0.0309626  ; IVCL
 $OMEGA 0.0309626  ; IVV
 $OMEGA 0.0309626  ; IVMAT
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_error.py` & `pharmpy-core-0.95.0/tests/modeling/test_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,21 +76,21 @@
     assert model.model_code.split('\n')[11] == 'Y=F+F*EPS(1)'
     assert model.model_code.split('\n')[17] == '$SIGMA 0.013241'
 
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'pheno_dvid.mod')
     model = set_proportional_error_model(model, dv=2)
     rec = model.internals.control_stream.get_records('ERROR')[0]
     correct = """$ERROR
+Y_1 = F + EPS(1)*F
 IF (F.EQ.0) THEN
     IPREDADJ = 2.22500000000000E-16
 ELSE
     IPREDADJ = F
 END IF
-Y_1 = F + EPS(3)*IPREDADJ
-Y_2 = F + EPS(1)*F + EPS(2)
+Y_2 = F + EPS(2)*IPREDADJ
 
 IF (DVID.EQ.1) THEN
     Y = Y_1
 ELSE
     Y = Y_2
 END IF
 """
@@ -991,17 +991,22 @@
     shutil.copy(testdata / 'nonmem/pheno_real.phi', tmp_path / 'run1.phi')
     shutil.copy(testdata / 'nonmem/pheno_real.ext', tmp_path / 'run1.ext')
     shutil.copy(testdata / 'nonmem/pheno.dta', tmp_path / 'pheno.dta')
 
     with chdir(tmp_path):
         model_pheno = load_model_for_test('run1.mod')
         model_more_eps = re.sub(
+            r'V=TVV\*EXP\(ETA\(2\)\)',
+            'V=TVV',
+            model_pheno.model_code,
+        )
+        model_more_eps = re.sub(
             r'( 0.031128  ;        IVV\n)',
             '$SIGMA 0.1\n$SIGMA 0.1',
-            model_pheno.model_code,
+            model_more_eps,
         )
         model_more_eps = re.sub(
             r'IPRED=F\nIRES=DV-IPRED',
             r'IPRED=F+EPS(2)\nIRES=DV-IPRED+EPS(3)',
             model_more_eps,
         )
         model = create_model_for_test(model_more_eps)
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.95.0/tests/modeling/test_estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_eta_additions.py` & `pharmpy-core-0.95.0/tests/modeling/test_eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_eta_transformations.py` & `pharmpy-core-0.95.0/tests/modeling/test_eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_evaluate.py` & `pharmpy-core-0.95.0/tests/modeling/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_expressions.py` & `pharmpy-core-0.95.0/tests/modeling/test_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import sympy
 
 from pharmpy.model import (
     Assignment,
+    DataInfo,
     Model,
     NormalDistribution,
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
 )
@@ -157,23 +158,27 @@
             [Assignment.create('CL', s('THETA(1)') + s('ETA(1)') + s('ETA(2)'))],
             [Assignment.create('CL', s('THETA(1)') + s('ETA(1)') + s('ETA(2)'))],
         ),
     ],
 )
 def test_mu_reference_model_generic(statements, correct):
     model = Model()
+    datainfo = DataInfo.create(['AGE'])
     eta1 = NormalDistribution.create('ETA(1)', 'iiv', 0, s('omega1'))
     eta2 = NormalDistribution.create('ETA(2)', 'iiv', 0, s('omega2'))
     rvs = RandomVariables.create([eta1, eta2])
     th1 = Parameter('THETA(1)', 2, lower=1)
     th2 = Parameter('THETA(2)', 2, lower=1)
     th3 = Parameter('THETA(3)', 2, lower=1)
     params = Parameters((th1, th2, th3))
     model = model.replace(
-        statements=Statements(statements), parameters=params, random_variables=rvs
+        statements=Statements(statements),
+        parameters=params,
+        random_variables=rvs,
+        datainfo=datainfo,
     )
     model = mu_reference_model(model)
     assert model.statements == Statements(correct)
 
 
 def test_simplify_expression():
     model = Model()
```

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_has_covariate_effect.py` & `pharmpy-core-0.95.0/tests/modeling/test_has_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_help_functions.py` & `pharmpy-core-0.95.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_iterators.py` & `pharmpy-core-0.95.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_lrt.py` & `pharmpy-core-0.95.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_modeling.py` & `pharmpy-core-0.95.0/tests/modeling/test_modeling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.95.0/tests/modeling/test_parameter_sampling.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_parameters.py` & `pharmpy-core-0.95.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_plots.py` & `pharmpy-core-0.95.0/tests/modeling/test_plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_remove_covariate_effect.py` & `pharmpy-core-0.95.0/tests/modeling/test_remove_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/modeling/test_results.py` & `pharmpy-core-0.95.0/tests/modeling/test_results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.95.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_code.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_code.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_data.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.95.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_advan.py` & `pharmpy-core-0.95.0/tests/nonmem/test_advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_des.py` & `pharmpy-core-0.95.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_input.py` & `pharmpy-core-0.95.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_modelfit_results.py` & `pharmpy-core-0.95.0/tests/nonmem/test_modelfit_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,60 @@
 import re
 import shutil
 
 import pandas as pd
 import pytest
 
+from pharmpy.deps import numpy as np
 from pharmpy.internals.fs.cwd import chdir
+from pharmpy.plugins.nonmem.model import parse_code
 from pharmpy.plugins.nonmem.results import simfit_results
 from pharmpy.results import read_results
 
 
 def test_ofv(pheno):
     res = pheno.modelfit_results
     assert res.ofv == 586.27605628188053
 
 
+def test_failed_ofv(testdata, load_model_for_test):
+    code = '''$PROBLEM
+$INPUT ID TIME AMT WGT APGR DV
+$DATA file.csv
+$SUBROUTINES ADVAN2 TRANS2
+$PK
+MAT = THETA(3)*EXP(ETA(1))
+CL = THETA(1)*EXP(ETA(2))
+VC = THETA(2)*EXP(ETA(3))
+KA = 1/MAT
+V = VC
+$ERROR
+Y=F+F*EPS(1)
+$THETA  (0,0.01) ; POP_CL
+$THETA  (0,0.1) ; POP_VC
+$THETA  (0,0.01) ; POP_MAT
+$OMEGA BLOCK(2)
+0.1	; IIV_CL
+0.01	; IIV_CL_IIV_VC
+0.1	; IIV_VC
+$OMEGA  0.1 ; IIV_MAT
+$SIGMA  0.09 ; sigma
+$ESTIMATION METHOD=1 INTER
+'''
+    model = parse_code(code, testdata / 'nonmem' / 'errors' / 'failed_run')
+    res = model.modelfit_results
+    assert np.isnan(res.ofv)
+    assert res.parameter_estimates.isnull().all()
+
+    model = load_model_for_test(testdata / 'nonmem' / 'errors' / 'run_interrupted.mod')
+    res = model.modelfit_results
+    assert np.isnan(res.ofv)
+    assert res.parameter_estimates.isnull().all()
+
+
 def test_special_models(testdata, load_model_for_test):
     onePROB = testdata / 'nonmem' / 'modelfit_results' / 'onePROB'
     withBayes = load_model_for_test(onePROB / 'multEST' / 'noSIM' / 'withBayes.mod')
     assert pytest.approx(withBayes.modelfit_results.standard_errors['POP_CL'], 1e-13) == 2.51942e00
     succ1 = withBayes.modelfit_results.minimization_successful_iterations.iloc[0]
     succ2 = withBayes.modelfit_results.minimization_successful_iterations.iloc[1]
     assert succ1 is not None and not succ1
```

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.95.0/tests/nonmem/test_nonmem_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,32 +189,38 @@
 
     assert len(model.parameters) == 8
     assert model.parameters['COVEFF1'].init == 0.2
     assert model.parameters['COVEFF2'].init == 0.1
 
 
 @pytest.mark.parametrize(
-    'statement_new,buf_new',
+    'statement_new,param_new,buf_new',
     [
-        (Assignment(S('CL'), sympy.Integer(2)), 'CL = 2'),
-        (Assignment(S('Y'), S('THETA(4)') + S('THETA(5)')), 'Y = THETA(4) + THETA(5)'),
+        (Assignment(S('CL'), sympy.Integer(2)), None, 'CL = 2'),
+        (
+            Assignment(S('Y'), S('THETA(4)') + S('THETA(5)')),
+            [Parameter.create('THETA(4)', 0.1), Parameter.create('THETA(5)', 0.1)],
+            'Y = THETA(4) + THETA(5)',
+        ),
     ],
 )
-def test_add_statements(pheno, statement_new, buf_new):
+def test_add_statements(pheno, statement_new, buf_new, param_new):
     sset = pheno.statements
     assert len(sset) == 15
 
     # Insert new statement before ODE system.
     new_sset = []
     for s in sset:
         if isinstance(s, ODESystem):
             new_sset.append(statement_new)
         new_sset.append(s)
 
-    model = pheno.replace(statements=Statements(new_sset))
+    model = pheno.replace(
+        statements=Statements(new_sset), parameters=pheno.parameters + Parameters.create(param_new)
+    )
     model = model.update_source()
 
     assert len(model.statements) == 16
 
     parser = NMTranParser()
     stream = parser.parse(model.model_code)
 
@@ -347,47 +353,14 @@
     model = load_model_for_test(path)
     inits = model.initial_individual_estimates
     assert len(inits) == 59
     assert len(inits.columns) == 2
     assert inits['ETA_1'][2] == -0.166321
 
 
-@pytest.mark.parametrize(
-    'buf_new, len_expected',
-    [
-        (
-            'IF(AMT.GT.0) BTIME=TIME\nTAD=TIME-BTIME\n'
-            'TVCL=THETA(1)*WGT\nTVV=THETA(2)*WGT\n'
-            'IF(APGR.LT.5) TVV=TVV*(1+THETA(3))\nCL=TVCL*EXP(ETA(1))'
-            '\nV=TVV*EXP(ETA(2))\nS1=V\nY=A+B',
-            9,
-        ),
-        (
-            'IF(AMT.GT.0) BTIME=TIME\nTAD=TIME-BTIME\n'
-            'TVCL=THETA(1)*WGT\nTVV=THETA(2)*WGT\n'
-            'IF(APGR.LT.5) TVV=TVV*(1+THETA(3))\nCL=TVCL*EXP(ETA(1))'
-            '\nV=TVV*EXP(ETA(2))\nS1=2*V',
-            8,
-        ),
-    ],
-)
-def test_statements_setter(pheno, buf_new, len_expected):
-    parser = NMTranParser()
-    buf_new = _ensure_trailing_newline(buf_new)
-    statements_new = parser.parse(f'$PRED\n{buf_new}').records[0].statements
-
-    assert len(pheno.statements) == 15
-    assert len(statements_new) == len_expected
-
-    model = pheno.replace(statements=statements_new)
-
-    assert len(model.statements) == len_expected
-    assert model.statements == statements_new
-
-
 def test_deterministic_theta_comments(pheno):
     no_option = 0
     for theta_record in pheno.internals.control_stream.get_records('THETA'):
         no_option += len(list(theta_record.root.subtrees('option')))
 
     assert no_option == 0
```

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.95.0/tests/nonmem/test_nonmem_table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_parser.py` & `pharmpy-core-0.95.0/tests/nonmem/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/nonmem/test_read.py` & `pharmpy-core-0.95.0/tests/nonmem/test_read.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/frem/results.json` & `pharmpy-core-0.95.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.95.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'columns'": "{insert: [(6, OrderedDict([('name', 'FA1'), ('type', 'unknown'), ('scale', "*

 * *              "'nominal'), ('categories', [0, 1])])), (7, OrderedDict([('name', 'FA2'), ('type', "*

 * *              "'unknown'), ('scale', 'nominal'), ('categories', [0, 1])]))]}"}*

```diff
@@ -46,11 +46,29 @@
         },
         {
             "descriptor": "plasma concentration",
             "name": "DV",
             "scale": "ratio",
             "type": "dv",
             "unit": "mg/l"
+        },
+        {
+            "categories": [
+                0,
+                1
+            ],
+            "name": "FA1",
+            "scale": "nominal",
+            "type": "unknown"
+        },
+        {
+            "categories": [
+                0,
+                1
+            ],
+            "name": "FA2",
+            "scale": "nominal",
+            "type": "unknown"
         }
     ],
     "separator": "\\s+"
 }
```

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 Q=THETA(4)*EXP(ETA_Q)
 
 $ERROR
 Y=F+F*EPS(1)
 
 $THETA (0,0.00469307) ; TVCL
 $THETA (0,1.00916) ; TVV
+$THETA (0,0.1)
+$THETA (0,0.1)
 $OMEGA DIAGONAL(2)
 0.0309626  ; IVCL
 0.031128  ; IVV
 $OMEGA 0.1
 $OMEGA BLOCK(2)
 0.0309626
 0.0005 0.031128
```

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.95.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/pheno_data.csv` & `pharmpy-core-0.95.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/metadata.json` & `pharmpy-core-0.95.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/qa_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.95.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_allometry.py` & `pharmpy-core-0.95.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_amd.py` & `pharmpy-core-0.95.0/tests/tools/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_bootstrap.py` & `pharmpy-core-0.95.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_cdd.py` & `pharmpy-core-0.95.0/tests/tools/test_cdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_covsearch.py` & `pharmpy-core-0.95.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_estmethod.py` & `pharmpy-core-0.95.0/tests/tools/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_exports.py` & `pharmpy-core-0.95.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_frem.py` & `pharmpy-core-0.95.0/tests/tools/test_frem.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from io import StringIO
 
 import numpy as np
 import pandas as pd
 import pytest
 from pytest import approx
 
-import pharmpy.modeling as modeling
 import pharmpy.tools as tools
 from pharmpy.tools.frem.models import calculate_parcov_inits, create_model3b
 from pharmpy.tools.frem.results import (
     calculate_results,
     calculate_results_using_bipp,
     get_params,
     psn_frem_results,
@@ -538,11 +537,11 @@
     ofv = res.ofv['ofv']
     assert len(ofv) == 5
 
 
 def test_create_report(testdata, tmp_path):
     res = tools.read_results(testdata / 'frem' / 'results.json')
     shutil.copy(testdata / 'frem' / 'results.json', tmp_path)
-    modeling.create_report(res, tmp_path)
+    tools.create_report(res, tmp_path)
     html = tmp_path / 'results.html'
     assert html.is_file()
     assert html.stat().st_size > 500000
```

### Comparing `pharmpy-core-0.94.0/tests/tools/test_iivsearch.py` & `pharmpy-core-0.95.0/tests/tools/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_iovsearch.py` & `pharmpy-core-0.95.0/tests/tools/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_linearize.py` & `pharmpy-core-0.95.0/tests/tools/test_linearize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from io import StringIO
 
 import pandas as pd
 import pytest
 
+from pharmpy.model import DataInfo
 from pharmpy.tools.linearize.results import calculate_results, psn_linearize_results
 from pharmpy.tools.linearize.tool import create_linearized_model
 from pharmpy.tools.psn_helpers import create_results
 
 
 def test_ofv(load_model_for_test, testdata):
     base = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
@@ -104,9 +105,13 @@
     assert len(res.iofv) == 59
     assert res.ofv['ofv']['base'] == pytest.approx(730.894727)
 
 
 def test_create_linearized_model(load_model_for_test, testdata):
     path = testdata / 'nonmem' / 'pheno_real.mod'
     model = load_model_for_test(path)
+    datainfo = DataInfo.create(
+        ['D_ETA1', 'OETA', 'OPRED', 'D_EPS1', 'D_EPSETA1_1', 'OETA1', 'D_EPSETA1_2', 'OETA2']
+    )
+    model = model.replace(datainfo=datainfo)
     linbase = create_linearized_model(model)
     assert len(linbase.statements) == 8
```

### Comparing `pharmpy-core-0.94.0/tests/tools/test_mfl.py` & `pharmpy-core-0.95.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_ml.py` & `pharmpy-core-0.95.0/tests/tools/test_ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_modelfit.py` & `pharmpy-core-0.95.0/tests/tools/test_modelfit.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_modelsearch.py` & `pharmpy-core-0.95.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_qa.py` & `pharmpy-core-0.95.0/tests/tools/test_qa.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.95.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_run.py` & `pharmpy-core-0.95.0/tests/tools/test_run.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_runtool.py` & `pharmpy-core-0.95.0/tests/tools/test_runtool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.95.0/tests/tools/test_ruvsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_scm.py` & `pharmpy-core-0.95.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_start_model.py` & `pharmpy-core-0.95.0/tests/tools/test_start_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def test_create_start_model(testdata):
     path = testdata / 'nonmem' / 'pheno.dta'
     model = create_start_model(path, modeltype='pk_iv')
     sep = model.datainfo.separator
     assert sep == "\\s+"
-    assert len(model.dataset.columns) == 6
+    assert len(model.dataset.columns) == 8
     assert len(model.parameters) == 6
     assert 'POP_CL' in model.parameters
     assert 'POP_MAT' not in model.parameters
     assert model.statements.ode_system.dosing_compartment.dose == Bolus.create("AMT")
     model = create_start_model(path, modeltype='pk_oral')
     assert 'IIV_MAT' in model.parameters
     assert 'POP_CL' in model.parameters
```

### Comparing `pharmpy-core-0.94.0/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.95.0/tests/tools/test_summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/tools/test_wrap.py` & `pharmpy-core-0.95.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/workflows/test_call.py` & `pharmpy-core-0.95.0/tests/workflows/test_call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/workflows/test_execute.py` & `pharmpy-core-0.95.0/tests/workflows/test_execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/workflows/test_model_database.py` & `pharmpy-core-0.95.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tests/workflows/test_workflow.py` & `pharmpy-core-0.95.0/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.94.0/tox.ini` & `pharmpy-core-0.95.0/tox.ini`

 * *Files identical despite different names*

