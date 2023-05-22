# Comparing `tmp/img2table-0.1.3.tar.gz` & `tmp/img2table-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.1.3.tar", last modified: Tue May  9 22:41:48 2023, max compression
+gzip compressed data, was "dist/img2table-0.1.4.tar", last modified: Mon May 22 19:44:18 2023, max compression
```

## Comparing `img2table-0.1.3.tar` & `img2table-0.1.4.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 22:39:27.000000 img2table-0.1.3/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-09 22:39:27.000000 img2table-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-09 22:39:27.000000 img2table-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-09 22:41:48.000000 img2table-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-09 22:39:27.000000 img2table-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-09 22:39:27.000000 img2table-0.1.3/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46047 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-09 22:39:27.000000 img2table-0.1.3/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 22:39:27.000000 img2table-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 22:39:27.000000 img2table-0.1.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 22:39:27.000000 img2table-0.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 22:39:27.000000 img2table-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 22:41:48.000000 img2table-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 22:39:27.000000 img2table-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-09 22:39:27.000000 img2table-0.1.3/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 22:41:47.000000 img2table-0.1.3/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-09 22:39:27.000000 img2table-0.1.3/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:41:48.000000 img2table-0.1.3/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-09 22:39:28.000000 img2table-0.1.3/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 19:41:35.000000 img2table-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-22 19:41:35.000000 img2table-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-22 19:44:18.000000 img2table-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-22 19:41:35.000000 img2table-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-22 19:41:35.000000 img2table-0.1.4/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46047 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 19:41:35.000000 img2table-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 19:41:35.000000 img2table-0.1.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 19:41:35.000000 img2table-0.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 19:41:35.000000 img2table-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-22 19:44:18.000000 img2table-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 19:41:35.000000 img2table-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.1.3/LICENSE.txt` & `img2table-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/Makefile` & `img2table-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/PKG-INFO` & `img2table-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.3
+Version: 0.1.4
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -109,23 +109,27 @@
         methods might not correspond to the original image.
         
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
-        pdf = PDF(src, pages=[0, 2])
+        pdf = PDF(src, 
+                  pages=[0, 2],
+                  detect_rotation=False)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
+        >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
+        >    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
         ></dl>
         
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
@@ -405,14 +409,19 @@
         The library is tailored for usage on documents with white/light background. 
         Effectiveness can not be guaranteed on other type of documents. 
         </li>
         <li>
         Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
         Improvements to the algorithm will be released in future versions.
         </li>
+        <li>
+        Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
+        you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
+        the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
+        </li>
         </ul>
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.3 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.4 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -51,15 +51,16 @@
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
+img2table.document import PDF pdf = PDF(src, pages=[0, 2],
+detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -164,12 +165,15 @@
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
     * Borderless tables extraction is still in alpha stage and might be
       inconsistent on complex cases. Improvements to the algorithm will be
       released in future versions.
+    * Table detection using only OpenCV processing can have some limitations.
+      If the library fails to detect tables, you may check CNN based solutions
+      like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
 Provides-Extra: paddle Provides-Extra: paddle_gpu
```

### Comparing `img2table-0.1.3/README.md` & `img2table-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,27 @@
 methods might not correspond to the original image.
 
 #### PDF <a name="pdf-doc"></a>
 PDF files are instantiated as follows :
 ```python
 from img2table.document import PDF
 
-pdf = PDF(src, pages=[0, 2])
+pdf = PDF(src, 
+          pages=[0, 2],
+          detect_rotation=False)
 ```
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
 >    <dd style="font-style: italic;">PDF source</dd>
 >    <dt>pages : list, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
+>    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
+>    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
 ></dl>
 
 PDF pages are converted to images with a 200 DPI for table identification.
 
 ---
 
 ### OCR <a name="ocr"></a>
@@ -398,8 +402,13 @@
 The library is tailored for usage on documents with white/light background. 
 Effectiveness can not be guaranteed on other type of documents. 
 </li>
 <li>
 Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
 Improvements to the algorithm will be released in future versions.
 </li>
+<li>
+Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
+you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
+the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
+</li>
 </ul>
```

#### html2text {}

```diff
@@ -47,15 +47,16 @@
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
+img2table.document import PDF pdf = PDF(src, pages=[0, 2],
+detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -160,7 +161,10 @@
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
     * Borderless tables extraction is still in alpha stage and might be
       inconsistent on complex cases. Improvements to the algorithm will be
       released in future versions.
+    * Table detection using only OpenCV processing can have some limitations.
+      If the library fails to detect tables, you may check CNN based solutions
+      like CascadeTabNet or the PaddleOCR_implementation.
```

### Comparing `img2table-0.1.3/examples/Basic_usage.ipynb` & `img2table-0.1.4/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/Implicit_rows.ipynb` & `img2table-0.1.4/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/borderless.ipynb` & `img2table-0.1.4/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/borderless_aws.jpg` & `img2table-0.1.4/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/borderless_ocr.jpg` & `img2table-0.1.4/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/implicit.png` & `img2table-0.1.4/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/tables.pdf` & `img2table-0.1.4/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/tables.png` & `img2table-0.1.4/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/examples/data/tables.xlsx` & `img2table-0.1.4/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/setup.cfg` & `img2table-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/__init__.py` & `img2table-0.1.4/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/document/base/__init__.py` & `img2table-0.1.4/src/img2table/document/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     src: Union[str, Path, io.BytesIO, bytes]
 
     def validate_src(self, value, **_) -> Union[str, Path, io.BytesIO, bytes]:
         if not isinstance(value, (str, Path, io.BytesIO, bytes)):
             raise TypeError(f"Invalid type {type(value)} for src argument")
         return value
 
-    def validate_dpi(self, value, **_) -> int:
-        if not isinstance(value, int):
-            raise TypeError(f"Invalid type {type(value)} for dpi argument")
+    def validate_detect_rotation(self, value, **_) -> int:
+        if not isinstance(value, bool):
+            raise TypeError(f"Invalid type {type(value)} for detect_rotation argument")
         return value
 
     def __post_init__(self):
         super(Document, self).__post_init__()
         # Initialize ocr_df
         self.ocr_df = None
```

### Comparing `img2table-0.1.3/src/img2table/document/base/rotation.py` & `img2table-0.1.4/src/img2table/document/base/rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,19 +91,21 @@
                           .count()
                           .sort(by=['count', pl.col('angle').abs()], descending=[True, False])
                           .limit(n_max)
                           .collect(streaming=True)
                           .to_dicts()
                           )
 
-    if most_likely_angles[0].get('angle') == 0:
-        return [0]
-    else:
-        return sorted(list(set([angle.get('angle') for angle in most_likely_angles
-                                if angle.get('count') >= 0.25 * max([a.get('count') for a in most_likely_angles])])))
+    if most_likely_angles:
+        if most_likely_angles[0].get('angle') == 0:
+            return [0]
+        else:
+            return sorted(list(set([angle.get('angle') for angle in most_likely_angles
+                                    if angle.get('count') >= 0.25 * max([a.get('count') for a in most_likely_angles])])))
+    return [0]
 
 
 def angle_dixon_q_test(angles: List[float], confidence: float = 0.9) -> float:
     """
     Compute best angle according to Dixon Q test
     :param angles: list of possible angles
     :param confidence: confidence level for outliers (0.9, 0.95, 0.99)
```

### Comparing `img2table-0.1.3/src/img2table/document/image.py` & `img2table-0.1.4/src/img2table/document/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 from img2table.tables.objects.extraction import ExtractedTable
 
 
 @dataclass
 class Image(Document):
     detect_rotation: bool = False
 
-    def validate_detect_rotation(self, value, **_) -> int:
-        if not isinstance(value, bool):
-            raise TypeError(f"Invalid type {type(value)} for detect_rotation argument")
-        return value
-
     def __post_init__(self):
         self.pages = None
 
         super(Image, self).__post_init__()
 
     @cached_property
     def images(self) -> List[np.ndarray]:
```

### Comparing `img2table-0.1.3/src/img2table/document/pdf.py` & `img2table-0.1.4/src/img2table/document/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # coding: utf-8
 from dataclasses import dataclass
+
+from img2table.document.base.rotation import fix_rotation_image
+
 try:
     from functools import cached_property
 except ImportError:
     from cached_property import cached_property
 from typing import Dict, List, Optional
 
 import cv2
@@ -14,14 +17,15 @@
 from img2table.ocr.pdf import PdfOCR
 from img2table.tables.objects.extraction import ExtractedTable
 
 
 @dataclass
 class PDF(Document):
     pages: List[int] = None
+    detect_rotation: bool = False
 
     def validate_pages(self, value, **_) -> Optional[List[int]]:
         if value is not None:
             if not isinstance(value, list):
                 raise TypeError(f"Invalid type {type(value)} for pages argument")
             if not all(isinstance(x, int) for x in value):
                 raise TypeError("All values in pages argument should be integers")
@@ -37,28 +41,33 @@
 
         # Get all images
         images = list()
         for page_number in self.pages or range(doc.page_count):
             page = doc.load_page(page_id=page_number)
             pix = page.get_pixmap(matrix=mat)
             img = np.frombuffer(buffer=pix.samples, dtype=np.uint8).reshape((pix.height, pix.width, 3))
-            images.append(cv2.cvtColor(img, cv2.COLOR_BGR2GRAY))
+            # To grayscale
+            gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+            # Handle rotation if needed
+            final = fix_rotation_image(img=gray) if self.detect_rotation else gray
+            images.append(final)
 
         return images
 
     def extract_tables(self, ocr: "OCRInstance" = None, implicit_rows: bool = False, borderless_tables: bool = False,
                        min_confidence: int = 50) -> Dict[int, List[ExtractedTable]]:
         """
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :param min_confidence: minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)
         :return: dictionary with page number as key and list of extracted tables as values
         """
-        # Try to get OCRDataframe from PDF
-        self.ocr_df = PdfOCR().of(document=self)
+        if not self.detect_rotation:
+            # Try to get OCRDataframe from PDF
+            self.ocr_df = PdfOCR().of(document=self)
 
         return super().extract_tables(ocr=ocr,
                                       implicit_rows=implicit_rows,
                                       borderless_tables=borderless_tables,
                                       min_confidence=min_confidence)
```

### Comparing `img2table-0.1.3/src/img2table/ocr/aws_textract.py` & `img2table-0.1.4/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/azure.py` & `img2table-0.1.4/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/base.py` & `img2table-0.1.4/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/data.py` & `img2table-0.1.4/src/img2table/ocr/data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/google_vision.py` & `img2table-0.1.4/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/paddle.py` & `img2table-0.1.4/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/pdf.py` & `img2table-0.1.4/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/ocr/tesseract.py` & `img2table-0.1.4/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/image.py` & `img2table-0.1.4/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/metrics.py` & `img2table-0.1.4/src/img2table/tables/metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/objects/__init__.py` & `img2table-0.1.4/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/objects/extraction.py` & `img2table-0.1.4/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/objects/line.py` & `img2table-0.1.4/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/objects/row.py` & `img2table-0.1.4/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/objects/table.py` & `img2table-0.1.4/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/common.py` & `img2table-0.1.4/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/prepare_image.py` & `img2table-0.1.4/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table/tables/processing/text/titles.py` & `img2table-0.1.4/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/src/img2table.egg-info/PKG-INFO` & `img2table-0.1.4/src/img2table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.3
+Version: 0.1.4
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -109,23 +109,27 @@
         methods might not correspond to the original image.
         
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
-        pdf = PDF(src, pages=[0, 2])
+        pdf = PDF(src, 
+                  pages=[0, 2],
+                  detect_rotation=False)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
+        >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
+        >    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
         ></dl>
         
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
@@ -405,14 +409,19 @@
         The library is tailored for usage on documents with white/light background. 
         Effectiveness can not be guaranteed on other type of documents. 
         </li>
         <li>
         Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
         Improvements to the algorithm will be released in future versions.
         </li>
+        <li>
+        Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
+        you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
+        the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
+        </li>
         </ul>
         
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.3 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.1.4 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -51,15 +51,16 @@
 >
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
-img2table.document import PDF pdf = PDF(src, pages=[0, 2]) ``` >
+img2table.document import PDF pdf = PDF(src, pages=[0, 2],
+detect_rotation=False) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -164,12 +165,15 @@
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
     * Borderless tables extraction is still in alpha stage and might be
       inconsistent on complex cases. Improvements to the algorithm will be
       released in future versions.
+    * Table detection using only OpenCV processing can have some limitations.
+      If the library fails to detect tables, you may check CNN based solutions
+      like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
 Provides-Extra: paddle Provides-Extra: paddle_gpu
```

### Comparing `img2table-0.1.3/src/img2table.egg-info/SOURCES.txt` & `img2table-0.1.4/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/_mock_data/azure.pkl` & `img2table-0.1.4/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/_mock_data/tesseract_hocr.html` & `img2table-0.1.4/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/_mock_data/textract.json` & `img2table-0.1.4/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/_mock_data/vision.json` & `img2table-0.1.4/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/_mock_data/vision.pkl` & `img2table-0.1.4/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/conftest.py` & `img2table-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/base/test_data/test.png` & `img2table-0.1.4/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/base/test_rotation.py` & `img2table-0.1.4/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/image/test_data/blank.png` & `img2table-0.1.4/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/image/test_data/dark.png` & `img2table-0.1.4/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/image/test_data/expected.xlsx` & `img2table-0.1.4/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/image/test_data/test.png` & `img2table-0.1.4/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/image/test_image.py` & `img2table-0.1.4/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/pdf/test_data/test.pdf` & `img2table-0.1.4/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/document/pdf/test_pdf.py` & `img2table-0.1.4/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.1.4/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.1.4/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.1.4/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/azure/test_azure.py` & `img2table-0.1.4/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/azure/test_data/test.png` & `img2table-0.1.4/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/data/test_data/expected_table.json` & `img2table-0.1.4/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/data/test_ocr_data.py` & `img2table-0.1.4/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.1.4/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/google_vision/test_data/test.png` & `img2table-0.1.4/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.1.4/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.1.4/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/paddle/test_data/test.png` & `img2table-0.1.4/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/paddle/test_paddle.py` & `img2table-0.1.4/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/pdf/test_data/content.json` & `img2table-0.1.4/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.1.4/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.1.4/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.1.4/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/tesseract/test_data/test.png` & `img2table-0.1.4/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.1.4/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/image/test_data/blank.png` & `img2table-0.1.4/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/image/test_data/ocr.csv` & `img2table-0.1.4/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/image/test_data/test.png` & `img2table-0.1.4/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/image/test_image.py` & `img2table-0.1.4/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/image/test_metrics.py` & `img2table-0.1.4/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_data/expected_tables.json` & `img2table-0.1.4/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_data/ocr.csv` & `img2table-0.1.4/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_data/tables.json` & `img2table-0.1.4/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_extraction.py` & `img2table-0.1.4/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_line.py` & `img2table-0.1.4/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_row.py` & `img2table-0.1.4/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/objects/test_table.py` & `img2table-0.1.4/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/common/test_common.py` & `img2table-0.1.4/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.1.4/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.1.4/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.1.4/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/text/test_data/table.json` & `img2table-0.1.4/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.1.4/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.3/tests/tables/processing/text/test_titles.py` & `img2table-0.1.4/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

