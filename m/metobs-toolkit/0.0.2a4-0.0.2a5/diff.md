# Comparing `tmp/metobs_toolkit-0.0.2a4.tar.gz` & `tmp/metobs_toolkit-0.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.0.2a4.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.0.2a5.tar", max compression
```

## Comparing `metobs_toolkit-0.0.2a4.tar` & `metobs_toolkit-0.0.2a5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a4/LICENSE
--rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a4/README.md
--rw-r--r--   0        0        0      222 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/custom_template.csv
--rw-r--r--   0        0        0      485 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/custom_template_Ian.csv
--rw-r--r--   0        0        0      295 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/vlindersmall_template.csv
--rw-r--r--   0        0        0      160 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/cache/wow_template.csv
--rw-r--r--   0        0        0     1426 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/data_func.py
--rw-r--r--   0        0        0      825 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/errors.py
--rw-r--r--   0        0        0     4857 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/extra_windows.py
--rw-r--r--   0        0        0     3369 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/fig_window.ui
--rw-r--r--   0        0        0     2323 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/figuremodel.py
--rw-r--r--   0        0        0     2029 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/json_save_func.py
--rw-r--r--   0        0        0    11180 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/main.py
--rw-r--r--   0        0        0     1435 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/merge_overview.ui
--rw-r--r--   0        0        0     2367 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/pandasmodel.py
--rw-r--r--   0        0        0     2288 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/path_handler.py
--rw-r--r--   0        0        0      283 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/save_gui_vals.json
--rw-r--r--   0        0        0    46804 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/templ_build.ui
--rw-r--r--   0        0        0    11554 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/template_func.py
--rw-r--r--   0        0        0     7330 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/tlk_scripts.py
--rw-r--r--   0        0        0     2503 2023-05-17 14:40:31.641025 metobs_toolkit-0.0.2a4/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/analysis.py
--rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_datafile.csv
--rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_metadatafile.csv
--rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_templatefile.csv
--rw-r--r--   0        0        0    83222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0    18352 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/dataset_settings_updater.py
--rw-r--r--   0        0        0    13810 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    24294 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    17104 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0      222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/gui_launcher.py
--rw-r--r--   0        0        0    18380 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     9081 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a4/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     5078 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    20732 2023-05-17 14:40:15.908854 metobs_toolkit-0.0.2a4/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     3978 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    14130 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      225 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4505 2023-05-17 14:40:15.908854 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1888 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gaps_and_missing_settings.py
--rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a4/metobs_toolkit/station.py
--rw-r--r--   0        0        0     2269 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a4/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      933 2023-05-17 14:40:31.537024 metobs_toolkit-0.0.2a4/pyproject.toml
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a5/LICENSE
+-rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a5/README.md
+-rw-r--r--   0        0        0      222 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/cache/custom_template.csv
+-rw-r--r--   0        0        0      485 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/cache/custom_template_Ian.csv
+-rw-r--r--   0        0        0      295 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/cache/vlindersmall_template.csv
+-rw-r--r--   0        0        0      160 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/cache/wow_template.csv
+-rw-r--r--   0        0        0     1426 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/data_func.py
+-rw-r--r--   0        0        0      825 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/errors.py
+-rw-r--r--   0        0        0     4857 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/extra_windows.py
+-rw-r--r--   0        0        0     3369 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/fig_window.ui
+-rw-r--r--   0        0        0     2323 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/figuremodel.py
+-rw-r--r--   0        0        0     2029 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/json_save_func.py
+-rw-r--r--   0        0        0    11180 2023-05-17 14:33:54.259368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/main.py
+-rw-r--r--   0        0        0     1435 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/merge_overview.ui
+-rw-r--r--   0        0        0     2367 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/pandasmodel.py
+-rw-r--r--   0        0        0     2288 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/path_handler.py
+-rw-r--r--   0        0        0      283 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/save_gui_vals.json
+-rw-r--r--   0        0        0    46804 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/templ_build.ui
+-rw-r--r--   0        0        0    11554 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/template_func.py
+-rw-r--r--   0        0        0     7330 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/tlk_scripts.py
+-rw-r--r--   0        0        0     2503 2023-05-17 15:08:44.622521 metobs_toolkit-0.0.2a5/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a5/metobs_toolkit/analysis.py
+-rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a5/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a5/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_datafile.csv
+-rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_metadatafile.csv
+-rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_templatefile.csv
+-rw-r--r--   0        0        0    83222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0    18352 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a5/metobs_toolkit/dataset_settings_updater.py
+-rw-r--r--   0        0        0    13810 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    24294 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    17104 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a5/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0      222 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/gui_launcher.py
+-rw-r--r--   0        0        0    18380 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0     9081 2023-05-17 14:33:54.263368 metobs_toolkit-0.0.2a5/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0     5078 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a5/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    22849 2023-05-17 15:04:21.765513 metobs_toolkit-0.0.2a5/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a5/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a5/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     3978 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a5/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    14130 2023-05-17 07:20:37.243724 metobs_toolkit-0.0.2a5/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      225 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     4599 2023-05-17 15:04:21.765513 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1888 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/gaps_and_missing_settings.py
+-rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a5/metobs_toolkit/station.py
+-rw-r--r--   0        0        0     2269 2023-05-17 07:20:37.247724 metobs_toolkit-0.0.2a5/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      933 2023-05-17 15:08:44.518520 metobs_toolkit-0.0.2a5/pyproject.toml
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a5/PKG-INFO
```

### Comparing `metobs_toolkit-0.0.2a4/LICENSE` & `metobs_toolkit-0.0.2a5/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/data_func.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/data_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/errors.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/errors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/extra_windows.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/extra_windows.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/fig_window.ui` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/fig_window.ui`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/figuremodel.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/figuremodel.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/json_save_func.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/json_save_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/main.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/main.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/merge_overview.ui` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/merge_overview.ui`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/pandasmodel.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/pandasmodel.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/path_handler.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/path_handler.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/templ_build.ui` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/templ_build.ui`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/template_func.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/template_func.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/GUI/tlk_scripts.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/GUI/tlk_scripts.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/__init__.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,9 +76,9 @@
 from metobs_toolkit.dataset_settings_updater import Dataset
 
 # =============================================================================
 # Version
 # =============================================================================
 
 # DO not change this manually!
-__version__ = "0.0.2a4"
+__version__ = "0.0.2a5"
```

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/analysis.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/analysis.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/convertors.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/convertors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/data_import.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/data_import.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/db_templates.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/db_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/import_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.0.2a5/metobs_toolkit/data_templates/template_defaults/default_template.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_datafile.csv` & `metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_datafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_metadatafile.csv` & `metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_metadatafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/datafiles/demo_templatefile.csv` & `metobs_toolkit-0.0.2a5/metobs_toolkit/datafiles/demo_templatefile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/dataset.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/dataset.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/dataset_settings_updater.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/dataset_settings_updater.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/df_helpers.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/df_helpers.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/gap.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/gap.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/gap_filling.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/geometry_functions.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/landcover_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/missingobs.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/missingobs.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/modeldata.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/modeldata.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/plotting_functions.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/plotting_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,14 +238,30 @@
     ax.set_ylim(bottom=extent[1], top=extent[3])
 
     ax.set_title(title)
 
     return ax
 
 
+def sorting_function(label_vec, custom_handles, number_of_labels_types=3):
+    # TODO: clean this up? rewrite to better code?
+    sorted_vec = []            
+    # group 1, 2, 3
+    for i in range(1, number_of_labels_types+1): # loop over the type of labels
+        for l in range(len(label_vec)): #loop over the length of the label_vec
+            if label_vec[l] == i:
+                sorted_vec.append(l) 
+                # makes a vector of same size as label_vec
+                # but with the right order of permutations. 
+    sorted_handles = [custom_handles[i] for i in sorted_vec] 
+    # reordering the custom handles to put 1 at the front    
+    
+    return sorted_handles
+
+
 def timeseries_plot(
     mergedf,
     # obstype,
     title,
     xlabel,
     ylabel,
     colorby,
@@ -279,23 +295,26 @@
     fill_labels.extend(missing_fill_labels)
 
     # outlier groups
     # Catching with an else
 
 
     custom_handles = [] #add legend items to it
+    label_vec=[] # add type of label
+    
 
     if colorby == "label":
         # iterate over label groups
         col_mapper = _all_possible_labels_colormapper(settings) # get color mapper
 
         outl_groups = mergedf.groupby('label')
         legenddict = {}
         for outl_label, groupdf in outl_groups:
             outl_color = col_mapper[outl_label]
+            
 
             # plot data for the 'ok' group
             if outl_label == ok_group_label:  # ok data as lines
                 # add init_idx andf fill with nans (to avoid matplotlib interpolation)
                 fill_idx = init_idx.to_frame().drop(groupdf.index)
                 groupdf = pd.concat([groupdf, fill_idx])
                 groupdf = groupdf.drop(columns=["name", "datetime"], errors="ignore")
@@ -313,14 +332,15 @@
                     zorder=plot_settings["time_series"]["linezorder"],
                     linewidth=plot_settings["time_series"]["linewidth"],
                 )
 
                 # add legend handl
                 custom_handles.append(
                     Line2D([0], [0], color=outl_color, label="ok", lw=4))
+                label_vec.append(1)
 
 
 
             # plot filled data
             elif outl_label in  fill_labels:  # fill gaps as dashed lines
 
                 fill_idx = init_idx.to_frame().drop(groupdf.index)
@@ -345,14 +365,15 @@
                 custom_handles.append(
                     Line2D([0],[0],
                         color=outl_color,
                         label=f"filled value ({outl_label})",
                         lw=1,
                         linestyle="--",)
                     )
+                label_vec.append(2)
 
             else:  # outliers as scatters
                 plotdf = groupdf['value']
                 plotdf.index = plotdf.index.droplevel("name")
                 plotdf = plotdf.reset_index()
                 ax = plotdf.plot(
                     kind="scatter",
@@ -368,32 +389,46 @@
                 # add legend handle
                 custom_handles.append(
                     Line2D([0],[0], marker="o", color="w",
                         markerfacecolor=outl_color,
                         label=outl_label,
                         lw=1,)
                     )
+                label_vec.append(3)
             legenddict[outl_label] = outl_color
 
         # make legend
         if show_legend:
             # TODO: sort items
-            # # sort legend items
-            # sorted_handles = []
-            # # group 1, 2, 3
-            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 1])
-            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 2])
-            # sorted_handles.append([item[1] for item in custom_handles if item[0] == 3])
-            ax.legend(handles=custom_handles)
+            # sort legend items
+            custom_handles = sorting_function(label_vec, custom_handles)
+            #ax.legend(handles=custom_handles)
+            box = ax.get_position()
+            ax.set_position([box.x0, box.y0 + box.height * 0.2,
+                 box.width, box.height * 0.95])
+            ax.legend(handles=custom_handles, loc='upper center',
+                bbox_to_anchor=(0.5, -0.2),
+                fancybox=True, shadow=True,
+                ncol=plot_settings["time_series"]["legend_n_columns"])
+            
 
     elif colorby == "name":
         plotdf = mergedf.reset_index().pivot(
             index="datetime", columns="name", values='value'
         )
-        ax = plotdf.plot(kind="line", legend=show_legend, ax=ax)
+        #ax = plotdf.plot(kind="line", legend=show_legend, ax=ax)
+        ax = plotdf.plot(kind="line", legend=False, ax=ax)
+        if show_legend == True:
+            box = ax.get_position()
+            ax.set_position([box.x0, box.y0 + box.height * 0.2,
+                 box.width, box.height * 0.95])
+            ax.legend(plotdf.columns.values.tolist(), loc='upper center',
+                bbox_to_anchor=(0.5, -0.2),
+                fancybox=True, shadow=True,
+                ncol=plot_settings["time_series"]["legend_n_columns"])
 
     # Set title
     ax.set_title(title)
     # ax.legend().set_title('')
 
     # Set x and y labels
     ax.set_xlabel(xlabel)
@@ -427,28 +462,41 @@
             stations = [sta for sta in diurnaldf.columns if lcz_dict[sta] == lcz_cat]
             diurnaldf[stations].plot(ax=ax, title=title, color=colordict[lcz_cat], legend=False)
 
             # add legend item
             custom_handles.append(
                 Line2D([0], [0], color=colordict[lcz_cat], label=lcz_cat, lw=4)
             )
-
-        ax.legend(handles=custom_handles)
+            
+        box = ax.get_position()
+        ax.set_position([box.x0, box.y0 + box.height * 0.2,
+             box.width, box.height * 0.95])
+        ax.legend(handles=custom_handles, loc='upper center',
+            bbox_to_anchor=(0.5, -0.1),
+            fancybox=True, shadow=True,
+            ncol=plot_settings["legend_n_columns"])
 
 
 
 
     if colorby == 'name':
         # which colormap to use:
         if diurnaldf.shape[1] <= plot_settings['n_cat_max']:
             cmap = plot_settings['cmap_categorical']
         else:
             cmap = plot_settings['cmap_continious']
 
-        diurnaldf.plot(ax=ax, title=title, cmap=cmap)
+        diurnaldf.plot(ax=ax, title=title, legend=False, cmap=cmap)
+        box = ax.get_position()
+        ax.set_position([box.x0, box.y0 + box.height * 0.2,
+                 box.width, box.height * 0.95])
+        ax.legend(diurnaldf.columns.values.tolist(), loc='upper center',
+                bbox_to_anchor=(0.5, -0.1),
+                fancybox=True, shadow=True,
+                ncol=plot_settings["legend_n_columns"])
 
 
 
     if not errorbandsdf is None:
         # Extract colorscheme from the plot
         col_sheme = {line.get_label(): line.get_color() for line in ax.get_lines()}
```

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/printing.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/printing.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/qc_checks.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/qc_statistics.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/default_formats_settings.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/default_formats_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     # shape
     "figsize": (10, 5),
     "linewidth": 2,  #
     "linezorder": 1,  # for ok obs
     "scattersize": 4,  # for outliers
     "scatterzorder": 2,  # for outliers
     "dashedzorder": 2,  # for gapfills
+    "legend_n_columns": 5, # for the number of columns in the plot
 }
 # =============================================================================
 # Spatial plot settings
 # =============================================================================
 
 plot_settings["spatial_geo"] = {
     # projection
@@ -114,14 +115,15 @@
 plot_settings["diurnal"] = {
     "figsize": (10,10),
     'alpha_error_bands': 0.3,
     'cmap_continious' : "viridis", #if many stations are present, best to use continious rather than categorical
 
     'n_cat_max': 20, #when less or equal categories are detected, use the categorical col mapping
     'cmap_categorical': "tab20",
+    "legend_n_columns": 5,
 
 
 
 
 
 }
```

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gaps_and_missing_settings.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/gaps_and_missing_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/gee_settings.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/gee_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/qc_settings.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/qc_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.0.2a5/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/station.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/station.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.0.2a5/metobs_toolkit/writing_files.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a4/pyproject.toml` & `metobs_toolkit-0.0.2a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.0.2a4"
+version = "0.0.2a5"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
```

### Comparing `metobs_toolkit-0.0.2a4/PKG-INFO` & `metobs_toolkit-0.0.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
```

