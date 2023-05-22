# Comparing `tmp/molfeat-0.8.8.tar.gz` & `tmp/molfeat-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.8.tar", last modified: Wed May  3 22:38:44 2023, max compression
+gzip compressed data, was "molfeat-0.8.9.tar", last modified: Mon May 22 03:06:09 2023, max compression
```

## Comparing `molfeat-0.8.8.tar` & `molfeat-0.8.9.tar`

### file list

```diff
@@ -1,165 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-03 22:38:28.000000 molfeat-0.8.8/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 22:37:10.000000 molfeat-0.8.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 22:37:10.000000 molfeat-0.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 22:38:28.000000 molfeat-0.8.8/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 22:38:28.000000 molfeat-0.8.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-03 22:38:28.000000 molfeat-0.8.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 22:37:10.000000 molfeat-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-03 22:38:44.558586 molfeat-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-03 22:37:10.000000 molfeat-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.538587 molfeat-0.8.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.530587 molfeat-0.8.8/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.542587 molfeat-0.8.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 22:37:10.000000 molfeat-0.8.8/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-03 22:37:10.000000 molfeat-0.8.8/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-03 22:37:10.000000 molfeat-0.8.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.550587 molfeat-0.8.8/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16348 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.554587 molfeat-0.8.8/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-03 22:37:10.000000 molfeat-0.8.8/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.546587 molfeat-0.8.8/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:38:36.000000 molfeat-0.8.8/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 22:38:44.000000 molfeat-0.8.8/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 22:37:10.000000 molfeat-0.8.8/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 22:37:10.000000 molfeat-0.8.8/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-03 22:37:10.000000 molfeat-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 22:37:10.000000 molfeat-0.8.8/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:38:44.558586 molfeat-0.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:38:44.558586 molfeat-0.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 22:37:10.000000 molfeat-0.8.8/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-22 03:05:53.000000 molfeat-0.8.9/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-22 03:04:49.000000 molfeat-0.8.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 03:04:49.000000 molfeat-0.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 03:05:53.000000 molfeat-0.8.9/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-22 03:05:53.000000 molfeat-0.8.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 03:05:54.000000 molfeat-0.8.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-22 03:04:49.000000 molfeat-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-22 03:06:09.774696 molfeat-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-22 03:04:49.000000 molfeat-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.754696 molfeat-0.8.9/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.762696 molfeat-0.8.9/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/custom_model_store.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-22 03:04:49.000000 molfeat-0.8.9/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 03:04:49.000000 molfeat-0.8.9/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 03:04:49.000000 molfeat-0.8.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.770696 molfeat-0.8.9/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-22 03:04:49.000000 molfeat-0.8.9/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.766696 molfeat-0.8.9/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:06:02.000000 molfeat-0.8.9/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 03:06:09.000000 molfeat-0.8.9/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.758696 molfeat-0.8.9/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/nb/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)    29350 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/chemberta-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/chemgpt-fix-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/dgl-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/entropy-transforner-zinc-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    60998 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/featurizer-etl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-22 03:04:49.000000 molfeat-0.8.9/nb/etl/molt5-etl.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 03:04:49.000000 molfeat-0.8.9/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 03:04:49.000000 molfeat-0.8.9/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-22 03:04:49.000000 molfeat-0.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 03:04:49.000000 molfeat-0.8.9/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:06:09.774696 molfeat-0.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:06:09.774696 molfeat-0.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 03:04:49.000000 molfeat-0.8.9/tests/test_viz.py
```

### Comparing `molfeat-0.8.8/.authors.yml` & `molfeat-0.8.9/.authors.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-- name: maclandrol
+- name: Emmanuel Noutahi
   email: emmanuel.noutahi@hotmail.ca
+  aliases:
+  - maclandrol
   alternate_emails:
   - maclandrol@users.noreply.github.com
   num_commits: 0
   first_commit: 2021-04-06 11:53:10
 - name: Cas Wognum
   email: caswognum@outlook.com
   aliases:
```

### Comparing `molfeat-0.8.8/.github/CODE_OF_CONDUCT.md` & `molfeat-0.8.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.8.9/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.8.9/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.8.9/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.8.9/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.8.9/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/workflows/doc.yml` & `molfeat-0.8.9/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/workflows/release.yml` & `molfeat-0.8.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.github/workflows/test.yml` & `molfeat-0.8.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.gitignore` & `molfeat-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/.mailmap` & `molfeat-0.8.9/.mailmap`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 # You can skip bad-name if it is the same as good-name and is unique in the repo.
 #
 # This file is up-to-date if the command git log --format="%aN <%aE>" | sort -u
 # gives no duplicates.
 
 Cas Wognum <caswognum@outlook.com> cwognum <caswognum@outlook.com>
 DomInvivo <dominique@invivoai.com>
+Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca> maclandrol <maclandrol@users.noreply.github.com>
 Hadrien Mary <hadrien.mary@gmail.com> Hadrien Mary <hadim@users.noreply.github.com>
 Honore Hounwanou <mercuryseries@gmail.com>
 Saurav Maheshkar <sauravvmaheshkar@gmail.com>
 Therence <38595485+Therence1@users.noreply.github.com>
 dessygil <desmondgilmour@gmail.com>
-maclandrol <emmanuel.noutahi@hotmail.ca> maclandrol <maclandrol@users.noreply.github.com>
 rbyrne-momatx <113197924+rbyrne-momatx@users.noreply.github.com>
```

### Comparing `molfeat-0.8.8/CHANGELOG.rst` & `molfeat-0.8.9/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 ==================
 molfeat Change Log
 ==================
 
 .. current developments
 
+v0.8.9
+====================
+
+**Added:**
+
+* Support for new featurizers (GPT2-Zinc480M-87M and  Roberta-Zinc480M-102M)
+* ETL scripts/notebooks for transparency
+
+**Fixed:**
+
+* Nav Bar with Tabs
+* Typos in docs
+
+**Authors:**
+
+* Cas Wognum
+* Emmanuel Noutahi
+
+
+
 v0.8.8
 ====================
 
 **Added:**
 
 * A model named Molt5
 * Existing plugins to a the `plugin.yml` file
```

### Comparing `molfeat-0.8.8/LICENSE` & `molfeat-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/PKG-INFO` & `molfeat-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.8
+Version: 0.8.9
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.8 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.9 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.8.8/README.md` & `molfeat-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/api/molfeat.calc.md` & `molfeat-0.8.9/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/assets/css/custom-molfeat.css` & `molfeat-0.8.9/docs/assets/css/custom-molfeat.css`

 * *Files 21% similar despite different names*

```diff
@@ -35,14 +35,18 @@
   background-image: linear-gradient(to right, #1E2F6C, #217EBB);
 }
 
 .md-footer {
   background-image: linear-gradient(to right, #1E2F6C, #217EBB);
 }
 
+.md-tabs {
+  background-image: linear-gradient(to right, #F4F6F9, #C3CFE2);
+}
+
 .md-header__topic {
   color: rgb(255, 255, 255);
 }
 
 .md-source__repository,
 .md-source__icon,
 .md-header__button,
```

### Comparing `molfeat-0.8.8/docs/assets/css/custom.css` & `molfeat-0.8.9/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/benchmark.ipynb` & `molfeat-0.8.9/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/developers/contribute.md` & `molfeat-0.8.9/docs/developers/contribute.md`

 * *Files 17% similar despite different names*

```diff
@@ -49,27 +49,33 @@
 You can build and serve the documentation locally with:
 
 ```bash
 # Build and serve the doc
 mkdocs serve
 ```
 
+
 ## Submitting Pull Requests
 
-If you're considering a large code contribution to Molfeat, please open an issue first to get early feedback on the idea.
+If you're considering a large code contribution to molfeat, please open an issue first to get early feedback on the idea.
 
 Once you think the code is ready to be reviewed, push it to your fork and open a pull request. We will assign a reviewer to your PR.
 For a change to be accepted all existing tests will need to pass. We expect additional tests and documentation for any new features.
 
-If you are developing a plugin for Molfeat, please refer to the corresponding section [Extending Molfeat](./create-plugin.md)
+If you are developing a plugin for molfeat, please refer to the corresponding section [Extending molfeat](./create-plugin.md)
+
+
+## Adding ETL notebooks
+
+Here's an improved version:
+
+## Adding ETL Notebooks
+
+The ETL (extraction, transformation, and loading) scripts document the process of creating new featurizers, and we make our ETL notebooks open to the community for transparency purposes. As a developer adding new featurizers, please document your process in the [etl notebook folder](https://github.com/datamol-io/molfeat/tree/main/nb/etl).
+
+By documenting your process in the ETL notebook, you help ensure that the registration of new models can be reviewed by the community and provide greater visibility into the development process. This can help build trust with our users and contributors, and encourage collaboration and feedback.
+
+## Releasing a New Version
 
-## Release a new version
+To release a new version, code maintainers can use the `release` GitHub action. However, before releasing a new version, it is important to coordinate with the code owners to ensure that the release roadmap is followed and any critical pull requests have been merged.
 
-- Run check: `rever check`.
-- Bump and release new version: `rever VERSION_NUMBER`.
-- Releasing a new version will do the following tasks in this order:
-  - Update `AUTHORS.rst`.
-  - Update `CHANGELOG.rst`.
-  - Bump the version number in `setup.py` and `_version.py`.
-  - Add a git tag.
-  - Push the git tag.
-  - Add a new release on the GH repo associated with the git tag.
+The release roadmap should be followed to ensure that the new version is stable, functional, and meets the requirements of the release. This includes proper testing, documentation, and ensuring backward compatibility where necessary. By following these guidelines, we can ensure that new versions are released smoothly and efficiently, with clear communication to our users and contributors.
```

### Comparing `molfeat-0.8.8/docs/developers/create-plugin.md` & `molfeat-0.8.9/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/developers/register-plugin.md` & `molfeat-0.8.9/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/images/logo-black.png` & `molfeat-0.8.9/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/images/logo-black.svg` & `molfeat-0.8.9/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/images/logo-title.svg` & `molfeat-0.8.9/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/images/logo.png` & `molfeat-0.8.9/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/images/logo.svg` & `molfeat-0.8.9/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/index.md` & `molfeat-0.8.9/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Overview
+# What is molfeat ?
 
 Molfeat is a hub of molecular featurizers. It supports a wide variety of out-of-the-box molecular featurizers and can be easily extended to include your own custom featurizers.
 
 - 🚀 Fast, with a simple and efficient API.
 - 🔄 Unify pre-trained molecular embeddings and hand-crafted featurizers in a single package.
 - ➕ Easily add your own featurizers through plugins.
 - 📈 Benefit from increased performance through a trouble-free caching system.
```

### Comparing `molfeat-0.8.8/docs/tutorials/add_your_own.ipynb` & `molfeat-0.8.9/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/datacache.ipynb` & `molfeat-0.8.9/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/graphs.ipynb` & `molfeat-0.8.9/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/integrations.ipynb` & `molfeat-0.8.9/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.8.9/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/save_and_load.ipynb` & `molfeat-0.8.9/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.8.9/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.8.9/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/docs/usage.md` & `molfeat-0.8.9/docs/usage.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Getting started
-## Organization
+# Usage
+## Structure
 Molfeat is organized in three main modules:
 
 - `molfeat.store`: The model store loads, lists and registers all featurizers.
 - `molfeat.calc`: A calculator is a callable that featurizes a single molecule. 
 - `molfeat.trans`: A transformer is a scikit-learn compatible class that wraps a calculator in a featurization pipeline.
 
 !!! note annotate "Learn more about the different types of featurizers"
```

### Comparing `molfeat-0.8.8/env.yml` & `molfeat-0.8.9/env.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/mkdocs.yml` & `molfeat-0.8.9/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 repo_name: "datamol-io/molfeat"
 
 remote_branch: "gh-pages"
 use_directory_urls: false
 copyright: Copyright 2020 - 2023 datamol.io
 
 nav:
-  - Overview: index.md
-  - Why should you care?: benchmark.ipynb
-  - Getting Started: usage.md
+  - Getting started:
+      - What is molfeat ?: index.md
+      - How to use ?: usage.md
+      - Why should you care?: benchmark.ipynb
+      - License: license.md
+
   - Tutorials:
       - Types of featurizers: tutorials/types_of_featurizers.ipynb
-      - Add your own featurizer: tutorials/add_your_own.ipynb
+      - Add your own:
+          - Create your own featurizers: tutorials/add_your_own.ipynb
+          - Create a custom modelstore: tutorials/custom_model_store.ipynb
       - Featurizing graphs: tutorials/graphs.ipynb
       - Integrations:
           - Integration with scikit-learn and PyTorch: tutorials/integrations.ipynb
           - Training a GNN with PyG: tutorials/pyg_integration.ipynb
           - Finetuning a pretrained transformer: tutorials/transformer_finetuning.ipynb
       - Save and Load: tutorials/save_and_load.ipynb
       - The Data Cache: tutorials/datacache.ipynb
@@ -42,26 +47,26 @@
               - DGL: api/molfeat.trans.pretrained.dgl_pretrained.md
               - FCD: api/molfeat.trans.pretrained.fcd.md
       - molfeat.store: api/molfeat.store.md
       - molfeat.plugins: api/molfeat.plugins.md
       - molfeat.utils: api/molfeat.utils.md
       - molfeat.viz: api/molfeat.viz.md
 
-  - License: license.md
-
 theme:
   name: material
-  # NOTE(cwognum): to customize the material primary and secondary
-  # color check `docs/assets/css/custom-molfeat.css`.
   features:
     - navigation.tabs
-    - navigation.expand
+    - navigation.tracking
+    - navigation.top
+
   favicon: images/logo-black.png
   logo: images/logo.svg
 
+# NOTE(cwognum): to customize the material primary and secondary
+# color check `docs/assets/css/custom-molfeat.css`.
 extra_css:
   - assets/css/custom.css
   - assets/css/custom-molfeat.css
   - assets/css/tweak-width.css
 
 extra_javascript:
   - assets/js/google-analytics.js
```

### Comparing `molfeat-0.8.8/molfeat/calc/__init__.py` & `molfeat-0.8.9/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/_atom_bond_features.py` & `molfeat-0.8.9/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/_map4.py` & `molfeat-0.8.9/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/_mhfp.py` & `molfeat-0.8.9/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/atom.py` & `molfeat-0.8.9/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/base.py` & `molfeat-0.8.9/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/bond.py` & `molfeat-0.8.9/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/cats.py` & `molfeat-0.8.9/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/descriptors.py` & `molfeat-0.8.9/molfeat/calc/descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/fingerprints.py` & `molfeat-0.8.9/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/pharmacophore.py` & `molfeat-0.8.9/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/shape.py` & `molfeat-0.8.9/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/skeys.py` & `molfeat-0.8.9/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/calc/tree.py` & `molfeat-0.8.9/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/data/cats_features.fdef` & `molfeat-0.8.9/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/data/elements.xz` & `molfeat-0.8.9/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/data/elements_completed.xz` & `molfeat-0.8.9/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/data/origin.xz` & `molfeat-0.8.9/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/data/skey_parameters.csv` & `molfeat-0.8.9/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/plugins/entry_point.py` & `molfeat-0.8.9/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/plugins/factories.py` & `molfeat-0.8.9/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/store/loader.py` & `molfeat-0.8.9/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/store/modelcard.py` & `molfeat-0.8.9/molfeat/store/modelcard.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     representation: Literal["graph", "line-notation", "vector", "tensor", "other"]
     require_3D: Optional[bool] = False
     tags: Optional[List[str]]
     authors: Optional[List[str]]
     reference: Optional[str]
     created_at: datetime = Field(default_factory=datetime.now)
     sha256sum: Optional[str]
+    model_usage: Optional[str]
 
     def path(self, root_path: str):
         """Generate the folder path where to save this model
 
         Args:
             root_path: path to the root folder
         """
@@ -93,16 +94,26 @@
         self_content.pop("created_at", None)
         new_content.pop("created_at", None)
         if match_only is not None:
             self_content = {k: self_content.get(k) for k in match_only}
             new_content = {k: new_content.get(k) for k in match_only}
         return self_content == new_content
 
+    def set_usage(self, usage: str):
+        """Set the usage of the model
+
+        Args:
+            usage: usage of the model
+        """
+        self.model_usage = usage
+
     def usage(self):
         """Return the usage of the model"""
+        if self.model_usage is not None and self.model_usage:
+            return self.model_usage
         import_statement, loader_statement = get_model_init(self)
         comment = "# sanitize and standardize your molecules if needed"
         if self.require_3D:
             comment += "\n# <generate 3D coordinates here> "
         usage = f"""
         import datamol as dm
         {import_statement}
```

### Comparing `molfeat-0.8.8/molfeat/store/modelstore.py` & `molfeat-0.8.9/molfeat/store/modelstore.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,47 +8,62 @@
 import pathlib
 import os
 import fsspec
 import tempfile
 import platformdirs
 import filelock
 import datamol as dm
+from dotenv import load_dotenv
 from loguru import logger
 
 from molfeat.store.modelcard import ModelInfo
 from molfeat.utils import commons
 
 
+load_dotenv()
+
+
 class ModelStoreError(Exception):
     pass
 
 
 class ModelStore:
-    """A class emulating artefact serializing from any url
+    """A class for artefact serializing from any url
 
-    This class should not only allow pretrained model serializing and loading,
-    but should also help in listing model availability and registering models
+    This class not only allow pretrained model serializing and loading,
+    but also help in listing model availability and registering models.
 
     For simplicity.
         * There is no versioning.
-        * Only one model per model name is permitted
-        * Model deletion is not allowed
-        * Only a single Cloud storage is supported
+        * Only one model should match a given name
+        * Model deletion is not allowed (on the read-only default store)
+        * Only a single store is supported per model store instance
+
+    !!! note "Building a New Model Store"
+        To create a new model store, you will mainly need a model store bucket path. The default model store bucket, located at `gs://molfeat-store-prod/artifacts/`, is **read-only**.
+
+        To build your own model store bucket, follow the instructions below:
+
+        1. Create a local or remote cloud directory that can be accessed by fsspec (and the corresponding filesystem).
+        2. [Optional] Sync the default model store bucket to your new path if you want to access the default models.
+        3. Set the environment variable `MOLFEAT_MODEL_STORE_BUCKET` to your new path. This variable will be used as the default model store bucket when creating a new model store instance without specifying a path.
+            Note that setting up this path is necessary if you want to access models directly by their names, without manually loading them from your custom model store.
+
 
     """
 
     # EN: be careful not to recreate ada
     # EN: should we just use modelstore ?
     MODEL_STORE_BUCKET = "gs://molfeat-store-prod/artifacts/"
     MODEL_PATH_NAME = "model.save"
     METADATA_PATH_NAME = "metadata.json"
 
     def __init__(self, model_store_bucket: Optional[str] = None):
         if model_store_bucket is None:
-            model_store_bucket = self.MODEL_STORE_BUCKET
+            model_store_bucket = os.getenv("MOLFEAT_MODEL_STORE_BUCKET", self.MODEL_STORE_BUCKET)
         self.model_store_bucket = model_store_bucket
         self._available_models = []
         self._update_store()
 
     def _update_store(self):
         """Initialize the store with all available models"""
         all_metadata = dm.fs.glob(dm.fs.join(self.model_store_bucket, "**/metadata.json"))
@@ -60,31 +75,41 @@
                 self._available_models.append(model_info)
 
     @property
     def available_models(self):
         """Return a list of all models that have been serialized in molfeat"""
         return self._available_models
 
+    def __len__(self):
+        """Return the length of the model store"""
+        return len(self.available_models)
+
     def register(
         self,
         modelcard: Union[ModelInfo, dict],
         model: Optional[Any] = None,
         chunk_size: int = 2048,
         save_fn: Optional[Callable] = None,
         save_fn_kwargs: Optional[dict] = None,
         force: bool = True,
     ):
         """
         Register a new model to the store
 
+        !!! note `save_fn`
+            You can pass additional kwargs for your `save_fn` through the `save_fn_kwargs` argument.
+            It's expected that `save_fn` will be called as : `save_fn(model, <model_upload_path>, **save_fn_wargs)`,
+            with `<model_upload_path>` being provided by the model store, and that it will return the path to the serialized model.
+            If not provided, `joblib.dump` is used by default.
+
         Args:
             modelcard: Model information
             model: A path to the model artifact or any object that needs to be saved
             chunk_size: the chunk size for the upload
-            save_fn: any custom function for serializing the model, that takes the model, the upload path and parameters as inputs
+            save_fn: any custom function for serializing the model, that takes the model, the upload path and parameters `save_fn_kwargs` as inputs.
             save_fn_kwargs: any additional kwargs to pass to save_fn
             force: whether to force upload to the bucket
 
         """
         if not isinstance(modelcard, ModelInfo):
             modelcard = ModelInfo(**modelcard)
         # we save the model first
@@ -112,14 +137,16 @@
                 progress=True,
                 leave_progress=False,
                 chunk_size=chunk_size,
                 force=force,
             )
         else:
             model_path = save_fn(model, model_upload_path, **save_fn_kwargs)
+            # we reset to None if the save_fn has not returned anything
+            model_path = model_path or model_upload_path
         modelcard.sha256sum = commons.sha256sum(model_path)
         # then we save the metadata as json
         with fsspec.open(model_metadata_upload_path, "w") as OUT:
             OUT.write(modelcard.json())
         self._update_store()
         logger.info(f"Successfuly registered model {modelcard.name} !")
```

### Comparing `molfeat-0.8.8/molfeat/trans/base.py` & `molfeat-0.8.9/molfeat/trans/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/concat.py` & `molfeat-0.8.9/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/fp.py` & `molfeat-0.8.9/molfeat/trans/fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/graph/adj.py` & `molfeat-0.8.9/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/graph/tree.py` & `molfeat-0.8.9/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/pretrained/base.py` & `molfeat-0.8.9/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.8.9/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,14 @@
 
     def __init__(
         self,
         name: str,
         cache_path: Optional[os.PathLike] = None,
         store: Optional[ModelStore] = None,
     ):
-        if name not in self.AVAILABLE_MODELS:
-            raise ValueError(f"{name} is not a supported pretrained gin model")
-
         super().__init__(name, cache_path=cache_path, store=store)
         self._model = None
 
     @classmethod
     def available_models(cls, query: Optional[str] = None):
         """List available models
         Args:
```

### Comparing `molfeat-0.8.8/molfeat/trans/pretrained/fcd.py` & `molfeat-0.8.9/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.8.9/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.8.9/molfeat/trans/pretrained/hf_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
         !!! note
             The pooling module of this featurizer is accessible through the `_pooling_obj` attribute.
 
         Args:
             kind: name of the featurizer as available in the model store
             notation: optional line notation to use. Only use if it cannot be found from the model card.
-            pooling: type of pooling to use. One of ['default', 'mean', 'max', 'sum']. The value "default" corresponds to the default litterature pooling for each model type.
+            pooling: type of pooling to use. One of ['default', 'mean', 'max', 'sum', 'clf', ]. The value "default" corresponds to the default litterature pooling for each model type.
                 See `molfeat.utils.pooler.get_default_hf_pooler` for more details.
             concat_layers: Layer to concat to get the representation. By default the last hidden layer is returned.
             prefer_encoder: For an encoder-decoder model, prefer the embeddings provided by the encoder.
             dtype: Data type to output
             device: Torch device on which to run the featurizer.
             max_length: Maximum length of the input sequence to consider. Please update this for large sequences
             ignore_padding: Whether to ignore padding in the representation (default: True) to avoid effect of batching
```

### Comparing `molfeat-0.8.8/molfeat/trans/struct/esm.py` & `molfeat-0.8.9/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/trans/struct/prot1D.py` & `molfeat-0.8.9/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/cache.py` & `molfeat-0.8.9/molfeat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/commons.py` & `molfeat-0.8.9/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/const.py` & `molfeat-0.8.9/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/converters.py` & `molfeat-0.8.9/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/datatype.py` & `molfeat-0.8.9/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/log.py` & `molfeat-0.8.9/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/parsing.py` & `molfeat-0.8.9/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/pooler.py` & `molfeat-0.8.9/molfeat/utils/pooler.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             mask = mask.unsqueeze(-1)  # B, S, 1
         return self.pooling(h, indices=None, mask=mask)
 
 
 class BertPooler(nn.Module):
     """
     Default Bert pooler as implemented in huggingface transformers
-    The bert pooling function focuses on the first token ([CLS]) to get a sentence representation.
+    The bert pooling function focuses on a projection of the first token ([CLS]) to get a sentence representation.
     """
 
     def __init__(
         self,
         config,
         activation: Optional[Callable] = None,
         random_seed: int = None,
@@ -153,15 +153,15 @@
         pooled_output = self.activation(pooled_output)
         return pooled_output
 
 
 class BartPooler(nn.Module):
     """
     Default Bart pooler as implemented in huggingface transformers
-    The Bart pooling function focusing on the first token ([CLS]) to get a sentence representation.
+    The Bart pooling function focusing on the eos token ([EOS]) to get a sentence representation.
     """
 
     def __init__(self, config, **kwargs):
         super().__init__()
         self.config = config
 
     def forward(
@@ -182,15 +182,15 @@
         pooled_output = h[eos_mask, :].view(h.size(0), -1, h.size(-1))[:, -1, :]
         return pooled_output
 
 
 class GPTPooler(nn.Module):
     """
     Default GPT pooler as implemented in huggingface transformers
-    The Bart pooling function focusing on the first token ([CLS]) to get a sentence representation.
+    The GPT pooling function focusing on the last non-padding token given sequence length to get a sentence representation.
     """
 
     def __init__(self, config, **kwargs):
         super().__init__()
         self.config = config
         self.pad_token_id = config.get("pad_token_id")
```

### Comparing `molfeat-0.8.8/molfeat/utils/requires.py` & `molfeat-0.8.9/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/utils/state.py` & `molfeat-0.8.9/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat/viz.py` & `molfeat-0.8.9/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/molfeat.egg-info/PKG-INFO` & `molfeat-0.8.9/molfeat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.8
+Version: 0.8.9
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.8 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.9 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.8.8/molfeat.egg-info/SOURCES.txt` & `molfeat-0.8.9/molfeat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 docs/developers/register-plugin.md
 docs/images/logo-black.png
 docs/images/logo-black.svg
 docs/images/logo-title.svg
 docs/images/logo.png
 docs/images/logo.svg
 docs/tutorials/add_your_own.ipynb
+docs/tutorials/custom_model_store.ipynb
 docs/tutorials/datacache.ipynb
 docs/tutorials/graphs.ipynb
 docs/tutorials/integrations.ipynb
 docs/tutorials/pyg_integration.ipynb
 docs/tutorials/save_and_load.ipynb
 docs/tutorials/transformer_finetuning.ipynb
 docs/tutorials/types_of_featurizers.ipynb
@@ -121,14 +122,20 @@
 molfeat/utils/converters.py
 molfeat/utils/datatype.py
 molfeat/utils/log.py
 molfeat/utils/parsing.py
 molfeat/utils/pooler.py
 molfeat/utils/requires.py
 molfeat/utils/state.py
+nb/etl/chemberta-etl.ipynb
+nb/etl/chemgpt-fix-etl.ipynb
+nb/etl/dgl-etl.ipynb
+nb/etl/entropy-transforner-zinc-etl.ipynb
+nb/etl/featurizer-etl.ipynb
+nb/etl/molt5-etl.ipynb
 news/TEMPLATE.rst
 tests/test_atom_bond_calculator.py
 tests/test_descriptors.py
 tests/test_fp.py
 tests/test_graphs.py
 tests/test_pharmacophore.py
 tests/test_pretrained.py
```

### Comparing `molfeat-0.8.8/pyproject.toml` & `molfeat-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_atom_bond_calculator.py` & `molfeat-0.8.9/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_descriptors.py` & `molfeat-0.8.9/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_fp.py` & `molfeat-0.8.9/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_graphs.py` & `molfeat-0.8.9/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_pharmacophore.py` & `molfeat-0.8.9/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_pretrained.py` & `molfeat-0.8.9/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_prot_embed.py` & `molfeat-0.8.9/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_state.py` & `molfeat-0.8.9/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.8/tests/test_utils.py` & `molfeat-0.8.9/tests/test_utils.py`

 * *Files identical despite different names*

