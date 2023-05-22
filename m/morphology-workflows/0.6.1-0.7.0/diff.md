# Comparing `tmp/morphology-workflows-0.6.1.tar.gz` & `tmp/morphology-workflows-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphology-workflows-0.6.1.tar", last modified: Mon Mar 27 20:31:52 2023, max compression
+gzip compressed data, was "morphology-workflows-0.7.0.tar", last modified: Mon May 22 19:14:17 2023, max compression
```

## Comparing `morphology-workflows-0.6.1.tar` & `morphology-workflows-0.7.0.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.547841 morphology-workflows-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-03-27 20:31:52.547841 morphology-workflows-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.511841 morphology-workflows-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.511841 morphology-workflows-0.6.1/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)       21 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.511841 morphology-workflows-0.6.1/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (123)   239826 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/logo/BBP-Morphology-Workflows.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/docs/source/luigi_cfg.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.511841 morphology-workflows-0.6.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/examples/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/examples/luigi.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/examples/neuromorpho_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/examples/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:31:52.547841 morphology-workflows-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.495841 morphology-workflows-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_data/default_placeholders.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/allen_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows/_templates/config_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/config_templates/default.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/config_templates/example_template_curate_dataset.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/luigi.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/mouselight_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/neuromorpho_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows/_templates/source_report/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2549 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/_templates/source_report/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10303 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/marker_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/repair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/src/morphology_workflows/tasks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/tasks/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/src/morphology_workflows/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.515841 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 20:31:52.000000 morphology-workflows-0.6.1/src/morphology_workflows.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/allen_config_download.json
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/mouselight_config_download.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/neuromorpho_config_download.json
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/placeholders.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.503841 morphology-workflows-0.6.1/tests/data/test_example_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/Annotate/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24957 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/Annotate/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/ApicalPoint/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.519841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CollectCurated/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CollectCurated/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CutLeaves/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CutLeaves/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/HardLimit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/HardLimit/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/MType/
--rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/MType/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotApicalPoint/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3207 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotCutLeaves/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotHardLimit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5108 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     7192 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/annotated_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Align/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Align/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/CheckNeurites/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/CheckNeurites/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Collect/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Collect/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Curate/
--rw-r--r--   0 runner    (1001) docker     (123)    37582 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Curate/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/DetectErrors/
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/DetectErrors/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/ExtractMarkers/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Orient/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Orient/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.523841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotErrors/
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotErrors/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMarkers/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMarkers/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMorphologies/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Recenter/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Recenter/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Sanitize/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Sanitize/report.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/curated_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/CollectAnnotated/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2964 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/FixZeroDiameters/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeCollage/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeCollage/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeRelease/
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeRelease/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/PlotRepair/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/PlotRepair/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Repair/
--rw-r--r--   0 runner    (1001) docker     (123)    43809 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Repair/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/RepairNeurites/
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Unravel/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Unravel/report.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/repaired_dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-asc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.527841 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-h5/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-swc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-asc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-h5/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-swc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-asc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-h5/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-swc/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_report/
--rwxr-xr-x   0 runner    (1001) docker     (123)    57075 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_report/report_latexpdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)    16643 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_report/report_no_exception_rst2pdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   123901 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_report/report_rst2pdf.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.531841 morphology-workflows-0.6.1/tests/data/test_report_before_run/
--rwxr-xr-x   0 runner    (1001) docker     (123)    42350 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_report_before_run/report_latexpdf.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)    10085 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/data/test_report_before_run/report_rst2pdf.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.535841 morphology-workflows-0.6.1/tests/examples_test/
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/builder_recipe.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/dataset.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:31:52.543841 morphology-workflows-0.6.1/tests/examples_test/morphologies/
--rw-r--r--   0 runner    (1001) docker     (123)  1255757 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/C060114A5.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)   395836 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/C270106A.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/README
--rwxr-xr-x   0 runner    (1001) docker     (123)   589072 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/astrocyte.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)    10180 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/circle_contour.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/complexe.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/disconnected_neurite.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/iterators.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/mono-type.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/multiple_point_section.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/multiple_soma.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/nested_single_children.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/neurite_wrong_root_point.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)   107856 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/nrn-order-already-sorted.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)   165400 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/nrn_ordering.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/pia.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/reversed_NRN_neurite_order.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)   491711 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/rp100427-123_idC.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/sections-block.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/simple-with-font.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/simple-with-image-coord.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      548 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/simple.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      610 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/simple.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/simple2.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/soma_cylinders.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/soma_multiple_frustums.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/soma_single_frustum.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/soma_three_points_cylinder.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/spine.asc
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/morphologies/three_point_soma.swc
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/mouse_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/placement_rules.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)    57762 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/report_CurateDataset.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   130944 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/report_example.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/run_curation.sh
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/examples_test/transform_rules.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/test_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/test_download_morphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/test_example_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-27 20:31:39.000000 morphology-workflows-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.520093 morphology-workflows-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-22 19:14:17.520093 morphology-workflows-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.492093 morphology-workflows-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       21 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)   239826 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/logo/BBP-Morphology-Workflows.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/docs/source/luigi_cfg.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/examples/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/examples/luigi.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/examples/neuromorpho_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/examples/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:14:17.520093 morphology-workflows-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.484093 morphology-workflows-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/src/morphology_workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/src/morphology_workflows/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_data/default_placeholders.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.500093 morphology-workflows-0.7.0/src/morphology_workflows/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/allen_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.500093 morphology-workflows-0.7.0/src/morphology_workflows/_templates/config_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/config_templates/default.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/config_templates/example_template_curate_dataset.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/luigi.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/mouselight_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/neuromorpho_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.500093 morphology-workflows-0.7.0/src/morphology_workflows/_templates/source_report/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2549 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/_templates/source_report/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10303 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/marker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/repair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.500093 morphology-workflows-0.7.0/src/morphology_workflows/tasks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      427 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/tasks/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/src/morphology_workflows/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.496093 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 19:14:17.000000 morphology-workflows-0.7.0/src/morphology_workflows.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.500093 morphology-workflows-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/allen_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/mouselight_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/neuromorpho_config_download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/placeholders.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.488093 morphology-workflows-0.7.0/tests/data/test_example_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/Annotate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24957 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/Annotate/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/ApicalPoint/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CollectCurated/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CollectCurated/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CutLeaves/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3302 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CutLeaves/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/HardLimit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3554 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/HardLimit/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/MType/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/MType/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotApicalPoint/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3207 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotCutLeaves/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotHardLimit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5108 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7192 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/annotated_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Align/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Align/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/CheckNeurites/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/CheckNeurites/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Collect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Collect/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Curate/
+-rw-r--r--   0 runner    (1001) docker     (123)    37582 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Curate/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/DetectErrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/DetectErrors/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/ExtractMarkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Orient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Orient/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotErrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotErrors/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMarkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMarkers/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMorphologies/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Recenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Recenter/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Sanitize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Sanitize/report.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/curated_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.504093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/CollectAnnotated/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2964 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/FixZeroDiameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeCollage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeCollage/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeRelease/
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeRelease/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/PlotRepair/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/PlotRepair/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Repair/
+-rw-r--r--   0 runner    (1001) docker     (123)    43809 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Repair/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/RepairNeurites/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Unravel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Unravel/report.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/repaired_dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-asc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-h5/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-swc/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_report/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57075 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_report/report_latexpdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16643 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_report/report_no_exception_rst2pdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   123901 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_report/report_rst2pdf.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.508093 morphology-workflows-0.7.0/tests/data/test_report_before_run/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42350 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_report_before_run/report_latexpdf.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10085 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/data/test_report_before_run/report_rst2pdf.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.512093 morphology-workflows-0.7.0/tests/examples_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/builder_recipe.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/dataset.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:14:17.520093 morphology-workflows-0.7.0/tests/examples_test/morphologies/
+-rw-r--r--   0 runner    (1001) docker     (123)  1255757 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/C060114A5.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)   395836 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/C270106A.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)   589072 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/astrocyte.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10180 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/circle_contour.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/complexe.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/disconnected_neurite.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      275 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/iterators.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      315 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/mono-type.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/multiple_point_section.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/multiple_soma.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/nested_single_children.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      271 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/neurite_wrong_root_point.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)   107856 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/nrn-order-already-sorted.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165400 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/nrn_ordering.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/pia.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/reversed_NRN_neurite_order.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)   491711 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/rp100427-123_idC.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      609 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/sections-block.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/simple-with-font.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/simple-with-image-coord.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      548 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/simple.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      610 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/simple.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/simple2.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/soma_cylinders.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/soma_multiple_frustums.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/soma_single_frustum.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/soma_three_points_cylinder.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/spine.asc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/morphologies/three_point_soma.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/mouse_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/placement_rules.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57762 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/report_CurateDataset.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   130944 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/report_example.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/run_curation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/examples_test/transform_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24159 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/test_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/test_download_morphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19799 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/test_example_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-22 19:14:05.000000 morphology-workflows-0.7.0/tox.ini
```

### Comparing `morphology-workflows-0.6.1/.auto-changelog` & `morphology-workflows-0.7.0/.auto-changelog`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/.auto-changelog-template.hbs` & `morphology-workflows-0.7.0/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/.copier-answers.yml` & `morphology-workflows-0.7.0/.copier-answers.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.40
+_commit: 0.1.43
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
 copyright_license: Apache License 2.0
 copyright_year: '2022'
 distribution_name: morphology-workflows
 download_url: https://github.com/BlueBrain/morphology-workflows
```

### Comparing `morphology-workflows-0.6.1/.gitignore` & `morphology-workflows-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/.pre-commit-config.yaml` & `morphology-workflows-0.7.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,30 @@
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
-    rev: v9.4.0
+    rev: v9.5.0
     hooks:
         - id: commitlint
           stages:
             - commit-msg
           additional_dependencies: ['conventional-changelog-conventionalcommits']
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-x", ".codespellignorelines"]
   - repo: https://github.com/PyCQA/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
```

### Comparing `morphology-workflows-0.6.1/.pylintrc` & `morphology-workflows-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/CHANGELOG.md` & `morphology-workflows-0.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## [0.7.0](https://github.com/BlueBrain/morphology-workflows/compare/0.6.1..0.7.0)
+
+> 22 May 2023
+
+### New Features
+
+- Change entry point from morphology_workflows to morphology-workflows (Adrien Berchet - [#98](https://github.com/BlueBrain/morphology-workflows/pull/98))
+
+### Fixes
+
+- Compatibility with Pandas&gt;=2 and urllib3&gt;=2 (Adrien Berchet - [#96](https://github.com/BlueBrain/morphology-workflows/pull/96))
+
+### Documentation Changes
+
+- Add link to the schema of the Repair params (Adrien Berchet - [#91](https://github.com/BlueBrain/morphology-workflows/pull/91))
+
+### General Changes
+
+- Fix layers not int (Alexis Arnaudon - [#92](https://github.com/BlueBrain/morphology-workflows/pull/92))
+- Use JSON schema from NeuroR.main.Repair and fix CLI command in docs (Adrien Berchet - [#90](https://github.com/BlueBrain/morphology-workflows/pull/90))
+
 ## [0.6.1](https://github.com/BlueBrain/morphology-workflows/compare/0.6.0..0.6.1)
 
 > 27 March 2023
 
 ### New Features
 
 - Update command and doc (Adrien Berchet - [#88](https://github.com/BlueBrain/morphology-workflows/pull/88))
```

### Comparing `morphology-workflows-0.6.1/CONTRIBUTING.md` & `morphology-workflows-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/LICENSE.txt` & `morphology-workflows-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/PKG-INFO` & `morphology-workflows-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphology-workflows
-Version: 0.6.1
+Version: 0.7.0
 Summary: Workflows used for morphology processing.
 Home-page: https://morphology-workflows.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/morphology-workflows/issues
 Project-URL: Source, https://github.com/BlueBrain/morphology-workflows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morphology-workflows-0.6.1/README.md` & `morphology-workflows-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/commitlint.config.js` & `morphology-workflows-0.7.0/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/docs/Makefile` & `morphology-workflows-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/docs/source/conf.py` & `morphology-workflows-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/docs/source/logo/BBP-Morphology-Workflows.jpg` & `morphology-workflows-0.7.0/docs/source/logo/BBP-Morphology-Workflows.jpg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/examples/logging.conf` & `morphology-workflows-0.7.0/src/morphology_workflows/_templates/logging.conf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/examples/luigi.cfg` & `morphology-workflows-0.7.0/examples/luigi.cfg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/package.json` & `morphology-workflows-0.7.0/package.json`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/pyproject.toml` & `morphology-workflows-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/setup.py` & `morphology-workflows-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     "luigi>=3.2",
     "luigi-tools>=0.3.3",
     "matplotlib>=3.4",
     "morphapi>=0.1.8",
     "morph_tool>=2.9.0,<3.0",
     "morphio>=3.1.1,<4.0",
     "neurom>=3.2.0,<4.0",
-    "neuror>=1.6,<2.0",
+    "neuror>=1.6.3,<2.0",
     "numpy>=1.21",
     "pandas>=1.5",
     "plotly-helper>=0.0.8,<1.0",
     "PyYAML>=5.3",
     "rst2pdf>=0.99",
     "scipy>=1.6",
     "tqdm>=4.44",
+    "urllib3>=1.26,<2; python_version < '3.9'",
 ]
 
 doc_reqs = [
     "graphviz",
     "m2r2",
     "sphinx-argparse",
     "sphinx-autoapi",
@@ -33,14 +34,15 @@
 ]
 
 test_reqs = [
     "diff-pdf-visually>=1.7",
     "dir-content-diff>=1.4",
     "mock>=3",
     "pytest>=6",
+    "pytest-console-scripts>=1.3",
     "pytest-cov>=3",
     "pytest-html>=2",
     "pytest-xdist>=2",
 ]
 
 setup(
     name="morphology-workflows",
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/_data/default_placeholders.csv` & `morphology-workflows-0.7.0/src/morphology_workflows/_data/default_placeholders.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/_templates/logging.conf` & `morphology-workflows-0.7.0/examples/logging.conf`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 class=StreamHandler
 formatter=PrettyFormatter
 args=(sys.stdout,)
 
 [handler_fileHandler]
 class=FileHandler
 formatter=PrettyFormatter
-args=('logs.log',)
+args=('logs.log', 'w')
 
 [formatter_PrettyFormatter]
 format=%(asctime)s - %(name)s - %(levelname)s - %(message)s
 datefmt=%Y-%m-%d %H:%M:%S
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/_templates/luigi.cfg` & `morphology-workflows-0.7.0/src/morphology_workflows/_templates/luigi.cfg`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/_templates/source_report/conf.py` & `morphology-workflows-0.7.0/src/morphology_workflows/_templates/source_report/conf.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/annotation.py` & `morphology-workflows-0.7.0/src/morphology_workflows/annotation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/curation.py` & `morphology-workflows-0.7.0/src/morphology_workflows/curation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/marker_helper.py` & `morphology-workflows-0.7.0/src/morphology_workflows/marker_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 
         plot_data = vector(_get_lim(1), _get_lim(-1), name=f"{marker.label}", **marker.plot_style)
         builder.helper.add_data({f"{marker.label}": plot_data})
 
     def plot(self, filename="markers.html", with_plotly=True, plane="3d", **kwargs):
         """Plot morphology with markers."""
         if with_plotly:
-
             neuron = load_morphology(self.morph_path)
             builder = NeuronBuilder(neuron, plane, line_width=4, title=f"{self.morph_name}")
 
             if "auto_open" not in kwargs:
                 kwargs["auto_open"] = False
 
             for marker in self.markers:
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/placeholders.py` & `morphology-workflows-0.7.0/src/morphology_workflows/placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/repair.py` & `morphology-workflows-0.7.0/src/morphology_workflows/repair.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from morph_tool.converter import convert
 from morph_tool.exceptions import MorphToolException
 from morph_tool.morphdb import MorphDB
 from morph_tool.morphdb import MorphInfo
 from morphio.mut import Morphology
 from neurom import load_morphology
 from neurom import view
-from neuror.main import RepairType
 from neuror.main import repair as _repair
 from neuror.unravel import unravel as _unravel
+from neuror.utils import RepairType
 from neuror.zero_diameter_fixer import fix_zero_diameters as _fix_zero_diameters
 from scipy.spatial import KDTree
 from tqdm import tqdm
 
 from morphology_workflows import MorphologyWorkflowsError
 from morphology_workflows.marker_helper import MarkerSet
 from morphology_workflows.utils import silent_loggers
@@ -327,15 +327,15 @@
 
 def _create_db_row(_data, zero_diameter_path, unravel_path, repair_path, extension):
     """Create a db row and convert morphology."""
     index, data = _data
     m = MorphInfo(
         name=data["morph_name"],
         mtype=data["mtype"] if isinstance(data["mtype"], str) else "",
-        layer=int(data["layer"]),
+        layer=data["layer"],
         use_dendrite=data["has_basal"],
         use_axon=data["has_axon"],
     )
 
     if zero_diameter_path is not None:
         zero_diameter_release_path = (
             str(zero_diameter_path / Path(data["zero_diameter_morph_path"]).stem) + extension
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/annotation.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/annotation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/cli.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,19 @@
         return self.parsers["root"]
 
     def _get_parsers(self):
         """Return the main argument parser."""
         parser = argparse.ArgumentParser(
             description="Run the workflow",
         )
+        parser.add_argument(
+            "--version",
+            action="version",
+            version=f"%(prog)s, version {morphology_workflows.__version__}",
+        )
 
         parser.add_argument("-c", "--config-path", help="Path to the Luigi config file.")
 
         parser.add_argument(
             "-m",
             "--master-scheduler",
             default=False,
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/curation.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/curation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/fetch.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/fetch.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/placeholders.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/repair.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/repair.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Repair tasks."""
+import copy
 import logging
 
 import luigi
 from data_validation_framework.task import ElementValidationTask
 from data_validation_framework.task import SetValidationTask
 from data_validation_framework.task import SkippableMixin
 from luigi_tools.parameter import BoolParameter
+from neuror.main import _PARAM_SCHEMA
 
 from morphology_workflows.curation import collect
 from morphology_workflows.repair import fix_zero_diameters
 from morphology_workflows.repair import make_collage
 from morphology_workflows.repair import make_release
 from morphology_workflows.repair import plot_repair
 from morphology_workflows.repair import plot_smooth_diameters
 from morphology_workflows.repair import repair
 from morphology_workflows.repair import smooth_diameters
 from morphology_workflows.repair import unravel
 from morphology_workflows.utils import StrIndexMixin
 
 logger = logging.getLogger(__name__)
 
+_REPAIR_SCHEMA = copy.deepcopy(_PARAM_SCHEMA)
+_REPAIR_SCHEMA["required"] = []  # Here the parameters can be partially filled
+
 
 class CollectAnnotated(StrIndexMixin, ElementValidationTask):
     """Collect annotated dataset to work with on this phase."""
 
     output_columns = {
         "morph_path": None,
         "has_apical": None,
@@ -98,15 +103,20 @@
 
     output_columns = {"morph_path": None}
     validation_function = repair
     with_plot = BoolParameter(
         default=False, description=":bool: Save plots with highlighted repaired branches"
     )
     repair_params = luigi.OptionalDictParameter(
-        default=None, description=":dict: Repair internal parameters"
+        default=None,
+        description=(
+            ":dict: Repair internal parameters (see details in "
+            "https://neuror.readthedocs.io/en/stable/neuror.main.html#neuror.main.Repair)"
+        ),
+        schema=_REPAIR_SCHEMA,
     )
 
     def kwargs(self):
         return {"with_plot": self.with_plot, "repair_params": self.repair_params}
 
     def inputs(self):
         return {
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/tasks/workflows.py` & `morphology-workflows-0.7.0/src/morphology_workflows/tasks/workflows.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows/utils.py` & `morphology-workflows-0.7.0/src/morphology_workflows/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     output_path = Path(output_path)
     morph_files = []
 
     for i in dir_path.iterdir():
         if i.suffix.lower() in EXTS:
             morph_files.append((i.with_suffix("").name, str(i)))
         else:
-            L.info("The file '%s' is not a valid morphology and is thus discarded", i)
+            L.info("The file '%s' is not detected as a morphology file and is thus discarded", i)
     df = pd.DataFrame(morph_files, columns=["morph_name", "morph_path"])
 
     # Deduplicate names
-    for idx, name in df.loc[df["morph_name"].duplicated(), "morph_name"].iteritems():
+    for idx, name in df.loc[df["morph_name"].duplicated(), "morph_name"].items():
         i = 2
         new_name = name + f"_{i}"
         while (df["morph_name"] == new_name).any():
             i += 1
             new_name = name + f"_{i}"
         df.loc[idx, "morph_name"] = new_name
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows.egg-info/PKG-INFO` & `morphology-workflows-0.7.0/src/morphology_workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphology-workflows
-Version: 0.6.1
+Version: 0.7.0
 Summary: Workflows used for morphology processing.
 Home-page: https://morphology-workflows.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/morphology-workflows/issues
 Project-URL: Source, https://github.com/BlueBrain/morphology-workflows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows.egg-info/SOURCES.txt` & `morphology-workflows-0.7.0/src/morphology_workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/src/morphology_workflows.egg-info/requires.txt` & `morphology-workflows-0.7.0/src/morphology_workflows.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 luigi>=3.2
 luigi-tools>=0.3.3
 matplotlib>=3.4
 morphapi>=0.1.8
 morph_tool<3.0,>=2.9.0
 morphio<4.0,>=3.1.1
 neurom<4.0,>=3.2.0
-neuror<2.0,>=1.6
+neuror<2.0,>=1.6.3
 numpy>=1.21
 pandas>=1.5
 plotly-helper<1.0,>=0.0.8
 PyYAML>=5.3
 rst2pdf>=0.99
 scipy>=1.6
 tqdm>=4.44
 
+[:python_version < "3.9"]
+urllib3<2,>=1.26
+
 [allen_brain]
 allensdk>=2.13.5
 
 [docs]
 graphviz
 m2r2
 sphinx-argparse
@@ -30,10 +33,11 @@
 bg_atlasapi
 
 [test]
 diff-pdf-visually>=1.7
 dir-content-diff>=1.4
 mock>=3
 pytest>=6
+pytest-console-scripts>=1.3
 pytest-cov>=3
 pytest-html>=2
 pytest-xdist>=2
```

### Comparing `morphology-workflows-0.6.1/tests/__init__.py` & `morphology-workflows-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/conftest.py` & `morphology-workflows-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/placeholders.csv` & `morphology-workflows-0.7.0/tests/data/placeholders.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/Annotate/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/Annotate/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/ApicalPoint/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CollectCurated/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CollectCurated/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/CutLeaves/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/CutLeaves/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/HardLimit/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/HardLimit/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/MType/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/MType/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotApicalPoint/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotCutLeaves/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/PlotHardLimit/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_annotated/annotated_dataset.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_annotated/annotated_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Align/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Align/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/CheckNeurites/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/CheckNeurites/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Collect/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Collect/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Curate/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Curate/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/DetectErrors/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/DetectErrors/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/EnsureNeuritesOutsideSoma/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/ExtractMarkers/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Orient/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Orient/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotErrors/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotErrors/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMarkers/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMarkers/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/PlotMorphologies/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Recenter/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Recenter/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/Sanitize/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/Sanitize/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_curated/curated_dataset.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_curated/curated_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/CollectAnnotated/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/FixZeroDiameters/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeCollage/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeCollage/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/MakeRelease/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/MakeRelease/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/PlotRepair/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/PlotRepair/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Repair/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Repair/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/RepairNeurites/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/Unravel/report.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/Unravel/report.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/out_repaired/repaired_dataset.csv` & `morphology-workflows-0.7.0/tests/data/test_example_1/out_repaired/repaired_dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-asc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-h5/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/repair_release-swc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/repair_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-asc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-h5/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/unravel_release-swc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/unravel_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-asc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-h5/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml` & `morphology-workflows-0.7.0/tests/data/test_example_1/zero_diameter_release-swc/neurondb.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_report/report_latexpdf.pdf` & `morphology-workflows-0.7.0/tests/data/test_report/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_report/report_no_exception_rst2pdf.pdf` & `morphology-workflows-0.7.0/tests/data/test_report/report_no_exception_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_report/report_rst2pdf.pdf` & `morphology-workflows-0.7.0/tests/data/test_report/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_report_before_run/report_latexpdf.pdf` & `morphology-workflows-0.7.0/tests/data/test_report_before_run/report_latexpdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/data/test_report_before_run/report_rst2pdf.pdf` & `morphology-workflows-0.7.0/tests/data/test_report_before_run/report_rst2pdf.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/builder_recipe.xml` & `morphology-workflows-0.7.0/tests/examples_test/builder_recipe.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/dataset.csv` & `morphology-workflows-0.7.0/tests/examples_test/dataset.csv`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/C060114A5.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/C060114A5.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/C270106A.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/C270106A.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/README` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/README`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/astrocyte.h5` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/astrocyte.h5`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/circle_contour.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/circle_contour.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/complexe.swc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/complexe.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/nrn-order-already-sorted.h5` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/nrn-order-already-sorted.h5`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/nrn_ordering.swc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/nrn_ordering.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/pia.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/pia.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/rp100427-123_idC.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/rp100427-123_idC.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/sections-block.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/sections-block.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/simple-with-image-coord.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/simple-with-image-coord.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/simple.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/simple.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/simple.swc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/simple.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/spine.asc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/spine.asc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/morphologies/three_point_soma.swc` & `morphology-workflows-0.7.0/tests/examples_test/morphologies/three_point_soma.swc`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/placement_rules.xml` & `morphology-workflows-0.7.0/tests/examples_test/placement_rules.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/report_CurateDataset.pdf` & `morphology-workflows-0.7.0/tests/examples_test/report_CurateDataset.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/report_example.pdf` & `morphology-workflows-0.7.0/tests/examples_test/report_example.pdf`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/examples_test/transform_rules.xml` & `morphology-workflows-0.7.0/tests/examples_test/transform_rules.xml`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/test_cli.py` & `morphology-workflows-0.7.0/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,7 +37,15 @@
                 "--config-file",
                 str(output_path),
             ]
         )
 
         assert output_path.exists()
         assert (tmpdir / "dependency_graph.png").exists()
+
+
+def test_entry_point(script_runner):
+    """Test the entry point."""
+    ret = script_runner.run("morphology-workflows", "--version")
+    assert ret.success
+    assert ret.stdout.startswith("morphology-workflows, version ")
+    assert ret.stderr == ""
```

### Comparing `morphology-workflows-0.6.1/tests/test_curation.py` & `morphology-workflows-0.7.0/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/test_download_morphs.py` & `morphology-workflows-0.7.0/tests/test_download_morphs.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tests/test_example_1.py` & `morphology-workflows-0.7.0/tests/test_example_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Test the complete workflow on the example."""
 # pylint: disable=redefined-outer-name
 import shutil
 
 import luigi
 import numpy as np
+import pandas as pd
 import pytest
 from dir_content_diff import assert_equal_trees
 from dir_content_diff import compare_files
 from dir_content_diff.base_comparators import IniComparator
 from dir_content_diff.base_comparators import JsonComparator
 
 from morphology_workflows.tasks import cli
 from morphology_workflows.tasks import workflows
+from morphology_workflows.utils import EXTS
 
 from . import clean_exception
 
 
 @pytest.fixture()
 def example_1(tmp_working_dir, examples_test_dir):
     """Setup the working directory."""
@@ -469,7 +471,32 @@
         IniComparator(),
     )
     compare_files(
         tmp_working_dir / f"{db_source.lower()}_config.json",
         examples_dir / f"{db_source.lower()}_config.json",
         JsonComparator(),
     )
+
+
+def test_initialize_from_dir(tmp_working_dir, examples_dir, examples_test_dir):
+    """Test that the example is the same as the one generated by the Initialize workflow."""
+    cli.main(["Initialize", "--input-dir", str(examples_test_dir / "morphologies")])
+
+    assert (tmp_working_dir / "logging.conf").exists()
+    assert (tmp_working_dir / "luigi.cfg").exists()
+
+    compare_files(
+        tmp_working_dir / "logging.conf",
+        examples_dir / "logging.conf",
+        IniComparator(),
+    )
+    compare_files(
+        tmp_working_dir / "luigi.cfg",
+        examples_dir / "luigi.cfg",
+        IniComparator(),
+    )
+
+    res = pd.read_csv(tmp_working_dir / "dataset.csv")
+    assert len(res) == len(
+        [i for i in (examples_test_dir / "morphologies").iterdir() if i.suffix.lower() in EXTS]
+    )
+    assert res.columns.tolist() == ["morph_name", "morph_path"]
```

### Comparing `morphology-workflows-0.6.1/tests/test_placeholders.py` & `morphology-workflows-0.7.0/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `morphology-workflows-0.6.1/tox.ini` & `morphology-workflows-0.7.0/tox.ini`

 * *Files identical despite different names*

