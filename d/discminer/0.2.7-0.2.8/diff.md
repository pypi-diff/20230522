# Comparing `tmp/discminer-0.2.7.tar.gz` & `tmp/discminer-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.7.tar", last modified: Fri May 19 10:09:33 2023, max compression
+gzip compressed data, was "discminer-0.2.8.tar", last modified: Mon May 22 09:05:24 2023, max compression
```

## Comparing `discminer-0.2.7.tar` & `discminer-0.2.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.255324 discminer-0.2.7/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.7/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-19 10:09:33.255594 discminer-0.2.7/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.7/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.222289 discminer-0.2.7/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5155 2023-05-05 18:15:57.000000 discminer-0.2.7/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    11031 2023-05-17 20:12:58.000000 discminer-0.2.7/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1248 2023-05-05 08:45:28.000000 discminer-0.2.7/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3346 2023-05-08 15:34:54.000000 discminer-0.2.7/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     3565 2023-05-18 10:58:10.000000 discminer-0.2.7/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4445 2023-05-08 15:33:38.000000 discminer-0.2.7/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4305 2023-05-08 15:25:01.000000 discminer-0.2.7/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6604 2023-05-17 21:21:31.000000 discminer-0.2.7/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    12138 2023-05-16 12:46:47.000000 discminer-0.2.7/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5693 2023-05-10 12:27:07.000000 discminer-0.2.7/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     5072 2023-05-14 22:11:49.000000 discminer-0.2.7/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    14004 2023-05-12 15:45:13.000000 discminer-0.2.7/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.235396 discminer-0.2.7/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.7/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-19 10:08:56.000000 discminer-0.2.7/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.7/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.7/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.7/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.7/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.7/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.7/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.244412 discminer-0.2.7/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.7/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.7/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.7/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12955 2023-05-17 22:25:10.000000 discminer-0.2.7/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    35724 2023-05-14 22:07:59.000000 discminer-0.2.7/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    36001 2023-05-19 10:08:32.000000 discminer-0.2.7/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.7/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.246474 discminer-0.2.7/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.7/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.7/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.7/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.7/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.237446 discminer-0.2.7/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-19 10:09:33.000000 discminer-0.2.7/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.7/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-19 10:09:33.256176 discminer-0.2.7/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.7/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-19 10:09:33.254451 discminer-0.2.7/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.7/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.7/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.7/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.7/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.386105 discminer-0.2.8/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.8/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-22 09:05:24.386365 discminer-0.2.8/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.8/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.360969 discminer-0.2.8/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5155 2023-05-05 18:15:57.000000 discminer-0.2.8/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    11031 2023-05-17 20:12:58.000000 discminer-0.2.8/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1248 2023-05-05 08:45:28.000000 discminer-0.2.8/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3346 2023-05-08 15:34:54.000000 discminer-0.2.8/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     3565 2023-05-18 10:58:10.000000 discminer-0.2.8/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4445 2023-05-08 15:33:38.000000 discminer-0.2.8/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4305 2023-05-08 15:25:01.000000 discminer-0.2.8/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6604 2023-05-17 21:21:31.000000 discminer-0.2.8/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    12138 2023-05-16 12:46:47.000000 discminer-0.2.8/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5693 2023-05-10 12:27:07.000000 discminer-0.2.8/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2023-05-14 22:11:49.000000 discminer-0.2.8/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    14004 2023-05-12 15:45:13.000000 discminer-0.2.8/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.372555 discminer-0.2.8/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.8/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-22 09:04:11.000000 discminer-0.2.8/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.8/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.8/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.8/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.8/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.8/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.8/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.379591 discminer-0.2.8/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.8/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.8/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.8/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.8/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.8/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.8/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.8/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12955 2023-05-17 22:25:10.000000 discminer-0.2.8/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    35724 2023-05-14 22:07:59.000000 discminer-0.2.8/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    36967 2023-05-22 08:30:55.000000 discminer-0.2.8/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.8/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.381416 discminer-0.2.8/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.8/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.8/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.8/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.8/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.373952 discminer-0.2.8/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-22 09:05:24.000000 discminer-0.2.8/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-22 09:05:24.000000 discminer-0.2.8/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-22 09:05:24.000000 discminer-0.2.8/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-22 09:05:24.000000 discminer-0.2.8/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-22 09:05:24.000000 discminer-0.2.8/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.8/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-22 09:05:24.386949 discminer-0.2.8/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.8/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-22 09:05:24.385207 discminer-0.2.8/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.8/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.8/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.8/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.8/template/prepare_data.py
```

### Comparing `discminer-0.2.7/LICENSE` & `discminer-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/PKG-INFO` & `discminer-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.7 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.8 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.7/README.md` & `discminer-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/make_channels.py` & `discminer-0.2.8/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/make_parfile.py` & `discminer-0.2.8/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/make_single_moments.py` & `discminer-0.2.8/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_attributes_model.py` & `discminer-0.2.8/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.8/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_moment+offset.py` & `discminer-0.2.8/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_moment+residuals.py` & `discminer-0.2.8/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_peak_residuals.py` & `discminer-0.2.8/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_radial_profiles.py` & `discminer-0.2.8/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_residuals+all.py` & `discminer-0.2.8/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/plot_residuals+deproj.py` & `discminer-0.2.8/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/_mining/utils.py` & `discminer-0.2.8/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/cart.py` & `discminer-0.2.8/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/core.py` & `discminer-0.2.8/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/cube.py` & `discminer-0.2.8/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/disc2d.py` & `discminer-0.2.8/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/grid.py` & `discminer-0.2.8/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_box.png` & `discminer-0.2.8/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_cursor.jpeg` & `discminer-0.2.8/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_path.png` & `discminer-0.2.8/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_return.png` & `discminer-0.2.8/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_surface.png` & `discminer-0.2.8/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/icons/button_trash.jpg` & `discminer-0.2.8/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/pick.py` & `discminer-0.2.8/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/plottools.py` & `discminer-0.2.8/discminer/plottools.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/rail.py` & `discminer-0.2.8/discminer/rail.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,49 +67,15 @@
             self.coord_levels = coord_levels
 
         self._lev_list = None
         self._coord_list = None
         self._resid_list = None
         self._color_list = None
 
-    def make_filaments(self, surface='upper', **kwargs):
-        #FIND FILAMENTS
-        #adapt_thresh is the width of the element used for the adaptive thresholding mask.
-        # This is primarily the step that picks out the filamentary structure. The element size should be similar to the width of the expected filamentary structure
-
-        from fil_finder import FilFinder2D
-
-        kw_fil_mask = dict(
-            verbose=False,
-            border_masking=False,
-            adapt_thresh=self.beam_size,
-            smooth_size=0.2*self.beam_size,
-            size_thresh=500*u.pix**2,
-            fill_hole_size=0.01*u.arcsec**2
-        )
-        kw_fil_mask.update(kwargs)
-        
-        Rgrid = self.R_nonan[surface]        
-        R_min_m=self.Rmin.to('m').value
-        ang_scale = np.abs(self.header['CDELT1'])*u.Unit(self.header['CUNIT1']) #pix size
-                       
-        Rind = (Rgrid>R_min_m) #& (Rgrid<R_max)
-        fil_pos = FilFinder2D(np.where(Rind & (self.prop>0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
-        fil_pos.preprocess_image(skip_flatten=True) 
-        fil_pos.create_mask(**kw_fil_mask)
-        fil_pos.medskel(verbose=False)
-        
-        fil_neg = FilFinder2D(np.where(Rind & (self.prop<0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
-        fil_neg.preprocess_image(skip_flatten=True) 
-        fil_neg.create_mask(**kw_fil_mask)
-        fil_neg.medskel(verbose=False)
-        
-        fil_pos.analyze_skeletons(prune_criteria='length')
-        fil_neg.analyze_skeletons(prune_criteria='length')
-        return fil_pos, fil_neg
+        self.model = model
         
     def prop_along_coords(self,
                           coord_ref=None,
                           surface='upper',
                           ax=None,
                           ax2=None,
                           acc_threshold=10, #0.05
@@ -311,40 +277,95 @@
         return [np.asarray(tmp, dtype=dty)
                 for tmp,dty in zip([lev_list, coord_list, resid_list, color_list],
                                    [float, object, object, object]
                 )
         ]
 
     
-    def get_average(self, surface='upper',
-                    av_func=np.nanmean, mask_ang=0, resid_thres='3sigma',
+    def get_average(self, surface='upper', 
+                    av_func=np.nanmean, mask_ang=0,
+                    sigma_thres=np.inf,
+                    mask_from_map=None, mask_perc_init=0.2, plot_diagnostics=False, tag='', forward_error=False,
                     error_func=True, error_unit=1.0, error_thres=np.inf,
                     **kwargs_along_coords):
         #mask_ang: +- angles to reject around minor axis (i.e. phi=+-90) 
-        #resid_thres: None, '3sigma', or list of thresholds with size len(lev_list)        
 
         if self._lev_list is None:
             kwargs_along_coords.update({'surface': surface})
             self.prop_along_coords(**kwargs_along_coords)
 
         lev_list, coord_list, resid_list = self._lev_list, self._coord_list, self._resid_list
         Rgrid = self.R_nonan[surface]/sfu.au
         X = self.X
         Y = self.Y
         beam_size = self.beam_size.to('au').value
         
         frac_annulus = 1.0 #if halves, 0.5; if quadrants, 0.25
         nconts = len(lev_list)
-        if resid_thres is None: resid_thres = [np.inf]*nconts #consider all values for the average
-        elif resid_thres == '3sigma': resid_thres = [3*np.nanstd(resid_list[i]) for i in range(nconts)] #anything higher than 3sigma is rejected from annulus
-        # -np.pi<coord_list<np.pi        
-        ind_accep = [(((coord_list[i]<90-mask_ang) & (coord_list[i]>-90+mask_ang)) |
-                      ((coord_list[i]>90+mask_ang) | (coord_list[i]<-90-mask_ang))) &
-                     (np.abs(resid_list[i]-np.nanmean(resid_list[i]))<resid_thres[i])
-                     for i in range(nconts)]
+
+        if mask_from_map is not None:
+            mrail = Rail(self.model, mask_from_map, lev_list)
+            _, coord_list2, resid_list2, _ = mrail.prop_along_coords(surface=surface)
+            
+            resid_thres = []
+            ind_accep = []
+            mean_list, sigma_list = [], []
+            
+            for i in range(nconts):
+                psig = int(mask_perc_init*len(resid_list2[i]))
+                isort = np.argsort(resid_list2[i])
+                sigma = np.nanstd(resid_list2[i][isort][psig:-psig])
+                mean_val = np.nanmean(resid_list2[i][isort][psig:-psig])
+                ind = np.abs(resid_list2[i]-mean_val)<sigma_thres*sigma
+                ind_accep.append(
+                    (
+                        ((coord_list[i]<90-mask_ang) & (coord_list[i]>-90+mask_ang)) |
+                        ((coord_list[i]>90+mask_ang) | (coord_list[i]<-90-mask_ang))
+                    )
+                    & ind
+                    )
+                mean_list.append(mean_val)
+                sigma_list.append(sigma)
+                
+            if plot_diagnostics:
+                fig, ax = plt.subplots(nrows=2, figsize=(12,10))                
+                ax0, ax1 = ax
+                idiag = (np.array([0.3, 0.6, 0.9])*nconts).astype(int) #ind of radii to be plotted
+
+                for i in idiag:
+                    ax0.plot(coord_list2[i], resid_list2[i], lw=2.5, alpha=0.5, label='R=%.1f'%lev_list[i])
+                    ax0.scatter(coord_list2[i][ind_accep[i]], resid_list2[i][ind_accep[i]], ec='k', fc='none', s=40, lw=1.2)
+                    ax1.plot(coord_list[i], resid_list[i], lw=2.5, alpha=0.5)
+                    ax1.scatter(coord_list[i][ind_accep[i]], resid_list[i][ind_accep[i]], ec='k', fc='none', s=40, lw=1.2)
+
+                i = idiag[0]
+                yfac = 10                
+                ax0.set_ylim(mean_list[idiag[-1]]-yfac*sigma_list[idiag[-1]], mean_list[i]+yfac*sigma_list[i])
+                mean_eval_map = np.nanmean(resid_list[i][ind_accep[i]])
+                sigma_eval_map = np.nanstd(resid_list[i][ind_accep[i]])
+                ax1.set_ylim(mean_eval_map-yfac*sigma_eval_map, mean_eval_map+yfac*sigma_eval_map)
+
+                tick_angles = np.arange(-150, 180, 30)
+                ax0.legend(frameon=False, fontsize=15)
+
+                for axi in ax:
+                    axi.set_xticks(tick_angles)
+                    axi.set_xlabel(r'Azimuth [deg]')                        
+
+                fig.savefig('diagnostics_mask_average_from_map_%s.png'%tag)
+                plt.close()
+                
+        else:
+            #anything higher than sigma_thres will be rejected from annulus
+            resid_thres = [sigma_thres*np.nanstd(resid_list[i]) for i in range(nconts)] 
+
+            ind_accep = [(((coord_list[i]<90-mask_ang) & (coord_list[i]>-90+mask_ang)) |
+                          ((coord_list[i]>90+mask_ang) | (coord_list[i]<-90-mask_ang))) &
+                         (np.abs(resid_list[i]-np.nanmean(resid_list[i]))<resid_thres[i])
+                         for i in range(nconts)]
 
         av_annulus = np.array([av_func(resid_list[i][ind_accep[i]]) for i in range(nconts)])
         
         if error_func is None: av_error = None
         else:
             beams_ring_sqrt = np.sqrt([frac_annulus*Contours.beams_along_ring(lev, Rgrid, beam_size, X, Y) for lev in lev_list])
             if callable(error_func): #if error map provided, compute average error per radius, divided by sqrt of number of beams (see Michiel Hogerheijde notes on errors)
@@ -352,15 +373,19 @@
                 for i in range(nconts):
                     x_accep, y_accep, __ = get_sky_from_disc_coords(lev_list[i], coord_list[i][ind_accep[i]]) #MISSING z, incl, PA for the function to work
                     error_accep = np.array(list(map(error_func, x_accep, y_accep))).T[0]
                     sigma2_accep = np.where((np.isfinite(error_accep)) & (error_unit*error_accep<error_thres) & (error_accep>0), (error_unit*error_accep)**2, 0)
                     Np_accep = len(coord_list[i][ind_accep[i]])
                     av_error[i] = np.sqrt(np.nansum(sigma2_accep)/Np_accep)/beams_ring_sqrt[i]  
             else: #compute standard error of mean value
-                av_error = np.array([np.std(resid_list[i][ind_accep[i]], ddof=1) for i in range(nconts)])/beams_ring_sqrt
+                if mask_from_map is not None and forward_error:
+                    resid = resid_list2
+                else:
+                    resid = resid_list
+                av_error = np.array([np.std(resid[i][ind_accep[i]], ddof=1) for i in range(nconts)])/beams_ring_sqrt
                 
         return av_annulus, av_error
 
     def make_2d_map(self, prop_thres=np.inf, return_coords=False): 
         #compute x,y coords from azimuthal contours and interpolate onto 2D grid
         n_conts = len(self._coord_list)
         R_list = np.array([np.repeat(self._lev_list[i], len(self._coord_list[i]))
@@ -377,14 +402,50 @@
         y = R*np.sin(phi)
         prop2D = griddata((x, y), prop, (self.X, self.Y), method='linear')
         
         if return_coords:
             return x, y, prop, prop2D
         else:
             return prop2D
+
+    def make_filaments(self, surface='upper', **kwargs):
+        #FIND FILAMENTS
+        #kwargs docs at https://fil-finder.readthedocs.io/en/latest/tutorial.html#masking
+
+        from fil_finder import FilFinder2D
+
+        kw_fil_mask = dict(
+            verbose=False,
+            border_masking=False,
+            adapt_thresh=self.beam_size,
+            smooth_size=0.2*self.beam_size,
+            size_thresh=500*u.pix**2,
+            fill_hole_size=0.01*u.arcsec**2
+        )
+        kw_fil_mask.update(kwargs)
+        
+        Rgrid = self.R_nonan[surface]        
+        R_min_m=self.Rmin.to('m').value
+        ang_scale = np.abs(self.header['CDELT1'])*u.Unit(self.header['CUNIT1']) #pix size
+                       
+        Rind = (Rgrid>R_min_m) #& (Rgrid<R_max)
+        fil_pos = FilFinder2D(np.where(Rind & (self.prop>0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
+        fil_pos.preprocess_image(skip_flatten=True) 
+        fil_pos.create_mask(**kw_fil_mask)
+        fil_pos.medskel(verbose=False)
+        
+        fil_neg = FilFinder2D(np.where(Rind & (self.prop<0), np.abs(self.prop), 0), ang_scale=ang_scale, distance=self.dpc)
+        fil_neg.preprocess_image(skip_flatten=True) 
+        fil_neg.create_mask(**kw_fil_mask)
+        fil_neg.medskel(verbose=False)
+        
+        fil_pos.analyze_skeletons(prune_criteria='length')
+        fil_neg.analyze_skeletons(prune_criteria='length')
+        return fil_pos, fil_neg
+
     
 class Contours(object):
     @staticmethod
     def emission_surface(ax, R, phi, extent, R_lev=None, phi_lev=None,
                          proj_offset=None, X=None, Y=None, which='both',
                          kwargs_R={}, kwargs_phi={}):
         kwargs_phif = dict(linestyles=':', linewidths=0.4, colors='k')
@@ -631,38 +692,7 @@
                                   for j in range(nzones)]
                     np_ind = [len(coord_list[i][ind[i]]) for ind in inds]
                     av_error.append([np.sqrt(np.nansum(sigma2_ind[j])/np_ind[j])/beams_zone_sqrt[i][j] for j in range(nzones) in np_ind])
             else: #compute standard error of mean value 
                 av_error = [np.array([np.std(resid_list[i][inds[j][i]], ddof=1)/beams_zone_sqrt[i][j] for i in range(nconts)]) for j in range(nzones)]
 
         return av_on_inds, av_error    
-
-    @staticmethod
-    def make_filaments(prop_2D, R_nonan_up_au, R_inner_au, beam_size_au, distance_pc, dpix_arcsec, **kwargs):
-        #FIND FILAMENTS
-        #adapt_thresh is the width of the element used for the adaptive thresholding mask.
-        # This is primarily the step that picks out the filamentary structure. The element size should be similar to the width of the expected filamentary structure
-
-        from fil_finder import FilFinder2D
-        from astropy import units as apu
-
-        distance=distance_pc*apu.pc
-        ang_scale=dpix_arcsec*apu.arcsec
-        R_min=R_inner_au
-        
-        kw_fil_mask = dict(verbose=False, adapt_thresh=1*beam_size_au*apu.au, smooth_size=0.2*beam_size_au*apu.au, size_thresh=500*apu.pix**2, border_masking=False, fill_hole_size=0.01*apu.arcsec**2)
-        kw_fil_mask.update(kwargs)
-        Rgrid = R_nonan_up_au
-        Rind = (Rgrid>R_min) #& (Rgrid<R_max)
-        fil_pos = FilFinder2D(np.where(Rind & (prop_2D>0), np.abs(prop_2D), 0), ang_scale=ang_scale, distance=distance)
-        fil_pos.preprocess_image(skip_flatten=True) 
-        fil_pos.create_mask(**kw_fil_mask)
-        fil_pos.medskel(verbose=False)
-        
-        fil_neg = FilFinder2D(np.where(Rind & (prop_2D<0), np.abs(prop_2D), 0), ang_scale=ang_scale, distance=distance)
-        fil_neg.preprocess_image(skip_flatten=True) 
-        fil_neg.create_mask(**kw_fil_mask)
-        fil_neg.medskel(verbose=False)
-        
-        fil_pos.analyze_skeletons(prune_criteria='length')
-        fil_neg.analyze_skeletons(prune_criteria='length')
-        return fil_pos, fil_neg
```

### Comparing `discminer-0.2.7/discminer/testyapf.py` & `discminer-0.2.8/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/tools/discminer.mplstyle` & `discminer-0.2.8/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/tools/fit_kernel.py` & `discminer-0.2.8/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer/tools/utils.py` & `discminer-0.2.8/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/discminer.egg-info/PKG-INFO` & `discminer-0.2.8/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.7 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.8 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.7/discminer.egg-info/SOURCES.txt` & `discminer-0.2.8/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/setup.py` & `discminer-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/template/README.rst` & `discminer-0.2.8/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/template/download_MAPS.sh` & `discminer-0.2.8/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.8/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.7/template/prepare_data.py` & `discminer-0.2.8/template/prepare_data.py`

 * *Files identical despite different names*

