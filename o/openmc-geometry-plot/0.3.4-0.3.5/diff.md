# Comparing `tmp/openmc_geometry_plot-0.3.4.tar.gz` & `tmp/openmc_geometry_plot-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_geometry_plot-0.3.4.tar", last modified: Sat Feb 25 21:21:00 2023, max compression
+gzip compressed data, was "openmc_geometry_plot-0.3.5.tar", last modified: Mon May 22 17:56:06 2023, max compression
```

## Comparing `openmc_geometry_plot-0.3.4.tar` & `openmc_geometry_plot-0.3.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.975839 openmc_geometry_plot-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.963839 openmc_geometry_plot-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-25 21:21:00.975839 openmc_geometry_plot-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.963839 openmc_geometry_plot-0.3.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_cylinder_box/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_cylinder_box/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_cylinder_box/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_infinite_cylinder/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_infinite_cylinder/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_infinite_cylinder/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_and_cell/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_and_cell/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_and_cell/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_with_legend/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_with_legend/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_with_legend/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.967839 openmc_geometry_plot-0.3.4/examples/csg_tokamak/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_tokamak/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/csg_tokamak/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.971840 openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/
--rw-r--r--   0 runner    (1001) docker     (123)  3808724 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/dagmc_180_tokamak.h5m
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/geometry.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 21:21:00.975839 openmc_geometry_plot-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.963839 openmc_geometry_plot-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.971840 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/
--rw-r--r--   0 runner    (1001) docker     (123)   295464 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/He4.h5
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    22155 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/cross_sections.xml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.975839 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-25 21:21:00.000000 openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:21:00.975839 openmc_geometry_plot-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/tests/test_dagmc_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/tests/test_get_slice_of_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/tests/test_get_slice_of_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    58468 2023-02-25 21:20:45.000000 openmc_geometry_plot-0.3.4/tests/two_disconnected_cubes.h5m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/examples/csg_cylinder_box/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_cylinder_box/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_cylinder_box/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/examples/csg_infinite_cylinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_infinite_cylinder/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_infinite_cylinder/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.473191 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.473191 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_and_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_and_cell/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_and_cell/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.473191 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_with_legend/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_with_legend/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_with_legend/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.473191 openmc_geometry_plot-0.3.5/examples/csg_tokamak/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_tokamak/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/csg_tokamak/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/
+-rw-r--r--   0 runner    (1001) docker     (123)  3808724 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/dagmc_180_tokamak.h5m
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/geometry.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.469191 openmc_geometry_plot-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)   295464 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/He4.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/cross_sections.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 17:56:06.000000 openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:06.477191 openmc_geometry_plot-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/tests/test_dagmc_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/tests/test_get_slice_of_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/tests/test_get_slice_of_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58468 2023-05-22 17:55:50.000000 openmc_geometry_plot-0.3.5/tests/two_disconnected_cubes.h5m
```

### Comparing `openmc_geometry_plot-0.3.4/.github/workflows/ci_with_install.yml` & `openmc_geometry_plot-0.3.5/.github/workflows/ci_with_install.yml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/.github/workflows/python-publish.yml` & `openmc_geometry_plot-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/.gitignore` & `openmc_geometry_plot-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/PKG-INFO` & `openmc_geometry_plot-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_geometry_plot
-Version: 0.3.4
+Version: 0.3.5
 Summary: Plot OpenMC geometry, interactive or static 2D slice plots.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/openmc_geometry_plot
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_geometry_plot/issues
 Keywords: openmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openmc_geometry_plot-0.3.4/README.md` & `openmc_geometry_plot-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_cylinder_box/geometry.xml` & `openmc_geometry_plot-0.3.5/examples/csg_cylinder_box/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_cylinder_box/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_cylinder_box/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_infinite_cylinder/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_infinite_cylinder/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_and_cell/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_and_cell/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_spheres_colored_by_material_with_legend/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_spheres_colored_by_material_with_legend/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_tokamak/geometry.xml` & `openmc_geometry_plot-0.3.5/examples/csg_tokamak/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/csg_tokamak/plot.py` & `openmc_geometry_plot-0.3.5/examples/csg_tokamak/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/dagmc_180_tokamak.h5m` & `openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/dagmc_180_tokamak.h5m`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/geometry.xml` & `openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/geometry.xml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/examples/dagmc_tokamak/plot.py` & `openmc_geometry_plot-0.3.5/examples/dagmc_tokamak/plot.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/pyproject.toml` & `openmc_geometry_plot-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/He4.h5` & `openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/He4.h5`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/app.py` & `openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 import plotly.graph_objects as go
 import matplotlib.pyplot as plt
 import openmc
 import streamlit as st
 from matplotlib import colors
-from pylab import cm, colormaps  # *
+from pylab import cm, colormaps
 import numpy as np
 
-# import dagmc_h5m_file_inspector as di
-
 import openmc_geometry_plot  # adds extra functions to openmc.Geometry
 
 
 def save_uploadedfile(uploadedfile):
     with open(uploadedfile.name, "wb") as f:
         f.write(uploadedfile.getbuffer())
     return st.success(f"Saved File to {uploadedfile.name}")
@@ -55,15 +53,14 @@
             🔗 This package forms part of a more [comprehensive openmc plotting](https://github.com/fusion-energy/openmc_plot) package where geometry, tallies, slices, etc can be plotted and is hosted on [xsplot.com](https://www.xsplot.com/) .
         """
     )
     st.write("<br>", unsafe_allow_html=True)
 
 
 def main():
-    header()
 
     file_label_col1, file_label_col2 = st.columns([1, 1])
     file_label_col1.write(
         """
             👉 Create your ```openmc.Geometry()``` and export the geometry xml file using ```export_to_xml()```.
 
             Not got a geometry.xml file handy, right mouse 🖱️ click and save these links 
@@ -95,15 +92,14 @@
         st.markdown(new_title, unsafe_allow_html=True)
 
         sub_title = '<center><p> Not got geometry files handy? Download an example <a href="https://raw.githubusercontent.com/fusion-energy/openmc_plot/main/examples/tokamak/geometry.xml" download>geometry.xml</a> or DAGMC h5m file</p></center>'
         st.markdown(sub_title, unsafe_allow_html=True)
 
     # DAGMC route
     elif dagmc_file is not None and geometry_xml_file is not None:
-
         save_uploadedfile(dagmc_file)
         save_uploadedfile(geometry_xml_file)
 
         bound_dag_univ = openmc.DAGMCUniverse(
             filename=dagmc_file.name
         ).bounded_universe()
         my_geometry = openmc.Geometry(root=bound_dag_univ)
@@ -121,15 +117,14 @@
         # set_cell_ids = set(di.get_volumes_from_h5m(dagmc_file.name))
         set_cell_ids = list(range(1, dag_universe.n_cells + 1))
         set_mat_names = set(dag_universe.material_names)
         all_cell_names = set_cell_ids
         set_cell_names = set(all_cell_names)
 
     elif dagmc_file is not None and geometry_xml_file is None:
-
         save_uploadedfile(dagmc_file)
 
         # make a basic openmc geometry
         bound_dag_univ = openmc.DAGMCUniverse(
             filename=dagmc_file.name
         ).bounded_universe()
         my_geometry = openmc.Geometry(root=bound_dag_univ)
@@ -148,14 +143,15 @@
         set_cell_ids = list(range(1, dag_universe.n_cells + 1))
         set_mat_names = set(dag_universe.material_names)
         all_cell_names = set_cell_ids
         set_cell_names = set(all_cell_names)
 
     # CSG route
     elif dagmc_file is None and geometry_xml_file is not None:
+
         save_uploadedfile(geometry_xml_file)
 
         tree = ET.parse(geometry_xml_file.name)
 
         root = tree.getroot()
         all_cells = root.findall("cell")
         mat_ids = []
@@ -195,38 +191,36 @@
         set_cell_ids = set(all_cell_ids)
         set_cell_names = set(all_cell_names)
 
     if my_geometry:
         print("geometry is set to something so attempting to plot")
         bb = my_geometry.bounding_box
 
-        col1, col2 = st.columns([1, 3])
-
-        view_direction = col1.selectbox(
+        view_direction = st.sidebar.selectbox(
             label="View direction",
             options=("z", "x", "y"),
             index=0,
             key="geometry_view_direction",
             help="Setting the direction of view automatically sets the horizontal and vertical axis used for the plot.",
         )
-        backend = col1.selectbox(
+        backend = st.sidebar.selectbox(
             label="Ploting backend",
             options=("matplotlib", "plotly"),
             index=0,
             key="geometry_ploting_backend",
             help="Create png images with MatPlotLib or HTML plots with Plotly",
         )
-        outline = col1.selectbox(
+        outline = st.sidebar.selectbox(
             label="Outline",
             options=("materials", "cells", None),
             index=0,
             key="outline",
             help="Allows an outline to be drawn around the cells or materials, select None for no outline",
         )
-        color_by = col1.selectbox(
+        color_by = st.sidebar.selectbox(
             label="Color by",
             options=("materials", "cells"),
             index=0,
             key="color_by",
             help="Should the plot be colored by material or by cell",
         )
         plot_left, plot_right = None, None
@@ -235,87 +229,97 @@
         y_min, y_max = None, None
 
         x_index = {"z": 0, "y": 0, "x": 1}[view_direction]
         y_index = {"z": 1, "y": 2, "x": 2}[view_direction]
         slice_index = {"z": 2, "y": 1, "x": 0}[view_direction]
 
         if np.isinf(bb[0][x_index]) or np.isinf(bb[1][x_index]):
-            x_min = col1.number_input(label="minimum vertical axis value", key="x_min")
-            x_max = col1.number_input(label="maximum vertical axis value", key="x_max")
+            x_min = st.sidebar.number_input(
+                label="minimum vertical axis value", key="x_min"
+            )
+            x_max = st.sidebar.number_input(
+                label="maximum vertical axis value", key="x_max"
+            )
         else:
             x_min = float(bb[0][x_index])
             x_max = float(bb[1][x_index])
 
         # y axis is y values
         if np.isinf(bb[0][y_index]) or np.isinf(bb[1][y_index]):
-            y_min = col1.number_input(label="minimum vertical axis value", key="y_min")
-            y_max = col1.number_input(label="maximum vertical axis value", key="y_max")
+            y_min = st.sidebar.number_input(
+                label="minimum vertical axis value", key="y_min"
+            )
+            y_max = st.sidebar.number_input(
+                label="maximum vertical axis value", key="y_max"
+            )
         else:
             y_min = float(bb[0][y_index])
             y_max = float(bb[1][y_index])
 
         # slice axis is z
         if np.isinf(bb[0][slice_index]) or np.isinf(bb[1][slice_index]):
-            slice_min = col1.number_input(label="minimum slice value", key="slice_min")
-            slice_max = col1.number_input(label="maximum slice value", key="slice_max")
+            slice_min = st.sidebar.number_input(
+                label="minimum slice value", key="slice_min"
+            )
+            slice_max = st.sidebar.number_input(
+                label="maximum slice value", key="slice_max"
+            )
         else:
             slice_min = float(bb[0][slice_index])
             slice_max = float(bb[1][slice_index])
 
         if isinstance(x_min, float) and isinstance(x_max, float):
-            plot_right, plot_left = col1.slider(
+            plot_right, plot_left = st.sidebar.slider(
                 label="Left and right values for the horizontal axis",
                 min_value=x_min,
                 max_value=x_max,
                 value=(x_min, x_max),
                 key="left_right_slider",
                 help="Set the lowest visible value and highest visible value on the horizontal axis",
             )
 
         if isinstance(y_min, float) and isinstance(y_max, float):
-            plot_bottom, plot_top = col1.slider(
+            plot_bottom, plot_top = st.sidebar.slider(
                 label="Bottom and top values for the vertical axis",
                 min_value=y_min,
                 max_value=y_max,
                 value=(y_min, y_max),
                 key="bottom_top_slider",
                 help="Set the lowest visible value and highest visible value on the vertical axis",
             )
         if isinstance(slice_min, float) and isinstance(slice_max, float):
-            slice_value = col1.slider(
+            slice_value = st.sidebar.slider(
                 label="Slice value",
                 min_value=slice_min,
                 max_value=slice_max,
                 value=(slice_min + slice_max) / 2,
                 key="slice_slider",
                 help="Set the value of the slice axis",
             )
 
-        pixels_across = col1.number_input(
+        pixels_across = st.sidebar.number_input(
             label="Number of horizontal pixels",
             value=500,
             help="Increasing this value increases the image resolution but also requires longer to create the image",
         )
 
-        selected_color_map = col1.selectbox(
+        selected_color_map = st.sidebar.selectbox(
             label="Color map", options=colormaps(), index=82
-        )  # index 81 is tab20c
+        )  # index 82 is tab20c
 
         if color_by == "materials":
-
             cmap = cm.get_cmap(selected_color_map, len(set_mat_ids))
             initial_hex_color = []
             for i in range(cmap.N):
                 rgba = cmap(i)
                 # rgb2hex accepts rgb or rgba
                 initial_hex_color.append(colors.rgb2hex(rgba))
 
             for c, id in enumerate(set_mat_ids):
-                # todo add
-                st.color_picker(
+                st.sidebar.color_picker(
                     f"Color of material with id {id}",
                     key=f"mat_{id}",
                     value=initial_hex_color[c],
                 )
 
             my_colors = {}
             for id in set_mat_ids:
@@ -330,27 +334,27 @@
                 rgba = cmap(i)
                 # rgb2hex accepts rgb or rgba
                 initial_hex_color.append(colors.rgb2hex(rgba))
 
             for c, (cell_id, cell_name) in enumerate(zip(set_cell_ids, all_cell_names)):
                 if cell_name in ["", None]:
                     cell_name = "not set"
-                st.color_picker(
+                st.sidebar.color_picker(
                     f"Color of cell id {cell_id}, cell name {cell_name}",
                     key=f"cell_{cell_id}",
                     value=initial_hex_color[c],
                 )
 
             my_colors = {0: (1, 1, 1)}  # adding entry for void cells
             for id in set_cell_ids:
                 hex_color = st.session_state[f"cell_{id}"].lstrip("#")
                 RGB = tuple(int(hex_color[i : i + 2], 16) / 255 for i in (0, 2, 4))
                 my_colors[id] = RGB
 
-        title = col1.text_input(
+        title = st.sidebar.text_input(
             "Plot title",
             help="Optionally set your own title for the plot",
             value=f"Slice through OpenMC geometry with view direction {view_direction}",
         )
 
         if (
             isinstance(plot_left, float)
@@ -409,15 +413,14 @@
                     )
                 else:
                     raise ValueError(
                         f"outline can only be cells or materials, not {outline}"
                     )
 
             if backend == "matplotlib":
-
                 extent = my_geometry.get_plot_extent(
                     plot_left,
                     plot_right,
                     plot_bottom,
                     plot_top,
                     slice_value,
                     bb,
@@ -459,26 +462,25 @@
                         linestyles="solid",
                         levels=levels,
                         linewidths=0.5,
                         extent=extent,
                     )
 
                 plt.savefig("openmc_plot_geometry_image.png")
-                col2.pyplot(plt)
-                # col2.image("openmc_plot_geometry_image.png", use_column_width="always")
+                st.pyplot(plt)
+                # st.image("openmc_plot_geometry_image.png", use_column_width="always")
 
                 with open("openmc_plot_geometry_image.png", "rb") as file:
-                    col1.download_button(
+                    st.sidebar.download_button(
                         label="Download image",
                         data=file,
                         file_name="openmc_plot_geometry_image.png",
                         mime="image/png",
                     )
             else:
-
                 data = [
                     go.Heatmap(
                         z=color_data_slice,
                         showscale=False,
                         colorscale="viridis",
                         x0=plot_left,
                         dx=abs(plot_left - plot_right) / (len(color_data_slice[0]) - 1),
@@ -494,15 +496,14 @@
                         # + ": %{x} cm<br>"
                         # + ylabel[:2].title()
                         # + ": %{y} cm<br>",
                     )
                 ]
 
                 if outline is not None:
-
                     data.append(
                         go.Contour(
                             z=outline_data_slice,
                             x0=plot_left,
                             dx=abs(plot_left - plot_right)
                             / (len(outline_data_slice[0]) - 1),
                             y0=plot_bottom,
@@ -529,30 +530,27 @@
                     scaleanchor="x",
                     scaleratio=1,
                 )
 
                 plot.write_html("openmc_plot_geometry_image.html")
 
                 with open("openmc_plot_geometry_image.html", "rb") as file:
-                    col1.download_button(
+                    st.sidebar.download_button(
                         label="Download image",
                         data=file,
                         file_name="openmc_plot_geometry_image.html",
                         mime=None,
                     )
-                col2.plotly_chart(plot, use_container_width=True)
+                st.plotly_chart(plot, use_container_width=True)
 
-            col2.write("Model info")
-            col2.write(f"Material IDS found {set_mat_ids}")
-            col2.write(f"Material names found {set_mat_names}")
-            col2.write(f"Cell IDS found {set_cell_ids}")
-            col2.write(f"Cell names found {set_cell_names}")
-            col2.write(
-                f"Bounding box lower left x={bb[0][0]} y={bb[0][1]} z={bb[0][2]}"
-            )
-            col2.write(
-                f"Bounding box upper right x={bb[1][0]} y={bb[1][1]} z={bb[1][2]}"
-            )
+            st.write("Model info")
+            st.write(f"Material IDS found {set_mat_ids}")
+            st.write(f"Material names found {set_mat_names}")
+            st.write(f"Cell IDS found {set_cell_ids}")
+            st.write(f"Cell names found {set_cell_names}")
+            st.write(f"Bounding box lower left x={bb[0][0]} y={bb[0][1]} z={bb[0][2]}")
+            st.write(f"Bounding box upper right x={bb[1][0]} y={bb[1][1]} z={bb[1][2]}")
 
 
 if __name__ == "__main__":
+    header()
     main()
```

### Comparing `openmc_geometry_plot-0.3.4/src/openmc_geometry_plot/core.py` & `openmc_geometry_plot-0.3.5/src/openmc_geometry_plot/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,23 +295,26 @@
     my_plot.colors = colors_dict
     my_plot.background = (0, 0, 0)  # void material is 0
     my_plot.color_by = "material"
     my_plot.id = 42  # the integer used to name of the plot_1.ppm file
     my_plots = openmc.Plots([my_plot])
     my_plots.export_to_xml(tmp_folder)
 
-    # TODO unset this afterwards
-    original_cross_sections = openmc.config["cross_sections"]
+    if 'cross_sections' in openmc.config.keys():
+        original_cross_sections = openmc.config["cross_sections"]
+    else:
+        original_cross_sections = None
 
     package_dir = Path(__file__).parent
     openmc.config["cross_sections"] = package_dir / "cross_sections.xml"
 
     openmc.plot_geometry(cwd=tmp_folder, output=verbose)
 
-    openmc.config["cross_sections"] = original_cross_sections
+    if original_cross_sections:
+        openmc.config["cross_sections"] = original_cross_sections
 
     if verbose:
         print(f"Temporary image and xml files written to {tmp_folder}")
 
     # load the image
     if (Path(tmp_folder) / f"plot_{my_plot.id}.ppm").is_file():
         image = Image.open(Path(tmp_folder) / f"plot_{my_plot.id}.ppm")
@@ -398,15 +401,14 @@
         mat_ids = range(1, len(mat_names) + 1)
 
         # if any of the plot_ are None then this needs calculating
         # might need to be self.bounding_box
         bb = dag_universe.bounding_box
 
     else:
-
         original_materials = self.get_all_materials()
         mat_ids = original_materials.keys()
 
         mat_names = []
         for key, value in original_materials.items():
             mat_names.append(value.name)
 
@@ -472,23 +474,27 @@
     my_plot.colors = colors_dict
     my_plot.background = (0, 0, 0)  # void material is 0
     my_plot.color_by = "cell"
     my_plot.id = 24  # the integer used to name of the plot_1.ppm file
     my_plots = openmc.Plots([my_plot])
     my_plots.export_to_xml(tmp_folder)
 
-    original_cross_sections = openmc.config["cross_sections"]
+    if 'cross_sections' in openmc.config.keys():
+        original_cross_sections = openmc.config["cross_sections"]
+    else:
+        original_cross_sections = None
 
     # TODO unset this afterwards
     package_dir = Path(__file__).parent
     openmc.config["cross_sections"] = package_dir / "cross_sections.xml"
 
     openmc.plot_geometry(cwd=tmp_folder, output=verbose)
 
-    openmc.config["cross_sections"] = original_cross_sections
+    if original_cross_sections:
+        openmc.config["cross_sections"] = original_cross_sections
 
     if verbose:
         print(f"Temporary image and xml files written to {tmp_folder}")
 
     # load the image
     if (Path(tmp_folder) / f"plot_{my_plot.id}.ppm").is_file():
         image = Image.open(Path(tmp_folder) / f"plot_{my_plot.id}.ppm")
```

### Comparing `openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/PKG-INFO` & `openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc-geometry-plot
-Version: 0.3.4
+Version: 0.3.5
 Summary: Plot OpenMC geometry, interactive or static 2D slice plots.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/openmc_geometry_plot
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_geometry_plot/issues
 Keywords: openmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openmc_geometry_plot-0.3.4/src/openmc_geometry_plot.egg-info/SOURCES.txt` & `openmc_geometry_plot-0.3.5/src/openmc_geometry_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/tests/test_dagmc_slice.py` & `openmc_geometry_plot-0.3.5/tests/test_dagmc_slice.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/tests/test_get_slice_of_cell.py` & `openmc_geometry_plot-0.3.5/tests/test_get_slice_of_cell.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/tests/test_get_slice_of_material.py` & `openmc_geometry_plot-0.3.5/tests/test_get_slice_of_material.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.3.4/tests/two_disconnected_cubes.h5m` & `openmc_geometry_plot-0.3.5/tests/two_disconnected_cubes.h5m`

 * *Files identical despite different names*

