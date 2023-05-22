# Comparing `tmp/gs_quant-0.9.99.tar.gz` & `tmp/gs_quant-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gs_quant-0.9.99.tar", last modified: Thu Apr  6 10:52:41 2023, max compression
+gzip compressed data, was "dist/gs_quant-1.0.0.tar", last modified: Mon May 22 08:54:47 2023, max compression
```

## Comparing `gs_quant-0.9.99.tar` & `gs_quant-1.0.0.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-06 10:52:24.000000 gs_quant-0.9.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-06 10:52:40.000000 gs_quant-0.9.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-06 10:52:24.000000 gs_quant-0.9.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/common/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/common/enumerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/common/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/core/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/core/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/core/processor_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/core/query_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/data_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/data_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/datagrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/analysis_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/econometrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/scale_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/special_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/statistics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/processors/utility_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/analytics/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/workspaces/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/analytics/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/api/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/api/fred/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/fred/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/fred/fred_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/api/gs/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    36633 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/hedges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/thematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/gs/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/backtests/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/action_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/backtest_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/backtest_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/backtest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/equity_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    39309 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/predefined_asset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/strategy_systematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/backtests/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/config/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/content/reports_and_screens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/content/reports_and_screens/00_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/content/reports_and_screens/00_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/content/reports_and_screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/data/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/data/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/datetime/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.add.html
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
--rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.log.html
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.power.html
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.count.html
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.first.html
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.last.html
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.align.html
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.day.html
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.month.html
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.union.html
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.value.html
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.year.html
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.median.html
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.product.html
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.std.html
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.var.html
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20227 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/entities/entitlements.py
--rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/entities/tree_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/instrument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/instrument/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/instrument/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/json_convertors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/markets/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38713 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/historical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/portfolio_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27816 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/position_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    62801 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/markets/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29605 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/models/epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/models/risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/models/risk_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/priceable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/quote_reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/quote_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/quote_reports/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/risk/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/result_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/scenario_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/risk/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/target/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/assets_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    30101 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)   241535 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    36279 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/secmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/workflow_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/target/workspaces_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/analytics/test_datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/analytics/test_sorting_and_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/analytics/test_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_fred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_thread_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/backtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_flow_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/test_generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/backtest/test_triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/data/test_data_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/data/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/datetime_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/test_gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/test_relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/datetime_/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/fixtures/content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_hedger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_pricing_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/markets/test_securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/models/test_epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    25829 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/models/test_risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/test_commod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16880 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   238167 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    58601 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)    29270 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_technicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/datagrid_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/mock_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/test/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   227330 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    30098 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/timeseries/technicals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-06 10:52:24.000000 gs_quant-0.9.99/gs_quant/tracing/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 10:52:40.000000 gs_quant-0.9.99/gs_quant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-06 10:52:40.000000 gs_quant-0.9.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-06 10:52:24.000000 gs_quant-0.9.99/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68673 2023-04-06 10:52:24.000000 gs_quant-0.9.99/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-22 08:54:28.000000 gs_quant-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-22 08:54:47.000000 gs_quant-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-22 08:54:28.000000 gs_quant-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/common/enumerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/common/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/core/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/core/processor_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/core/query_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/data_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/data_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/datagrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/analysis_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/econometrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/scale_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/special_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/statistics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/processors/utility_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/analytics/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/workspaces/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/analytics/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/api/fred/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/fred/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/fred/fred_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/api/gs/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38344 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/hedges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/thematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/gs/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/backtests/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/action_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/backtest_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/backtest_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/backtest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/equity_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/predefined_asset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/strategy_systematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/backtests/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/content/reports_and_screens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/content/reports_and_screens/00_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/content/reports_and_screens/00_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/content/reports_and_screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/data/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/datetime/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.add.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.log.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.power.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.count.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.first.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.last.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.align.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.day.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.month.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.union.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.value.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.year.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.median.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.product.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.var.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/entities/entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/entities/tree_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/instrument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/instrument/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/instrument/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/json_convertors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/portfolio_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29040 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/position_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62817 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/markets/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/models/epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/models/risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/models/risk_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/priceable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/quote_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/quote_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/quote_reports/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/result_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/scenario_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/risk/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/target/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/assets_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/secmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/workflow_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/target/workspaces_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/analytics/test_datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/analytics/test_sorting_and_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/analytics/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_thread_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/backtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_flow_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/test_generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/backtest/test_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/data/test_data_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/data/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/datetime_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/test_gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/test_relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/datetime_/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/fixtures/content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_hedger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_pricing_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/markets/test_securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/models/test_epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/models/test_risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/test_commod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_technicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/datagrid_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/mock_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/test/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/timeseries/technicals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-22 08:54:28.000000 gs_quant-1.0.0/gs_quant/tracing/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 08:54:47.000000 gs_quant-1.0.0/gs_quant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-22 08:54:47.000000 gs_quant-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-22 08:54:28.000000 gs_quant-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-05-22 08:54:28.000000 gs_quant-1.0.0/versioneer.py
```

### Comparing `gs_quant-0.9.99/PKG-INFO` & `gs_quant-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs_quant
-Version: 0.9.99
+Version: 1.0.0
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
         
@@ -35,16 +35,19 @@
         
         ## Help
         
         Please reach out to `gs-quant@gs.com` with any questions, comments or feedback.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 Provides-Extra: internal
 Provides-Extra: turbo
 Provides-Extra: notebook
 Provides-Extra: test
```

### Comparing `gs_quant-0.9.99/README.md` & `gs_quant-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/__init__.py` & `gs_quant-1.0.0/gs_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/common/__init__.py` & `gs_quant-1.0.0/gs_quant/analytics/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/common/constants.py` & `gs_quant-1.0.0/gs_quant/analytics/common/constants.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/common/enumerators.py` & `gs_quant-1.0.0/gs_quant/analytics/common/enumerators.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/common/helpers.py` & `gs_quant-1.0.0/gs_quant/analytics/common/helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/core/__init__.py` & `gs_quant-1.0.0/gs_quant/analytics/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/core/processor.py` & `gs_quant-1.0.0/gs_quant/analytics/core/processor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/core/processor_result.py` & `gs_quant-1.0.0/gs_quant/analytics/core/processor_result.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/core/query_helpers.py` & `gs_quant-1.0.0/gs_quant/analytics/core/query_helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/__init__.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/data_cell.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/data_cell.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/data_column.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/data_column.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/data_row.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/data_row.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/datagrid.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/serializers.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/serializers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/datagrid/utils.py` & `gs_quant-1.0.0/gs_quant/analytics/datagrid/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/__init__.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 """
 
 from .analysis_processors import DiffProcessor
 from .econometrics_processors import SharpeRatioProcessor, VolatilityProcessor, CorrelationProcessor, ChangeProcessor, \
     ReturnsProcessor, BetaProcessor, FXImpliedCorrProcessor
 from .special_processors import EntityProcessor, CoordinateProcessor
 from .statistics_processors import PercentilesProcessor, PercentileProcessor, StdMoveProcessor, \
-    CovarianceProcessor, ZscoresProcessor, MeanProcessor, VarianceProcessor, SumProcessor, StdDevProcessor
+    CovarianceProcessor, ZscoresProcessor, MeanProcessor, VarianceProcessor, SumProcessor, StdDevProcessor, \
+    CompoundGrowthRate
 from .utility_processors import LastProcessor, AppendProcessor, AdditionProcessor, SubtractionProcessor, \
     MultiplicationProcessor, DivisionProcessor, MinProcessor, MaxProcessor, NthLastProcessor, OneDayProcessor
 from .scale_processors import ScaleProcessor, BarMarkerProcessor, SpotMarkerProcessor, ScaleShape
```

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/analysis_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/analysis_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/econometrics_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/econometrics_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     def process(self):
         a_data = self.children_data.get('a')
         if isinstance(a_data, ProcessorResult):
             if a_data.success:
                 data = a_data.data
                 if self.observations is None:
                     if len(data) > 1:
-                        self.value = ProcessorResult(True, Series([(data.iloc[-1] - data.iloc[0]) / data.iloc[-1]]))
+                        self.value = ProcessorResult(True, Series([(data.iloc[-1] - data.iloc[0]) / data.iloc[0]]))
                     else:
                         self.value = ProcessorResult(True, 'Series has is less than 2.')
                 else:
                     value = returns(a_data.data, self.observations, self.type_)
                     self.value = ProcessorResult(True, value)
 
         return self.value
```

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/scale_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/scale_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/special_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/special_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/statistics_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/statistics_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 specific language governing permissions and limitations
 under the License.
 """
 
 from typing import Optional, Union
 
 import pandas as pd
+from pandas import Series
 
 from gs_quant.analytics.core.processor import BaseProcessor, DataCoordinateOrProcessor, DateOrDatetimeOrRDate
 from gs_quant.analytics.core.processor_result import ProcessorResult
 from gs_quant.timeseries import returns
 from gs_quant.timeseries.statistics import percentiles, percentile, Window, mean, sum_, std, var, cov, zscores
 
 
@@ -487,7 +488,46 @@
                 self.value = ProcessorResult(False, "StdMoveProcessor does not have 'a' series values yet")
         else:
             self.value = ProcessorResult(False, "StdMoveProcessor does not have 'a' series yet")
         return self.value
 
     def get_plot_expression(self):
         pass
+
+
+class CompoundGrowthRate(BaseProcessor):
+    def __init__(self,
+                 a: DataCoordinateOrProcessor,
+                 *,
+                 start: Optional[DateOrDatetimeOrRDate] = None,
+                 end: Optional[DateOrDatetimeOrRDate] = None,
+                 n: Optional[float] = None,
+                 **kwargs):
+        """ CompoundGrowthRate: indicates the growth rate over given time period n
+
+        :param a: DataCoordinate or BaseProcessor of series
+        :param start: start date or time used in the underlying data query
+        :param end: end date or time used in the underlying data query
+        :param n: Number of time
+        """
+        super().__init__(**kwargs)
+        self.children['a'] = a
+
+        self.start = start
+        self.end = end
+        self.n = n
+
+    def process(self):
+        a_data = self.children_data.get('a')
+        if isinstance(a_data, ProcessorResult):
+            if a_data.success:
+                data_series = a_data.data
+                self.value = ProcessorResult(True,
+                                             Series([(data_series.iloc[-1] / data_series.iloc[0]) ** (1 / self.n) - 1]))
+            else:
+                self.value = ProcessorResult(False, "CompoundGrowthRate does not have 'a' series values yet")
+        else:
+            self.value = ProcessorResult(False, "CompoundGrowthRate does not have 'a' series yet")
+        return self.value
+
+    def get_plot_expression(self):
+        pass
```

### Comparing `gs_quant-0.9.99/gs_quant/analytics/processors/utility_processors.py` & `gs_quant-1.0.0/gs_quant/analytics/processors/utility_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/workspaces/__init__.py` & `gs_quant-1.0.0/gs_quant/analytics/workspaces/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .components import (ArticleComponent,
                          CommentaryComponent,
+                         Component,
                          ContainerComponent,
                          DataGridComponent,
                          LegendComponent,
                          MonitorComponent,
                          PlotComponent,
                          PromoComponent,
                          RelatedLinksComponent,
```

### Comparing `gs_quant-0.9.99/gs_quant/analytics/workspaces/components.py` & `gs_quant-1.0.0/gs_quant/analytics/workspaces/components.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/analytics/workspaces/workspace.py` & `gs_quant-1.0.0/gs_quant/analytics/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/__init__.py` & `gs_quant-1.0.0/gs_quant/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/data.py` & `gs_quant-1.0.0/gs_quant/api/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/fred/__init__.py` & `gs_quant-1.0.0/gs_quant/api/fred/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/fred/data.py` & `gs_quant-1.0.0/gs_quant/api/fred/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/fred/fred_query.py` & `gs_quant-1.0.0/gs_quant/api/fred/fred_query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/__init__.py` & `gs_quant-1.0.0/gs_quant/api/gs/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/assets.py` & `gs_quant-1.0.0/gs_quant/api/gs/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,29 @@
     ) -> Union[Tuple[GsAsset, ...], Tuple[dict, ...]]:
         query = cls.__create_query(fields, as_of, limit, order_by=order_by, **kwargs)
         response = GsSession.current._post('/assets/query', payload=query, cls=return_type)
         return response['results']
 
     @classmethod
     @_cached
+    async def get_many_assets_async(
+            cls,
+            fields: IdList = None,
+            as_of: dt.datetime = None,
+            limit: int = 100,
+            return_type: Optional[type] = GsAsset,
+            order_by: List[str] = None,
+            **kwargs
+    ) -> Union[Tuple[GsAsset, ...], Tuple[dict, ...]]:
+        query = cls.__create_query(fields, as_of, limit, order_by=order_by, **kwargs)
+        response = await GsSession.current._post_async('/assets/query', payload=query, cls=return_type)
+        return response['results']
+
+    @classmethod
+    @_cached
     def get_many_assets_data(
             cls,
             fields: IdList = None,
             as_of: dt.datetime = None,
             limit: int = None,
             **kwargs
     ) -> dict:
```

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/backtests.py` & `gs_quant-1.0.0/gs_quant/api/gs/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/base_screener.py` & `gs_quant-1.0.0/gs_quant/api/gs/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/carbon.py` & `gs_quant-1.0.0/gs_quant/api/gs/carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/content.py` & `gs_quant-1.0.0/gs_quant/api/gs/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/countries.py` & `gs_quant-1.0.0/gs_quant/api/gs/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/data.py` & `gs_quant-1.0.0/gs_quant/api/gs/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import logging
 import time
 from enum import Enum
 from itertools import chain
 from typing import Iterable, List, Optional, Tuple, Union, Dict
 
 import cachetools
-import numpy as np
 import pandas as pd
 from cachetools import TTLCache
 
 from gs_quant.api.data import DataApi
 from gs_quant.base import Base
 from gs_quant.data.core import DataContext, DataFrequency
 from gs_quant.data.log import log_debug, log_warning
@@ -187,18 +186,27 @@
     def execute_query(dataset_id: str, query: Union[DataQuery, MDAPIDataQuery]):
         kwargs = {'payload': query}
         if getattr(query, 'format', None) in (Format.MessagePack, 'MessagePack'):
             kwargs['request_headers'] = {'Accept': 'application/msgpack'}
         return GsSession.current._post('/data/{}/query'.format(dataset_id), **kwargs)
 
     @staticmethod
-    def get_results(dataset_id: str, response: Union[DataQueryResponse, dict], query: DataQuery) -> list:
+    def get_results(dataset_id: str, response: Union[DataQueryResponse, dict], query: DataQuery) -> \
+            Union[list, Tuple[list, list]]:
         if isinstance(response, dict):
             total_pages = response.get('totalPages')
-            results = response.get('data', ())
+            results = response.get('data', [])
+            if 'groups' in response:
+                group_by = set()
+                for group in response['groups']:
+                    group_by.update(group['context'].keys())
+                    for row in group['data']:
+                        row.update(group['context'])
+                    results += group['data']
+                results = (results, list(group_by))
         else:
             total_pages = response.total_pages if response.total_pages is not None else 0
             results = response.data if response.data is not None else ()
 
         if total_pages:
             if query.page is None:
                 query.page = total_pages - 1
@@ -231,54 +239,78 @@
 
     @classmethod
     def time_field(cls, dataset_id: str) -> str:
         definition = cls.get_definition(dataset_id)
         return definition.dimensions.timeField
 
     # GS-specific functionality
+    @classmethod
+    def _build_params(cls, scroll: str, scroll_id: Optional[str], limit: int, offset: int, fields: List[str],
+                      include_history: bool, **kwargs) -> dict:
+        params = {'limit': limit or 4000, 'scroll': scroll}
+        if scroll_id:
+            params['scrollId'] = scroll_id
+        if offset:
+            params['offset'] = offset
+        if fields:
+            params['fields'] = fields
+        if include_history:
+            params['includeHistory'] = 'true'
+        params = {**params, **kwargs}
+        return params
 
     @classmethod
     def get_coverage(
             cls,
             dataset_id: str,
             scroll: str = DEFAULT_SCROLL,
             scroll_id: Optional[str] = None,
             limit: int = None,
             offset: int = None,
             fields: List[str] = None,
             include_history: bool = False,
             **kwargs
     ) -> List[dict]:
-        params = {
-            'limit': limit or 4000,
-            'scroll': scroll
-        }
-
-        if scroll_id:
-            params['scrollId'] = scroll_id
-        if offset:
-            params['offset'] = offset
-        if fields:
-            params['fields'] = fields
-        if include_history:
-            params['includeHistory'] = 'true'
-
-        params = {**params, **kwargs}
+        params = cls._build_params(scroll, scroll_id, limit, offset, fields, include_history, **kwargs)
         body = GsSession.current._get(f'/data/{dataset_id}/coverage', payload=params)
         results = scroll_results = body['results']
         total_results = body['totalResults']
         while len(scroll_results) and len(results) < total_results:
             params['scrollId'] = body['scrollId']
             body = GsSession.current._get(f'/data/{dataset_id}/coverage', payload=params)
             scroll_results = body['results']
             results += scroll_results
 
         return results
 
     @classmethod
+    async def get_coverage_async(
+            cls,
+            dataset_id: str,
+            scroll: str = DEFAULT_SCROLL,
+            scroll_id: Optional[str] = None,
+            limit: int = None,
+            offset: int = None,
+            fields: List[str] = None,
+            include_history: bool = False,
+            **kwargs
+    ) -> List[dict]:
+        params = cls._build_params(scroll, scroll_id, limit, offset, fields, include_history, **kwargs)
+        body = await GsSession.current._get_async(f'/data/{dataset_id}/coverage', payload=params)
+        results = scroll_results = body['results']
+        total_results = body['totalResults']
+        while len(scroll_results) and len(results) < total_results:
+            params['scrollId'] = body['scrollId']
+            body = await GsSession.current._get_async(f'/data/{dataset_id}/coverage', payload=params)
+            scroll_results = body['results']
+            if scroll_results:
+                results += scroll_results
+        return results
+
+    @classmethod
     def create(cls, definition: Union[DataSetEntity, dict]) -> DataSetEntity:
         result = GsSession.current._post('/data/datasets', payload=definition)
         return result
 
     @classmethod
     def delete_dataset(cls, dataset_id: str) -> dict:
         result = GsSession.current._delete(f'/data/datasets/{dataset_id}')
@@ -780,15 +812,15 @@
             incoming_data_data_types = pd.DataFrame(sample).dtypes.to_dict()
 
             df = pd.DataFrame(data, columns={**dataset_types, **incoming_data_data_types})
 
             for field_name, type_name in dataset_types.items():
                 if df.get(field_name) is not None and type_name in ('date', 'date-time') and \
                         len(df.get(field_name).value_counts()) > 0:
-                    df = df.astype({field_name: np.datetime64})
+                    df = df.astype({field_name: 'datetime64[ns]'})
 
             field_names = dataset_types.keys()
 
             if 'date' in field_names:
                 df = df.set_index('date')
             elif 'time' in field_names:
                 df = df.set_index('time')
```

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/data_screen.py` & `gs_quant-1.0.0/gs_quant/api/gs/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/datagrid.py` & `gs_quant-1.0.0/gs_quant/api/gs/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/esg.py` & `gs_quant-1.0.0/gs_quant/api/gs/esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/groups.py` & `gs_quant-1.0.0/gs_quant/api/gs/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/hedges.py` & `gs_quant-1.0.0/gs_quant/api/gs/hedges.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/indices.py` & `gs_quant-1.0.0/gs_quant/api/gs/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/monitors.py` & `gs_quant-1.0.0/gs_quant/api/gs/monitors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/parser.py` & `gs_quant-1.0.0/gs_quant/api/gs/parser.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/plots.py` & `gs_quant-1.0.0/gs_quant/api/gs/plots.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/portfolios.py` & `gs_quant-1.0.0/gs_quant/api/gs/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/price.py` & `gs_quant-1.0.0/gs_quant/api/gs/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/reports.py` & `gs_quant-1.0.0/gs_quant/api/gs/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/risk.py` & `gs_quant-1.0.0/gs_quant/api/gs/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/risk_models.py` & `gs_quant-1.0.0/gs_quant/api/gs/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/screens.py` & `gs_quant-1.0.0/gs_quant/api/gs/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/thematics.py` & `gs_quant-1.0.0/gs_quant/api/gs/thematics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/users.py` & `gs_quant-1.0.0/gs_quant/api/gs/users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/gs/workspaces.py` & `gs_quant-1.0.0/gs_quant/api/gs/workspaces.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/risk.py` & `gs_quant-1.0.0/gs_quant/api/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/api/utils.py` & `gs_quant-1.0.0/gs_quant/api/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/__init__.py` & `gs_quant-1.0.0/gs_quant/backtests/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/action_handler.py` & `gs_quant-1.0.0/gs_quant/backtests/action_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/actions.py` & `gs_quant-1.0.0/gs_quant/backtests/actions.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/backtest_engine.py` & `gs_quant-1.0.0/gs_quant/backtests/backtest_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/backtest_objects.py` & `gs_quant-1.0.0/gs_quant/backtests/backtest_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,20 +231,21 @@
         self.csa_term = csa_term
         self.scaling_parameter = scaling_parameter
         self.risk_transformation = risk_transformation
         self.results = None
 
 
 class CashPayment:
-    def __init__(self, trade, effective_date=None, scale_date=None, direction=1):
+    def __init__(self, trade, effective_date=None, scale_date=None, direction=1, scaling_parameter='notional_amount'):
         self.trade = trade
         self.effective_date = effective_date
         self.scale_date = scale_date
         self.direction = direction
         self.cash_paid = defaultdict(float)
+        self.scaling_parameter = scaling_parameter
 
     def to_frame(self):
         df = pd.DataFrame(self.cash_paid.items(), columns=['Cash Ccy', 'Cash Amount'])
         df['Instrument Name'] = self.trade.name
         df['Pricing Date'] = self.effective_date
         return df
```

### Comparing `gs_quant-0.9.99/gs_quant/backtests/backtest_utils.py` & `gs_quant-1.0.0/gs_quant/backtests/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/core.py` & `gs_quant-1.0.0/gs_quant/backtests/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/data_handler.py` & `gs_quant-1.0.0/gs_quant/backtests/data_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/data_sources.py` & `gs_quant-1.0.0/gs_quant/backtests/data_sources.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/decorator.py` & `gs_quant-1.0.0/gs_quant/backtests/decorator.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/equity_vol_engine.py` & `gs_quant-1.0.0/gs_quant/backtests/equity_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/event.py` & `gs_quant-1.0.0/gs_quant/backtests/event.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/execution_engine.py` & `gs_quant-1.0.0/gs_quant/backtests/execution_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/generic_engine.py` & `gs_quant-1.0.0/gs_quant/backtests/generic_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,17 +227,19 @@
                                                   Iterable[EnterPositionQuantityScaledActionInfo]]] = None):
 
         orders = self._raise_order(state)
 
         # record entry and unwind cashflows
         for create_date, portfolio in orders.items():
             for inst in portfolio.all_instruments:
-                backtest.cash_payments[create_date].append(CashPayment(inst, effective_date=create_date, direction=-1))
+                backtest.cash_payments[create_date].append(CashPayment(inst, effective_date=create_date, direction=-1,
+                                                                       scaling_parameter=self.action.trade_quantity))
                 final_date = get_final_date(inst, create_date, self.action.trade_duration)
-                backtest.cash_payments[final_date].append(CashPayment(inst, effective_date=final_date))
+                backtest.cash_payments[final_date].append(CashPayment(inst, effective_date=final_date,
+                                                                      scaling_parameter=self.action.trade_quantity))
 
         for s in backtest.states:
             pos = []
             for create_date, portfolio in orders.items():
                 pos += [inst for inst in portfolio.instruments
                         if get_final_date(inst, create_date, self.action.trade_duration) > s >= create_date]
             if len(pos):
@@ -269,18 +271,20 @@
             active_dates = [s for s in backtest.states if create_date <= s < final_date]
 
             if len(active_dates):
                 scaling_portfolio = ScalingPortfolio(trade=hedge_trade, dates=active_dates, risk=self.action.risk,
                                                      csa_term=self.action.csa_term,
                                                      scaling_parameter=self.action.scaling_parameter,
                                                      risk_transformation=self.action.risk_transformation)
-                entry_payment = CashPayment(trade=hedge_trade, effective_date=create_date, direction=-1)
+                entry_payment = CashPayment(trade=hedge_trade, effective_date=create_date, direction=-1,
+                                            scaling_parameter=self.action.scaling_parameter)
                 backtest.transaction_costs[create_date] -= self.action.transaction_cost.get_cost(state, backtest,
                                                                                                  trigger_info)
-                exit_payment = CashPayment(trade=hedge_trade, effective_date=final_date, scale_date=create_date) \
+                exit_payment = CashPayment(trade=hedge_trade, effective_date=final_date, scale_date=create_date,
+                                           scaling_parameter=self.action.scaling_parameter) \
                     if final_date <= dt.date.today() else None
                 backtest.transaction_costs[final_date] -= self.action.transaction_cost.get_cost(state, backtest,
                                                                                                 trigger_info)
                 hedge = Hedge(scaling_portfolio=scaling_portfolio,
                               entry_payment=entry_payment,
                               exit_payment=exit_payment)
                 backtest.hedges[create_date].append(hedge)
@@ -363,22 +367,23 @@
                 current_size += getattr(trade, self.action.size_parameter)
         # if we are already at the required size then do nothing.
         if new_size - current_size == 0:
             return backtest
         pos = self.action.priceable.clone(**{self.action.size_parameter: new_size - current_size,
                                              'name': f'{self.action.priceable.name}_{state}'})
 
-        backtest.cash_payments[state].append(CashPayment(pos, effective_date=state, direction=-1))
+        backtest.cash_payments[state].append(CashPayment(pos, effective_date=state, direction=-1,
+                                                         scaling_parameter=self.action.size_parameter))
         backtest.transaction_costs[state] -= self.action.transaction_cost.get_cost(state, backtest, trigger_info)
         unwind_payment = None
         cash_payment_dates = backtest.cash_payments.keys()
         for d in reversed(sorted(cash_payment_dates)):
             for cp in backtest.cash_payments[d]:
                 if self.action.priceable.name.split('_')[-1] in cp.trade.name and cp.direction == 1:
-                    unwind_payment = CashPayment(pos, effective_date=d)
+                    unwind_payment = CashPayment(pos, effective_date=d, scaling_parameter=self.action.size_parameter)
                     backtest.cash_payments[d].append(unwind_payment)
                     backtest.transaction_costs[d] -= self.action.transaction_cost.get_cost(state, backtest,
                                                                                            trigger_info)
                     break
             if unwind_payment:
                 break
 
@@ -605,26 +610,24 @@
                 if t.name not in backtest.results[d].portfolio:
                     port.append(t)
 
             if len(port):
                 with PricingContext(pricing_date=d):
                     results = Portfolio(port).calc(tuple(risks))
 
+                backtest.add_results(d, results)
+
             for hedge in backtest.hedges[d]:
                 sp = hedge.scaling_portfolio
                 if sp.results is None:
                     with HistoricalPricingContext(dates=sp.dates):
                         backtest.calculations += len(risks) * len(sp.dates)
                         port_sp = sp.trade if isinstance(sp.trade, Portfolio) else Portfolio([sp.trade])
                         sp.results = port_sp.calc(tuple(risks))
 
-            # results should be added outside of pricing context and not in the same call as valuating them
-            if len(port):
-                backtest.add_results(d, results)
-
             # semi path dependent scaling
             if d in backtest.hedges:
                 if len(backtest.hedges[d]) and d not in backtest.results:
                     # No risk found to hedge, proceed to the next date
                     continue
                 for hedge in backtest.hedges[d]:
                     p = hedge.scaling_portfolio
@@ -745,17 +748,17 @@
                                                    f'{cp.effective_date} received value of {value}')
                             ccy = next(iter(value.unit))
                             if d not in backtest.cash_dict:
                                 backtest.cash_dict[d] = {ccy: initial_value}
                             if ccy not in backtest.cash_dict[d]:
                                 backtest.cash_dict[d][ccy] = 0
                             if cp.scale_date:
-                                scale_notional = backtest.portfolio_dict[cp.scale_date][cp.trade.name]. \
-                                    notional_amount
-                                scale_date_adj = scale_notional / cp.trade.notional_amount
+                                scale_notional = getattr(backtest.portfolio_dict[cp.scale_date][cp.trade.name],
+                                                         cp.scaling_parameter)
+                                scale_date_adj = scale_notional / getattr(cp.trade, cp.scaling_parameter)
                                 cp.cash_paid[ccy] += value * scale_date_adj * cp.direction
                             else:
                                 cp.cash_paid[ccy] += value * cp.direction
 
                         for ccy, cash_paid in cp.cash_paid.items():
                             backtest.cash_dict[d][ccy] += cash_paid
```

### Comparing `gs_quant-0.9.99/gs_quant/backtests/order.py` & `gs_quant-1.0.0/gs_quant/backtests/order.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/predefined_asset_engine.py` & `gs_quant-1.0.0/gs_quant/backtests/predefined_asset_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/strategy.py` & `gs_quant-1.0.0/gs_quant/backtests/strategy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/strategy_systematic.py` & `gs_quant-1.0.0/gs_quant/backtests/strategy_systematic.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/backtests/triggers.py` & `gs_quant-1.0.0/gs_quant/backtests/triggers.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 
 from typing import Optional
 import warnings
 from gs_quant.backtests.actions import Action, AddTradeAction, AddTradeActionInfo
 from gs_quant.backtests.backtest_objects import BackTest, PredefinedAssetBacktest
 from gs_quant.backtests.backtest_utils import make_list, CalcType
-from gs_quant.datetime.relative_date import RelativeDateSchedule
 from gs_quant.backtests.data_sources import *
+from gs_quant.datetime.relative_date import RelativeDateSchedule
+from gs_quant.risk.transform import Transformer
+from gs_quant.risk import RiskMeasure
 
 
 class TriggerDirection(Enum):
     ABOVE = 1
     BELOW = 2
     EQUAL = 3
 
@@ -37,44 +39,47 @@
 
 class TriggerRequirements(object):
     def __init__(self):
         pass
 
 
 class PeriodicTriggerRequirements(TriggerRequirements):
-    def __init__(self, start_date=None, end_date=None, frequency=None, calendar=None):
+    def __init__(self, start_date: dt.date = None, end_date: dt.date = None, frequency: str = None,
+                 calendar: str = None):
         super().__init__()
         self.start_date = start_date
         self.end_date = end_date
         self.frequency = frequency
         self.calendar = calendar
 
 
 class IntradayTriggerRequirements(TriggerRequirements):
-    def __init__(self, start_time, end_time, frequency):
+    def __init__(self, start_time: dt.datetime, end_time: dt.datetime, frequency: str):
         super().__init__()
         self.start_time = start_time
         self.end_time = end_time
         self.frequency = frequency
 
 
 class MktTriggerRequirements(TriggerRequirements):
-    def __init__(self, data_source, trigger_level, direction):
+    def __init__(self, data_source: DataSource, trigger_level: float, direction: TriggerDirection):
         super().__init__()
         self.data_source = data_source
         self.trigger_level = trigger_level
         self.direction = direction
 
 
 class RiskTriggerRequirements(TriggerRequirements):
-    def __init__(self, risk, trigger_level, direction):
+    def __init__(self, risk: RiskMeasure, trigger_level: float, direction: TriggerDirection,
+                 risk_transformation: Optional[Transformer] = None):
         super().__init__()
         self.risk = risk
         self.trigger_level = trigger_level
         self.direction = direction
+        self.risk_transformation = risk_transformation
 
 
 class AggregateTriggerRequirements(TriggerRequirements):
     def __init__(self, triggers: Iterable[object], aggregate_type: AggType = AggType.ALL_OF):
         super().__init__()
         self.triggers = triggers
         self.aggregate_type = aggregate_type
@@ -254,15 +259,20 @@
                  trigger_requirements: RiskTriggerRequirements,
                  actions: Union[Action, Iterable[Action]]):
         super().__init__(trigger_requirements, actions)
         self._calc_type = CalcType.path_dependent
         self._risks += [trigger_requirements.risk]
 
     def has_triggered(self, state: dt.date, backtest: BackTest = None) -> TriggerInfo:
-        risk_value = backtest.results[state][self._trigger_requirements.risk].aggregate()
+        if self.trigger_requirements.risk_transformation is None:
+            risk_value = backtest.results[state][self._trigger_requirements.risk].aggregate()
+        else:
+            risk_value = backtest.results[state][self._trigger_requirements.risk].transform(
+                risk_transformation=self.trigger_requirements.risk_transformation).aggregate(
+                allow_mismatch_risk_keys=True)
         if self._trigger_requirements.direction == TriggerDirection.ABOVE:
             if risk_value > self._trigger_requirements.trigger_level:
                 return TriggerInfo(True)
         elif self._trigger_requirements.direction == TriggerDirection.BELOW:
             if risk_value < self._trigger_requirements.trigger_level:
                 return TriggerInfo(True)
         else:
```

### Comparing `gs_quant-0.9.99/gs_quant/base.py` & `gs_quant-1.0.0/gs_quant/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,26 @@
 
     def __repr__(self):
         return self.value
 
 
 class HashableDict(dict):
 
+    @staticmethod
+    def hashables(in_dict) -> Tuple:
+        hashables = []
+        for it in in_dict.items():
+            if isinstance(it[1], dict):
+                hashables.append((it[0], HashableDict.hashables(it[1])))
+            else:
+                hashables.append(it)
+        return tuple(hashables)
+
     def __hash__(self):
-        return hash(tuple(self.items()))
+        return hash(HashableDict.hashables(self))
 
 
 class DictBase(HashableDict):
 
     _PROPERTIES = set()
 
     def __init__(self, *args, **kwargs):
```

### Comparing `gs_quant-0.9.99/gs_quant/common.py` & `gs_quant-1.0.0/gs_quant/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/config/__init__.py` & `gs_quant-1.0.0/gs_quant/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/config/options.py` & `gs_quant-1.0.0/gs_quant/config/options.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/config.ini` & `gs_quant-1.0.0/gs_quant/config.ini`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py` & `gs_quant-1.0.0/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/context_base.py` & `gs_quant-1.0.0/gs_quant/context_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,14 +114,27 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self._on_exit(exc_type, exc_val, exc_tb)
         finally:
             self._cls.pop()
             setattr(thread_local, self.__entered_key, False)
 
+    async def __aenter__(self):
+        self._cls.push(self)
+        setattr(thread_local, self.__entered_key, True)
+        await self._on_aenter()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        try:
+            await self._on_aexit(exc_type, exc_val, exc_tb)
+        finally:
+            self._cls.pop()
+            setattr(thread_local, self.__entered_key, False)
+
     @property
     def __entered_key(self) -> str:
         return '{}_entered'.format(id(self))
 
     @property
     def _cls(self) -> ContextMeta:
         seen = set()
@@ -146,14 +159,20 @@
 
     def _on_enter(self):
         pass
 
     def _on_exit(self, exc_type, exc_val, exc_tb):
         pass
 
+    async def _on_aenter(self):
+        pass
+
+    async def _on_aexit(self, exc_type, exc_val, exc_tb):
+        pass
+
 
 class ContextBaseWithDefault(ContextBase):
 
     @classmethod
     def default_value(cls) -> object:
         return cls()
```

### Comparing `gs_quant-0.9.99/gs_quant/data/__init__.py` & `gs_quant-1.0.0/gs_quant/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/coordinate.py` & `gs_quant-1.0.0/gs_quant/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/core.py` & `gs_quant-1.0.0/gs_quant/data/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/dataset.py` & `gs_quant-1.0.0/gs_quant/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,19 @@
             end=end,
             as_of=as_of,
             since=since,
             fields=field_names,
             **kwargs
         )
         data = self.provider.query_data(query, self.id, asset_id_type=asset_id_type)
-
-        return self.provider.construct_dataframe_with_types(self.id, data, schema_varies)
+        if type(data) is tuple:
+            df = self.provider.construct_dataframe_with_types(self.id, data[0], schema_varies)
+            return df.groupby(data[1], group_keys=True).apply(lambda x: x)
+        else:
+            return self.provider.construct_dataframe_with_types(self.id, data, schema_varies)
 
     def get_data_series(
             self,
             field: Union[str, Fields],
             start: Optional[Union[dt.date, dt.datetime]] = None,
             end: Optional[Union[dt.date, dt.datetime]] = None,
             as_of: Optional[dt.datetime] = None,
@@ -280,14 +283,49 @@
             self.id,
             limit=limit,
             offset=offset,
             fields=fields,
             include_history=include_history,
             **kwargs
         )
+
+        return pd.DataFrame(coverage)
+
+    async def get_coverage_async(
+            self,
+            limit: Optional[int] = None,
+            offset: Optional[int] = None,
+            fields: Optional[List[str]] = None,
+            include_history: bool = False,
+            **kwargs
+    ) -> pd.DataFrame:
+        """
+        Get the assets covered by this DataSet
+
+        :param limit: The maximum number of assets to return
+        :param offset: The offset
+        :param fields: The fields to return, e.g. assetId
+        :param include_history: Return column for historyStartDate
+        :return: A Dataframe of the assets covered
+
+        **Examples**
+
+        >>> from gs_quant.data import Dataset
+        >>>
+        >>> weather = Dataset('WEATHER')
+        >>> cities = await weather.get_coverage_async()
+        """
+        coverage = await self.provider.get_coverage_async(
+            self.id,
+            limit=limit,
+            offset=offset,
+            fields=fields,
+            include_history=include_history,
+            **kwargs
+        )
 
         return pd.DataFrame(coverage)
 
     def delete(self) -> Dict:
         """
         Delete dataset definition.
```

### Comparing `gs_quant-0.9.99/gs_quant/data/fields.py` & `gs_quant-1.0.0/gs_quant/data/fields.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/log.py` & `gs_quant-1.0.0/gs_quant/data/log.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/query.py` & `gs_quant-1.0.0/gs_quant/data/query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/data/stream.py` & `gs_quant-1.0.0/gs_quant/data/stream.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/__init__.py` & `gs_quant-1.0.0/gs_quant/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/date.py` & `gs_quant-1.0.0/gs_quant/datetime/date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/point.py` & `gs_quant-1.0.0/gs_quant/datetime/point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/relative_date.py` & `gs_quant-1.0.0/gs_quant/datetime/relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/rules.py` & `gs_quant-1.0.0/gs_quant/datetime/rules.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/datetime/time.py` & `gs_quant-1.0.0/gs_quant/datetime/time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.business_day_count.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.business_day_count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.date_range.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.is_business_day.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.is_business_day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.add.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.add.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.and_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.and_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.divide.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.divide.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.exp.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.exp.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.floor.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.floor.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.if_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.if_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.log.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.log.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.not_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.not_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.or_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.or_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.power.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.power.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.count.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.diff.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.diff.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.first.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.first.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.lag.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.lag.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.last.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.last.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.align.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.align.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.day.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.month.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.month.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.union.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.union.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.value.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.datetime.year.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.datetime.year.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.change.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.change.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.index.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.cov.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.cov.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.max_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.max_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.mean.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.mean.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.median.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.median.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.min_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.min_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.mode.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.mode.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.product.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.product.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.range_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.range_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.std.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.var.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.var.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html` & `gs_quant-1.0.0/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/entities/entitlements.py` & `gs_quant-1.0.0/gs_quant/entities/entitlements.py`

 * *Files 7% similar despite different names*

```diff
@@ -320,18 +320,21 @@
                            tags=self.tags)
 
 
 class EntitlementBlock:
     def __init__(self,
                  users: List[User] = None,
                  groups: List[Group] = None,
-                 roles: List[str] = None):
+                 roles: List[str] = None,
+                 unconverted_tokens: List[str] = None,
+                 ):
         self.__users = list(set(users)) if users else []
         self.__groups = list(set(groups)) if groups else []
         self.__roles = list(set(roles)) if roles else []
+        self.__unconverted_tokens = unconverted_tokens
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, EntitlementBlock):
             return False
         for prop in ['users', 'groups', 'roles']:
             slf, oth = get(self, prop), get(other, prop)
             if not (slf is None and oth is None) and not slf == oth:
@@ -358,31 +361,36 @@
     def roles(self):
         return self.__roles
 
     @roles.setter
     def roles(self, value: List[str]):
         self.__roles = list(set(value))
 
+    @property
+    def unconverted_tokens(self) -> List[str]:
+        return self.__unconverted_tokens
+
     def is_empty(self):
         return len(self.users + self.groups + self.roles) == 0
 
-    def to_list(self, as_dicts: bool = False, action: str = None):
+    def to_list(self, as_dicts: bool = False, action: str = None, include_all_tokens: bool = False):
         if as_dicts:
             all_entitled = []
             for user in self.users:
                 all_entitled.append(dict(action=action, type='user', name=user.name, id=user.id))
             for group in self.groups:
                 all_entitled.append(dict(action=action, type='group', name=group.name, id=group.id))
             for role in self.roles:
                 all_entitled.append(dict(action=action, type='role', name=role, id=role))
             return all_entitled
         else:
+            unconverted_tokens = self.unconverted_tokens or [] if include_all_tokens else []
             return [f'guid:{user.id}' for user in self.users] + \
                    [f'group:{group.id}' for group in self.groups] + \
-                   [f'role:{role}' for role in self.roles]
+                   [f'role:{role}' for role in self.roles] + unconverted_tokens
 
 
 class Entitlements:
     def __init__(self,
                  admin: EntitlementBlock = None,
                  delete: EntitlementBlock = None,
                  display: EntitlementBlock = None,
@@ -500,42 +508,42 @@
     def view(self):
         return self.__view
 
     @view.setter
     def view(self, value: EntitlementBlock):
         self.__view = value
 
-    def to_target(self) -> TargetEntitlements:
+    def to_target(self, include_all_tokens: bool = False) -> TargetEntitlements:
         """
         Return Entitlement object as a target object
         :return: Entitlements as a target object
         """
         target_entitlements = TargetEntitlements.default_instance()
         if not self.admin.is_empty():
-            target_entitlements.admin = self.admin.to_list()
+            target_entitlements.admin = self.admin.to_list(include_all_tokens=include_all_tokens)
         if not self.delete.is_empty():
-            target_entitlements.delete = self.delete.to_list()
+            target_entitlements.delete = self.delete.to_list(include_all_tokens=include_all_tokens)
         if not self.display.is_empty():
-            target_entitlements.display = self.display.to_list()
+            target_entitlements.display = self.display.to_list(include_all_tokens=include_all_tokens)
         if not self.upload.is_empty():
-            target_entitlements.upload = self.upload.to_list()
+            target_entitlements.upload = self.upload.to_list(include_all_tokens=include_all_tokens)
         if not self.edit.is_empty():
-            target_entitlements.edit = self.edit.to_list()
+            target_entitlements.edit = self.edit.to_list(include_all_tokens=include_all_tokens)
         if not self.execute.is_empty():
-            target_entitlements.execute = self.execute.to_list()
+            target_entitlements.execute = self.execute.to_list(include_all_tokens=include_all_tokens)
         if not self.plot.is_empty():
-            target_entitlements.plot = self.plot.to_list()
+            target_entitlements.plot = self.plot.to_list(include_all_tokens=include_all_tokens)
         if not self.query.is_empty():
-            target_entitlements.query = self.query.to_list()
+            target_entitlements.query = self.query.to_list(include_all_tokens=include_all_tokens)
         if not self.rebalance.is_empty():
-            target_entitlements.rebalance = self.rebalance.to_list()
+            target_entitlements.rebalance = self.rebalance.to_list(include_all_tokens=include_all_tokens)
         if not self.trade.is_empty():
-            target_entitlements.trade = self.trade.to_list()
+            target_entitlements.trade = self.trade.to_list(include_all_tokens=include_all_tokens)
         if not self.view.is_empty():
-            target_entitlements.view = self.view.to_list()
+            target_entitlements.view = self.view.to_list(include_all_tokens=include_all_tokens)
         return target_entitlements
 
     def to_dict(self) -> Dict:
         """
         Return Entitlement object as a dictionary
         :return: Entitlements as a dictionary
         """
@@ -569,23 +577,40 @@
     @classmethod
     def from_dict(cls, entitlements: Dict):
         """
         Create an Entitlement object from a dictionary object
         :param entitlements: Entitlements as a dictionary object
         :return: A new Entitlements object with all specified entitlements
         """
-        entitlement_kwargs = {}
-        for action_info in entitlements:
-            users, groups, roles = [], [], []
-            for user in entitlements[action_info]:
-                if user.startswith('guid:'):
-                    users.append(user)
-                elif user.startswith('group:'):
-                    groups.append(user)
-                elif user.startswith('role:'):
-                    roles.append(user[5:])
-            if users or groups or roles:
-                entitlement_kwargs[action_info] = EntitlementBlock(
-                    users=User.get_many(user_ids=users),
-                    groups=Group.get_many(group_ids=groups),
-                    roles=roles)
+        entitlement_kwargs, token_map = {}, {}
+        user_ids, group_ids = set(), set()
+        for token_set in entitlements.values():
+            for t in token_set:
+                if t.startswith('guid:'):
+                    user_ids.add(t)
+                elif t.startswith('group:'):
+                    group_ids.add(t)
+                elif t.startswith('role:'):
+                    token_map[t] = t[5:]
+        all_users = User.get_many(user_ids=list(user_ids))
+        all_groups = Group.get_many(group_ids=list(group_ids))
+        for u in all_users:
+            token_map[f'guid:{u.id}'] = u
+        for g in all_groups:
+            token_map[f'group:{g.id}'] = g
+        for action, token_set in entitlements.items():
+            users, groups, roles, unconverted_tokens = [], [], [], []
+            for t in token_set:
+                if t in token_map.keys():
+                    if t in user_ids:
+                        users.append(token_map.get(t))
+                    elif t in group_ids:
+                        groups.append(token_map.get(t))
+                    else:
+                        roles.append(token_map.get(t))
+                else:
+                    unconverted_tokens.append(t)
+            unconverted_tokens = unconverted_tokens if len(unconverted_tokens) else None
+            if users or groups or roles or unconverted_tokens:
+                entitlement_kwargs[action] = EntitlementBlock(users=users, groups=groups, roles=roles,
+                                                              unconverted_tokens=unconverted_tokens)
         return Entitlements(**entitlement_kwargs)
```

### Comparing `gs_quant-0.9.99/gs_quant/entities/entity.py` & `gs_quant-1.0.0/gs_quant/entities/entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/entities/tree_entity.py` & `gs_quant-1.0.0/gs_quant/entities/tree_entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/errors.py` & `gs_quant-1.0.0/gs_quant/errors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/instrument/__init__.py` & `gs_quant-1.0.0/gs_quant/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/instrument/core.py` & `gs_quant-1.0.0/gs_quant/instrument/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/instrument/overrides.py` & `gs_quant-1.0.0/gs_quant/instrument/overrides.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/json_convertors.py` & `gs_quant-1.0.0/gs_quant/json_convertors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/json_encoder.py` & `gs_quant-1.0.0/gs_quant/json_encoder.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/__init__.py` & `gs_quant-1.0.0/gs_quant/markets/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/baskets.py` & `gs_quant-1.0.0/gs_quant/markets/baskets.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,18 +213,19 @@
 
         """
         edit_inputs, rebal_inputs = self.__get_updates()
         response = None
 
         init_entitlements = BasketEntitlements.from_target(self.__initial_entitlements)
         if not init_entitlements == self.__entitlements:
-            response = GsAssetApi.update_asset_entitlements(self.id, self.__entitlements.to_target())
+            response = GsAssetApi.update_asset_entitlements(self.id,
+                                                            self.__entitlements.to_target(include_all_tokens=True))
         if edit_inputs is None and rebal_inputs is None:
             if response:
-                return response.as_dict()
+                return response
             raise MqValueError('Update failed: Nothing on the basket was changed')
         elif edit_inputs is not None and rebal_inputs is None:
             response = GsIndexApi.edit(self.id, edit_inputs)
         elif rebal_inputs is not None and edit_inputs is None:
             response = GsIndexApi.rebalance(self.id, rebal_inputs)
         else:
             response = self.__edit_and_rebalance(edit_inputs, rebal_inputs)
@@ -829,15 +830,15 @@
         _logger.info('Current update request requires multiple reports. Your rebalance request will be submitted \
                       once the edit report has completed. Submitting basket edits now...')
         response = GsIndexApi.edit(self.id, edit_inputs)
         report_id = response.report_id
         self.__latest_create_report = GsReportApi.get_report(response.report_id)
         report_status = self.poll_report(report_id, timeout=600, step=15)
         if report_status != ReportStatus.done:
-            raise MqError(f'The basket edit report\'s status is {status}. The current rebalance request will \
+            raise MqError(f'The basket edit report\'s status is {report_status}. The current rebalance request will \
                             not be submitted in the meantime.')
         _logger.info('Your basket edits have completed successfuly. Submitting rebalance request now...')
         response = GsIndexApi.rebalance(self.id, rebal_inputs)
         return response
 
     def __finish_initialization(self):
         """ Fetches remaining data not retrieved during basket initialization """
@@ -975,14 +976,18 @@
             if not any(t in user_tokens for t in tokens):
                 errors.append(ErrorMessage.NON_ADMIN)
         self.__error_messages = set(errors)
 
     @staticmethod
     def __validate_position_set(position_set: PositionSet):
         position_set.resolve()
+        neg_pos = [p.identifier for p in position_set.positions if (p.weight or 1) < 0 or (p.quantity or 1) < 0]
+        if len(neg_pos):
+            raise MqValueError(f'Position weights/quantities must be positive. Found negative values for date \
+            {position_set.date}: {neg_pos}')
         if position_set.unresolved_positions is not None and len(position_set.unresolved_positions):
             raise MqValueError(f'Error in resolving the following identifiers for date {position_set.date}: \
             {[p.identifier for p in position_set.unresolved_positions]}')
 
     def __validate_ticker(self, ticker: str):
         """ Blocks ticker setter if entry is invalid """
         if not len(ticker) == 8:
```

### Comparing `gs_quant-0.9.99/gs_quant/markets/core.py` & `gs_quant-1.0.0/gs_quant/markets/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import logging
 import queue
 import sys
 import weakref
 from abc import ABCMeta
 from concurrent.futures import ThreadPoolExecutor
 from inspect import signature
-from itertools import zip_longest
+from itertools import zip_longest, takewhile
 from typing import Optional, Union
 
 from gs_quant.base import InstrumentBase, RiskKey, Scenario, get_enum_value
 from gs_quant.common import PricingLocation, RiskMeasure
 from gs_quant.context_base import ContextBaseWithDefault
 from gs_quant.datetime.date import business_day_offset, today
 from gs_quant.risk import CompositeScenario, DataFrameWithInfo, ErrorValue, FloatWithInfo, MarketDataScenario, \
@@ -180,16 +180,16 @@
         self.__use_cache = use_cache
         self.__visible_to_gs = visible_to_gs
         self.__request_priority = request_priority
         self.__market_data_location = market_data_location
         self.__market = market
         self.__show_progress = show_progress
         self.__use_server_cache = use_server_cache
-        self._max_per_batch = None
-        self._max_concurrent = None
+        self.__max_per_batch = None
+        self.__max_concurrent = None
 
         self.__set_parameters_only = set_parameters_only
 
         self.__pending = {}
         self._group_by_date = True
 
         self.__attrs_on_entry = {}
@@ -204,59 +204,53 @@
         attr_dict['use_cache'] = self.__use_cache
         attr_dict['visible_to_gs'] = self.__visible_to_gs
         attr_dict['request_priority'] = self.__request_priority
         attr_dict['market_data_location'] = self.__market_data_location
         attr_dict['market'] = self.__market
         attr_dict['show_progress'] = self.__show_progress
         attr_dict['use_server_cache'] = self.__use_server_cache
-        attr_dict['_max_concurrent'] = self._max_concurrent
-        attr_dict['_max_per_batch'] = self._max_per_batch
+        attr_dict['_max_concurrent'] = self.__max_concurrent
+        attr_dict['_max_per_batch'] = self.__max_per_batch
 
-    def _on_enter(self):
-        def _inherited_val(parameter, from_active, from_prior, default):
-            if from_active:
-                if self != self.active_context and getattr(self.active_context, parameter) is not None:
-                    return getattr(self.active_context, parameter)
-            if from_prior:
-                if PricingContext.has_prior and getattr(PricingContext.prior, parameter) is not None:
-                    return getattr(PricingContext.prior, parameter)
-            return default
-
-        def _inherit_if_not_init(parameter, from_active=False, from_prior=True, default=None):
-            on_entry = self.__attrs_on_entry.get(parameter)
-            if on_entry is not None:
-                return on_entry
-            else:
-                return _inherited_val(parameter, from_active, from_prior, default)
+    def _inherited_val(self, parameter, default=None, from_active=False):
+        if from_active:
+            # some properties are inherited from the active context
+            if self != self.active_context and getattr(self.active_context, parameter) is not None:
+                return getattr(self.active_context, parameter)
+        if not self.is_entered and (not PricingContext.has_prior or self is not PricingContext.prior):
+            # if not yet entered, get property from current (would-be prior) so that getters still display correctly
+            if PricingContext.current is not self and PricingContext.current and getattr(PricingContext.current,
+                                                                                         parameter) is not None:
+                return getattr(PricingContext.current, parameter)
+        else:
+            # if entered, inherit from the prior
+            if PricingContext.has_prior and PricingContext.prior is not self and getattr(PricingContext.prior,
+                                                                                         parameter) is not None:
+                return getattr(PricingContext.prior, parameter)
+        # default if nothing to inherit
+        return default
 
+    def _on_enter(self):
         self.__save_attrs_to(self.__attrs_on_entry)
 
-        self.__market_data_location = _inherit_if_not_init('market_data_location',
-                                                           from_active=True,
-                                                           default=PricingLocation.LDN)
-        default_pricing_date = business_day_offset(today(self.__market_data_location), 0, roll='preceding')
-        self.__pricing_date = _inherit_if_not_init('pricing_date', default=default_pricing_date)
-
-        if self.__attrs_on_entry.get('market') is None:
-            self.__market = CloseMarket(
-                date=close_market_date(self.__market_data_location, self.__pricing_date),
-                location=self.__market_data_location)
-
-        self.__csa_term = _inherit_if_not_init('csa_term')
-        self.__market_behaviour = _inherit_if_not_init('market_behaviour', default='ContraintsBased')
-        self.__is_async = _inherit_if_not_init('is_async', default=False)
-        self.__is_batch = _inherit_if_not_init('is_batch', default=False)
-        self.__timeout = _inherit_if_not_init('timeout')
-        self.__use_cache = _inherit_if_not_init('use_cache', default=False)
-        self.__visible_to_gs = _inherit_if_not_init('visible_to_gs')
-        self.__request_priority = _inherit_if_not_init('request_priority')
-        self.__show_progress = _inherit_if_not_init('show_progress', default=False)
-        self.__use_server_cache = _inherit_if_not_init('use_server_cache', default=False)
-        self._max_concurrent = _inherit_if_not_init('_max_concurrent', default=1000)
-        self._max_per_batch = _inherit_if_not_init('_max_per_batch', default=1000)
+        self.__market_data_location = self.market_data_location
+        self.__pricing_date = self.pricing_date
+        self.__market = self.market
+        self.__csa_term = self.csa_term
+        self.__market_behaviour = self.market_behaviour
+        self.__is_async = self.is_async
+        self.__is_batch = self.is_batch
+        self.__timeout = self.timeout
+        self.__use_cache = self.use_cache
+        self.__visible_to_gs = self.visible_to_gs
+        self.__request_priority = self.request_priority
+        self.__show_progress = self.show_progress
+        self.__use_server_cache = self.use_server_cache
+        self.__max_concurrent = self._max_concurrent
+        self.__max_per_batch = self._max_per_batch
 
     def __reset_atts(self):
         self.__pricing_date = self.__attrs_on_entry.get('pricing_date')
         self.__csa_term = self.__attrs_on_entry.get('csa_term')
         self.__market_behaviour = self.__attrs_on_entry.get('market_behaviour')
         self.__is_async = self.__attrs_on_entry.get('is_async')
         self.__is_batch = self.__attrs_on_entry.get('is_batch')
@@ -264,16 +258,16 @@
         self.__use_cache = self.__attrs_on_entry.get('use_cache')
         self.__visible_to_gs = self.__attrs_on_entry.get('visible_to_gs')
         self.__request_priority = self.__attrs_on_entry.get('request_priority')
         self.__market_data_location = self.__attrs_on_entry.get('market_data_location')
         self.__market = self.__attrs_on_entry.get('market')
         self.__show_progress = self.__attrs_on_entry.get('show_progress')
         self.__use_server_cache = self.__attrs_on_entry.get('use_server_cache')
-        self._max_concurrent = self.__attrs_on_entry.get('_max_concurrent')
-        self._max_per_batch = self.__attrs_on_entry.get('_max_per_batch')
+        self.__max_concurrent = self.__attrs_on_entry.get('_max_concurrent')
+        self.__max_per_batch = self.__attrs_on_entry.get('_max_per_batch')
 
         self.__attrs_on_entry = {}
 
     def _on_exit(self, exc_type, exc_val, exc_tb):
         try:
             if exc_val:
                 raise exc_val
@@ -360,15 +354,15 @@
                                 use_cache=self.__use_server_cache,
                                 priority=self.__request_priority
                             ))
 
                 requests_for_provider[provider] = requests
 
             show_status = self.__show_progress and \
-                (len(requests_for_provider) > 1 or len(next(iter(requests_for_provider.values()))) > 1)
+                          (len(requests_for_provider) > 1 or len(next(iter(requests_for_provider.values()))) > 1)
             request_pool = ThreadPoolExecutor(len(requests_for_provider)) \
                 if len(requests_for_provider) > 1 or self.__is_async else None
             progress_bar = tqdm(total=len(self.__pending), position=0, maxinterval=1,
                                 file=sys.stdout) if show_status else None
             completion_futures = []
 
             # Requests might get dispatched asynchronously and the PricingContext gets cleaned up on exit.
@@ -402,79 +396,106 @@
     @property
     def _scenario(self) -> Optional[MarketDataScenario]:
         scenarios = Scenario.path
         if not scenarios:
             return None
 
         return MarketDataScenario(scenario=scenarios[0] if len(scenarios) == 1 else
-                                  CompositeScenario(scenarios=tuple(reversed(scenarios))))
+        CompositeScenario(scenarios=tuple(reversed(scenarios))))
 
     @property
     def active_context(self):
-        return next((c for c in reversed(PricingContext.path) if c.is_entered and not c.set_parameters_only),
-                    self)
+        # active context cannot be below self on the stack - this also prevents infinite recursion when inheriting
+        path = takewhile(lambda x: x != self, reversed(PricingContext.path))
+        return next((c for c in path if c.is_entered and not c.set_parameters_only), self)
 
     @property
     def is_current(self) -> bool:
         return self == PricingContext.current
 
     @property
+    def _max_concurrent(self) -> int:
+        return self.__max_concurrent if self.__max_concurrent else self._inherited_val('_max_concurrent', default=1000)
+
+    @_max_concurrent.setter
+    def _max_concurrent(self, value):
+        self.__max_concurrent = value
+
+    @property
+    def _max_per_batch(self) -> int:
+        return self.__max_per_batch if self.__max_per_batch else self._inherited_val('_max_per_batch', default=1000)
+
+    @_max_per_batch.setter
+    def _max_per_batch(self, value):
+        self.__max_per_batch = value
+
+    @property
     def is_async(self) -> bool:
-        return self.__is_async
+        if self.__is_async is not None:
+            return self.__is_async
+        return self._inherited_val('is_async', default=False)
 
     @property
     def is_batch(self) -> bool:
-        return self.__is_batch
+        return self.__is_batch if self.__is_batch else self._inherited_val('is_batch', default=False)
 
     @property
     def market(self) -> Market:
-        return self.__market
+        return self.__market if self.__market else CloseMarket(
+            date=close_market_date(self.market_data_location, self.pricing_date),
+            location=self.market_data_location)
 
     @property
     def market_data_location(self) -> PricingLocation:
-        return self.__market_data_location
+        return self.__market_data_location if self.__market_data_location else self._inherited_val(
+            'market_data_location', from_active=True, default=PricingLocation.LDN)
 
     @property
     def csa_term(self) -> str:
-        return self._parameters.csa_term
+        return self.__csa_term if self.__csa_term else self._inherited_val('csa_term')
 
     @property
     def show_progress(self) -> bool:
-        return self.__show_progress
+        return self.__show_progress if self.__show_progress else self._inherited_val('show_progress', default=False)
 
     @property
     def timeout(self) -> int:
-        return self.__timeout
+        return self.__timeout if self.__timeout else self._inherited_val('timeout')
 
     @property
     def request_priority(self) -> int:
-        return self.__request_priority
+        return self.__request_priority if self.__request_priority else self._inherited_val('request_priority')
 
     @property
     def use_server_cache(self) -> bool:
-        return self.__use_server_cache
+        return self.__use_server_cache if self.__use_server_cache is not None else self._inherited_val(
+            'use_server_cache', False)
 
     @property
     def market_behaviour(self) -> str:
-        return self._parameters.market_behaviour
+        return self.__market_behaviour if self.__market_behaviour else self._inherited_val(
+            'market_behaviour', default='ContraintsBased')
 
     @property
     def pricing_date(self) -> dt.date:
         """Pricing date"""
-        return self.__pricing_date
+        if self.__pricing_date is not None:
+            return self.__pricing_date
+        default_pricing_date = business_day_offset(today(self.market_data_location), 0, roll='preceding')
+        return self._inherited_val('pricing_date', default=default_pricing_date)
 
     @property
     def use_cache(self) -> bool:
         """Cache results"""
-        return self.__use_cache
+        return self.__use_cache if self.__use_cache else self._inherited_val('use_cache', default=False)
 
     @property
     def visible_to_gs(self) -> Optional[bool]:
         """Request contents visible to GS"""
-        return self.__visible_to_gs
+        return self.__visible_to_gs if self.__visible_to_gs else self._inherited_val('visible_to_gs')
 
     @property
     def set_parameters_only(self) -> bool:
         return self.__set_parameters_only
 
     def clone(self, **kwargs):
         clone_kwargs = {k: getattr(self, k, None) for k in signature(self.__init__).parameters.keys()}
```

### Comparing `gs_quant-0.9.99/gs_quant/markets/factor.py` & `gs_quant-1.0.0/gs_quant/markets/factor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/hedge.py` & `gs_quant-1.0.0/gs_quant/markets/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/historical.py` & `gs_quant-1.0.0/gs_quant/markets/historical.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/index.py` & `gs_quant-1.0.0/gs_quant/markets/index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/indices_utils.py` & `gs_quant-1.0.0/gs_quant/markets/indices_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/markets.py` & `gs_quant-1.0.0/gs_quant/markets/markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/optimizer.py` & `gs_quant-1.0.0/gs_quant/markets/optimizer.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/portfolio.py` & `gs_quant-1.0.0/gs_quant/markets/portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/portfolio_manager.py` & `gs_quant-1.0.0/gs_quant/markets/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/portfolio_manager_utils.py` & `gs_quant-1.0.0/gs_quant/markets/portfolio_manager_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/position_set.py` & `gs_quant-1.0.0/gs_quant/markets/position_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 class Position:
     def __init__(self,
                  identifier: str,
                  weight: float = None,
                  quantity: float = None,
                  name: str = None,
                  asset_id: str = None,
-                 tags: Dict = None):
+                 tags: List[PositionTag] = None):
         self.__identifier = identifier
         self.__weight = weight
         self.__quantity = quantity
         self.__name = name
         self.__asset_id = asset_id
         self.__tags = tags
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, Position):
             return False
-        for prop in ['asset_id', 'weight', 'quantity']:
+        for prop in ['asset_id', 'weight', 'quantity', 'tags']:
             slf = get(self, prop)
             oth = get(other, prop)
             if not (slf is None and oth is None) and not slf == oth:
                 return False
         return True
 
     def __hash__(self):
@@ -95,31 +95,30 @@
         return self.__asset_id
 
     @asset_id.setter
     def asset_id(self, value: str):
         self.__asset_id = value
 
     @property
-    def tags(self) -> Dict:
+    def tags(self) -> List[PositionTag]:
         return self.__tags
 
     @tags.setter
-    def tags(self, value: Dict):
+    def tags(self, value: List[PositionTag]):
         self.__tags = value
 
     def as_dict(self) -> Dict:
         position_dict = dict(identifier=self.identifier, weight=self.weight,
                              quantity=self.quantity, name=self.name, asset_id=self.asset_id, tags=self.tags)
         return {k: v for k, v in position_dict.items() if v is not None}
 
     def to_target(self, common: bool = True) -> Union[CommonPosition, PositionPriceInput]:
-        """ Returns Postion type defined in target file for API payloads """
+        """ Returns Position type defined in target file for API payloads """
         if common:
-            tags_as_target = tuple(PositionTag(name=key, value=self.tags[key]) for key in self.tags) if self.tags \
-                else None
+            tags_as_target = self.tags if self.tags else None
             return CommonPosition(self.asset_id, quantity=self.quantity, tags=tags_as_target)
         return PositionPriceInput(self.asset_id, quantity=self.quantity, weight=self.weight)
 
 
 class PositionSet:
     """
 
@@ -143,14 +142,30 @@
         self.__positions = positions
         self.__date = date
         self.__divisor = divisor
         self.__reference_notional = reference_notional
         self.__unresolved_positions = unresolved_positions if unresolved_positions is not None else []
         self.__unpriced_positions = unpriced_positions if unpriced_positions is not None else []
 
+    def __eq__(self, other) -> bool:
+        if len(self.positions) != len(other.positions):
+            return False
+        if self.date != other.date:
+            return False
+        if self.reference_notional != other.reference_notional:
+            return False
+        positions = self.positions
+        positions.sort(key=lambda position: position.asset_id)
+        other_positions = other.positions
+        other_positions.sort(key=lambda position: position.asset_id)
+        for i in range(0, len(positions)):
+            if positions[i] != other_positions[i]:
+                return False
+        return True
+
     @property
     def positions(self) -> List[Position]:
         return self.__positions
 
     @positions.setter
     def positions(self, value: List[Position]):
         self.__positions = value
@@ -462,14 +477,15 @@
     def price(self, currency: Optional[Currency] = Currency.USD,
               weighting_strategy: Optional[PositionSetWeightingStrategy] = None, **kwargs):
         """
         Fetch positions weights from quantities, or vice versa
 
         :param currency: Reference notional currency (defaults to USD if not passed in)
         :param weighting_strategy: Quantity or Weighted weighting strategy (defaults based on positions info)
+        :param use_tags: Determines if tags are used to index the position response for non-netted positions
 
         **Usage**
 
         Fetch positions weights from quantities, or vice versa
 
         **Examples**
 
@@ -507,20 +523,21 @@
                                            notional_type='Gross',
                                            pricing_date=self.date,
                                            price_regardless_of_assets_missing_prices=True,
                                            weighting_strategy=weighting_strategy)
         for k, v in kwargs.items():
             price_parameters[k] = v
         results = GsPriceApi.price_positions(PositionSetPriceInput(positions=positions, parameters=price_parameters))
-        position_result_map = {p.asset_id: p for p in results.positions}
+        position_result_map = {f'{p.asset_id}{self.__hash_position_tag_list(p.tags)}': p for p in results.positions}
         priced_positions, unpriced_positions = [], []
         for p in self.positions:
-            if p.asset_id in position_result_map:
-                p.weight = position_result_map.get(p.asset_id).weight
-                p.quantity = position_result_map.get(p.asset_id).quantity
+            asset_key = f'{p.asset_id}{self.__hash_position_tag_list(p.tags)}'
+            if asset_key in position_result_map:
+                p.weight = position_result_map.get(asset_key).weight
+                p.quantity = position_result_map.get(asset_key).quantity
                 priced_positions.append(p)
             else:
                 unpriced_positions.append(p)
         self.positions = priced_positions
         self.__unpriced_positions = unpriced_positions
 
     def to_target(self, common: bool = True) -> Union[CommonPositionSet, List[PositionPriceInput]]:
@@ -627,23 +644,23 @@
         positions.columns = cls.__normalize_position_columns(positions)
         tag_columns = cls.__get_tag_columns(positions) if add_tags else []
         positions = positions[~positions['identifier'].isnull()]
         equalize = not ('quantity' in positions.columns.str.lower() or 'weight' in positions.columns.str.lower())
         equal_weight = 1 / len(positions)
 
         positions_list = []
-        for i, row in positions.iterrows():
+        for row in positions.to_dict(orient='records'):
             positions_list.append(
                 Position(
                     identifier=row.get('identifier'),
                     asset_id=row.get('id'),
                     name=row.get('name'),
                     weight=equal_weight if equalize else row.get('weight'),
                     quantity=None if equalize else row.get('quantity'),
-                    tags={tag: get(row, tag) for tag in tag_columns} if len(tag_columns) else None
+                    tags=tuple(PositionTag(tag, get(row, tag)) for tag in tag_columns) if len(tag_columns) else None
                 )
             )
 
         return cls(positions_list, date, reference_notional=reference_notional)
 
     @staticmethod
     def __get_tag_columns(positions: pd.DataFrame) -> List[str]:
@@ -718,12 +735,21 @@
         use_weight = weighting_strategy == PositionSetWeightingStrategy.Weight
         for p in positions:
             if p.asset_id is None:
                 missing_ids.append(p.identifier)
             else:
                 position_inputs.append(PositionPriceInput(asset_id=p.asset_id,
                                                           weight=p.weight if use_weight else None,
-                                                          quantity=None if use_weight else p.quantity))
+                                                          quantity=None if use_weight else p.quantity,
+                                                          tags=p.tags))
         if len(missing_ids):
             raise MqValueError(f'Positions: {missing_ids} are missing asset ids. Resolve your position \
             set or remove unmapped identifiers.')
         return position_inputs
+
+    @staticmethod
+    def __hash_position_tag_list(position_tags: List[PositionTag]) -> str:
+        hashed_results = ''
+        if position_tags is not None:
+            for tag in position_tags:
+                hashed_results = hashed_results + tag.name + '-' + tag.value
+        return hashed_results
```

### Comparing `gs_quant-0.9.99/gs_quant/markets/report.py` & `gs_quant-1.0.0/gs_quant/markets/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -944,15 +944,15 @@
             column_info = table.get('table').get('metadata').get('columnInfo')
             column_info[0].update({'columns': ['name', 'symbol', 'sector']})
             rows = table.get('table').get('rows')
             sorted_columns = []
             for column_group in column_info:
                 sorted_columns = sorted_columns + column_group.get('columns')
             rows_data_frame = pd.DataFrame(rows)
-            rows_data_frame = rows_data_frame[sorted_columns]
+            rows_data_frame = rows_data_frame.reindex(columns=sorted_columns)
             rows_data_frame = rows_data_frame.set_index('name')
             return rows_data_frame
         return table
 
     def get_factor_pnl(self,
                        mode: FactorRiskResultsMode = FactorRiskResultsMode.Portfolio,
                        factor_names: List[str] = None,
```

### Comparing `gs_quant-0.9.99/gs_quant/markets/report_utils.py` & `gs_quant-1.0.0/gs_quant/markets/report_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/screens.py` & `gs_quant-1.0.0/gs_quant/markets/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/markets/securities.py` & `gs_quant-1.0.0/gs_quant/markets/securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/models/__init__.py` & `gs_quant-1.0.0/gs_quant/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/models/epidemiology.py` & `gs_quant-1.0.0/gs_quant/models/epidemiology.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 """
 from abc import ABC, abstractmethod
-from typing import Type
+from typing import Type, Union
 
 import numpy as np
-from scipy.integrate import odeint
 from lmfit import minimize, Parameters, report_fit
+from scipy.integrate import odeint
 
 """
 Statistical models for the transmission of infectious diseases
 """
 
 
 class CompartmentalModel(ABC):
@@ -40,15 +40,15 @@
         raise NotImplementedError
 
 
 class SIR(CompartmentalModel):
     """SIR Model"""
 
     @classmethod
-    def calibrate(cls, xs: tuple, t: float, parameters: [Parameters, tuple]) -> tuple:
+    def calibrate(cls, xs: tuple, t: float, parameters: Union[Parameters, tuple]) -> tuple:
         """
         SIR model derivatives at t.
 
         :param xs: variables that we are solving for, i.e. [S]usceptible, [I]nfected, [R]emoved
         :param t: time parameter, inactive for this model
         :param parameters: parameters of the model (not including initial conditions), i.e. beta, gamma, N
         :return: tuple, the derivatives dSdt, dIdt, dRdt of each of the S, I, R variables
@@ -70,15 +70,15 @@
 
         return dSdt, dIdt, dRdt
 
     @classmethod
     def get_parameters(cls, S0: float, I0: float, R0: float, N: float, beta: float = 0.2, gamma: float = 0.1,
                        beta_max: float = 10, gamma_max: float = 1, S0_fixed: bool = True, S0_max: float = 1e6,
                        beta_fixed: bool = False, gamma_fixed: bool = False, R0_fixed: bool = True, R0_max: float = 1e6,
-                       I0_fixed: bool = True, I0_max: float = 1e6)\
+                       I0_fixed: bool = True, I0_max: float = 1e6) \
             -> tuple:
         """
         Produce a set of parameters for the SIR model.
 
         :param S0: initial number of susceptible in the population
         :param I0: initial number of infected in the population, usually set to 1
         :param R0: initial number of recovered/removed in the population, usually set to 0
@@ -107,15 +107,15 @@
         return parameters, initial_conditions
 
 
 class SEIR(CompartmentalModel):
     """SEIR Model"""
 
     @classmethod
-    def calibrate(cls, xs: tuple, t: float, parameters: [Parameters, tuple]) -> tuple:
+    def calibrate(cls, xs: tuple, t: float, parameters: Union[Parameters, tuple]) -> tuple:
         """
         SEIR model derivatives at t.
 
         :param xs: variables that we are solving for, i.e. [S]usceptible, [E]xposed, [I]nfected, [R]emoved
         :param t: time parameter, inactive for this model
         :param parameters: parameters of the model (not including initial conditions), i.e. beta, gamma, sigma, N
         :return: tuple, the derivatives dSdt, dEdt, dIdt, dRdt of each of the S, E, I, R variables
@@ -210,15 +210,15 @@
 
 
 class SEIRCM(CompartmentalModel):
     """ SEIR Model from https://www.medrxiv.org/content/10.1101/2020.03.04.20031104v1.full.pdf
         with cumulative cases (C) and cumulative fatalities (M) """
 
     @classmethod
-    def calibrate(cls, xs: tuple, t: float, parameters: [Parameters, tuple]) -> tuple:
+    def calibrate(cls, xs: tuple, t: float, parameters: Union[Parameters, tuple]) -> tuple:
         """
         SEIRCM model derivatives at t.
 
         :param xs: variables that we are solving for
                    i.e. [S]usceptible, [E]xposed, [I]nfected, [R]emoved, [C]ases, [M]ortality
         :param t: time parameter
         :param parameters: parameters of the model (not including initial conditions)
@@ -450,15 +450,14 @@
                                vary=not eval(f'{param}_fixed'))
                 initial_conditions.append(f'{param}_{k}')
 
         return parameters, initial_conditions
 
 
 class EpidemicModel:
-
     """Class to perform solutions and parameter-fitting of epidemic models"""
 
     def __init__(self, model: Type[CompartmentalModel], parameters: tuple = None, data: np.array = None,
                  initial_conditions: list = None, fit_method: str = 'leastsq', error: callable = None,
                  fit_period: float = None):
         """
         A class to standardize fitting and solving epidemiological models.
@@ -478,15 +477,15 @@
         self.initial_conditions = initial_conditions
         self.fit_method = fit_method
         self.error = error
         self.fit_period = fit_period
         self.result = None
         self.fitted_parameters = None
 
-    def solve(self, time_range: np.ndarray, initial_conditions: [list, tuple], parameters) -> np.ndarray:
+    def solve(self, time_range: np.ndarray, initial_conditions: Union[list, tuple], parameters) -> np.ndarray:
         """
         Integrate the model ODEs to get a solution.
 
         :param time_range: the time range to solve for
         :param initial_conditions: the initial conditions for the solution
         :param parameters: the parameters for the solution
         :return:
@@ -515,15 +514,16 @@
         residual = solution - data if self.error is None else self.error(solution, data, parameters)
 
         if self.fit_period is not None:
             residual = residual[-self.fit_period:]
 
         return residual.ravel()
 
-    def fit(self, time_range: np.arange = None, parameters: [Parameters, tuple] = None, initial_conditions: list = None,
+    def fit(self, time_range: np.arange = None, parameters: Union[Parameters, tuple] = None,
+            initial_conditions: list = None,
             residual=None, verbose: bool = False, data: np.array = None, fit_period: float = None):
         """
         Fit the model based on data in the form np.array([X1,...,Xn])
         """
         if data is None:
             if self.data is None:
                 raise ValueError("No data to fit the model on!")
```

### Comparing `gs_quant-0.9.99/gs_quant/models/risk_model.py` & `gs_quant-1.0.0/gs_quant/models/risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/models/risk_model_utils.py` & `gs_quant-1.0.0/gs_quant/models/risk_model_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,52 +201,36 @@
 
 def batch_and_upload_partial_data(model_id: str, data: dict, max_asset_size: int):
     """ Takes in total risk model data for one day and batches requests according to
     asset data size, returns a list of messages from resulting post calls"""
     date = data.get('date')
     _upload_factor_data_if_present(model_id, data, date)
     sleep(2)
-    _repeat_try_catch_request(_batch_data_v2, model_id=model_id, data=data, max_asset_size=max_asset_size, date=date)
+    for risk_model_data_type in ["assetData", "issuerSpecificCovariance", "factorPortfolios"]:
+        _repeat_try_catch_request(_batch_data_v2, model_id=model_id, data=data.get(risk_model_data_type),
+                                  data_type=risk_model_data_type, max_asset_size=max_asset_size, date=date)
+        sleep(2)
 
 
-def _batch_data_v2(model_id: str, data: dict, max_asset_size: int, date: Union[str, dt.date]):
-    if data.get('assetData'):
-        asset_data_list, target_size = _batch_input_data({'assetData': data.get('assetData')}, max_asset_size)
-        for i in range(len(asset_data_list)):
-            final_upload = True if i == len(asset_data_list) - 1 else False
+def _batch_data_v2(model_id: str, data: dict, data_type: str, max_asset_size: int, date: Union[str, dt.date]):
+    if data:
+        if data_type in ["issuerSpecificCovariance", "factorPortfolios"]:
+            max_asset_size //= 2
+        data_list, _ = _batch_input_data({data_type: data}, max_asset_size)
+        for i in range(len(data_list)):
+            final_upload = True if i == len(data_list) - 1 else False
             try:
                 res = GsFactorRiskModelApi.upload_risk_model_data(model_id=model_id,
-                                                                  model_data={'assetData': asset_data_list[i],
-                                                                              'date': date},
+                                                                  model_data={data_type: data_list[i], 'date': date},
                                                                   partial_upload=True,
                                                                   final_upload=final_upload)
                 logging.info(res)
             except (MqRequestError, Exception) as e:
                 raise e
 
-    if 'issuerSpecificCovariance' in data.keys() or 'factorPortfolios' in data.keys():
-        for optional_input_key in ['issuerSpecificCovariance', 'factorPortfolios']:
-            if data.get(optional_input_key):
-                optional_data = data.get(optional_input_key)
-                optional_data_list, target_size = _batch_input_data({optional_input_key: optional_data},
-                                                                    max_asset_size // 2)
-                logging.info(f'{optional_input_key} being uploaded for {date}...')
-                for i in range(len(optional_data_list)):
-                    final_upload = True if i == len(optional_data_list) - 1 else False
-                    try:
-                        res = GsFactorRiskModelApi.upload_risk_model_data(model_id=model_id,
-                                                                          model_data={
-                                                                              optional_input_key: optional_data_list[i],
-                                                                              'date': date},
-                                                                          partial_upload=True,
-                                                                          final_upload=final_upload)
-                        logging.info(res)
-                    except (MqRequestError, Exception) as e:
-                        raise e
-
 
 def batch_and_upload_coverage_data(date: dt.date, gsid_list: list, model_id: str):
     update_time = dt.datetime.today().strftime("%Y-%m-%dT%H:%M:%SZ")
     request_array = [{'date': date.strftime('%Y-%m-%d'),
                       'gsid': gsid,
                       'riskModel': model_id,
                       'updateTime': update_time} for gsid in set(gsid_list)]
```

### Comparing `gs_quant-0.9.99/gs_quant/priceable.py` & `gs_quant-1.0.0/gs_quant/priceable.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/quote_reports/core.py` & `gs_quant-1.0.0/gs_quant/quote_reports/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/__init__.py` & `gs_quant-1.0.0/gs_quant/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/core.py` & `gs_quant-1.0.0/gs_quant/risk/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/measures.py` & `gs_quant-1.0.0/gs_quant/risk/measures.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,19 +16,15 @@
 from typing import Union
 
 from gs_quant.base import Market
 from gs_quant.common import AssetClass, AggregationLevel, RiskMeasure
 from gs_quant.target.common import RiskMeasureType, RiskMeasureUnit
 from gs_quant.target.measures import IRBasis, IRVega, IRDelta, IRXccyDelta, InflationDelta
 
-DEPRECATED_MEASURES = {'IRDeltaParallelLocalCcy': 'IRDelta',
-                       'InflationDeltaParallelLocalCcy': 'InflationDelta',
-                       'IRXccyDeltaParallelLocalCurrency': 'IRXccyDelta',
-                       'IRVegaParallelLocalCcy': 'IRVega',
-                       }
+DEPRECATED_MEASURES = {}
 
 
 class __RelativeRiskMeasure(RiskMeasure):
     def __init__(self,
                  to_market: Market,
                  asset_class: Union[AssetClass, str] = None,
                  measure_type: Union[RiskMeasureType, str] = None,
@@ -74,20 +70,12 @@
         from gs_quant.markets import LiveMarket
         super().__init__(LiveMarket(), measure_type=RiskMeasureType.PnlPredict, name=RiskMeasureType.PnlPredict.value)
 
 
 # Defining Parameterised Risk Measures
 IRBasisParallel = IRBasis(aggregation_level=AggregationLevel.Asset, name='IRBasisParallel')
 InflationDeltaParallel = InflationDelta(aggregation_level=AggregationLevel.Type, name='InflationDeltaParallel')
-InflationDeltaParallelLocalCcy = InflationDelta(aggregation_level=AggregationLevel.Type, currency='local',
-                                                name='InflationDeltaParallelLocalCcy')
 IRDeltaParallel = IRDelta(aggregation_level=AggregationLevel.Asset, name='IRDeltaParallel')
 IRDeltaLocalCcy = IRDelta(currency='local', name='IRDeltaLocalCcy')
-IRDeltaParallelLocalCcy = IRDelta(aggregation_level=AggregationLevel.Type, currency='local',
-                                  name='IRDeltaParallelLocalCcy')
 IRXccyDeltaParallel = IRXccyDelta(aggregation_level=AggregationLevel.Type, name='IRXccyDeltaParallel')
-IRXccyDeltaParallelLocalCurrency = IRXccyDelta(aggregation_level=AggregationLevel.Type, currency='local',
-                                               name='IRXccyDeltaParallelLocalCurrency')
 IRVegaParallel = IRVega(aggregation_level=AggregationLevel.Asset, name='IRVegaParallel')
 IRVegaLocalCcy = IRVega(currency='local', name='IRVegaLocalCcy')
-IRVegaParallelLocalCcy = IRVega(aggregation_level=AggregationLevel.Type, currency='local',
-                                name='IRVegaParallelLocalCcy')
```

### Comparing `gs_quant-0.9.99/gs_quant/risk/result_handlers.py` & `gs_quant-1.0.0/gs_quant/risk/result_handlers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/results.py` & `gs_quant-1.0.0/gs_quant/risk/results.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/scenario_utils.py` & `gs_quant-1.0.0/gs_quant/risk/scenario_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/scenarios.py` & `gs_quant-1.0.0/gs_quant/risk/scenarios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/risk/transform.py` & `gs_quant-1.0.0/gs_quant/risk/transform.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/session.py` & `gs_quant-1.0.0/gs_quant/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 import json
 import logging
 import os
 import ssl
 from abc import abstractmethod
 from configparser import ConfigParser
 from enum import Enum, auto, unique
-from typing import Optional, Union, Iterable
+from typing import Optional, Union, Iterable, Tuple
 
 import backoff
 import certifi
 import msgpack
 import pandas as pd
 import requests
 import requests.adapters
 import requests.cookies
+import asyncio
 import urllib3
 from gs_quant import version as APP_VERSION
 from gs_quant.base import Base
 from gs_quant.context_base import ContextBase
 from gs_quant.errors import MqError, MqRequestError, MqAuthenticationError, MqUninitialisedError
 from gs_quant.json_encoder import JSONEncoder, encode_default
 
@@ -94,14 +95,15 @@
                 cls.READ_USER_PROFILE.value
             )
 
     def __init__(self, domain: str, api_version: str = API_VERSION, application: str = DEFAULT_APPLICATION, verify=True,
                  http_adapter: requests.adapters.HTTPAdapter = None, application_version=APP_VERSION, proxies=None):
         super().__init__()
         self._session = None
+        self._session_async = None
         self.domain = domain
         self.api_version = api_version
         self.application = application
         self.verify = verify
         if http_adapter is None:
             if ssl.OPENSSL_VERSION_INFO >= (3, 0, 0):
                 self.http_adapter = CustomHttpAdapter(self.__ssl_context())
@@ -118,22 +120,52 @@
     @backoff.on_predicate(lambda: backoff.expo(factor=2),
                           lambda x: x.status_code in (500, 502, 503, 504),
                           max_tries=5)
     @abstractmethod
     def _authenticate(self):
         raise NotImplementedError("Must implement _authenticate")
 
+    def _authenticate_async(self):
+        if self._session_async:
+            self._session_async.headers.update([(k, v) for k, v in self._session.headers.items()])
+            for cookie in self._session.cookies:
+                self._session_async.cookies.set(cookie.name, cookie.value, domain=cookie.domain)
+
+    def _authenticate_all_sessions(self):
+        self._authenticate()
+        self._authenticate_async()
+
     def _on_enter(self):
         self.__close_on_exit = self._session is None
         if not self._session:
             self.init()
 
     def _on_exit(self, exc_type, exc_val, exc_tb):
         if self.__close_on_exit:
             self._session = None
+            self._session_async = None
+
+    def _init_async(self):
+        import httpx
+        if not self._session_async:
+            self._session_async = httpx.AsyncClient(follow_redirects=True, verify=self.verify, proxies=self.proxies)
+            self._session_async.headers.update({'X-Application': self.application})
+            self._session_async.headers.update({'X-Version': self.application_version})
+            self._authenticate_async()
+
+    async def _on_aenter(self):
+        self.__close_on_exit = self._session is None
+        if not self._session_async:
+            self.init()
+            self._init_async()
+
+    async def _on_aexit(self, exc_type, exc_val, exc_tb):
+        if self.__close_on_exit:
+            self._session = None
+            self._session_async = None
 
     def init(self):
         if not self._session:
             self._session = requests.Session()
             if self.http_adapter is not None:
                 self._session.mount('https://', self.http_adapter)
             if self.proxies is not None:
@@ -141,20 +173,29 @@
             self._session.verify = self.verify
             self._session.headers.update({'X-Application': self.application})
             self._session.headers.update({'X-Version': self.application_version})
             self._authenticate()
 
     def close(self):
         self._session: requests.Session
-
         if self._session:
             # don't close a shared adapter
             if self.http_adapter is None:
                 self._session.close()
             self._session = None
+        if self._session_async:
+            try:
+                asyncio.run(self._close_async())
+            except Exception:
+                pass
+
+    async def _close_async(self):
+        if self._session_async:
+            await self._session_async.aclose()
+            self._session_async = None
 
     def __del__(self):
         self.close()
 
     @staticmethod
     def __ssl_context() -> ssl.SSLContext:
         if GsSession.__ssl_ctx is None:
@@ -176,37 +217,32 @@
                 return None if results is None else cls.from_dict(results)
         else:
             if isinstance(results, list):
                 return tuple(cls(**r) for r in results)
             else:
                 return cls(**results)
 
-    def __request(
+    def _build_request_params(
             self,
             method: str,
             path: str,
-            payload: Optional[Union[dict, str, bytes, Base, pd.DataFrame]] = None,
-            request_headers: Optional[dict] = None,
-            cls: Optional[type] = None,
-            try_auth: Optional[bool] = True,
-            include_version: Optional[bool] = True,
-            timeout: Optional[int] = DEFAULT_TIMEOUT,
-            return_request_id: Optional[bool] = False,
-            use_body: bool = False
-    ) -> Union[Base, tuple, dict]:
+            payload: Optional[Union[dict, str, bytes, Base, pd.DataFrame]],
+            request_headers: Optional[dict],
+            include_version: Optional[bool],
+            timeout: Optional[int],
+            use_body: bool,
+            data_key: str
+    ) -> Tuple[dict, str]:
         is_dataframe = isinstance(payload, pd.DataFrame)
         if not is_dataframe:
             payload = payload or {}
-
         url = '{}{}{}'.format(self.domain, '/' + self.api_version if include_version else '', path)
-
         kwargs = {
             'timeout': timeout
         }
-
         if method in ['GET', 'DELETE'] and not use_body:
             kwargs['params'] = payload
         elif method in ['POST', 'PUT'] or (method in ['GET', 'DELETE'] and use_body):
             headers = self._session.headers.copy()
 
             if request_headers:
                 headers.update(request_headers)
@@ -214,96 +250,166 @@
             if 'Content-Type' not in headers:
                 headers.update({'Content-Type': 'application/json; charset=utf-8'})
 
             use_msgpack = headers.get('Content-Type') == 'application/x-msgpack'
             kwargs['headers'] = headers
 
             if is_dataframe or payload:
-                kwargs['data'] = payload if isinstance(payload, (str, bytes)) else \
+                kwargs[data_key] = payload if isinstance(payload, (str, bytes)) else \
                     msgpack.dumps(payload, default=encode_default) if use_msgpack else \
                     json.dumps(payload, cls=JSONEncoder)
         else:
             raise MqError('not implemented')
+        return kwargs, url
 
-        response = self._session.request(method, url, **kwargs)
-        request_id = response.headers.get('x-dash-requestid')
-        logger.debug('Handling response for [Request ID]: %s [Method]: %s [URL]: %s', request_id, method, url)
-
-        if response.status_code == 401:
-            # Expired token or other authorization issue
-            if not try_auth:
-                raise MqRequestError(response.status_code, response.text,
-                                     context=f'{request_id}: {method} {url}')
-            self._authenticate()
-            return self.__request(method, path, payload=payload, cls=cls,
-                                  include_version=include_version, return_request_id=return_request_id,
-                                  use_body=use_body, try_auth=False)
-        elif not 199 < response.status_code < 300:
-            raise MqRequestError(response.status_code, response.text,
+    def _parse_response(self, request_id, response, method: str, url: str,
+                        cls: Optional[type], return_request_id: Optional[bool]):
+        ret = {}
+        if not 199 < response.status_code < 300:
+            raise MqRequestError(response.status_code, f'{response.reason}: {response.text}',
                                  context=f'{request_id}: {method} {url}')
         elif 'Content-Type' in response.headers:
             if 'application/x-msgpack' in response.headers['Content-Type']:
-                res = msgpack.unpackb(response.content, raw=False)
-
-                if cls:
-                    if isinstance(res, dict) and 'results' in res:
-                        res['results'] = self.__unpack(res['results'], cls)
-                    else:
-                        res = self.__unpack(res, cls)
-
-                return (res, request_id) if return_request_id else res
+                ret = msgpack.unpackb(response.content, raw=False)
             elif 'application/json' in response.headers['Content-Type']:
-                res = json.loads(response.text)
-
-                if cls:
-                    if isinstance(res, dict) and 'results' in res:
-                        res['results'] = self.__unpack(res['results'], cls)
-                    else:
-                        res = self.__unpack(res, cls)
-
-                return (res, request_id) if return_request_id else res
+                ret = json.loads(response.text)
+            if cls and ret:
+                if isinstance(ret, dict) and 'results' in ret:
+                    ret['results'] = self.__unpack(ret['results'], cls)
+                else:
+                    ret = self.__unpack(ret, cls)
+            return (ret, request_id) if return_request_id else ret
         else:
             ret = {'raw': response}
             if return_request_id:
                 ret['request_id'] = request_id
-
             return ret
 
+    def __request(
+            self,
+            method: str,
+            path: str,
+            payload: Optional[Union[dict, str, bytes, Base, pd.DataFrame]] = None,
+            request_headers: Optional[dict] = None,
+            cls: Optional[type] = None,
+            try_auth: Optional[bool] = True,
+            include_version: Optional[bool] = True,
+            timeout: Optional[int] = DEFAULT_TIMEOUT,
+            return_request_id: Optional[bool] = False,
+            use_body: bool = False
+    ) -> Union[Base, tuple, dict]:
+        kwargs, url = self._build_request_params(method, path, payload, request_headers, include_version, timeout,
+                                                 use_body, "data")
+        response = self._session.request(method, url, **kwargs)
+        request_id = response.headers.get('x-dash-requestid')
+        logger.debug('Handling response for [Request ID]: %s [Method]: %s [URL]: %s', request_id, method, url)
+        if response.status_code == 401:
+            # Expired token or other authorization issue
+            if not try_auth:
+                raise MqRequestError(response.status_code, response.text, context=f'{request_id}: {method} {url}')
+            self._authenticate()
+            return self.__request(method, path, payload=payload, cls=cls, include_version=include_version,
+                                  return_request_id=return_request_id, use_body=use_body, try_auth=False)
+        return self._parse_response(request_id, response, method, url, cls, return_request_id)
+
+    async def __request_async(
+            self,
+            method: str,
+            path: str,
+            payload: Optional[Union[dict, str, bytes, Base, pd.DataFrame]] = None,
+            request_headers: Optional[dict] = None,
+            cls: Optional[type] = None,
+            try_auth: Optional[bool] = True,
+            include_version: Optional[bool] = True,
+            timeout: Optional[int] = DEFAULT_TIMEOUT,
+            return_request_id: Optional[bool] = False,
+            use_body: bool = False
+    ) -> Union[Base, tuple, dict]:
+        self._init_async()
+        kwargs, url = self._build_request_params(method, path, payload, request_headers, include_version, timeout,
+                                                 use_body, "content")
+        response = await self._session_async.request(method, url, **kwargs)
+        request_id = response.headers.get('x-dash-requestid')
+        logger.debug('Handling response for [Request ID]: %s [Method]: %s [URL]: %s', request_id, method, url)
+        if response.status_code == 401:
+            # Expired token or other authorization issue
+            if not try_auth:
+                raise MqRequestError(response.status_code, response.text, context=f'{request_id}: {method} {url}')
+            self._authenticate_all_sessions()
+            res = await self.__request_async(method, path, payload=payload, cls=cls, include_version=include_version,
+                                             return_request_id=return_request_id, use_body=use_body, try_auth=False)
+            return res
+        return self._parse_response(request_id, response, method, url, cls, return_request_id)
+
     def _get(self, path: str, payload: Optional[Union[dict, Base]] = None, request_headers: Optional[dict] = None,
              cls: Optional[type] = None, include_version: Optional[bool] = True,
              timeout: Optional[int] = DEFAULT_TIMEOUT, return_request_id: Optional[bool] = False) \
             -> Union[Base, tuple, dict]:
-        return self.__request('GET', path, payload=payload, request_headers=request_headers,
-                              cls=cls, include_version=include_version, timeout=timeout,
-                              return_request_id=return_request_id)
+        return self.__request('GET', path, payload=payload, request_headers=request_headers, cls=cls,
+                              include_version=include_version, timeout=timeout, return_request_id=return_request_id)
+
+    async def _get_async(self, path: str, payload: Optional[Union[dict, Base]] = None,
+                         request_headers: Optional[dict] = None, cls: Optional[type] = None,
+                         include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
+                         return_request_id: Optional[bool] = False) -> Union[Base, tuple, dict]:
+        ret = await self.__request_async('GET', path, payload=payload, request_headers=request_headers, cls=cls,
+                                         include_version=include_version, timeout=timeout,
+                                         return_request_id=return_request_id)
+        return ret
 
     def _post(self, path: str, payload: Optional[Union[dict, bytes, Base, pd.DataFrame]] = None,
               request_headers: Optional[dict] = None, cls: Optional[type] = None,
               include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
               return_request_id: Optional[bool] = False) -> Union[Base, tuple, dict]:
-        return self.__request('POST', path, payload=payload, request_headers=request_headers,
-                              cls=cls, include_version=include_version, timeout=timeout,
-                              return_request_id=return_request_id)
+        return self.__request('POST', path, payload=payload, request_headers=request_headers, cls=cls,
+                              include_version=include_version, timeout=timeout, return_request_id=return_request_id)
+
+    async def _post_async(self, path: str, payload: Optional[Union[dict, bytes, Base, pd.DataFrame]] = None,
+                          request_headers: Optional[dict] = None, cls: Optional[type] = None,
+                          include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
+                          return_request_id: Optional[bool] = False) -> Union[Base, tuple, dict]:
+        ret = await self.__request_async('POST', path, payload=payload, request_headers=request_headers, cls=cls,
+                                         include_version=include_version, timeout=timeout,
+                                         return_request_id=return_request_id)
+        return ret
 
     def _delete(self, path: str, payload: Optional[Union[dict, Base]] = None,
                 request_headers: Optional[dict] = None, cls: Optional[type] = None,
                 include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
-                return_request_id: Optional[bool] = False, use_body: Optional[bool] = False) -> \
-            Union[Base, tuple, dict]:
-        return self.__request('DELETE', path, payload=payload, request_headers=request_headers,
-                              cls=cls, include_version=include_version, timeout=timeout,
-                              return_request_id=return_request_id, use_body=use_body)
+                return_request_id: Optional[bool] = False, use_body: Optional[bool] = False) \
+            -> Union[Base, tuple, dict]:
+        return self.__request('DELETE', path, payload=payload, request_headers=request_headers, cls=cls,
+                              include_version=include_version, timeout=timeout, return_request_id=return_request_id,
+                              use_body=use_body)
+
+    async def _delete_async(self, path: str, payload: Optional[Union[dict, Base]] = None,
+                            request_headers: Optional[dict] = None, cls: Optional[type] = None,
+                            include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
+                            return_request_id: Optional[bool] = False, use_body: Optional[bool] = False) \
+            -> Union[Base, tuple, dict]:
+        ret = await self.__request_async('DELETE', path, payload=payload, request_headers=request_headers, cls=cls,
+                                         include_version=include_version, timeout=timeout,
+                                         return_request_id=return_request_id, use_body=use_body)
+        return ret
 
     def _put(self, path: str, payload: Optional[Union[dict, Base]] = None,
              request_headers: Optional[dict] = None, cls: Optional[type] = None, include_version: Optional[bool] = True,
              timeout: Optional[int] = DEFAULT_TIMEOUT, return_request_id: Optional[bool] = False) \
             -> Union[Base, tuple, dict]:
-        return self.__request('PUT', path, payload=payload, request_headers=request_headers,
-                              cls=cls, include_version=include_version, timeout=timeout,
-                              return_request_id=return_request_id)
+        return self.__request('PUT', path, payload=payload, request_headers=request_headers, cls=cls,
+                              include_version=include_version, timeout=timeout, return_request_id=return_request_id)
+
+    async def _put_async(self, path: str, payload: Optional[Union[dict, Base]] = None,
+                         request_headers: Optional[dict] = None, cls: Optional[type] = None,
+                         include_version: Optional[bool] = True, timeout: Optional[int] = DEFAULT_TIMEOUT,
+                         return_request_id: Optional[bool] = False) -> Union[Base, tuple, dict]:
+        ret = await self.__request_async('PUT', path, payload=payload, request_headers=request_headers, cls=cls,
+                                         include_version=include_version, timeout=timeout,
+                                         return_request_id=return_request_id)
+        return ret
 
     def _connect_websocket(self, path: str, headers: Optional[dict] = None):
         import websockets
         url = 'ws{}{}{}'.format(self.domain[4:], '/' + self.api_version, path)
         extra_headers = self._headers() + list((headers or {}).items())
         return websockets.connect(url,
                                   extra_headers=extra_headers,
```

### Comparing `gs_quant-0.9.99/gs_quant/target/__init__.py` & `gs_quant-1.0.0/gs_quant/target/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/assets.py` & `gs_quant-1.0.0/gs_quant/target/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/assets_screener.py` & `gs_quant-1.0.0/gs_quant/target/assets_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/backtests.py` & `gs_quant-1.0.0/gs_quant/target/backtests.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Delta = 'Delta'
     Gamma = 'Gamma'
     Vega = 'Vega'
     Forward = 'Forward'
     Implied_Volatility = 'Implied Volatility'
     Fair_Variance = 'Fair Variance'
     Strike_Level = 'Strike Level'
+    Spot = 'Spot'
     Price_ATMS = 'Price ATMS'
     Price_ATMF_Volatility = 'Price ATMF Volatility'    
 
 
 class BacktestTradingQuantityType(EnumBase, Enum):    
     
     """The trading quantity unit of a backtest strategy"""
```

### Comparing `gs_quant-0.9.99/gs_quant/target/base_screener.py` & `gs_quant-1.0.0/gs_quant/target/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/charts.py` & `gs_quant-1.0.0/gs_quant/target/charts.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/common.py` & `gs_quant-1.0.0/gs_quant/target/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -4822,28 +4822,29 @@
     volume: Optional[float] = field(default=None, metadata=field_metadata)
     name: Optional[str] = field(default=None, metadata=name_metadata)
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
+class PositionTag(Base):
+    name: str = field(default=None, metadata=field_metadata)
+    value: str = field(default=None, metadata=field_metadata)
+
+
+@handle_camel_case_args
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass(unsafe_hash=True, repr=False)
 class PositionPriceInput(Base):
     asset_id: str = field(default=None, metadata=field_metadata)
     quantity: Optional[float] = field(default=None, metadata=field_metadata)
     weight: Optional[float] = field(default=None, metadata=field_metadata)
     notional: Optional[float] = field(default=None, metadata=field_metadata)
     name: Optional[str] = field(default=None, metadata=name_metadata)
-
-
-@handle_camel_case_args
-@dataclass_json(letter_case=LetterCase.CAMEL)
-@dataclass(unsafe_hash=True, repr=False)
-class PositionTag(Base):
-    name: str = field(default=None, metadata=field_metadata)
-    value: str = field(default=None, metadata=field_metadata)
+    tags: Optional[Tuple[PositionTag, ...]] = field(default=None, metadata=field_metadata)
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
 class RefMarket(BaseMarket):
     market_ref: Optional[str] = field(default=None, metadata=field_metadata)
```

### Comparing `gs_quant-0.9.99/gs_quant/target/content.py` & `gs_quant-1.0.0/gs_quant/target/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/coordinates.py` & `gs_quant-1.0.0/gs_quant/target/coordinates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/countries.py` & `gs_quant-1.0.0/gs_quant/target/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/data.py` & `gs_quant-1.0.0/gs_quant/target/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
     times: Optional[Tuple[datetime.datetime, ...]] = field(default=None, metadata=field_metadata)
     delay: Optional[int] = field(default=None, metadata=field_metadata)
     intervals: Optional[int] = field(default=None, metadata=field_metadata)
     samples: Optional[int] = field(default=None, metadata=field_metadata)
     limit: Optional[int] = field(default=None, metadata=field_metadata)
     polling_interval: Optional[int] = field(default=None, metadata=field_metadata)
     grouped: Optional[bool] = field(default=None, metadata=field_metadata)
-    group_by: Optional[bool] = field(default=None, metadata=field_metadata)
+    group_by: Optional[Tuple[str, ...]] = field(default=None, metadata=field_metadata)
     fields: Optional[Tuple[Union[DictBase, str], ...]] = field(default=None, metadata=field_metadata)
     restrict_fields: Optional[bool] = field(default=False, metadata=field_metadata)
     entity_filter: Optional[FieldFilterMapDataQuery] = field(default=None, metadata=field_metadata)
     interval: Optional[str] = field(default=None, metadata=field_metadata)
     distinct_consecutive: Optional[bool] = field(default=False, metadata=field_metadata)
     time_filter: Optional[TimeFilter] = field(default=None, metadata=field_metadata)
     use_field_alias: Optional[bool] = field(default=False, metadata=field_metadata)
@@ -490,14 +490,15 @@
     offset_to_exchange_open: Optional[str] = field(default=None, metadata=field_metadata)
     offset_to_exchange_close: Optional[str] = field(default=None, metadata=field_metadata)
     multi_trading_session: Optional[bool] = field(default=None, metadata=field_metadata)
     multi_session: Optional[bool] = field(default=None, metadata=field_metadata)
     quote_consolidation: Optional[bool] = field(default=None, metadata=field_metadata)
     time_index: Optional[str] = field(default=None, metadata=field_metadata)
     name: Optional[str] = field(default=None, metadata=name_metadata)
+    adjust_as_of: Optional[datetime.datetime] = field(default=None, metadata=field_metadata)
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
 class DataSetCatalogEntry(Base):
     id_: str = field(default=None, metadata=config(field_name='id', exclude=exclude_none))
```

### Comparing `gs_quant-0.9.99/gs_quant/target/data_screen.py` & `gs_quant-1.0.0/gs_quant/target/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/groups.py` & `gs_quant-1.0.0/gs_quant/target/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/hedge.py` & `gs_quant-1.0.0/gs_quant/target/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/indices.py` & `gs_quant-1.0.0/gs_quant/target/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/instrument.py` & `gs_quant-1.0.0/gs_quant/target/instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/measures.py` & `gs_quant-1.0.0/gs_quant/target/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/monitor.py` & `gs_quant-1.0.0/gs_quant/target/monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/portfolios.py` & `gs_quant-1.0.0/gs_quant/target/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/price.py` & `gs_quant-1.0.0/gs_quant/target/price.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     composite10_day_adv: Optional[float] = field(default=None, metadata=field_metadata)
     composite22_day_adv: Optional[float] = field(default=None, metadata=field_metadata)
     adv5_day_pct: Optional[float] = field(default=None, metadata=field_metadata)
     adv10_day_pct: Optional[float] = field(default=None, metadata=field_metadata)
     adv22_day_pct: Optional[float] = field(default=None, metadata=field_metadata)
     median_daily_volume22_day: Optional[float] = field(default=None, metadata=field_metadata)
     name: Optional[str] = field(default=None, metadata=name_metadata)
+    tags: Optional[Tuple[PositionTag, ...]] = field(default=None, metadata=name_metadata)
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
 class PositionSetPriceResponse(Base):
     positions: Optional[Tuple[PositionPriceResponse, ...]] = field(default=None, metadata=field_metadata)
```

### Comparing `gs_quant-0.9.99/gs_quant/target/reports.py` & `gs_quant-1.0.0/gs_quant/target/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/risk.py` & `gs_quant-1.0.0/gs_quant/target/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/risk_models.py` & `gs_quant-1.0.0/gs_quant/target/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/screens.py` & `gs_quant-1.0.0/gs_quant/target/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/secmaster.py` & `gs_quant-1.0.0/gs_quant/target/secmaster.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/trades.py` & `gs_quant-1.0.0/gs_quant/target/trades.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/target/workflow_quote.py` & `gs_quant-1.0.0/gs_quant/target/workflow_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     Delta = 'Delta'
     Vega = 'Vega'
     Theta = 'Theta'
     RelativeCheapness = 'RelativeCheapness'
     ProbabilityDistribution = 'ProbabilityDistribution'
     RealisedProbability = 'RealisedProbability'
     MacroEvents = 'MacroEvents'
+    MicroEvents = 'MicroEvents'
     Gamma = 'Gamma'
     _None = 'None'    
 
 
 @handle_camel_case_args
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass(unsafe_hash=True, repr=False)
```

### Comparing `gs_quant-0.9.99/gs_quant/target/workspaces_markets.py` & `gs_quant-1.0.0/gs_quant/target/workspaces_markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/analytics/test_datagrid.py` & `gs_quant-1.0.0/gs_quant/test/analytics/test_datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/analytics/test_sorting_and_filtering.py` & `gs_quant-1.0.0/gs_quant/test/analytics/test_sorting_and_filtering.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/analytics/test_workspace.py` & `gs_quant-1.0.0/gs_quant/test/analytics/test_workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_assets.py` & `gs_quant-1.0.0/gs_quant/test/api/test_assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_backtests.py` & `gs_quant-1.0.0/gs_quant/test/api/test_backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_base_screener.py` & `gs_quant-1.0.0/gs_quant/test/api/test_base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_cache.py` & `gs_quant-1.0.0/gs_quant/test/api/test_cache.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_carbon.py` & `gs_quant-1.0.0/gs_quant/test/api/test_carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_content.py` & `gs_quant-1.0.0/gs_quant/test/api/test_content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_data.py` & `gs_quant-1.0.0/gs_quant/test/api/test_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_data_screen.py` & `gs_quant-1.0.0/gs_quant/test/api/test_data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_esg.py` & `gs_quant-1.0.0/gs_quant/test/api/test_esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_fred.py` & `gs_quant-1.0.0/gs_quant/test/api/test_fred.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_groups.py` & `gs_quant-1.0.0/gs_quant/test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_index.py` & `gs_quant-1.0.0/gs_quant/test/api/test_index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_instruments.py` & `gs_quant-1.0.0/gs_quant/test/api/test_instruments.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_json.py` & `gs_quant-1.0.0/gs_quant/test/api/test_json.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_monitor.py` & `gs_quant-1.0.0/gs_quant/test/api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_portfolios.py` & `gs_quant-1.0.0/gs_quant/test/api/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_reports.py` & `gs_quant-1.0.0/gs_quant/test/api/test_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_risk.py` & `gs_quant-1.0.0/gs_quant/test/api/test_risk.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,58 +66,58 @@
     expected = risk.sort_risk(pd.DataFrame([
         {'mkt_type': 'IR', 'mkt_asset': 'USD', 'mkt_class': 'Swap', 'mkt_point': '1y', 'value': 0.01},
         {'mkt_type': 'IR', 'mkt_asset': 'USD', 'mkt_class': 'Swap', 'mkt_point': '2y', 'value': 0.015}
     ]))
 
     result = priceable.calc(measure)
     assert result.raw_value.equals(expected)
-    with PricingContext.current as cur:
-        default_date = cur.pricing_date
-        default_mkt = cur.market
+    default_date = PricingContext.current.pricing_date
+    default_mkt = PricingContext.current.market
     risk_requests = (risk.RiskRequest(
         positions=(RiskPosition(instrument=priceable, quantity=1),),
         measures=(measure,),
+        use_cache=PricingContext.current.use_server_cache,
         pricing_and_market_data_as_of=(PricingDateAndMarketDataAsOf(pricing_date=default_date,
                                                                     market=default_mkt),),
         parameters=RiskRequestParameters(raw_results=True),
         wait_for_results=True),)
     mocker.assert_called_with(risk_requests)
 
 
 def scalar_calc(mocker, priceable: Priceable, measure: risk.RiskMeasure):
     set_session()
     mocker.return_value = [[[[{'$type': 'Risk', 'val': 0.01}]]]]
 
     result = priceable.calc(measure)
     assert result == 0.01
-    with PricingContext.current as cur:
-        default_date = cur.pricing_date
-        default_mkt = cur.market
+    default_date = PricingContext.current.pricing_date
+    default_mkt = PricingContext.current .market
     risk_requests = (risk.RiskRequest(
         positions=(RiskPosition(instrument=priceable, quantity=1),),
         measures=(measure,),
+        use_cache=PricingContext.current.use_server_cache,
         pricing_and_market_data_as_of=(PricingDateAndMarketDataAsOf(pricing_date=default_date,
                                                                     market=default_mkt),),
         parameters=RiskRequestParameters(raw_results=True),
         wait_for_results=True),)
     mocker.assert_called_with(risk_requests)
 
 
 def price(mocker, priceable: Priceable):
     set_session()
     mocker.return_value = [[[[{'$type': 'Risk', 'val': 0.01}]]]]
 
     result = priceable.dollar_price()
     assert result == 0.01
-    with PricingContext.current as cur:
-        default_date = cur.pricing_date
-        default_mkt = cur.market
+    default_date = PricingContext.current.pricing_date
+    default_mkt = PricingContext.current.market
     risk_requests = (risk.RiskRequest(
         positions=(RiskPosition(instrument=priceable, quantity=1),),
         measures=(risk.DollarPrice,),
+        use_cache=PricingContext.current.use_server_cache,
         pricing_and_market_data_as_of=(PricingDateAndMarketDataAsOf(pricing_date=default_date,
                                                                     market=default_mkt),),
         parameters=RiskRequestParameters(raw_results=True),
         wait_for_results=True),)
     mocker.assert_called_with(risk_requests)
```

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_risk_models.py` & `gs_quant-1.0.0/gs_quant/test/api/test_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_target.py` & `gs_quant-1.0.0/gs_quant/test/api/test_target.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_thread_manager.py` & `gs_quant-1.0.0/gs_quant/test/api/test_thread_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/api/test_users.py` & `gs_quant-1.0.0/gs_quant/test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_eq_vol_engine.py` & `gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_eq_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_flow_vol.py` & `gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_flow_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/backtest/test_backtest_predefined.py` & `gs_quant-1.0.0/gs_quant/test/backtest/test_backtest_predefined.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/backtest/test_generic_engine.py` & `gs_quant-1.0.0/gs_quant/test/backtest/test_generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/backtest/test_triggers.py` & `gs_quant-1.0.0/gs_quant/test/backtest/test_triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/data/test_data_coordinate.py` & `gs_quant-1.0.0/gs_quant/test/data/test_data_coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/data/test_dataset.py` & `gs_quant-1.0.0/gs_quant/test/data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/datetime_/test_date.py` & `gs_quant-1.0.0/gs_quant/test/datetime_/test_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/datetime_/test_gscalendar.py` & `gs_quant-1.0.0/gs_quant/test/datetime_/test_gscalendar.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 
 from unittest import mock
 import pandas as pd
 import datetime
 
 
 # Test GsCalendar initiated with single PricingLocation
+@mock.patch.object(Dataset, 'get_coverage', return_value=pd.DataFrame())
 @mock.patch.object(Dataset, 'get_data')
-def test_gs_calendar_single(mocker):
+def test_gs_calendar_single(mocker, mocker_cov):
     set_session()
     mocker.return_value = pd.DataFrame(index=[datetime.datetime(1999, 9, 12)],
                                        data={'holiday': 'Labor Day'})
     nyc = PricingLocation.NYC
     GsCalendar.reset()
     days = GsCalendar(nyc).holidays
     assert days
 
 
 # Test GsCalendar initiated with tuple
 @mock.patch.object(Dataset, 'get_data')
-def test_gs_calendar_tuple(mocker):
+@mock.patch.object(Dataset, 'get_coverage', return_value=pd.DataFrame())
+def test_gs_calendar_tuple(mocker_coverage, mocker):
     set_session()
     mocker.return_value = pd.DataFrame(index=[datetime.datetime(1999, 9, 12)],
                                        data={'holiday': 'Labor Day'})
     locs = (PricingLocation.NYC, PricingLocation.LDN)
     days = GsCalendar(locs).holidays
     assert days
```

### Comparing `gs_quant-0.9.99/gs_quant/test/datetime_/test_point.py` & `gs_quant-1.0.0/gs_quant/test/datetime_/test_point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/datetime_/test_relative_date.py` & `gs_quant-1.0.0/gs_quant/test/datetime_/test_relative_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 specific language governing permissions and limitations
 under the License.
 """
 
 from datetime import date as dt
 from unittest.mock import Mock
 
+import pandas as pd
 import pytest
-from gs_quant.datetime.relative_date import RelativeDate
 from testfixtures import Replacer
 
+from gs_quant.datetime.relative_date import RelativeDate
+
 holiday_calendar = [dt(2021, 1, 18)]
 
 
 def test_rule_parsing():
     assert RelativeDate('A')._get_rules() == ['A']
     assert RelativeDate('1d')._get_rules() == ['1d']
     assert RelativeDate('-1d')._get_rules() == ['-1d']
@@ -240,14 +242,16 @@
     'updateTime': 'date'}
 
 
 # test holiday calendar logic
 def test_currency_holiday_calendars(mocker):
     replace = Replacer()
     replace('gs_quant.api.gs.data.GsDataApi.query_data', Mock(side_effect=mock_holiday_data))
+    mocker.patch("gs_quant.api.gs.data.GsDataApi.get_coverage",
+                 return_value=pd.DataFrame([['USD'], ['GBP']], columns=['currency']))
     mocker.patch("gs_quant.api.gs.data.GsDataApi.get_types", return_value=test_types)
     rdate = RelativeDate('-1b', base_date=dt(2022, 4, 12))
     assert dt(2022, 4, 11) == rdate.apply_rule(currencies=[])
     assert dt(2022, 4, 11) == rdate.apply_rule(currencies=['GBP'])
     assert dt(2022, 4, 8) == rdate.apply_rule(currencies=['USD'])
     assert dt(2022, 4, 11) == rdate.apply_rule()  # No longer using USD by default
     replace.restore()
```

### Comparing `gs_quant-0.9.99/gs_quant/test/datetime_/test_time.py` & `gs_quant-1.0.0/gs_quant/test/datetime_/test_time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/fixtures/content.py` & `gs_quant-1.0.0/gs_quant/test/fixtures/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_baskets.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_baskets.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     new_admin = User.get(user_id='user_xyz')
     basket.entitlements.admin.users += [new_admin]
 
     entitlements_response = TargetEntitlements(admin=['guid:user_abc', 'guid:user_xyz'])
     mock_response(mocker, GsAssetApi, 'update_asset_entitlements', entitlements_response)
     response = basket.update()
     GsAssetApi.update_asset_entitlements.assert_called()
-    assert response == entitlements_response.as_dict()
+    assert response == entitlements_response
 
 
 def test_upload_position_history(mocker):
     mock_session()
 
     # test errors
     mock_basket_init(mocker, user_ea, False)
```

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_hedger.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_hedger.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_instrument.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_portfolio.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_portfolio_manager.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_pricing_context.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_pricing_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,20 +129,21 @@
 
     PricingContext.pop()
     assert len(PricingContext.path) == 0
 
 
 def test_creation():
     c1 = PricingContext(pricing_date=datetime.date(2022, 6, 15))
-    # All props except for the initialised one are None. Context is not useable as-is
-    assert c1.market is None
-    assert c1.market_data_location is None
-    assert c1.is_batch is None
-    assert c1.use_cache is None
-    assert c1._max_concurrent is None
+
+    # All props except for the initialised one are defaulted. Context is not useable as-is
+    assert c1.market == CloseMarket(c1.pricing_date, 'LDN')
+    assert c1.market_data_location == PricingLocation.LDN
+    assert c1.is_batch is False
+    assert c1.use_cache is False
+    assert c1._max_concurrent == 1000
 
     assert c1.pricing_date == datetime.date(2022, 6, 15)
 
 
 def test_inheritance():
     c1 = PricingContext(pricing_date=datetime.date(2022, 6, 16), market_data_location='NYC')
     c2 = PricingContext(pricing_date=datetime.date(2022, 7, 1))
@@ -165,54 +166,77 @@
                 assert c3.pricing_date == c2.pricing_date
                 # all other props have default values
                 assert c3.is_batch is False
                 assert c3.use_cache is False
                 assert c3._max_concurrent == 1000
 
 
+def test_max_concurrent():
+    a = PricingContext()
+    assert a._max_concurrent == 1000  # Default value
+
+    b = PricingContext()
+    b._max_concurrent = 2000
+
+    c = PricingContext()
+    c._max_concurrent = 3000
+
+    assert b._max_concurrent == 2000  # setter working?
+    with b:
+        assert a._max_concurrent == 2000  # a was unset so defaults to inheriting b's value
+        assert c._max_concurrent == 3000  # c was explicitly set so keep's it's value
+        with a:
+            assert PricingContext.current._max_concurrent == 2000  # should be same as above property accessor
+        with c:
+            assert PricingContext.current._max_concurrent == 3000  # should be same as above property accessor
+
+
 def test_current_inheritance():
     cur = PricingContext.current
-    assert cur.market_data_location is None
+    assert cur.market_data_location == PricingLocation.LDN
 
     with PricingContext() as pc:
         assert pc.market_data_location == PricingLocation.LDN
 
     PricingContext.current = PricingContext(market_data_location='TKO')
 
     # We can set props on the current so that props are inherited globally
     new_cur = PricingContext.current
     assert new_cur.market_data_location == PricingLocation.TKO
 
-    with PricingContext() as pc:
-        assert pc.market_data_location == new_cur.market_data_location
+    assert PricingContext().market_data_location == new_cur.market_data_location
 
     with PricingContext():
         with PricingContext() as pc2:
             assert pc2.market_data_location == new_cur.market_data_location
 
     # Exit the current
     PricingContext.pop()
 
 
 def test_cleanup():
     c1 = PricingContext(pricing_date=datetime.date(2022, 4, 6))
     c2 = PricingContext(request_priority=5000)
+    default_date = c2.pricing_date
 
     with c1:
         with c2:
             assert c2.request_priority == 5000
             # pricing_date is inherited from c1
             assert c2.pricing_date is not None
             assert c2.pricing_date == c1.pricing_date
-        # pricing date is cleaned up on exit from c2. request priority remains set
-        assert c2.request_priority == 5000
-        assert c2.pricing_date is None
+        # on exit from c2, the pricing date would still show what it would be as inside c1 still
+        assert c2.pricing_date == c1.pricing_date
+    # pricing date is cleaned up on exit from c1. request priority remains set
+    assert c2.request_priority == 5000
+    assert c2.pricing_date == default_date
 
 
 def test_market_props():
+    PricingContext.current = PricingContext()  # Reset
     # market_data_location cannot conflict with market.location
     with pytest.raises(ValueError):
         PricingContext(market=CloseMarket(date=datetime.date(2022, 4, 6), location='NYC'),
                        pricing_date=datetime.date(2022, 7, 4), market_data_location='TKO')
 
     # Default pricing date and market location are today and LDN, respectively
     pc = PricingContext()
@@ -226,19 +250,17 @@
 
     with pc:
         assert pc.pricing_date == datetime.date(2022, 7, 4)
         assert pc.market.date == datetime.date(2022, 4, 6)
 
     # if market is not specified, it is inferred from pricing_date and market_data_location
     pc = PricingContext(pricing_date=datetime.date(2022, 7, 4), market_data_location='TKO')
-    assert pc.market is None
-    with pc:
-        cm = CloseMarket(date=pc.pricing_date, location=pc.market_data_location)
-        assert pc.market.date == cm.date
-        assert pc.market.location == cm.location
+    cm = CloseMarket(date=pc.pricing_date, location=pc.market_data_location)
+    assert pc.market.date == cm.date
+    assert pc.market.location == cm.location
 
     # market is not inherited
     pc = PricingContext(market=CloseMarket(date=datetime.date(2022, 4, 6), location='NYC'))
     with pc:
         # pc gets market_data_location from its market
         assert pc.market_data_location == PricingLocation.NYC
         with PricingContext() as inner:
@@ -260,15 +282,15 @@
     port = Portfolio([swap1, swap2])
     with MockCalc(mocker):
         cm = CloseMarket(date=datetime.date(2022, 7, 5), location='TKO')
         pc = PricingContext(market_data_location='TKO', pricing_date=datetime.date(2022, 4, 6), market=cm)
         assert pc.market_data_location == PricingLocation.TKO
         assert pc.pricing_date == datetime.date(2022, 4, 6)
         assert pc.market == cm
-        assert pc.is_batch is None
+        assert pc.is_batch is False
 
         with pc:
             assert pc.is_batch is False
             swap1.resolve()
             swap1.dollar_price()
             swap2.calc(risk.IRDelta)
             port.resolve()
@@ -278,15 +300,15 @@
             assert pc.pricing_date == datetime.date(2022, 4, 6)
             assert pc.market == cm
             assert pc.is_batch is False
 
         assert pc.market_data_location == PricingLocation.TKO
         assert pc.pricing_date == datetime.date(2022, 4, 6)
         assert pc.market == cm
-        assert pc.is_batch is None
+        assert pc.is_batch is False
 
 
 def test_different_nested_locations(mocker):
     s = IRSwap(name='location_test_swap')
     with MockCalc(mocker):
         with PricingContext(market_data_location='TKO', pricing_date=datetime.date(2022, 7, 5)):
             with PricingContext(market_data_location='NYC', pricing_date=datetime.date(2022, 7, 11)):
@@ -304,20 +326,19 @@
 def test_async_behaviour(queue_mock, run_mock):
     s = IRSwap()
     # we do not actually run requests from the RiskApi
     run_mock.return_value = None
     # queue to drain should hence be empty
     queue_mock.return_value = True, []
 
-    with PricingContext(is_async=True) as pc:
+    with PricingContext(is_async=True):
         s.price()
     # sleep to give spawned threads time to call RiskApi.run
     sleep(1)
     # threads should see the _max_concurrent property of the PricingContext as 1000 even though it's exited
-    assert pc._max_concurrent is None
     run_mock.assert_called_with(ANY, ANY, 1000, ANY, timeout=ANY, span=ANY)
 
 
 def test_use_context_for_inheritance():
     cur = PricingContext.current
     assert cur.active_context == cur
```

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_report.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_report.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/markets/test_securities.py` & `gs_quant-1.0.0/gs_quant/test/markets/test_securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/models/__init__.py` & `gs_quant-1.0.0/gs_quant/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/models/test_epidemiology.py` & `gs_quant-1.0.0/gs_quant/test/models/test_epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/models/test_risk_model.py` & `gs_quant-1.0.0/gs_quant/test/models/test_risk_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 under the License.
 """
 import pytest
 from unittest import mock
 
 from gs_quant.models.risk_model import FactorRiskModel, MacroRiskModel, ReturnFormat, Unit
 from gs_quant.session import *
-from gs_quant.target.risk_models import RiskModel as Risk_Model, RiskModelCoverage, RiskModelTerm,\
+from gs_quant.target.risk_models import RiskModel as Risk_Model, RiskModelCoverage, RiskModelTerm, \
     RiskModelUniverseIdentifier, RiskModelType, RiskModelDataAssetsRequest as DataAssetsRequest, \
     RiskModelDataMeasure as Measure, RiskModelUniverseIdentifierRequest as UniverseIdentifier
 import datetime as dt
 
-
 empty_entitlements = {
     "execute": [],
     "edit": [],
     "view": [],
     "admin": [],
     "query": [],
     "upload": []
@@ -673,9 +672,129 @@
                                          format=ReturnFormat.JSON)
 
     GsSession.current._post.assert_called_with('/risk/models/data/{id}/query'.format(id='model_id'),
                                                query, timeout=200)
     assert response == specific_return_response
 
 
+def test_upload_risk_model_data(mocker):
+    model = mock_risk_model(mocker)
+    risk_model_data = {
+        'date': '2023-04-14',
+        'assetData': {
+            'universe': ['2407966', '2046251', 'USD'],
+            'specificRisk': [12.09, 45.12, 3.09],
+            'factorExposure': [
+                {'1': 0.23, '2': 0.023},
+                {'1': 0.23},
+                {'3': 0.23, '2': 0.023}
+            ],
+            'totalRisk': [0.12, 0.45, 1.2]
+        },
+        'factorData': [
+            {
+                'factorId': '1',
+                'factorName': 'USD',
+                'factorCategory': 'Currency',
+                'factorCategoryId': 'CUR'
+            },
+            {
+                'factorId': '2',
+                'factorName': 'ST',
+                'factorCategory': 'ST',
+                'factorCategoryId': 'ST'
+            },
+            {
+                'factorId': '3',
+                'factorName': 'IND',
+                'factorCategory': 'IND',
+                'factorCategoryId': 'IND'
+            }
+        ],
+        'covarianceMatrix': [[0.089, 0.0123, 0.345],
+                             [0.0123, 3.45, 0.345],
+                             [0.345, 0.345, 1.23]],
+        'issuerSpecificCovariance': {
+            'universeId1': ['2407966'],
+            'universeId2': ['2046251'],
+            'covariance': [0.03754]
+        },
+        'factorPortfolios': {
+            'universe': ['2407966', '2046251'],
+            'portfolio': [{'factorId': 1, 'weights': [0.25, 0.75]},
+                          {'factorId': 2, 'weights': [0.25, 0.75]},
+                          {'factorId': 3, 'weights': [0.25, 0.75]}]
+        }
+    }
+
+    base_url = f"/risk/models/data/{model.id}?partialUpload=true"
+    date = risk_model_data.get("date")
+    max_asset_batch_size = 2
+
+    batched_asset_data = [
+        {"assetData": {key: value[i:i + max_asset_batch_size] for key, value in
+                       risk_model_data.get("assetData").items()}, "date": date,
+         } for i in range(0, len(risk_model_data.get("assetData").get("universe")), max_asset_batch_size)
+    ]
+
+    max_asset_batch_size //= 2
+    batched_factor_portfolios = [
+        {"factorPortfolios":
+            {key: (value[i:i + max_asset_batch_size] if key in "universe" else
+                   [{"factorId": factor_weights.get("factorId"),
+                     "weights": factor_weights.get("weights")[i:i + max_asset_batch_size]} for factor_weights in value])
+             for key, value in risk_model_data.get("factorPortfolios").items()},
+         "date": date
+         } for i in range(0, len(risk_model_data.get("factorPortfolios").get("universe")), max_asset_batch_size)
+    ]
+
+    expected_factor_data_calls = [
+        mock.call(base_url, {"date": date, "factorData": risk_model_data.get("factorData"),
+                             "covarianceMatrix": risk_model_data.get("covarianceMatrix")}, timeout=200)
+    ]
+
+    expected_asset_data_calls = []
+    for batch_num, batch_asset_payload in enumerate(batched_asset_data):
+        final_upload_flag = 'true' if batch_num == len(batched_asset_data) - 1 else 'false'
+        expected_asset_data_calls.append(
+            mock.call(f"{base_url}&finalUpload={final_upload_flag}", batch_asset_payload, timeout=200)
+        )
+
+    expected_factor_portfolios_data_calls = []
+    for batch_num, batched_fp_payload in enumerate(batched_factor_portfolios):
+        final_upload_flag = 'true' if batch_num == len(batched_factor_portfolios) - 1 else 'false'
+        expected_factor_portfolios_data_calls.append(
+            mock.call(f"{base_url}&finalUpload={final_upload_flag}", batched_fp_payload, timeout=200)
+        )
+
+    expected_isc_data_calls = [
+        mock.call(f"{base_url}&finalUpload=true",
+                  {"issuerSpecificCovariance": risk_model_data.get("issuerSpecificCovariance"), "date": date},
+                  timeout=200)
+    ]
+
+    expected_calls = expected_factor_data_calls + expected_asset_data_calls + \
+        expected_isc_data_calls + expected_factor_portfolios_data_calls
+
+    # mock GsSession
+    mocker.patch.object(
+        GsSession.__class__,
+        'default_value',
+        return_value=GsSession.get(
+            Environment.QA,
+            'client_id',
+            'secret'))
+    mocker.patch.object(GsSession.current, '_post', return_value='Upload Successful')
+
+    max_asset_batch_size = 2
+    model.upload_data(risk_model_data, max_asset_batch_size=max_asset_batch_size)
+
+    call_args_list = GsSession.current._post.call_args_list
+
+    assert len(call_args_list) == len(expected_calls)
+    assert call_args_list == expected_calls
+
+    GsSession.current._post.assert_has_calls(expected_calls, any_order=False)
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

### Comparing `gs_quant-0.9.99/gs_quant/test/test_base.py` & `gs_quant-1.0.0/gs_quant/test/test_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/test_commod.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/test_commod.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/multi_measure/test_measure_registry.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/multi_measure/test_measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_algebra.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_analysis.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_backtesting.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_backtesting.py`

 * *Files 17% similar despite different names*

```diff
@@ -66,31 +66,61 @@
     ]
     mreb = pd.Series(
         [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792,
          100.0, 101, 103.02, 100.9596, 100.9596, 102.978792],
         index=dates)
     assert_series_equal(mreb, basket_series([mreb], [1], rebal_freq=RebalFreq.MONTHLY))
 
+    dates = [
+        datetime.datetime(2019, 1, 1),
+        datetime.datetime(2019, 1, 2),
+        datetime.datetime(2019, 1, 3),
+        datetime.datetime(2019, 1, 4),
+        datetime.datetime(2019, 1, 5),
+        datetime.datetime(2019, 1, 8),
+        datetime.datetime(2019, 1, 9),
+        datetime.datetime(2019, 1, 10),
+        datetime.datetime(2019, 1, 11),
+        datetime.datetime(2019, 1, 12),
+        datetime.datetime(2019, 1, 13)
+    ]
+    wreb = pd.Series(
+        [100.0, 105, 110, 115, 120, 125,
+         130, 135, 140, 145, 150],
+        index=dates)
+
+    wreb_2 = pd.Series(
+        [100.0, 105, 110, 115, 120, 125,
+         130, 135, 140, 145, 150],
+        index=dates)
+
+    ret_wreb = pd.Series(
+        [100.0, 110.0, 120.0, 130.0, 140.0, 150.0,
+         162.0, 174.0, 186.0, 198.0, 210.0],
+        index=dates)
+
+    assert_series_equal(ret_wreb, basket_series([wreb, wreb_2], [1, 1], rebal_freq=RebalFreq.WEEKLY))
+
 
 def _mock_spot_data():
     dates = pd.date_range(start='2021-01-01', periods=6)
     x = pd.DataFrame({'spot': [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'spot': [100.0, 100, 100, 100, 100, 100]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    return x.append(y)
+    return pd.concat([x, y])
 
 
 def _mock_spot_data_feb():
     dates_feb = pd.date_range(start='2021-02-01', periods=6)
     x = pd.DataFrame({'spot': [100.0, 101.5, 106.02, 100.1, 105.3, 102.9]}, index=dates_feb)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'spot': [100.0, 101.5, 100.02, 98.1, 95.3, 93.9]}, index=dates_feb)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    return x.append(y)
+    return pd.concat([x, y])
 
 
 def test_basket_price():
     with pytest.raises(MqValueError):
         Basket(['AAPL UW'], [0.1, 0.9], RebalFreq.MONTHLY)
 
     dates = pd.DatetimeIndex([date(2021, 1, 1), date(2021, 1, 2), date(2021, 1, 3), date(2021, 1, 4), date(2021, 1, 5),
@@ -135,15 +165,15 @@
     dates = pd.DatetimeIndex([date(2021, 1, 1), date(2021, 1, 2), date(2021, 1, 3), date(2021, 1, 4), date(2021, 1, 5),
                               date(2021, 1, 6)])
 
     x = pd.DataFrame({'impliedVolatility': [30.0, 30.2, 29.8, 30.6, 30.1, 30.0]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'impliedVolatility': [20.0, 20.2, 20.3, 20.6, 21.1, 20.0]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    implied_vol = x.append(y)
+    implied_vol = pd.concat([x, y])
     implied_vol.index.name = 'date'
 
     mock_spot = replace('gs_quant.timeseries.backtesting.ts.get_historical_and_last_for_measure', Mock())
     mock_spot.side_effect = [implied_vol.rename(columns={'impliedVolatility': 'spot'})]
 
     mock_data = replace('gs_quant.api.utils.ThreadPoolManager.run_async', Mock())
     mock_data.return_value = [implied_vol]
@@ -221,32 +251,32 @@
     a = pd.Series([1 for i in range(5)], index=pd.date_range('2021-09-01', '2021-09-05'))
     x = pd.DataFrame({'spot': a.tolist()}, index=a.index)
     x['assetId'] = 'XLC_MOCK_MQID'
     y = pd.DataFrame({'spot': a.tolist()}, index=a.index)
     y['assetId'] = 'XLB_MOCK_MQID'
     z = pd.DataFrame({'spot': (a ** 3).tolist()}, index=a.index)
     z['assetId'] = 'SPX_MOCK_MQID'
-    return x.append(y).append(z)
+    return pd.concat([x, y, z])
 
 
 def _mock_spot_data_identical():
     dates = pd.date_range(start='2021-01-01', periods=6)
     x = pd.DataFrame({'spot': [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'spot': [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    return x.append(y)
+    return pd.concat([x, y])
 
 
 def _mock_spot_data_corr():
     dates = pd.date_range(start='2021-01-01', periods=6)
     x = pd.DataFrame({'spot': [78, 9, 1003, 17, -12, 5], 'assetId': 'MA4B66MW5E27U9VBB94'}, index=dates)
     y = pd.DataFrame({'spot': [-33, 33, 15, 21, -3, 2], 'assetId': 'MA4B66MW5E27UAL9SUX'}, index=dates)
     z = pd.DataFrame({'spot': [86, 86, 56, 86, 86, 9], 'assetId': 'MA4B66MW5E27UANZH2M'}, index=dates)
-    return x.append(y).append(z)
+    return pd.concat([x, y, z])
 
 
 def test_basket_average_realized_vol_wts():
     replace = Replacer()
 
     mock_data = replace('gs_quant.timeseries.backtesting.ts.get_historical_and_last_for_measure', Mock())
     mock_data.side_effect = [_mock_data_simple()]
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_datetime.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 """
+from unittest import mock
 
 import pytest
 from pandas.testing import assert_series_equal
 
+from gs_quant.test.api.test_risk import set_session
 from gs_quant.timeseries.datetime import *
 
 
 def test_basic():
     assert type(RelativeDate('0d').apply_rule()) == dt.date
 
 
@@ -405,15 +407,15 @@
     assert_series_equal(actual, expected, obj='append two series')
 
     x = pd.Series([3.1, 4.1, 5.1], index=pd.date_range('2019-01-01 02:00', periods=3, freq='H'))
     y = pd.Series([1.0, 2.0, 3.0, 4.0, 5.0, 7.0], index=pd.date_range('2019-01-01', periods=6, freq='H'))
 
     actual = append([x, y])
     expected = pd.Series([3.1, 4.1, 5.1, 7.0], index=pd.date_range('2019-01-01 02:00', periods=4, freq='H'))
-    assert_series_equal(actual, expected, obj='prepend two real-time series')
+    assert_series_equal(actual, expected, obj='append two real-time series')
 
 
 def test_prepend():
     x = pd.Series([1.0, 2.0, 3.0, 4.0, 5.0, 7.0], index=pd.date_range('2019-01-01', "2019-01-06"))
     y = pd.Series([3.1, 4.1, 5.1], index=pd.date_range('2019-01-03', '2019-01-05'))
 
     assert_series_equal(prepend([]), pd.Series(dtype='float64'), obj='prepend empty')
@@ -470,9 +472,29 @@
     assert day_count(dt.date(2021, 5, 10), dt.date(2021, 5, 14)) == 4
     assert day_count(dt.date(2021, 5, 10), dt.date(2021, 5, 17)) == 5
 
     with pytest.raises(MqValueError):
         day_count(dt.date(2021, 5, 7), '2021-05-10')
 
 
+@mock.patch.object(Dataset, 'get_data')
+def test_align_calendar(mocker):
+    dates = pd.date_range(start='1/1/2023', end='1/31/2023')
+    series = pd.Series(range(len(dates)), index=dates)
+
+    set_session()
+    mocker.return_value = pd.DataFrame(index=[dt.datetime(2023, 1, 3)],
+                                       data={'holiday': 'New Year'})
+
+    GsCalendar.reset()
+
+    aligned_series = align_calendar(series, 'NYC')
+    # Check if the holiday was removed
+    assert dt.datetime(2023, 1, 3) not in aligned_series
+    # Check the first saturday was removed
+    assert dt.datetime(2023, 1, 7) not in aligned_series
+    # Check full series length is correct
+    assert aligned_series.size == 21
+
+
 if __name__ == "__main__":
     pytest.main(args=["test_datetime.py"])
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_econometrics.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_econometrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 """
 from unittest.mock import Mock
 
 import pytest
-from pandas.testing import assert_series_equal
-from testfixtures import Replacer
 from gs_quant.timeseries import *
 from gs_quant.timeseries.econometrics import _get_ratio
+from pandas.testing import assert_series_equal
+from testfixtures import Replacer
 
 
 def test_returns():
     dates = [
         date(2019, 1, 1),
         date(2019, 1, 2),
         date(2019, 1, 3),
@@ -351,15 +351,15 @@
     assert_series_equal(result, expected)
 
     result = correlation(x, y, "2d")
     expected = pd.Series([-1, 1, np.nan, -1], index=daily_dates[2:])
     assert_series_equal(result, expected, obj="Correlation strdate as window")
 
     result = correlation(x, y, "3m")
-    expected = pd.Series(dtype=float)
+    expected = pd.Series(dtype=float, index=[])
     assert_series_equal(result, expected, obj="Correlation strdate as window with too large of window")
 
 
 def test_beta():
     x = pd.Series(dtype=float)
     assert_series_equal(pd.Series(dtype=float), beta(x, x))
     assert_series_equal(pd.Series(dtype=float), beta(x, x, 1))
@@ -428,14 +428,16 @@
     expected = pd.Series([0.0, 0.0, 0.0, -0.2, -0.2, -0.8], index=daily_dates)
     assert_series_equal(result, expected, obj="Max drawdown")
 
     result = max_drawdown(series, Window(2, 0))
     expected = pd.Series([0.0, 0.0, 0.0, -0.2, -0.2, -0.75], index=daily_dates)
     assert_series_equal(result, expected, obj="Max drawdown window 2")
 
+    with pytest.raises(TypeError):
+        max_drawdown(pd.Series([1, 5, 5, 4, 4, 1]), Window('2d', 0))
     result = max_drawdown(series, Window('2d', 0))
     expected = pd.Series([0.0, 0.0, 0.0, -0.2, 0.0, -0.75], index=daily_dates)
     assert_series_equal(result, expected, obj="Max drawdown window 2d")
 
 
 def test_excess_returns():
     replace = Replacer()
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_helper.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import datetime
 import datetime as dt
 import json
 import os
 from typing import Union, Dict
 from unittest import mock
+from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
 import pytest
 import pytz
 from numpy.testing import assert_equal
 from pandas.testing import assert_series_equal
@@ -1535,21 +1536,21 @@
                               dt.date(2021, 1, 5), dt.date(2021, 1, 6)])
     x = pd.DataFrame({'impliedVolatility': [0.1, 0.11, 0.12, 0.13, 0.14, 0.15]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'impliedVolatility': [0.2, 0.21, 0.22, 0.23, 0.24, 0.25]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
     z = pd.DataFrame({'impliedVolatility': [0.13, 0.21, 0.3, 0.31, 0.23, 0.24]}, index=dates)
     z['assetId'] = 'MA4B66MW5E27U8P32SB'
-    implied_vol = x.append(y).append(z)
+    implied_vol = pd.concat([x, y, z])
 
     x = pd.DataFrame({'spot': [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'spot': [100.0, 100, 100, 100, 100, 100]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    spot_data = x.append(y)
+    spot_data = pd.concat([x, y])
 
     mock_data = replace('gs_quant.timeseries.measures.GsDataApi.get_market_data', Mock())
     mock_data.side_effect = [implied_vol, spot_data]
 
     mock_asset = replace('gs_quant.timeseries.backtesting.GsAssetApi.get_many_assets_data', Mock())
     mock_asset.return_value = [{'id': 'MA4B66MW5E27U9VBB94', 'bbid': 'AAPL UW'},
                                {'id': 'MA4B66MW5E27UAL9SUX', 'bbid': 'MSFT UW'}]
@@ -1574,15 +1575,15 @@
 
     dates = pd.DatetimeIndex([dt.date(2021, 1, 1), dt.date(2021, 1, 2), dt.date(2021, 1, 3), dt.date(2021, 1, 4),
                               dt.date(2021, 1, 5), dt.date(2021, 1, 6)])
     x = pd.DataFrame({'spot': [100.0, 101, 103.02, 100.9596, 100.9596, 102.978792]}, index=dates)
     x['assetId'] = 'MA4B66MW5E27U9VBB94'
     y = pd.DataFrame({'spot': [100.0, 99.5, 100.1, 101, 100.7, 100.6]}, index=dates)
     y['assetId'] = 'MA4B66MW5E27UAL9SUX'
-    constituents_spot = x.append(y)
+    constituents_spot = pd.concat([x, y])
 
     index_spot = pd.DataFrame({'spot': [100.0, 101, 102, 103, 103.3, 104]}, index=dates)
     index_spot['assetId'] = 'MA4B66MW5E27U8P32SB'
 
     mock_data = replace('gs_quant.timeseries.measures.GsDataApi.get_market_data', Mock())
     mock_data.side_effect = [index_spot, constituents_spot]
 
@@ -1593,15 +1594,15 @@
     mock_data.return_value = constituents_spot
 
     spx = Index('MA4B66MW5E27U8P32SB', AssetClass.Equity, 'SPX')
     a_basket = tm.Basket(['AAPL UW', 'MSFT UW'], [0.1, 0.9])
     actual = tm.realized_correlation_with_basket(spx, '2d', a_basket)
     expected = pd.Series([np.nan, np.nan, -501.344109, -108.318770, -168.132382, 109.044958], index=dates)
     expected = ExtendedSeries(expected)
-    assert_series_equal(actual, expected)
+    assert_series_equal(actual, expected, check_dtype=False)
 
     with pytest.raises(NotImplementedError):
         tm.realized_correlation_with_basket(spx, '2d', a_basket, real_time=True)
 
     replace.restore()
 
 
@@ -2282,14 +2283,20 @@
         actual = tm_rates.swap_term_structure(**args)
     actual.dataset_ids = _test_datasets
     expected = tm.ExtendedSeries([1, 2, 3, 4], index=pd.to_datetime(['2020-01-01', '2021-01-01', '2021-12-31',
                                                                      '2022-12-30']))
     expected.dataset_ids = _test_datasets
     assert_series_equal(expected, actual, check_names=False)
     assert actual.dataset_ids == expected.dataset_ids
+
+    with patch('gs_quant.datetime.GsCalendar.holidays', (dt.date(2023, 1, 1),)):
+        args['pricing_date'] = dt.date(2023, 1, 1)
+        with pytest.raises(MqValueError):
+            tm_rates.swap_term_structure(**args)
+
     replace.restore()
 
 
 def test_basis_swap_term_structure():
     replace = Replacer()
     range_mock = replace('gs_quant.timeseries.measures_rates._range_from_pricing_date', Mock())
     range_mock.return_value = [datetime.date(2019, 1, 1), datetime.date(2019, 1, 1)]
@@ -2413,14 +2420,20 @@
     with DataContext('2019-01-01', '2025-01-01'):
         actual = tm_rates.basis_swap_term_structure(**args)
     actual.dataset_ids = _test_datasets
     expected = tm.ExtendedSeries([1], index=pd.to_datetime(['2020-01-01']))
     expected.dataset_ids = _test_datasets
     assert_series_equal(expected, actual, check_names=False)
     assert actual.dataset_ids == expected.dataset_ids
+
+    with patch('gs_quant.datetime.GsCalendar.holidays', (dt.date(2023, 1, 1),)):
+        args['pricing_date'] = dt.date(2023, 1, 1)
+        with pytest.raises(MqValueError):
+            tm_rates.basis_swap_term_structure(**args)
+
     replace.restore()
 
 
 def test_cap_floor_vol():
     replace = Replacer()
     mock_usd = Currency('MA890', 'USD')
     xrefs = replace('gs_quant.timeseries.measures.GsAssetApi.get_asset_xrefs', Mock())
@@ -3591,15 +3604,15 @@
     assert actual.dataset_ids == _test_datasets
 
     actual = tm.carry_term(Index('MA123', AssetClass.FX, '123'))
     idx = pd.DatetimeIndex(['2018-01-08', '2018-01-15', '2019-01-01', '2020-01-01'], name='expirationDate')
     expected = pd.Series([0.001667, 0.004714, 0.036105, 0.05621], name='carry', index=idx)
     expected = expected.loc[DataContext.current.start_date: DataContext.current.end_date]
 
-    assert_series_equal(expected, pd.Series(actual), check_exact=False, check_less_precise=3)
+    assert_series_equal(expected, pd.Series(actual), check_exact=False, atol=0.00001)
     assert actual.dataset_ids == _test_datasets
 
     with pytest.raises(NotImplementedError):
         tm.carry_term(Index('MA123', AssetClass.FX, '123'), real_time=True)
 
     thread_mock.return_value = [pd.DataFrame(), pd.DataFrame()]
     actual = tm.carry_term(Index('MA123', AssetClass.FX, '123'))
@@ -3881,15 +3894,15 @@
 
         actual = tm.forward_price(mock_spp,
                                   price_method='LMP',
                                   contract_range='2Q20',
                                   bucket='7x24'
                                   )
 
-        assert_series_equal(pd.Series(dtype=float), pd.Series(actual), check_names=False)
+        assert_series_equal(pd.Series(dtype=float, index=[]), pd.Series(actual), check_names=False)
 
         actual = tm.forward_price(mock_spp,
                                   price_method='LMP',
                                   contract_range='2Q20',
                                   bucket='PEAK'
                                   )
         assert_series_equal(pd.Series(target['peak'],
@@ -4089,15 +4102,15 @@
 
         actual = tm.implied_volatility_elec(mock_spp,
                                             price_method='LMP',
                                             contract_range='2Q20',
                                             bucket='7x24'
                                             )
 
-        assert_series_equal(pd.Series(dtype=float), pd.Series(actual), check_names=False)
+        assert_series_equal(pd.Series(dtype=float, index=[]), pd.Series(actual), check_names=False)
 
         actual = tm.implied_volatility_elec(mock_spp,
                                             price_method='LMP',
                                             contract_range='2Q20',
                                             bucket='PEAK'
                                             )
         assert_series_equal(pd.Series(target['peak'],
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_countries.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_fx_vol.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_fx_vol.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,21 @@
 
 _index = [pd.Timestamp('2021-03-30')]
 _test_datasets = ('TEST_DATASET',)
 
 
 def test_currencypair_to_tdapi_fxfwd_asset():
     mock_eur = Cross('MA8RY265Q34P7TWZ', 'EURUSD')
+    replace = Replacer()
+    xrefs = replace('gs_quant.timeseries.measures_fx_vol._get_tdapi_fxo_assets', Mock())
+    xrefs.return_value = 'MA8RY265Q34P7TWZ'
+    bbid_mock = replace('gs_quant.timeseries.measures_fx_vol.Asset.get_identifier', Mock())
+    bbid_mock.return_value = {'EURUSD'}
     assert _currencypair_to_tdapi_fxfwd_asset(mock_eur) == "MA8RY265Q34P7TWZ"
+    replace.restore()
 
 
 def test_currencypair_to_tdapi_fxo_asset(mocker):
     replace = Replacer()
     mocker.patch.object(GsSession.__class__, 'current',
                         return_value=GsSession.get(Environment.QA, 'client_id', 'secret'))
     mocker.patch.object(GsSession.current, '_get', side_effect=mock_request)
@@ -149,15 +155,17 @@
 def test_get_tdapi_fxo_assets():
     mock_asset_1 = GsAsset(asset_class='FX', id='MAW8SAXPSKYA94E2', type_='Option', name='Test_asset')
     mock_asset_2 = GsAsset(asset_class='FX', id='MATDD783JM1C2GGD', type_='Option', name='Test_asset')
 
     replace = Replacer()
     assets = replace('gs_quant.timeseries.measures.GsAssetApi.get_many_assets', Mock())
     assets.return_value = [mock_asset_1]
-    assert 'MAW8SAXPSKYA94E2' == tm_fxo._get_tdapi_fxo_assets()
+    kwargs = dict(asset_parameters_expiration_date='5y', asset_parameters_call_currency='USD',
+                  asset_parameters_put_currency='EUR')
+    assert 'MAW8SAXPSKYA94E2' == tm_fxo._get_tdapi_fxo_assets(**kwargs)
     replace.restore()
 
     assets = replace('gs_quant.timeseries.measures.GsAssetApi.get_many_assets', Mock())
     assets.return_value = [mock_asset_1, mock_asset_2]
     kwargs = dict(asset_parameters_expiration_date='5y', asset_parameters_call_currency='USD',
                   asset_parameters_put_currency='EUR')
     with pytest.raises(MqValueError):
@@ -195,15 +203,16 @@
     assert 'MAW8SAXPSKYA94E2' == tm_fxo._get_tdapi_fxo_assets(**kwargs)
     replace.restore()
 
 
 def mock_curr(_cls, _q):
     d = {
         'impliedVolatility': [1, 2, 3],
-        'fwdPoints': [4, 5, 6]
+        'fwdPoints': [4, 5, 6],
+        'forwardPoint': [7, 8, 9]
     }
     df = MarketDataResponseFrame(data=d, index=_index * 3)
     df.dataset_ids = _test_datasets
     return df
 
 
 def test_fx_vol_measure(mocker):
@@ -291,16 +300,24 @@
 
     args['settlement_date'] = '1yr'
     with pytest.raises(MqValueError):
         tm_fxo.fwd_points(**args)
     args['settlement_date'] = '6m'
 
     args['real_time'] = True
-    with pytest.raises(NotImplementedError):
-        tm_fxo.fwd_points(**args)
+    xrefs = replace('gs_quant.timeseries.measures.Asset.get_identifier', Mock())
+    xrefs.return_value = 'EURUSD'
+    identifiers = replace('gs_quant.timeseries.measures_fx_vol._get_tdapi_fxo_assets', Mock())
+    identifiers.return_value = {'MAGZMXVM0J282ZTR'}
+    mocker.patch.object(GsDataApi, 'get_market_data', return_value=mock_curr(None, None))
+    actual = tm_fxo.fwd_points(**args)
+    expected = tm.ExtendedSeries([7, 8, 9], index=_index * 3, name='forwardPoint')
+    expected.dataset_ids = _test_datasets
+    assert_series_equal(expected, actual)
+    assert actual.dataset_ids == _test_datasets
     args['real_time'] = False
 
     args['asset'] = Cross('MAGZMXVM0J282ZTR', 'EURUSD')
     xrefs = replace('gs_quant.timeseries.measures.Asset.get_identifier', Mock())
     xrefs.return_value = 'EURUSD'
     identifiers = replace('gs_quant.timeseries.measures_fx_vol._get_tdapi_fxo_assets', Mock())
     identifiers.return_value = {'MAGZMXVM0J282ZTR'}
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_inflation.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_portfolios.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_rates.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     # mock
     cbd = replace('gs_quant.timeseries.measures._get_custom_bd', Mock())
     cbd.return_value = pd.tseries.offsets.BusinessDay()
     today = replace('gs_quant.timeseries.measures.pd.Timestamp.today', Mock())
     today.return_value = pd.Timestamp(2019, 5, 25)
     # cases
     assert tm_rates.parse_meeting_date() == dt.date(2019, 5, 24)
-    assert tm_rates.parse_meeting_date('3m') == pd.Timestamp(2019, 2, 24)
-    assert tm_rates.parse_meeting_date('3b') == pd.Timestamp(2019, 5, 22)
+    assert tm_rates.parse_meeting_date('3m') == dt.date(2019, 2, 24)
+    assert tm_rates.parse_meeting_date('3b') == dt.date(2019, 5, 22)
     # restore
     replace.restore()
 
 
 def test_get_swaption_parameter_floating_rate_option_returns_default():
     provider = TdapiRatesDefaultsProvider(SWAPTION_DEFAULTS)
     value = provider.get_swaption_parameter(CurrencyEnum.GBP, "floatingRateTenor")
@@ -1123,14 +1123,16 @@
             tm_rates.policy_rate_term_structure_rt(mock_eur, tm_rates.EventType.EOY, tm_rates.RateType.ABSOLUTE)
 
         with pytest.raises(MqError):
             tm_rates.policy_rate_term_structure_rt(mock_eur, tm_rates.EventType.SPOT, tm_rates.RateType.RELATIVE)
 
         mock_get_data = replace('gs_quant.data.dataset.Dataset.get_data', Mock())
         mock_get_data.return_value = mock_policy_term_rt_meeting()
+        mock_get_data_coverage = replace('gs_quant.data.dataset.Dataset.get_coverage', Mock())
+        mock_get_data_coverage.return_value = pd.DataFrame(columns=['exchange'])
 
         actual_abs = tm_rates.policy_rate_term_structure_rt(
             mock_eur,
             tm_rates.EventType.MEETING,
             tm_rates.RateType.ABSOLUTE,
             None)
         assert (target['meeting_absolute'] == actual_abs.loc[dt.date(2022, 7, 27)])
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_reports.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_risk_models.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_measures_xccy.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_rolling.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_rolling.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_statistics.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
     assert_series_equal(result, expected, obj="z-score window 1w")
 
     result = zscores(x, '1w')
     expected = pd.Series([1.603567], index=dates[-1:])
     assert_series_equal(result, expected, obj='z-score window string 1w')
 
     result = zscores(x, '1m')
-    expected = pd.Series(dtype=float)
+    expected = pd.Series(dtype=float, index=[])
     assert_series_equal(result, expected, obj="z-score window too large")
 
 
 def test_winsorize():
     assert_series_equal(winsorize(pd.Series(dtype=float)), pd.Series(dtype=float))
 
     x = generate_series(10000)
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_tca.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_technicals.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_technicals.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,14 @@
     result = relative_strength_index(SPX, w)
     assert_series_equal(result, expected, check_names=False, obj="Relative Strength Index")
 
     increasing_series = pd.Series(np.arange(1, 23, 1), index=dates)
     expected = pd.Series(data=np.ones(7) * 100, index=dates[15:])
     result = relative_strength_index(increasing_series, w)
     assert_series_equal(result, expected, check_names=False, obj="Relative Strength Index")
-
     result = relative_strength_index(SPX, "2w")
     print(result)
 
 
 def test_exponential_moving_average():
 
     def ema_by_hand(ts, alpha=0.75):
```

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/test_timeseries.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/timeseries/utils.py` & `gs_quant-1.0.0/gs_quant/test/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/utils/datagrid_test_utils.py` & `gs_quant-1.0.0/gs_quant/test/utils/datagrid_test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/utils/mock_calc.py` & `gs_quant-1.0.0/gs_quant/test/utils/mock_calc.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/utils/mock_data.py` & `gs_quant-1.0.0/gs_quant/test/utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/test/utils/mock_request.py` & `gs_quant-1.0.0/gs_quant/test/utils/mock_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import json
 import os
 from abc import abstractmethod
 from os.path import exists
 from typing import List
 from unittest import mock
 
+from gs_quant.errors import MqUninitialisedError
 from gs_quant.session import GsSession, Environment
 
 
 class MockRequest:
     __looked_at_files = {}
     __saved_files = set()
     api = None
@@ -41,17 +42,20 @@
 
     def __enter__(self):
         if self.save_files:
             GsSession.use(Environment.PROD, None, None, application=self.application)
             self.mocker.patch.object(self.api, self.method, side_effect=self.mock_calc_create_new_files if str(
                 self.save_files).casefold() == 'new' else self.mock_calc_create_files)
         else:
-            from gs_quant.session import OAuth2Session
-            OAuth2Session.init = mock.MagicMock(return_value=None)
-            GsSession.use(Environment.PROD, 'fake_client_id', 'fake_secret', application=self.application)
+            try:
+                _ = GsSession.current
+            except MqUninitialisedError:
+                from gs_quant.session import OAuth2Session
+                OAuth2Session._authenticate = mock.MagicMock(return_value=None)
+                GsSession.use(Environment.PROD, 'fake_client_id', 'fake_secret', application=self.application)
             self.mocker.patch.object(self.api, self.method, side_effect=self.mock_calc)
 
     def mock_calc(self, *args, **kwargs):
         request_id = self.get_request_id(args, kwargs)
         file_name = f'request{request_id}.json'
         with open(self.paths / f'calc_cache/{file_name}') as json_data:
             MockRequest.__looked_at_files.setdefault(self.paths, set()).add(file_name)
```

### Comparing `gs_quant-0.9.99/gs_quant/test/utils/test_utils.py` & `gs_quant-1.0.0/gs_quant/test/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/__init__.py` & `gs_quant-1.0.0/gs_quant/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/algebra.py` & `gs_quant-1.0.0/gs_quant/timeseries/algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/analysis.py` & `gs_quant-1.0.0/gs_quant/timeseries/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
         y = x.copy()  # avoid mutating the provided series
 
         match = re.fullmatch('(\\d+)y', obs)
         if match:
             y.index += pd.DateOffset(years=int(match.group(1)))
             y = y.groupby(y.index).first()
         else:
-            y.index += pd.DateOffset(relative_date_add(obs))
+            y.index = pd.DatetimeIndex([(i + pd.DateOffset(relative_date_add(obs))).date() for i in y.index])
 
         if mode == LagMode.EXTEND:
             return y
         return y[:end]
 
     obs = getattr(obs, 'w', obs)
     # Determine how we want to handle observations prior to start date
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/backtesting.py` & `gs_quant-1.0.0/gs_quant/timeseries/backtesting.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .statistics import *
 from ..api.gs.assets import GsAssetApi
 from ..api.gs.data import GsDataApi, MarketDataResponseFrame
 from ..data.log import log_debug
 
 _logger = logging.getLogger(__name__)
 
-RebalFreq = _create_enum('RebalFreq', ['Daily', 'Monthly'])
+RebalFreq = _create_enum('RebalFreq', ['Daily', 'Weekly', 'Monthly'])
 ReturnType = _create_enum('ReturnType', ['excess_return'])
 
 
 def backtest_basket(
         series: list,
         weights: list,
         costs: list = None,
@@ -66,20 +66,25 @@
     series = pd.concat([curve.reindex(cal) for curve in series], axis=1)
     weights = pd.concat([pd.Series(w, index=cal) for w in weights], axis=1)
     costs = pd.concat([pd.Series(c, index=cal) for c in costs], axis=1)
 
     if rebal_freq == RebalFreq.DAILY:
         rebal_dates = cal
     else:
-        # Get hypothetical monthly rebalances
-        num_rebals = (cal[-1].year - cal[0].year) * 12 + cal[-1].month - cal[0].month
-        rebal_dates = [cal[0] + i * rdelta(months=1) for i in range(num_rebals + 1)]
-        # Convert these to actual calendar days
-        rebal_dates = [d for d in rebal_dates if d < max(cal)]
-        rebal_dates = [min(cal[cal >= date]) for date in rebal_dates]
+        if rebal_freq == RebalFreq.WEEKLY:
+            # Get hypothetical weekly rebalances
+            num_rebals = ((cal[-1] - cal[0]).days) // 7
+            rebal_dates = [cal[0] + i * rdelta(weeks=1) for i in range(num_rebals + 1)]
+        else:
+            # Get hypothetical monthly rebalances
+            num_rebals = (cal[-1].year - cal[0].year) * 12 + cal[-1].month - cal[0].month
+            rebal_dates = [cal[0] + i * rdelta(months=1) for i in range(num_rebals + 1)]
+
+        # Convert the hypothetical weekly/monthly rebalance dates to actual calendar days
+        rebal_dates = [min(cal[cal >= date]) for date in rebal_dates if date < max(cal)]
 
     # Create Units dataframe
     units = pd.DataFrame(index=cal, columns=series.columns)
     actual_weights = pd.DataFrame(index=cal, columns=series.columns)
     output = pd.Series(dtype='float64', index=cal)
 
     # Initialize backtest
@@ -136,15 +141,15 @@
 ) -> pd.Series:
     """
     Calculates a basket return series.
 
     :param series: list of time series of instrument prices
     :param weights: list of weights (defaults to evenly weight series)
     :param costs: list of execution costs in decimal (defaults to costs of 0)
-    :param rebal_freq: rebalancing frequency - Daily or Monthly (defaults to Daily)
+    :param rebal_freq: rebalancing frequency - Daily, Weekly or Monthly (defaults to Daily)
     :param return_type: return type of underlying instruments - only excess return is supported
     :return: time series of the resulting basket
 
     **Usage**
 
     Calculates a basket return series.
 
@@ -451,10 +456,10 @@
                                    name='forwardVol')
             s[asset_id] = series
 
         vols = pd.DataFrame(s)
         actual_weights = self.get_actual_weights(request_id)
 
         # Necessary when current values appended - set weights index to match vols index
-        actual_weights = actual_weights.reindex(vols.index).fillna(method='pad')
+        actual_weights = actual_weights.reindex(pd.DatetimeIndex(vols.index)).fillna(method='pad')
 
         return actual_weights.mul(vols).sum(axis=1, skipna=False)
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/datetime.py` & `gs_quant-1.0.0/gs_quant/timeseries/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,46 +12,51 @@
 #
 #
 # Chart Service will attempt to make public functions (not prefixed with _) from this module available. Such functions
 # should be fully documented: docstrings should describe parameters and the return value, and provide a 1-line
 # description. Type annotations should be provided for parameters.
 from datetime import date, time, timedelta
 from numbers import Real
+from typing import Any
 
-import numpy as np
+from pandas.tseries.offsets import CustomBusinessDay
 
 from .helper import *
 from .helper import _create_enum
+from ..datetime import GsCalendar
 from ..datetime.date import DayCountConvention, PaymentFrequency, day_count_fraction
 from ..datetime.date import date_range as _date_range
 from ..errors import MqValueError, MqTypeError
 
 """
 Date and time manipulation for timeseries, including date or time shifting, calendar operations, curve alignment and
 interpolation operations. Includes sampling operations based on daif dates[0]te or time manipulation
 """
 
-AggregateFunction = _create_enum('AggregateFunction', ['max', 'min', 'mean', 'sum'])
+AggregateFunction: Union[Union[type, Enum], Any] = _create_enum(
+    'AggregateFunction',
+    ['max', 'min', 'mean', 'sum', 'first', 'last']
+)
 AggregatePeriod = _create_enum('AggregatePeriod', ['week', 'month', 'year'])
 
 
 def __interpolate_step(x: pd.Series, dates: pd.Series = None) -> pd.Series:
     if x.empty:
         raise MqValueError('Cannot perform step interpolation on an empty series')
 
     first_date = pd.Timestamp(dates.index[0]) if isinstance(x.index[0], pd.Timestamp) else dates.index[0]
 
     # locate previous valid date or take first value from series
-    prev = x.index[0] if first_date < x.index[0] else x.index[x.index.get_loc(first_date, 'pad')]
+    prev = x.index[0] if first_date < x.index[0] else x.index[x.index.get_indexer([first_date], method='pad')]
 
     current = x[prev]
 
     curve = x.align(dates, 'right', )[0]  # only need values from dates
 
-    for knot in curve.iteritems():
+    for knot in curve.items():
         if np.isnan(knot[1]):
             curve[knot[0]] = current
         else:
             current = knot[1]
     return curve
 
 
@@ -271,15 +276,15 @@
     >>> days = day(series)
 
     **See also**
 
     :func:`month` :func:`year`
 
     """
-    return pd.to_datetime(x.index.to_series()).dt.day
+    return pd.Series(pd.to_datetime(x.index.to_series()).dt.day, dtype=np.int64)
 
 
 @plot_function
 def month(x: pd.Series) -> pd.Series:
     """
     Month of each value in series
 
@@ -302,15 +307,15 @@
     >>> days = month(series)
 
     **See also**
 
     :func:`day` :func:`year`
 
     """
-    return pd.to_datetime(x.index.to_series()).dt.month
+    return pd.Series(pd.to_datetime(x.index.to_series()).dt.month, dtype=np.int64)
 
 
 @plot_function
 def year(x: pd.Series) -> pd.Series:
     """
     Year of each value in series
 
@@ -333,15 +338,15 @@
     >>> days = year(series)
 
     **See also**
 
     :func:`day` :func:`month`
 
     """
-    return pd.to_datetime(x.index.to_series()).dt.year
+    return pd.Series(pd.to_datetime(x.index.to_series()).dt.year, dtype=np.int64)
 
 
 @plot_function
 def quarter(x: pd.Series) -> pd.Series:
     """
     Quarter of each value in series
 
@@ -364,15 +369,15 @@
     >>> days = quarter(series)
 
     **See also**
 
     :func:`day` :func:`month`
 
     """
-    return pd.to_datetime(x.index.to_series()).dt.quarter
+    return pd.Series(pd.to_datetime(x.index.to_series()).dt.quarter, dtype=np.int64)
 
 
 @plot_function
 def weekday(x: pd.Series) -> pd.Series:
     """
     Weekday of each value in series
 
@@ -395,15 +400,15 @@
     >>> days = weekday(series)
 
     **See also**
 
     :func:`day` :func:`month`
 
     """
-    return pd.to_datetime(x.index.to_series()).dt.weekday
+    return pd.Series(pd.to_datetime(x.index.to_series()).dt.weekday, dtype=np.int64)
 
 
 @plot_function
 def day_count_fractions(
         dates: Union[List[date], pd.Series],
         convention: DayCountConvention = DayCountConvention.ACTUAL_360,
         frequency: PaymentFrequency = PaymentFrequency.MONTHLY
@@ -490,15 +495,15 @@
     **See also**
 
     :func:`day` :func: `lag`
 
     """
     if not isinstance(weekdays_only, bool):
         raise MqTypeError('expected a boolean value for "weekdays_only"')
-    if not (x.index.is_all_dates or all(map(lambda a: isinstance(a, date), x.index.values))):
+    if not (isinstance(x.index, pd.DatetimeIndex) or all(map(lambda a: isinstance(a, date), x.index.values))):
         raise MqValueError('input is not a time series')
 
     if isinstance(start_date, int):
         start_date = x.index[start_date]
     if isinstance(end_date, int):
         end_date = x.index[- (1 + end_date)]
 
@@ -512,15 +517,15 @@
         week_mask = None
         wd = start_date.weekday()
         if wd > 4:
             start_date += timedelta(days=7 - wd)
     else:
         week_mask = tuple([True] * 7)
 
-    return x.loc[x.index.intersection(list(_date_range(start_date, end_date, week_mask=week_mask)))]
+    return x.loc[x.index.isin(list(_date_range(start_date, end_date, week_mask=week_mask)))]
 
 
 @plot_function
 def append(series: List[pd.Series]) -> pd.Series:
     """
     Append data series
 
@@ -547,15 +552,15 @@
     """
     if not len(series):
         return pd.Series(dtype='float64')
     res = series[0].copy()
     for i in range(1, len(series)):
         cur = series[i]
         start = res.index[-1]
-        res = res.append(cur.loc[cur.index > start])
+        res = pd.concat([res, cur.loc[cur.index > start]])
     return res
 
 
 @plot_function
 def prepend(x: List[pd.Series]) -> pd.Series:
     """
     Prepend data series
@@ -582,17 +587,17 @@
     :func:`union`
 
     """
     res = pd.Series(dtype='float64')
     for i in range(len(x)):
         this = x[i]
         if i == len(x) - 1:
-            return res.append(this)
+            return pd.concat([res, this])
         end = x[i + 1].index[0]
-        res = res.append(this.loc[this.index < end])
+        res = pd.concat([res, this.loc[this.index < end]])
     return res
 
 
 @plot_function
 def union(x: List[pd.Series]) -> pd.Series:
     """
     Fill in missing dates or times of one series with another
@@ -672,7 +677,30 @@
     :param first: first date
     :param second: second date
     :return: number of business days between first and second
     """
     if not (isinstance(first, date) and isinstance(second, date)):
         raise MqValueError('inputs must be dates')
     return np.busday_count(first, second)
+
+
+@plot_function
+def align_calendar(series: pd.Series, calendar: str) -> pd.Series:
+    """
+    Aligns a series to a given calendar removing values in the holiday calendar and the week mask (i.e. remove Saturday
+    and Sunday)
+
+    :param series: data series to align
+    :param calendar: calendar to align the series (i.e. NYC, NYSE, USD)
+
+    :return: timeseries of the data aligned to a calendar
+
+    **Examples**
+
+    >>> x = generate_series(100)
+    >>> align_calendar(x, 'NYC')
+    """
+    gs_calendar = GsCalendar.get(calendar)
+    cbd = CustomBusinessDay(calendar=gs_calendar.business_day_calendar())
+    filtered_series = series[
+        series.index.isin(pd.date_range(start=series.first_valid_index(), end=series.last_valid_index(), freq=cbd))]
+    return filtered_series
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/econometrics.py` & `gs_quant-1.0.0/gs_quant/timeseries/econometrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 #
 # Chart Service will attempt to make public functions (not prefixed with _) from this module available. Such functions
 # should be fully documented: docstrings should describe parameters and the return value, and provide a 1-line
 # description. Type annotations should be provided for parameters.
-from .analysis import LagMode, lag
-from .statistics import *
-from ..errors import *
 from typing import Union
+
 import numpy as np
 import pandas as pd
 from gs_quant.api.gs.data import GsDataApi
 from gs_quant.data import DataContext
 from gs_quant.datetime.date import DayCountConvention
 from gs_quant.markets.securities import Asset
 from gs_quant.target.common import Currency
 from gs_quant.timeseries.datetime import align
 
+from .analysis import LagMode, lag
+from .statistics import *
+from ..errors import *
+
 """
 Econometrics timeseries library is for standard economic and time series analytics operations, including returns,
 diffs, lags, volatilities and other numerical operations which are generally finance-oriented
 """
 
 
 class AnnualizationFactor(IntEnum):
@@ -632,16 +634,21 @@
     ret_1 = returns(x) if given_prices else x
     ret_2 = returns(y) if given_prices else y
 
     clean_ret1 = ret_1.dropna()
     clean_ret2 = ret_2.dropna()
 
     if isinstance(w.w, pd.DateOffset):
-        values = [clean_ret1.loc[(clean_ret1.index > idx - w.w) & (clean_ret1.index <= idx)].corr(clean_ret2)
-                  for idx in clean_ret1.index]
+        if isinstance(clean_ret1.index, pd.DatetimeIndex):
+            values = [clean_ret1.loc[(clean_ret1.index > idx - w.w) & (clean_ret1.index <= idx)].corr(clean_ret2)
+                      for idx in clean_ret1.index]
+        else:
+            values = [clean_ret1.loc[(clean_ret1.index > (idx - w.w).date()) &
+                                     (clean_ret1.index <= idx)].corr(clean_ret2)
+                      for idx in clean_ret1.index]
         corr = pd.Series(values, index=clean_ret1.index)
     else:
         corr = clean_ret1.rolling(w.w, 0).corr(clean_ret2)
 
     return apply_ramp(interpolate(corr, x, Interpolate.NAN), w)
 
 
@@ -714,15 +721,15 @@
 
         cov_results = np.empty(size, dtype=np.double)
         var_results = np.empty(size, dtype=np.double)
 
         offset = w.w
         start = 0
         for i in range(1, size):
-            min_index_value = series_index[i] - offset
+            min_index_value = (series_index[i] - offset).date()
             for idx in range(start, i + 1):
                 if series_index[idx] > min_index_value:
                     start = idx
                     break
 
             sub_benchmark_values = benchmark_values[start:i + 1]
             var_results[i] = np.var(sub_benchmark_values, ddof=1)
@@ -761,15 +768,18 @@
     **See also**
 
     :func:`returns`
 
     """
     w = normalize_window(x, w)
     if isinstance(w.w, pd.DateOffset):
-        scores = pd.Series([x[idx] / x.loc[(x.index > idx - w.w) & (x.index <= idx)].max() - 1 for idx in x.index],
-                           index=x.index)
-        result = pd.Series([scores.loc[(scores.index > idx - w.w) & (scores.index <= idx)].min()
-                            for idx in scores.index], index=scores.index)
+        if np.issubdtype(x.index, dt.date):
+            scores = pd.Series([x[idx] / x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].max() - 1
+                                for idx in x.index], index=x.index)
+            result = pd.Series([scores.loc[(scores.index > (idx - w.w).date()) & (scores.index <= idx)].min()
+                                for idx in scores.index], index=scores.index)
+        else:
+            raise TypeError('Please pass in list of dates as index')
     else:
         rolling_max = x.rolling(w.w, 0).max()
         result = (x / rolling_max - 1).rolling(w.w, 0).min()
     return apply_ramp(result, w)
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/helper.py` & `gs_quant-1.0.0/gs_quant/timeseries/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
 
 try:
     from quant_extensions.timeseries.rolling import rolling_apply
 except ImportError as e:
     _logger.debug('unable to import rolling_apply extension: %s', e)
 
     def rolling_apply(s: pd.Series, offset: pd.DateOffset, function: Callable[[np.ndarray], float]) -> pd.Series:
-        values = [function(s.loc[(s.index > idx - offset) & (s.index <= idx)]) for idx in s.index]
+        if isinstance(s.index, pd.DatetimeIndex):
+            values = [function(s.loc[(s.index > (idx - offset)) & (s.index <= idx)]) for idx in s.index]
+        else:
+            values = [function(s.loc[(s.index > (idx - offset).date()) & (s.index <= idx)]) for idx in s.index]
         return pd.Series(values, index=s.index, dtype=np.double)
 
 
 def _create_enum(name, members):
     return Enum(name, {n.upper(): n.lower() for n in members}, module=__name__)
 
 
@@ -141,15 +144,18 @@
 
 
 def apply_ramp(x: pd.Series, window: Window) -> pd.Series:
     _check_window(len(x), window)
     if isinstance(window.w, int) and window.w > len(x):  # does not restrict window size when it is a DataOffset
         return pd.Series(dtype=float)
     if isinstance(window.r, pd.DateOffset):
-        return x.loc[x.index[0] + window.r:]
+        if np.issubdtype(x.index, dt.date):
+            return x.loc[(x.index[0] + window.r).date():]
+        else:
+            return x.loc[(x.index[0] + window.r).to_pydatetime():]
     else:
         return x[window.r:]
 
 
 def normalize_window(x: Union[pd.Series, pd.DataFrame], window: Union[Window, int, str, None],
                      default_window: int = None) -> Window:
     if default_window is None:
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measure_registry.py` & `gs_quant-1.0.0/gs_quant/timeseries/measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 from collections import namedtuple
 from numbers import Real
 
 import cachetools.func
 import inflection
 import numpy as np
 from dateutil import tz
-from pandas import Series, DatetimeIndex
-from pandas.tseries.holiday import Holiday, AbstractHolidayCalendar, USMemorialDay, USLaborDay, USThanksgivingDay, \
-    sunday_to_monday
-from pydash import chunk, flatten
-
 from gs_quant.api.gs.data import MarketDataResponseFrame
 from gs_quant.api.gs.data import QueryType
 from gs_quant.api.gs.indices import GsIndexApi
 from gs_quant.data.core import DataContext
 from gs_quant.data.fields import Fields
 from gs_quant.data.log import log_debug, log_warning
 from gs_quant.datetime import DAYS_IN_YEAR
@@ -42,14 +37,18 @@
     plot_measure,
     _to_offset,
     check_forward_looking,
     get_df_with_retries,
     get_dataset_data_with_retries, _tenor_to_month, _month_to_tenor, _split_where_conditions
 )
 from gs_quant.timeseries.measures_helper import EdrDataReference, VolReference, preprocess_implied_vol_strikes_eq
+from pandas import Series, DatetimeIndex
+from pandas.tseries.holiday import Holiday, AbstractHolidayCalendar, USMemorialDay, USLaborDay, USThanksgivingDay, \
+    sunday_to_monday
+from pydash import chunk, flatten
 
 GENERIC_DATE = Union[datetime.date, str]
 ASSET_SPEC = Union[Asset, str]
 TD_ONE = datetime.timedelta(days=1)
 
 _logger = logging.getLogger(__name__)
 
@@ -2236,35 +2235,41 @@
     check_forward_looking(pricing_date, source, 'fwd_term')
     cbd = _get_custom_bd(asset.exchange)
     start, end = _range_from_pricing_date(asset.exchange, pricing_date)
     start = start + cbd - cbd  # get previous business day's pricing if start, end on a non-BD
     with DataContext(start, end):
         q = GsDataApi.build_market_data_query([asset_id], QueryType.FORWARD_POINT, where={}, source=source,
                                               real_time=real_time)
-        q_spot = GsDataApi.build_market_data_query([asset_id], QueryType.SPOT, where={}, source=source,
+        # setting pricing location as NYC as we have forward points only for NYC close
+        q_spot = GsDataApi.build_market_data_query([asset_id], QueryType.SPOT, where={'pricingLocation': 'NYC'},
+                                                   source=source,
                                                    real_time=real_time)
         data_requests = [partial(_market_data_timed, q, request_id),
                          partial(_market_data_timed, q_spot, request_id)]
         df, spot_df = measure_request_safe('fwd_term', asset, ThreadPoolManager.run_async, request_id, data_requests)
     dataset_ids = set(getattr(df, 'dataset_ids', ()) + getattr(spot_df, 'dataset_ids', ()))
     if df.empty:
         series = ExtendedSeries(dtype=float)
     else:
         latest = df.index.max()
         _logger.info('selected pricing date %s', latest)
         df = df.loc[latest]
-        df.loc[:, 'expirationDate'] = df.index + df['tenor'].map(_to_offset) + cbd - cbd
+        df = df.assign(expirationDate=df.index + df['tenor'].map(_to_offset) + cbd - cbd)
+
         df = df.set_index('expirationDate')
         df.sort_index(inplace=True)
         df = df.loc[DataContext.current.start_date: DataContext.current.end_date]
         spot = spot_df.loc[latest]['spot']
-        df[forward_col_name] = df[forward_col_name] / spot
+
         if annualized == FXSpotCarry.ANNUALIZED:
-            df[forward_col_name] = df[forward_col_name] * np.sqrt((df.index.to_series() - latest).dt.days / 252)
-        series = ExtendedSeries(dtype=float) if df.empty else ExtendedSeries(df[forward_col_name])
+            df['carry'] = df[forward_col_name] * np.sqrt((df.index.to_series() - latest).dt.days / 252) / spot
+        else:
+            df['carry'] = df[forward_col_name] / spot
+
+        series = ExtendedSeries(dtype=float) if df.empty else ExtendedSeries(df['carry'])
     series.name = 'carry'
     series.dataset_ids = tuple(dataset_ids)
     return series
 
 
 @cachetools.func.ttl_cache()  # fine as long as availability is not different between users
 def _var_swap_tenors(asset: Asset, request_id=None):
@@ -2964,18 +2969,16 @@
         return _forward_price_eu_natgas(asset, contract_range, price_method)
     else:
         raise MqTypeError('The forward_price_ng is not supported for this asset')
 
 
 def get_contract_range(start_contract_range, end_contract_range, timezone):
     if timezone:
-        df = pd.date_range(start=start_contract_range,
-                           end=end_contract_range + datetime.timedelta(days=1), freq='H',
-                           closed='left',
-                           tz=timezone).to_frame()
+        df = pd.date_range(start_contract_range, end_contract_range + datetime.timedelta(days=1), None, 'H',
+                           timezone, False, None, 'left').to_frame()
 
         df['hour'] = df.index.hour
         df['day'] = df.index.dayofweek
     else:
         df = pd.date_range(start=start_contract_range,
                            end=end_contract_range,
                            ).to_frame()
@@ -3058,15 +3061,16 @@
         df = df.drop_duplicates()
         # freq is the frequency at which the ISO publishes data for e.g. 15 min, 1hr
         freq = int(min(np.diff(df.index).astype('timedelta64[s]') / np.timedelta64(1, 's')))
         if freq == 0:
             raise MqValueError('Duplicate data rows probable for this period')
         # checking missing data points
         ref_hour_range = pd.date_range(str(start_date), str(end_date + datetime.timedelta(days=1)),
-                                       freq=str(freq) + "S", tz=timezone, closed='left')
+                                       None, str(freq) + "S", timezone, False, None, 'left')
+
         missing_hours = ref_hour_range[~ref_hour_range.isin(df.index)]
         missing_dates = np.unique(missing_hours.date)
         missing_months = np.unique(np.array(missing_dates, dtype='M8[D]').astype('M8[M]')).astype('str')
 
         # drop dates and months which have missing data
         df = df.loc[(~df['date'].isin(missing_dates))]
         if granularity == 'M':
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_countries.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_fx_vol.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_fx_vol.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,16 +285,25 @@
     "NZDUSD": "MA9RP21MYV18TW3E",
     "USDCNH": "MAQEB18HP88FEP5G",
     "INRUSD": "MAMC996297G5GEAM",
     "USDSGD": "MAFCHSQN3NH77G17"
 }
 
 
-def _currencypair_to_tdapi_fxfwd_asset(_asset_spec: ASSET_SPEC) -> str:
-    return "MA8RY265Q34P7TWZ"
+def _currencypair_to_tdapi_fxfwd_asset(asset_spec: ASSET_SPEC) -> str:
+    asset = _asset_from_spec(asset_spec)
+    bbid = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
+
+    kwargs = dict(asset_class='FX', type='Forward',
+                  asset_parameters_pair=bbid,
+                  asset_parameters_settlement_date='1y',
+                  )
+
+    mqid = _get_tdapi_fxo_assets(**kwargs)
+    return mqid
 
 
 def _currencypair_to_tdapi_fxo_asset(asset_spec: ASSET_SPEC) -> str:
     asset = _asset_from_spec(asset_spec)
     bbid = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
     # for each currency, get a dummy asset for checking availability
     result = CURRENCY_TO_DUMMY_FFO_BBID.get(bbid, asset.get_marquee_id())
@@ -319,14 +328,55 @@
         raise MqValueError('Specified arguments match multiple assets' + str(kwargs))
     elif len(assets) == 0:
         raise MqValueError('Specified arguments did not match any asset in the dataset' + str(kwargs))
     else:
         return assets[0].id
 
 
+def get_fxo_asset(asset: Asset, expiry_tenor: str, strike: str, option_type: str = None,
+                  expiration_location: str = None, premium_payment_date: str = None) -> str:
+    cross = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
+
+    if cross not in FX_DEFAULTS.keys():
+        raise NotImplementedError('Data not available for {} FX Vanilla options'.format(cross))
+
+    defaults = _get_fxo_defaults(cross)
+
+    if not (tm_rates._is_valid_relative_date_tenor(expiry_tenor)):
+        raise MqValueError('invalid expiry ' + expiry_tenor)
+
+    if expiration_location is None:
+        _ = defaults["expirationTime"]
+    else:
+        _ = expiration_location
+
+    if premium_payment_date is None:
+        premium_date = defaults["premiumPaymentDate"]
+    else:
+        premium_date = premium_payment_date
+
+    if option_type == "Put":
+        call_ccy = defaults["over"]
+        put_ccy = defaults["under"]
+    else:
+        call_ccy = defaults["under"]
+        put_ccy = defaults["over"]
+
+    kwargs = dict(asset_class='FX', type='Option',
+                  asset_parameters_call_currency=call_ccy,
+                  asset_parameters_put_currency=put_ccy,
+                  asset_parameters_expiration_date=expiry_tenor,
+                  asset_parameters_option_type=option_type,
+                  asset_parameters_premium_payment_date=premium_date,
+                  asset_parameters_strike_price_relative=strike,
+                  )
+
+    return _get_tdapi_fxo_assets(**kwargs)
+
+
 def _get_tdapi_fxo_assets_vol_swaps(**kwargs) -> Union[str, list]:
     # sanitize input for asset query.
 
     expiry_tenor = kwargs.get("expiry_tenor")
     ignore_list = ["expiry_tenor", "pricing_location"]
     inputs = {k: v for k, v in kwargs.items() if k not in ignore_list}
 
@@ -372,15 +422,15 @@
 
 def _get_fx_vol_swap_data(asset: Asset, expiry_tenor: str, strike_type: str = None,
                           location: PricingLocation = None,
                           source: str = None, real_time: bool = False,
                           query_type: QueryType = QueryType.STRIKE_VOL) \
         -> pd.DataFrame:
     if real_time:
-        raise NotImplementedError('realtime inflation swap data not implemented')
+        raise NotImplementedError('realtime FX Vol swap data not implemented')
 
     cross = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
 
     if cross not in FX_VOL_SWAP_DEFAULTS:
         raise NotImplementedError('Data not available for {} FX Vol Swaps'.format(cross))
 
     kwargs = dict(asset_class='FX', type='VolatilitySwap',
@@ -406,86 +456,58 @@
 
 def _get_fxfwd_data(asset: Asset, settlement_date: str,
                     location: str = None,
                     source: str = None, real_time: bool = False,
                     query_type: QueryType = QueryType.FWD_POINTS) \
         -> pd.DataFrame:
     if real_time:
-        raise NotImplementedError('realtime inflation swap data not implemented')
+        mqid = asset.get_identifier(AssetIdentifier.MARQUEE_ID)
+        q = GsDataApi.build_market_data_query([mqid], QueryType.FORWARD_POINT, source=source,
+                                              real_time=real_time, where={'tenor': settlement_date})
+        _logger.debug('q %s', q)
+        df = _market_data_timed(q)
+        return df
+
     cross = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
 
     if not (tm_rates._is_valid_relative_date_tenor(settlement_date)):
         raise MqValueError('invalid settlements date ' + settlement_date)
 
     kwargs = dict(asset_class='FX', type='Forward',
                   asset_parameters_pair=cross,
                   asset_parameters_settlement_date=settlement_date,
                   )
 
-    rate_mqid = _get_tdapi_fxo_assets(**kwargs)
+    mqid = _get_tdapi_fxo_assets(**kwargs)
 
     if location is None:
         pricing_location = PricingLocation.NYC
     else:
         pricing_location = PricingLocation(location)
 
     where = dict(pricingLocation=pricing_location.value)
 
-    q = GsDataApi.build_market_data_query([rate_mqid], query_type, where=where, source=source,
+    q = GsDataApi.build_market_data_query([mqid], query_type, where=where, source=source,
                                           real_time=real_time)
     _logger.debug('q %s', q)
     df = _market_data_timed(q)
     return df
 
 
 def _get_fxo_data(asset: Asset, expiry_tenor: str, strike: str, option_type: str = None,
                   expiration_location: str = None,
                   location: PricingLocation = None, premium_payment_date: str = None,
                   source: str = None, real_time: bool = False,
                   query_type: QueryType = QueryType.IMPLIED_VOLATILITY) \
         -> pd.DataFrame:
     if real_time:
-        raise NotImplementedError('realtime inflation swap data not implemented')
-    cross = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
-
-    if cross not in FX_DEFAULTS.keys():
-        raise NotImplementedError('Data not available for {} FX Vanilla options'.format(cross))
-
-    defaults = _get_fxo_defaults(cross)
-
-    if not (tm_rates._is_valid_relative_date_tenor(expiry_tenor)):
-        raise MqValueError('invalid expiry ' + expiry_tenor)
-
-    if expiration_location is None:
-        _ = defaults["expirationTime"]
-    else:
-        _ = expiration_location
-
-    if premium_payment_date is None:
-        premium_date = defaults["premiumPaymentDate"]
-    else:
-        premium_date = premium_payment_date
+        raise NotImplementedError('realtime FX Option data not implemented')
 
-    if option_type == "Put":
-        call_ccy = defaults["over"]
-        put_ccy = defaults["under"]
-    else:
-        call_ccy = defaults["under"]
-        put_ccy = defaults["over"]
-
-    kwargs = dict(asset_class='FX', type='Option',
-                  asset_parameters_call_currency=call_ccy,
-                  asset_parameters_put_currency=put_ccy,
-                  asset_parameters_expiration_date=expiry_tenor,
-                  asset_parameters_option_type=option_type,
-                  asset_parameters_premium_payment_date=premium_date,
-                  asset_parameters_strike_price_relative=strike,
-                  )
-
-    asset_mqid = _get_tdapi_fxo_assets(**kwargs)
+    asset_mqid = get_fxo_asset(asset=asset, expiry_tenor=expiry_tenor, strike=strike, option_type=option_type,
+                               expiration_location=expiration_location, premium_payment_date=premium_payment_date)
 
     if location is None:
         pricing_location = PricingLocation.NYC
     else:
         pricing_location = PricingLocation(location)
 
     where = dict(pricingLocation=pricing_location.value)
@@ -569,15 +591,15 @@
 
 
 """
 New Implementation
 """
 
 
-@plot_measure((AssetClass.FX,), None,
+@plot_measure((AssetClass.FX,), (AssetType.Cross,),
               [MeasureDependency(id_provider=cross_stored_direction_for_fx_vol,
                                  query_type=QueryType.IMPLIED_VOLATILITY)],
               display_name="implied_volatility")
 def implied_volatility_fxvol(asset: Asset, tenor: str, strike_reference: VolReference = None,
                              relative_strike: Real = None, location: Optional[PricingLocation] = None,
                              legacy_implementation: bool = False, *,
                              source: str = None, real_time: bool = False,
@@ -603,14 +625,18 @@
                                           source=source, real_time=real_time, request_id=request_id))
 
     bbid = asset.get_identifier(AssetIdentifier.BLOOMBERG_ID)
     if bbid is not None:
         cross = _cross_stored_direction_helper(bbid)
         if cross != bbid:
             cross_asset = SecurityMaster.get_asset(cross, AssetIdentifier.BLOOMBERG_ID)
+            if strike_reference.value == VolReference.DELTA_CALL.value:
+                strike_reference = VolReference.DELTA_PUT
+            elif strike_reference.value == VolReference.DELTA_PUT.value:
+                strike_reference = VolReference.DELTA_CALL
         else:
             cross_asset = asset
     else:
         raise MqValueError('Badly setup cross ' + asset.name)
 
     ref_string, relative_strike = _preprocess_implied_vol_strikes_fx(strike_reference, relative_strike)
 
@@ -655,16 +681,18 @@
     :param source: name of function caller
     :param real_time: whether to retrieve intraday data instead of EOD
     :return: fwd points
     """
     df = _get_fxfwd_data(asset=asset, settlement_date=settlement_date,
                          location=location, source=source,
                          real_time=real_time, query_type=QueryType.FWD_POINTS)
-
-    series = ExtendedSeries(dtype=float) if df.empty else ExtendedSeries(df['fwdPoints'])
+    if real_time:
+        series = ExtendedSeries(dtype=float) if df.empty else ExtendedSeries(df['forwardPoint'])
+    else:
+        series = ExtendedSeries(dtype=float) if df.empty else ExtendedSeries(df['fwdPoints'])
     series.dataset_ids = getattr(df, 'dataset_ids', ())
     return series
 
 
 @plot_measure((AssetClass.FX,), (AssetType.Cross,),
               [MeasureDependency(id_provider=_currencypair_to_tdapi_fx_vol_swap_asset,
                                  query_type=QueryType.STRIKE_VOL)])
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_helper.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_inflation.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_portfolios.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_rates.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_reports.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_risk_models.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/measures_xccy.py` & `gs_quant-1.0.0/gs_quant/timeseries/measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/statistics.py` & `gs_quant-1.0.0/gs_quant/timeseries/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #
 # Marquee Plot Service will attempt to make public functions (not prefixed with _) from this module available.
 # Such functions should be fully documented: docstrings should describe parameters and the return value, and provide
 # a 1-line description. Type annotations should be provided for parameters.
 
 import datetime
 import numpy
+import pandas as pd
 import scipy.stats.mstats as stats
 from scipy.stats import percentileofscore
 from statsmodels.regression.rolling import RollingOLS
 from .algebra import *
 import statsmodels.api as sm
 from ..models.epidemiology import SIR, SEIR, EpidemicModel
 from ..data import DataContext
@@ -124,15 +125,15 @@
     """
     if isinstance(x, list):
         x = _concat_series(x).min(axis=1)
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
         values = rolling_offset(x, w.w, np.nanmin, 'min') if isinstance(x, pd.Series) else [
-            x.loc[(x.index > idx - w.w) & (x.index <= idx)].min() for idx in x.index]
+            x.loc[(x.index > (idx - w.w).datetime()) & (x.index <= idx)].min() for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).min(), w)
 
 
 @plot_function
 def max_(x: Union[pd.Series, List[pd.Series]], w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -289,15 +290,15 @@
         x = pd.concat(x, axis=1)
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
         if isinstance(x, pd.Series):
             values = rolling_offset(x, w.w, np.nanmean, 'mean')
         else:
-            values = [np.nanmean(x.loc[(x.index > idx - w.w) & (x.index <= idx)]) for idx in x.index]
+            values = [np.nanmean(x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)]) for idx in x.index]
     else:
         if isinstance(x, pd.Series):
             values = x.rolling(w.w, 0).mean()  # faster than slicing in Python
         else:
             values = [np.nanmean(x.iloc[max(idx - w.w + 1, 0): idx + 1]) for idx in range(0, len(x))]
     return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
 
@@ -337,15 +338,15 @@
 
     :func:`mean` :func:`mode`
     """
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
         values = rolling_offset(x, w.w, np.nanmedian, 'median') if isinstance(x, pd.Series) else [
-            x.loc[(x.index > idx - w.w) & (x.index <= idx)].median() for idx in x.index]
+            x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].median() for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).median(), w)
 
 
 @plot_function
 def mode(x: pd.Series, w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -377,15 +378,15 @@
 
     :func:`mean` :func:`median`
     """
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
         values = rolling_apply(x, w.w, lambda a: stats.mode(a).mode[0]) if isinstance(x, pd.Series) else [
-            stats.mode(x.loc[(x.index > idx - w.w) & (x.index <= idx)]).mode[0] for idx in x.index]
+            stats.mode(x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)]).mode[0] for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).apply(lambda y: stats.mode(y).mode, raw=True), w)
 
 
 @plot_function
 def sum_(x: Union[pd.Series, List[pd.Series]], w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -472,15 +473,15 @@
 
     :func:`sum_`
     """
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing
     if isinstance(w.w, pd.DateOffset):
         values = rolling_offset(x, w.w, np.nanprod, 'prod') if isinstance(x, pd.Series) else [
-            x.loc[(x.index > idx - w.w) & (x.index <= idx)].prod() for idx in x.index]
+            x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].prod() for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).agg(pd.Series.prod), w)
 
 
 @plot_function
 def std(x: pd.Series, w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -612,15 +613,15 @@
     :func:`var` :func:`mean` :func:`std`
 
     """
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
         values = rolling_offset(x, w.w, lambda a: np.nanvar(a, ddof=1), 'var') if isinstance(x, pd.Series) else [
-            x.loc[(x.index > idx - w.w) & (x.index <= idx)].var() for idx in x.index]
+            x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].var() for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).var(), w)
 
 
 @plot_function
 def cov(x: pd.Series, y: pd.Series, w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -660,15 +661,15 @@
     **See also**
 
     :func:`sum` :func:`mean` :func:`var`
     """
     w = normalize_window(x, w)
     assert x.index.is_monotonic_increasing, "series index is monotonic increasing"
     if isinstance(w.w, pd.DateOffset):
-        values = [x.loc[(x.index > idx - w.w) & (x.index <= idx)].cov(y) for idx in x.index]
+        values = [x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].cov(y) for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).cov(y), w)
 
 
 def _zscore(x):
     if x.size == 1:
@@ -726,15 +727,15 @@
             return pd.Series([0.0], index=x.index, dtype=np.dtype(float))
 
         clean_series = x.dropna()
         zscore_series = pd.Series(stats.zscore(clean_series, ddof=1), clean_series.index, dtype=np.dtype(float))
         return interpolate(zscore_series, x, Interpolate.NAN)
     if not isinstance(w.w, int):
         w = normalize_window(x, w)
-        values = [_zscore(x.loc[(x.index > idx - w.w) & (x.index <= idx)]) for idx in x.index]
+        values = [_zscore(x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)]) for idx in x.index]
         return apply_ramp(pd.Series(values, index=x.index, dtype=np.dtype(float)), w)
     else:
         return apply_ramp(x.rolling(w.w, 0).apply(_zscore, raw=False), w)
 
 
 @plot_function
 def winsorize(x: pd.Series, limit: float = 2.5, w: Union[Window, int, str] = Window(None, 0)) -> pd.Series:
@@ -896,19 +897,20 @@
         raise ValueError('Ramp value must be less than the length of the series y.')
 
     if isinstance(w.w, int) and w.w > len(x):
         return pd.Series(dtype=float)
 
     res = pd.Series(dtype=np.dtype(float))
     for idx, val in y.items():
-        sample = x.loc[(x.index > idx - w.w) & (x.index <= idx)] if isinstance(w.w, pd.DateOffset) else x[:idx][-w.w:]
+        sample = x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)] if isinstance(w.w, pd.DateOffset) \
+            else x[:idx][-w.w:]
         res.loc[idx] = percentileofscore(sample, val, kind='mean')
 
     if isinstance(w.r, pd.DateOffset):
-        return res.loc[res.index[0] + w.r:]
+        return res.loc[(res.index[0] + w.r).date():]
     else:
         return res[w.r:]
 
 
 @plot_function
 def percentile(x: pd.Series, n: float, w: Union[Window, int, str] = None) -> Union[pd.Series, float]:
     """
@@ -941,15 +943,18 @@
     if w is None:
         return numpy.percentile(x.values, n)
 
     n /= 100
     w = normalize_window(x, w)
     if isinstance(w.w, pd.DateOffset):
         try:
-            values = [x.loc[(x.index > idx - w.w) & (x.index <= idx)].quantile(n) for idx in x.index]
+            if isinstance(x.index, pd.DatetimeIndex):
+                values = [x.loc[(x.index > (idx - w.w)) & (x.index <= idx)].quantile(n) for idx in x.index]
+            else:
+                values = [x.loc[(x.index > (idx - w.w).date()) & (x.index <= idx)].quantile(n) for idx in x.index]
         except TypeError:
             raise MqTypeError(f'cannot use relative dates with index {x.index}')
         res = pd.Series(values, index=x.index, dtype=np.dtype(float))
     else:
         res = x.rolling(w.w, 0).quantile(n)
     return apply_ramp(res, w)
 
@@ -983,15 +988,15 @@
         if not isinstance(fit_intercept, bool):
             raise MqTypeError('expected a boolean value for "fit_intercept"')
 
         df = pd.concat(X, axis=1) if isinstance(X, list) else X.to_frame()
         df = sm.add_constant(df) if fit_intercept else df
         df.columns = range(len(df.columns)) if fit_intercept else range(1, len(df.columns) + 1)
 
-        df = df[~df.isin([np.nan, np.inf, -np.inf]).any(1)]  # filter out nan and inf
+        df = df[~df.isin([np.nan, np.inf, -np.inf]).any(axis=1)]  # filter out nan and inf
         y = y[~y.isin([np.nan, np.inf, -np.inf])]
         df_aligned, y_aligned = df.align(y, 'inner', axis=0)  # align series
 
         self._index_scope = range(0, len(df.columns)) if fit_intercept else range(1, len(df.columns) + 1)
         self._res = sm.OLS(y_aligned, df_aligned).fit()
         self._fit_intercept = fit_intercept
 
@@ -1080,15 +1085,15 @@
         df = pd.concat(X, axis=1) if isinstance(X, list) else X.to_frame()
         df = sm.add_constant(df) if fit_intercept else df
         df.columns = range(len(df.columns)) if fit_intercept else range(1, len(df.columns) + 1)
 
         if w <= len(df.columns):
             raise MqValueError('Window length must be larger than the number of explanatory variables')
 
-        df = df[~df.isin([np.nan, np.inf, -np.inf]).any(1)]  # filter out nan and inf
+        df = df[~df.isin([np.nan, np.inf, -np.inf]).any(axis=1)]  # filter out nan and inf
         y = y[~y.isin([np.nan, np.inf, -np.inf])]
         df_aligned, y_aligned = df.align(y, 'inner', axis=0)  # align series
 
         self._X = df_aligned.copy()
         self._res = RollingOLS(y_aligned, df_aligned, w).fit()
 
     @plot_method
```

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/tca.py` & `gs_quant-1.0.0/gs_quant/timeseries/tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/timeseries/technicals.py` & `gs_quant-1.0.0/gs_quant/timeseries/technicals.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     smoothed_moving_averages = x.copy()
     smoothed_moving_averages *= 0
     smoothed_moving_averages[0] = initial_moving_average
     for i in range(1, len(x)):
         if isinstance(window_size, int):
             window_num_elem = window_size
         else:
-            window_num_elem = len(x[(x.index > (x.index[i] - window_size)) & (x.index <= x.index[i])])
+            window_num_elem = len(x[(x.index > (x.index[i] - window_size).date()) & (x.index <= x.index[i])])
         smoothed_moving_averages[i] = ((window_num_elem - 1) * smoothed_moving_averages[i - 1] + x[i]) / window_num_elem
     return smoothed_moving_averages
 
 
 @plot_function
 def relative_strength_index(x: pd.Series, w: Union[Window, int, str] = 14) -> pd.DataFrame:
     """
@@ -416,18 +416,15 @@
     'D' and frequency == Monthly --> period = 30
     'M' and frequency == Quarterly --> Period = 3
     'W' and frequency == Quarterly --> period = 13
     """
     if not isinstance(x.index, pd.DatetimeIndex):
         raise MqValueError("Series must have a pandas.DateTimeIndex.")
     pfreq = getattr(getattr(x, 'index', None), 'inferred_freq', None)
-    try:
-        period = statsmodels.tsa.seasonal.freq_to_period(pfreq)
-    except (ValueError, AttributeError):
-        period = None
+    period = None if pfreq is None else statsmodels.tsa.seasonal.freq_to_period(pfreq)
     if period in [7, None]:  # daily
         x = x.asfreq('D', method='ffill')
         if freq == Frequency.YEAR:
             return x, 365
         elif freq == Frequency.QUARTER:
             return x, 91
         elif freq == Frequency.MONTH:
```

### Comparing `gs_quant-0.9.99/gs_quant/tracing/__init__.py` & `gs_quant-1.0.0/gs_quant/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant/tracing/tracing.py` & `gs_quant-1.0.0/gs_quant/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant.egg-info/SOURCES.txt` & `gs_quant-1.0.0/gs_quant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-0.9.99/gs_quant.egg-info/requires.txt` & `gs_quant-1.0.0/gs_quant.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 backoff
 cachetools
 certifi
 dataclasses_json>=0.5.6
 deprecation
 funcsigs
 inflection
-lmfit<=1.0.2
+lmfit
 more_itertools
 msgpack
 nest-asyncio
 opentracing
-pandas<2.0.0,>1.0.0
 pydash
 python-dateutil>=2.7.0
 requests
 tqdm
 websockets
 
 [:python_version < "3.7"]
 dataclasses
+pandas<2.0.0,>1.0.0
 scipy<1.6.0,>=1.2.0
 statsmodels<=0.12.2
 typing
 
 [:python_version < "3.8"]
 scipy<1.8.0,>=1.2.0
 
 [:python_version > "3.6"]
+httpx>=0.23.3
 statsmodels>=0.13.0
 
+[:python_version > "3.7"]
+pandas>=2.0
+
 [:python_version > "3.8"]
 scipy>=1.2.0
 
 [develop]
 wheel
 sphinx
 sphinx_rtd_theme
@@ -59,10 +63,11 @@
 pytest-cov
 pytest-mock
 pytest-ordering
 testfixtures
 nbconvert
 nbformat
 jupyter_client
+pipreqs
 
 [turbo]
 quant-extensions
```

### Comparing `gs_quant-0.9.99/setup.py` & `gs_quant-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import setuptools
 import versioneer
 
 if "sdist" in sys.argv:
     reference = os.path.dirname(__file__)
     doc_dir = os.path.join(reference, "docs")
-    p = subprocess.Popen(["make", "html"], cwd=doc_dir, shell=True)
+    p = subprocess.Popen("sphinx-build -M help . _build", cwd=doc_dir, shell=True)
     p.wait(30)
     if p.returncode != 0:
         raise RuntimeError("unable to make docs")
 
     generated_dir = Path(os.path.join(doc_dir, "_build", "html", "functions"))
     generated_dir.mkdir(parents=True, exist_ok=True)
     target_dir = os.path.join(reference, "gs_quant", "docs")
@@ -49,52 +49,57 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://marquee.gs.com",
     license="http://www.apache.org/licenses/LICENSE-2.0",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
-        "asteval<0.9.24",  # temporary, until interal PyPI mirror catches up
+        "asteval<0.9.24",
         "aenum",
         "backoff",
         "cachetools",
         "certifi",
         "dataclasses;python_version<'3.7'",
         "dataclasses_json>=0.5.6",
         "deprecation",
         "funcsigs",
         "inflection",
-        "lmfit<=1.0.2",  # version 1.0.3 requires a newer version of pip (21.3 works, but 18.1 doesn't)
+        "lmfit",
         "more_itertools",
         "msgpack",
         "nest-asyncio",
         "opentracing",
-        "pandas>1.0.0,<2.0.0",
+        "pandas>1.0.0,<2.0.0;python_version<'3.7'",
+        "pandas>=2.0;python_version>'3.7'",
         "pydash",
         "python-dateutil>=2.7.0",
         "requests",
+        "httpx>=0.23.3;python_version>'3.6'",
         "scipy>=1.2.0;python_version>'3.8'",
         "scipy>=1.2.0,<1.6.0;python_version<'3.7'",
         "scipy>=1.2.0,<1.8.0;python_version<'3.8'",
         "statsmodels<=0.12.2;python_version<'3.7'",
         "statsmodels>=0.13.0;python_version>'3.6'",
         "tqdm",
         "typing;python_version<'3.7'",
         "websockets"
     ],
     extras_require={
         "internal": ["gs_quant_internal>=1.4.9"],
         "turbo": ["quant-extensions"],
         "notebook": ["jupyter", "matplotlib", "seaborn", "treelib"],
         "test": ["pytest", "pytest-cov", "pytest-mock", "pytest-ordering", "testfixtures", "nbconvert", "nbformat",
-                 "jupyter_client"],
+                 "jupyter_client", "pipreqs"],
         "develop": ["wheel", "sphinx", "sphinx_rtd_theme", "sphinx_autodoc_typehints", "pytest", "pytest-cov",
                     "pytest-mock", "pytest-ordering", "testfixtures"]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License"
     ],
 )
```

### Comparing `gs_quant-0.9.99/versioneer.py` & `gs_quant-1.0.0/versioneer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 
-# Version: 0.18
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +187,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,36 +275,62 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable, Dict
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -317,128 +357,144 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Callable, Dict
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -468,84 +524,89 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
@@ -554,75 +615,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -630,52 +699,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -684,15 +793,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -709,21 +818,22 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
@@ -753,27 +863,75 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -796,20 +954,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -872,18 +1059,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -911,15 +1102,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -946,75 +1137,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1022,52 +1221,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.exe", "I:\sw\gs\git-1.16\dist\win\cmd\git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1076,15 +1315,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1101,91 +1340,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.exe", "I:\sw\gs\git-1.16\dist\win\cmd\git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1199,15 +1438,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1254,27 +1493,75 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -1297,20 +1584,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1373,18 +1689,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1476,35 +1796,39 @@
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1519,50 +1843,89 @@
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
@@ -1589,17 +1952,17 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1615,19 +1978,56 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -1683,29 +2083,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
 def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1721,62 +2126,36 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -1809,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

