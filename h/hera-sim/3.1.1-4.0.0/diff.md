# Comparing `tmp/hera_sim-3.1.1.tar.gz` & `tmp/hera_sim-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_sim-3.1.1.tar", last modified: Thu Feb 23 20:59:19 2023, max compression
+gzip compressed data, was "hera_sim-4.0.0.tar", last modified: Mon May 22 20:28:31 2023, max compression
```

## Comparing `hera_sim-3.1.1.tar` & `hera_sim-4.0.0.tar`

### file list

```diff
@@ -1,140 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.937856 hera_sim-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.901854 hera_sim-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-23 20:59:09.000000 hera_sim-3.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-23 20:59:09.000000 hera_sim-3.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-02-23 20:59:09.000000 hera_sim-3.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-23 20:59:09.000000 hera_sim-3.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 20:59:09.000000 hera_sim-3.1.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-23 20:59:09.000000 hera_sim-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-23 20:59:19.937856 hera_sim-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-02-23 20:59:09.000000 hera_sim-3.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 20:59:09.000000 hera_sim-3.1.1/ci/tests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/config_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-23 20:59:09.000000 hera_sim-3.1.1/config_examples/simulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-23 20:59:09.000000 hera_sim-3.1.1/config_examples/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/notes_for_developers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.913854 hera_sim-3.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.925855 hera_sim-3.1.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/end_to_end_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/hera_sim_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/hera_sim_defaults.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/hera_sim_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/hera_sim_tour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/hera_sim_vis_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/mutual_coupling_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/polybeam_simulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials/visibility_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-23 20:59:09.000000 hera_sim-3.1.1/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.925855 hera_sim-3.1.1/hera_sim/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/__yaml_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    41370 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    48520 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.929855 hera_sim-3.1.1/hera_sim/config/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/config/H1C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/config/H2C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/config/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.929855 hera_sim-3.1.1/hera_sim/data/
--rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/H37_FR_Filters_small.npz
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H1C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H1C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H2C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H2C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_LAT_LON_ALT.npy
--rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_Tsky_Reformatted.npz
--rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/HERA_Tsky_vs_LST.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.905854 hera_sim-3.1.1/hera_sim/data/tutorials_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.933856 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.933856 hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/eor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    60722 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    63062 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.937856 hera_sim-3.1.1/hera_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_eor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_sim_red_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_simulate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19978 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/test_yaml_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.937856 hera_sim-3.1.1/hera_sim/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/tests/testdata/healvis_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24738 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.937856 hera_sim-3.1.1/hera_sim/visibilities/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/visibilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/visibilities/healvis_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/visibilities/pyuvsim_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/visibilities/simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-02-23 20:59:09.000000 hera_sim-3.1.1/hera_sim/visibilities/vis_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.929855 hera_sim-3.1.1/hera_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 20:59:19.000000 hera_sim-3.1.1/hera_sim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-23 20:59:09.000000 hera_sim-3.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 20:59:19.937856 hera_sim-3.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-02-23 20:59:09.000000 hera_sim-3.1.1/scripts/hera-sim-simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-02-23 20:59:09.000000 hera_sim-3.1.1/scripts/hera-sim-vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-23 20:59:19.937856 hera_sim-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 20:59:09.000000 hera_sim-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.360020 hera_sim-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.364020 hera_sim-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 20:28:19.000000 hera_sim-4.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-22 20:28:19.000000 hera_sim-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-22 20:28:19.000000 hera_sim-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 20:28:19.000000 hera_sim-4.0.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 20:28:19.000000 hera_sim-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:28:31.396020 hera_sim-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-22 20:28:19.000000 hera_sim-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.364020 hera_sim-4.0.0/config_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 20:28:19.000000 hera_sim-4.0.0/config_examples/simulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-22 20:28:19.000000 hera_sim-4.0.0/config_examples/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/notes_for_developers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.376020 hera_sim-4.0.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/end_to_end_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_defaults.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_tour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_vis_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/mutual_coupling_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/polybeam_simulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/visibility_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.380020 hera_sim-4.0.0/hera_sim/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/__yaml_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41518 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48424 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.384020 hera_sim-4.0.0/hera_sim/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/H1C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/H2C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/H37_FR_Filters_small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_LAT_LON_ALT.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_Tsky_Reformatted.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_Tsky_vs_LST.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.360020 hera_sim-4.0.0/hera_sim/data/tutorials_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60721 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63166 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.392020 hera_sim-4.0.0/hera_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34096 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_sim_red_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_simulate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_yaml_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.392020 hera_sim-4.0.0/hera_sim/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/testdata/healvis_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/hera_sim/visibilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/pyuvsim_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/vis_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.384020 hera_sim-4.0.0/hera_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:28:30.000000 hera_sim-4.0.0/hera_sim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-22 20:28:19.000000 hera_sim-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-22 20:28:19.000000 hera_sim-4.0.0/scripts/hera-sim-simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-22 20:28:19.000000 hera_sim-4.0.0/scripts/hera-sim-vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 20:28:31.396020 hera_sim-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:28:19.000000 hera_sim-4.0.0/setup.py
```

### Comparing `hera_sim-3.1.1/.coveragerc` & `hera_sim-4.0.0/.coveragerc`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [report]
 omit = hera_sim/tests/*
 
 # Regexes for lines to exclude from consideration
 exclude_lines =
     # Have to re-enable the standard pragma
     pragma: no cover
+    pragma: nocover
 
     # Don't complain about missing debug-only code:
     def __repr__
     if self\.debug
 
     # Don't complain if tests don't hit defensive assertion code:
     raise AssertionError
```

### Comparing `hera_sim-3.1.1/.flake8` & `hera_sim-4.0.0/.flake8`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/.github/workflows/publish.yaml` & `hera_sim-4.0.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/.pre-commit-config.yaml` & `hera_sim-4.0.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,13 +46,13 @@
   hooks:
   - id: isort
 
 - repo: https://github.com/asottile/pyupgrade
   rev: v3.3.1
   hooks:
   - id: pyupgrade
-    args: [--py38-plus]
+    args: [--py39-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
   rev: v2.2.0
   hooks:
   - id: setup-cfg-fmt
```

### Comparing `hera_sim-3.1.1/CHANGELOG.rst` & `hera_sim-4.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 =========
 Changelog
 =========
 
-dev-version
-===========
+v4.0.0 [2023.05.22]
+===================
+
+Breaking Changes
+----------------
+- Removed the ``HealVis`` wrapper. Use ``pyuvsim`` instead.
+
+Changed
+-------
+- Updated package to always use future array shapes for ``pyuvdata`` objects (this
+  includes updates to ``PolyBeam`` and ``Simulator`` objects amongst others).
 
 v3.1.1 [2023.02.23]
 ===================
 
 Changed
 -------
 - Coupling matrix calculation in :class:`~.sigchain.MutualCoupling` has been updated
```

### Comparing `hera_sim-3.1.1/CONTRIBUTING.rst` & `hera_sim-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/LICENSE.rst` & `hera_sim-4.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/PKG-INFO` & `hera_sim-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera_sim
-Version: 3.1.1
+Version: 4.0.0
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
@@ -13,16 +13,17 @@
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: all
 Provides-Extra: bda
 Provides-Extra: cal
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: tests
 Provides-Extra: vis
```

### Comparing `hera_sim-3.1.1/README.rst` & `hera_sim-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/config_examples/template_config.yaml` & `hera_sim-4.0.0/config_examples/template_config.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/Makefile` & `hera_sim-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/_templates/class.rst` & `hera_sim-4.0.0/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/_templates/module.rst` & `hera_sim-4.0.0/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/conf.py` & `hera_sim-4.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 pygments_style = "sphinx"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `hera_sim-3.1.1/docs/reference/index.rst` & `hera_sim-4.0.0/docs/reference/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -41,10 +41,9 @@
 Built-In Simulators
 +++++++++++++++++++
 
 .. autosummary::
     :toctree: _autosummary
     :template: class.rst
 
-    hera_sim.visibilities.healvis_wrapper.HealVis
     hera_sim.visibilities.vis_cpu.VisCPU
     hera_sim.visibilities.pyuvsim_wrapper.UVSim
```

### Comparing `hera_sim-3.1.1/docs/tutorials/end_to_end_example.ipynb` & `hera_sim-4.0.0/docs/tutorials/end_to_end_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/hera_sim_cli.rst` & `hera_sim-4.0.0/docs/tutorials/hera_sim_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/hera_sim_defaults.ipynb` & `hera_sim-4.0.0/docs/tutorials/hera_sim_defaults.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/hera_sim_simulator.ipynb` & `hera_sim-4.0.0/docs/tutorials/hera_sim_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/hera_sim_tour.ipynb` & `hera_sim-4.0.0/docs/tutorials/hera_sim_tour.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/hera_sim_vis_cli.rst` & `hera_sim-4.0.0/docs/tutorials/hera_sim_vis_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/mutual_coupling_example.ipynb` & `hera_sim-4.0.0/docs/tutorials/mutual_coupling_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/polybeam_simulation.ipynb` & `hera_sim-4.0.0/docs/tutorials/polybeam_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials/visibility_simulator.ipynb` & `hera_sim-4.0.0/docs/tutorials/visibility_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/docs/tutorials.rst` & `hera_sim-4.0.0/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/__init__.py` & `hera_sim-4.0.0/hera_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/__yaml_constructors.py` & `hera_sim-4.0.0/hera_sim/__yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/adjustment.py` & `hera_sim-4.0.0/hera_sim/adjustment.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,16 @@
         raise TypeError(
             "position_tolerance must be a real-valued scalar or length-3 array."
         )
 
     # Check if the target object is a Simulator, but work with a UVData object.
     target_is_simulator = isinstance(target, Simulator)
     target = _to_uvdata(target)
+    if not target.future_array_shapes:  # pragma: no cover
+        target.use_future_array_shapes()
 
     # Pull the reference metadata.
     if not isinstance(reference, UVData):
         if isinstance(reference, Simulator):
             reference_metadata = reference.data.copy(metadata_only=True)
         else:
             reference_files = _listify(reference)
@@ -267,16 +269,20 @@
     # address whether it is acceptable to modify the target antenna positions
     # in a way that allows them to be reflected through the local origin. While
     # this is a mathematically necessary consideration for finding the optimal
     # match in non-exponential time, adjusting the antenna positions like-so
     # is pretty unrealistic.
     target_is_simulator = isinstance(target, Simulator)
     target = _to_uvdata(target)
+    if not target.future_array_shapes:  # pragma: nocover
+        target.use_future_array_shapes()
     target_copy = copy.deepcopy(target)
     reference = _to_uvdata(reference)
+    if not reference.future_array_shapes:  # pragma: nocover
+        reference.use_future_array_shapes()
     reference_metadata = reference.copy(metadata_only=True)
 
     # Find the best choice of mapping between antennas.
     target_antpos = _get_antpos(target, ENU=ENU)
     ref_antpos = _get_antpos(reference, ENU=ENU)
     # This contains the downselected and shifted target antenna positions.
     array_intersection, is_reflected = _get_array_intersection(
@@ -372,20 +378,20 @@
         else:
             new_antpairpol = antpairpol
 
         # Figure out how to slice through the new data array.
         blts, conj_blts, pol_inds = target_copy._key2inds(new_antpairpol)
         if len(blts) > 0:
             # The new baseline has the same conjugation as the old one.
-            this_slice = (blts, 0, slice(None), pol_inds[0])
-        else:
+            this_slice = (blts, slice(None), pol_inds[0])
+        else:  # pragma: no cover
             # The new baseline is conjugated relative to the old one.
             # Given the handling of the antenna relabeling, this might not actually
             # ever be called.
-            this_slice = (conj_blts, 0, slice(None), pol_inds[1])
+            this_slice = (conj_blts, slice(None), pol_inds[1])
             vis = vis.conj()
             new_antpairpol = new_antpairpol[:2][::-1] + (pol,)
 
         # If we needed to reflect the entire array to find the best match, then
         # we need to make sure to conjugate the visibilities since the reflection
         # is effectively undone by baseline conjugation.
         if is_reflected:
@@ -538,31 +544,31 @@
         new_lst_array = np.empty(new_Nblts, dtype=float)
         new_ant_1_array = np.empty(new_Nblts, dtype=int)
         new_ant_2_array = np.empty(new_Nblts, dtype=int)
         new_baseline_array = np.empty(new_Nblts, dtype=int)
         new_uvw_array = np.empty((new_Nblts, 3), dtype=float)
         new_integration_times = np.empty(new_Nblts, dtype=float)
         if axis == "both":
-            new_data_shape = (new_Nblts, 1, ref_freqs.size, target.Npols)
+            new_data_shape = (new_Nblts, ref_freqs.size, target.Npols)
         else:
-            new_data_shape = (new_Nblts, 1, target_freqs.size, target.Npols)
+            new_data_shape = (new_Nblts, target_freqs.size, target.Npols)
         new_data = np.zeros(new_data_shape, dtype=complex)
     else:
-        new_data_shape = (target.Nblts, 1, ref_freqs.size, target.Npols)
+        new_data_shape = (target.Nblts, ref_freqs.size, target.Npols)
 
     # Actually update metadata and interpolate the data.
     new_data = np.empty(new_data_shape, dtype=complex)
     for i, antpair in enumerate(target.get_antpairs()):
         if axis == "freq":
             for pol_ind, pol in enumerate(target.polarization_array):
                 vis = target.get_data(antpair + (pol,))
                 this_blt_slice = target._key2inds(antpair + (pol,))[0]
                 re_spline = interp1d(target_freqs, vis.real, axis=1, kind=kind)
                 im_spline = interp1d(target_freqs, vis.imag, axis=1, kind=kind)
-                new_data[this_blt_slice, 0, :, pol_ind] = re_spline(
+                new_data[this_blt_slice, :, pol_ind] = re_spline(
                     ref_freqs
                 ) + 1j * im_spline(ref_freqs)
             continue
 
         # Preparation for updating metadata.
         ant1, ant2 = antpair
         this_slice = slice(i, None, target.Nbls)
@@ -594,23 +600,23 @@
                 im_spline = RectBivariateSpline(
                     target_lsts,
                     target_freqs,
                     vis.imag,
                     kx=kt,
                     ky=kf,
                 )
-                new_data[this_slice, 0, :, pol_ind] = re_spline(
+                new_data[this_slice, :, pol_ind] = re_spline(
                     ref_lsts, ref_freqs
                 ) + 1j * im_spline(ref_lsts, ref_freqs)
             else:
                 re_spline = interp1d(target_lsts, vis.real, axis=0, kind=kind)
                 im_spline = interp1d(target_lsts, vis.imag, axis=0, kind=kind)
-                new_data[this_slice, 0, :, pol_ind] = re_spline(
+                new_data[this_slice, :, pol_ind] = re_spline(ref_lsts) + 1j * im_spline(
                     ref_lsts
-                ) + 1j * im_spline(ref_lsts)
+                )
 
     # Finally, update all of the metadata.
     if axis in ("freq", "both"):
         target.Nfreqs = ref_freqs.size
         target.freq_array = ref_freqs
     if axis in ("time", "both"):
         target.Nblts = ref_times.size * target.Nbls
@@ -680,36 +686,30 @@
     if reference is not None:
         if not isinstance(reference, UVData):
             try:
                 reference = _to_uvdata(reference)
             except TypeError:
                 raise TypeError("reference must be convertible to a UVData object.")
 
-        ref_time_to_lst_map = {
-            ref_time: ref_lst
-            for ref_time, ref_lst in zip(reference.time_array, reference.lst_array)
-        }
+        ref_time_to_lst_map = dict(zip(reference.time_array, reference.lst_array))
         ref_times = np.array(list(ref_time_to_lst_map.keys()))
         ref_lsts = np.array(list(ref_time_to_lst_map.values()))
     else:
         if ref_times is None or ref_lsts is None:
             raise ValueError(
                 "Both ref_times and ref_lsts must be provided if reference is not."
             )
 
         if len(ref_times) != len(ref_lsts):
             raise ValueError("ref_times and ref_lsts must have the same length.")
 
         ref_time_to_lst_map = dict(zip(ref_times, ref_lsts))
 
     # Construct the reference -> target time map.
-    target_time_to_lst_map = {
-        target_time: target_lst
-        for target_time, target_lst in zip(target.time_array, target.lst_array)
-    }
+    target_time_to_lst_map = dict(zip(target.time_array, target.lst_array))
     target_times = np.array(list(target_time_to_lst_map.keys()))
     target_lsts = np.array(list(target_time_to_lst_map.values()))
     ref_to_target_time_map = get_d2m_time_map(
         ref_times, ref_lsts, target_times, target_lsts
     )
 
     # Use only reference LSTs within the bounds of the target LSTs.
@@ -753,15 +753,15 @@
     target.select(times=np.unique(target_times))
     data = target.build_datacontainers()[0]
     data.select_or_expand_times(target_times)
     antpos = data.antpos
     bls = {(ai, aj, pol): antpos[aj] - antpos[ai] for ai, aj, pol in data.bls()}
     lat = target.telescope_location_lat_lon_alt_degrees[0]
     new_Nblts = target.Nbls * target_times.size
-    new_data = np.zeros((new_Nblts, 1, target.Nfreqs, target.Npols), dtype=complex)
+    new_data = np.zeros((new_Nblts, target.Nfreqs, target.Npols), dtype=complex)
     new_time_array = np.empty(new_Nblts, dtype=float)
     new_lst_array = np.empty(new_Nblts, dtype=float)
     new_integration_times = np.empty(new_Nblts, dtype=float)
     new_ant_1_array = np.empty(new_Nblts, dtype=int)
     new_ant_2_array = np.empty(new_Nblts, dtype=int)
     new_baseline_array = np.empty(new_Nblts, dtype=int)
     new_uvw_array = np.empty((new_Nblts, 3), dtype=float)
@@ -785,15 +785,15 @@
 
         # Update the data
         for pol_ind, pol in enumerate(target.polarization_array):
             pol = polnum2str(pol)
             antpairpol = antpair + (pol,)
             vis = data[antpairpol]
             bl = bls[antpairpol]
-            new_data[this_slice, 0, :, pol_ind] = lst_rephase(
+            new_data[this_slice, :, pol_ind] = lst_rephase(
                 vis, bl, data.freqs, dlst, lat=lat, array=True
             )
 
     # Convert from HERAData object to UVData object
     _uvd = UVData()
     for attr in _uvd:
         setattr(_uvd, attr, getattr(target, attr))
```

### Comparing `hera_sim-3.1.1/hera_sim/antpos.py` & `hera_sim-4.0.0/hera_sim/antpos.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,14 @@
                             )
                         else:
                             positions.append(
                                 np.asarray([x_pos, y_pos, 0])
                                 - 3 * (up_right + up_left) / 3
                             )
 
-        antpos = {j: pos for j, pos in enumerate(np.array(positions))}
+        antpos = dict(enumerate(np.array(positions)))
 
         return dict(antpos)
 
 
 linear_array = LinearArray()
 hex_array = HexArray()
```

### Comparing `hera_sim-3.1.1/hera_sim/beams.py` & `hera_sim-4.0.0/hera_sim/beams.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,18 @@
 
     pol_strings = ["pI", "pQ", "pU", "pV"]
     power_data = np.zeros((1, 1, 4, Nfreqs, npix), dtype=np.complex128)
 
     for fq_i in range(Nfreqs):
         jones = np.zeros((npix, 2, 2), dtype=np.complex128)
         pol_strings = ["pI", "pQ", "pU", "pV"]
-        jones[:, 0, 0] = efield_beam[0, 0, 0, fq_i, :]
-        jones[:, 0, 1] = efield_beam[0, 0, 1, fq_i, :]
-        jones[:, 1, 0] = efield_beam[1, 0, 0, fq_i, :]
-        jones[:, 1, 1] = efield_beam[1, 0, 1, fq_i, :]
+        jones[:, 0, 0] = efield_beam[0, 0, fq_i, :]
+        jones[:, 0, 1] = efield_beam[0, 1, fq_i, :]
+        jones[:, 1, 0] = efield_beam[1, 0, fq_i, :]
+        jones[:, 1, 1] = efield_beam[1, 1, fq_i, :]
 
         for pol_i in range(len(pol_strings)):
             power_data[:, :, pol_i, fq_i, :] = construct_mueller(jones, pol_i, pol_i)
 
     return power_data
 
 
@@ -178,27 +178,24 @@
     # stretched zenith angle, shape (Nfreq, za.size)
     za_scale = za[np.newaxis, :] / fscale[:, np.newaxis]
     # phase component, shape za_scale.shape = (Nfreq, za.size)
     ph = q(za_scale) * (1.0 + p(za_scale) * 1.0j)
     # shape (2, 2, 1, az.size)
     dipole_mod = ph[np.newaxis, np.newaxis, ...] * dipole[:, :, np.newaxis, :]
     # shape (2, 1, 2, Nfreq, az.size)
-    pol_efield_beam = (
-        dipole_mod[:, np.newaxis, ...]
-        * beam_vals[np.newaxis, np.newaxis, np.newaxis, ...]
-    )
+    pol_efield_beam = dipole_mod[:, ...] * beam_vals[np.newaxis, np.newaxis, ...]
 
     # Correct it for frequency dependency.
     # extract modulus and phase of the beams
     modulus = np.abs(pol_efield_beam)
     phase = np.angle(pol_efield_beam)
     # assume linear shift of phase along frequency
     shift = -np.pi / 18e6 * (freqs[:, np.newaxis] - ref_freq)  # shape (Nfreq, 1)
     # shift the phase
-    phase += shift[np.newaxis, np.newaxis, np.newaxis, :, :]
+    phase += shift[np.newaxis, np.newaxis, :, :]
     # upscale the modulus
     modulus = np.power(modulus, 0.6)  # ad-hoc
     # map the phase to [-pi; +pi]
     phase = utils.wrap2pipi(phase)
     # reconstruct
     pol_efield_beam = modulus * np.exp(1j * phase)
 
@@ -349,15 +346,15 @@
         if az_array.size != za_array.size:
             raise ValueError(
                 "Azimuth and zenith angle coordinate arrays must have same length."
             )
 
         # Empty data array
         interp_data = np.zeros(
-            (2, 1, 2, freq_array.size, az_array.size), dtype=np.complex128
+            (2, 2, freq_array.size, az_array.size), dtype=np.complex128
         )
 
         # Frequency scaling
         fscale = (freq_array / self.ref_freq) ** self.spectral_index
 
         # Transformed zenith angle, also scaled with frequency
         x = 2.0 * np.sin(za_array[np.newaxis, ...] / fscale[:, np.newaxis]) - 1.0
@@ -371,36 +368,38 @@
         # Axes: [phi, theta] (az and za) / Feeds: [n, e]
         # interp_data shape: (Naxes_vec, Nspws, Nfeeds or Npols, Nfreqs, Naz)
         if self.polarized:
             interp_data = modulate_with_dipole(
                 az_array, za_array, freq_array, self.ref_freq, beam_values, fscale
             )
         else:
-            interp_data[1, 0, 0, :, :] = beam_values  # (theta, n)
-            interp_data[0, 0, 1, :, :] = beam_values  # (phi, e)
+            interp_data[1, 0, :, :] = beam_values  # (theta, n)
+            interp_data[0, 1, :, :] = beam_values  # (phi, e)
 
         interp_basis_vector = None
 
         if self.beam_type == "power":
             # Cross-multiplying feeds, adding vector components
             pairs = [(i, j) for i in range(2) for j in range(2)]
-            power_data = np.zeros((1, 1, 4) + beam_values.shape, dtype=float)
+            power_data = np.zeros((1, 4) + beam_values.shape, dtype=float)
             for pol_i, pair in enumerate(pairs):
-                power_data[:, :, pol_i] = (
-                    interp_data[0, :, pair[0]] * np.conj(interp_data[0, :, pair[1]])
-                ) + (interp_data[1, :, pair[0]] * np.conj(interp_data[1, :, pair[1]]))
+                power_data[:, pol_i] = (
+                    interp_data[0, pair[0]] * np.conj(interp_data[0, pair[1]])
+                ) + (interp_data[1, pair[0]] * np.conj(interp_data[1, pair[1]]))
             interp_data = power_data
 
         return interp_data, interp_basis_vector
 
     def __eq__(self, other):
         """Evaluate equality with another object."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.beam_coeffs == other.beam_coeffs
+        return (
+            self.beam_coeffs == other.beam_coeffs
+            if isinstance(other, self.__class__)
+            else False
+        )
 
 
 class PerturbedPolyBeam(PolyBeam):
     """A :class:`PolyBeam` in which the shape of the beam has been modified.
 
     The perturbations can be applied to the mainlobe, sidelobes, or
     the entire beam. While the underlying :class:`PolyBeam` depends on
@@ -729,15 +728,15 @@
             Npixels/(Naxis1, Naxis2) or az_array.size if az/za_arrays are passed)
         interp_basis_vector : array_like
             Array of interpolated basis vectors (or self.basis_vector_array
             if az/za_arrays are not passed), shape: (Naxes_vec, Ncomponents_vec,
             Npixels/(Naxis1, Naxis2) or az_array.size if az/za_arrays are passed)
         """
         # Empty data array
-        interp_data = np.zeros((2, 1, 2, freq_array.size, az_array.size), dtype=float)
+        interp_data = np.zeros((2, 2, freq_array.size, az_array.size), dtype=float)
 
         # Frequency scaling
         fscale = (freq_array / self.ref_freq) ** self.spectral_index
         radial_coord = za_array[np.newaxis, ...] / fscale[:, np.newaxis]
         axial_coord = az_array[np.newaxis, ...]
 
         # Primary beam values from Zernike polynomial
@@ -747,35 +746,37 @@
             y=radial_coord * np.sin(axial_coord),
         )
         central_val = self.zernike(coeffs=self.beam_coeffs, x=0.0, y=0.0)
         if self.peak_normalized:
             values /= central_val  # ensure normalized to 1 at za=0
 
         # Set values
-        interp_data[1, 0, 0, :, :] = values
-        interp_data[0, 0, 1, :, :] = values
+        interp_data[1, 0] = values
+        interp_data[0, 1] = values
         interp_basis_vector = None
 
         if self.beam_type == "power":
             # Cross-multiplying feeds, adding vector components
             pairs = [(i, j) for i in range(2) for j in range(2)]
-            power_data = np.zeros((1, 1, 4) + values.shape, dtype=float)
+            power_data = np.zeros((1, 4) + values.shape, dtype=float)
             for pol_i, pair in enumerate(pairs):
-                power_data[:, :, pol_i] = (
-                    interp_data[0, :, pair[0]] * np.conj(interp_data[0, :, pair[1]])
-                ) + (interp_data[1, :, pair[0]] * np.conj(interp_data[1, :, pair[1]]))
+                power_data[:, pol_i] = (
+                    interp_data[0, pair[0]] * np.conj(interp_data[0, pair[1]])
+                ) + (interp_data[1, pair[0]] * np.conj(interp_data[1, pair[1]]))
             interp_data = power_data
 
         return interp_data, interp_basis_vector
 
     def __eq__(self, other):
         """Evaluate equality with another object."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.beam_coeffs == other.beam_coeffs
+        return (
+            self.beam_coeffs == other.beam_coeffs
+            if isinstance(other, self.__class__)
+            else False
+        )
 
     @staticmethod
     def zernike(coeffs, x, y):
         """
         Zernike polynomials (up to degree 66) on the unit disc.
 
         This code was adapted from:
```

### Comparing `hera_sim-3.1.1/hera_sim/cli_utils.py` & `hera_sim-4.0.0/hera_sim/cli_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     pol_array = list({antpol[1] for antpol in gains})
     jones_array = [
         jnum2str(
             jstr2num(pol, x_orientation=x_orientation), x_orientation=x_orientation
         )
         for pol in pol_array
     ]
-    mapping = {pol: jpol for pol, jpol in zip(pol_array, jones_array)}
+    mapping = dict(zip(pol_array, jones_array))
     return {(antpol[0], mapping[antpol[1]]): gain for antpol, gain in gains.items()}
 
 
 def _validate_freq_params(freq_params):
     """Ensure frequency parameters specified are sufficient."""
     allowed_params = (
         "Nfreqs",
```

### Comparing `hera_sim-3.1.1/hera_sim/components.py` & `hera_sim-4.0.0/hera_sim/components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/config/H1C.yaml` & `hera_sim-4.0.0/hera_sim/config/H1C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/config/H2C.yaml` & `hera_sim-4.0.0/hera_sim/config/H2C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/config/debug.yaml` & `hera_sim-4.0.0/hera_sim/config/debug.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/H37_FR_Filters_small.npz` & `hera_sim-4.0.0/hera_sim/data/H37_FR_Filters_small.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy` & `hera_sim-4.0.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz` & `hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy` & `hera_sim-4.0.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/HERA_Tsky_Reformatted.npz` & `hera_sim-4.0.0/hera_sim/data/HERA_Tsky_Reformatted.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/HERA_Tsky_vs_LST.npz` & `hera_sim-4.0.0/hera_sim/data/HERA_Tsky_vs_LST.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py` & `hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt` & `hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv` & `hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5` & `hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/defaults.py` & `hera_sim-4.0.0/hera_sim/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,18 +304,15 @@
         def new_func(*args, **kwargs):
             # get the full argspec
             argspec = inspect.getfullargspec(func)
 
             # get dictionary of kwargs and their defaults
             try:
                 offset = len(argspec.args) - len(argspec.defaults)
-                old_kwargs = {
-                    arg: default
-                    for arg, default in zip(argspec.args[offset:], argspec.defaults)
-                }
+                old_kwargs = dict(zip(argspec.args[offset:], argspec.defaults))
             except TypeError:
                 # if there are no defaults in the argspec
                 old_kwargs = {}
 
             # make the args list into a dictionary
             args = {argspec.args[i]: arg for i, arg in enumerate(args)}
```

### Comparing `hera_sim-3.1.1/hera_sim/eor.py` & `hera_sim-4.0.0/hera_sim/eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/foregrounds.py` & `hera_sim-4.0.0/hera_sim/foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/interpolators.py` & `hera_sim-4.0.0/hera_sim/interpolators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/io.py` & `hera_sim-4.0.0/hera_sim/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Methods for input/output of data."""
 import numpy as np
 import os
 import pyuvdata
 import re
 import warnings
+from collections.abc import Sequence
 from pyuvdata import UVData
 from pyuvsim.simsetup import initialize_uvdata_from_keywords
-from typing import Dict, Sequence
 
 from . import DATA_PATH
 from .defaults import _defaults
 
 HERA_LAT_LON_ALT = np.load(DATA_PATH / "HERA_LAT_LON_ALT.npy")
 
 
 # this decorator allows the parameters specified in the function
 # signature to be overridden by the defaults module
 @_defaults
 def empty_uvdata(
     Ntimes=None,
     start_time=2456658.5,  # Jan 1 2014
     integration_time=None,
-    array_layout: Dict[int, Sequence[float]] = None,
+    array_layout: dict[int, Sequence[float]] = None,
     Nfreqs=None,
     start_freq=None,
     channel_width=None,
     n_freq=None,
     n_times=None,
     antennas=None,  # back-compat
     conjugation=None,
@@ -112,17 +112,17 @@
     # TODO: the following is a hack patch for pyuvsim which should be fixed there.
     if "x_orientation" in kwargs and uvd.x_orientation is None:
         uvd.x_orientation = kwargs["x_orientation"]
 
     if conjugation is not None:
         uvd.conjugate_bls(convention=conjugation)
 
-    # Temporary fix for future array shape - to be removed after v3.
-    if uvd.future_array_shapes:
-        uvd.use_current_array_shapes()
+    # Ensure we're using future array shapes
+    if not uvd.future_array_shapes:  # pragma: no cover
+        uvd.use_future_array_shapes()
 
     return uvd
 
 
 def chunk_sim_and_save(
     sim_uvd,
     save_dir,
```

### Comparing `hera_sim-3.1.1/hera_sim/noise.py` & `hera_sim-4.0.0/hera_sim/noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/rfi.py` & `hera_sim-4.0.0/hera_sim/rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/sigchain.py` & `hera_sim-4.0.0/hera_sim/sigchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from __future__ import annotations
 
 import astropy_healpix as aph
 import copy
 import numpy as np
 import warnings
 from astropy import constants, units
+from collections.abc import Sequence
 from pathlib import Path
 from pyuvdata import UVBeam
 from pyuvsim import AnalyticBeam
 from scipy import stats
 from scipy.signal import blackmanharris
-from typing import Callable, Sequence
+from typing import Callable
 
 from . import DATA_PATH, interpolators, utils
 from .components import component
 from .defaults import _defaults
 
 
 @component
@@ -781,15 +782,15 @@
         pol_array="polarization_array",
         array_layout="antpos",
         visibilities="data_array",
     )
 
     def __init__(
         self,
-        uvbeam: UVBeam | str | Path | None,
+        uvbeam: UVBeam | str | Path | None = None,
         reflection: np.ndarray | Callable | None = None,
         omega_p: np.ndarray | Callable | None = None,
         ant_1_array: np.ndarray | None = None,
         ant_2_array: np.ndarray | None = None,
         pol_array: np.ndarray | None = None,
         array_layout: dict | None = None,
         coupling_matrix: np.ndarray | None = None,
@@ -881,15 +882,15 @@
         array_layout = {ant: array_layout[ant] for ant in sorted(antpos_ants)}
         antenna_numbers = np.array(list(array_layout.keys()))
 
         # Figure out how to reshape the visibility array
         n_bls = np.unique(np.vstack([ant_1_array, ant_2_array]), axis=1).shape[1]
         n_ants = antenna_numbers.size
         n_times = ant_1_array.size // n_bls
-        n_freqs = visibilities.squeeze().shape[1]
+        n_freqs = visibilities.shape[1]
         n_pols = visibilities.shape[-1]
         visibilities = utils.reshape_vis(
             vis=visibilities,
             ant_1_array=ant_1_array,
             ant_2_array=ant_2_array,
             pol_array=pol_array,
             antenna_numbers=antenna_numbers,
@@ -1028,21 +1029,20 @@
                 power_beam.efield_to_power()
                 nside = 128
                 npix = aph.nside_to_npix(nside)
                 pix_area = aph.nside_to_pixel_area(nside).to("sr").value
                 pix_inds = np.arange(npix)
                 lon, lat = aph.healpix_to_lonlat(pix_inds, nside)
                 above_horizon = lat.value > 0
+                # Just take the XX polarization
                 beam_vals = power_beam.interp(
                     az_array=lon.to("rad").value,
                     za_array=np.pi / 2 - lat.to("rad").value,
                     freq_array=freqs * units.GHz.to("Hz"),
-                )[0][
-                    0, 0, 0
-                ]  # Just take the XX polarization
+                )[0][0, 0]
                 beam_vals[:, ~above_horizon] = 0  # Apply horizon cut
                 omega_p = beam_vals.sum(axis=1).real * pix_area
             else:
                 power_beam = uvbeam.copy()
                 power_beam.efield_to_power()
                 if power_beam.interpolation_function is None:
                     power_beam.interpolation_function = pixel_interp
@@ -1116,15 +1116,15 @@
                 jones_ji = jones_matrices[antpair2angle[aj, ai]]
                 jones_prod = jones_ij @ jones_ji.conj().transpose(0, 2, 1)
 
                 # If we wanted to add a baseline orientation/length cut,
                 # then this is where we would do it.
                 bl_len = np.linalg.norm(enu_antpos[j] - enu_antpos[i])
                 delay = np.exp(
-                    2j * np.pi * freqs * bl_len / constants.c.to("m/ns").value
+                    -2j * np.pi * freqs * bl_len / constants.c.to("m/ns").value
                 ).reshape(-1, 1, 1)
                 coupling = delay * jones_prod / bl_len
 
                 # Fill in the upper-triangular part
                 # Even indices are "X" feed; odd are "Y" feed
                 coupling_matrix[0, :, ::2, ::2][:, i, j] = coupling[:, 0, 0]
                 coupling_matrix[0, :, 1::2, ::2][:, i, j] = coupling[:, 0, 1]
```

### Comparing `hera_sim-3.1.1/hera_sim/simulate.py` & `hera_sim-4.0.0/hera_sim/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 import inspect
 import numpy as np
 import time
 import warnings
 import yaml
 from astropy import constants as const
 from cached_property import cached_property
+from collections.abc import Sequence
 from deprecation import deprecated
 from pathlib import Path
 from pyuvdata import UVData
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Optional, Union
 
 from . import __version__, io, utils
 from .components import SimulationComponent, get_model, list_all_components
 from .defaults import defaults
 
 _add_depr = deprecated(
     deprecated_in="1.0", removed_in="2.0", details="Use the :meth:`add` method instead."
 )
 
 # Define some commonly used types for typing purposes.
-AntPairPol = Tuple[int, int, str]
-AntPair = Tuple[int, int]
-AntPol = Tuple[int, str]
-Component = Union[str, Type[SimulationComponent], SimulationComponent]
+AntPairPol = tuple[int, int, str]
+AntPair = tuple[int, int]
+AntPol = tuple[int, str]
+Component = Union[str, type[SimulationComponent], SimulationComponent]
 
 
 # wrapper for the run_sim method, necessary for part of the CLI
 def _generator_to_list(func, *args, **kwargs):
     @functools.wraps(func)
     def new_func(*args, **kwargs):
         result = list(func(*args, **kwargs))
@@ -205,16 +206,16 @@
             Whether to refresh the defaults.
         """
         defaults.set(config, refresh=refresh)
 
     def calculate_filters(
         self,
         *,
-        delay_filter_kwargs: Optional[Dict[str, Union[float, str]]] = None,
-        fringe_filter_kwargs: Optional[Dict[str, Union[float, str, np.ndarray]]] = None,
+        delay_filter_kwargs: Optional[dict[str, Union[float, str]]] = None,
+        fringe_filter_kwargs: Optional[dict[str, Union[float, str, np.ndarray]]] = None,
     ):
         """
         Pre-compute fringe-rate and delay filters for the entire array.
 
         Parameters
         ----------
         delay_filter_kwargs
@@ -235,15 +236,15 @@
         *,
         add_vis: bool = True,
         ret_vis: bool = False,
         seed: Optional[Union[str, int]] = None,
         vis_filter: Optional[Sequence] = None,
         component_name: Optional[str] = None,
         **kwargs,
-    ) -> Optional[Union[np.ndarray, Dict[int, np.ndarray]]]:
+    ) -> Optional[Union[np.ndarray, dict[int, np.ndarray]]]:
         """
         Simulate an effect then apply and/or return the result.
 
         Parameters
         ----------
         component
             Effect to be simulated. This can either be an alias of the effect,
@@ -323,15 +324,15 @@
 
         return data
 
     def get(
         self,
         component: Component,
         key: Optional[Union[int, str, AntPair, AntPairPol]] = None,
-    ) -> Union[np.ndarray, Dict[int, np.ndarray]]:
+    ) -> Union[np.ndarray, dict[int, np.ndarray]]:
         """
         Retrieve an effect that was previously simulated.
 
         Parameters
         ----------
         component
             Effect that is to be retrieved. See :meth:`add` for more details.
@@ -417,15 +418,15 @@
                 **kwargs,
             )
 
             # Trim the data if a specific polarization is requested.
             if pol is None:
                 return data
             pol_ind = self.pols.index(pol)
-            return data[:, 0, :, pol_ind]
+            return data[:, :, pol_ind]
 
         # We're only simulating for a particular baseline.
         # First, find out if it needs to be conjugated.
         try:
             blt_inds = self.data.antpair2ind(ant1, ant2)
             if blt_inds.size == 0:
                 raise ValueError
@@ -441,15 +442,15 @@
                 model,
                 add_vis=False,
                 ret_vis=True,
                 seed=seed,
                 vis_filter=vis_filter,
                 antpairpol_cache=None,
                 **kwargs,
-            )[blt_inds, 0, :, :]
+            )[blt_inds, :, :]
             if conj_data:  # pragma: no cover
                 data = np.conj(data)
             if pol is None:
                 return data
             pol_ind = self.data.get_pols().index(pol)
             return data[..., pol_ind]
         elif seed == "redundant":
@@ -465,15 +466,15 @@
             data_shape = (self.lsts.size, self.freqs.size, len(self.pols))
             pols = self.pols
             return_slice = (slice(None),) * 3
         else:
             data_shape = (self.lsts.size, self.freqs.size, 1)
             pols = (pol,)
             return_slice = (slice(None), slice(None), 0)
-        data = np.zeros(data_shape, dtype=np.complex)
+        data = np.zeros(data_shape, dtype=complex)
         for i, _pol in enumerate(pols):
             args = self._initialize_args_from_model(model)
             args = self._update_args(args, model, ant1, ant2, pol)
             args.update(kwargs)
             if conj_data:
                 self._seed_rng(seed, model, ant2, ant1, _pol)
             else:
@@ -888,14 +889,17 @@
         else:
             raise TypeError(
                 "data type not understood. Only a UVData object or a path to "
                 "a UVData-compatible file may be passed as the data parameter. "
                 "Otherwise, keywords must be provided to build a UVData object."
             )
 
+        if not self.data.future_array_shapes:  # pragma: nocover
+            self.data.use_future_array_shapes()
+
     def _initialize_args_from_model(self, model):
         """
         Retrieve the LSTs and/or frequencies required for a model.
 
         Parameters
         ----------
         model: callable
@@ -953,15 +957,15 @@
         *,
         add_vis: bool = True,
         ret_vis: bool = False,
         seed: Optional[Union[str, int]] = None,
         vis_filter: Optional[Sequence] = None,
         antpairpol_cache: Optional[Sequence[AntPairPol]] = None,
         **kwargs,
-    ) -> Optional[Union[np.ndarray, Dict[int, np.ndarray]]]:
+    ) -> Optional[Union[np.ndarray, dict[int, np.ndarray]]]:
         """
         Simulate an effect for an entire array.
 
         This method loops over every baseline and polarization in order
         to simulate the effect ``model`` for the full array. The result
         is optionally applied to the simulation's data and/or returned.
 
@@ -1103,27 +1107,27 @@
                 if not (bl_in_cache or conj_in_cache or apply_filter):
                     antpairpol_cache.append((ant1, ant2, pol))
 
                 # Check whether we're simulating a gain or a visibility.
                 if is_multiplicative:
                     # Calculate the complex gain, but only apply it if requested.
                     gain = gains[(ant1, pol[0])] * np.conj(gains[(ant2, pol[1])])
-                    data_copy[blt_inds, 0, :, pol_ind] *= gain
+                    data_copy[blt_inds, :, pol_ind] *= gain
                 else:
                     # I don't think this will ever be executed, but just in case...
                     if conj_in_cache and seed is None:  # pragma: no cover
                         conj_blts = self.data.antpair2ind((ant2, ant1))
                         vis = (data_copy - self.data.data_array)[
-                            conj_blts, 0, :, pol_ind
+                            conj_blts, :, pol_ind
                         ].conj()
                     else:
                         vis = model(**use_args)
 
                     # and add it in
-                    data_copy[blt_inds, 0, :, pol_ind] += vis
+                    data_copy[blt_inds, :, pol_ind] += vis
 
         # return the component if desired
         # this is a little complicated, but it's done this way so that
         # there aren't *three* copies of the data array floating around
         # this is to minimize the potential of triggering a MemoryError
         if ret_vis:
             # return the gain dictionary if gains are simulated
@@ -1317,15 +1321,15 @@
     def _get_filters(
         self,
         ant1: int,
         ant2: int,
         *,
         get_delay_filter: bool = True,
         get_fringe_filter: bool = True,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """
         Retrieve delay and fringe filters from the cache.
 
         Parameters
         ----------
         ant1
             First antenna in the baseline.
@@ -1379,16 +1383,16 @@
             for parameter, value in params.items():
                 model_params[parameter] = value.default
         model_params.pop("kwargs", None)
         return model_params
 
     @staticmethod
     def _get_component(
-        component: Union[str, Type[SimulationComponent], SimulationComponent]
-    ) -> Union[SimulationComponent, Type[SimulationComponent]]:
+        component: Union[str, type[SimulationComponent], SimulationComponent]
+    ) -> Union[SimulationComponent, type[SimulationComponent]]:
         """Normalize a component to be either a class or instance."""
         if np.issubclass_(component, SimulationComponent):
             return component
         elif isinstance(component, str):
             try:
                 return get_model(component)
             except KeyError:
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/conftest.py` & `hera_sim-4.0.0/hera_sim/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_adjustment.py` & `hera_sim-4.0.0/hera_sim/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_antpos.py` & `hera_sim-4.0.0/hera_sim/tests/test_antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_beams.py` & `hera_sim-4.0.0/hera_sim/tests/test_beams.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import astropy_healpix.healpy as hp
 import copy
 import numpy as np
 from astropy import units
 from astropy.coordinates import Latitude, Longitude
 from pyradiosky import SkyModel
-from typing import List
 
 from hera_sim import io
 from hera_sim.beams import (
     PerturbedPolyBeam,
     PolyBeam,
     ZernikeBeam,
     efield_to_pstokes,
@@ -77,16 +76,16 @@
     """
     Convert an E-field to its pseudo-Stokes power beam.
     """
     nside_test = 64
     pixel_indices_test = hp.ang2pix(nside_test, za, az)
     npix_test = hp.nside2npix(nside_test)
 
-    pol_efield_beam_plot = np.zeros((2, 1, 2, Nfreq, npix_test), dtype=np.complex128)
-    pol_efield_beam_plot[:, :, :, :, pixel_indices_test] = eval_beam[:, :, :, :]
+    pol_efield_beam_plot = np.zeros((2, 2, Nfreq, npix_test), dtype=np.complex128)
+    pol_efield_beam_plot[:, :, :, pixel_indices_test] = eval_beam[:, :, :, :]
     return efield_to_pstokes(pol_efield_beam_plot, npix_test, Nfreq)
 
 
 def run_sim(
     ants,
     sources,
     beams,
@@ -148,15 +147,15 @@
 
     return np.abs(simulation.uvdata.get_data(0, 0, pol)[0][0])
 
 
 class TestPerturbedPolyBeam:
     def get_perturbed_beams(
         self, rotation, polarized=False, power_beam=False
-    ) -> List[PerturbedPolyBeam]:
+    ) -> list[PerturbedPolyBeam]:
         """
         Elliptical PerturbedPolyBeam.
 
         This will also test PolyBeam, from which PerturbedPolybeam is derived.
         """
         cfg_beam = dict(
             ref_freq=1.0e8,
@@ -397,15 +396,15 @@
         eval_beam, az, za, Nfreq = evaluate_polybeam(polarized_polybeam)
 
         # Check that the beam is normalized between 1 and 0 (± 1e-2),
         # at all polarizations and a range of selected frequencies.
         for vec in [0, 1]:
             for feed in [0, 1]:
                 for freq in [0, 5, 10, 15, 20, 25]:
-                    modulus = np.abs(eval_beam[vec, 0, feed, freq])
+                    modulus = np.abs(eval_beam[vec, feed, freq])
                     M = np.max(modulus)
                     m = np.min(modulus)
                     assert M <= 1 and M == pytest.approx(
                         1, rel=3e-2
                     ), "beam not properly normalized"
                     assert m >= 0 and m == pytest.approx(
                         0, abs=1e-3
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_cli_utils.py` & `hera_sim-4.0.0/hera_sim/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_compare_pyuvsim.py` & `hera_sim-4.0.0/hera_sim/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_components.py` & `hera_sim-4.0.0/hera_sim/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_defaults.py` & `hera_sim-4.0.0/hera_sim/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_eor.py` & `hera_sim-4.0.0/hera_sim/tests/test_eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_foregrounds.py` & `hera_sim-4.0.0/hera_sim/tests/test_foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_interpolators.py` & `hera_sim-4.0.0/hera_sim/tests/test_interpolators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_io.py` & `hera_sim-4.0.0/hera_sim/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_noise.py` & `hera_sim-4.0.0/hera_sim/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_rfi.py` & `hera_sim-4.0.0/hera_sim/tests/test_rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_sigchain.py` & `hera_sim-4.0.0/hera_sim/tests/test_sigchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         enu_bl = enu_antpos[aj] - enu_antpos[ai]
         dbdt = np.linalg.norm(np.cross(ecef_bl, omega))
         sign = np.sign(np.round(enu_bl[0], 3))
         frates = sign * freq_mesh * dbdt / constants.c.si.value
         blt_inds = uvdata.antpair2ind(ai, aj)
 
         # Make visibilities compact in delay/freq, and localized in fringe-rate.
-        uvdata.data_array[blt_inds, 0, :, 0] = np.exp(
+        uvdata.data_array[blt_inds, :, 0] = np.exp(
             -((delay_width * (freq_mesh - ref_freq)) ** 2)
         ) * np.exp(2j * np.pi * frates[None, :] * time_mesh)
 
         # Let's also track the delays/fringe-rates
         delays[(ai, aj)] = np.linalg.norm(enu_bl) / constants.c.to("m/ns").value
         delays[(aj, ai)] = delays[(ai, aj)]
         mean_frate = sign * dbdt * np.mean(freqs) / constants.c.si.value
@@ -412,15 +412,15 @@
     mutual_coupling = sigchain.MutualCoupling(
         uvbeam="uniform",
         ant_1_array=uvdata.ant_1_array,
         ant_2_array=uvdata.ant_2_array,
         pol_array=uvdata.polarization_array,
         array_layout=dict(zip(*uvdata.get_ENU_antpos()[::-1])),
         reflection=np.ones(uvdata.Nfreqs) * refl_amp,
-        omega_p=constants.c.si.value / uvdata.freq_array[0],
+        omega_p=constants.c.si.value / uvdata.freq_array,
     )
     uvdata.data_array += mutual_coupling(
         freqs=freqs / 1e9,
         visibilities=uvdata.data_array,
         use_numba=use_numba,
     )
 
@@ -430,16 +430,16 @@
     for (ai, aj, _pol), vis in uvdata.antpairpol_iter():
         vis_fft = uvtools.utils.FFT(
             uvtools.utils.FFT(vis, axis=0, taper="bh"),
             axis=1,
             taper="bh",
         )
         for ak in uvdata.antenna_numbers:
-            dly_ik = delays[(ai, ak)]
-            dly_kj = -delays[(ak, aj)]  # This coupling term is conjugated.
+            dly_ik = -delays[(ai, ak)]
+            dly_kj = delays[(ak, aj)]  # This coupling term is conjugated.
             frate_ik = fringe_rates[(ai, ak)]
             frate_kj = fringe_rates[(ak, aj)]
 
             # Check that the coupling was performed correctly.
             if aj != ak:
                 ik_ind = (
                     np.argmin(np.abs(frate_ik - frate_mHz)),
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_sim_red_data.py` & `hera_sim-4.0.0/hera_sim/tests/test_sim_red_data.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_simulate_cli.py` & `hera_sim-4.0.0/hera_sim/tests/test_simulate_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_simulator.py` & `hera_sim-4.0.0/hera_sim/tests/test_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             pols="polarization_array",
         )
 
         def __init__(self):
             pass
 
         def __call__(self, freqs, ant_1_array, pols):
-            data_shape = (ant_1_array.size, 1, freqs.size, pols.size)
+            data_shape = (ant_1_array.size, freqs.size, pols.size)
             return np.ones(data_shape, dtype=complex)
 
     base_sim.add(Test)
     assert np.all(base_sim.data_array == 1)
 
 
 def test_refresh(base_sim):
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_utils.py` & `hera_sim-4.0.0/hera_sim/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,25 +407,25 @@
     )
     # Make the autos real otherwise we're going to have problems
     for ai, aj, pol in sim.get_antpairpols():
         if ai != aj:
             continue
         inds = sim.data.antpair2ind(ai, ai)
         p = list(sim.polarization_array).index(uvutils.polstr2num(pol))
-        sim.data.data_array[inds, 0, :, p] = np.random.normal(
+        sim.data.data_array[inds, :, p] = np.random.normal(
             size=(sim.Ntimes, sim.Nfreqs)
         ).astype(complex)
 
     if "xy" in sim.get_pols() and "yx" in sim.get_pols():
         # Need to fix these autos as well
         for ai in sim.antenna_numbers:
             inds = sim.data.antpair2ind(ai, ai)
             p1 = list(sim.get_pols()).index("xy")
             p2 = list(sim.get_pols()).index("yx")
-            sim.data.data_array[inds, 0, :, p1] = sim.data_array[inds, 0, :, p2].conj()
+            sim.data.data_array[inds, :, p1] = sim.data_array[inds, :, p2].conj()
 
     reshape_args = [
         sim.data.data_array,
         sim.ant_1_array,
         sim.ant_2_array,
         sim.polarization_array,
         sim.antenna_numbers,
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_vis.py` & `hera_sim-4.0.0/hera_sim/tests/test_vis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 import astropy_healpix as aph
 import copy
-import healvis
 import numpy as np
 from astropy import time as apt
 from astropy import units
 from astropy.coordinates.angles import Latitude, Longitude
 from astropy.units import rad, sday
 from pathlib import Path
 from pyradiosky import SkyModel
@@ -23,21 +22,14 @@
     VisibilitySimulation,
     load_simulator_from_yaml,
 )
 from vis_cpu import HAVE_GPU
 
 SIMULATORS = (VisCPU, UVSim)
 
-try:
-    from hera_sim.visibilities import HealVis
-
-    SIMULATORS = SIMULATORS + (HealVis,)
-except ImportError:
-    pass
-
 if HAVE_GPU:
 
     class VisGPU(VisCPU):
         """Simple mock class to make testing VisCPU with use_gpu=True easier"""
 
         def __init__(self, *args, **kwargs):
             super().__init__(*args, use_gpu=True, **kwargs)
@@ -112,90 +104,14 @@
         uvdataJD,
         ra=np.array([0.0]) * rad,
         dec=np.array(uvdata.telescope_location_lat_lon_alt[0]) * rad,
         align=False,
     )
 
 
-def test_healvis_beam(uvdata, sky_model):
-    pytest.importorskip("healvis")
-    sim = VisibilitySimulation(
-        simulator=HealVis(),
-        data_model=ModelData(
-            uvdata=uvdata,
-            sky_model=sky_model,
-        ),
-        n_side=2**4,
-    )
-
-    assert len(sim.data_model.beams) == 1
-    assert isinstance(sim.data_model.beams[0], healvis.beam_model.AnalyticBeam)
-
-
-def test_healvis_beam_obsparams(tmpdir):
-    # Now try creating with an obsparam file
-    pytest.importorskip("healvis")
-    direc = tmpdir.mkdir("test_healvis_beam")
-
-    with open(Path(__file__).parent / "testdata" / "healvis_catalog.txt") as fl:
-        txt = fl.read()
-
-    with open(direc.join("catalog.txt"), "w") as fl:
-        fl.write(txt)
-
-    with open(direc.join("telescope_config.yml"), "w") as fl:
-        fl.write(
-            """
-    beam_paths:
-        0 : 'uniform'
-    telescope_location: (-30.72152777777791, 21.428305555555557, 1073.0000000093132)
-    telescope_name: MWA
-    """
-        )
-
-    with open(direc.join("layout.csv"), "w") as fl:
-        fl.write(
-            """Name     Number   BeamID   E          N          U
-
-    Tile061        40        0   -34.8010   -41.7365     1.5010
-    Tile062        41        0   -28.0500   -28.7545     1.5060
-    Tile063        42        0   -11.3650   -29.5795     1.5160
-    Tile064        43        0    -9.0610   -20.7885     1.5160
-    """
-        )
-
-    with open(direc.join("obsparams.yml"), "w") as fl:
-        fl.write(
-            """
-    freq:
-      Nfreqs: 1
-      channel_width: 80000.0
-      start_freq: 100000000.0
-    sources:
-      catalog: {0}/catalog.txt
-    telescope:
-      array_layout: {0}/layout.csv
-      telescope_config_name: {0}/telescope_config.yml
-    time:
-      Ntimes: 1
-      integration_time: 11.0
-      start_time: 2458098.38824015
-    """.format(
-                direc.strpath
-            )
-        )
-
-    sim = VisibilitySimulation(
-        data_model=ModelData.from_config(direc.join("obsparams.yml").strpath),
-        simulator=HealVis(),
-    )
-    beam = sim.data_model.beams[0]
-    assert isinstance(beam, healvis.beam_model.AnalyticBeam)
-
-
 def test_JD(uvdata, uvdataJD, sky_model):
     model_data = ModelData(sky_model=sky_model, uvdata=uvdata)
 
     vis = VisCPU()
 
     sim1 = VisibilitySimulation(data_model=model_data, simulator=vis).simulate()
 
@@ -644,31 +560,14 @@
     print(type(pth))
     uvdata.write_uvh5(str(pth))
 
     model_data = ModelData(uvdata=pth, sky_model=sky_model)
     assert model_data.uvdata.Nants_data == uvdata.Nants_data
 
 
-def test_bad_healvis_skymodel(sky_model):
-    pytest.importorskip("healvis")
-    hv = HealVis()
-    sky_model.stokes *= units.sr  # something stupid
-    with pytest.raises(ValueError, match="not compatible with healvis"):
-        hv.get_sky_model(sky_model)
-
-
-def test_mK_healvis_skymodel(sky_model):
-    pytest.importorskip("healvis")
-    hv = HealVis()
-    sky_model.stokes = sky_model.stokes.value * units.mK
-    sky_model.nside = 2**3
-    sky = hv.get_sky_model(sky_model)
-    assert np.isclose(np.sum(sky.data), np.sum(sky_model.stokes[0].value / 1000))
-
-
 def test_ref_time_viscpu(uvdata2):
     vc_mean = VisCPU(ref_time="mean")
     vc_min = VisCPU(ref_time="min")
     vc_max = VisCPU(ref_time="max")
 
     sky_model = half_sky_model(uvdata2)
```

### Comparing `hera_sim-3.1.1/hera_sim/tests/test_yaml_constructors.py` & `hera_sim-4.0.0/hera_sim/tests/test_yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/utils.py` & `hera_sim-4.0.0/hera_sim/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from __future__ import annotations
 
 import numpy as np
 import pyuvdata.utils as uvutils
 import warnings
 from astropy import constants, units
 from astropy.coordinates import Longitude
+from collections.abc import Sequence
 from scipy.interpolate import RectBivariateSpline
-from typing import Sequence
 
 from .interpolators import Beam
 
 try:
     import numba
 
     HAVE_NUMBA = True
@@ -512,15 +512,15 @@
     n_pols: int,
     invert: bool = False,
     use_numba: bool = True,
 ) -> np.ndarray:
     """Reshaping helper for mutual coupling sims.
 
     The mutual coupling simulations take as input, and return, a data array with
-    shape ``(Nblts, 1, Nfreqs, Npols)``, but perform matrix multiplications on
+    shape ``(Nblts, Nfreqs, Npols)``, but perform matrix multiplications on
     the data array reshaped to ``(Ntimes, Nfreqs, 2*Nants, 2*Nants)``. This
     function performs the reshaping between the matrix multiply shape and the
     input/output array shapes.
 
     Parameters
     ----------
     vis
@@ -548,31 +548,33 @@
 
     Returns
     -------
     reshaped_vis
         Input data reshaped to desired shape.
     """
     if invert:
-        out = np.zeros((ant_1_array.size, 1, n_freqs, n_pols), dtype=complex)
+        out = np.zeros((ant_1_array.size, n_freqs, n_pols), dtype=complex)
     else:
         out = np.zeros((n_times, n_freqs, 2 * n_ants, 2 * n_ants), dtype=complex)
 
     # If we have numba, then this is a bit faster.
-    if HAVE_NUMBA and use_numba:
-        return jit_reshape_vis(
+    if HAVE_NUMBA and use_numba:  # pragma: no cover
+        if invert:
+            fnc = jit_reshape_vis_invert
+        else:
+            fnc = jit_reshape_vis
+        fnc(
             vis=vis,
             out=out,
             ant_1_array=ant_1_array,
             ant_2_array=ant_2_array,
             pol_array=pol_array,
             antenna_numbers=antenna_numbers,
-            n_ants=n_ants,
-            n_pols=n_pols,
-            invert=invert,
         )
+        return out
 
     # We don't have numba, so we need to do this a bit more slowly.
     pol_slices = {"x": slice(None, None, 2), "y": slice(1, None, 2)}
     polnum2str = {pol: uvutils.polnum2str(pol) for pol in pol_array}
     for i, ai in enumerate(antenna_numbers):
         for j, aj in enumerate(antenna_numbers[i:]):
             j += i
@@ -590,21 +592,22 @@
 
             for k, pol in enumerate(pol_array):
                 p1, p2 = polnum2str[pol]
                 if flipped:
                     p1, p2 = p2, p1
                 sl1, sl2 = (pol_slices[p.lower()] for p in (p1, p2))
 
+                # NOTE: this is hard-coded to use the new-style UVData shapes!
                 if invert:
                     # Going back to UVData shape
-                    out[uvd_inds, 0, :, k] = vis[:, :, sl1, sl2][:, :, ii, jj]
+                    out[uvd_inds, :, k] = vis[:, :, sl1, sl2][:, :, ii, jj]
                 else:
                     # Changing from UVData shape
-                    out[:, :, sl1, sl2][:, :, ii, jj] = vis[uvd_inds, 0, :, k]
-                    out[:, :, sl2, sl1][:, :, jj, ii] = np.conj(vis[uvd_inds, 0, :, k])
+                    out[:, :, sl1, sl2][:, :, ii, jj] = vis[uvd_inds, :, k]
+                    out[:, :, sl2, sl1][:, :, jj, ii] = np.conj(vis[uvd_inds, :, k])
     return out
 
 
 def matmul(left: np.ndarray, right: np.ndarray, use_numba: bool = False) -> np.ndarray:
     """Helper function for matrix multiplies used in mutual coupling sims.
 
     The :class:`~sigchain.MutualCoupling` class performs two matrix
@@ -687,17 +690,14 @@
     def jit_reshape_vis(
         vis,
         out,
         ant_1_array,
         ant_2_array,
         pol_array,
         antenna_numbers,
-        n_ants,
-        n_pols,
-        invert=False,
     ):
         """JIT-accelerated reshaping function.
 
         See :func:`~reshape_vis` for parameter information.
         """
         # This is basically the same as the non-numba reshape function,
         # but it's not as pretty.
@@ -715,36 +715,87 @@
                     flipped = True
                     ii, jj = j, i
 
                 # Don't do anything if this baseline isn't present.
                 if np.all(~uvd_inds):
                     continue
 
+                uvd_inds = np.argwhere(uvd_inds).flatten()
                 for k, pol in enumerate(pol_array):
                     if pol == -5:
                         p1, p2 = x_sl, x_sl
                     elif pol == -6:
                         p1, p2 = y_sl, y_sl
                     elif pol == -7:
                         p1, p2 = x_sl, y_sl
                     else:
                         p1, p2 = y_sl, x_sl
 
                     if flipped:
                         p1, p2 = p2, p1
 
-                    # NOTE: This is hard-coded to use old-style UVData arrays!
-                    if invert:
-                        # Go back to UVData shape
-                        out[uvd_inds, 0, :, k] = vis[:, :, p1, p2][:, :, ii, jj]
+                    _p = out[:, :, p1, p2]
+                    for tidx, uvd_ind in enumerate(uvd_inds):
+                        _p[tidx, :, ii, jj] = vis[uvd_ind, :, k]
+                        _p[tidx, :, jj, ii] = np.conj(vis[uvd_ind, :, k])
+        return out
+
+    @numba.njit
+    def jit_reshape_vis_invert(
+        vis,
+        out,
+        ant_1_array,
+        ant_2_array,
+        pol_array,
+        antenna_numbers,
+    ):
+        """JIT-accelerated reshaping function.
+
+        See :func:`~reshape_vis` for parameter information.
+        """
+        # This is basically the same as the non-numba reshape function,
+        # but it's not as pretty.
+        x_sl = slice(None, None, 2)
+        y_sl = slice(1, None, 2)
+        for i, ai in enumerate(antenna_numbers):
+            for j, aj in enumerate(antenna_numbers[i:]):
+                j += i
+                uvd_inds = (ant_1_array == ai) & (ant_2_array == aj)
+
+                flipped = False
+                ii, jj = i, j
+                if np.all(~uvd_inds):
+                    uvd_inds = (ant_2_array == ai) & (ant_1_array == aj)
+                    flipped = True
+                    ii, jj = j, i
+
+                # Don't do anything if this baseline isn't present.
+                if np.all(~uvd_inds):
+                    continue
+
+                uvd_inds = np.argwhere(uvd_inds).flatten()
+                for k, pol in enumerate(pol_array):
+                    if pol == -5:
+                        p1, p2 = x_sl, x_sl
+                    elif pol == -6:
+                        p1, p2 = y_sl, y_sl
+                    elif pol == -7:
+                        p1, p2 = x_sl, y_sl
                     else:
-                        out[:, :, p1, p2][:, :, ii, jj] = vis[uvd_inds, 0, :, k]
-                        out[:, :, p2, p1][:, :, jj, ii] = np.conj(
-                            vis[uvd_inds, 0, :, k]
-                        )
+                        p1, p2 = y_sl, x_sl
+
+                    if flipped:
+                        p1, p2 = p2, p1
+
+                    # NOTE: This is hard-coded to use new-style UVData arrays!
+                    # Go back to UVData shape
+                    _p = vis[:, :, p1, p2]
+                    for tidx, uvd_ind in enumerate(uvd_inds):
+                        out[uvd_ind, :, k] = _p[tidx, :, ii, jj]
+                        tidx += 1
         return out
 
     @numba.njit
     def _left_matmul(left, right):
         """JIT-accelerated matrix multiplication.
 
         This multiply assumes the zeroth axis of the ``left`` array is length 1.
```

### Comparing `hera_sim-3.1.1/hera_sim/vis.py` & `hera_sim-4.0.0/hera_sim/vis.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/visibilities/__init__.py` & `hera_sim-4.0.0/hera_sim/visibilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/visibilities/pyuvsim_wrapper.py` & `hera_sim-4.0.0/hera_sim/visibilities/pyuvsim_wrapper.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim/visibilities/simulators.py` & `hera_sim-4.0.0/hera_sim/visibilities/simulators.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 import astropy_healpix as aph
 import importlib
 import numpy as np
 import yaml
 from abc import ABCMeta, abstractmethod
 from astropy import units
 from cached_property import cached_property
+from collections.abc import Sequence
 from dataclasses import dataclass
 from os import path
 from pathlib import Path
 from pyradiosky import SkyModel
 from pyuvdata import UVBeam, UVData
 from pyuvsim import BeamList
 from pyuvsim import analyticbeam as ab
 from pyuvsim.simsetup import (
     _complete_uvdata,
     initialize_catalog_from_params,
     initialize_uvdata_from_params,
     uvdata_to_telescope_config,
 )
-from typing import List, Sequence, Union
+from typing import Union
 
 from .. import __version__
 from .. import visibilities as vis
 
-BeamListType = Union[BeamList, List[Union[ab.AnalyticBeam, UVBeam]]]
+BeamListType = Union[BeamList, list[Union[ab.AnalyticBeam, UVBeam]]]
 
 
 class ModelData:
     """
     An object containing all the information required to perform visibility simulation.
 
     Parameters
```

### Comparing `hera_sim-3.1.1/hera_sim/visibilities/vis_cpu.py` & `hera_sim-4.0.0/hera_sim/visibilities/vis_cpu.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/hera_sim.egg-info/PKG-INFO` & `hera_sim-4.0.0/hera_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-sim
-Version: 3.1.1
+Version: 4.0.0
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
@@ -13,16 +13,17 @@
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: all
 Provides-Extra: bda
 Provides-Extra: cal
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: gpu
 Provides-Extra: tests
 Provides-Extra: vis
```

### Comparing `hera_sim-3.1.1/hera_sim.egg-info/SOURCES.txt` & `hera_sim-4.0.0/hera_sim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/publish.yaml
 .github/workflows/test_suite.yaml
-ci/tests.yaml
 config_examples/simulator.yaml
 config_examples/template_config.yaml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
@@ -107,13 +106,12 @@
 hera_sim/tests/test_simulate_cli.py
 hera_sim/tests/test_simulator.py
 hera_sim/tests/test_utils.py
 hera_sim/tests/test_vis.py
 hera_sim/tests/test_yaml_constructors.py
 hera_sim/tests/testdata/healvis_catalog.txt
 hera_sim/visibilities/__init__.py
-hera_sim/visibilities/healvis_wrapper.py
 hera_sim/visibilities/pyuvsim_wrapper.py
 hera_sim/visibilities/simulators.py
 hera_sim/visibilities/vis_cpu.py
 scripts/hera-sim-simulate.py
 scripts/hera-sim-vis.py
```

### Comparing `hera_sim-3.1.1/scripts/hera-sim-simulate.py` & `hera_sim-4.0.0/scripts/hera-sim-simulate.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/scripts/hera-sim-vis.py` & `hera_sim-4.0.0/scripts/hera-sim-vis.py`

 * *Files identical despite different names*

### Comparing `hera_sim-3.1.1/setup.cfg` & `hera_sim-4.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -25,61 +25,65 @@
 [options]
 packages = find:
 install_requires = 
 	astropy
 	astropy-healpix
 	cached-property
 	deprecation
-	numpy>=1.14
+	numpy>=1.18
 	pyuvdata
-	pyuvsim>=1.1.2
+	pyuvsim>=1.2.5
 	pyyaml>=5.1
 	rich
 	scipy
-python_requires = >=3.8
+python_requires = >=3.9
 include_package_data = True
 scripts = 
 	scripts/hera-sim-simulate.py
 	scripts/hera-sim-vis.py
 zip_safe = False
 
 [options.packages.find]
 exclude = 
 	tests
 
 [options.extras_require]
+all = 
+	hera-sim[vis,bda,cal,gpu]
 bda = 
 	bda
 cal = 
 	hera-calibration
 dev = 
-	vis-cpu[docs,tests]
+	hera-sim[docs,tests]
 docs = 
+	furo
+	hera-sim
 	ipython
 	nbsphinx
-	nbsphinx
 	numpydoc>=0.8
+	pyradiosky>=0.1.2
 	sphinx>=1.8
 	sphinx-autorun
-	vis-cpu[vis]
+	vis-cpu>=1.1.0
 gpu = 
 	pycuda
 	scikit-cuda
 tests = 
 	coverage>=4.5.1
+	hera-sim[bda,cal,vis]
 	matplotlib>=3.4.2
 	pre-commit
 	pytest>=3.5.1
 	pytest-cov>=2.5.1
 	uvtools
-	vis-cpu[vis,bda,cal]
 vis = 
 	mpi4py
 	pyradiosky>=0.1.2
-	vis-cpu>=1.0.0
+	vis-cpu>=1.1.0
 
 [tool:pytest]
 addopts = 
 	--cov hera_sim
 	--cov-config=.coveragerc
 	--cov-report xml:./coverage.xml
 	--durations=25
```

