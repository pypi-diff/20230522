# Comparing `tmp/spatialdata-0.0.7.tar.gz` & `tmp/spatialdata-0.0.8.tar.gz`

## Comparing `spatialdata-0.0.7.tar` & `spatialdata-0.0.8.tar`

### file list

```diff
@@ -1,107 +1,106 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.bumpversion.cfg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.gitmodules
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.mypy.ini
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.7/_version.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/codecov.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/Makefile
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/changelog.md
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/conf.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/contributing.md
--rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/design_doc.md
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/index.md
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/installation.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/.gitkeep
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/css/custom.css
--rw-r--r--   0        0        0    51748 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/img/spatialdata_horizontal.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/function.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/__main__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_compat.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_logging.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_types.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_utils.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/__init__.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/concatenate.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/data_extent.py
--rw-r--r--   0        0        0    62038 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/spatialdata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/__init__.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/aggregate.py
--rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/rasterize.py
--rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/__init__.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/_utils.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/relational_query.py
--rw-r--r--   0        0        0    29788 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/spatial_query.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/__init__.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/_utils.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/format.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_points.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_raster.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_shapes.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_table.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_zarr.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/dataloader/__init__.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/dataloader/datasets.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/__init__.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/_utils.py
--rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/models.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/_utils.py
--rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/operations.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/_utils.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
--rw-r--r--   0        0        0    48233 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_aggregations.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_rasterize.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_spatialdata_operations.py
--rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/query/__init__.py
--rw-r--r--   0        0        0    21090 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/query/test_spatial_query.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/multipolygon.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/points.json
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/polygon.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/test_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/datasets/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/datasets/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_format.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_readwrite.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/models/__init__.py
--rw-r--r--   0        0        0    14739 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/models/test_models.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/test_dataloader/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/__init__.py
--rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/test_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/conftest.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/test_ngff_coordinate_system.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/test_ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/utils/__init__.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/utils/test_element_utils.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.7/LICENSE
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 spatialdata-0.0.7/README.md
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 spatialdata-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 spatialdata-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.bumpversion.cfg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.gitmodules
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.mypy.ini
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.8/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/Makefile
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/changelog.md
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/conf.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/contributing.md
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/design_doc.md
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/index.md
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/installation.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    51748 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_static/img/spatialdata_horizontal.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.8/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/__main__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_compat.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_logging.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_types.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_utils.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/__init__.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/concatenate.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/data_extent.py
+-rw-r--r--   0        0        0    62038 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/spatialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/__init__.py
+-rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/aggregate.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/rasterize.py
+-rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/operations/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/_utils.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/relational_query.py
+-rw-r--r--   0        0        0    30119 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_core/query/spatial_query.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/__init__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/_utils.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/format.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_points.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_raster.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_shapes.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_table.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/_io/io_zarr.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/dataloader/__init__.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/dataloader/datasets.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/__init__.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/_utils.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/models/models.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/_utils.py
+-rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/operations.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/_utils.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
+-rw-r--r--   0        0        0    48233 2020-02-02 00:00:00.000000 spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/__init__.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_aggregations.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_rasterize.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_spatialdata_operations.py
+-rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/operations/test_transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/query/__init__.py
+-rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/core/query/test_spatial_query.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/multipolygon.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/points.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/data/polygon.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/__init__.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/dataloader/test_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_format.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_readwrite.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/io/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/models/__init__.py
+-rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/models/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/__init__.py
+-rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/test_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/conftest.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/test_ngff_coordinate_system.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/transformations/ngff/test_ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.8/tests/utils/test_element_utils.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 spatialdata-0.0.8/README.md
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 spatialdata-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 spatialdata-0.0.8/PKG-INFO
```

### Comparing `spatialdata-0.0.7/.mypy.ini` & `spatialdata-0.0.8/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/.pre-commit-config.yaml` & `spatialdata-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/.github/workflows/build.yaml` & `spatialdata-0.0.8/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/.github/workflows/test_and_deploy.yaml` & `spatialdata-0.0.8/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/Makefile` & `spatialdata-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/api.md` & `spatialdata-0.0.8/docs/api.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/conf.py` & `spatialdata-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/contributing.md` & `spatialdata-0.0.8/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/design_doc.md` & `spatialdata-0.0.8/docs/design_doc.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/index.md` & `spatialdata-0.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/installation.md` & `spatialdata-0.0.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/references.bib` & `spatialdata-0.0.8/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/_static/css/custom.css` & `spatialdata-0.0.8/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/_static/img/spatialdata_horizontal.png` & `spatialdata-0.0.8/docs/_static/img/spatialdata_horizontal.png`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/_templates/autosummary/class.rst` & `spatialdata-0.0.8/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/docs/extensions/typed_returns.py` & `spatialdata-0.0.8/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/__init__.py` & `spatialdata-0.0.8/src/spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/__main__.py` & `spatialdata-0.0.8/src/spatialdata/__main__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_compat.py` & `spatialdata-0.0.8/src/spatialdata/_compat.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_logging.py` & `spatialdata-0.0.8/src/spatialdata/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_utils.py` & `spatialdata-0.0.8/src/spatialdata/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/datasets.py` & `spatialdata-0.0.8/src/spatialdata/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/concatenate.py` & `spatialdata-0.0.8/src/spatialdata/_core/concatenate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/data_extent.py` & `spatialdata-0.0.8/src/spatialdata/_core/data_extent.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/spatialdata.py` & `spatialdata-0.0.8/src/spatialdata/_core/spatialdata.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/operations/aggregate.py` & `spatialdata-0.0.8/src/spatialdata/_core/operations/aggregate.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from spatialdata.models import (
     Image2DModel,
     Labels2DModel,
     PointsModel,
     ShapesModel,
     get_model,
 )
-from spatialdata.models._utils import get_axes_names
 from spatialdata.transformations import BaseTransformation, Identity, get_transformation
 
 __all__ = ["aggregate"]
 
 
 def aggregate(
     values: ddf.DataFrame | gpd.GeoDataFrame | SpatialImage | MultiscaleSpatialImage,
@@ -108,28 +107,27 @@
     points: ddf.DataFrame | pd.DataFrame,
     shapes: gpd.GeoDataFrame,
     id_key: str | None = None,
     *,
     value_key: str | None = None,
     agg_func: str | list[str] = "count",
 ) -> ad.AnnData:
-    # Have to get dims on dask dataframe, can't get from pandas
-    dims = get_axes_names(points)
+    from spatialdata.models import points_dask_dataframe_to_geopandas
+
     # Default value for id_key
     if id_key is None:
         id_key = points.attrs[PointsModel.ATTRS_KEY][PointsModel.FEATURE_KEY]
         if id_key is None:
             raise ValueError(
                 "`FEATURE_KEY` is not specified for points, please pass `id_key` to the aggregation call, or specify "
                 "`FEATURE_KEY` for the points."
             )
 
-    if isinstance(points, ddf.DataFrame):
-        points = points.compute()
-    points = gpd.GeoDataFrame(points, geometry=gpd.points_from_xy(*[points[dim] for dim in dims]))
+    points = points_dask_dataframe_to_geopandas(points, suppress_z_warning=True)
+    shapes = circles_to_polygons(shapes)
 
     return _aggregate_shapes(points, shapes, id_key, value_key, agg_func)
 
 
 def _aggregate_shapes_by_shapes(
     values: gpd.GeoDataFrame,
     by: gpd.GeoDataFrame,
@@ -249,23 +247,27 @@
     to_agg = pd.DataFrame(
         {
             by_id_key: joined.index,
             id_key: joined[id_key].values,
             value_key: point_values,
         }
     )
+    ##
     aggregated = to_agg.groupby([by_id_key, id_key]).agg(agg_func).reset_index()
-    obs_id_categorical = pd.Categorical(aggregated[by_id_key])
+
+    # this is for only shapes in "by" that intersect with something in "value"
+    obs_id_categorical_categories = by.index.tolist()
+    obs_id_categorical = pd.Categorical(aggregated[by_id_key], categories=obs_id_categorical_categories)
 
     X = sparse.coo_matrix(
         (
             aggregated[value_key].values,
             (obs_id_categorical.codes, aggregated[id_key].cat.codes),
         ),
         shape=(len(obs_id_categorical.categories), len(joined[id_key].cat.categories)),
     ).tocsr()
     return ad.AnnData(
         X,
-        obs=pd.DataFrame(index=obs_id_categorical.categories),
+        obs=pd.DataFrame(index=pd.Categorical(obs_id_categorical_categories).categories),
         var=pd.DataFrame(index=joined[id_key].cat.categories),
         dtype=X.dtype,
     )
```

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/operations/rasterize.py` & `spatialdata-0.0.8/src/spatialdata/_core/operations/rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/operations/transform.py` & `spatialdata-0.0.8/src/spatialdata/_core/operations/transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/query/_utils.py` & `spatialdata-0.0.8/src/spatialdata/_core/query/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/query/relational_query.py` & `spatialdata-0.0.8/src/spatialdata/_core/query/relational_query.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_core/query/spatial_query.py` & `spatialdata-0.0.8/src/spatialdata/_core/query/spatial_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,20 +243,26 @@
     in_bounding_box_masks = da.stack(in_bounding_box_masks, axis=-1)
     return da.all(in_bounding_box_masks, axis=1)
 
 
 def _dict_query_dispatcher(
     elements: dict[str, SpatialElement], query_function: Callable[[SpatialElement], SpatialElement], **kwargs: Any
 ) -> dict[str, SpatialElement]:
+    from spatialdata.transformations import get_transformation
+
     queried_elements = {}
     for key, element in elements.items():
-        result = query_function(element, **kwargs)
-        if result is not None:
-            # query returns None if it is empty
-            queried_elements[key] = result
+        target_coordinate_system = kwargs["target_coordinate_system"]
+        d = get_transformation(element, get_all=True)
+        assert isinstance(d, dict)
+        if target_coordinate_system in d:
+            result = query_function(element, **kwargs)
+            if result is not None:
+                # query returns None if it is empty
+                queried_elements[key] = result
     return queried_elements
 
 
 @singledispatch
 def bounding_box_query(
     element: Union[SpatialElement, SpatialData],
     axes: tuple[str, ...],
@@ -645,20 +651,20 @@
             queried_shapes = ShapesModel.parse(queried_shapes)
             set_transformation(queried_shapes, transformation, target_coordinate_system)
             new_shapes[shapes_name] = queried_shapes
 
     new_points = {}
     if points:
         for points_name, p in sdata.points.items():
-            points_gdf = points_dask_dataframe_to_geopandas(p)
+            points_gdf = points_dask_dataframe_to_geopandas(p, suppress_z_warning=True)
             indices = points_gdf.geometry.intersects(polygon)
             if np.sum(indices) == 0:
                 raise ValueError("we expect at least one point")
             queried_points = points_gdf[indices]
-            ddf = points_geopandas_to_dask_dataframe(queried_points)
+            ddf = points_geopandas_to_dask_dataframe(queried_points, suppress_z_warning=True)
             transformation = get_transformation(p, target_coordinate_system)
             if "z" in ddf.columns:
                 ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y", "z": "z"})
             else:
                 ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y"})
             set_transformation(ddf, transformation, target_coordinate_system)
             new_points[points_name] = ddf
```

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/_utils.py` & `spatialdata-0.0.8/src/spatialdata/_io/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/format.py` & `spatialdata-0.0.8/src/spatialdata/_io/format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/io_points.py` & `spatialdata-0.0.8/src/spatialdata/_io/io_points.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,14 +50,26 @@
     fmt: Format = CurrentPointsFormat(),
 ) -> None:
     axes = get_axes_names(points)
     t = _get_transformations(points)
 
     points_groups = group.require_group(name)
     path = Path(points_groups._store.path) / points_groups.path / "points.parquet"
+
+    # The following code iterates through all columns in the 'points' DataFrame. If the column's datatype is
+    # 'category', it checks whether the categories of this column are known. If not, it explicitly converts the
+    # categories to known categories using 'c.cat.as_known()' and assigns the transformed Series back to the original
+    # DataFrame. This step is crucial when the number of categories exceeds 127, as pyarrow defaults to int8 for
+    # unknown categories which can only hold values from -128 to 127.
+    for column_name in points.columns:
+        c = points[column_name]
+        if c.dtype == "category" and not c.cat.known:
+            c = c.cat.as_known()
+            points[column_name] = c
+
     points.to_parquet(path)
 
     attrs = fmt.attrs_to_dict(points.attrs)
     attrs["version"] = fmt.version
 
     _write_metadata(
         points_groups,
```

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/io_raster.py` & `spatialdata-0.0.8/src/spatialdata/_io/io_raster.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/io_shapes.py` & `spatialdata-0.0.8/src/spatialdata/_io/io_shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/io_table.py` & `spatialdata-0.0.8/src/spatialdata/_io/io_table.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/_io/io_zarr.py` & `spatialdata-0.0.8/src/spatialdata/_io/io_zarr.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/dataloader/datasets.py` & `spatialdata-0.0.8/src/spatialdata/dataloader/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/models/__init__.py` & `spatialdata-0.0.8/src/spatialdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/models/_utils.py` & `spatialdata-0.0.8/src/spatialdata/models/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     for c in dims:
         if c not in (X, Y, Z, C):
             raise ValueError(f"Invalid dimension: {c}")
     if dims not in [(X,), (Y,), (Z,), (C,), (X, Y), (X, Y, Z), (Y, X), (Z, Y, X), (C, Y, X), (C, Z, Y, X)]:
         raise ValueError(f"Invalid dimensions: {dims}")
 
 
-def points_dask_dataframe_to_geopandas(points: DaskDataFrame) -> GeoDataFrame:
+def points_dask_dataframe_to_geopandas(points: DaskDataFrame, suppress_z_warning: bool = False) -> GeoDataFrame:
     """
     Convert a Dask DataFrame to a GeoDataFrame.
 
     Parameters
     ----------
     points
         Dask DataFrame with columns "x" and "y". Eventually, it can contain a column "z" that will be not included in
@@ -208,24 +208,33 @@
     Notes
     -----
     The "z" column is not included in the geometry column because it is not supported by GeoPandas.
     The resulting GeoDataFrame does not currenlty passes the validation of the SpatialData models. In fact currently
     points need to be saved as a Dask DataFrame. We will be restructuring the models to allow for GeoDataFrames soon.
 
     """
-    if "z" in points.columns:
+    from spatialdata.transformations import get_transformation, set_transformation
+
+    if "z" in points.columns and not suppress_z_warning:
         logger.warning("Constructing the GeoDataFrame without considering the z coordinate in the geometry.")
 
-    points_gdf = GeoDataFrame(geometry=geopandas.points_from_xy(points["x"], points["y"]))
-    for c in points.columns:
-        points_gdf[c] = points[c]
+    transformations = get_transformation(points, get_all=True)
+    assert isinstance(transformations, dict)
+    assert len(transformations) > 0
+    points = points.compute()
+    points_gdf = GeoDataFrame(points, geometry=geopandas.points_from_xy(points["x"], points["y"]))
+    points_gdf.reset_index(drop=True, inplace=True)
+    # keep the x and y either in the geometry either as columns: we don't duplicate because having this redundancy could
+    # lead to subtle bugs when coverting back to dask dataframes
+    points_gdf.drop(columns=["x", "y"], inplace=True)
+    set_transformation(points_gdf, transformations, set_all=True)
     return points_gdf
 
 
-def points_geopandas_to_dask_dataframe(gdf: GeoDataFrame) -> DaskDataFrame:
+def points_geopandas_to_dask_dataframe(gdf: GeoDataFrame, suppress_z_warning: bool = False) -> DaskDataFrame:
     """
     Convert a GeoDataFrame which represents 2D or 3D points to a Dask DataFrame that passes the schema validation.
 
     Parameters
     ----------
     gdf
         GeoDataFrame with a geometry column that contains 2D or 3D points.
@@ -237,20 +246,25 @@
     Notes
     -----
     The returned Dask DataFrame gets the 'x' and 'y' columns from the geometry column, and eventually the 'z' column
     (and the rest of the columns), from the remaining columns of the GeoDataFrame.
     """
     from spatialdata.models import PointsModel
 
+    # transformations are transferred automatically
     ddf = dd.from_pandas(gdf[gdf.columns.drop("geometry")], npartitions=1)
+    # we don't want redundancy in the columns since this could lead to subtle bugs when converting back to geopandas
+    assert "x" not in ddf.columns
+    assert "y" not in ddf.columns
     ddf["x"] = gdf.geometry.x
     ddf["y"] = gdf.geometry.y
     # parse
     if "z" in ddf.columns:
-        logger.warning(
-            "Constructing the Dask DataFrame using the x and y coordinates from the geometry and the z from an "
-            "additional column."
-        )
+        if not suppress_z_warning:
+            logger.warning(
+                "Constructing the Dask DataFrame using the x and y coordinates from the geometry and the z from an "
+                "additional column."
+            )
         ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y", "z": "z"})
     else:
         ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y"})
     return ddf
```

### Comparing `spatialdata-0.0.7/src/spatialdata/models/models.py` & `spatialdata-0.0.8/src/spatialdata/models/models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/__init__.py` & `spatialdata-0.0.8/src/spatialdata/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/_utils.py` & `spatialdata-0.0.8/src/spatialdata/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/operations.py` & `spatialdata-0.0.8/src/spatialdata/transformations/operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/transformations.py` & `spatialdata-0.0.8/src/spatialdata/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/ngff/_utils.py` & `spatialdata-0.0.8/src/spatialdata/transformations/ngff/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_coordinate_system.py` & `spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_transformations.py` & `spatialdata-0.0.8/src/spatialdata/transformations/ngff/ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/core/operations/test_aggregations.py` & `spatialdata-0.0.8/tests/core/operations/test_aggregations.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from anndata import AnnData
 from anndata.tests.helpers import assert_equal
 from numpy.random import default_rng
 from spatialdata import SpatialData
 from spatialdata._core.operations.aggregate import aggregate
 from spatialdata.models import Image2DModel, Labels2DModel, PointsModel, ShapesModel
 
+from tests.conftest import _make_sdata_for_testing_querying_and_aggretation
+
 RNG = default_rng(42)
 
 
 def test_aggregate_points_by_polygons() -> None:
     points = PointsModel.parse(
         pd.DataFrame(
             {
@@ -21,34 +23,63 @@
                 "y": [3.5, 4.8, 7.5, 4.0, 9.0, 5.5, 9.8],
                 "gene": list("aaabbbb"),
             }
         ),
         coordinates={"x": "x", "y": "y"},
         feature_key="gene",
     )
+    # shape_0 doesn't contain points, the other two shapes do
     shapes = ShapesModel.parse(
         gpd.GeoDataFrame(
             geometry=[
+                shapely.Polygon([(0.0, 10.0), (2.0, 10.0), (0.0, 9.0)]),
                 shapely.Polygon([(0.5, 7.0), (4.0, 2.0), (5.0, 8.0)]),
                 shapely.Polygon([(3.0, 8.0), (7.0, 2.0), (10.0, 6.0), (7.0, 10.0)]),
             ],
-            index=["shape_0", "shape_1"],
+            index=["shape_0", "shape_1", "shape_2"],
         )
     )
 
     result_adata = aggregate(points, shapes, "gene", agg_func="sum")
-    assert result_adata.obs_names.to_list() == ["shape_0", "shape_1"]
+    assert result_adata.obs_names.to_list() == ["shape_0", "shape_1", "shape_2"]
     assert result_adata.var_names.to_list() == ["a", "b"]
-    np.testing.assert_equal(result_adata.X.A, np.array([[2, 0], [1, 3]]))
+    np.testing.assert_equal(result_adata.X.A, np.array([[0, 0], [2, 0], [1, 3]]))
 
     # id_key can be implicit for points
     result_adata_implicit = aggregate(points, shapes, agg_func="sum")
     assert_equal(result_adata, result_adata_implicit)
 
 
+def test_aggregate_points_by_circles():
+    sdata = _make_sdata_for_testing_querying_and_aggretation()
+    # checks also that cound and sum behave the same for categorical variables
+    adata0 = aggregate(
+        values=sdata["points"],
+        by=sdata["by_circles"],
+        id_key="genes",
+        agg_func="count",
+        target_coordinate_system="global",
+    )
+    adata1 = aggregate(
+        values=sdata["points"],
+        by=sdata["by_circles"],
+        id_key="genes",
+        agg_func="sum",
+        target_coordinate_system="global",
+    )
+
+    assert adata0.var_names.tolist() == ["a", "b"]
+    assert adata1.var_names.tolist() == ["a", "b"]
+    X0 = adata0.X.todense()
+    X1 = adata1.X.todense()
+
+    assert np.all(np.matrix([[3, 3], [0, 0]]) == X0)
+    assert np.all(np.matrix([[3, 3], [0, 0]]) == X1)
+
+
 def test_aggregate_polygons_by_polygons() -> None:
     cellular = ShapesModel.parse(
         gpd.GeoDataFrame(
             geometry=[
                 shapely.Polygon([(0.5, 7.0), (4.0, 2.0), (5.0, 8.0)]),
                 shapely.Polygon([(3.0, 8.0), (7.0, 2.0), (10.0, 6.0), (7.0, 10.0)]),
             ],
@@ -119,10 +150,10 @@
     out = aggregate(image, labels, zone_ids=[1, 2, 3])
     assert len(out) == 3
 
 
 def test_aggregate_spatialdata(sdata_blobs: SpatialData) -> None:
     sdata = sdata_blobs.aggregate(sdata_blobs.points["blobs_points"], by="blobs_polygons")
     assert isinstance(sdata, SpatialData)
-    assert len(sdata.shapes["blobs_polygons"]) == 2
-    assert sdata.table.shape == (2, 2)
+    assert len(sdata.shapes["blobs_polygons"]) == 3
+    assert sdata.table.shape == (3, 2)
     assert len(sdata.points["points"].compute()) == 300
```

### Comparing `spatialdata-0.0.7/tests/core/operations/test_rasterize.py` & `spatialdata-0.0.8/tests/core/operations/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/core/operations/test_spatialdata_operations.py` & `spatialdata-0.0.8/tests/core/operations/test_spatialdata_operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/core/operations/test_transform.py` & `spatialdata-0.0.8/tests/core/operations/test_transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/core/query/test_spatial_query.py` & `spatialdata-0.0.8/tests/core/query/test_spatial_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from dataclasses import FrozenInstanceError
 
-import geopandas as gpd
 import numpy as np
-import pandas as pd
 import pytest
 from anndata import AnnData
-from dask.dataframe.core import DataFrame as DaskDataFrame
-from geopandas import GeoDataFrame
 from multiscale_spatial_image import MultiscaleSpatialImage
-from shapely import linearrings, polygons
 from spatial_image import SpatialImage
 from spatialdata import SpatialData
 from spatialdata._core.query.spatial_query import (
     BaseSpatialRequest,
     BoundingBoxRequest,
     bounding_box_query,
     polygon_query,
@@ -27,52 +22,18 @@
     TableModel,
 )
 from spatialdata.transformations.operations import (
     get_transformation,
     set_transformation,
 )
 
-
-def _make_points(coordinates: np.ndarray) -> DaskDataFrame:
-    """Helper function to make a Points element."""
-    k0 = int(len(coordinates) / 3)
-    k1 = len(coordinates) - k0
-    genes = np.hstack((np.repeat("a", k0), np.repeat("b", k1)))
-    return PointsModel.parse(coordinates, annotation=pd.DataFrame({"genes": genes}), feature_key="genes")
-
-
-def _make_squares(centroid_coordinates: np.ndarray, half_widths: list[float]) -> polygons:
-    linear_rings = []
-    for centroid, half_width in zip(centroid_coordinates, half_widths):
-        min_coords = centroid - half_width
-        max_coords = centroid + half_width
-
-        linear_rings.append(
-            linearrings(
-                [
-                    [min_coords[0], min_coords[1]],
-                    [min_coords[0], max_coords[1]],
-                    [max_coords[0], max_coords[1]],
-                    [max_coords[0], min_coords[1]],
-                ]
-            )
-        )
-    s = polygons(linear_rings)
-    polygon_series = gpd.GeoSeries(s)
-    cell_polygon_table = gpd.GeoDataFrame(geometry=polygon_series)
-    return ShapesModel.parse(cell_polygon_table)
-
-
-def _make_circles(centroid_coordinates: np.ndarray, radius: list[float]) -> GeoDataFrame:
-    return ShapesModel.parse(centroid_coordinates, geometry=0, radius=radius)
+from tests.conftest import _make_points, _make_sdata_for_testing_querying_and_aggretation, _make_squares
 
 
 # ---------------- test bounding box queries ---------------[
-
-
 def test_bounding_box_request_immutable():
     """Test that the bounding box request is immutable."""
     request = BoundingBoxRequest(
         axes=("y", "x"),
         min_coordinate=np.array([0, 0]),
         max_coordinate=np.array([10, 10]),
         target_coordinate_system="global",
@@ -392,89 +353,14 @@
         target_coordinate_system="global",
     )
     assert len(queried0.table) == 1
     assert len(queried1.table) == 3
 
 
 # ----------------- test polygon query -----------------
-def _make_sdata_for_testing_querying_and_aggretation() -> SpatialData:
-    """
-    Creates a SpatialData object with many edge cases for testing querying and aggregation.
-
-    Returns
-    -------
-    The SpatialData object.
-
-    Notes
-    -----
-    Description of what is tested (for a quick visualization, plot the returned SpatialData object):
-    - values to query/aggregate: polygons, points, circles
-    - values to query by: polygons, circles
-    - the shapes are completely inside, outside, or intersecting the query region (with the centroid inside or outside
-     the query region)
-
-    Additional cases:
-    - concave shape intersecting multiple times the same shape; used both as query and as value
-    - shape intersecting multiple shapes; used both as query and as value
-    """
-    values_centroids_squares = np.array([[x * 18, 0] for x in range(8)] + [[8 * 18 + 7, 0]] + [[0, 90], [50, 90]])
-    values_centroids_circles = np.array([[x * 18, 30] for x in range(8)] + [[8 * 18 + 7, 30]])
-    by_centroids_squares = np.array([[119, 15], [100, 90], [150, 90]])
-    by_centroids_circles = np.array([[24, 15]])
-    values_points = _make_points(np.vstack((values_centroids_squares, values_centroids_circles)))
-    values_squares = _make_squares(values_centroids_squares, half_widths=[6] * 9 + [15, 15])
-    values_circles = _make_circles(values_centroids_circles, radius=[6] * 9)
-    by_squares = _make_squares(by_centroids_squares, half_widths=[30, 15, 15])
-    by_circles = _make_circles(by_centroids_circles, radius=[30])
-
-    from shapely.geometry import Polygon
-
-    polygon = Polygon([(100, 90 - 10), (100 + 30, 90), (100, 90 + 10), (150, 90)])
-    values_squares.loc[len(values_squares)] = [polygon]
-    ShapesModel.validate(values_squares)
-
-    polygon = Polygon([(0, 90 - 10), (0 + 30, 90), (0, 90 + 10), (50, 90)])
-    by_squares.loc[len(by_squares)] = [polygon]
-    ShapesModel.validate(by_squares)
-
-    sdata = SpatialData(
-        points={"points": values_points},
-        shapes={
-            "values_polygons": values_squares,
-            "values_circles": values_circles,
-            "by_polygons": by_squares,
-            "by_circles": by_circles,
-        },
-    )
-    # to visualize the cases considered in the test, much more immediate than reading them as text as done above
-    PLOT = False
-    if PLOT:
-        import matplotlib.pyplot as plt
-
-        ax = plt.gca()
-        sdata.pl.render_shapes(element="values_polygons", na_color=(0.5, 0.2, 0.5, 0.5)).pl.render_points().pl.show(
-            ax=ax
-        )
-        sdata.pl.render_shapes(element="values_circles", na_color=(0.5, 0.2, 0.5, 0.5)).pl.show(ax=ax)
-        sdata.pl.render_shapes(element="by_polygons", na_color=(1.0, 0.7, 0.7, 0.5)).pl.show(ax=ax)
-        sdata.pl.render_shapes(element="by_circles", na_color=(1.0, 0.7, 0.7, 0.5)).pl.show(ax=ax)
-        plt.show()
-
-    # generate table
-    x = np.ones((21, 2)) * np.array([1, 2])
-    region = np.array(["values_circles"] * 9 + ["values_polygons"] * 12)
-    instance_id = np.array(list(range(9)) + list(range(12)))
-    table = AnnData(x, obs=pd.DataFrame({"region": region, "instance_id": instance_id}))
-    table = TableModel.parse(
-        table, region=["values_circles", "values_polygons"], region_key="region", instance_key="instance_id"
-    )
-    sdata.table = table
-    return sdata
-
-
 def test_polygon_query_points():
     sdata = _make_sdata_for_testing_querying_and_aggretation()
     polygon = sdata["by_polygons"].geometry.iloc[0]
     queried = polygon_query(sdata, polygons=polygon, target_coordinate_system="global", shapes=False, points=True)
     points = queried["points"].compute()
     assert len(points) == 6
     assert len(queried.table) == 0
@@ -549,23 +435,26 @@
 @pytest.mark.skip
 def test_polygon_query_image2d():
     # single image case
     # multiscale case
     pass
 
 
+@pytest.mark.skip
 def test_polygon_query_image3d():
     # single image case
     # multiscale case
     pass
 
 
+@pytest.mark.skip
 def test_polygon_query_labels2d():
     # single image case
     # multiscale case
     pass
 
 
+@pytest.mark.skip
 def test_polygon_query_labels3d():
     # single image case
     # multiscale case
     pass
```

### Comparing `spatialdata-0.0.7/tests/data/multipolygon.json` & `spatialdata-0.0.8/tests/data/multipolygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/data/polygon.json` & `spatialdata-0.0.8/tests/data/polygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/datasets/test_datasets.py` & `spatialdata-0.0.8/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/io/test_format.py` & `spatialdata-0.0.8/tests/io/test_format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/io/test_readwrite.py` & `spatialdata-0.0.8/tests/io/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/io/test_utils.py` & `spatialdata-0.0.8/tests/io/test_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/models/test_models.py` & `spatialdata-0.0.8/tests/models/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     Image3DModel,
     Labels2DModel,
     Labels3DModel,
     PointsModel,
     ShapesModel,
     TableModel,
     get_model,
+    points_dask_dataframe_to_geopandas,
+    points_geopandas_to_dask_dataframe,
 )
 from spatialdata.models._utils import validate_axis_name
 from spatialdata.models.models import RasterSchema
 from spatialdata.transformations._utils import (
     _set_transformations,
     _set_transformations_xarray,
 )
@@ -329,7 +331,35 @@
         schema = get_model(v)
         assert schema == PointsModel
     for v in shapes.values():
         schema = get_model(v)
         assert schema == ShapesModel
     schema = get_model(table)
     assert schema == TableModel
+
+
+def test_points_and_shapes_conversions(shapes, points):
+    from spatialdata.transformations import get_transformation
+
+    circles0 = shapes["circles"]
+    circles1 = points_geopandas_to_dask_dataframe(circles0)
+    circles2 = points_dask_dataframe_to_geopandas(circles1)
+    circles0 = circles0[circles2.columns]
+    assert np.all(circles0.values == circles2.values)
+
+    t0 = get_transformation(circles0, get_all=True)
+    t1 = get_transformation(circles1, get_all=True)
+    t2 = get_transformation(circles2, get_all=True)
+    assert t0 == t1
+    assert t0 == t2
+
+    points0 = points["points_0"]
+    points1 = points_dask_dataframe_to_geopandas(points0)
+    points2 = points_geopandas_to_dask_dataframe(points1)
+    points0 = points0[points2.columns]
+    assert np.all(points0.values == points2.values)
+
+    t0 = get_transformation(points0, get_all=True)
+    t1 = get_transformation(points1, get_all=True)
+    t2 = get_transformation(points2, get_all=True)
+    assert t0 == t1
+    assert t0 == t2
```

### Comparing `spatialdata-0.0.7/tests/test_dataloader/test_datasets.py` & `spatialdata-0.0.8/tests/dataloader/test_datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/transformations/test_transformations.py` & `spatialdata-0.0.8/tests/transformations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/transformations/ngff/conftest.py` & `spatialdata-0.0.8/tests/transformations/ngff/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/transformations/ngff/test_ngff_coordinate_system.py` & `spatialdata-0.0.8/tests/transformations/ngff/test_ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/transformations/ngff/test_ngff_transformations.py` & `spatialdata-0.0.8/tests/transformations/ngff/test_ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/tests/utils/test_element_utils.py` & `spatialdata-0.0.8/tests/utils/test_element_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/.gitignore` & `spatialdata-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/LICENSE` & `spatialdata-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/README.md` & `spatialdata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/pyproject.toml` & `spatialdata-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.7/PKG-INFO` & `spatialdata-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spatial data format.
 Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata.git
 Author: scverse
 Maintainer-email: scverse <giov.pll@gmail.com>
 License: BSD 3-Clause License
```

