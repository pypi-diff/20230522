# Comparing `tmp/tidy3d-2.1.1.tar.gz` & `tmp/tidy3d-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.1.1.tar", last modified: Tue Apr 25 18:27:59 2023, max compression
+gzip compressed data, was "tidy3d-2.2.0.tar", last modified: Mon May 22 17:05:06 2023, max compression
```

## Comparing `tidy3d-2.1.1.tar` & `tidy3d-2.2.0.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-25 18:27:42.000000 tidy3d-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 18:27:42.000000 tidy3d-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-25 18:27:59.092064 tidy3d-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-25 18:27:42.000000 tidy3d-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-25 18:27:42.000000 tidy3d-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:27:59.092064 tidy3d-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-25 18:27:42.000000 tidy3d-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.064063 tidy3d-2.1.1/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    49787 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.064063 tidy3d-2.1.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.068063 tidy3d-2.1.1/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.068063 tidy3d-2.1.1/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.076063 tidy3d-2.1.1/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    77646 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146851 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   115912 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-22 17:04:49.000000 tidy3d-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-22 17:04:49.000000 tidy3d-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-22 17:05:06.777744 tidy3d-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-22 17:04:49.000000 tidy3d-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-22 17:04:49.000000 tidy3d-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.757744 tidy3d-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 17:04:49.000000 tidy3d-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:05:06.777744 tidy3d-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 17:04:49.000000 tidy3d-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.757744 tidy3d-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.761744 tidy3d-2.2.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40386 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117741 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.769744 tidy3d-2.2.0/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.773744 tidy3d-2.2.0/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.777744 tidy3d-2.2.0/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-05-22 17:04:49.000000 tidy3d-2.2.0/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:05:06.765744 tidy3d-2.2.0/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 17:05:06.000000 tidy3d-2.2.0/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.1.1/LICENSE` & `tidy3d-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/PKG-INFO` & `tidy3d-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.1.1
+Version: 2.2.0
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.1.1/README.md` & `tidy3d-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/setup.py` & `tidy3d-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.2.0/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/_test_local/_test_data_performance.py` & `tidy3d-2.2.0/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/_test_local/_test_fit_web.py` & `tidy3d-2.2.0/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.2.0/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/_test_local/_test_web.py` & `tidy3d-2.2.0/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_IO.py` & `tidy3d-2.2.0/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_apodization.py` & `tidy3d-2.2.0/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_base.py` & `tidy3d-2.2.0/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_boundaries.py` & `tidy3d-2.2.0/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_custom.py` & `tidy3d-2.2.0/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_field_projection.py` & `tidy3d-2.2.0/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_geometry.py` & `tidy3d-2.2.0/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_grid.py` & `tidy3d-2.2.0/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_grid_spec.py` & `tidy3d-2.2.0/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_meshgenerate.py` & `tidy3d-2.2.0/tests/test_components/test_meshgenerate.py`

 * *Files 4% similar despite different names*

```diff
@@ -657,7 +657,65 @@
         m = GradedMesher().parse_structures(
             axis=2,
             structures=[BOX1, BOX2],
             wavelength=1.0,
             min_steps_per_wvl=6,
             dl_min=1.0,
         )
+
+
+def test_anisotropic_material_meshing():
+    """Make sure the largest propagation index defines refinement in all directions."""
+    perm_diag = [3, 2, 1]
+    cond_diag = [0.2, 0.15, 0.1]
+
+    box = td.Box(
+        center=(0, 0, 0),
+        size=(1, 2, 3),
+    )
+
+    box_iso = td.Structure(
+        geometry=box,
+        medium=td.Medium(permittivity=perm_diag[0], conductivity=cond_diag[0]),
+    )
+
+    box_diag = td.Structure(
+        geometry=box,
+        medium=td.AnisotropicMedium(
+            xx=td.Medium(permittivity=perm_diag[0], conductivity=cond_diag[0]),
+            yy=td.Medium(permittivity=perm_diag[1], conductivity=cond_diag[1]),
+            zz=td.Medium(permittivity=perm_diag[2], conductivity=cond_diag[2]),
+        ),
+    )
+
+    box_full = td.Structure(
+        geometry=box,
+        medium=td.FullyAnisotropicMedium(
+            permittivity=np.diag(perm_diag),
+            conductivity=np.diag(cond_diag),
+        ),
+    )
+
+    sim_iso = td.Simulation(
+        size=(3, 3, 6),
+        grid_spec=td.GridSpec.auto(wavelength=WAVELENGTH),
+        run_time=1e-13,
+        structures=[box_iso],
+    )
+
+    sim_diag = td.Simulation(
+        size=(3, 3, 6),
+        grid_spec=td.GridSpec.auto(wavelength=WAVELENGTH),
+        run_time=1e-13,
+        structures=[box_diag],
+    )
+
+    sim_full = td.Simulation(
+        size=(3, 3, 6),
+        grid_spec=td.GridSpec.auto(wavelength=WAVELENGTH),
+        run_time=1e-13,
+        structures=[box_full],
+    )
+
+    for dim in range(3):
+        assert np.allclose(sim_iso.grid.sizes.to_list[dim], sim_diag.grid.sizes.to_list[dim])
+        assert np.allclose(sim_iso.grid.sizes.to_list[dim], sim_full.grid.sizes.to_list[dim])
```

### Comparing `tidy3d-2.1.1/tests/test_components/test_mode.py` & `tidy3d-2.2.0/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_monitor.py` & `tidy3d-2.2.0/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_sidewall.py` & `tidy3d-2.2.0/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_simulation.py` & `tidy3d-2.2.0/tests/test_components/test_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,31 +154,41 @@
                 continue
             with pytest.raises(pydantic.ValidationError) as e_info:
                 place_box(tuple(center))
 
 
 def test_sim_size():
 
-    mesh1d = td.UniformGrid(dl=1e-6)
+    # note dl may need to change if we change the maximum allowed number of cells
+    mesh1d = td.UniformGrid(dl=2e-4)
     grid_spec = td.GridSpec(grid_x=mesh1d, grid_y=mesh1d, grid_z=mesh1d)
 
+    # check too many cells
     with pytest.raises(SetupError):
         s = td.Simulation(
             size=(1, 1, 1),
             grid_spec=grid_spec,
-            run_time=1e-12,
-            boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+            run_time=1e-13,
         )
         s._validate_size()
 
+    # should pass if symmetries applied
+    s = td.Simulation(
+        size=(1, 1, 1),
+        grid_spec=grid_spec,
+        run_time=1e-13,
+        symmetry=(1, -1, 1),
+    )
+    s._validate_size()
+
+    # check too many time steps
     with pytest.raises(pydantic.ValidationError):
         s = td.Simulation(
             size=(1, 1, 1),
             run_time=1e-7,
-            boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
         )
         s._validate_size()
 
 
 def _test_monitor_size():
 
     with pytest.raises(SetupError):
@@ -252,14 +262,59 @@
                 z=td.Boundary.bloch(bloch_vec=1.0),
             ),
             symmetry=(1, 1, 1),
             grid_spec=td.GridSpec(wavelength=1.0),
         )
 
 
+def test_validate_normalize_index():
+    src = td.UniformCurrentSource(
+        source_time=td.GaussianPulse(freq0=2.0, fwidth=1.0),
+        size=(0, 0, 0),
+        polarization="Ex",
+    )
+    src0 = td.UniformCurrentSource(
+        source_time=td.GaussianPulse(freq0=2.0, fwidth=1.0, amplitude=0),
+        size=(0, 0, 0),
+        polarization="Ex",
+    )
+
+    # negative normalize index
+    with pytest.raises(pydantic.ValidationError):
+        td.Simulation(
+            size=(1, 1, 1),
+            run_time=1e-12,
+            grid_spec=td.GridSpec.uniform(dl=0.1),
+            normalize_index=-1,
+        )
+
+    # normalize index out of bounds
+    with pytest.raises(pydantic.ValidationError):
+        td.Simulation(
+            size=(1, 1, 1),
+            run_time=1e-12,
+            grid_spec=td.GridSpec.uniform(dl=0.1),
+            sources=[src],
+            normalize_index=1,
+        )
+    # skipped if no sources
+    td.Simulation(
+        size=(1, 1, 1), run_time=1e-12, grid_spec=td.GridSpec.uniform(dl=0.1), normalize_index=1
+    )
+
+    # normalize by zero-amplitude source
+    with pytest.raises(pydantic.ValidationError):
+        td.Simulation(
+            size=(1, 1, 1),
+            run_time=1e-12,
+            grid_spec=td.GridSpec.uniform(dl=0.1),
+            sources=[src0],
+        )
+
+
 def test_validate_plane_wave_boundaries(log_capture):
     src1 = td.PlaneWave(
         source_time=td.GaussianPulse(freq0=2.5e14, fwidth=1e13),
         center=(0, 0, 0),
         size=(td.inf, td.inf, 0),
         direction="+",
         pol_angle=-1.0,
@@ -373,15 +428,15 @@
 def test_validate_components_none():
 
     assert SIM._structures_not_at_edges(val=None, values=SIM.dict()) is None
     assert SIM._validate_num_mediums(val=None) is None
     assert SIM._warn_monitor_mediums_frequency_range(val=None, values=SIM.dict()) is None
     assert SIM._warn_monitor_simulation_frequency_range(val=None, values=SIM.dict()) is None
     assert SIM._warn_grid_size_too_small(val=None, values=SIM.dict()) is None
-    assert SIM._source_homogeneous(val=None, values=SIM.dict()) is None
+    assert SIM._source_homogeneous_isotropic(val=None, values=SIM.dict()) is None
 
 
 def test_sources_edge_case_validation():
     values = SIM.dict()
     values.pop("sources")
     with pytest.raises(ValidationError):
         SIM._warn_monitor_simulation_frequency_range(val="test", values=values)
@@ -397,16 +452,24 @@
 def test_validate_size_spatial_and_time(monkeypatch):
     monkeypatch.setattr(simulation, "MAX_CELLS_TIMES_STEPS", 1)
     with pytest.raises(SetupError):
         s = SIM.copy(update=dict(run_time=1e-12))
         s._validate_size()
 
 
-def test_validate_mnt_size(monkeypatch):
-    monkeypatch.setattr(simulation, "MAX_MONITOR_DATA_SIZE_BYTES", 1)
+def test_validate_mnt_size(monkeypatch, log_capture):
+
+    # warning for monitor size
+    monkeypatch.setattr(simulation, "WARN_MONITOR_DATA_SIZE_GB", 1 / 2**30)
+    s = SIM.copy(update=dict(monitors=(td.FieldMonitor(name="f", freqs=[1], size=(1, 1, 1)),)))
+    s._validate_monitor_size()
+    assert_log_level(log_capture, "WARNING")
+
+    # error for simulation size
+    monkeypatch.setattr(simulation, "MAX_SIMULATION_DATA_SIZE_GB", 1 / 2**30)
     with pytest.raises(SetupError):
         s = SIM.copy(update=dict(monitors=(td.FieldMonitor(name="f", freqs=[1], size=(1, 1, 1)),)))
         s._validate_monitor_size()
 
 
 def test_no_monitor():
     with pytest.raises(Tidy3dKeyError):
@@ -597,14 +660,20 @@
 
 
 def test_sim_plane_wave_error():
     """ "Make sure we error if plane wave is not intersecting homogeneous region of simulation."""
 
     medium_bg = td.Medium(permittivity=2)
     medium_air = td.Medium(permittivity=1)
+    medium_bg_diag = td.AnisotropicMedium(
+        xx=td.Medium(permittivity=1),
+        yy=td.Medium(permittivity=2),
+        zz=td.Medium(permittivity=3),
+    )
+    medium_bg_full = td.FullyAnisotropicMedium(permittivity=[[4, 0.1, 0], [0.1, 2, 0], [0, 0, 3]])
 
     box = td.Structure(geometry=td.Box(size=(0.1, 0.1, 0.1)), medium=medium_air)
 
     box_transparent = td.Structure(geometry=td.Box(size=(0.1, 0.1, 0.1)), medium=medium_bg)
 
     src = td.PlaneWave(
         source_time=td.GaussianPulse(freq0=2.5e14, fwidth=1e13),
@@ -630,14 +699,31 @@
             size=(1, 1, 1),
             medium=medium_bg,
             structures=[box_transparent, box],
             sources=[src],
             boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
         )
 
+    # raise with anisotropic medium
+    with pytest.raises(pydantic.ValidationError):
+        _ = td.Simulation(
+            size=(1, 1, 1),
+            medium=medium_bg_diag,
+            sources=[src],
+            boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+        )
+
+    with pytest.raises(pydantic.ValidationError):
+        _ = td.Simulation(
+            size=(1, 1, 1),
+            medium=medium_bg_full,
+            sources=[src],
+            boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+        )
+
 
 def test_sim_monitor_homogeneous():
     """Make sure we error if a field projection monitor is not intersecting a
     homogeneous region of the simulation.
     """
 
     medium_bg = td.Medium(permittivity=2)
@@ -1302,14 +1388,33 @@
                 medium=custom_medium,
             )
         ],
     )
     with pytest.raises(SetupError) as e:
         sim.validate_pre_upload()
 
+    # TFSF box must not intersect a fully anisotropic medium
+    anisotropic_medium = td.FullyAnisotropicMedium(
+        permittivity=np.eye(3).tolist(), conductivity=np.eye(3).tolist()
+    )
+    sim = td.Simulation(
+        size=(2.0, 2.0, 2.0),
+        grid_spec=td.GridSpec.auto(wavelength=1.0),
+        run_time=1e-12,
+        sources=[source],
+        structures=[
+            td.Structure(
+                geometry=td.Box(center=(0.5, 0, 0), size=(td.inf, td.inf, 0.25)),
+                medium=anisotropic_medium,
+            )
+        ],
+    )
+    with pytest.raises(SetupError) as e:
+        sim.validate_pre_upload()
+
 
 @pytest.mark.parametrize(
     "size, num_struct, log_level", [(1, 1, None), (50, 1, "WARNING"), (1, 11000, "WARNING")]
 )
 def test_warn_large_epsilon(log_capture, size, num_struct, log_level):
     """Make sure we get a warning if the epsilon grid is too large."""
 
@@ -1468,15 +1573,15 @@
         grid_spec=td.GridSpec.uniform(dl=grid_dl),
         run_time=1e-12,
     )
 
     assert np.isclose(sim.volumetric_structures[1].medium.xx.permittivity, 2, rtol=RTOL)
 
     # test simulation.medium can't be Medium2D
-    with pytest.raises(Exception):
+    with pytest.raises(pydantic.ValidationError):
         sim = td.Simulation(
             size=(10, 10, 10),
             structures=[],
             sources=[src],
             medium=box.medium,
             boundary_spec=td.BoundarySpec(
                 x=td.Boundary.pml(num_layers=5),
@@ -1484,24 +1589,24 @@
                 z=td.Boundary.pml(num_layers=5),
             ),
             grid_spec=td.GridSpec.uniform(dl=grid_dl),
             run_time=1e-12,
         )
 
     # test 2d medium is added to 2d geometry
-    with pytest.raises(Exception):
+    with pytest.raises(pydantic.ValidationError):
         _ = td.Structure(geometry=td.Box(center=(0, 0, 0), size=(1, 1, 1)), medium=box.medium)
-    with pytest.raises(Exception):
+    with pytest.raises(pydantic.ValidationError):
         _ = td.Structure(geometry=td.Cylinder(radius=1, length=1), medium=box.medium)
-    with pytest.raises(Exception):
+    with pytest.raises(pydantic.ValidationError):
         _ = td.Structure(
             geometry=td.PolySlab(vertices=[(0, 0), (1, 0), (1, 1)], slab_bounds=(-1, 1)),
             medium=box.medium,
         )
-    with pytest.raises(Exception):
+    with pytest.raises(pydantic.ValidationError):
         _ = td.Structure(geometry=td.Sphere(radius=1), medium=box.medium)
 
 
 @pytest.mark.parametrize("normal_axis", (0, 1, 2))
 def test_pml_boxes_2D(normal_axis):
     """Ensure pml boxes have non-zero dimension for 2D sim."""
```

### Comparing `tidy3d-2.1.1/tests/test_components/test_source.py` & `tidy3d-2.2.0/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_components/test_types.py` & `tidy3d-2.2.0/tests/test_components/test_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """Tests type definitions."""
 import pytest
 import tidy3d as td
-from tidy3d.components.types import ArrayLike, Complex, constrained_array
+from tidy3d.components.types import ArrayLike, Complex, constrained_array, Tuple
 from tidy3d.components.base import Tidy3dBaseModel
 from tidy3d.exceptions import ValidationError
 import numpy as np
 
 
 def _test_validate_array_like():
     class S(Tidy3dBaseModel):
         f: ArrayLike[float, 2]
 
     s = S(f=np.array([[1.0, 2.0, 3.0], [4.0, 5.0, 6.0]]))
     with pytest.raises(pydantic.ValidationError):
         s = S(f=np.array([1.0, 2.0, 3.0]))
 
+    class MyClass(Tidy3dBaseModel):
+        f: constrained_array(ndim=3, shape=(1, 2, 3))
+
+    with pytest.raises(pydantic.ValidationError):
+        _ = MyClass(f=np.ones((2, 2, 3)))
+
+    with pytest.raises(pydantic.ValidationError):
+        _ = MyClass(f=np.ones((1, 2, 3, 4)))
+
 
 def test_schemas():
     class S(Tidy3dBaseModel):
         f: ArrayLike
         ca: constrained_array(ndim=1, dtype=complex)
         c: Complex
 
@@ -31,21 +40,23 @@
     class MyClass(Tidy3dBaseModel):
 
         a: ArrayLike = None  # can be any array-like thing
         b: constrained_array(ndim=2) = None  # must be 2D
         c: constrained_array(dtype=float) = None  # must be float-like
         d: constrained_array(ndim=1, dtype=complex) = None  # 1D complex
         e: ArrayLike
+        f: constrained_array(ndim=3, shape=(1, 2, 3)) = None  # must have certain shape
 
     my_obj = MyClass(
         a=1.0 + 2j,
         b=np.array([[1.0, 2.0]]),
         c=[1, 3.0],
         d=[1.0],
         e=[[[[1.0]]]],
+        f=np.ones((1, 2, 3)),
     )
 
     assert np.all(my_obj.a == [1.0 + 2j])  # scalars converted to list of len 1
     assert np.all(my_obj.b == [1.0, 2.0])  # numpy arrays converted tolist()
     assert np.all(my_obj.c == [1.0, 3.0])  # converted to float
     assert np.all(my_obj.d == [1.0 + 0.0j])  # converted to complex
 
@@ -53,10 +64,11 @@
 
 
 def test_hash():
     class MyClass(Tidy3dBaseModel):
 
         a: ArrayLike
         b: constrained_array(ndim=1)
+        c: Tuple[ArrayLike, ...]
 
-    c = MyClass(a=[1.0], b=[2.0, 1.0])
+    c = MyClass(a=[1.0], b=[2.0, 1.0], c=([2.0, 1.0]))
     hash(c.json())
```

### Comparing `tidy3d-2.1.1/tests/test_data/test_data_arrays.py` & `tidy3d-2.2.0/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_data/test_monitor_data.py` & `tidy3d-2.2.0/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_data/test_sim_data.py` & `tidy3d-2.2.0/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_package/test_config.py` & `tidy3d-2.2.0/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_package/test_log.py` & `tidy3d-2.2.0/tests/test_package/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     td.log.error("error test")
     td.log.critical("critical test")
     td.log.log(0, "zero test")
 
 
 def test_log_config():
     td.config.logging_level = "DEBUG"
-    td.set_logging_file("test.log")
+    td.set_logging_file("tests/tmp/test.log")
     assert len(td.log.handlers) == 2
     assert td.log.handlers["console"].level == _get_level_int("DEBUG")
     assert td.log.handlers["file"].level == _get_level_int(DEFAULT_LEVEL)
 
 
 def test_log_level_not_found():
     with pytest.raises(ValueError):
```

### Comparing `tidy3d-2.1.1/tests/test_package/test_make_script.py` & `tidy3d-2.2.0/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_package/test_material_library.py` & `tidy3d-2.2.0/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_package/test_parametric_variants.py` & `tidy3d-2.2.0/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_adjoint.py` & `tidy3d-2.2.0/tests/test_plugins/test_adjoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,201 @@
 """Tests adjoint plugin."""
 
-from typing import Callable, Tuple
+from typing import Callable, Tuple, Dict
 
 import pytest
 import pydantic
 import jax.numpy as jnp
 import numpy as np
 from jax import grad, custom_vjp
 import jax
 from numpy.random import random
+import time
+import matplotlib.pylab as plt
 
 import tidy3d as td
-from typing import Tuple, Any
+from typing import Tuple, Any, List
 
 from tidy3d.exceptions import DataError, Tidy3dKeyError, AdjointError
 from tidy3d.plugins.adjoint.components.base import JaxObject
-from tidy3d.plugins.adjoint.components.geometry import JaxBox, JaxPolySlab
+from tidy3d.plugins.adjoint.components.geometry import JaxBox, JaxPolySlab, MAX_NUM_VERTICES
 from tidy3d.plugins.adjoint.components.medium import JaxMedium, JaxAnisotropicMedium
-from tidy3d.plugins.adjoint.components.medium import JaxCustomMedium
+from tidy3d.plugins.adjoint.components.medium import JaxCustomMedium, MAX_NUM_CELLS_CUSTOM_MEDIUM
 from tidy3d.plugins.adjoint.components.structure import JaxStructure
-from tidy3d.plugins.adjoint.components.simulation import JaxSimulation
+from tidy3d.plugins.adjoint.components.simulation import JaxSimulation, JaxInfo
 from tidy3d.plugins.adjoint.components.data.sim_data import JaxSimulationData
 from tidy3d.plugins.adjoint.components.data.monitor_data import JaxModeData, JaxDiffractionData
 from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray
 from tidy3d.plugins.adjoint.components.data.dataset import JaxPermittivityDataset
 from tidy3d.plugins.adjoint.web import run, run_async
+from tidy3d.plugins.adjoint.web import run_local, run_async_local
 from tidy3d.plugins.adjoint.components.data.data_array import VALUE_FILTER_THRESHOLD
+from tidy3d.web.container import BatchData
 
-from ..utils import run_emulated, assert_log_level, log_capture, run_async_emulated
-
+from ..utils import (
+    run_emulated,
+    assert_log_level,
+    log_capture,
+    run_async_emulated,
+    SIM_DATA_PATH,
+    SIM_FULL,
+    TMP_DIR,
+)
+
+FWD_SIM_DATA_FILE = TMP_DIR + "adjoint_grad_data_fwd.hdf5"
+SIM_VJP_FILE = TMP_DIR + "adjoint_sim_vjp_file.hdf5"
+RUN_PATH = TMP_DIR + "simulation.hdf5"
 
 EPS = 2.0
 SIZE = (1.0, 2.0, 3.0)
 CENTER = (2.0, -1.0, 1.0)
 VERTICES = ((-1.0, -1.0), (0.0, 0.0), (-1.0, 0.0))
 POLYSLAB_AXIS = 2
 FREQ0 = 2e14
 BASE_EPS_VAL = 2.0
 
 # name of the output monitor used in tests
 MNT_NAME = "mode"
 
+# Emulated forward and backward run functions
+def run_emulated_fwd(
+    simulation: td.Simulation,
+    jax_info: JaxInfo,
+    task_name: str,
+    folder_name: str,
+    path: str,
+    callback_url: str,
+    verbose: bool,
+):
+    """Runs the forward simulation on our servers, stores the gradient data for later."""
+
+    # Simulation data with both original and gradient data
+    sim_data = run_emulated(
+        simulation=simulation,
+        task_name=str(task_name),
+        path=path,
+    )
+
+    # simulation data (without gradient data), written to the path file
+    sim_data_orig, sim_data_store = JaxSimulationData.split_fwd_sim_data(
+        sim_data=sim_data, jax_info=jax_info
+    )
+
+    # Test file IO
+    sim_data_orig.to_file(path)
+    sim_data_orig = td.SimulationData.from_file(path)
+
+    # gradient data stored for later use
+    jax_sim_data_store = JaxSimulationData.from_sim_data(sim_data_store, jax_info)
+    jax_sim_data_store.to_file(FWD_SIM_DATA_FILE)
+
+    task_id = "test"
+    return sim_data_orig, task_id
+
+
+def run_emulated_bwd(
+    sim_adj: td.Simulation,
+    jax_info_adj: JaxInfo,
+    fwd_task_id: str,
+    task_name: str,
+    folder_name: str,
+    callback_url: str,
+    verbose: bool,
+) -> JaxSimulation:
+    """Runs adjoint simulation on our servers, grabs the gradient data from fwd for processing."""
+
+    # Forward data
+    sim_data_fwd = JaxSimulationData.from_file(FWD_SIM_DATA_FILE)
+    grad_data_fwd = sim_data_fwd.grad_data_symmetry
+    grad_eps_data_fwd = sim_data_fwd.grad_eps_data_symmetry
+
+    # Adjoint data
+    sim_data_adj = run_emulated(
+        simulation=sim_adj,
+        task_name=str(task_name),
+        path=RUN_PATH,
+    )
+
+    jax_sim_data_adj = JaxSimulationData.from_sim_data(sim_data_adj, jax_info_adj)
+    grad_data_adj = jax_sim_data_adj.grad_data_symmetry
+
+    # get gradient and insert into the resulting simulation structure medium
+    sim_vjp = jax_sim_data_adj.simulation.store_vjp(grad_data_fwd, grad_data_adj, grad_eps_data_fwd)
+
+    # write VJP sim to and from file to emulate webapi download and loading
+    sim_vjp.to_file(SIM_VJP_FILE)
+    sim_vjp = JaxSimulation.from_file(SIM_VJP_FILE)
+
+    return sim_vjp
+
+
+# Emulated forward and backward run functions
+def run_async_emulated_fwd(
+    simulations: Tuple[td.Simulation, ...],
+    jax_infos: Tuple[JaxInfo, ...],
+    folder_name: str,
+    path_dir: str,
+    callback_url: str,
+    verbose: bool,
+) -> Tuple[BatchData, Dict[str, str]]:
+    """Runs the forward simulation on our servers, stores the gradient data for later."""
+
+    sim_datas_orig = {}
+    task_ids = []
+
+    for i, (sim, jax_info) in enumerate(zip(simulations, jax_infos)):
+        sim_data_orig, task_id = run_emulated_fwd(
+            simulation=sim,
+            jax_info=jax_info,
+            task_name=str(i),
+            folder_name=folder_name,
+            path=path_dir + str(i) + ".hdf5",
+            callback_url=callback_url,
+            verbose=verbose,
+        )
+        task_ids.append(task_id)
+        sim_datas_orig[str(i)] = sim_data_orig
+
+    return sim_datas_orig, task_ids
+
+
+def run_async_emulated_bwd(
+    simulations: Tuple[td.Simulation, ...],
+    jax_infos: Tuple[JaxInfo, ...],
+    folder_name: str,
+    path_dir: str,
+    callback_url: str,
+    verbose: bool,
+    parent_tasks: List[List[str]],
+) -> List[JaxSimulation]:
+    """Runs adjoint simulation on our servers, grabs the gradient data from fwd for processing."""
+
+    sim_vjps_orig = []
+
+    for i, (sim, jax_info, parent_tasks_i) in enumerate(zip(simulations, jax_infos, parent_tasks)):
+        sim_vjp = run_emulated_bwd(
+            sim_adj=sim,
+            jax_info_adj=jax_info,
+            fwd_task_id="test",
+            task_name=str(i),
+            folder_name=folder_name,
+            callback_url=callback_url,
+            verbose=verbose,
+        )
+        sim_vjps_orig.append(sim_vjp)
+
+    return sim_vjps_orig
+
 
 def make_sim(
     permittivity: float, size: Tuple[float, float, float], vertices: tuple, base_eps_val: float
 ) -> JaxSimulation:
     """Construt a simulation out of some input parameters."""
 
-    box = td.Box(size=(1, 1, 1), center=(1, 2, 2))
+    box = td.Box(size=(0.2, 0.2, 0.2), center=(5, 0, 2))
     med = td.Medium(permittivity=2.0)
     extraneous_structure = td.Structure(geometry=box, medium=med)
 
     # NOTE: Any new input structures should be added below as they are made
 
     # JaxBox
     jax_box1 = JaxBox(size=size, center=(1, 0, 2))
@@ -63,32 +207,33 @@
         xx=JaxMedium(permittivity=permittivity),
         yy=JaxMedium(permittivity=permittivity + 2),
         zz=JaxMedium(permittivity=permittivity * 2),
     )
     jax_struct2 = JaxStructure(geometry=jax_box2, medium=jax_med2)
 
     jax_polyslab1 = JaxPolySlab(axis=POLYSLAB_AXIS, vertices=vertices, slab_bounds=(-1, 1))
-    # jax_struct3 = JaxStructure(geometry=jax_polyslab1, medium=jax_med1)
+    jax_struct3 = JaxStructure(geometry=jax_polyslab1, medium=jax_med1)
 
     # custom medium
-    Nx, Ny, Nz = 10, 10, 1
+    Nx, Ny, Nz = 10, 1, 10
     (xmin, ymin, zmin), (xmax, ymax, zmax) = jax_box1.bounds
     coords = dict(
         x=np.linspace(xmin, xmax, Nx).tolist(),
         y=np.linspace(ymin, ymax, Ny).tolist(),
         z=np.linspace(zmin, zmax, Nz).tolist(),
         f=[FREQ0],
     )
 
+    jax_box_custom = JaxBox(size=size, center=(1, 0, 2))
     values = base_eps_val + np.random.random((Nx, Ny, Nz, 1))
     eps_ii = JaxDataArray(values=values, coords=coords)
     field_components = {f"eps_{dim}{dim}": eps_ii for dim in "xyz"}
     jax_eps_dataset = JaxPermittivityDataset(**field_components)
     jax_med_custom = JaxCustomMedium(eps_dataset=jax_eps_dataset)
-    jax_struct_custom = JaxStructure(geometry=jax_box1, medium=jax_med_custom)
+    jax_struct_custom = JaxStructure(geometry=jax_box_custom, medium=jax_med_custom)
 
     # TODO: Add new geometries as they are created.
 
     # NOTE: Any new output monitors should be added below as they are made
 
     # ModeMonitors
     output_mnt1 = td.ModeMonitor(
@@ -122,17 +267,16 @@
     sim = JaxSimulation(
         size=(10, 10, 10),
         run_time=1e-12,
         grid_spec=td.GridSpec(wavelength=1.0),
         monitors=(extraneous_field_monitor,),
         structures=(extraneous_structure,),
         output_monitors=(output_mnt1, output_mnt2),  # , output_mnt3),
-        input_structures=(jax_struct1, jax_struct2, jax_struct_custom),
+        input_structures=(jax_struct1, jax_struct2, jax_struct_custom, jax_struct3),
         boundary_spec=td.BoundarySpec.pml(x=False, y=False, z=False),
-        # input_structures=(jax_struct_custom,),
     )
 
     return sim
 
 
 def objective(amp: complex) -> float:
     """Objective function as a function of the complex amplitude."""
@@ -168,76 +312,104 @@
 
 @pytest.fixture
 def use_emulated_run(monkeypatch):
     """If this fixture is used, the `tests.utils.run_emulated` function is used for simulation."""
     import tidy3d.plugins.adjoint.web as adjoint_web
 
     monkeypatch.setattr(adjoint_web, "tidy3d_run_fn", run_emulated)
+    monkeypatch.setattr(adjoint_web, "webapi_run_adjoint_fwd", run_emulated_fwd)
+    monkeypatch.setattr(adjoint_web, "webapi_run_adjoint_bwd", run_emulated_bwd)
 
 
 @pytest.fixture
 def use_emulated_run_async(monkeypatch):
     """If this fixture is used, the `tests.utils.run_emulated` function is used for simulation."""
     import tidy3d.plugins.adjoint.web as adjoint_web
 
     monkeypatch.setattr(adjoint_web, "tidy3d_run_async_fn", run_async_emulated)
+    monkeypatch.setattr(adjoint_web, "webapi_run_async_adjoint_fwd", run_async_emulated_fwd)
+    monkeypatch.setattr(adjoint_web, "webapi_run_async_adjoint_bwd", run_async_emulated_bwd)
 
 
-def test_adjoint_pipeline(use_emulated_run):
+@pytest.mark.parametrize("local", (True, False))
+def test_adjoint_pipeline(local, use_emulated_run):
     """Test computing gradient using jax."""
 
+    run_fn = run_local if local else run
+
     sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
-    sim_data = run(sim, task_name="test")
+    sim_data = run_fn(sim, task_name="test", path=RUN_PATH)
 
     def f(permittivity, size, vertices, base_eps_val):
         sim = make_sim(
             permittivity=permittivity, size=size, vertices=vertices, base_eps_val=base_eps_val
         )
-        sim_data = run(sim, task_name="test")
+        sim_data = run_fn(sim, task_name="test", path=RUN_PATH)
         amp = extract_amp(sim_data)
         return objective(amp)
 
     grad_f = grad(f, argnums=(0, 1, 2, 3))
     df_deps, df_dsize, df_dvertices, d_eps_base = grad_f(EPS, SIZE, VERTICES, BASE_EPS_VAL)
 
     print("gradient: ", df_deps, df_dsize, df_dvertices, d_eps_base)
 
 
+@pytest.mark.parametrize("local", (True, False))
+def test_adjoint_pipeline_2d(local, use_emulated_run):
+
+    run_fn = run_local if local else run
+
+    sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+
+    sim_size_2d = list(sim.size)
+    sim_size_2d[1] = 0
+    sim = sim.updated_copy(size=sim_size_2d)
+
+    sim_data = run_fn(sim, task_name="test", path=RUN_PATH)
+
+    def f(permittivity, size, vertices, base_eps_val):
+        sim = make_sim(
+            permittivity=permittivity, size=size, vertices=vertices, base_eps_val=base_eps_val
+        )
+        sim_size_2d = list(sim.size)
+        sim_size_2d[1] = 0
+
+        sim = sim.updated_copy(size=sim_size_2d)
+
+        sim_data = run_fn(sim, task_name="test", path=RUN_PATH)
+        amp = extract_amp(sim_data)
+        return objective(amp)
+
+    grad_f = grad(f, argnums=(0, 1, 2, 3))
+    df_deps, df_dsize, df_dvertices, d_eps_base = grad_f(EPS, SIZE, VERTICES, BASE_EPS_VAL)
+
+
 def test_adjoint_setup_fwd(use_emulated_run):
     """Test that the forward pass works as expected."""
     sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
-    sim_data_orig, (sim_data_fwd,) = run.fwd(
+    sim_data_orig, (task_id_fwd) = run.fwd(
         simulation=sim,
         task_name="test",
         folder_name="default",
-        path="simulation_data.hdf5",
+        path=RUN_PATH,
         callback_url=None,
         verbose=False,
     )
-    sim_orig = sim_data_orig.simulation
-    sim_fwd = sim_data_fwd.simulation
-
-    # check the cached objects are as expected
-    assert sim_orig == sim, "original simulation wasnt cached properly"
-    assert len(sim_orig.monitors) == len(sim_data_fwd.data) == len(sim_data_orig.data)
-    assert len(sim_orig.output_monitors) == len(sim_data_fwd.output_data)
-    assert len(sim_orig.input_structures) == len(sim_data_fwd.grad_data)
-    assert len(sim_data_fwd.grad_data) == len(sim_fwd.grad_monitors)
 
 
 def _test_adjoint_setup_adj(use_emulated_run):
     """Test that the adjoint pass works as expected."""
     sim_orig = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
 
     # call forward pass
     sim_data_fwd, (sim_data_fwd,) = run.fwd(
         simulation=sim_orig,
         task_name="test",
         folder_name="default",
-        path="simulation_data.hdf5",
+        path=RUN_PATH,
         callback_url=None,
     )
 
     # create some contrived vjp sim_data to be able to call backward pass
     sim_data_vjp = sim_data_fwd.copy()
     output_data_vjp = []
     for mode_data in sim_data_vjp.output_data:
@@ -246,15 +418,15 @@
         amps_vjp = mode_data.amps.copy(update=dict(values=new_values.tolist()))
         mode_data_vjp = mode_data.copy(update=dict(amps=amps_vjp))
         output_data_vjp.append(mode_data_vjp)
     sim_data_vjp = sim_data_vjp.copy(update=dict(output_data=output_data_vjp))
     (sim_vjp,) = run.bwd(
         task_name="test",
         folder_name="default",
-        path="simulation_data.hdf5",
+        path=RUN_PATH,
         callback_url=None,
         res=(sim_data_fwd,),
         sim_data_vjp=sim_data_vjp,
     )
 
     # check the lengths of various tuples are correct
     assert len(sim_vjp.monitors) == len(sim_orig.monitors)
@@ -467,15 +639,15 @@
         da.interp(b=2.5)
 
 
 def test_jax_sim_data(use_emulated_run):
     """Test mechanics of the JaxSimulationData."""
 
     sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
-    sim_data = run(sim, task_name="test")
+    sim_data = run(sim, task_name="test", path=RUN_PATH)
 
     for i in range(len(sim.output_monitors)):
         mnt_name = MNT_NAME + str(i + 1)
         mnt_data_a = sim_data.output_data[i]
         mnt_data_b = sim_data.output_monitor_data[mnt_name]
         mnt_data_c = sim_data[mnt_name]
 
@@ -583,15 +755,18 @@
 def test_strict_types():
     """Test that things fail if you try to use just any object in a Jax component."""
     with pytest.raises(pydantic.ValidationError):
         b = JaxBox(size=(1, 1, [1, 2]), center=(0, 0, 0))
 
 
 def _test_polyslab_box(use_emulated_run):
-    """Make sure box made with polyslab gives equivalent gradients (note, doesn't pass now)."""
+    """Make sure box made with polyslab gives equivalent gradients.
+    Note: doesn't pass now since JaxBox samples the permittivity inside and outside the box,
+    and a random permittivity data is created by the emulated run function. JaxPolySlab just
+    uses the slab permittivity and the background simulation permittivity."""
 
     np.random.seed(0)
 
     def f(size, center, is_box=True):
 
         jax_med = JaxMedium(permittivity=2.0)
         POLYSLAB_AXIS = 2
@@ -608,50 +783,44 @@
             jax_struct = JaxStructure(geometry=jax_box, medium=jax_med)
 
         else:
 
             size_axis, (size_1, size_2) = JaxPolySlab.pop_axis(size, axis=POLYSLAB_AXIS)
             cent_axis, (cent_1, cent_2) = JaxPolySlab.pop_axis(center, axis=POLYSLAB_AXIS)
 
-            pos_x1 = cent_1 - size_1 / 2.0
             pos_x2 = cent_1 + size_1 / 2.0
+            pos_x1 = cent_1 - size_1 / 2.0
             pos_y1 = cent_2 - size_2 / 2.0
             pos_y2 = cent_2 + size_2 / 2.0
 
             vertices = ((pos_x1, pos_y1), (pos_x2, pos_y1), (pos_x2, pos_y2), (pos_x1, pos_y2))
             slab_bounds = (cent_axis - size_axis / 2, cent_axis + size_axis / 2)
             slab_bounds = tuple(jax.lax.stop_gradient(x) for x in slab_bounds)
             jax_polyslab = JaxPolySlab(
                 vertices=vertices, axis=POLYSLAB_AXIS, slab_bounds=slab_bounds
             )
             jax_struct = JaxStructure(geometry=jax_polyslab, medium=jax_med)
 
         # ModeMonitors
         output_mnt1 = td.ModeMonitor(
-            size=(10, 10, 0),
+            size=(td.inf, td.inf, 0),
             mode_spec=td.ModeSpec(num_modes=3),
             freqs=[2e14],
             name=MNT_NAME + "1",
         )
 
         # DiffractionMonitor
         output_mnt2 = td.DiffractionMonitor(
             center=(0, 0, 4),
             size=(td.inf, td.inf, 0),
             normal_dir="+",
             freqs=[2e14],
             name=MNT_NAME + "2",
         )
 
-        extraneous_field_monitor = td.FieldMonitor(
-            size=(10, 10, 0),
-            freqs=[1e14, 2e14],
-            name="field",
-        )
-
         sim = JaxSimulation(
             size=(10, 10, 10),
             run_time=1e-12,
             grid_spec=td.GridSpec(wavelength=1.0),
             boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
             output_monitors=(output_mnt1, output_mnt2),
             input_structures=(jax_struct,),
@@ -680,37 +849,111 @@
     gs_b, gc_b, gs_p, gc_p = map(np.array, (gs_b, gc_b, gs_p, gc_p))
 
     print("grad_size_box  = ", gs_b)
     print("grad_size_poly = ", gs_p)
     print("grad_cent_box  = ", gc_b)
     print("grad_cent_poly = ", gc_p)
 
+    print(gs_b / (gs_p + 1e-12))
+    print(gc_b / (gc_p + 1e-12))
+
     assert np.allclose(gs_b, gs_p), f"size gradients dont match, got {gs_b} and {gs_p}"
     assert np.allclose(gc_b, gc_p), f"center gradients dont match, got {gc_b} and {gc_p}"
 
 
-# @pytest.mark.asyncio
-def test_adjoint_run_async(use_emulated_run_async):
+@pytest.mark.parametrize("sim_size_axis", [0, 10])
+def test_polyslab_2d(sim_size_axis, use_emulated_run):
+    """Make sure box made with polyslab gives equivalent gradients (note, doesn't pass now)."""
+
+    np.random.seed(0)
+
+    def f(size, center):
+
+        jax_med = JaxMedium(permittivity=2.0)
+        POLYSLAB_AXIS = 2
+
+        size_axis, (size_1, size_2) = JaxPolySlab.pop_axis(size, axis=POLYSLAB_AXIS)
+        cent_axis, (cent_1, cent_2) = JaxPolySlab.pop_axis(center, axis=POLYSLAB_AXIS)
+
+        pos_x2 = cent_1 + size_1 / 2.0
+        pos_x1 = cent_1 - size_1 / 2.0
+        pos_y1 = cent_2 - size_2 / 2.0
+        pos_y2 = cent_2 + size_2 / 2.0
+
+        vertices = ((pos_x1, pos_y1), (pos_x2, pos_y1), (pos_x2, pos_y2), (pos_x1, pos_y2))
+        slab_bounds = (cent_axis - size_axis / 2, cent_axis + size_axis / 2)
+        slab_bounds = tuple(jax.lax.stop_gradient(x) for x in slab_bounds)
+        jax_polyslab = JaxPolySlab(vertices=vertices, axis=POLYSLAB_AXIS, slab_bounds=slab_bounds)
+        jax_struct = JaxStructure(geometry=jax_polyslab, medium=jax_med)
+
+        # ModeMonitors
+        output_mnt1 = td.ModeMonitor(
+            size=(td.inf, td.inf, 0),
+            mode_spec=td.ModeSpec(num_modes=3),
+            freqs=[2e14],
+            name=MNT_NAME + "1",
+        )
+
+        # DiffractionMonitor
+        output_mnt2 = td.DiffractionMonitor(
+            center=(0, 4, 0),
+            size=(td.inf, 0, td.inf),
+            normal_dir="+",
+            freqs=[2e14],
+            name=MNT_NAME + "2",
+        )
+
+        sim = JaxSimulation(
+            size=(10, 10, sim_size_axis),
+            run_time=1e-12,
+            grid_spec=td.GridSpec(wavelength=1.0),
+            boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+            output_monitors=(output_mnt1, output_mnt2),
+            input_structures=(jax_struct,),
+            sources=[
+                td.PointDipole(
+                    source_time=td.GaussianPulse(freq0=1e14, fwidth=1e14),
+                    center=(0, 0, 0),
+                    polarization="Ex",
+                )
+            ],
+        )
+
+        sim_data = run(sim, task_name="test")
+        amp = extract_amp(sim_data)
+        return objective(amp)
+
+    f_b = lambda size, center: f(size, center)
+
+    g_b = grad(f_b, argnums=(0, 1))
+
+    gs_b, gc_b = g_b((1.0, 2.0, 100.0), CENTER)
+
+
+@pytest.mark.parametrize("local", (True, False))
+def test_adjoint_run_async(local, use_emulated_run_async):
     """Test differnetiating thorugh async adjoint runs"""
 
+    run_fn = run_async_local if local else run_async
+
     def make_sim_simple(permittivity: float) -> JaxSimulation:
         """Make a sim as a function of a single parameter."""
         return make_sim(
             permittivity=permittivity, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL
         )
 
     def f(x):
         """Objective function to differentiate."""
 
         sims = []
-        for i in range(2):
-            permittivity = x + float(1.0 + i)
+        for i in range(1):
+            permittivity = x + 1.0
             sims.append(make_sim_simple(permittivity=permittivity))
 
-        sim_data_list = run_async(sims)
+        sim_data_list = run_fn(sims, path_dir=TMP_DIR)
 
         result = 0.0
         for sim_data in sim_data_list:
             amp = extract_amp(sim_data)
             result += objective(amp)
 
         return result
@@ -784,7 +1027,193 @@
     data = JaxDataArray(values=values, coords=coords)
 
     values_after, _ = data.nonzero_val_coords
 
     # assert that the terms <= VALUE_FILTER_THRESHOLD should be removed
     values_expected = np.array([1, 2 * VALUE_FILTER_THRESHOLD])
     assert np.allclose(np.array(values_after), values_expected)
+
+
+def test_jax_info_to_file():
+    """Test writing jax info to file."""
+
+    sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+    _, jax_info = sim.to_simulation()
+    jax_info.to_file("tests/tmp/jax_info.json")
+
+
+def test_split_fwd_sim_data():
+    """Test splitting of regular simulation data into user and server data."""
+
+    jax_sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+    sim, jax_info = jax_sim.to_simulation()
+    sim_data = run_emulated(sim, task_name="test", path=SIM_DATA_PATH)
+    data_user, data_adj = JaxSimulationData.split_fwd_sim_data(sim_data=sim_data, jax_info=jax_info)
+
+
+def test_save_load_simdata(use_emulated_run):
+    """Make sure a simulation data can be saved and loaded from file and retain info."""
+
+    sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+    sim_data = run(sim, task_name="test", path=RUN_PATH)
+    sim_data.to_file("tests/tmp/adjoint_simdata.hdf5")
+    sim_data2 = JaxSimulationData.from_file("tests/tmp/adjoint_simdata.hdf5")
+    assert sim_data == sim_data2
+
+
+def _test_polyslab_scale(use_emulated_run):
+    """Make sure box made with polyslab gives equivalent gradients (note, doesn't pass now)."""
+
+    nums = np.logspace(np.log10(3), 3, 13)
+    times = []
+    for num_vertices in nums:
+        num_vertices = int(num_vertices)
+
+        angles = 2 * np.pi * np.arange(num_vertices) / num_vertices
+        xs = np.cos(angles)
+        ys = np.sin(angles)
+        vertices = np.stack((xs, ys), axis=1).tolist()
+        np.random.seed(0)
+        start_time = time.time()
+
+        def f(scale=1.0):
+
+            jax_med = JaxMedium(permittivity=2.0)
+            POLYSLAB_AXIS = 2
+
+            size_axis, (size_1, size_2) = JaxPolySlab.pop_axis(SIZE, axis=POLYSLAB_AXIS)
+            cent_axis, (cent_1, cent_2) = JaxPolySlab.pop_axis(CENTER, axis=POLYSLAB_AXIS)
+
+            vertices_jax = [(scale * x, scale * y) for x, y in vertices]
+            # vertices_jax = [(x, y) for x, y in vertices]
+
+            slab_bounds = (cent_axis - size_axis / 2, cent_axis + size_axis / 2)
+            slab_bounds = tuple(jax.lax.stop_gradient(x) for x in slab_bounds)
+            jax_polyslab = JaxPolySlab(
+                vertices=vertices_jax, axis=POLYSLAB_AXIS, slab_bounds=slab_bounds
+            )
+            jax_struct = JaxStructure(geometry=jax_polyslab, medium=jax_med)
+
+            # ModeMonitors
+            output_mnt1 = td.ModeMonitor(
+                size=(td.inf, td.inf, 0),
+                mode_spec=td.ModeSpec(num_modes=3),
+                freqs=[2e14],
+                name=MNT_NAME + "1",
+            )
+
+            # DiffractionMonitor
+            output_mnt2 = td.DiffractionMonitor(
+                center=(0, 4, 0),
+                size=(td.inf, 0, td.inf),
+                normal_dir="+",
+                freqs=[2e14],
+                name=MNT_NAME + "2",
+            )
+
+            sim = JaxSimulation(
+                size=(10, 10, 10),
+                run_time=1e-12,
+                grid_spec=td.GridSpec(wavelength=1.0),
+                boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+                output_monitors=(output_mnt1, output_mnt2),
+                input_structures=(jax_struct,),
+                sources=[
+                    td.PointDipole(
+                        source_time=td.GaussianPulse(freq0=1e14, fwidth=1e14),
+                        center=(0, 0, 0),
+                        polarization="Ex",
+                    )
+                ],
+            )
+
+            sim_data = run(sim, task_name="test")
+            amp = extract_amp(sim_data)
+            return objective(amp)
+
+        g = grad(f)
+
+        g_eval = g(1.0)
+
+        total_time = time.time() - start_time
+        print(f"{num_vertices} vertices took {total_time:.2e} seconds")
+        times.append(total_time)
+
+    plt.plot(nums, times)
+    plt.xlabel("number of vertices")
+    plt.ylabel("time to compute gradient")
+    plt.xscale("log")
+    plt.yscale("log")
+    plt.show()
+
+
+def test_validate_vertices():
+    """Test the maximum number of vertices."""
+    vertices = np.random.rand(MAX_NUM_VERTICES, 2)
+    poly = JaxPolySlab(vertices=vertices, slab_bounds=(-1, 1))
+    vertices = np.random.rand(MAX_NUM_VERTICES + 1, 2)
+    with pytest.raises(pydantic.ValidationError):
+        poly = JaxPolySlab(vertices=vertices, slab_bounds=(-1, 1))
+
+
+def test_custom_medium_3D(use_emulated_run):
+    """Ensure custom medium fails if 3D pixelated grid."""
+
+    jax_box = JaxBox(size=(1, 1, 1), center=(0, 0, 0))
+
+    def make_custom_medium(Nx: int, Ny: int, Nz: int) -> JaxCustomMedium:
+
+        # custom medium
+        (xmin, ymin, zmin), (xmax, ymax, zmax) = jax_box.bounds
+        coords = dict(
+            x=np.linspace(xmin, xmax, Nx).tolist(),
+            y=np.linspace(ymin, ymax, Ny).tolist(),
+            z=np.linspace(zmin, zmax, Nz).tolist(),
+            f=[FREQ0],
+        )
+
+        values = np.random.random((Nx, Ny, Nz, 1))
+        eps_ii = JaxDataArray(values=values, coords=coords)
+        field_components = {f"eps_{dim}{dim}": eps_ii for dim in "xyz"}
+        jax_eps_dataset = JaxPermittivityDataset(**field_components)
+        return JaxCustomMedium(eps_dataset=jax_eps_dataset)
+
+    make_custom_medium(1, 1, 1)
+    make_custom_medium(10, 1, 1)
+    make_custom_medium(1, 10, 1)
+    make_custom_medium(1, 1, 10)
+    make_custom_medium(1, 10, 10)
+    make_custom_medium(10, 1, 10)
+    make_custom_medium(10, 10, 1)
+    with pytest.raises(pydantic.ValidationError):
+        make_custom_medium(10, 10, 10)
+
+
+def test_custom_medium_size(use_emulated_run):
+    """Ensure custom medium fails if too many cells provided."""
+
+    jax_box = JaxBox(size=(1, 1, 1), center=(0, 0, 0))
+
+    def make_custom_medium(num_cells: int) -> JaxCustomMedium:
+
+        Nx = num_cells
+        Ny = Nz = 1
+
+        # custom medium
+        (xmin, ymin, zmin), (xmax, ymax, zmax) = jax_box.bounds
+        coords = dict(
+            x=np.linspace(xmin, xmax, Nx).tolist(),
+            y=np.linspace(ymin, ymax, Ny).tolist(),
+            z=np.linspace(zmin, zmax, Nz).tolist(),
+            f=[FREQ0],
+        )
+
+        values = np.random.random((Nx, Ny, Nz, 1))
+        eps_ii = JaxDataArray(values=values, coords=coords)
+        field_components = {f"eps_{dim}{dim}": eps_ii for dim in "xyz"}
+        jax_eps_dataset = JaxPermittivityDataset(**field_components)
+        return JaxCustomMedium(eps_dataset=jax_eps_dataset)
+
+    make_custom_medium(num_cells=1)
+    make_custom_medium(num_cells=MAX_NUM_CELLS_CUSTOM_MEDIUM)
+    with pytest.raises(pydantic.ValidationError):
+        make_custom_medium(num_cells=MAX_NUM_CELLS_CUSTOM_MEDIUM + 1)
```

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.2.0/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.2.0/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.2.0/tests/test_plugins/test_mode_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
 def test_compute_modes():
     """Test direct call to ``compute_modes`` (used in e.g. gdsfactory)."""
     eps_cross = np.random.rand(10, 10)
     coords = np.arange(11)
     mode_spec = td.ModeSpec(num_modes=3, target_neff=2.0)
     modes = compute_modes(
-        eps_cross=[eps_cross] * 3,
+        eps_cross=[eps_cross] * 9,
         coords=[coords, coords],
         freq=td.C_0 / 1.0,
         mode_spec=mode_spec,
     )
 
 
 def test_group_index():
```

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_polyslab.py` & `tidy3d-2.2.0/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.2.0/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_plugins/test_waveguide.py` & `tidy3d-2.2.0/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_auth.py` & `tidy3d-2.2.0/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_cli.py` & `tidy3d-2.2.0/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_material_fitter.py` & `tidy3d-2.2.0/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.2.0/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.2.0/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.2.0/tests/test_web/test_tidy3d_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,24 @@
         match=[matchers.query_param_matcher({"projectName": "test folder2"})],
         json={"data": {"projectId": "1234", "projectName": "test folder2"}},
         status=200,
     )
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
-        match=[matchers.json_params_matcher({"taskName": "test task", "callbackUrl": None})],
+        match=[
+            matchers.json_params_matcher(
+                {
+                    "taskName": "test task",
+                    "call_back_url": None,
+                    "simulationType": "tidy3d",
+                    "parentTasks": None,
+                }
+            )
+        ],
         json={
             "data": {
                 "taskId": "1234",
                 "taskName": "test task",
                 "createdAt": "2022-01-01T00:00:00.000Z",
             }
         },
@@ -163,15 +172,24 @@
         match=[matchers.query_param_matcher({"projectName": "test folder1"})],
         json={"data": {"projectId": "1234", "projectName": "test folder1"}},
         status=200,
     )
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
-        match=[matchers.json_params_matcher({"taskName": "test task", "callbackUrl": None})],
+        match=[
+            matchers.json_params_matcher(
+                {
+                    "taskName": "test task",
+                    "call_back_url": None,
+                    "simulationType": "tidy3d",
+                    "parentTasks": None,
+                }
+            )
+        ],
         json={
             "data": {
                 "taskId": "1234",
                 "taskName": "test task",
                 "createdAt": "2022-01-01T00:00:00.000Z",
             }
         },
@@ -242,7 +260,20 @@
         status=200,
     )
     task = SimulationTask.get("3eb06d16-208b-487b-864b-e9b1d3e010a7")
     LOG_FNAME = "tests/tmp/test.log"
     with open(LOG_FNAME, "w") as f:
         task.get_log(LOG_FNAME)
         assert os.path.getsize(LOG_FNAME) > 0
+
+
+@responses.activate
+def test_get_running_tasks(set_api_key):
+    responses.add(
+        responses.GET,
+        f"{Env.current.web_api_endpoint}/tidy3d/py/tasks",
+        json={"data": [{"taskId": "1234", "status": "queued"}]},
+        status=200,
+    )
+
+    tasks = SimulationTask.get_running_tasks()
+    assert len(tasks) == 1
```

### Comparing `tidy3d-2.1.1/tests/test_web/test_webapi.py` & `tidy3d-2.2.0/tests/test_web/test_webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,24 @@
         json={"data": {"projectId": TASK_ID, "projectName": PROJECT_NAME}},
         status=200,
     )
 
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/{TASK_ID}/tasks",
-        match=[matchers.json_params_matcher({"taskName": TASK_NAME, "callbackUrl": None})],
+        match=[
+            matchers.json_params_matcher(
+                {
+                    "taskName": TASK_NAME,
+                    "call_back_url": None,
+                    "simulationType": "tidy3d",
+                    "parentTasks": None,
+                }
+            )
+        ],
         json={
             "data": {
                 "taskId": TASK_ID,
                 "taskName": TASK_NAME,
                 "createdAt": CREATED_AT,
             }
         },
```

### Comparing `tidy3d-2.1.1/tests/utils.py` & `tidy3d-2.2.0/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import os
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Tuple
+import pydantic as pd
 
 import pytest
 import numpy as np
 from tidy3d import *
 import tidy3d as td
 from tidy3d.log import _get_level_int
 from tidy3d.web import BatchData
-
+from tidy3d.components.base import Tidy3dBaseModel
 
 """ utilities shared between all tests """
 
 
 def clear_dir(path: str):
     """clears a dir"""
     for f in os.listdir(path):
         full_path = os.path.join(path, f)
         if not os.path.isdir(full_path):
             os.remove(full_path)
 
 
 TMP_DIR = "tests/tmp/"
+SIM_DATA_PATH = TMP_DIR + "simulation_data.hdf5"
 
 
 # decorator that clears the tmp/ directory before test
 def clear_tmp(fn):
     if not os.path.exists(TMP_DIR):
         os.mkdir(TMP_DIR)
 
@@ -307,25 +309,28 @@
                 medium=Medium(permittivity=2.0),
             )
         ],
     ),
 )
 
 
-def run_emulated(simulation: Simulation, **kwargs) -> SimulationData:
+def run_emulated(simulation: Simulation, path: str = SIM_DATA_PATH, **kwargs) -> SimulationData:
     """Emulates a simulation run."""
 
     from scipy.ndimage.filters import gaussian_filter
 
     def make_data(coords: dict, data_array_type: type, is_complex: bool = False) -> "data_type":
         """make a random DataArray out of supplied coordinates and data_type."""
         data_shape = [len(coords[k]) for k in data_array_type._dims]
+        np.random.seed(1)
         data = np.random.random(data_shape)
+
+        # data = np.ones(data_shape)
         data = (1 + 1j) * data if is_complex else data
-        data = gaussian_filter(data, sigma=0.5)  # smooth out the data a little so it isnt random
+        data = gaussian_filter(data, sigma=1.0)  # smooth out the data a little so it isnt random
         data_array = data_array_type(data, coords=coords)
         return data_array
 
     def make_field_data(monitor: FieldMonitor) -> FieldData:
         """make a random FieldData from a FieldMonitor."""
         field_cmps = {}
         coords = {}
@@ -346,15 +351,15 @@
             )
 
         return FieldData(
             monitor=monitor,
             symmetry=simulation.symmetry,
             symmetry_center=simulation.center,
             grid_expanded=simulation.discretize(monitor, extend=True),
-            **field_cmps
+            **field_cmps,
         )
 
     def make_eps_data(monitor: PermittivityMonitor) -> PermittivityData:
         """make a random PermittivityData from a PermittivityMonitor."""
         field_mnt = FieldMonitor(**monitor.dict(exclude={"type", "fields"}))
         field_data = make_field_data(monitor=field_mnt)
         return PermittivityData(
@@ -391,21 +396,58 @@
         FieldMonitor: make_field_data,
         ModeMonitor: make_mode_data,
         PermittivityMonitor: make_eps_data,
         DiffractionMonitor: make_diff_data,
     }
 
     data = [MONITOR_MAKER_MAP[type(mnt)](mnt) for mnt in simulation.monitors]
+    sim_data = SimulationData(simulation=simulation, data=data)
+    sim_data.to_file(path)
+
+    return sim_data
+
+
+class BatchDataTest(Tidy3dBaseModel):
+    """Holds a collection of :class:`.SimulationData` returned by :class:`.Batch`."""
+
+    task_paths: Dict[str, str] = pd.Field(
+        ...,
+        title="Data Paths",
+        description="Mapping of task_name to path to corresponding data for each task in batch.",
+    )
 
-    return SimulationData(simulation=simulation, data=data)
+    task_ids: Dict[str, str] = pd.Field(
+        ..., title="Task IDs", description="Mapping of task_name to task_id for each task in batch."
+    )
+
+    sim_data: Dict[str, SimulationData]
+
+    def load_sim_data(self, task_name: str) -> SimulationData:
+        """Load a :class:`.SimulationData` from file by task name."""
+        task_data_path = self.task_paths[task_name]
+        task_id = self.task_ids[task_name]
+        return self.sim_data[task_name]
+
+    def items(self) -> Tuple[str, SimulationData]:
+        """Iterate through the :class:`.SimulationData` for each task_name."""
+        for task_name in self.task_paths.keys():
+            yield task_name, self.load_sim_data(task_name)
+
+    def __getitem__(self, task_name: str) -> SimulationData:
+        """Get the :class:`.SimulationData` for a given ``task_name``."""
+        return self.load_sim_data(task_name)
 
 
 def run_async_emulated(simulations: Dict[str, Simulation], **kwargs) -> BatchData:
     """Emulate an async run function."""
-    return {task_name: run_emulated(sim) for task_name, sim in simulations.items()}
+    task_ids = {task_name: f"task_id={i}" for i, task_name in enumerate(simulations.keys())}
+    task_paths = {task_name: "NONE" for task_name in simulations.keys()}
+    sim_data = {task_name: run_emulated(sim) for task_name, sim in simulations.items()}
+
+    return BatchDataTest(task_paths=task_paths, task_ids=task_ids, sim_data=sim_data)
 
 
 # Log handler used to store log records during tests
 class CaptureHandler:
     def __init__(self):
         self.level = 0
         self.records = []
```

### Comparing `tidy3d-2.1.1/tidy3d/__init__.py` & `tidy3d-2.2.0/tidy3d/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # geometry
 from .components.geometry import Box, Sphere, Cylinder, PolySlab, GeometryGroup
 from .components.geometry import TriangleMesh
 
 # medium
 from .components.medium import Medium, PoleResidue, AnisotropicMedium, PEC, PECMedium, Medium2D
 from .components.medium import Sellmeier, Debye, Drude, Lorentz
-from .components.medium import CustomMedium
+from .components.medium import CustomMedium, FullyAnisotropicMedium
+from .components.transformation import RotationAroundAxis
 
 # structures
 from .components.structure import Structure, MeshOverrideStructure
 
 # modes
 from .components.mode import ModeSpec
```

### Comparing `tidy3d-2.1.1/tidy3d/__main__.py` & `tidy3d-2.2.0/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/apodization.py` & `tidy3d-2.2.0/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/base.py` & `tidy3d-2.2.0/tidy3d/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     """Base pydantic model that all Tidy3d components inherit from.
     Defines configuration for handling data structures
     as well as methods for imporing, exporting, and hashing tidy3d objects.
     For more details on pydantic base models, see:
     `Pydantic Models <https://pydantic-docs.helpmanual.io/usage/models/>`_
     """
 
+    def __hash__(self) -> int:
+        """Hash method."""
+        try:
+            return super().__hash__(self)
+        except TypeError:
+            return hash(self.json())
+
     def __init__(self, **kwargs):
         """Init method, includes post-init validators."""
         super().__init__(**kwargs)
         self._post_init_validators()
 
     def _post_init_validators(self) -> None:
         """Call validators taking ``self`` that get run after init, implement in subclasses."""
```

### Comparing `tidy3d-2.1.1/tidy3d/components/boundary.py` & `tidy3d-2.2.0/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/data/data_array.py` & `tidy3d-2.2.0/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/data/dataset.py` & `tidy3d-2.2.0/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/data/monitor_data.py` & `tidy3d-2.2.0/tidy3d/components/data/monitor_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         """
 
         field_components = self._grid_corrected_fields
         if self.monitor.colocate:
             return field_components
 
         # Interpolate field components to cell centers
-        interp_dict = {}
+        interp_dict = {"assume_sorted": True}
         for dim, cents in zip(self._tangential_dims, self._plane_grid_centers):
             if cents.size > 0:
                 interp_dict[dim] = cents
 
         centered_fields = {key: val.interp(**interp_dict) for key, val in field_components.items()}
 
         return centered_fields
@@ -452,15 +452,15 @@
 
         Return
         ------
             Dictionary with interpolated fields.
         """
         fields = self._tangential_fields
 
-        interp_dict = {}
+        interp_dict = {"assume_sorted": True}
         for dim, cents in zip(self._tangential_dims, centers):
             if cents.size > 0:
                 interp_dict[dim] = cents
 
         kwargs = {"bounds_error": False, "fill_value": 0.0}
         for component, field in fields.items():
             fields[component] = field.interp(kwargs=kwargs, **interp_dict)
@@ -581,15 +581,17 @@
     >>> f = [2e14, 3e14]
     >>> coords = dict(x=x, y=y, z=z, f=f)
     >>> scalar_field = ScalarFieldDataArray((1+1j) * np.random.random((2,3,4,2)), coords=coords)
     >>> monitor = FieldMonitor(size=(2,4,6), freqs=[2e14, 3e14], name='field', fields=['Ex', 'Hz'])
     >>> data = FieldData(monitor=monitor, Ex=scalar_field, Hz=scalar_field)
     """
 
-    monitor: FieldMonitor
+    monitor: FieldMonitor = pd.Field(
+        ..., title="Monitor", description="Frequency-domain field monitor associated with the data."
+    )
 
     _contains_monitor_fields = enforce_monitor_fields_present()
 
     def normalize(self, source_spectrum_fn: Callable[[float], complex]) -> FieldDataset:
         """Return copy of self after normalization is applied using source spectrum function."""
         fields_norm = {}
         for field_name, field_data in self.field_components.items():
@@ -650,15 +652,17 @@
     >>> t = [0, 1e-12, 2e-12]
     >>> coords = dict(x=x, y=y, z=z, t=t)
     >>> scalar_field = ScalarFieldTimeDataArray(np.random.random((2,3,4,3)), coords=coords)
     >>> monitor = FieldTimeMonitor(size=(2,4,6), interval=100, name='field', fields=['Ex', 'Hz'])
     >>> data = FieldTimeData(monitor=monitor, Ex=scalar_field, Hz=scalar_field)
     """
 
-    monitor: FieldTimeMonitor
+    monitor: FieldTimeMonitor = pd.Field(
+        ..., title="Monitor", description="Time-domain field monitor associated with the data."
+    )
 
     _contains_monitor_fields = enforce_monitor_fields_present()
 
     @property
     def poynting(self) -> ScalarFieldTimeDataArray:
         """Instantaneous Poynting vector for time-domain data associated to a 2D monitor, projected
         to the direction normal to the monitor plane."""
@@ -730,15 +734,17 @@
     ...     Hx=field,
     ...     Hy=field,
     ...     Hz=field,
     ...     n_complex=index_data
     ... )
     """
 
-    monitor: ModeSolverMonitor
+    monitor: ModeSolverMonitor = pd.Field(
+        ..., title="Monitor", description="Mode solver monitor associated with the data."
+    )
 
     # pylint:disable=too-many-locals
     def overlap_sort(
         self,
         track_freq: TrackFreq,
         overlap_thresh: float = 0.9,
     ) -> ModeSolverData:
@@ -952,15 +958,17 @@
     >>> f = [2e14, 3e14]
     >>> coords = dict(x=x, y=y, z=z, f=f)
     >>> sclr_fld = ScalarFieldDataArray((1+1j) * np.random.random((2,3,4,2)), coords=coords)
     >>> monitor = PermittivityMonitor(size=(2,4,6), freqs=[2e14, 3e14], name='eps')
     >>> data = PermittivityData(monitor=monitor, eps_xx=sclr_fld, eps_yy=sclr_fld, eps_zz=sclr_fld)
     """
 
-    monitor: PermittivityMonitor
+    monitor: PermittivityMonitor = pd.Field(
+        ..., title="Monitor", description="Permittivity monitor associated with the data."
+    )
 
 
 class ModeData(MonitorData):
     """Data associated with a :class:`.ModeMonitor`: modal amplitudes and propagation indices.
 
     Example
     -------
@@ -978,15 +986,17 @@
     ...    freqs=[2e14, 3e14],
     ...    mode_spec=ModeSpec(num_modes=5),
     ...    name='mode',
     ... )
     >>> data = ModeData(monitor=monitor, amps=amp_data, n_complex=index_data)
     """
 
-    monitor: ModeMonitor
+    monitor: ModeMonitor = pd.Field(
+        ..., title="Monitor", description="Mode monitor associated with the data."
+    )
 
     amps: ModeAmpsDataArray = pd.Field(
         ..., title="Amplitudes", description="Complex-valued amplitudes associated with the mode."
     )
 
     n_complex: ModeIndexDataArray = pd.Field(
         ...,
@@ -1020,16 +1030,21 @@
     >>> f = [2e14, 3e14]
     >>> coords = dict(f=f)
     >>> flux_data = FluxDataArray(np.random.random(2), coords=coords)
     >>> monitor = FluxMonitor(size=(2,0,6), freqs=[2e14, 3e14], name='flux')
     >>> data = FluxData(monitor=monitor, flux=flux_data)
     """
 
-    monitor: FluxMonitor
-    flux: FluxDataArray
+    monitor: FluxMonitor = pd.Field(
+        ..., title="Monitor", description="Frequency-domain flux monitor associated with the data."
+    )
+
+    flux: FluxDataArray = pd.Field(
+        ..., title="Flux", description="Flux values in the frequency-domain."
+    )
 
     def normalize(self, source_spectrum_fn) -> FluxData:
         """Return copy of self after normalization is applied using source spectrum function."""
         source_freq_amps = source_spectrum_fn(self.flux.f)
         source_power = abs(source_freq_amps) ** 2
         new_flux = (self.flux / source_power).astype(self.flux.dtype)
         return self.copy(update=dict(flux=new_flux))
@@ -1044,16 +1059,21 @@
     >>> t = [0, 1e-12, 2e-12]
     >>> coords = dict(t=t)
     >>> flux_data = FluxTimeDataArray(np.random.random(3), coords=coords)
     >>> monitor = FluxTimeMonitor(size=(2,0,6), interval=100, name='flux_time')
     >>> data = FluxTimeData(monitor=monitor, flux=flux_data)
     """
 
-    monitor: FluxTimeMonitor
-    flux: FluxTimeDataArray
+    monitor: FluxTimeMonitor = pd.Field(
+        ..., title="Monitor", description="Time-domain flux monitor associated with the data."
+    )
+
+    flux: FluxTimeDataArray = pd.Field(
+        ..., title="Flux", description="Flux values in the time-domain."
+    )
 
 
 ProjFieldType = Union[
     FieldProjectionAngleDataArray,
     FieldProjectionCartesianDataArray,
     FieldProjectionKSpaceDataArray,
     DiffractionDataArray,
@@ -1698,15 +1718,17 @@
     >>> data = DiffractionData(
     ...     monitor=monitor, sim_size=[1,1], bloch_vecs=[1,2],
     ...     Etheta=field, Ephi=field, Er=field,
     ...     Htheta=field, Hphi=field, Hr=field,
     ... )
     """
 
-    monitor: DiffractionMonitor
+    monitor: DiffractionMonitor = pd.Field(
+        ..., title="Monitor", description="Diffraction monitor associated with the data."
+    )
 
     Er: DiffractionDataArray = pd.Field(
         ...,
         title="Er",
         description="Spatial distribution of r-component of the electric field.",
     )
     Etheta: DiffractionDataArray = pd.Field(
```

### Comparing `tidy3d-2.1.1/tidy3d/components/data/sim_data.py` & `tidy3d-2.2.0/tidy3d/components/data/sim_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,29 +137,31 @@
         if source_index is None or len(self.simulation.sources) == 0:
             return np.ones_like
 
         source = self.simulation.sources[source_index]
         source_time = source.source_time
         times = self.simulation.tmesh
         dt = self.simulation.dt
-        user_defined_phase = np.exp(1j * source_time.phase)
 
         # get boundary information to determine whether to use complex fields
         boundaries = self.simulation.boundary_spec.to_list
         boundaries_1d = [boundary_1d for dim_boundary in boundaries for boundary_1d in dim_boundary]
         complex_fields = any(isinstance(boundary, BlochBoundary) for boundary in boundaries_1d)
         complex_fields = complex_fields and not isinstance(source, TFSF)
 
         # plug in mornitor_data frequency domain information
         def source_spectrum_fn(freqs):
             """Source amplitude as function of frequency."""
             spectrum = source_time.spectrum(times, freqs, dt, complex_fields)
 
-            # remove user defined phase from normalization so its effect is present in the result
-            return spectrum * np.conj(user_defined_phase)
+            # Remove user defined amplitude and phase from the normalization
+            # such that they would still have an effect on the output fields.
+            # In other words, we are only normalizing out the arbitrary part of the spectrum
+            # that depends on things like freq0, fwidth and offset.
+            return spectrum / source_time.amplitude / np.exp(1j * source_time.phase)
 
         return source_spectrum_fn
 
     def renormalize(self, normalize_index: int) -> SimulationData:
         """Return a copy of the :class:`.SimulationData` with a different source used for the
         normalization."""
```

### Comparing `tidy3d-2.1.1/tidy3d/components/field_projection.py` & `tidy3d-2.2.0/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/geometry.py` & `tidy3d-2.2.0/tidy3d/components/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple, Union, Any, Callable, Optional
 from math import isclose
 import functools
 
 import pydantic
 import numpy as np
-from matplotlib import patches
+from matplotlib import patches, path
 from shapely.geometry import Point, Polygon, box, MultiPolygon
 from shapely.validation import make_valid
 
 from .base import Tidy3dBaseModel, cached_property
 from .types import Bound, Size, Coordinate, Axis, Coordinate2D, ArrayFloat3D, PlanePosition
 from .types import Vertices, Ax, Shapely, annotate_type
 from .viz import add_ax_if_none, equal_aspect
 from .viz import PLOT_BUFFER, ARROW_LENGTH, arrow_style
 from .viz import PlotParams, plot_params_geometry, polygon_patch
 from ..log import log
 from ..exceptions import Tidy3dKeyError, SetupError, ValidationError, DataError
 from ..constants import MICROMETER, LARGE_NUMBER, RADIAN, fp_eps, inf
 from .data.dataset import TriangleMeshDataset
 from .data.data_array import TriangleMeshDataArray, DATA_ARRAY_MAP
+from .transformation import RotationAroundAxis
 
 try:
     import trimesh
 
     TRIMESH_AVAILABLE = True
 except Exception:  # pylint:disable=broad-except
     TRIMESH_AVAILABLE = False
@@ -640,39 +641,16 @@
         points : ArrayLike[float]
             Array of shape ``(3, ...)``.
         axis : Coordinate
             Axis of rotation
         angle : float
             Angle of rotation counter-clockwise around the axis (rad).
         """
-
-        if isclose(angle % (2 * np.pi), 0):
-            return points
-
-        # Normalized axis vector components
-        (ux, uy, uz) = axis / np.linalg.norm(axis)
-
-        # General rotation matrix
-        rot_mat = np.zeros((3, 3))
-        cos = np.cos(angle)
-        sin = np.sin(angle)
-        rot_mat[0, 0] = cos + ux**2 * (1 - cos)
-        rot_mat[0, 1] = ux * uy * (1 - cos) - uz * sin
-        rot_mat[0, 2] = ux * uz * (1 - cos) + uy * sin
-        rot_mat[1, 0] = uy * ux * (1 - cos) + uz * sin
-        rot_mat[1, 1] = cos + uy**2 * (1 - cos)
-        rot_mat[1, 2] = uy * uz * (1 - cos) - ux * sin
-        rot_mat[2, 0] = uz * ux * (1 - cos) - uy * sin
-        rot_mat[2, 1] = uz * uy * (1 - cos) + ux * sin
-        rot_mat[2, 2] = cos + uz**2 * (1 - cos)
-
-        if len(points.shape) == 1:
-            return rot_mat @ points
-
-        return np.tensordot(rot_mat, points, axes=1)
+        rotation = RotationAroundAxis(axis=axis, angle=angle)
+        return rotation.rotate_vector(points)
 
     def reflect_points(
         self,
         points: Points,
         polar_axis: Axis,
         angle_theta: float,
         angle_phi: float,
@@ -2529,31 +2507,34 @@
         if not np.any(inside_height):
             return inside_height
 
         # check what points are inside polygon cross section (face)
         z_local = z - z0  # distance to the middle
         dist = -z_local * self._tanq
 
-        def contains_pointwise(face_polygon):
-            def fun_contain(xy_point):
-                point = Point(xy_point)
-                return face_polygon.covers(point)
-
-            return fun_contain
+        # # Leaving this function and commented out lines using it below in case we want to revert
+        # # to it at some point, e.g. if we introduce a MATPLOTLIB_INSTALLED flag.
+        # def contains_pointwise(face_polygon):
+        #     def fun_contain(xy_point):
+        #         point = Point(xy_point)
+        #         return face_polygon.covers(point)
+        #     return fun_contain
 
         if isinstance(x, np.ndarray):
             inside_polygon = np.zeros_like(inside_height)
             xs_slab = x[inside_height]
             ys_slab = y[inside_height]
 
             # vertical sidewall
             if isclose(self.sidewall_angle, 0):
-                face_polygon = Polygon(self.reference_polygon)
-                fun_contain = contains_pointwise(face_polygon)
-                contains_vectorized = np.vectorize(fun_contain, signature="(n)->()")
+                # face_polygon = Polygon(self.reference_polygon)
+                # fun_contain = contains_pointwise(face_polygon)
+                # contains_vectorized = np.vectorize(fun_contain, signature="(n)->()")
+                poly_path = path.Path(self.reference_polygon)
+                contains_vectorized = poly_path.contains_points
                 points_stacked = np.stack((xs_slab, ys_slab), axis=1)
                 inside_polygon_slab = contains_vectorized(points_stacked)
                 inside_polygon[inside_height] = inside_polygon_slab
             # slanted sidewall, offsetting vertices at each z
             else:
                 # a helper function for moving axis
                 def _move_axis(arr):
@@ -2568,17 +2549,19 @@
 
                 for z_i in range(z.shape[self.axis]):
                     if not _move_axis(inside_height)[0, 0, z_i]:
                         continue
                     vertices_z = self._shift_vertices(
                         self.middle_polygon, _move_axis(dist)[0, 0, z_i]
                     )[0]
-                    face_polygon = Polygon(vertices_z)
-                    fun_contain = contains_pointwise(face_polygon)
-                    contains_vectorized = np.vectorize(fun_contain, signature="(n)->()")
+                    # face_polygon = Polygon(vertices_z)
+                    # fun_contain = contains_pointwise(face_polygon)
+                    # contains_vectorized = np.vectorize(fun_contain, signature="(n)->()")
+                    poly_path = path.Path(vertices_z)
+                    contains_vectorized = poly_path.contains_points
                     points_stacked = np.stack(
                         (x_axis[:, :, 0].flatten(), y_axis[:, :, 0].flatten()), axis=1
                     )
                     inside_polygon_slab = contains_vectorized(points_stacked)
                     inside_polygon_axis[:, :, z_i] = inside_polygon_slab.reshape(x_axis.shape[:2])
                 inside_polygon = _move_axis_reverse(inside_polygon_axis)
         else:
```

### Comparing `tidy3d-2.1.1/tidy3d/components/grid/grid.py` & `tidy3d-2.2.0/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.2.0/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/grid/mesher.py` & `tidy3d-2.2.0/tidy3d/components/grid/mesher.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,17 +376,18 @@
         min_steps = []
         for structure in structures:
             if isinstance(structure, Structure):
                 if isinstance(structure.medium, (PECMedium, Medium2D)):
                     index = 1.0
                 else:
                     n, k = structure.medium.eps_complex_to_nk(
-                        structure.medium.eps_diagonal(C_0 / wavelength)[axis]
+                        structure.medium.eps_diagonal(C_0 / wavelength)
                     )
-                    index = max(abs(n), abs(k))
+                    # take max among all directions because perpendicular eps defines wavelength
+                    index = max(max(abs(n)), max(abs(k)))
                 min_steps.append(max(dl_min, wavelength / index / min_steps_per_wvl))
             elif isinstance(structure, MeshOverrideStructure):
                 min_steps.append(max(dl_min, structure.dl[axis]))
         return np.array(min_steps)
 
     @staticmethod
     def rotate_structure_bounds(structures: List[StructureType], axis: Axis) -> List[ArrayFloat1D]:
```

### Comparing `tidy3d-2.1.1/tidy3d/components/medium.py` & `tidy3d-2.2.0/tidy3d/components/medium.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 import pydantic as pd
 import numpy as np
 import xarray as xr
 
 from .base import Tidy3dBaseModel, cached_property
 from .grid.grid import Coords, Grid
 from .types import PoleAndResidue, Ax, FreqBound, TYPE_TAG_STR, InterpMethod, Bound, ArrayComplex4D
-from .types import Axis
+from .types import Axis, TensorReal
 from .data.dataset import PermittivityDataset
 from .data.data_array import ScalarFieldDataArray
 from .viz import add_ax_if_none
 from .geometry import Geometry
 from .validators import validate_name_str
 from ..constants import C_0, pec_val, EPSILON_0, LARGE_NUMBER, fp_eps
 from ..constants import HERTZ, CONDUCTIVITY, PERMITTIVITY, RADPERSEC, MICROMETER, SECOND
 from ..exceptions import ValidationError, SetupError
 from ..log import log
+from .transformation import RotationType
 
 
 # evaluate frequency as this number (Hz) if inf
 FREQ_EVAL_INF = 1e50
 
 # extrapolation option in custom medium
 FILL_VALUE = "extrapolate"
@@ -127,14 +128,37 @@
             The diagonal elements of the relative permittivity tensor evaluated at ``frequency``.
         """
 
         # This only needs to be overwritten for anisotropic materials
         eps = self.eps_model(frequency)
         return (eps, eps, eps)
 
+    def eps_comp(self, row: Axis, col: Axis, frequency: float) -> complex:
+        """Single component of the complex-valued permittivity tensor as a function of frequency.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        complex
+           Element of the relative permittivity tensor evaluated at ``frequency``.
+        """
+
+        # This only needs to be overwritten for anisotropic materials
+        if row == col:
+            return self.eps_model(frequency)
+        return 0j
+
     @cached_property
     @abstractmethod
     def n_cfl(self):
         """To ensure a stable FDTD simulation, it is essential to select an appropriate
         time step size in accordance with the CFL condition. The maximal time step
         size is inversely proportional to the speed of light in the medium, and thus
         proportional to the index of refraction. However, for dispersive medium,
@@ -535,30 +559,67 @@
             np.array(
                 self._interp(eps_freq.field_components[comp], coords, self.interp_method)
             ).reshape(interp_shape)
             for comp in ["eps_xx", "eps_yy", "eps_zz"]
         ]
         return tuple(eps_list)
 
+    def eps_comp_on_grid(
+        self,
+        row: Axis,
+        col: Axis,
+        frequency: float,
+        coords: Coords,
+    ) -> ArrayComplex4D:
+        """Spatial profile of a single component of the complex-valued permittivity tensor at
+        ``frequency`` interpolated at the supplied coordinates.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+        coords : :class:`.Coords`
+            The grid point coordinates over which interpolation is performed.
+
+        Returns
+        -------
+        np.ndarray
+            Single component of the complex-valued permittivity tensor at ``frequency`` interpolated
+            at the supplied coordinates.
+        """
+
+        if row == col:
+            eps_freq = self.eps_dataset_freq(frequency)
+            interp_shape = [len(coord_comp) for coord_comp in coords.to_list]
+            comp = ["eps_xx", "eps_yy", "eps_zz"][row]
+            eps = self._interp(eps_freq.field_components[comp], coords, self.interp_method)
+            eps = np.array(eps).reshape(interp_shape)
+            return eps
+        return 0
+
     @ensure_freq_in_range
     def eps_diagonal(self, frequency: float) -> Tuple[complex, complex, complex]:
         """Main diagonal of the complex-valued permittivity tensor
-        at ``frequency``. Spatially, we take max{||eps||}, so that autoMesh generation
+        at ``frequency``. Spatially, we take max{|eps|}, so that autoMesh generation
         works appropriately.
         """
         eps_freq = self.eps_dataset_freq(frequency)
         eps_np_list = [
             np.array(sclr_fld).ravel() for _, sclr_fld in eps_freq.field_components.items()
         ]
         eps_list = [eps_comp[np.argmax(np.abs(eps_comp))] for eps_comp in eps_np_list]
         return tuple(eps_list)
 
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
-        """Spatial and poloarizaiton average of complex-valued permittivity
+        """Spatial and polarizaiton average of complex-valued permittivity
         as a function of frequency.
         """
         eps_freq = self.eps_dataset_freq(frequency)
         eps_array_avgs = [np.mean(eps_array) for _, eps_array in eps_freq.field_components.items()]
         return np.mean(eps_array_avgs)
 
     @classmethod
@@ -1237,14 +1298,38 @@
         """Main diagonal of the complex-valued permittivity tensor as a function of frequency."""
 
         eps_xx = self.xx.eps_model(frequency)
         eps_yy = self.yy.eps_model(frequency)
         eps_zz = self.zz.eps_model(frequency)
         return (eps_xx, eps_yy, eps_zz)
 
+    def eps_comp(self, row: Axis, col: Axis, frequency: float) -> complex:
+        """Single component the complex-valued permittivity tensor as a function of frequency.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        complex
+           Element of the relative permittivity tensor evaluated at ``frequency``.
+        """
+
+        if row != col:
+            return 0j
+        cmp = "xyz"[row]
+        field_name = cmp + cmp
+        return self.components[field_name].eps_model(frequency)
+
     @add_ax_if_none
     def plot(self, freqs: float, ax: Ax = None) -> Ax:
         """Plot n, k of a :class:`.Medium` as a function of frequency."""
 
         freqs = np.array(freqs)
         freqs_thz = freqs / 1e12
 
@@ -1263,26 +1348,229 @@
 
     @property
     def elements(self) -> Dict[str, IsotropicMediumType]:
         """The diagonal elements of the medium as a dictionary."""
         return dict(xx=self.xx, yy=self.yy, zz=self.zz)
 
 
+class FullyAnisotropicMedium(AbstractMedium):
+    """Fully anisotropic medium including all 9 components of the permittivity and conductivity
+    tensors. Provided permittivity tensor and the symmetric part of the conductivity tensor must
+    have coinciding main directions. A non-symmetric conductivity tensor can be used to model
+    magneto-optic effects. Note that dispersive properties and subpixel averaging are currently not
+    supported for fully anisotropic materials.
+
+    Note
+    ----
+    Simulations involving fully anisotropic materials are computationally more intensive, thus,
+    they take longer time to complete. This increase strongly depends on the filling fraction of
+    the simulation domain by fully anisotropic materials, varying approximately in the range from
+    1.5 to 5. Cost of running a simulation is adjusted correspondingly.
+
+    Example
+    -------
+    >>> perm = [[2, 0, 0], [0, 1, 0], [0, 0, 3]]
+    >>> cond = [[0.1, 0, 0], [0, 0, 0], [0, 0, 0]]
+    >>> anisotropic_dielectric = FullyAnisotropicMedium(permittivity=perm, conductivity=cond)
+    """
+
+    permittivity: TensorReal = pd.Field(
+        [[1, 0, 0], [0, 1, 0], [0, 0, 1]],
+        title="Permittivity",
+        description="Relative permittivity tensor.",
+        units=PERMITTIVITY,
+    )
+
+    conductivity: TensorReal = pd.Field(
+        [[0, 0, 0], [0, 0, 0], [0, 0, 0]],
+        title="Conductivity",
+        description="Electric conductivity tensor. Defined such that the imaginary part "
+        "of the complex permittivity at angular frequency omega is given by conductivity/omega.",
+        units=CONDUCTIVITY,
+    )
+
+    @pd.validator("permittivity", always=True)
+    def permittivity_spd_and_ge_one(cls, val):
+        """Check that provided permittivity tensor is symmetric positive definite
+        with eigenvalues >= 1.
+        """
+
+        if not np.allclose(val, np.transpose(val), atol=fp_eps):
+            raise ValidationError("Provided permittivity tensor is not symmetric.")
+
+        if np.any(np.linalg.eigvals(val) < 1 - fp_eps):
+            raise ValidationError("Main diagonal of provided permittivity tensor is not >= 1.")
+
+        return val
+
+    @pd.validator("conductivity", always=True)
+    def conductivity_ge_zero_and_commutes(cls, val, values):
+        """Check that the symmetric part of conductivity tensor commutes with permittivity tensor
+        (that is, simultaneously diagonalizable) with eigenvalues >= 0.
+        """
+
+        perm = values.get("permittivity")
+        cond_sym = 0.5 * (val + val.T)
+        comm_diff = np.abs(np.matmul(perm, cond_sym) - np.matmul(cond_sym, perm))
+
+        if not np.allclose(comm_diff, 0, atol=fp_eps):
+            raise ValidationError(
+                "Main directions of conductivity and permittivity tensor do not coincide."
+            )
+
+        if np.any(np.linalg.eigvals(cond_sym) < -fp_eps):
+            raise ValidationError("Main diagonal of provided conductivity tensor is not >= 0.")
+
+        return val
+
+    @classmethod
+    def from_diagonal(cls, xx: Medium, yy: Medium, zz: Medium, rotation: RotationType):
+        """Construct a fully anisotropic medium by rotating a diagonally ansisotropic medium.
+
+        Parameters
+        ----------
+        xx : :class:`.Medium`
+            Medium describing the xx-component of the diagonal permittivity tensor.
+        yy : :class:`.Medium`
+            Medium describing the yy-component of the diagonal permittivity tensor.
+        zz : :class:`.Medium`
+            Medium describing the zz-component of the diagonal permittivity tensor.
+        rotation : :class:`.RotationType`
+                Rotation applied to diagonal permittivity tensor.
+
+        Returns
+        -------
+        :class:`FullyAnisotropicMedium`
+            Resulting fully anisotropic medium.
+        """
+
+        permittivity_diag = np.diag([comp.permittivity for comp in [xx, yy, zz]]).tolist()
+        conductivity_diag = np.diag([comp.conductivity for comp in [xx, yy, zz]]).tolist()
+
+        permittivity = rotation.rotate_tensor(permittivity_diag)
+        conductivity = rotation.rotate_tensor(conductivity_diag)
+
+        return cls(permittivity=permittivity, conductivity=conductivity)
+
+    @cached_property
+    def _to_diagonal(self) -> AnisotropicMedium:
+        """Construct a diagonally anisotropic medium from main components.
+
+        Returns
+        -------
+        :class:`AnisotropicMedium`
+            Resulting diagonally anisotropic medium.
+        """
+
+        perm, cond, _ = self.eps_sigma_diag
+
+        return AnisotropicMedium(
+            xx=Medium(permittivity=perm[0], conductivity=cond[0]),
+            yy=Medium(permittivity=perm[1], conductivity=cond[1]),
+            zz=Medium(permittivity=perm[2], conductivity=cond[2]),
+        )
+
+    @cached_property
+    def eps_sigma_diag(
+        self,
+    ) -> Tuple[Tuple[float, float, float], Tuple[float, float, float], TensorReal]:
+        """Main components of permittivity and conductivity tensors and their directions."""
+
+        perm_diag, vecs = np.linalg.eig(self.permittivity)
+        cond_diag = np.diag(np.matmul(np.transpose(vecs), np.matmul(self.conductivity, vecs)))
+
+        return (perm_diag, cond_diag, vecs)
+
+    @ensure_freq_in_range
+    def eps_model(self, frequency: float) -> complex:
+        """Complex-valued permittivity as a function of frequency."""
+        perm_diag, cond_diag, _ = self.eps_sigma_diag
+
+        eps_diag = AbstractMedium.eps_sigma_to_eps_complex(perm_diag, cond_diag, frequency)
+        return np.mean(eps_diag)
+
+    @ensure_freq_in_range
+    def eps_diagonal(self, frequency: float) -> Tuple[complex, complex, complex]:
+        """Main diagonal of the complex-valued permittivity tensor as a function of frequency."""
+
+        perm_diag, cond_diag, _ = self.eps_sigma_diag
+
+        if not np.isscalar(frequency):
+            perm_diag = perm_diag[:, None]
+            cond_diag = cond_diag[:, None]
+        return AbstractMedium.eps_sigma_to_eps_complex(perm_diag, cond_diag, frequency)
+
+    def eps_comp(self, row: Axis, col: Axis, frequency: float) -> complex:
+        """Single component the complex-valued permittivity tensor as a function of frequency.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        complex
+           Element of the relative permittivity tensor evaluated at ``frequency``.
+        """
+
+        eps = self.permittivity[row][col]
+        sig = self.conductivity[row][col]
+        return AbstractMedium.eps_sigma_to_eps_complex(eps, sig, frequency)
+
+    @cached_property
+    def n_cfl(self):
+        """This property computes the index of refraction related to CFL condition, so that
+        the FDTD with this medium is stable when the time step size that doesn't take
+        material factor into account is multiplied by ``n_cfl``.
+
+        For this medium, it take the minimal of ``sqrt(permittivity)`` for main directions.
+        """
+
+        perm_diag, _, _ = self.eps_sigma_diag
+        return min(np.sqrt(perm_diag))
+
+    @add_ax_if_none
+    def plot(self, freqs: float, ax: Ax = None) -> Ax:
+        """Plot n, k of a :class:`FullyAnisotropicMedium` as a function of frequency."""
+
+        diagonal_medium = self._to_diagonal
+        ax = diagonal_medium.plot(freqs=freqs, ax=ax)
+        _, _, directions = self.eps_sigma_diag
+
+        # rename components from xx, yy, zz to 1, 2, 3 to avoid misleading
+        # and add their directions
+        for label, n_line, k_line, direction in zip(
+            ("1", "2", "3"), ax.lines[-6::2], ax.lines[-5::2], directions.T
+        ):
+            direction_str = f"({direction[0]:.2f}, {direction[1]:.2f}, {direction[2]:.2f})"
+            k_line.set_label(f"k, eps_{label} {direction_str}")
+            n_line.set_label(f"n, eps_{label} {direction_str}")
+
+        ax.legend()
+        return ax
+
+
 # types of mediums that can be used in Simulation and Structures
 
 MediumType3D = Union[
     Medium,
     CustomMedium,
     AnisotropicMedium,
     PECMedium,
     PoleResidue,
     Sellmeier,
     Lorentz,
     Debye,
     Drude,
+    FullyAnisotropicMedium,
 ]
 
 
 class Medium2D(AbstractMedium):
     """2D diagonally anisotropic medium.
 
     Note
```

### Comparing `tidy3d-2.1.1/tidy3d/components/mode.py` & `tidy3d-2.2.0/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/monitor.py` & `tidy3d-2.2.0/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/simulation.py` & `tidy3d-2.2.0/tidy3d/components/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .validators import validate_mode_objects_symmetry
 from .geometry import Box, TriangleMesh, Geometry, PolySlab, Cylinder
 from .types import Ax, Shapely, FreqBound, Axis, annotate_type, Symmetry
 from .grid.grid import Coords1D, Grid, Coords
 from .grid.grid_spec import GridSpec, UniformGrid, AutoGrid
 from .medium import Medium, MediumType, AbstractMedium, PECMedium
 from .medium import CustomMedium, Medium2D, MediumType3D
+from .medium import AnisotropicMedium, FullyAnisotropicMedium
 from .boundary import BoundarySpec, BlochBoundary, PECBoundary, PMCBoundary, Periodic
 from .boundary import PML, StablePML, Absorber, AbsorberSpec
 from .structure import Structure
 from .source import SourceType, PlaneWave, GaussianBeam, AstigmaticGaussianBeam, CustomFieldSource
 from .source import TFSF, Source
 from .monitor import MonitorType, Monitor, FreqMonitor
 from .monitor import AbstractFieldMonitor, DiffractionMonitor, AbstractFieldProjectionMonitor
@@ -46,16 +47,17 @@
 
 # maximum number of mediums supported
 MAX_NUM_MEDIUMS = 65530
 
 # maximum numbers of simulation parameters
 MAX_TIME_STEPS = 1e8
 MAX_GRID_CELLS = 20e9
-MAX_CELLS_TIMES_STEPS = 1e17
-MAX_MONITOR_DATA_SIZE_BYTES = 10e9
+MAX_CELLS_TIMES_STEPS = 1e16
+WARN_MONITOR_DATA_SIZE_GB = 10
+MAX_SIMULATION_DATA_SIZE_GB = 50
 
 # number of grid cells at which we warn about slow Simulation.epsilon()
 NUM_CELLS_WARN_EPSILON = 100_000_000
 # number of structures at which we warn about slow Simulation.epsilon()
 NUM_STRUCTURES_WARN_EPSILON = 10_000
 # for 2d materials. to find neighboring media, search a distance on either side
 # equal to this times the grid size
@@ -121,15 +123,15 @@
         title="Run Time",
         description="Total electromagnetic evolution time in seconds. "
         "Note: If simulation 'shutoff' is specified, "
         "simulation will terminate early when shutoff condition met. ",
         units=SECOND,
     )
 
-    medium: MediumType = pydantic.Field(
+    medium: MediumType3D = pydantic.Field(
         Medium(),
         title="Background Medium",
         description="Background medium of simulation, defaults to vacuum if not specified.",
     )
 
     symmetry: Tuple[Symmetry, Symmetry, Symmetry] = pydantic.Field(
         (0, 0, 0),
@@ -229,21 +231,14 @@
         if "version" not in values:
             return values
 
         # otherwise, call the updator to update the values dictionary
         updater = Updater(sim_dict=values)
         return updater.update_to_current()
 
-    @pydantic.validator("medium", always=True)
-    def _validate_medium(cls, val):
-        """Check that the medium is not a :class:`.Medium2D`."""
-        if isinstance(val, Medium2D):
-            raise ValidationError("'Simulation.medium' cannot be a 'Medium2D'.")
-        return val
-
     @pydantic.validator("grid_spec", always=True)
     def _validate_auto_grid_wavelength(cls, val, values):
         """Check that wavelength can be defined if there is auto grid spec."""
         if val.wavelength is None and val.auto_grid_used:
             _ = val.wavelength_from_sources(sources=values.get("sources"))
         return val
 
@@ -745,16 +740,18 @@
                         )
                         return val
                         # TODO: warn about custom grid spec
 
         return val
 
     @pydantic.validator("sources", always=True)
-    def _source_homogeneous(cls, val, values):
-        """Error if a plane wave or gaussian beam source is not in a homogeneous region."""
+    def _source_homogeneous_isotropic(cls, val, values):
+        """Error if a plane wave or gaussian beam source is not in a homogeneous and isotropic
+        region.
+        """
 
         if val is None:
             return val
 
         # list of structures including background as a Box()
         structure_bg = Structure(
             geometry=Box(
@@ -773,30 +770,45 @@
                 mediums = cls.intersecting_media(source, total_structures)
                 # make sure there is no more than one medium in the returned list
                 if len(mediums) > 1:
                     raise SetupError(
                         f"{len(mediums)} different mediums detected on plane "
                         f"intersecting a {source.type} source. Plane must be homogeneous."
                     )
+                if len(mediums) == 1 and isinstance(
+                    list(mediums)[0], (AnisotropicMedium, FullyAnisotropicMedium)
+                ):
+                    raise SetupError(
+                        f"An anisotropic medium is detected on plane intersecting a {source.type} "
+                        f"source. Injection of {source.type} into anisotropic media currently is "
+                        "not supported."
+                    )
 
         return val
 
     @pydantic.validator("normalize_index", always=True)
     def _check_normalize_index(cls, val, values):
         """Check validity of normalize index in context of simulation.sources."""
 
         # not normalizing
         if val is None:
             return val
 
-        assert val >= 0, "normalize_index can't be negative."
-        num_sources = len(values.get("sources"))
+        sources = values.get("sources")
+        num_sources = len(sources)
         if num_sources > 0:
             # No check if no sources, but it should be irrelevant anyway
-            assert val < num_sources, f"{num_sources} sources smaller than normalize_index of {val}"
+            if val >= num_sources:
+                raise ValidationError(
+                    f"'normalize_index' {val} out of bounds for number of sources {num_sources}."
+                )
+
+            # Also error if normalizing by a zero-amplitude source
+            if sources[val].source_time.amplitude == 0:
+                raise ValidationError("Cannot set 'normalize_index' to source with zero amplitude.")
 
         return val
 
     """ Post-init validators """
 
     def _post_init_validators(self) -> None:
         """Call validators taking z`self` that get run after init."""
@@ -880,57 +892,65 @@
         self._validate_tfsf_structure_intersections()
         # self._validate_run_time()
         _ = self.volumetric_structures
 
     def _validate_size(self) -> None:
         """Ensures the simulation is within size limits before simulation is uploaded."""
 
-        num_cells = self.num_cells
-        if num_cells > MAX_GRID_CELLS:
+        num_comp_cells = self.num_cells / 2 ** (np.sum(np.abs(self.symmetry)))
+        if num_comp_cells > MAX_GRID_CELLS:
             raise SetupError(
-                f"Simulation has {num_cells:.2e} computational cells, "
+                f"Simulation has {num_comp_cells:.2e} computational cells, "
                 f"a maximum of {MAX_GRID_CELLS:.2e} are allowed."
             )
 
         num_time_steps = self.num_time_steps
         if num_time_steps > MAX_TIME_STEPS:
             raise SetupError(
                 f"Simulation has {num_time_steps:.2e} time steps, "
                 f"a maximum of {MAX_TIME_STEPS:.2e} are allowed."
             )
 
-        num_cells_times_steps = num_time_steps * num_cells
+        num_cells_times_steps = num_time_steps * num_comp_cells
         if num_cells_times_steps > MAX_CELLS_TIMES_STEPS:
             raise SetupError(
                 f"Simulation has {num_cells_times_steps:.2e} grid cells * time steps, "
                 f"a maximum of {MAX_CELLS_TIMES_STEPS:.2e} are allowed."
             )
 
     def _validate_monitor_size(self) -> None:
         """Ensures the monitors arent storing too much data before simulation is uploaded."""
 
         tmesh = self.tmesh
         grid = self.grid
 
-        total_size_bytes = 0
+        total_size_gb = 0
         for monitor in self.monitors:
             monitor_inds = grid.discretize_inds(monitor, extend=True)
             num_cells = [inds[1] - inds[0] for inds in monitor_inds]
             # take monitor downsampling into account
             if isinstance(monitor, AbstractFieldMonitor):
                 num_cells = monitor.downsampled_num_cells(num_cells)
             num_cells = np.prod(num_cells)
             monitor_size = monitor.storage_size(num_cells=num_cells, tmesh=tmesh)
+            monitor_size_gb = monitor_size / 2**30
 
-            total_size_bytes += monitor_size
+            if monitor_size_gb > WARN_MONITOR_DATA_SIZE_GB:
+                log.warning(
+                    f"Monitor '{monitor.name}' estimated storage is {monitor_size_gb:1.2f}GB. "
+                    "Consider making it smaller, using fewer frequencies, or spatial or temporal "
+                    "downsampling using 'interval_space' and 'interval', respectively."
+                )
+
+            total_size_gb += monitor_size_gb
 
-        if total_size_bytes > MAX_MONITOR_DATA_SIZE_BYTES:
+        if total_size_gb > MAX_SIMULATION_DATA_SIZE_GB:
             raise SetupError(
-                f"Simulation's monitors have {total_size_bytes:.2e} bytes of estimated storage, "
-                f"a maximum of {MAX_MONITOR_DATA_SIZE_BYTES:.2e} are allowed."
+                f"Simulation's monitors have {total_size_gb:.2f}GB of estimated storage, "
+                f"a maximum of {MAX_SIMULATION_DATA_SIZE_GB:.2f}GB are allowed."
             )
 
     def _validate_datasets_not_none(self) -> None:
         """Ensures that all custom datasets are defined."""
         if any(dataset is None for dataset in self.custom_datasets):
             raise SetupError(
                 "Data for a custom data component is missing. This can happen for example if the "
@@ -938,15 +958,15 @@
                 "data, use hdf5 format instead."
             )
 
     def _validate_tfsf_structure_intersections(self) -> None:
         """Error if the 4 sidewalls of a TFSF box don't all intersect the same structures.
         This validator may need to compute permittivities on the grid, so it is called
         pre-upload rather than at the time of definition. Also errors if any side wall
-        intersects with a custom medium.
+        intersects with a custom medium or a fully anisotropic media.
         """
         for source in self.sources:
             if not isinstance(source, TFSF):
                 continue
             # get all TFSF surfaces
             tfsf_surfaces = Source.surfaces(
                 center=source.center, size=source.size, source_time=source.source_time
@@ -958,19 +978,20 @@
                 if surface.name[-2] != "xyz"[source.injection_axis]:
                     sidewall_surfaces.append(surface)
                     intersecting_structs = self.intersecting_structures(
                         test_object=surface, structures=self.structures
                     )
 
                     if any(
-                        isinstance(struct.medium, CustomMedium) for struct in intersecting_structs
+                        isinstance(struct.medium, (CustomMedium, FullyAnisotropicMedium))
+                        for struct in intersecting_structs
                     ):
                         raise SetupError(
-                            f"The surfaces of TFSF source '{source.name}' must not intersect "
-                            "any structures containing a 'CustomMedium'."
+                            f"The surfaces of TFSF source '{source.name}' must not intersect any "
+                            "structures containing a 'CustomMedium' or a 'FullyAnisotropicMedium'."
                         )
 
                     # if no structures intersect, just add a phantom associated with the simulation
                     # background, to prevent false positives below
                     if not intersecting_structs:
                         sidewall_structs.append(
                             [
@@ -2468,18 +2489,19 @@
 
         Parameters
         ----------
         box : :class:`.Box`
             Rectangular geometry specifying where to measure the permittivity.
         coord_key : str = 'centers'
             Specifies at what part of the grid to return the permittivity at.
-            Accepted values are ``{'centers', 'boundaries', 'Ex', 'Ey', 'Ez'}``.
-            The field values (eg. 'Ex') correspond to the correponding field locations on the yee
-            lattice. If field values are selected, the corresponding epsilon component from the
-            main diagonal of the epsilon tensor is returned. Otherwise, the average of the diagonal
+            Accepted values are ``{'centers', 'boundaries', 'Ex', 'Ey', 'Ez', 'Exy', 'Exz', 'Eyx',
+            'Eyz', 'Ezx', Ezy'}``. The field values (eg. 'Ex') correspond to the correponding field
+            locations on the yee lattice. If field values are selected, the corresponding diagonal
+            (eg. `eps_xx` in case of `Ex`) or off-diagonal (eg. `eps_xy` in case of `Exy`) epsilon
+            component from the epsilon tensor is returned. Otherwise, the average of the main
             values is returned.
         freq : float = None
             The frequency to evaluate the mediums at.
             If not specified, evaluates at infinite frequency.
         Returns
         -------
         xarray.DataArray
@@ -2501,18 +2523,19 @@
 
         Parameters
         ----------
         grid : :class:`.Grid`
             Grid specifying where to measure the permittivity.
         coord_key : str = 'centers'
             Specifies at what part of the grid to return the permittivity at.
-            Accepted values are ``{'centers', 'boundaries', 'Ex', 'Ey', 'Ez'}``.
-            The field values (eg. 'Ex') correspond to the correponding field locations on the yee
-            lattice. If field values are selected, the corresponding epsilon component from the
-            main diagonal of the epsilon tensor is returned. Otherwise, the average of the diagonal
+            Accepted values are ``{'centers', 'boundaries', 'Ex', 'Ey', 'Ez', 'Exy', 'Exz', 'Eyx',
+            'Eyz', 'Ezx', Ezy'}``. The field values (eg. 'Ex') correspond to the correponding field
+            locations on the yee lattice. If field values are selected, the corresponding diagonal
+            (eg. `eps_xx` in case of `Ex`) or off-diagonal (eg. `eps_xy` in case of `Exy`) epsilon
+            component from the epsilon tensor is returned. Otherwise, the average of the main
             values is returned.
         freq : float = None
             The frequency to evaluate the mediums at.
             If not specified, evaluates at infinite frequency.
         Returns
         -------
         xarray.DataArray
@@ -2534,16 +2557,20 @@
                 "Epsilon calculation may be slow."
             )
 
         def get_eps(structure: Structure, frequency: float, coords: Coords):
             """Select the correct epsilon component if field locations are requested."""
             if coord_key[0] != "E":
                 return np.mean(structure.eps_diagonal(frequency, coords), axis=0)
-            component = ["x", "y", "z"].index(coord_key[1])
-            return structure.eps_diagonal(frequency, coords)[component]
+            row = ["x", "y", "z"].index(coord_key[1])
+            if len(coord_key) == 2:  # diagonal component in case of Ex, Ey, and Ez
+                col = row
+            else:  # off-diagonal component in case of Exy, Exz, Eyx, etc
+                col = ["x", "y", "z"].index(coord_key[2])
+            return structure.eps_comp(row, col, frequency, coords)
 
         def make_eps_data(coords: Coords):
             """returns epsilon data on grid of points defined by coords"""
             arrays = (np.array(coords.x), np.array(coords.y), np.array(coords.z))
             eps_background = get_eps(
                 structure=self.background_structure, frequency=freq, coords=coords
             )
@@ -2576,15 +2603,19 @@
                 is_inside = structure.geometry.inside_meshgrid(*coords_reduced)
                 eps_array[inds][is_inside] = (eps_structure * is_inside)[is_inside]
 
             coords = dict(zip("xyz", arrays))
             return xr.DataArray(eps_array, coords=coords, dims=("x", "y", "z"))
 
         # combine all data into dictionary
-        coords = grid[coord_key]
+        if coord_key[0] == "E":
+            # off-diagonal componets are sampled at respective locations (eg. `eps_xy` at `Ex`)
+            coords = grid[coord_key[0:2]]
+        else:
+            coords = grid[coord_key]
         return make_eps_data(coords)
 
     @property
     def custom_datasets(self) -> List[Dataset]:
         """List of custom datasets for verification purposes. If the list is not empty, then
         the simulation needs to be exported to hdf5 to store the data.
         """
```

### Comparing `tidy3d-2.1.1/tidy3d/components/source.py` & `tidy3d-2.2.0/tidy3d/components/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         twidth = 1.0 / (2 * np.pi * self.fwidth)
         omega0 = 2 * np.pi * self.freq0
         time_shifted = time - self.offset * twidth
 
         const = 1j + time_shifted / twidth**2 / omega0
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
-        amp = np.exp(-(time_shifted**2) / 2 / twidth**2)
+        amp = np.exp(-(time_shifted**2) / 2 / twidth**2) * self.amplitude
 
         return const * offset * oscillation * amp
 
 
 class ContinuousWave(Pulse):
     """Source time dependence that ramps up to continuous oscillation
     and holds until end of simulation.
@@ -281,15 +281,15 @@
         twidth = 1.0 / (2 * np.pi * self.fwidth)
         omega0 = 2 * np.pi * self.freq0
         time_shifted = time - self.offset * twidth
 
         const = 1.0
         offset = np.exp(1j * self.phase)
         oscillation = np.exp(-1j * omega0 * time)
-        amp = 1 / (1 + np.exp(-time_shifted / twidth))
+        amp = 1 / (1 + np.exp(-time_shifted / twidth)) * self.amplitude
 
         return const * offset * oscillation * amp
 
 
 SourceTimeType = Union[GaussianPulse, ContinuousWave]
 
 """ Source objects """
@@ -853,15 +853,20 @@
         description="Distance to the beam waist along the propagation direction "
         "for the waist sizes in the local x and y directions.",
         units=MICROMETER,
     )
 
 
 class TFSF(AngledFieldSource, VolumeSource):
-    """Total field scattered field with a plane wave field in a volume."""
+    """Total-field scattered-field (TFSF) source that can inject a plane wave in a finite region.
+    The TFSF source injects 1 W / um^2 of power along the ``injection_axis``. Note that in the
+    case of angled incidence, 1 W / um^2 is still injected along the source's ``injection_axis``,
+    and not the propagation direction, unlike a ``PlaneWave`` source. This allows computing
+    scattering and absorption cross sections without the need for additional normalization.
+    """
 
     injection_axis: Axis = pydantic.Field(
         ...,
         title="Injection Axis",
         description="Specifies the injection axis. The plane of incidence is defined via this "
         "``injection_axis`` and the ``direction``. The popagation axis is defined with respect "
         "to the ``injection_axis`` by ``angle_theta`` and ``angle_phi``.",
```

### Comparing `tidy3d-2.1.1/tidy3d/components/structure.py` & `tidy3d-2.2.0/tidy3d/components/structure.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Union, Tuple, Optional
 import pydantic
 
 from .base import Tidy3dBaseModel
 from .validators import validate_name_str
 from .geometry import GeometryType
 from .medium import MediumType, CustomMedium, Medium2D
-from .types import Ax, TYPE_TAG_STR
+from .types import Ax, TYPE_TAG_STR, Axis
 from .viz import add_ax_if_none, equal_aspect
 from .grid.grid import Coords
 from ..constants import MICROMETER
 from ..exceptions import SetupError
 
 
 class AbstractStructure(Tidy3dBaseModel):
@@ -105,14 +105,37 @@
             if not geom:
                 raise SetupError(
                     "Can't validate 2D structure because its geometry did not pass validation."
                 )
             _ = geom._normal_2dmaterial  # pylint: disable=protected-access
         return val
 
+    def eps_comp(self, row: Axis, col: Axis, frequency: float, coords: Coords) -> complex:
+        """Single component of the complex-valued permittivity tensor as a function of frequency.
+
+        Parameters
+        ----------
+        row : int
+            Component's row in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        col : int
+            Component's column in the permittivity tensor (0, 1, or 2 for x, y, or z respectively).
+        frequency : float
+            Frequency to evaluate permittivity at (Hz).
+
+        Returns
+        -------
+        complex
+           Element of the relative permittivity tensor evaluated at ``frequency``.
+        """
+        if isinstance(self.medium, CustomMedium):
+            return self.medium.eps_comp_on_grid(
+                row=row, col=col, frequency=frequency, coords=coords
+            )
+        return self.medium.eps_comp(row=row, col=col, frequency=frequency)
+
 
 class MeshOverrideStructure(AbstractStructure):
     """Defines an object that is only used in the process of generating the mesh.
     A :class:`MeshOverrideStructure` is a combination of geometry :class:`Geometry`,
     grid size along x,y,z directions, and a boolean on whether the override
     will be enforced.
```

### Comparing `tidy3d-2.1.1/tidy3d/components/types.py` & `tidy3d-2.2.0/tidy3d/components/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,20 +39,22 @@
 
 
 class ArrayLike:
     """Type that stores a numpy array."""
 
     ndim = None
     dtype = None
+    shape = None
 
     @classmethod
     def __get_validators__(cls):
         yield cls.load_complex
         yield cls.convert_to_numpy
         yield cls.check_dims
+        yield cls.check_shape
 
     @classmethod
     def load_complex(cls, val):
         """Special handling to load a complex-valued np.ndarray saved to file."""
         if not isinstance(val, dict):
             return val
         if "real" not in val or "imag" not in val:
@@ -73,46 +75,59 @@
     def check_dims(cls, val):
         """Make sure the number of dimensions is correct."""
         if cls.ndim and val.ndim != cls.ndim:
             raise ValidationError(f"Expected {cls.ndim} dimensions for ArrayLike, got {val.ndim}.")
         return val
 
     @classmethod
+    def check_shape(cls, val):
+        """Make sure the shape is correct."""
+        if cls.shape and val.shape != cls.shape:
+            raise ValidationError(f"Expected shape {cls.shape} for ArrayLike, got {val.shape}.")
+        return val
+
+    @classmethod
     def __modify_schema__(cls, field_schema):
         """Sets the schema of DataArray object."""
 
         schema = dict(
             title="ArrayLike",
             type="ArrayLike",
         )
         field_schema.update(schema)
 
 
-def constrained_array(dtype: type = None, ndim: int = None) -> type:
+def constrained_array(
+    dtype: type = None, ndim: int = None, shape: Tuple[pydantic.NonNegativeInt, ...] = None
+) -> type:
     """Generate an ArrayLike sub-type with constraints built in."""
 
     # note, a unique name is required for each subclass of ArrayLike with constraints
     type_name = "ArrayLike"
     if dtype is not None:
         type_name += f"_dtype={dtype}"
     if ndim is not None:
         type_name += f"_ndim={ndim}"
-    return type(type_name, (ArrayLike,), dict(dtype=dtype, ndim=ndim))
+    if shape is not None:
+        type_name += f"_shape={shape}"
+    return type(type_name, (ArrayLike,), dict(dtype=dtype, ndim=ndim, shape=shape))
 
 
 # pre-define a set of commonly used array like instances for import and use in type hints
 ArrayFloat1D = constrained_array(dtype=float, ndim=1)
 ArrayFloat2D = constrained_array(dtype=float, ndim=2)
 ArrayFloat3D = constrained_array(dtype=float, ndim=3)
 ArrayFloat4D = constrained_array(dtype=float, ndim=4)
 ArrayComplex1D = constrained_array(dtype=complex, ndim=1)
 ArrayComplex2D = constrained_array(dtype=complex, ndim=2)
 ArrayComplex3D = constrained_array(dtype=complex, ndim=3)
 ArrayComplex4D = constrained_array(dtype=complex, ndim=4)
 
+TensorReal = constrained_array(dtype=float, ndim=2, shape=(3, 3))
+
 """ Complex Values """
 
 
 class ComplexNumber(pydantic.BaseModel):
     """Complex number with a well defined schema."""
 
     real: float
```

### Comparing `tidy3d-2.1.1/tidy3d/components/validators.py` & `tidy3d-2.2.0/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/components/viz.py` & `tidy3d-2.2.0/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/config.py` & `tidy3d-2.2.0/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/constants.py` & `tidy3d-2.2.0/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/exceptions.py` & `tidy3d-2.2.0/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/log.py` & `tidy3d-2.2.0/tidy3d/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Logging for Tidy3d."""
 
+import inspect
+
 from typing import Union
 from typing_extensions import Literal
 
 from rich.console import Console
 
 
 LogLevel = Literal["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
@@ -43,15 +45,20 @@
     def __init__(self, console: Console, level: LogValue):
         self.level = _get_level_int(level)
         self.console = console
 
     def handle(self, level, level_name, message):
         """Output log messages depending on log level"""
         if level >= self.level:
-            self.console.log(level_name, message, sep=": ")
+            stack = inspect.stack()
+            offset = 4
+            if stack[offset - 1].filename.endswith("exceptions.py"):
+                # We want the calling site for exceptions.py
+                offset += 1
+            self.console.log(level_name, message, sep=": ", _stack_offset=offset)
 
 
 class Logger:
     """Custom logger to avoid the complexities of the logging module"""
 
     def __init__(self):
         self.handlers = {}
```

### Comparing `tidy3d-2.1.1/tidy3d/material_library/material_library.py` & `tidy3d-2.2.0/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/material_library/material_reference.py` & `tidy3d-2.2.0/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.2.0/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Imports for adjoint plugin."""
 
 # import the jax version of tidy3d components
 try:
-    from .web import run, run_async
     from .components.geometry import JaxBox, JaxPolySlab
     from .components.medium import JaxMedium, JaxAnisotropicMedium, JaxCustomMedium
     from .components.structure import JaxStructure
     from .components.simulation import JaxSimulation
     from .components.data.sim_data import JaxSimulationData
     from .components.data.monitor_data import JaxModeData
     from .components.data.dataset import JaxPermittivityDataset
     from .components.data.data_array import JaxDataArray
 except ImportError as e:
     raise ImportError(
         "The 'jax' package is required for adjoint plugin and not installed. "
         "To get the appropriate packages, install tidy3d using '[jax]' option, for example: "
         "$pip install 'tidy3d[jax]'."
     ) from e
+
+try:
+    from .web import run, run_async
+except ImportError:
+    pass
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     )
 
     @pd.validator("coords", always=True)
     def _convert_coords_to_list(cls, val):
         """Convert supplied coordinates to Dict[str, list]."""
         return {coord_name: list(coord_list) for coord_name, coord_list in val.items()}
 
+    @pd.validator("values", always=True)
+    def _convert_values_to_np(cls, val):
+        """Convert supplied values to numpy if they are list (from file)."""
+        if isinstance(val, list):
+            return np.array(val)
+        return val
+
     # removed because it was slowing things down.
     # @pd.validator("coords", always=True)
     # def _coords_match_values(cls, val, values):
     #     """Make sure the coordinate dimensions and shapes match the values data."""
 
     #     values = values.get("values")
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Defines a jax-compatible SimulationData."""
 from __future__ import annotations
 
-from typing import Tuple, Dict, Union
+from typing import Tuple, Dict, Union, List
 
 import pydantic as pd
 
 from jax.tree_util import register_pytree_node_class
 
 from .....components.data.monitor_data import MonitorDataType, FieldData, PermittivityData
 from .....components.data.sim_data import SimulationData
@@ -40,77 +40,132 @@
 
     simulation: JaxSimulation = pd.Field(
         ...,
         title="Simulation",
         description="The jax-compatible simulation corresponding to the data.",
     )
 
+    task_id: str = pd.Field(
+        None,
+        title="Task ID",
+        description="Optional field storing the task_id for the original JaxSimulation.",
+    )
+
+    @property
+    def grad_data_symmetry(self) -> Tuple[FieldData, ...]:
+        """``self.grad_data`` but with ``symmetry_expanded_copy`` applied."""
+        return tuple(data.symmetry_expanded_copy for data in self.grad_data)
+
+    @property
+    def grad_eps_data_symmetry(self) -> Tuple[FieldData, ...]:
+        """``self.grad_eps_data`` but with ``symmetry_expanded_copy`` applied."""
+        return tuple(data.symmetry_expanded_copy for data in self.grad_eps_data)
+
     @property
     def output_monitor_data(self) -> Dict[str, JaxMonitorDataType]:
         """Dictionary of ``.output_data`` monitor ``.name`` to the corresponding data."""
         return {monitor_data.monitor.name: monitor_data for monitor_data in self.output_data}
 
     @property
     def monitor_data(self) -> Dict[str, Union[JaxMonitorDataType, MonitorDataType]]:
         """Dictionary of ``.output_data`` monitor ``.name`` to the corresponding data."""
         reg_mnt_data = {monitor_data.monitor.name: monitor_data for monitor_data in self.data}
         reg_mnt_data.update(self.output_monitor_data)
         return reg_mnt_data
 
+    @staticmethod
+    def split_data(
+        mnt_data: List[MonitorDataType], jax_info: JaxInfo
+    ) -> Dict[str, List[MonitorDataType]]:
+        """Split list of monitor data into data, output_data, grad_data, and grad_eps_data."""
+        # Get information needed to split the full data list
+        len_output_data = jax_info.num_output_monitors
+        len_grad_data = jax_info.num_grad_monitors
+        len_grad_eps_data = jax_info.num_grad_eps_monitors
+        len_data = len(mnt_data) - len_output_data - len_grad_data - len_grad_eps_data
+
+        # split the data list into regular data, output_data, and grad_data
+        all_data = list(mnt_data)
+        data = all_data[:len_data]
+        output_data = all_data[len_data : len_data + len_output_data]
+        grad_data = all_data[
+            len_data + len_output_data : len_data + len_output_data + len_grad_data
+        ]
+        grad_eps_data = all_data[len_data + len_output_data + len_grad_data :]
+
+        return dict(
+            data=data, output_data=output_data, grad_data=grad_data, grad_eps_data=grad_eps_data
+        )
+
     @classmethod
-    def from_sim_data(cls, sim_data: SimulationData, jax_info: JaxInfo) -> JaxSimulationData:
+    def from_sim_data(
+        cls, sim_data: SimulationData, jax_info: JaxInfo, task_id: str = None
+    ) -> JaxSimulationData:
         """Construct a :class:`.JaxSimulationData` instance from a :class:`.SimulationData`."""
 
         self_dict = sim_data.dict(exclude={"type", "simulation", "data"})
 
         # convert the simulation to JaxSimulation
         jax_sim = JaxSimulation.from_simulation(simulation=sim_data.simulation, jax_info=jax_info)
 
         # construct JaxSimulationData with no data (yet)
         self_dict["simulation"] = jax_sim
         self_dict["data"] = ()
 
-        # Get information needed to split the full data list
-        len_output_data = jax_info.num_output_monitors
-        len_grad_data = jax_info.num_grad_monitors
-        len_grad_eps_data = jax_info.num_grad_eps_monitors
-        len_data = len(sim_data.data) - len_output_data - len_grad_data - len_grad_eps_data
+        data_dict = cls.split_data(mnt_data=sim_data.data, jax_info=jax_info)
 
-        # split the data list into regular data, output_data, and grad_data
-        all_data = list(sim_data.data)
-        data = all_data[:len_data]
-        output_data = all_data[len_data : len_data + len_output_data]
-        grad_data = all_data[
-            len_data + len_output_data : len_data + len_output_data + len_grad_data
+        # convert the output data to the proper jax type
+        data_dict["output_data"] = [
+            JAX_MONITOR_DATA_MAP[type(x)].from_monitor_data(x) for x in data_dict["output_data"]
         ]
-        grad_eps_data = all_data[len_data + len_output_data + len_grad_data :]
 
-        # convert the jax data to the proper jax type
-        output_data = [
-            JAX_MONITOR_DATA_MAP[type(mnt_data)].from_monitor_data(mnt_data)
-            for mnt_data in output_data
-        ]
+        self_dict.update(data_dict)
+        self_dict.update(dict(task_id=task_id))
 
-        # add all data back in and return
-        self_dict.update(
-            dict(
-                data=data, output_data=output_data, grad_data=grad_data, grad_eps_data=grad_eps_data
-            )
+        return cls.parse_obj(self_dict)
+
+    @classmethod
+    def split_fwd_sim_data(
+        cls, sim_data: SimulationData, jax_info: JaxInfo
+    ) -> Tuple[SimulationData, SimulationData]:
+        """Split a :class:`.SimulationData` into two parts, containing user and gradient data."""
+
+        sim = sim_data.simulation
+
+        data_dict = cls.split_data(mnt_data=sim_data.data, jax_info=jax_info)
+        user_data = data_dict["data"] + data_dict["output_data"]
+        adjoint_data = data_dict["grad_data"] + data_dict["grad_eps_data"]
+
+        mnt_dict = JaxSimulation.split_monitors(
+            monitors=sim_data.simulation.monitors, jax_info=jax_info
         )
+        user_mnts = mnt_dict["monitors"] + mnt_dict["output_monitors"]
+        adjoint_mnts = mnt_dict["grad_monitors"] + mnt_dict["grad_eps_monitors"]
 
-        return cls.parse_obj(self_dict)
+        user_sim = sim.updated_copy(monitors=user_mnts)
+        adjoint_sim = sim.updated_copy(monitors=adjoint_mnts)
+
+        user_sim_data = sim_data.updated_copy(data=user_data, simulation=user_sim)
+        adjoint_sim_data = sim_data.updated_copy(data=adjoint_data, simulation=adjoint_sim)
+
+        return user_sim_data, adjoint_sim_data
 
     def make_adjoint_simulation(self, fwidth: float) -> JaxSimulation:
         """Make an adjoint simulation out of the data provided (generally, the vjp sim data)."""
 
         # grab boundary conditions with flipped bloch vectors (for adjoint)
         bc_adj = self.simulation.boundary_spec.flipped_bloch_vecs
 
         # add all adjoint sources and boundary conditions (at same time for BC validators to work)
         adj_srcs = []
         for mnt_data_vjp in self.output_data:
             for adj_source in mnt_data_vjp.to_adjoint_sources(fwidth=fwidth):
                 adj_srcs.append(adj_source)
 
         update_dict = dict(boundary_spec=bc_adj, sources=adj_srcs, monitors=(), output_monitors=())
-        update_dict.update(self.simulation.get_grad_monitors())
+        update_dict.update(
+            self.simulation.get_grad_monitors(
+                input_structures=self.simulation.input_structures,
+                freq_adjoint=self.simulation.freq_adjoint,
+            )
+        )
         return self.simulation.updated_copy(**update_dict)
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/medium.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 """Defines jax-compatible mediums."""
 from __future__ import annotations
 
-from typing import Dict, Tuple, Union
+from typing import Dict, Tuple, Union, Callable
+from abc import ABC
 
 import pydantic as pd
 import numpy as np
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
+import xarray as xr
 
 from ....components.types import Bound, Literal
 from ....components.medium import Medium, AnisotropicMedium, CustomMedium
 from ....components.geometry import Geometry
 from ....components.data.monitor_data import FieldData
 from ....components.data.dataset import PermittivityDataset
 from ....components.data.data_array import ScalarFieldDataArray
+from ....exceptions import SetupError
 
 from .base import JaxObject
 from .types import JaxFloat, validate_jax_float
 from .data.data_array import JaxDataArray
 from .data.dataset import JaxPermittivityDataset
 
 
 # number of integration points per unit wavelength in material
 PTS_PER_WVL_INTEGRATION = 20
 
+# maximum number of pixels allowed in each component of a JaxCustomMedium
+MAX_NUM_CELLS_CUSTOM_MEDIUM = 250_000
 
-@register_pytree_node_class
-class JaxMedium(Medium, JaxObject):
-    """A :class:`.Medium` registered with jax."""
-
-    permittivity: JaxFloat = pd.Field(
-        1.0,
-        title="Permittivity",
-        description="Relative permittivity of the medium. May be a ``jax`` ``DeviceArray``.",
-        jax_field=True,
-    )
 
-    _sanitize_permittivity = validate_jax_float("permittivity")
-
-    def to_medium(self) -> Medium:
-        """Convert :class:`.JaxMedium` instance to :class:`.Medium`"""
-        self_dict = self.dict(exclude={"type"})
-        return Medium.parse_obj(self_dict)
+class AbstractJaxMedium(ABC, JaxObject):
+    """Holds some utility functions for Jax medium types."""
 
     # pylint: disable =too-many-locals
     def _get_volume_disc(
         self, grad_data: FieldData, sim_bounds: Bound, wvl_mat: float
     ) -> Tuple[Dict[str, np.ndarray], float]:
         """Get the coordinates and volume element for the inside of the corresponding structure."""
 
@@ -56,75 +47,144 @@
         # assemble volume coordinates and differential volume element
         d_vol = 1.0
         vol_coords = {}
         for coord_name, min_edge, max_edge in zip("xyz", rmin, rmax):
 
             size = max_edge - min_edge
 
-            # ignore this dimension if there is no thickness along it
+            # don't discretize this dimension if there is no thickness along it
             if size == 0:
+                vol_coords[coord_name] = [max_edge]
                 continue
 
             # update the volume element value
             num_cells_dim = int(size * PTS_PER_WVL_INTEGRATION / wvl_mat) + 1
             d_len = size / num_cells_dim
             d_vol *= d_len
 
             # construct the interpolation coordinates along this dimension
             coords_interp = np.linspace(min_edge + d_len / 2, max_edge - d_len / 2, num_cells_dim)
             vol_coords[coord_name] = coords_interp
 
         return vol_coords, d_vol
 
-    # pylint:disable=too-many-arguments
-    def field_contribution(
+    @staticmethod
+    def make_inside_mask(vol_coords: Dict[str, np.ndarray], inside_fn: Callable) -> xr.DataArray:
+        """Make a 3D mask of where the volume coordinates are inside a supplied function."""
+
+        meshgrid_args = [vol_coords[dim] for dim in "xyz" if dim in vol_coords]
+        vol_coords_meshgrid = np.meshgrid(*meshgrid_args, indexing="ij")
+        inside_kwargs = dict(zip("xyz", vol_coords_meshgrid))
+        values = inside_fn(**inside_kwargs)
+        return xr.DataArray(values, coords=vol_coords)
+
+    # pylint: disable=too-many-arguments
+    def e_mult_volume(
         self,
         field: Literal["Ex", "Ey", "Ez"],
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
+        vol_coords: Dict[str, np.ndarray],
+        d_vol: float,
+        inside_fn: Callable,
+    ) -> xr.DataArray:
+        """Get the E_fwd * E_adj * dV field distribution inside of the discretized volume."""
+
+        e_fwd = grad_data_fwd.field_components[field]
+        e_adj = grad_data_adj.field_components[field]
+
+        e_dotted = (e_fwd * e_adj).real
+
+        inside_mask = self.make_inside_mask(vol_coords=vol_coords, inside_fn=inside_fn)
+
+        isel_kwargs = {
+            key: [0]
+            for key, value in vol_coords.items()
+            if isinstance(value, float) or len(value) <= 1
+        }
+        interp_kwargs = {key: value for key, value in vol_coords.items() if key not in isel_kwargs}
+
+        fields_eval = e_dotted.isel(f=0, **isel_kwargs).interp(**interp_kwargs, assume_sorted=True)
+        inside_mask = inside_mask.isel(**isel_kwargs)
+
+        return inside_mask * d_vol * fields_eval
+
+    def d_eps_map(
+        self,
+        grad_data_fwd: FieldData,
+        grad_data_adj: FieldData,
         sim_bounds: Bound,
         wvl_mat: float,
-    ) -> float:
-        """Compute the contribution to the VJP from a given field component."""
+        inside_fn: Callable,
+    ) -> xr.DataArray:
+        """Mapping of gradient w.r.t. permittivity at each point in discretized volume."""
 
         vol_coords, d_vol = self._get_volume_disc(
             grad_data=grad_data_fwd, sim_bounds=sim_bounds, wvl_mat=wvl_mat
         )
-        e_fwd = grad_data_fwd.field_components[field]
-        e_adj = grad_data_adj.field_components[field]
-        e_dotted = (e_fwd * e_adj).real
-        integrand = e_dotted.isel(f=0).interp(**vol_coords)
-        return d_vol * jnp.sum(integrand.values)
 
-    # pylint:disable=too-many-locals
+        e_mult_sum = 0.0
+
+        for field in ("Ex", "Ey", "Ez"):
+            e_mult_sum += self.e_mult_volume(
+                field=field,
+                grad_data_fwd=grad_data_fwd,
+                grad_data_adj=grad_data_adj,
+                vol_coords=vol_coords,
+                d_vol=d_vol,
+                inside_fn=inside_fn,
+            )
+
+        return e_mult_sum
+
+
+@register_pytree_node_class
+class JaxMedium(Medium, AbstractJaxMedium):
+    """A :class:`.Medium` registered with jax."""
+
+    permittivity: JaxFloat = pd.Field(
+        1.0,
+        title="Permittivity",
+        description="Relative permittivity of the medium. May be a ``jax`` ``DeviceArray``.",
+        jax_field=True,
+    )
+
+    _sanitize_permittivity = validate_jax_float("permittivity")
+
+    def to_medium(self) -> Medium:
+        """Convert :class:`.JaxMedium` instance to :class:`.Medium`"""
+        self_dict = self.dict(exclude={"type"})
+        return Medium.parse_obj(self_dict)
+
+    # pylint:disable=too-many-locals, too-many-arguments
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         sim_bounds: Bound,
         wvl_mat: float,
+        inside_fn: Callable[[np.ndarray, np.ndarray, np.ndarray], np.ndarray],
     ) -> JaxMedium:
         """Returns the gradient of the medium parameters given forward and adjoint field data."""
 
         # integrate the dot product of each E component over the volume, update vjp for epsilon
-        vjp_permittivty = 0.0
-        for field in ("Ex", "Ey", "Ez"):
-            vjp_permittivty += self.field_contribution(
-                field=field,
-                grad_data_fwd=grad_data_fwd,
-                grad_data_adj=grad_data_adj,
-                sim_bounds=sim_bounds,
-                wvl_mat=wvl_mat,
-            )
+        d_eps_map = self.d_eps_map(
+            grad_data_fwd=grad_data_fwd,
+            grad_data_adj=grad_data_adj,
+            sim_bounds=sim_bounds,
+            wvl_mat=wvl_mat,
+            inside_fn=inside_fn,
+        )
 
+        vjp_permittivty = jnp.sum(d_eps_map.values)
         return self.copy(update=dict(permittivity=vjp_permittivty))
 
 
 @register_pytree_node_class
-class JaxAnisotropicMedium(AnisotropicMedium, JaxObject):
+class JaxAnisotropicMedium(AnisotropicMedium, AbstractJaxMedium):
     """A :class:`.Medium` registered with jax."""
 
     xx: JaxMedium = pd.Field(
         ...,
         title="XX Component",
         description="Medium describing the xx-component of the diagonal permittivity tensor.",
         jax_field=True,
@@ -157,44 +217,51 @@
     def from_tidy3d(cls, tidy3d_obj: AnisotropicMedium) -> JaxAnisotropicMedium:
         """Convert :class:`.Tidy3dBaseModel` instance to :class:`.JaxObject`."""
         obj_dict = tidy3d_obj.dict(exclude={"type", "xx", "yy", "zz"})
         for component, tidy3d_medium in tidy3d_obj.components.items():
             obj_dict[component] = JaxMedium.from_tidy3d(tidy3d_medium)
         return cls.parse_obj(obj_dict)
 
-    # pylint:disable=too-many-locals
+    # pylint:disable=too-many-locals, too-many-arguments
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         sim_bounds: Bound,
         wvl_mat: float,
+        inside_fn: Callable,
     ) -> JaxMedium:
         """Returns the gradient of the medium parameters given forward and adjoint field data."""
 
         # integrate the dot product of each E component over the volume, update vjp for epsilon
+        vol_coords, d_vol = self._get_volume_disc(
+            grad_data=grad_data_fwd, sim_bounds=sim_bounds, wvl_mat=wvl_mat
+        )
+
         vjp_fields = {}
         for component in "xyz":
             field_name = "E" + component
             component_name = component + component
-            jax_medium = self.components[component_name]
-            vjp_ii = jax_medium.field_contribution(
+            e_mult_dim = self.e_mult_volume(
                 field=field_name,
                 grad_data_fwd=grad_data_fwd,
                 grad_data_adj=grad_data_adj,
-                sim_bounds=sim_bounds,
-                wvl_mat=wvl_mat,
+                vol_coords=vol_coords,
+                d_vol=d_vol,
+                inside_fn=inside_fn,
             )
+
+            vjp_ii = jnp.sum(e_mult_dim.real.values)
             vjp_fields[component_name] = JaxMedium(permittivity=vjp_ii)
 
         return self.copy(update=vjp_fields)
 
 
 @register_pytree_node_class
-class JaxCustomMedium(CustomMedium, JaxObject):
+class JaxCustomMedium(CustomMedium, AbstractJaxMedium):
     """A :class:`.CustomMedium` registered with ``jax``.
     Note: The gradient calculation assumes uniform field across the pixel.
     Therefore, the accuracy degrades as the pixel size becomes large
     with respect to the field variation.
     """
 
     eps_dataset: JaxPermittivityDataset = pd.Field(
@@ -203,14 +270,50 @@
         description="User-supplied dataset containing complex-valued permittivity "
         "as a function of space. Permittivity distribution over the Yee-grid will be "
         "interpolated based on the data nearest to the grid location.",
         jax_field=True,
     )
 
     @pd.validator("eps_dataset", always=True)
+    def _is_not_3d(cls, val):
+        """Ensure the custom medium pixels contain at least one dimension with only pixel thick."""
+
+        for field_dim in "xyz":
+            field_name = f"eps_{field_dim}{field_dim}"
+            data_array = val.field_components[field_name]
+            coord_lens = [len(data_array.coords[key]) for key in "xyz"]
+            dims_len1 = [val == 1 for val in coord_lens]
+            if sum(dims_len1) == 0:
+                raise SetupError(
+                    "For adjoint plugin, the 'JaxCustomMedium' is restricted to a 1D or 2D "
+                    "pixellated grid. It may not contain multiple pixels along all 3 dimensions. "
+                    f"Detected 3D pixelated grid in '{field_name}' component of 'eps_dataset'."
+                )
+
+        return val
+
+    @pd.validator("eps_dataset", always=True)
+    def _is_not_too_large(cls, val):
+        """Ensure number of pixels doesnt surpass a set amount."""
+
+        for field_dim in "xyz":
+            field_name = f"eps_{field_dim}{field_dim}"
+            data_array = val.field_components[field_name]
+            coord_lens = [len(data_array.coords[key]) for key in "xyz"]
+            num_cells_dim = np.prod(coord_lens)
+            if num_cells_dim > MAX_NUM_CELLS_CUSTOM_MEDIUM:
+                raise SetupError(
+                    "For the adjoint plugin, each component of the 'JaxCustomMedium.eps_dataset' "
+                    f"is restricted to have a maximum of {MAX_NUM_CELLS_CUSTOM_MEDIUM} cells. "
+                    f"Detected {num_cells_dim} grid cells in the '{field_name}' component ."
+                )
+
+        return val
+
+    @pd.validator("eps_dataset", always=True)
     def _single_frequency(cls, val):
         """Override of inherited validator."""
         return val
 
     @pd.validator("eps_dataset", always=True)
     def _eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
         """Override of inherited validator."""
@@ -248,71 +351,119 @@
             values = data_array.values.tolist()
             coords = {key: np.array(val).tolist() for key, val in data_array.coords.items()}
             field_components[field_name] = JaxDataArray(values=values, coords=coords)
         eps_dataset = JaxPermittivityDataset(**field_components)
         obj_dict["eps_dataset"] = eps_dataset
         return cls.parse_obj(obj_dict)
 
-    # pylint:disable=too-many-locals, unused-argument
+    # pylint:disable=too-many-locals, unused-argument, too-many-arguments
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         sim_bounds: Bound,
         wvl_mat: float,
+        inside_fn: Callable[[np.ndarray, np.ndarray, np.ndarray], np.ndarray],
     ) -> JaxMedium:
         """Returns the gradient of the medium parameters given forward and adjoint field data."""
 
         # get the boundaries of the intersection of the CustomMedium and the Simulation
         mnt_bounds = grad_data_fwd.monitor.geometry.bounds
         bounds_intersect = Geometry.bounds_intersection(mnt_bounds, sim_bounds)
 
         # get the grids associated with the user-supplied coordinates within these bounds
         grids = self.grids(bounds=bounds_intersect)
 
         vjp_field_components = {}
         for dim in "xyz":
 
             eps_field_name = f"eps_{dim}{dim}"
-            field_name = f"E{dim}"
 
             # grab the original data and its coordinatess
             orig_data_array = self.eps_dataset.field_components[eps_field_name]
             coords = orig_data_array.coords
 
-            # construct the coordinates for interpolation and selection within the custom medium
-            interp_coords = {dim_pt: coords[dim_pt] for dim_pt in "xyz" if len(coords[dim_pt]) > 1}
-            isel_coords = {dim_pt: 0 for dim_pt in "xyz" if len(coords[dim_pt]) <= 1}
-
-            # interpolate into the forward and adjoint fields along this dimension and dot them
-            e_fwd = grad_data_fwd.field_components[field_name]
-            e_adj = grad_data_adj.field_components[field_name]
-            e_dotted = (e_fwd * e_adj).isel(f=0, **isel_coords).interp(**interp_coords)
-
-            # compute the size of the user-supplied medium along each dimension.
             grid = grids[eps_field_name]
             d_sizes = grid.sizes
+            d_sizes = [d_sizes.x, d_sizes.y, d_sizes.z]
 
-            # if any of the sizes are just 0, indicating an ndim < 3, just normalize out to 1.0
-            d_sizes = (
-                np.ones(1) if len(dl) == 1 and dl[0] <= 0 else dl
-                for dl in (d_sizes.x, d_sizes.y, d_sizes.z)
-            )
+            # construct the coordinates for interpolation and selection within the custom medium
+            # TODO: extend this to all points within the volume.
+            interp_coords = {}
+            sum_axes = []
+
+            for dim_index, dim_pt in enumerate("xyz"):
+
+                coord_dim = coords[dim_pt]
+
+                # if it's uniform / single pixel along this dim
+                if len(np.array(coord_dim)) == 1:
+                    # discretize along this edge like a regular volume
+
+                    # compute the length of the pixel within the sim bounds
+                    r_min_coords, r_max_coords = grid.boundaries.to_list[dim_index]
+                    r_min_sim, r_max_sim = np.array(sim_bounds).T[dim_index]
+                    r_min = max(r_min_coords, r_min_sim)
+                    r_max = min(r_max_coords, r_max_sim)
+                    size = abs(r_max - r_min)
+
+                    # compute the length element along the dim, handling case of sim.size=0
+                    if size > 0:
+
+                        # discretize according to PTS_PER_WVL
+                        num_cells_dim = int(size * PTS_PER_WVL_INTEGRATION / wvl_mat) + 1
+                        d_len = size / num_cells_dim
+                        coords_interp = np.linspace(
+                            r_min + d_len / 2, r_max - d_len / 2, num_cells_dim
+                        )
+
+                    else:
+
+                        # just interpolate at the single position, dL=1 to normalize out
+                        d_len = 1.0
+                        coords_interp = np.array([(r_min + r_max) / 2.0])
+
+                    # construct the interpolation coordinates along this dimension
+                    d_sizes[dim_index] = np.array([d_len])
+                    interp_coords[dim_pt] = coords_interp
+
+                    # only sum this dimesion if there are multiple points
+                    sum_axes.append(dim_pt)
+
+                # otherwise
+                else:
+                    # just evaluate at the original data coords
+                    interp_coords[dim_pt] = coord_dim
 
             # outer product all dimensions to get a volume element mask
             d_vols = np.einsum("i, j, k -> ijk", *d_sizes)
 
-            # multiply volume element into gradient and reshape to expected vjp_shape
+            # grab the correpsonding dotted fields at these interp_coords and sum over len-1 pixels
+            field_name = "E" + dim
+            e_dotted = self.e_mult_volume(
+                field=field_name,
+                grad_data_fwd=grad_data_fwd,
+                grad_data_adj=grad_data_adj,
+                vol_coords=interp_coords,
+                d_vol=d_vols,
+                inside_fn=inside_fn,
+            ).sum(sum_axes)
+
+            # if np.any(np.isnan(e_dotted)) or np.isclose(np.sum(e_dotted), 0):
+            #     import pdb; pdb.set_trace()
+
+            # reshape values to the expected vjp shape to be more safe
             vjp_shape = tuple(len(coord) for _, coord in coords.items())
-            vjp_values = (np.squeeze(d_vols) * e_dotted.real.values).reshape(vjp_shape)
+            vjp_values = e_dotted.real.values.reshape(vjp_shape)
 
             # construct a DataArray storing the vjp
             vjp_data_array = JaxDataArray(values=vjp_values, coords=coords)
             vjp_field_components[eps_field_name] = vjp_data_array
 
+        # package everything into dataset
         vjp_eps_dataset = JaxPermittivityDataset(**vjp_field_components)
         return self.copy(update=dict(eps_dataset=vjp_eps_dataset))
 
 
 JaxMediumType = Union[JaxMedium, JaxAnisotropicMedium, JaxCustomMedium]
 
 # pylint: disable=unhashable-member
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,67 @@
 """Defines a jax-compatible simulation."""
 from __future__ import annotations
 
-from typing import Tuple, Union
-from collections import namedtuple
+from typing import Tuple, Union, List, Dict
 
 import pydantic as pd
 import numpy as np
 
 from jax.tree_util import register_pytree_node_class
 
 from ....log import log
-from ....components.base import cached_property
+from ....components.base import cached_property, Tidy3dBaseModel
 from ....components.monitor import FieldMonitor, PermittivityMonitor
-from ....components.monitor import ModeMonitor, DiffractionMonitor
+from ....components.monitor import ModeMonitor, DiffractionMonitor, Monitor
 from ....components.simulation import Simulation
 from ....components.data.monitor_data import FieldData, PermittivityData
+from ....components.structure import Structure
 from ....components.types import Ax, annotate_type
 from ....constants import HERTZ
 from ....exceptions import AdjointError
 
 from .base import JaxObject
 from .structure import JaxStructure
-from .geometry import JaxBox
+from .geometry import JaxPolySlab
 
 
-# used to store information when converting between jax and tidy3d
-JaxInfo = namedtuple(
-    "JaxInfo",
-    "num_input_structures num_output_monitors num_grad_monitors num_grad_eps_monitors "
-    "fwidth_adjoint",
-)
+class JaxInfo(Tidy3dBaseModel):
+    """Class to store information when converting between jax and tidy3d."""
+
+    num_input_structures: pd.NonNegativeInt = pd.Field(
+        ...,
+        title="Number of Input Structures",
+        description="Number of input structures in the original JaxSimulation.",
+    )
+
+    num_output_monitors: pd.NonNegativeInt = pd.Field(
+        ...,
+        title="Number of Output Monitors",
+        description="Number of output monitors in the original JaxSimulation.",
+    )
+
+    num_grad_monitors: pd.NonNegativeInt = pd.Field(
+        ...,
+        title="Number of Gradient Monitors",
+        description="Number of gradient monitors in the original JaxSimulation.",
+    )
+
+    num_grad_eps_monitors: pd.NonNegativeInt = pd.Field(
+        ...,
+        title="Number of Permittivity Monitors",
+        description="Number of permittivity monitors in the original JaxSimulation.",
+    )
+
+    fwidth_adjoint: float = pd.Field(
+        None,
+        title="Adjoint Frequency Width",
+        description="Custom frequency width of the original JaxSimulation.",
+        units=HERTZ,
+    )
+
 
 # bandwidth of adjoint source in units of freq0 if no sources and no `fwidth_adjoint` specified
 FWIDTH_FACTOR = 1.0 / 10
 
 
 @register_pytree_node_class
 class JaxSimulation(Simulation, JaxObject):
@@ -102,56 +130,75 @@
     def _subpixel_is_on(cls, val):
         """Assert subpixel is on."""
         if not val:
             raise AdjointError("'JaxSimulation.subpixel' must be 'True' to use adjoint plugin.")
         return val
 
     @pd.validator("input_structures", always=True)
-    def _no_overlap(cls, val):
-        """Assert no input structures overlap."""
+    def _warn_overlap(cls, val, values):
+        """Print appropriate warning if structures intersect in ways that cause gradient error."""
 
-        # only apply to boxes for now for simplicity..
-        structures = [struct for struct in val if isinstance(struct.geometry, JaxBox)]
+        input_structures = list(val)
+        structures = list(values.get("structures"))
 
         # if the center and size of all structure geometries do not contain all numbers, skip check
-        for struct in structures:
+        for struct in input_structures:
             geometry = struct.geometry
             size_all_floats = all(isinstance(s, (float, int)) for s in geometry.bound_size)
             cent_all_floats = all(isinstance(c, (float, int)) for c in geometry.bound_center)
             if not (size_all_floats and cent_all_floats):
                 return val
 
-        # flag to ensure that we only warn once for touching structures (otherwise, too many logs)
-        in_structs_background = []
-        for i, in_struct in enumerate(structures):
-            in_geometry = in_struct.geometry
-
-            # for all structures in the background
-            for j, in_struct_bck in enumerate(in_structs_background):
-
-                # if the contracted geometry intersects with a background structure, raise (overlap)
-                if in_geometry.intersects(in_struct_bck.geometry):
+        # check intersections with other input_structures
+        for i, in_struct_i in enumerate(input_structures):
+            geometry_i = in_struct_i.geometry
+            for j in range(i + 1, len(input_structures)):
+                geometry_j = input_structures[j].geometry
+                if geometry_i.intersects(geometry_j):
                     log.warning(
-                        f"'JaxSimulation.input_structures' elements {j} and {i} "
-                        "are overlapping or touching. "
-                        "Geometric gradients for overlapping structures may contain errors. "
+                        f"'JaxSimulation.input_structures[{i}]' overlaps or touches "
+                        f"'JaxSimulation.input_structures[{j}]'. "
+                        "Geometric gradients for overlapping input structures may contain errors. "
+                        "Skipping the rest of the structures."
                     )
+                    return val
 
-            in_structs_background.append(in_struct)
+        # check JaxPolySlab intersections with background structures
+        for i, in_struct_i in enumerate(input_structures):
+            geometry_i = in_struct_i.geometry
+            if not isinstance(geometry_i, JaxPolySlab):
+                continue
+            for j, struct_j in enumerate(structures):
+                geometry_j = struct_j.geometry
+                if geometry_i.intersects(geometry_j):
+                    log.warning(
+                        f"'JaxPolySlab'-containing 'JaxSimulation.input_structures[{i}]' "
+                        f"intersects with 'JaxSimulation.structures[{j}]'. "
+                        "Note that in this version of the adjoint plugin, there may be errors "
+                        "in the gradient when "
+                        "'JaxPolySlab' intersects with background structures. "
+                        "Skipping the rest of the structures."
+                    )
+                    return val
 
         return val
 
-    @cached_property
-    def freq_adjoint(self) -> float:
+    @staticmethod
+    def get_freq_adjoint(output_monitors: List[Monitor]) -> float:
         """Return the single adjoint frequency stripped from the output monitors."""
 
-        if len(self.output_monitors) == 0:
+        if len(output_monitors) == 0:
             raise AdjointError("Can't get adjoint frequency as no output monitors present.")
 
-        return self.output_monitors[0].freqs[0]
+        return output_monitors[0].freqs[0]
+
+    @cached_property
+    def freq_adjoint(self) -> float:
+        """Return the single adjoint frequency stripped from the output monitors."""
+        return self.get_freq_adjoint(output_monitors=self.output_monitors)
 
     @cached_property
     def _fwidth_adjoint(self) -> float:
         """Frequency width to use for adjoint source, user-defined or the average of the sources."""
 
         # if user-specified, use that
         if self.fwidth_adjoint is not None:
@@ -256,87 +303,162 @@
             monitor_alpha=monitor_alpha,
         )
 
     def __eq__(self, other: JaxSimulation) -> bool:
         """Are two JaxSimulation objects equal?"""
         return self.to_simulation()[0] == other.to_simulation()[0]
 
-    # pylint:disable=too-many-locals
     @classmethod
-    def from_simulation(cls, simulation: Simulation, jax_info: JaxInfo) -> JaxSimulation:
-        """Convert :class:`.Simulation` to :class:`.JaxSimulation` with extra info."""
-
-        sim_dict = simulation.dict(exclude={"type", "structures", "monitors"})  # .copy()
+    def split_monitors(cls, monitors: List[Monitor], jax_info: JaxInfo) -> Dict[str, Monitor]:
+        """Split monitors into user and adjoint required based on jax info."""
 
-        all_monitors = list(simulation.monitors)
-        all_structures = list(simulation.structures)
+        all_monitors = list(monitors)
 
+        # grab or compute the number of type of monitor
         num_grad_monitors = jax_info.num_grad_monitors
         num_grad_eps_monitors = jax_info.num_grad_eps_monitors
         num_output_monitors = jax_info.num_output_monitors
-        num_input_structures = jax_info.num_input_structures
-
-        num_structs = len(simulation.structures) - num_input_structures
-        structures = all_structures[:num_structs]
-        input_structures = [JaxStructure.from_structure(s) for s in all_structures[num_structs:]]
-
+        num_total_monitors = len(all_monitors)
         num_mnts = (
-            len(simulation.monitors)
-            - num_grad_monitors
-            - num_output_monitors
-            - num_grad_eps_monitors
+            num_total_monitors - num_grad_monitors - num_output_monitors - num_grad_eps_monitors
         )
+
+        # split the monitor list based on these numbers
         monitors = all_monitors[:num_mnts]
         output_monitors = all_monitors[num_mnts : num_mnts + num_output_monitors]
         grad_monitors = all_monitors[
             num_mnts + num_output_monitors : num_mnts + num_output_monitors + num_grad_monitors
         ]
         grad_eps_monitors = all_monitors[num_mnts + num_output_monitors + num_grad_monitors :]
 
-        sim_dict.update(
-            dict(
-                monitors=monitors,
-                output_monitors=output_monitors,
-                grad_monitors=grad_monitors,
-                grad_eps_monitors=grad_eps_monitors,
-                structures=structures,
-                input_structures=input_structures,
-                fwidth_adjoint=jax_info.fwidth_adjoint,
-            )
+        # load into a dictionary
+        return dict(
+            monitors=monitors,
+            output_monitors=output_monitors,
+            grad_monitors=grad_monitors,
+            grad_eps_monitors=grad_eps_monitors,
         )
 
+    @classmethod
+    def split_structures(
+        cls, structures: List[Structure], jax_info: JaxInfo
+    ) -> Dict[str, Structure]:
+        """Split structures into regular and input based on jax info."""
+
+        all_structures = list(structures)
+
+        # get numbers of regular and input structures
+        num_input_structures = jax_info.num_input_structures
+        num_structs = len(structures) - num_input_structures
+
+        # split the list based on these numbers
+        structures = all_structures[:num_structs]
+        input_structures = [JaxStructure.from_structure(s) for s in all_structures[num_structs:]]
+
+        # return a dictionary containing these split structures
+        return dict(structures=structures, input_structures=input_structures)
+
+    # pylint:disable=too-many-locals
+    @classmethod
+    def from_simulation(cls, simulation: Simulation, jax_info: JaxInfo) -> JaxSimulation:
+        """Convert :class:`.Simulation` to :class:`.JaxSimulation` with extra info."""
+
+        sim_dict = simulation.dict(exclude={"type", "structures", "monitors"})
+
+        # split structures and monitors into their respective fields for JaxSimulation
+        structures = cls.split_structures(structures=simulation.structures, jax_info=jax_info)
+        monitors = cls.split_monitors(monitors=simulation.monitors, jax_info=jax_info)
+
+        # update the dictionary with these and the adjoint fwidth
+        sim_dict.update(**structures)
+        sim_dict.update(**monitors)
+        sim_dict.update(dict(fwidth_adjoint=jax_info.fwidth_adjoint))
+
+        # load JaxSimulation from the dictionary
         return cls.parse_obj(sim_dict)
 
-    def get_grad_monitors(self) -> dict:
+    @classmethod
+    def make_sim_fwd(cls, simulation: Simulation, jax_info: JaxInfo) -> Tuple[Simulation, JaxInfo]:
+        """Make the forward :class:`.JaxSimulation` from the supplied :class:`.Simulation`."""
+
+        mnt_dict = JaxSimulation.split_monitors(monitors=simulation.monitors, jax_info=jax_info)
+        structure_dict = JaxSimulation.split_structures(
+            structures=simulation.structures, jax_info=jax_info
+        )
+        output_monitors = mnt_dict["output_monitors"]
+        input_structures = structure_dict["input_structures"]
+        grad_mnt_dict = cls.get_grad_monitors(
+            input_structures=input_structures,
+            freq_adjoint=cls.get_freq_adjoint(output_monitors=output_monitors),
+        )
+
+        grad_mnts = grad_mnt_dict["grad_monitors"]
+        grad_eps_mnts = grad_mnt_dict["grad_eps_monitors"]
+
+        full_monitors = list(simulation.monitors) + grad_mnts + grad_eps_mnts
+
+        # jax_sim_fwd = jax_sim.updated_copy(**grad_mnts)
+        # sim_fwd, jax_info = jax_sim_fwd.to_simulation()
+
+        sim_fwd = simulation.updated_copy(monitors=full_monitors)
+        jax_info = jax_info.updated_copy(
+            num_grad_monitors=len(grad_mnts),
+            num_grad_eps_monitors=len(grad_eps_mnts),
+        )
+
+        # cls.split_monitors(monitors=simulation.monitors, jax_info=jax_info)
+        # sim_fwd = simulation.updated_copy()
+
+        return sim_fwd, jax_info
+
+    def to_simulation_fwd(self) -> Tuple[Simulation, JaxInfo, JaxInfo]:
+        """Like ``to_simulation()`` but the gradient monitors are included."""
+        simulation, jax_info = self.to_simulation()
+        sim_fwd, jax_info_fwd = self.make_sim_fwd(simulation=simulation, jax_info=jax_info)
+        return sim_fwd, jax_info_fwd, jax_info
+
+    @staticmethod
+    def get_grad_monitors(input_structures: List[Structure], freq_adjoint: float) -> dict:
         """Return dictionary of gradient monitors for simulation."""
         grad_mnts = []
         grad_eps_mnts = []
-        for index, structure in enumerate(self.input_structures):
+        for index, structure in enumerate(input_structures):
             grad_mnt, grad_eps_mnt = structure.make_grad_monitors(
-                freq=self.freq_adjoint, name=f"grad_mnt_{index}"
+                freq=freq_adjoint, name=f"grad_mnt_{index}"
             )
             grad_mnts.append(grad_mnt)
             grad_eps_mnts.append(grad_eps_mnt)
         return dict(grad_monitors=grad_mnts, grad_eps_monitors=grad_eps_mnts)
 
     def store_vjp(
         self,
         grad_data_fwd: Tuple[FieldData],
         grad_data_adj: Tuple[FieldData],
         grad_eps_data: Tuple[PermittivityData],
     ) -> JaxSimulation:
         """Store the vjp w.r.t. each input_structure as a sim using fwd and adj grad_data."""
 
         input_structures_vjp = []
-        for in_struct, fld_fwd, fld_adj, eps_data in zip(
-            self.input_structures, grad_data_fwd, grad_data_adj, grad_eps_data
-        ):
+        adjoint_info = zip(self.input_structures, grad_data_fwd, grad_data_adj, grad_eps_data)
+
+        for in_struct, fld_fwd, fld_adj, eps_data in adjoint_info:
+
+            freq = float(eps_data.eps_xx.coords["f"])
+            eps_out = self.medium.eps_model(frequency=freq)
+            eps_in = in_struct.medium.eps_model(frequency=freq)
+
             input_structure_vjp = in_struct.store_vjp(
-                fld_fwd, fld_adj, eps_data, sim_bounds=self.bounds
+                grad_data_fwd=fld_fwd,
+                grad_data_adj=fld_adj,
+                grad_data_eps=eps_data,
+                sim_bounds=self.bounds,
+                eps_out=eps_out,
+                eps_in=eps_in,
             )
+
             input_structures_vjp.append(input_structure_vjp)
 
         return self.copy(
             update=dict(
                 input_structures=input_structures_vjp, grad_monitors=(), grad_eps_monitors=()
             )
         )
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     # pylint:disable=too-many-arguments
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         grad_data_eps: PermittivityData,
         sim_bounds: Bound,
+        eps_out: complex,
+        eps_in: complex,
     ) -> JaxStructure:
         """Returns the gradient of the structure parameters given forward and adjoint field data."""
 
         # compute wavelength in material (to use for determining integration points)
         freq = float(grad_data_eps.eps_xx.f)
         wvl_free_space = C_0 / freq
         ref_ind = np.sqrt(np.max(np.real(self.medium.eps_model(freq))))
@@ -74,21 +76,24 @@
 
         geo_vjp = self.geometry.store_vjp(
             grad_data_fwd=grad_data_fwd,
             grad_data_adj=grad_data_adj,
             grad_data_eps=grad_data_eps,
             sim_bounds=sim_bounds,
             wvl_mat=wvl_mat,
+            eps_out=eps_out,
+            eps_in=eps_in,
         )
 
         medium_vjp = self.medium.store_vjp(
             grad_data_fwd=grad_data_fwd,
             grad_data_adj=grad_data_adj,
             sim_bounds=sim_bounds,
             wvl_mat=wvl_mat,
+            inside_fn=self.geometry.inside,
         )
 
         return self.copy(update=dict(geometry=geo_vjp, medium=medium_vjp))
 
     def make_grad_monitors(self, freq: float, name: str) -> FieldMonitor:
         """Return gradient monitor associated with this object."""
         return self.geometry.make_grad_monitors(freq=freq, name=name)
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.2.0/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.2.0/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.2.0/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.2.0/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.2.0/tidy3d/plugins/mode/mode_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ...components.base import Tidy3dBaseModel, cached_property
 from ...components.geometry import Box
 from ...components.simulation import Simulation
 from ...components.grid.grid import Grid
 from ...components.mode import ModeSpec
 from ...components.monitor import ModeSolverMonitor, ModeMonitor
 from ...components.source import ModeSource, SourceTime
-from ...components.types import Direction, FreqArray, Ax, Literal, Axis, Symmetry
+from ...components.types import Direction, FreqArray, Ax, Literal, Axis, Symmetry, PlotScale
 from ...components.types import ArrayComplex3D, ArrayComplex4D, ArrayFloat1D
 from ...components.data.data_array import ModeIndexDataArray, ScalarModeFieldDataArray
 from ...components.data.data_array import FreqModeDataArray
 from ...components.data.sim_data import SimulationData
 from ...components.data.monitor_data import ModeSolverData
 from ...exceptions import ValidationError
 from ...constants import C_0
@@ -278,38 +278,52 @@
         """
         monitor_data = self.data
         new_monitors = list(self.simulation.monitors) + [monitor_data.monitor]
         new_simulation = self.simulation.copy(update=dict(monitors=new_monitors))
         return SimulationData(simulation=new_simulation, data=(monitor_data,))
 
     def _get_epsilon(self, freq: float) -> ArrayComplex4D:
-        """Compute the diagonal components of the epsilon tensor in the plane."""
-
-        eps_xx = self.simulation.epsilon_on_grid(self._solver_grid, "Ex", freq)
-        eps_yy = self.simulation.epsilon_on_grid(self._solver_grid, "Ey", freq)
-        eps_zz = self.simulation.epsilon_on_grid(self._solver_grid, "Ez", freq)
-
-        return np.stack((eps_xx, eps_yy, eps_zz), axis=0)
+        """Compute the epsilon tensor in the plane. Order of components is xx, xy, xz, yx, etc."""
+        eps_keys = ["Ex", "Exy", "Exz", "Eyx", "Ey", "Eyz", "Ezx", "Ezy", "Ez"]
+        eps_tensor = [
+            self.simulation.epsilon_on_grid(self._solver_grid, key, freq) for key in eps_keys
+        ]
+        return np.stack(eps_tensor, axis=0)
 
     def _solver_eps(self, freq: float) -> ArrayComplex4D:
-        """Get the diagonal permittivity in the shape needed to be supplied to the sovler, with the
+        """Get the permittivity tensor in the shape needed to be supplied to the sovler, with the
         normal axis rotated to z."""
 
         # Get diagonal epsilon components in the plane
-        eps_diag = self._get_epsilon(freq)
+        eps_tensor = self._get_epsilon(freq)
 
         # get rid of normal axis
-        eps_diag = np.take(eps_diag, indices=[0], axis=1 + self.normal_axis)
-        eps_diag = np.squeeze(eps_diag, axis=1 + self.normal_axis)
+        eps_tensor = np.take(eps_tensor, indices=[0], axis=1 + self.normal_axis)
+        eps_tensor = np.squeeze(eps_tensor, axis=1 + self.normal_axis)
+
+        # convert to into 3-by-3 representation for easier axis swap
+        flat_shape = np.shape(eps_tensor)  # 9 components flat
+        tensor_shape = [3, 3] + list(flat_shape[1:])  # 3-by-3 matrix
+        eps_tensor = eps_tensor.reshape(tensor_shape)
 
         # swap axes to plane coordinates (normal_axis goes to z)
-        eps_zz, (eps_xx, eps_yy) = self.plane.pop_axis(eps_diag, axis=self.normal_axis)
+        if self.normal_axis == 0:
+            # swap x and y
+            eps_tensor[[0, 1], :, ...] = eps_tensor[[1, 0], :, ...]
+            eps_tensor[:, [0, 1], ...] = eps_tensor[:, [1, 0], ...]
+        if self.normal_axis <= 1:
+            # swap x (normal_axis==0) or y (normal_axis==1) and z
+            eps_tensor[[1, 2], :, ...] = eps_tensor[[2, 1], :, ...]
+            eps_tensor[:, [1, 2], ...] = eps_tensor[:, [2, 1], ...]
+
+        # back to "flat" representation
+        eps_tensor = eps_tensor.reshape(flat_shape)
 
         # construct eps to feed to mode solver
-        return np.stack((eps_xx, eps_yy, eps_zz), axis=0)
+        return eps_tensor
 
     def _solve_all_freqs(
         self,
         coords: Tuple[ArrayFloat1D, ArrayFloat1D],
         symmetry: Tuple[Symmetry, Symmetry],
     ) -> Tuple[List[float], List[Dict[str, ArrayComplex4D]]]:
         """Call the mode solver at all requested frequencies."""
@@ -548,14 +562,15 @@
         )
 
     # pylint:disable=too-many-arguments
     def plot_field(
         self,
         field_name: str,
         val: Literal["real", "imag", "abs"] = "real",
+        scale: PlotScale = "lin",
         eps_alpha: float = 0.2,
         robust: bool = True,
         vmin: float = None,
         vmax: float = None,
         ax: Ax = None,
         **sel_kwargs,
     ) -> Ax:
@@ -598,14 +613,15 @@
         """
 
         sim_data = self.sim_data
         sim_data.plot_field(
             field_monitor_name=MODE_MONITOR_NAME,
             field_name=field_name,
             val=val,
+            scale=scale,
             eps_alpha=eps_alpha,
             robust=robust,
             vmin=vmin,
             vmax=vmax,
             ax=ax,
             **sel_kwargs,
         )
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/mode/solver.py` & `tidy3d-2.2.0/tidy3d/plugins/mode/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     ) -> Tuple[Numpy, Numpy]:
         """Solve for the modes of a waveguide cross section.
 
         Parameters
         ----------
         eps_cross : array_like or tuple of array_like
             Either a single 2D array defining the relative permittivity in the cross-section,
-            or three 2D arrays defining the permittivity at the Ex, Ey, and Ez locations
-            of the Yee grid.
+            or nine 2D arrays defining the permittivity at the Ex, Ey, and Ez locations
+            of the Yee grid in the order xx, xy, xz, yx, yy, yz, zx, zy, zz.
         coords : List[Numpy]
             Two 1D arrays with each with size one larger than the corresponding axis of
             ``eps_cross``.
             Defines a (potentially non-uniform) Cartesian grid on which the modes are computed.
         freq : float
             (Hertz) Frequency at which the eigenmodes are computed.
         mode_spec : ModeSpec
@@ -65,17 +65,19 @@
         bend_axis = mode_spec.bend_axis
         angle_theta = mode_spec.angle_theta
         angle_phi = mode_spec.angle_phi
         omega = 2 * np.pi * freq
         k0 = omega / C_0
 
         if isinstance(eps_cross, Numpy):
-            eps_xx, eps_yy, eps_zz = eps_cross
-        elif len(eps_cross) == 3:
-            eps_xx, eps_yy, eps_zz = [np.copy(e) for e in eps_cross]
+            eps_xx, eps_xy, eps_xz, eps_yx, eps_yy, eps_yz, eps_zx, eps_zy, eps_zz = eps_cross
+        elif len(eps_cross) == 9:
+            eps_xx, eps_xy, eps_xz, eps_yx, eps_yy, eps_yz, eps_zx, eps_zy, eps_zz = [
+                np.copy(e) for e in eps_cross
+            ]
         else:
             raise ValueError("Wrong input to mode solver pemittivity!")
 
         Nx, Ny = eps_xx.shape
         N = eps_xx.size
 
         if len(coords[0]) != Nx + 1 or len(coords[1]) != Ny + 1:
@@ -84,17 +86,20 @@
 
         """We work with full tensorial epsilon in mu to handle the most general cases that can
         be introduced by coordinate transformations. In the solver, we distinguish the case when
         these tensors are still diagonal, in which case the matrix for diagonalization has shape
         (2N, 2N), and the full tensorial case, in which case it has shape (4N, 4N)."""
         eps_tensor = np.zeros((3, 3, N), dtype=np.complex128)
         mu_tensor = np.zeros((3, 3, N), dtype=np.complex128)
-        for dim, eps in enumerate([eps_xx, eps_yy, eps_zz]):
-            eps_tensor[dim, dim, :] = eps.ravel()
-            mu_tensor[dim, dim, :] = 1.0
+        for row, eps_row in enumerate(
+            [[eps_xx, eps_xy, eps_xz], [eps_yx, eps_yy, eps_yz], [eps_zx, eps_zy, eps_zz]]
+        ):
+            mu_tensor[row, row, :] = 1.0
+            for col, eps in enumerate(eps_row):
+                eps_tensor[row, col, :] = eps.ravel()
 
         # Get Jacobian of all coordinate transformations. Initialize as identity (same as mu so far)
         jac_e = np.real(np.copy(mu_tensor))
         jac_h = np.real(np.copy(mu_tensor))
 
         if bend_radius is not None:
             new_coords, jac_e, jac_h = radial_transform(new_coords, bend_radius, bend_axis)
@@ -105,15 +110,15 @@
             jac_h = np.einsum("ij...,jp...->ip...", jac_h_tmp, jac_h)
 
         """We also need to keep track of the transformation of the k-vector. This is
         the eigenvalue of the momentum operator assuming some sort of translational invariance and is
         different from just the transformation of the derivative operator. For example, in a bent
         waveguide, there is strictly speaking no k-vector in the original coordinates as the system
         is not translationally invariant there. However, if we define kz = R k_phi, then the
-        effective index approaches that for a straight-waveguide in the limit of infinite radius. 
+        effective index approaches that for a straight-waveguide in the limit of infinite radius.
         Since we use w = R phi in the radial_transform, there is nothing else neede in the k transform.
         For the angled_transform, the transformation between k-vectors follows from writing the field as
         E' exp(i k_p w) in transformed coordinates, and identifying this with
         E exp(i k_x x + i k_y y + i k_z z) in the original ones."""
         kxy = np.cos(angle_theta) ** 2
         kz = np.cos(angle_theta) * np.sin(angle_theta)
         kp_to_k = np.array([kxy * np.sin(angle_phi), kxy * np.cos(angle_phi), kz])
@@ -233,14 +238,23 @@
             Magnetic field of the eigenmodes, shape (3, N, num_modes).
         neff : np.ndarray
             Real part of the effective index, shape (num_modes, ).
         keff : np.ndarray
             Imaginary part of the effective index, shape (num_modes, ).
         """
 
+        # use a high-conductivity model for locations associated with a PEC
+        def conductivity_model_for_pec(eps, threshold=0.9 * pec_val):
+            """PEC entries associated with 'eps' are converted to a high-conductivity model."""
+            eps = eps.astype(complex)
+            eps[eps <= threshold] = 1 + 1j * np.abs(pec_val)
+            return eps
+
+        eps_tensor = conductivity_model_for_pec(eps_tensor)
+
         # Determine if ``eps`` and ``mu`` are diagonal or tensorial
         off_diagonals = (np.ones((3, 3)) - np.eye(3)).astype(bool)
         eps_offd = np.abs(eps_tensor[off_diagonals])
         mu_offd = np.abs(mu_tensor[off_diagonals])
         is_tensorial = False
         if np.any(eps_offd > TOL_TENSORIAL) or np.any(mu_offd > TOL_TENSORIAL):
             is_tensorial = True
@@ -287,50 +301,104 @@
 
     @classmethod
     def solver_diagonal(
         cls, eps, mu, der_mats, num_modes, vec_init, neff_guess
     ):  # pylint:disable=too-many-arguments
         """EM eigenmode solver assuming ``eps`` and ``mu`` are diagonal everywhere."""
 
+        # code associated with these options is included below in case it's useful in the future
+        enable_incidence_matrices = False
+        enable_preconditioner = False
+        analyze_conditioning = False
+
+        def incidence_matrix_for_pec(eps_vec, threshold=0.9 * np.abs(pec_val)):
+            """Incidence matrix indicating non-PEC entries associated with 'eps_vec'."""
+            nnz = eps_vec[np.abs(eps_vec) < threshold]
+            eps_nz = eps_vec.copy()
+            eps_nz[np.abs(eps_vec) >= threshold] = 0
+            rows = np.arange(0, len(nnz))
+            cols = np.argwhere(eps_nz).flatten()
+            dnz = sp.csr_matrix(([1] * len(nnz), (rows, cols)), shape=(len(rows), len(eps_vec)))
+            return dnz
+
         mode_solver_type = "diagonal"
         N = eps.shape[-1]
 
         # Unpack eps, mu and derivatives
         eps_xx = eps[0, 0, :]
         eps_yy = eps[1, 1, :]
         eps_zz = eps[2, 2, :]
         mu_xx = mu[0, 0, :]
         mu_yy = mu[1, 1, :]
         mu_zz = mu[2, 2, :]
         dxf, dxb, dyf, dyb = der_mats
 
+        def any_pec(eps_vec, threshold=0.9 * np.abs(pec_val)):
+            """Check if there are any PEC values in the given permittivity array."""
+            return np.any(np.abs(eps_vec) >= threshold)
+
+        if np.any(any_pec(i) for i in [eps_xx, eps_yy, eps_zz]):
+            enable_preconditioner = True
+
         # Compute the matrix for diagonalization
         inv_eps_zz = sp.spdiags(1 / eps_zz, [0], N, N)
         inv_mu_zz = sp.spdiags(1 / mu_zz, [0], N, N)
+
+        if enable_incidence_matrices:
+            dnz_xx, dnz_yy, dnz_zz = [incidence_matrix_for_pec(i) for i in [eps_xx, eps_yy, eps_zz]]
+            dnz = sp.block_diag((dnz_xx, dnz_yy), format="csr")
+            inv_eps_zz = (dnz_zz.T) * dnz_zz * inv_eps_zz * (dnz_zz.T) * dnz_zz
+
         p11 = -dxf.dot(inv_eps_zz).dot(dyb)
         p12 = dxf.dot(inv_eps_zz).dot(dxb) + sp.spdiags(mu_yy, [0], N, N)
         p21 = -dyf.dot(inv_eps_zz).dot(dyb) - sp.spdiags(mu_xx, [0], N, N)
         p22 = dyf.dot(inv_eps_zz).dot(dxb)
         q11 = -dxb.dot(inv_mu_zz).dot(dyf)
         q12 = dxb.dot(inv_mu_zz).dot(dxf) + sp.spdiags(eps_yy, [0], N, N)
         q21 = -dyb.dot(inv_mu_zz).dot(dyf) - sp.spdiags(eps_xx, [0], N, N)
         q22 = dyb.dot(inv_mu_zz).dot(dxf)
 
         pmat = sp.bmat([[p11, p12], [p21, p22]])
         qmat = sp.bmat([[q11, q12], [q21, q22]])
+
         mat = pmat.dot(qmat)
 
+        if enable_incidence_matrices:
+            mat = dnz * mat * dnz.T  # pylint: disable=used-before-assignment
+            vec_init = dnz * vec_init  # pylint: disable=used-before-assignment
+
+        if enable_preconditioner:
+            precon = sp.diags(1 / mat.diagonal())
+            mat = mat * precon
+        else:
+            precon = None
+
+        if analyze_conditioning:
+            aca = mat.conjugate().T * mat
+            aac = mat * mat.conjugate().T
+            diff = aca - aac
+            print(spl.norm(diff, ord=np.inf), spl.norm(aca, ord=np.inf), spl.norm(aac, ord=np.inf))
+            print(spl.norm(diff, ord="fro"), spl.norm(aca, ord="fro"), spl.norm(aac, ord="fro"))
+
         # Call the eigensolver. The eigenvalues are -(neff + 1j * keff)**2
         vals, vecs = cls.solver_eigs(
             mat,
             num_modes,
             vec_init,
             guess_value=-(neff_guess**2),
             mode_solver_type=mode_solver_type,
+            M=precon,
         )
+
+        if enable_preconditioner:
+            vecs = precon * vecs
+
+        if enable_incidence_matrices:
+            vecs = dnz.T * vecs  # pylint: disable=used-before-assignment
+
         neff, keff = cls.eigs_to_effective_index(vals, mode_solver_type)
 
         # Sort by descending neff
         sort_inds = np.argsort(neff)[::-1]
         neff = neff[sort_inds]
         keff = keff[sort_inds]
         vecs = vecs[:, sort_inds]
@@ -462,28 +530,30 @@
         # The minus sign here is suspicious, need to check how modes are used in Mode objects
         H *= -1j / ETA_0
 
         return E, H, neff, keff
 
     @classmethod
     def solver_eigs(
-        cls, mat, num_modes, vec_init, guess_value=1.0, **kwargs
-    ):  # pylint:disable=unused-argument
+        cls, mat, num_modes, vec_init, guess_value=1.0, M=None, **kwargs
+    ):  # pylint:disable=unused-argument, too-many-arguments
         """Find ``num_modes`` eigenmodes of ``mat`` cloest to ``guess_value``.
 
         Parameters
         ----------
         mat : scipy.sparse matrix
             Square matrix for diagonalization.
         num_modes : int
             Number of eigenmodes to compute.
         guess_value : float, optional
         """
 
-        values, vectors = spl.eigs(mat, k=num_modes, sigma=guess_value, tol=TOL_EIGS, v0=vec_init)
+        values, vectors = spl.eigs(
+            mat, k=num_modes, sigma=guess_value, tol=TOL_EIGS, v0=vec_init, M=M
+        )
         return values, vectors
 
     @classmethod
     def isinstance_complex(cls, vec_or_mat, tol=TOL_COMPLEX):
         """Check if a numpy array or scipy csr_matrix has complex component by looking at
         norm(x.imag)/norm(x)>TOL_COMPLEX
```

### Comparing `tidy3d-2.1.1/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.2.0/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.2.0/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.2.0/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.2.0/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.2.0/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/updater.py` & `tidy3d-2.2.0/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/auth.py` & `tidy3d-2.2.0/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/cacert.pem` & `tidy3d-2.2.0/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/cli/app.py` & `tidy3d-2.2.0/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/cli/migrate.py` & `tidy3d-2.2.0/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/config.py` & `tidy3d-2.2.0/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/container.py` & `tidy3d-2.2.0/tidy3d/web/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,40 @@
         "otherwise uses default for the current front end version.",
     )
 
     verbose: bool = pd.Field(
         True, title="Verbose", description="Whether to print info messages and progressbars."
     )
 
+    simulation_type: str = pd.Field(
+        "tidy3d",
+        title="Simulation Type",
+        description="Type of simulation, used internally only.",
+    )
+
+    parent_tasks: Tuple[TaskId, ...] = pd.Field(
+        None, title="Parent Tasks", description="Tuple of parent task ids, used internally only."
+    )
+
     task_id: TaskId = pd.Field(
         None,
         title="Task Id",
         description="Task ID number, set when the task is uploaded, leave as None.",
     )
 
+    _upload_fields = (
+        "simulation",
+        "task_name",
+        "folder_name",
+        "callback_url",
+        "verbose",
+        "simulation_type",
+        "parent_tasks",
+    )
+
     def run(self, path: str = DEFAULT_DATA_PATH) -> SimulationData:
         """run :class:`Job` all the way through and return data.
 
         Parameters
         ----------
         path_dir : str = "./simulation_data.hdf5"
             Base directory where data will be downloaded, by default current working directory.
@@ -80,28 +100,29 @@
             Dictionary mapping task name to :class:`.SimulationData` for :class:`Job`.
         """
 
         self.start()
         self.monitor()
         return self.load(path=path)
 
-    @pd.validator("task_id", always=True)
-    def _upload(cls, val, values) -> None:
+    @pd.root_validator()
+    def _upload(cls, values) -> None:
         """Upload simulation to server without running."""
-        if val is not None:
-            return val
 
-        task_id = web.upload(
-            simulation=values.get("simulation"),
-            task_name=values.get("task_name"),
-            folder_name=values.get("folder_name"),
-            callback_url=values.get("callback_url"),
-            verbose=values.get("verbose"),
-        )
-        return task_id
+        # task_id already present, don't re-upload
+        if values.get("task_id") is not None:
+            return values
+
+        # upload kwargs with all fields except task_id
+        upload_kwargs = {key: values.get(key) for key in cls._upload_fields}
+        task_id = web.upload(**upload_kwargs)
+
+        # then set the task_id and return
+        values["task_id"] = task_id
+        return values
 
     def get_info(self) -> TaskInfo:
         """Return information about a :class:`Job`.
 
         Returns
         -------
         :class:`TaskInfo`
@@ -264,14 +285,34 @@
     solver_version: str = pd.Field(
         None,
         title="Solver Version",
         description_str="Custom solver version to use, "
         "otherwise uses default for the current front end version.",
     )
 
+    callback_url: str = pd.Field(
+        None,
+        title="Callback URL",
+        description="Http PUT url to receive simulation finish event. "
+        "The body content is a json file with fields "
+        "``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.",
+    )
+
+    simulation_type: str = pd.Field(
+        "tidy3d",
+        title="Simulation Type",
+        description="Type of each simulation in the batch, used internally only.",
+    )
+
+    parent_tasks: Dict[str, Tuple[TaskId, ...]] = pd.Field(
+        None,
+        title="Parent Tasks",
+        description="Collection of parent task ids for each job in batch, used internally only.",
+    )
+
     jobs: Dict[TaskName, Job] = pd.Field(
         None,
         title="Simulations",
         description="Mapping of task names to individual Job object for each task in the batch. "
         "Set by ``Batch.upload``, leave as None.",
     )
 
@@ -320,25 +361,30 @@
         Note
         ----
         To start the simulations running, must call :meth:`Batch.start` after uploaded.
         """
         if val is not None:
             return val
 
-        verbose = bool(values.get("verbose"))
+        # the type of job to upload (to generalize to subclasses)
+        JobType = cls.__fields__["jobs"].type_  # pylint:disable=invalid-name
+        parent_tasks = values.get("parent_tasks")
 
+        verbose = bool(values.get("verbose"))
         jobs = {}
         for task_name, simulation in values.get("simulations").items():
-            job = Job(
-                simulation=simulation,
-                task_name=task_name,
-                folder_name=values.get("folder_name"),
-                solver_version=values.get("solver_version"),
-                verbose=verbose,
-            )
+
+            # pylint:disable=protected-access
+            upload_kwargs = {key: values.get(key) for key in JobType._upload_fields}
+            upload_kwargs["task_name"] = task_name
+            upload_kwargs["simulation"] = simulation
+            upload_kwargs["verbose"] = verbose
+            if parent_tasks and task_name in parent_tasks:
+                upload_kwargs["parent_tasks"] = parent_tasks[task_name]
+            job = JobType(**upload_kwargs)
             jobs[task_name] = job
         return jobs
 
     def get_info(self) -> Dict[TaskName, TaskInfo]:
         """Get information about each task in the :class:`Batch`.
 
         Returns
```

### Comparing `tidy3d-2.1.1/tidy3d/web/environment.py` & `tidy3d-2.2.0/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/http_management.py` & `tidy3d-2.2.0/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/httputils.py` & `tidy3d-2.2.0/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/material_fitter.py` & `tidy3d-2.2.0/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/material_libray.py` & `tidy3d-2.2.0/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/s3utils.py` & `tidy3d-2.2.0/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/simulation_task.py` & `tidy3d-2.2.0/tidy3d/web/simulation_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,32 +150,50 @@
         None,
         title="Callback URL",
         description="Http PUT url to receive simulation finish event. "
         "The body content is a json file with fields "
         "``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.",
     )
 
+    # simulation_type: str = pd.Field(
+    #     None,
+    #     title="Simulation Type",
+    #     description="Type of simulation, used internally only.",
+    # )
+
+    # parent_tasks: Tuple[TaskId, ...] = pd.Field(
+    #     None,
+    #     title="Parent Tasks",
+    #     description="List of parent task ids for the simulation, used internally only."
+    # )
+
     @pd.root_validator(pre=True)
     def _error_if_jax_sim(cls, values):
         """Raise error if user tries to submit simulation that's a JaxSimulation."""
         sim = values.get("simulation")
         if sim is None:
             return values
         if "JaxSimulation" in str(type(sim)):
             raise ValueError(
                 "'JaxSimulation' not compatible with regular webapi functions. "
                 "Either convert it to Simulation with 'jax_sim.to_simulation()[0]' or use "
                 "the 'adjoint.run' function to run JaxSimulations."
             )
         return values
 
-    # pylint: disable=arguments-differ
+    # pylint: disable=arguments-differ,too-many-arguments
     @classmethod
     def create(
-        cls, simulation: Simulation, task_name: str, folder_name="default", callback_url=None
+        cls,
+        simulation: Simulation,
+        task_name: str,
+        folder_name="default",
+        call_back_url=None,
+        simulation_type: str = "tidy3d",
+        parent_tasks: List[str] = None,
     ) -> SimulationTask:
         """Create a new task on the server.
 
         Parameters
         ----------
         simulation: :class".Simulation"
             The :class:`.Simulation` will be uploaded to server in the submitting phase.
@@ -184,14 +202,18 @@
         task_name: str
             The name of the task.
         folder_name: str,
             The name of the folder to store the task. Default is "default".
         callback_url: str
             Http PUT url to receive simulation finish event. The body content is a json file with
             fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
+        simulation_type : str
+            Type of simulation being uploaded.
+        parent_tasks : List[str]
+            List of related task ids.
 
         Returns
         -------
         :class:`SimulationTask`
             :class:`SimulationTask` object containing info about status, size,
              credits of task and others.
         """
@@ -200,15 +222,20 @@
             folder = Folder.get(folder_name)
         if not folder:
             folder = Folder.create(folder_name)
         FOLDER_CACHE[folder_name] = folder
 
         resp = http.post(
             f"tidy3d/projects/{folder.folder_id}/tasks",
-            {"taskName": task_name, "callbackUrl": callback_url},
+            {
+                "taskName": task_name,
+                "call_back_url": call_back_url,
+                "simulationType": simulation_type,
+                "parentTasks": parent_tasks,
+            },
         )
 
         return SimulationTask(**resp, simulation=simulation, folder=folder)
 
     # pylint: disable=arguments-differ
     @classmethod
     def get(cls, task_id: str) -> SimulationTask:
@@ -224,14 +251,33 @@
         :class:`.SimulationTask`
             :class:`.SimulationTask` object containing info about status,
              size, credits of task and others.
         """
         resp = http.get(f"tidy3d/tasks/{task_id}/detail")
         return SimulationTask(**resp) if resp else None
 
+    @classmethod
+    def get_running_tasks(cls) -> List[SimulationTask]:
+        """Get a list of running tasks from the server"
+
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        List[:class:`.SimulationTask`]
+            :class:`.SimulationTask` object containing info about status,
+             size, credits of task and others.
+        """
+        resp = http.get("tidy3d/py/tasks")
+        if not resp:
+            return []
+        return parse_obj_as(List[SimulationTask], resp)
+
     def delete(self):
         """Delete current task from server."""
         if not self.task_id:
             raise ValueError("Task id not found.")
         http.delete(f"tidy3d/tasks/{self.task_id}")
 
     def get_simulation(self) -> Optional[Simulation]:
```

### Comparing `tidy3d-2.1.1/tidy3d/web/task.py` & `tidy3d-2.2.0/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/types.py` & `tidy3d-2.2.0/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.1/tidy3d/web/webapi.py` & `tidy3d-2.2.0/tidy3d/web/webapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Provides lowest level, user-facing interface to server."""
 
 import os
 import time
 from datetime import datetime, timedelta
 from typing import List, Dict, Callable
+from functools import wraps
+
+from requests import HTTPError
+from requests.exceptions import ConnectionError as ConnErr
+from urllib3.exceptions import NewConnectionError
 
 import pytz
 from rich.console import Console
 from rich.progress import Progress
 
 from .environment import Env
 from .simulation_task import SimulationTask, SIM_FILE_HDF5, Folder
@@ -21,20 +26,53 @@
 
 # time between checking task status
 REFRESH_TIME = 0.3
 
 # time between checking run status
 RUN_REFRESH_TIME = 1.0
 
-TOTAL_DOTS = 3
-
 # file names when uploading to S3
 SIM_FILE_JSON = "simulation.json"
 
+# number of seconds to keep re-trying connection before erroring
+CONNECTION_RETRY_TIME = 30
+
+
+def wait_for_connection(decorated_fn=None, wait_time_sec: float = CONNECTION_RETRY_TIME):
+    """Causes function to ignore connection errors and retry for ``wait_time_sec`` secs."""
+
+    def decorator(web_fn):
+        """Decorator returned by @wait_for_connection()"""
+
+        @wraps(web_fn)
+        def web_fn_wrapped(*args, **kwargs):
+            """Function to return including connection waiting."""
+            time_start = time.time()
+            warned_previously = False
+
+            while (time.time() - time_start) < wait_time_sec:
+                try:
+                    return web_fn(*args, **kwargs)
+                except (ConnErr, ConnectionError, NewConnectionError):
+                    if not warned_previously:
+                        log.warning(f"No connection: Retrying for {wait_time_sec} seconds.")
+                        warned_previously = True
+                    time.sleep(REFRESH_TIME)
+
+            raise WebError("No internet connection: giving up on connection waiting.")
 
+        return web_fn_wrapped
+
+    if decorated_fn:
+        return decorator(decorated_fn)
+
+    return decorator
+
+
+@wait_for_connection
 def run(  # pylint:disable=too-many-arguments
     simulation: Simulation,
     task_name: str,
     folder_name: str = "default",
     path: str = "simulation_data.hdf5",
     callback_url: str = None,
     verbose: bool = True,
@@ -90,21 +128,24 @@
     )
     monitor(task_id, verbose=verbose)
     return load(
         task_id=task_id, path=path, verbose=verbose, progress_callback=progress_callback_download
     )
 
 
+@wait_for_connection
 def upload(  # pylint:disable=too-many-locals,too-many-arguments
     simulation: Simulation,
     task_name: str,
     folder_name: str = "default",
     callback_url: str = None,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
+    simulation_type: str = "tidy3d",
+    parent_tasks: List[str] = None,
 ) -> TaskId:
     """Upload simulation to server, but do not start running :class:`.Simulation`.
 
     Parameters
     ----------
     simulation : :class:`.Simulation`
         Simulation to upload to server.
@@ -115,43 +156,50 @@
     callback_url : str = None
         Http PUT url to receive simulation finish event. The body content is a json file with
         fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
     verbose : bool = True
         If `True`, will print progressbars and status, otherwise, will run silently.
     progress_callback : Callable[[float], None] = None
         Optional callback function called when uploading file with ``bytes_in_chunk`` as argument.
+    simulation_type : str
+        Type of simulation being uploaded.
+    parent_tasks : List[str]
+        List of related task ids.
 
     Returns
     -------
     str
         Unique identifier of task on server.
 
     Note
     ----
     To start the simulation running, must call :meth:`start` after uploaded.
     """
 
     simulation.validate_pre_upload()
     log.debug("Creating task.")
 
-    task = SimulationTask.create(simulation, task_name, folder_name, callback_url)
+    task = SimulationTask.create(
+        simulation, task_name, folder_name, callback_url, simulation_type, parent_tasks
+    )
     if verbose:
         console = Console()
         console.log(f"Created task '{task_name}' with task_id '{task.task_id}'.")
         url = f"https://tidy3d.simulation.cloud/workbench?taskId={task.task_id}"
         console.log(f"View task using web UI at [link={url}]'{url}'[/link].")
     task.upload_simulation(verbose=verbose, progress_callback=progress_callback)
 
     # log the url for the task in the web UI
     log.debug(
         f"{Env.current.website_endpoint}/folders/{task.folder.folder_id}/tasks/{task.task_id}"
     )
     return task.task_id
 
 
+@wait_for_connection
 def get_info(task_id: TaskId) -> TaskInfo:
     """Return information about a task.
 
     Parameters
     ----------
     task_id : str
         Unique identifier of task on server.  Returned by :meth:`upload`.
@@ -163,14 +211,15 @@
     """
     task = SimulationTask.get(task_id)
     if not task:
         raise ValueError("Task not found.")
     return TaskInfo(**{"taskId": task.task_id, **task.dict()})
 
 
+@wait_for_connection
 def start(
     task_id: TaskId,
     solver_version: str = None,
     worker_group: str = None,
 ) -> None:
     """Start running the simulation associated with task.
 
@@ -190,14 +239,15 @@
     """
     task = SimulationTask.get(task_id)
     if not task:
         raise ValueError("Task not found.")
     task.submit(solver_version=solver_version, worker_group=worker_group)
 
 
+@wait_for_connection
 def get_run_info(task_id: TaskId):
     """Gets the % done and field_decay for a running task.
 
     Parameters
     ----------
     task_id : str
         Unique identifier of task on server.  Returned by :meth:`upload`.
@@ -340,14 +390,15 @@
                     console.log(f"status = {status}")
                 time.sleep(REFRESH_TIME)
     else:
         while get_status() not in break_statuses:
             time.sleep(REFRESH_TIME)
 
 
+@wait_for_connection
 def download(
     task_id: TaskId,
     path: str = "simulation_data.hdf5",
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> None:
     """Download results of task and log to file.
@@ -364,14 +415,15 @@
         Optional callback function called when downloading file with ``bytes_in_chunk`` as argument.
 
     """
     task = SimulationTask(taskId=task_id)
     task.get_simulation_hdf5(path, verbose=verbose, progress_callback=progress_callback)
 
 
+@wait_for_connection
 def download_json(
     task_id: TaskId,
     path: str = SIM_FILE_JSON,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> None:
     """Download the `.json` file associated with the :class:`.Simulation` of a given task.
@@ -389,14 +441,15 @@
 
     """
 
     task = SimulationTask(taskId=task_id)
     task.get_simulation_json(path, verbose=verbose, progress_callback=progress_callback)
 
 
+@wait_for_connection
 def download_hdf5(
     task_id: TaskId,
     path: str = SIM_FILE_HDF5,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> None:
     """Download the `.hdf5` file associated with the :class:`.Simulation` of a given task.
@@ -414,14 +467,15 @@
 
     """
 
     task = SimulationTask(taskId=task_id)
     task.get_simulation_hdf5(path, verbose=verbose, progress_callback=progress_callback)
 
 
+@wait_for_connection
 def load_simulation(
     task_id: TaskId,
     path: str = SIM_FILE_JSON,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> Simulation:
     """Download the `.json` file of a task and load the associated :class:`.Simulation`.
@@ -445,14 +499,15 @@
 
     # task = SimulationTask.get(task_id)
     task = SimulationTask(taskId=task_id)
     task.get_simulation_json(path, verbose=verbose, progress_callback=progress_callback)
     return Simulation.from_file(path)
 
 
+@wait_for_connection
 def download_log(
     task_id: TaskId,
     path: str = "tidy3d.log",
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> None:
     """Download the tidy3d log file associated with a task.
@@ -472,14 +527,15 @@
     ----
     To load downloaded results into data, call :meth:`load` with option `replace_existing=False`.
     """
     task = SimulationTask(taskId=task_id)
     task.get_log(path, verbose=verbose, progress_callback=progress_callback)
 
 
+@wait_for_connection
 def load(
     task_id: TaskId,
     path: str = "simulation_data.hdf5",
     replace_existing: bool = True,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
 ) -> SimulationData:
@@ -521,14 +577,15 @@
             f"is greater than the simulation shutoff threshold of {shutoff_value}. "
             "Consider simulation again with large run_time duration for more accurate results."
         )
 
     return sim_data
 
 
+@wait_for_connection
 def delete(task_id: TaskId) -> TaskInfo:
     """Delete server-side data associated with task.
 
     Parameters
     ----------
     task_id : str
         Unique identifier of task on server.  Returned by :meth:`upload`.
@@ -541,14 +598,15 @@
 
     # task = SimulationTask.get(task_id)
     task = SimulationTask(taskId=task_id)
     task.delete()
     return TaskInfo(**{"taskId": task.task_id, **task.dict()})
 
 
+@wait_for_connection
 def delete_old(
     days_old: int = 100,
     folder: str = "default",
 ) -> int:
     """Delete all tasks older than a given amount of days.
 
     Parameters
@@ -575,14 +633,15 @@
     )
     for task in tasks:
         task.delete()
     return len(tasks)
 
 
 # TODO: make this return a list of TaskInfo instead?
+@wait_for_connection
 def get_tasks(
     num_tasks: int = None, order: Literal["new", "old"] = "new", folder: str = "default"
 ) -> List[Dict]:
     """Get a list with the metadata of the last ``num_tasks`` tasks.
 
     Parameters
     ----------
@@ -605,14 +664,15 @@
     elif order == "old":
         tasks = sorted(tasks, key=lambda t: t.created_at)
     if num_tasks is not None:
         tasks = tasks[:num_tasks]
     return [task.dict() for task in tasks]
 
 
+@wait_for_connection
 def estimate_cost(task_id: str) -> float:
     """Compute the maximum FlexCredit charge for a given task.
 
     Parameters
     ----------
     task_id : str
         Unique identifier of task on server.  Returned by :meth:`upload`.
@@ -647,14 +707,15 @@
         log.warning(
             "Could not get estimated cost! It will be reported in preprocessing upon "
             "simulation run."
         )
     return flex_unit
 
 
+@wait_for_connection
 def real_cost(task_id: str) -> float:
     """Get the billed cost for given task after it has been run.
 
     Note
     ----
         The billed cost may not be immediately available when the task status is set to ``success``,
         but should be available shortly after.
@@ -663,7 +724,25 @@
     flex_unit = task_info.realFlexUnit
     if not flex_unit:
         log.warning(
             f"Billed FlexCredit for task '{task_id}' is not available. If the task has been "
             "successfully run, it should be available shortly."
         )
     return flex_unit
+
+
+@wait_for_connection
+def test() -> None:
+    """Confirm whether Tidy3D authentication is configured. Raises exception if not."""
+    try:
+        # note, this is a little slow, but the only call that doesn't require providing a task id.
+        get_tasks(num_tasks=0)
+        console = Console()
+        console.log("Authentication configured successfully!")
+    except (WebError, HTTPError) as e:
+        url = "https://docs.flexcompute.com/projects/tidy3d/en/latest/quickstart.html"
+
+        raise WebError(
+            "Tidy3D not configured correctly. Please refer to our documentation for installation "
+            "instructions at "
+            f"[link={url}]'{url}'[/link]."
+        ) from e
```

### Comparing `tidy3d-2.1.1/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.2.0/tidy3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.1.1
+Version: 2.2.0
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.1.1/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.2.0/tidy3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 tidy3d/components/geometry.py
 tidy3d/components/medium.py
 tidy3d/components/mode.py
 tidy3d/components/monitor.py
 tidy3d/components/simulation.py
 tidy3d/components/source.py
 tidy3d/components/structure.py
+tidy3d/components/transformation.py
 tidy3d/components/types.py
 tidy3d/components/validators.py
 tidy3d/components/viz.py
 tidy3d/components/data/__init__.py
 tidy3d/components/data/data_array.py
 tidy3d/components/data/dataset.py
 tidy3d/components/data/monitor_data.py
```

### Comparing `tidy3d-2.1.1/tidy3d.egg-info/requires.txt` & `tidy3d-2.2.0/tidy3d.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 rich<12.6.0
 matplotlib
 shapely>=2.0
 pydantic<2.0.0,>=1.10.0
 PyYAML
 dask
 toml
-nest_asyncio
 boto3==1.23.1
 requests
 pyjwt
 click==8.0.3
 responses
 
 [dev]
```

