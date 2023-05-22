# Comparing `tmp/qibocal-0.0.1.tar.gz` & `tmp/qibocal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibocal-0.0.1.tar", max compression
+gzip compressed data, was "qibocal-0.0.2.tar", max compression
```

## Comparing `qibocal-0.0.1.tar` & `qibocal-0.0.2.tar`

### file list

```diff
@@ -1,65 +1,113 @@
--rw-r--r--   0        0        0    11357 2022-10-10 12:20:52.086574 qibocal-0.0.1/LICENSE
--rw-r--r--   0        0        0     2671 2023-02-17 19:44:30.094586 qibocal-0.0.1/README.md
--rw-r--r--   0        0        0     2358 2023-02-21 18:01:19.030128 qibocal-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      201 2023-02-17 19:44:30.158587 qibocal-0.0.1/src/qibocal/__init__.py
--rw-r--r--   0        0        0      655 2023-02-17 19:44:30.158587 qibocal-0.0.1/src/qibocal/calibrations/__init__.py
--rw-r--r--   0        0        0        0 2022-10-11 12:24:43.694595 qibocal-0.0.1/src/qibocal/calibrations/characterization/__init__.py
--rw-r--r--   0        0        0    17566 2023-02-17 19:44:30.158587 qibocal-0.0.1/src/qibocal/calibrations/characterization/allXY.py
--rw-r--r--   0        0        0     3920 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/calibrate_qubit_states.py
--rw-r--r--   0        0        0     5397 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/flipping.py
--rw-r--r--   0        0        0    15453 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/qubit_spectroscopy.py
--rw-r--r--   0        0        0    23825 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/rabi.py
--rw-r--r--   0        0        0    15142 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/ramsey.py
--rw-r--r--   0        0        0    25596 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/resonator_spectroscopy.py
--rw-r--r--   0        0        0    14471 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/resonator_spectroscopy_sample.py
--rw-r--r--   0        0        0     4609 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/spin_echo.py
--rw-r--r--   0        0        0     4873 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/characterization/t1.py
--rw-r--r--   0        0        0     9028 2023-02-21 08:14:43.061601 qibocal-0.0.1/src/qibocal/calibrations/niGSC/XIdrb.py
--rw-r--r--   0        0        0        0 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/__init__.py
--rw-r--r--   0        0        0     4957 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/circuitfactory.py
--rw-r--r--   0        0        0     9436 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/experiment.py
--rw-r--r--   0        0        0     6335 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/fitting.py
--rw-r--r--   0        0        0     1785 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/noisemodels.py
--rw-r--r--   0        0        0     5196 2023-02-21 08:14:43.061601 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/plot.py
--rw-r--r--   0        0        0     4707 2023-02-21 08:14:43.061601 qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/utils.py
--rw-r--r--   0        0        0     9639 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/simulfilteredrb.py
--rw-r--r--   0        0        0     8522 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/calibrations/niGSC/standardrb.py
--rw-r--r--   0        0        0       78 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/cli/__init__.py
--rw-r--r--   0        0        0     9992 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/cli/_base.py
--rw-r--r--   0        0        0    14378 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/cli/builders.py
--rw-r--r--   0        0        0     1754 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/config.py
--rw-r--r--   0        0        0    14927 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/data.py
--rw-r--r--   0        0        0      591 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/decorators.py
--rw-r--r--   0        0        0        0 2022-10-11 12:24:43.694595 qibocal-0.0.1/src/qibocal/fitting/__init__.py
--rw-r--r--   0        0        0    35763 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/fitting/methods.py
--rw-r--r--   0        0        0     4712 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/fitting/utils.py
--rw-r--r--   0        0        0      302 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/__init__.py
--rw-r--r--   0        0        0    10259 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/allXY.py
--rw-r--r--   0        0        0     5862 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/calibrate_qubit_states.py
--rw-r--r--   0        0        0     4533 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/flipping.py
--rw-r--r--   0        0        0    22813 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/rabi.py
--rw-r--r--   0        0        0     4808 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/ramsey.py
--rw-r--r--   0        0        0    35402 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/spectroscopies.py
--rw-r--r--   0        0        0     4768 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/spin_echo.py
--rw-r--r--   0        0        0     4244 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/t1.py
--rw-r--r--   0        0        0      641 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/plots/utils.py
--rw-r--r--   0        0        0      527 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/niGSC.yml
--rw-r--r--   0        0        0    10312 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/test_data.py
--rw-r--r--   0        0        0    14041 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/test_fitting_methods.py
--rw-r--r--   0        0        0     4531 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/test_niGSC_circuitfactory.py
--rw-r--r--   0        0        0     7397 2023-02-21 08:14:43.065601 qibocal-0.0.1/src/qibocal/tests/test_niGSC_experiment.py
--rw-r--r--   0        0        0     3951 2023-02-21 08:14:43.065601 qibocal-0.0.1/src/qibocal/tests/test_niGSC_fitting.py
--rw-r--r--   0        0        0     1724 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/test_niGSC_noisemodels.py
--rw-r--r--   0        0        0     1312 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/tests/test_niGSC_qq.py
--rw-r--r--   0        0        0     7807 2023-02-21 08:14:43.065601 qibocal-0.0.1/src/qibocal/tests/test_niGSC_simulfilteredrb.py
--rw-r--r--   0        0        0     7723 2023-02-21 08:14:43.065601 qibocal-0.0.1/src/qibocal/tests/test_niGSC_standardrb.py
--rw-r--r--   0        0        0     5559 2023-02-21 08:14:43.065601 qibocal-0.0.1/src/qibocal/tests/test_niGSC_xidrb.py
--rw-r--r--   0        0        0        0 2022-10-11 12:24:43.694595 qibocal-0.0.1/src/qibocal/web/__init__.py
--rw-r--r--   0        0        0     5651 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/web/app.py
--rw-r--r--   0        0        0      842 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/web/report.py
--rw-r--r--   0        0        0     3027 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/web/server.py
--rw-r--r--   0        0        0     4300 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/web/static/styles.css
--rw-r--r--   0        0        0    13213 2023-02-17 19:44:30.162587 qibocal-0.0.1/src/qibocal/web/templates/template.html
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 qibocal-0.0.1/setup.py
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 qibocal-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 14:14:48.508111 qibocal-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2780 2023-05-22 14:14:48.508111 qibocal-0.0.2/README.md
+-rw-r--r--   0        0        0     3457 2023-05-22 14:14:48.608110 qibocal-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/draw.py
+-rw-r--r--   0        0        0     4127 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/execute.py
+-rw-r--r--   0        0        0     2021 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/graph.py
+-rw-r--r--   0        0        0     1079 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/history.py
+-rw-r--r--   0        0        0     4169 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/operation.py
+-rw-r--r--   0        0        0     1711 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/runcard.py
+-rw-r--r--   0        0        0     1179 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/status.py
+-rw-r--r--   0        0        0     2694 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/task.py
+-rw-r--r--   0        0        0      663 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/auto/validate.py
+-rw-r--r--   0        0        0      845 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/__init__.py
+-rw-r--r--   0        0        0    17522 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/allXY.py
+-rw-r--r--   0        0        0     3866 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/calibrate_qubit_states.py
+-rw-r--r--   0        0        0     9028 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/chevron.py
+-rw-r--r--   0        0        0    19407 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/cryoscope.py
+-rw-r--r--   0        0        0     5391 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/flipping.py
+-rw-r--r--   0        0        0    10582 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/qubit_spectroscopy.py
+-rw-r--r--   0        0        0    23727 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/rabi.py
+-rw-r--r--   0        0        0    15138 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/ramsey.py
+-rw-r--r--   0        0        0    24494 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/resonator_spectroscopy.py
+-rw-r--r--   0        0        0    14471 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/resonator_spectroscopy_sample.py
+-rw-r--r--   0        0        0    17740 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/ro_optimization.py
+-rw-r--r--   0        0        0     4603 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/spin_echo.py
+-rw-r--r--   0        0        0     4884 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/characterization/t1.py
+-rw-r--r--   0        0        0     8679 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/XIdrb.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/__init__.py
+-rw-r--r--   0        0        0     5069 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/circuitfactory.py
+-rw-r--r--   0        0        0     9394 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/experiment.py
+-rw-r--r--   0        0        0     7683 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/fitting.py
+-rw-r--r--   0        0        0     1776 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/noisemodels.py
+-rw-r--r--   0        0        0     5245 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/plot.py
+-rw-r--r--   0        0        0     3095 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/utils.py
+-rw-r--r--   0        0        0    10093 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/simulfilteredrb.py
+-rw-r--r--   0        0        0     8689 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/calibrations/niGSC/standardrb.py
+-rw-r--r--   0        0        0       95 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/cli/__init__.py
+-rw-r--r--   0        0        0     7911 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/cli/_base.py
+-rw-r--r--   0        0        0     3497 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/cli/auto_builder.py
+-rw-r--r--   0        0        0    13177 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/cli/builders.py
+-rw-r--r--   0        0        0     3756 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/cli/utils.py
+-rw-r--r--   0        0        0     1754 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/config.py
+-rw-r--r--   0        0        0    14927 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/data.py
+-rw-r--r--   0        0        0      591 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/ada_boost.py
+-rw-r--r--   0        0        0     1938 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/data.py
+-rw-r--r--   0        0        0      801 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/gaussian_process.py
+-rw-r--r--   0        0        0      689 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/linear_svm.py
+-rw-r--r--   0        0        0      643 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/naive_bayes.py
+-rw-r--r--   0        0        0     4251 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/nn.py
+-rw-r--r--   0        0        0     5821 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/plots.py
+-rw-r--r--   0        0        0     1608 2023-05-22 14:14:48.608110 qibocal-0.0.2/src/qibocal/fitting/classifier/qblox_fit.py
+-rw-r--r--   0        0        0     3807 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/classifier/qubit_fit.py
+-rw-r--r--   0        0        0     1138 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/classifier/random_forest.py
+-rw-r--r--   0        0        0     1024 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/classifier/rbf_svm.py
+-rw-r--r--   0        0        0    10514 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/classifier/run.py
+-rw-r--r--   0        0        0      353 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/classifier/utils.py
+-rw-r--r--   0        0        0    39873 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/methods.py
+-rw-r--r--   0        0        0     5394 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/fitting/utils.py
+-rw-r--r--   0        0        0      420 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/__init__.py
+-rw-r--r--   0        0        0     9952 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/allXY.py
+-rw-r--r--   0        0        0     5731 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/calibrate_qubit_states.py
+-rw-r--r--   0        0        0     8237 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/chevron.py
+-rw-r--r--   0        0        0    52739 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/cryoscope.py
+-rw-r--r--   0        0        0     4532 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/flipping.py
+-rw-r--r--   0        0        0    21679 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/rabi.py
+-rw-r--r--   0        0        0     4793 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/ramsey.py
+-rw-r--r--   0        0        0    18406 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/ro_optimization.py
+-rw-r--r--   0        0        0    40623 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/spectroscopies.py
+-rw-r--r--   0        0        0     4785 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/spin_echo.py
+-rw-r--r--   0        0        0     4256 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/t1.py
+-rw-r--r--   0        0        0     1136 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/plots/utils.py
+-rw-r--r--   0        0        0     1554 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/allxy/__init__.py
+-rw-r--r--   0        0        0     7407 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/allxy/allxy.py
+-rw-r--r--   0        0        0     4715 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py
+-rw-r--r--   0        0        0     7785 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/allxy/drag_pulse_tuning.py
+-rw-r--r--   0        0        0    11594 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/classification.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/coherence/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/coherence/spin_echo.py
+-rw-r--r--   0        0        0     5700 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/coherence/t1.py
+-rw-r--r--   0        0        0     4883 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/coherence/t2.py
+-rw-r--r--   0        0        0     1667 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/coherence/utils.py
+-rw-r--r--   0        0        0    10475 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/dispersive_shift.py
+-rw-r--r--   0        0        0     8115 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/flipping.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/flux_depedence/__init__.py
+-rw-r--r--   0        0        0     4289 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/flux_depedence/qubit_flux_dependence.py
+-rw-r--r--   0        0        0     4165 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/flux_depedence/resonator_flux_dependence.py
+-rw-r--r--   0        0        0     1584 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/flux_depedence/utils.py
+-rw-r--r--   0        0        0     4652 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/qubit_spectroscopy.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/rabi/__init__.py
+-rw-r--r--   0        0        0     6138 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/rabi/amplitude.py
+-rw-r--r--   0        0        0     5985 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/rabi/length.py
+-rw-r--r--   0        0        0     3585 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/rabi/utils.py
+-rw-r--r--   0        0        0    10002 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/ramsey.py
+-rw-r--r--   0        0        0     8990 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/resonator_punchout.py
+-rw-r--r--   0        0        0    11509 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py
+-rw-r--r--   0        0        0     6799 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/resonator_spectroscopy.py
+-rw-r--r--   0        0        0     6943 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/protocols/characterization/utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/__init__.py
+-rw-r--r--   0        0        0     5527 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/app.py
+-rw-r--r--   0        0        0     1522 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/report.py
+-rw-r--r--   0        0        0     3027 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/server.py
+-rw-r--r--   0        0        0     4300 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/static/styles.css
+-rw-r--r--   0        0        0    10341 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/templates/autocalibration.html
+-rw-r--r--   0        0        0    15133 2023-05-22 14:14:48.612110 qibocal-0.0.2/src/qibocal/web/templates/template.html
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 qibocal-0.0.2/PKG-INFO
```

### Comparing `qibocal-0.0.1/LICENSE` & `qibocal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/README.md` & `qibocal-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Qibocal
 ![Tests](https://github.com/qiboteam/qibocal/workflows/Tests/badge.svg)
-[![codecov](https://codecov.io/gh/qiboteam/qibocal/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibo)
+[![codecov](https://codecov.io/gh/qiboteam/qibocal/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibocal)
 [![Documentation Status](https://readthedocs.org/projects/qibocal/badge/?version=latest)](https://qibocal.readthedocs.io/en/latest/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7662185.svg)](https://doi.org/10.5281/zenodo.7662185)
 
 Qibocal provides Quantum Characterization Validation and Verification protocols using [Qibo](https://github.com/qiboteam/qibo) and [Qibolab](https://github.com/qiboteam/qibolab).
 
 Qibocal key features:
 
 - Automatization of calibration routines.
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
 # Qibocal ![Tests](https://github.com/qiboteam/qibocal/workflows/Tests/
 badge.svg) [![codecov](https://codecov.io/gh/qiboteam/qibocal/branch/main/
-graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibo) [!
+graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibocal) [!
 [Documentation Status](https://readthedocs.org/projects/qibocal/badge/
-?version=latest)](https://qibocal.readthedocs.io/en/latest/) Qibocal provides
-Quantum Characterization Validation and Verification protocols using [Qibo]
-(https://github.com/qiboteam/qibo) and [Qibolab](https://github.com/qiboteam/
-qibolab). Qibocal key features: - Automatization of calibration routines. -
-Declarative inputs using runcard. - Generation of a report. ## Installation The
-package can be installed by source: ```sh git clone https://github.com/
-qiboteam/qibocal.git cd qibocal pip install . ``` ### Developer instructions
-For development make sure to install the package using [`poetry`](https://
-python-poetry.org/) and to install the pre-commit hooks: ```sh git clone https:
-//github.com/qiboteam/qibocal.git cd qibocal poetry install pre-commit install
-``` ## Minimal working example This section shows the steps to perform a
-resonator spectroscopy with Qibocal. ### Write a runcard A runcard contains all
-the essential information to run a specific task. For our purposes, we can use
-the following: ```yml platform: tii1q qubits: [0] format: csv actions:
-resonator_spectroscopy: lowres_width: 5_000_000 lowres_step: 2_000_000
-highres_width: 1_500_000 highres_step: 200_000 precision_width: 1_500_000
-precision_step: 100_000 software_averages: 1 points: 5 ``` ### Run the routine
-To run all the calibration routines specified in the ```runcard```, Qibocal
-uses the `qq` command ```sh qq  -o  ``` if `````` is specified, the results
-will be saved in it, otherwise ```qq``` will automatically create a default
-folder containing the current date and the username. ### Visualize the data
-Qibocal gives the possibility to live-plotting with the `qq-live` command ```sh
-qq-live  ``` ### Uploading reports to server In order to upload the report to a
-centralized server, send to the server administrators your public ssh key (from
-the machine(s) you are planning to upload the report) and then use the `qq-
-upload ` command. This program will upload your report to the server and
-generate an unique URL. ## Contributing Contributions, issues and feature
-requests are welcome! Feel free to check [GitHub_issues]
+?version=latest)](https://qibocal.readthedocs.io/en/latest/) [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.7662185.svg)](https://doi.org/10.5281/
+zenodo.7662185) Qibocal provides Quantum Characterization Validation and
+Verification protocols using [Qibo](https://github.com/qiboteam/qibo) and
+[Qibolab](https://github.com/qiboteam/qibolab). Qibocal key features: -
+Automatization of calibration routines. - Declarative inputs using runcard. -
+Generation of a report. ## Installation The package can be installed by source:
+```sh git clone https://github.com/qiboteam/qibocal.git cd qibocal pip install
+. ``` ### Developer instructions For development make sure to install the
+package using [`poetry`](https://python-poetry.org/) and to install the pre-
+commit hooks: ```sh git clone https://github.com/qiboteam/qibocal.git cd
+qibocal poetry install pre-commit install ``` ## Minimal working example This
+section shows the steps to perform a resonator spectroscopy with Qibocal. ###
+Write a runcard A runcard contains all the essential information to run a
+specific task. For our purposes, we can use the following: ```yml platform:
+tii1q qubits: [0] format: csv actions: resonator_spectroscopy: lowres_width:
+5_000_000 lowres_step: 2_000_000 highres_width: 1_500_000 highres_step: 200_000
+precision_width: 1_500_000 precision_step: 100_000 software_averages: 1 points:
+5 ``` ### Run the routine To run all the calibration routines specified in the
+```runcard```, Qibocal uses the `qq` command ```sh qq  -o  ``` if `````` is
+specified, the results will be saved in it, otherwise ```qq``` will
+automatically create a default folder containing the current date and the
+username. ### Visualize the data Qibocal gives the possibility to live-plotting
+with the `qq-live` command ```sh qq-live  ``` ### Uploading reports to server
+In order to upload the report to a centralized server, send to the server
+administrators your public ssh key (from the machine(s) you are planning to
+upload the report) and then use the `qq-upload ` command. This program will
+upload your report to the server and generate an unique URL. ## Contributing
+Contributions, issues and feature requests are welcome! Feel free to check
+[GitHub_issues]
```

### Comparing `qibocal-0.0.1/pyproject.toml` & `qibocal-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,109 @@
 [tool.poetry]
 name = "qibocal"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["andrea-pasquale <andreapasquale97@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/qiboteam/qibocal/"
 documentation = ""
 keywords = []
-classifiers=[
-    "Programming Language :: Python :: 3",
-    "Topic :: Scientific/Engineering :: Physics",
-    ]
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "Topic :: Scientific/Engineering :: Physics",
+]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <4"
-qibolab = "^0.0.1"
+python = ">=3.8,<3.12"
+qibolab = "0.0.3"
 qibo = "^0.1.9"
 pandas = "^1.4.3"
 Pint-Pandas = "^0.3"
 dash = "^2.6.0"
 lmfit = "^1.0.3"
 # docs dependencies (for readthedocs, https://github.com/readthedocs/readthedocs.org/issues/4912#issuecomment-664002569)
-Sphinx = { version = "^4.3.2", optional = true }
-furo = { version = "^2022.9.29", optional = true }
+Sphinx = { version = "^5.0.0", optional = true }
+furo = { version = "^2023.3.27", optional = true }
 sphinxcontrib-bibtex = { version = "^2.4.1", optional = true }
 recommonmark = { version = "^0.7.1", optional = true }
 sphinx_markdown_tables = { version = "^0.0.17", optional = true }
+scikit-learn = { version = "^1.2.1", optional = true}
+keras-tuner = { version = "^1.3.0,<1.3.1", optional = true, markers = "sys_platform == 'linux' or sys_platform == 'darwin'"}
+matplotlib = { version = "^3.7.0", optional = true }
+seaborn = { version = "^0.12.2", optional = true }
+networkx = "^3.0"
+pydantic = "^1.10.5"
+pydot = { version = "^1.4.2", optional = true }
+tensorflow = { version = "^2.12.0", optional = true, markers = "sys_platform == 'linux' or sys_platform == 'darwin'"}
+# TODO: the marker is a temporary solution due to the lack of the tensorflow-io 0.32.0's wheels for Windows, this package is one of
+# the tensorflow requirements
+pint = "^0.20.1" # The new version of pint (0.21) is incompatible with Pint-Pandas
+
+[tool.poetry.group.test]
+optional = true
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
 pylint = "2.12.2"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
-poethepoet = "^0.16.0"
-Sphinx = "^4.3.2"
-furo = "^2022.9.29"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^5.0.0"
+furo = "^2023.3.27"
 sphinxcontrib-bibtex = "^2.4.1"
 recommonmark = "^0.7.1"
 sphinx_markdown_tables = "^0.0.17"
 
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+pdbpp = "^0.10.3"
+ipython = "^8.0"
+devtools = "^0.10.0"
+
 [tool.poetry.extras]
-docs = ["sphinx", "furo", "sphinxcontrib-bibtex", "recommonmark", "sphinx_markdown_tables"]
+
+classify = ["scikit-learn", "tensorflow", "keras-tuner", "matplotlib", "seaborn"]
+docs = [
+  "sphinx",
+  "furo",
+  "sphinxcontrib-bibtex",
+  "recommonmark",
+  "sphinx_markdown_tables",
+]
+viz = ["pydot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 qq = "qibocal:command"
 qq-live = "qibocal:live_plot"
 qq-upload = "qibocal:upload"
 qq-compare = "qibocal:compare"
+qq-auto = "qibocal:autocalibration"
 
 [tool.poe.tasks]
-test = "pytest src/qibocal/tests"
+test = "pytest"
 lint = "pylint src/**/*.py -E"
 lint-warnings = "pylint src/**/*.py --exit-zero"
 docs = "make -C doc html"
 docs-clean = "make -C doc clean"
 test-docs = "make -C doc doctest"
 
 [tool.pytest.ini_options]
-testpaths = ['src/qibocal/tests/']
-addopts = [
-    '--cov=qibocal',
-    '--cov-report=xml'
-]
+testpaths = ['tests/']
+addopts = ['--cov=qibocal', '--cov-report=xml', '--cov-report=html']
 
 [tool.pylint.master]
 # extensions not to check
 extension-pkg-whitelist = ["numpy"]
 jobs = 1
 
 [tool.pylint.messages_control]
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/__init__.py` & `qibocal-0.0.2/src/qibocal/calibrations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from qibocal.calibrations.characterization.allXY import *
 from qibocal.calibrations.characterization.calibrate_qubit_states import *
+from qibocal.calibrations.characterization.chevron import *
+from qibocal.calibrations.characterization.cryoscope import *
 from qibocal.calibrations.characterization.flipping import *
 from qibocal.calibrations.characterization.qubit_spectroscopy import *
 from qibocal.calibrations.characterization.rabi import *
 from qibocal.calibrations.characterization.ramsey import *
 from qibocal.calibrations.characterization.resonator_spectroscopy import *
 from qibocal.calibrations.characterization.resonator_spectroscopy_sample import *
+from qibocal.calibrations.characterization.ro_optimization import *
 from qibocal.calibrations.characterization.spin_echo import *
 from qibocal.calibrations.characterization.t1 import *
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/allXY.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/allXY.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     )
 
     count = 0
     # repeat the experiment as many times as defined by software_averages
     for iteration in range(software_averages):
         gateNumber = 1
         # sweep the parameter
-        for gates in gatelist:
+        for gateNumber, gates in enumerate(gatelist):
             # save data as often as defined by points
             if count % points == 0 and count > 0:
                 # save data
                 yield data
 
             # create a sequence of pulses
             ro_pulses = {}
@@ -106,15 +106,14 @@
                     "gateNumber": gateNumber,
                     "beta_param": beta_param,
                     "qubit": ro_pulse.qubit,
                     "iteration": iteration,
                 }
                 data.add(r)
             count += 1
-            gateNumber += 1
     # finally, save the remaining data
     yield data
 
 
 @plot("Probability vs Gate Sequence", plots.allXY_drag_pulse_tuning)
 def allXY_drag_pulse_tuning(
     platform: AbstractPlatform,
@@ -356,17 +355,15 @@
         labels=["optimal_beta_param"],
     )
 
 
 def _add_gate_pair_pulses_to_sequence(
     platform: AbstractPlatform, gates, qubit, beta_param, sequence
 ):
-    pulse_duration = platform.settings["native_gates"]["single_qubit"][qubit]["RX"][
-        "duration"
-    ]
+    pulse_duration = platform.create_RX_pulse(qubit, start=0).duration
     # All gates have equal pulse duration
 
     sequenceDuration = 0
     pulse_start = 0
 
     for gate in gates:
         if gate == "I":
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/calibrate_qubit_states.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/calibrate_qubit_states.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 @plot("Qubit States", plots.qubit_states)
 def calibrate_qubit_states(
     platform: AbstractPlatform,
     qubits: dict,
     nshots,
-    points=10,
 ):
     """
     Method which implements the state's calibration of a chosen qubit. Two analogous tests are performed
     for calibrate the ground state and the excited state of the oscillator.
     The subscripts `exc` and `gnd` will represent the excited state |1> and the ground state |0>.
 
     Args:
@@ -52,51 +51,52 @@
     state1_sequence = PulseSequence()
 
     RX_pulses = {}
     ro_pulses = {}
     for qubit in qubits:
         RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=RX_pulses[qubit].duration
+            qubit, start=RX_pulses[qubit].finish
         )
 
         state0_sequence.add(ro_pulses[qubit])
         state1_sequence.add(RX_pulses[qubit])
         state1_sequence.add(ro_pulses[qubit])
 
     # create a DataUnits object to store the results
     data = DataUnits(name="data", options=["qubit", "iteration", "state"])
 
     # execute the first pulse sequence
     state0_results = platform.execute_pulse_sequence(state0_sequence, nshots=nshots)
 
     # retrieve and store the results for every qubit
     for ro_pulse in ro_pulses.values():
-        r = state0_results[ro_pulse.serial].to_dict(average=False)
+        r = state0_results[ro_pulse.serial].raw
         r.update(
             {
                 "qubit": [ro_pulse.qubit] * nshots,
                 "iteration": np.arange(nshots),
                 "state": [0] * nshots,
             }
         )
         data.add_data_from_dict(r)
 
     # execute the second pulse sequence
     state1_results = platform.execute_pulse_sequence(state1_sequence, nshots=nshots)
 
     # retrieve and store the results for every qubit
     for ro_pulse in ro_pulses.values():
-        r = state1_results[ro_pulse.serial].to_dict(average=False)
+        r = state1_results[ro_pulse.serial].raw
         r.update(
             {
                 "qubit": [ro_pulse.qubit] * nshots,
                 "iteration": np.arange(nshots),
                 "state": [1] * nshots,
             }
         )
         data.add_data_from_dict(r)
+
     # finally, save the remaining data and the fits
     yield data
     yield calibrate_qubit_states_fit(
         data, x="i[V]", y="q[V]", nshots=nshots, qubits=qubits
     )
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/flipping.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/flipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 sequence.add(ro_pulses[qubit])
 
             # execute the pulse sequence
             results = platform.execute_pulse_sequence(sequence)
 
             for ro_pulse in ro_pulses.values():
                 # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
+                r = results[ro_pulse.serial].raw
                 r.update(
                     {
                         "flips[dimensionless]": flips,
                         "qubit": ro_pulse.qubit,
                         "iteration": iteration,
                     }
                 )
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/qubit_spectroscopy.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/ramsey.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,384 +1,380 @@
 import numpy as np
 from qibolab.platforms.abstract import AbstractPlatform
 from qibolab.pulses import PulseSequence
 
 from qibocal import plots
-from qibocal.config import raise_error
 from qibocal.data import DataUnits
 from qibocal.decorators import plot
-from qibocal.fitting.methods import lorentzian_fit
+from qibocal.fitting.methods import ramsey_fit
 
 
-@plot("MSR and Phase vs Qubit Drive Frequency", plots.frequency_msr_phase)
-def qubit_spectroscopy(
+@plot("MSR vs Time", plots.time_msr)
+def ramsey_frequency_detuned(
     platform: AbstractPlatform,
     qubits: dict,
-    fast_width,
-    fast_step,
-    precision_width,
-    precision_step,
+    delay_between_pulses_start,
+    delay_between_pulses_end,
+    delay_between_pulses_step,
+    n_osc,
     software_averages=1,
     points=10,
 ):
     r"""
-    Perform spectroscopy on the qubit.
-    This routine executes a fast scan around the expected qubit frequency indicated in the platform runcard.
-    Afterthat, a final sweep with more precision is executed centered in the new qubit frequency found.
+    We introduce an artificial detune over the drive pulse frequency to be off-resonance and, after fitting,
+    determine two of the qubit's properties: Ramsey or detuning frequency and T2. If our drive pulse is well
+    calibrated, the Ramsey experiment without artificial detuning results in an exponential that describes T2,
+    but we can not refine the detuning frequency.
+
+    In this method we iterate over diferent maximum time delays between the drive pulses of the ramsey sequence
+    in order to refine the fitted detuning frequency and T2.
+
+    Ramsey sequence: Rx(pi/2) - wait time - Rx(pi/2) - ReadOut
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
         qubits (dict): Dict of target Qubit objects to perform the action
-        fast_start (int): Initial frequency in HZ to perform the qubit fast sweep
-        fast_width (int): Width frequency in HZ to perform the high resolution sweep
-        fast_step (int): Step frequency in HZ for the high resolution sweep
-        precision_width (int): Width frequency in HZ to perform the precision resolution sweep
-        precision_step (int): Step frequency in HZ for the precission resolution sweep
+        delay_between_pulses_start (int): Initial time delay between drive pulses in the Ramsey sequence
+        delay_between_pulses_end (list): List of maximum time delays between drive pulses in the Ramsey sequence
+        delay_between_pulses_step (int): Scan range step for the time delay between drive pulses in the Ramsey sequence
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
 
     Returns:
-        - Two DataUnits objects with the raw data obtained for the fast and precision sweeps with the following keys
+        - A DataUnits object with the raw data obtained for the fast and precision sweeps with the following keys
 
             - **MSR[V]**: Resonator signal voltage mesurement in volts
             - **i[V]**: Resonator signal voltage mesurement for the component I in volts
             - **q[V]**: Resonator signal voltage mesurement for the component Q in volts
             - **phase[rad]**: Resonator signal phase mesurement in radians
-            - **frequency[Hz]**: Qubit drive frequency value in Hz
+            - **wait[ns]**: Wait time used in the current Ramsey execution
+            - **t_max[ns]**: Maximum time delay between drive pulses in the Ramsey sequence
             - **qubit**: The qubit being tested
             - **iteration**: The iteration number of the many determined by software_averages
 
         - A DataUnits object with the fitted data obtained with the following keys
 
+            - **delta_frequency**: Physical detunning of the actual qubit frequency
+            - **drive_frequency**:
+            - **T2**: New qubit frequency after correcting the actual qubit frequency with the detunning calculated
+            - **popt0**: offset
+            - **popt1**: oscillation amplitude
+            - **popt2**: frequency
+            - **popt3**: phase
+            - **popt4**: T2
             - **qubit**: The qubit being tested
-            - **drive_frequency**: frequency
-            - **peak_voltage**: peak voltage
-            - **popt0**: Lorentzian's amplitude
-            - **popt1**: Lorentzian's center
-            - **popt2**: Lorentzian's sigma
-            - **popt3**: Lorentzian's offset
     """
 
     # reload instrument settings from runcard
     platform.reload_settings()
 
-    # create a sequence of pulses for the experiment:
-    # long drive probing pulse - MZ
-
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence = PulseSequence()
+    # create a sequence of pulses for the experiment
+    # RX90 - wait t - RX90 - MZ
     ro_pulses = {}
-    qd_pulses = {}
+    RX90_pulses1 = {}
+    RX90_pulses2 = {}
+    sequence = PulseSequence()
     for qubit in qubits:
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=0, duration=5000
+        RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
+        RX90_pulses1[qubit].frequency = qubits[qubit].drive_frequency
+        RX90_pulses2[qubit] = platform.create_RX90_pulse(
+            qubit, start=RX90_pulses1[qubit].finish
+        )
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=RX90_pulses2[qubit].finish
         )
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=5000)
-        sequence.add(qd_pulses[qubit])
+        sequence.add(RX90_pulses1[qubit])
+        sequence.add(RX90_pulses2[qubit])
         sequence.add(ro_pulses[qubit])
 
-    # define the parameter to sweep and its range:
-    delta_frequency_range = np.arange(-fast_width // 2, fast_width // 2, fast_step)
+    sampling_rate = platform.sampling_rate
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
-    # additionally include qubit frequency
-    fast_sweep_data = DataUnits(
-        name="fast_sweep_data",
-        quantities={"frequency": "Hz"},
+    # additionally include wait time and t_max
+    data = DataUnits(
+        name="data",
+        quantities={"wait": "ns", "t_max": "ns"},
         options=["qubit", "iteration"],
     )
 
+    delay_between_pulses_end = np.array(delay_between_pulses_end)
     # repeat the experiment as many times as defined by software_averages
     count = 0
-    for iteration in range(software_averages):
-        # sweep the parameter
-        for delta_freq in delta_frequency_range:
-            # save data as often as defined by points
-            if count % points == 0 and count > 0:
-                # save data
-                yield fast_sweep_data
-                # calculate and save fit
-                yield lorentzian_fit(
-                    fast_sweep_data,
-                    x="frequency[Hz]",
-                    y="MSR[uV]",
-                    qubits=qubits,
-                    resonator_type=platform.resonator_type,
-                    labels=["drive_frequency", "peak_voltage"],
-                )
-            # reconfigure the instruments based on the new resonator frequency
-            # in this case setting the local oscillators
-            # the pulse sequence does not need to be modified or recreated between executions
-            for qubit in qubits:
-                qd_pulses[qubit].frequency = delta_freq + qubits[qubit].drive_frequency
-
-            # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
-
-            # retrieve the results for every qubit
-            for ro_pulse in ro_pulses.values():
-                # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
-                # store the results
-                r.update(
-                    {
-                        "frequency[Hz]": qd_pulses[ro_pulse.qubit].frequency,
-                        "qubit": ro_pulse.qubit,
-                        "iteration": iteration,
-                    }
-                )
-                fast_sweep_data.add(r)
-            count += 1
-    # finally, save the remaining data and fits
-    yield fast_sweep_data
-    yield lorentzian_fit(
-        fast_sweep_data,
-        x="frequency[Hz]",
-        y="MSR[uV]",
-        qubits=qubits,
-        resonator_type=platform.resonator_type,
-        labels=["drive_frequency", "peak_voltage"],
-    )
+    for t_max in delay_between_pulses_end:
+        for iteration in range(software_averages):
+            count = 0
+            offset_freq = n_osc / t_max * sampling_rate  # Hz
+
+            # define the parameter to sweep and its range:
+            # wait time between RX90 pulses
+            t_range = np.arange(
+                delay_between_pulses_start, t_max, delay_between_pulses_step
+            )
 
-    # store max/min peaks as new frequencies
-    for qubit in qubits:
-        qubit_data = (
-            fast_sweep_data.df[fast_sweep_data.df["qubit"] == qubit]
-            .drop(columns=["qubit", "iteration"])
-            .groupby("frequency", as_index=False)
-            .mean()
-        )
-        if platform.resonator_type == "3D":
-            qubits[qubit].drive_frequency = (
-                qubit_data["frequency"][
-                    np.argmin(qubit_data["MSR"].pint.to("V").pint.magnitude)
-                ]
-                .to("Hz")
-                .magnitude
+            # sweep the parameter
+            for wait in t_range:
+                # save data as often as defined by points
+                if count % points == 0 and count > 0:
+                    # save data
+                    yield data
+                    # calculate and save fit
+                    yield ramsey_fit(
+                        data,
+                        x="wait[ns]",
+                        y="MSR[uV]",
+                        qubits=qubits,
+                        resonator_type=platform.resonator_type,
+                        qubit_freqs={
+                            qubit: qubits[qubit].drive_frequency for qubit in qubits
+                        },
+                        sampling_rate=sampling_rate,
+                        offset_freq=offset_freq,
+                        labels=[
+                            "delta_frequency",
+                            "drive_frequency",
+                            "T2",
+                        ],
+                    )
+
+                for qubit in qubits:
+                    RX90_pulses2[qubit].start = RX90_pulses1[qubit].finish + wait
+                    RX90_pulses2[qubit].frequency = qubits[qubit].drive_frequency
+                    RX90_pulses2[qubit].relative_phase = (
+                        (RX90_pulses2[qubit].start / sampling_rate)
+                        * (2 * np.pi)
+                        * (-offset_freq)
+                    )
+                    ro_pulses[qubit].start = RX90_pulses2[qubit].finish
+
+                # execute the pulse sequence
+                results = platform.execute_pulse_sequence(sequence)
+
+                for ro_pulse in ro_pulses.values():
+                    # average msr, phase, i and q over the number of shots defined in the runcard
+                    r = results[ro_pulse.serial].average.raw
+                    r.update(
+                        {
+                            "wait[ns]": wait,
+                            "t_max[ns]": t_max,
+                            "qubit": ro_pulse.qubit,
+                            "iteration": iteration,
+                        }
+                    )
+                    data.add(r)
+                count += 1
+
+            data_fit = ramsey_fit(
+                data,
+                x="wait[ns]",
+                y="MSR[uV]",
+                qubits=qubits,
+                resonator_type=platform.resonator_type,
+                qubit_freqs={qubit: qubits[qubit].drive_frequency for qubit in qubits},
+                sampling_rate=sampling_rate,
+                offset_freq=offset_freq,
+                labels=[
+                    "delta_frequency",
+                    "drive_frequency",
+                    "T2",
+                ],
             )
-        else:
-            qubits[qubit].drive_frequency = (
-                qubit_data["frequency"][
-                    np.argmax(qubit_data["MSR"].pint.to("V").pint.magnitude)
-                ]
-                .to("Hz")
-                .magnitude
+        stop = False
+        for qubit in qubits:
+            new_t2 = float(data_fit.df[data_fit.df["qubit"] == qubit]["T2"])
+            corrected_qubit_freq = int(
+                data_fit.df[data_fit.df["qubit"] == qubit]["drive_frequency"]
             )
 
-    # run a precision sweep around the newly detected frequencies
-
-    delta_frequency_range = np.arange(
-        -precision_width // 2, precision_width // 2, precision_step
-    )
-
-    # create a second DataUnits object to store the results,
-    precision_sweep_data = DataUnits(
-        name="precision_sweep_data",
-        quantities={"frequency": "Hz"},
-        options=["qubit", "iteration"],
-    )
-
-    # repeat the experiment as many times as defined by software_averages
-    count = 0
-    for iteration in range(software_averages):
-        # sweep the parameter
-        for delta_freq in delta_frequency_range:
-            # save data as often as defined by points
-            if count % points == 0 and count > 0:
-                # save data
-                yield precision_sweep_data
-                # calculate and save fit
-                yield lorentzian_fit(
-                    precision_sweep_data,
-                    x="frequency[Hz]",
-                    y="MSR[uV]",
-                    qubits=qubits,
-                    resonator_type=platform.resonator_type,
-                    labels=["resonator_freq", "peak_voltage"],
+            if new_t2 > qubits[qubit].T2 and len(delay_between_pulses_end) > 1:
+                print(
+                    f"t_max: {t_max} -- new t2: {new_t2} > current t2: {qubits[qubit].T2} new iteration!"
                 )
-            # reconfigure the instrument based on the new resonator frequency
-            # in this case setting the local oscillators
-            # the pulse sequence does not need to be modified between executions
-            for qubit in qubits:
-                qd_pulses[qubit].frequency = delta_freq + qubits[qubit].drive_frequency
-
-            # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
-
-            # retrieve the results for every qubit
-            for ro_pulse in ro_pulses.values():
-                # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
-                # store the results
-                r.update(
-                    {
-                        "frequency[Hz]": qd_pulses[ro_pulse.qubit].frequency,
-                        "qubit": ro_pulse.qubit,
-                        "iteration": iteration,
-                    }
+                qubits[qubit].drive_frequency = int(corrected_qubit_freq)
+                qubits[qubit].T2 = new_t2
+                data = DataUnits(
+                    name=f"data",
+                    quantities={"wait": "ns", "t_max": "ns"},
+                    options=["qubit", "iteration"],
                 )
-                precision_sweep_data.add(r)
-            count += 1
-    # finally, save the remaining data and fits
-    yield precision_sweep_data
-    yield lorentzian_fit(
-        precision_sweep_data,
-        x="frequency[Hz]",
+            else:
+                print(
+                    f"t_max: {t_max} -- new t2: {new_t2} < current t2: {qubits[qubit].T2} stop!"
+                )
+                # corrected_qubit_freq = int(current_qubit_freqs[qubit])
+                # new_t2 = current_T2s[qubit]
+                # TODO: These best values need to be saved to the fits file so that they are returned to the user
+                stop = True
+        if stop:
+            break
+
+    yield data
+    yield ramsey_fit(
+        data,
+        x="wait[ns]",
         y="MSR[uV]",
         qubits=qubits,
         resonator_type=platform.resonator_type,
-        labels=["drive_frequency", "peak_voltage"],
+        qubit_freqs={qubit: qubits[qubit].drive_frequency for qubit in qubits},
+        sampling_rate=sampling_rate,
+        offset_freq=0,
+        labels=[
+            "delta_frequency",
+            "drive_frequency",
+            "T2",
+        ],
     )
 
 
-@plot(
-    "MSR and Phase vs Qubit Drive Frequency and Flux Current",
-    plots.frequency_flux_msr_phase,
-)
-def qubit_spectroscopy_flux(
+@plot("MSR vs Time", plots.time_msr)
+def ramsey(
     platform: AbstractPlatform,
     qubits: dict,
-    freq_width,
-    freq_step,
-    bias_width,
-    bias_step,
-    fluxlines,
+    delay_between_pulses_start,
+    delay_between_pulses_end,
+    delay_between_pulses_step,
     software_averages=1,
     points=10,
 ):
     r"""
-    Perform spectroscopy on the qubit modifying the bias applied in the flux control line.
-    This routine works for multiqubit devices flux controlled.
+    The purpose of the Ramsey experiment is to determine two of the qubit's properties: Ramsey or detuning frequency and T2.
+
+    Ramsey sequence: Rx(pi/2) - wait time - Rx(pi/2) - ReadOut
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
         qubits (dict): Dict of target Qubit objects to perform the action
-        freq_width (int): Width frequency in HZ to perform the spectroscopy sweep
-        freq_step (int): Step frequency in HZ for the spectroscopy sweep
-        bias_width (float): Width bias in A for the flux bias sweep
-        bias_step (float): Step bias in A for the flux bias sweep
-        fluxlines (list): List of flux lines to use to perform the experiment. If it is set to "qubits", it uses each of
-                        flux lines associated with the target qubits.
+        delay_between_pulses_start (int): Initial time delay between drive pulses in the Ramsey sequence
+        delay_between_pulses_end (list): Maximum time delay between drive pulses in the Ramsey sequence
+        delay_between_pulses_step (int): Scan range step for the time delay between drive pulses in the Ramsey sequence
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
 
     Returns:
         - A DataUnits object with the raw data obtained for the fast and precision sweeps with the following keys
 
             - **MSR[V]**: Resonator signal voltage mesurement in volts
             - **i[V]**: Resonator signal voltage mesurement for the component I in volts
             - **q[V]**: Resonator signal voltage mesurement for the component Q in volts
             - **phase[rad]**: Resonator signal phase mesurement in radians
-            - **frequency[Hz]**: Qubit drive frequency value in Hz
-            - **bias[V]**: Current value in A applied to the flux line
+            - **wait[ns]**: Wait time used in the current Ramsey execution
+            - **t_max[ns]**: Maximum time delay between drive pulses in the Ramsey sequence
             - **qubit**: The qubit being tested
-            - **fluxline**: The fluxline being tested
             - **iteration**: The iteration number of the many determined by software_averages
 
         - A DataUnits object with the fitted data obtained with the following keys
 
-            - **drive_frequency**: frequency
-            - **peak_voltage**: peak voltage
-            - **popt0**: Lorentzian's amplitude
-            - **popt1**: Lorentzian's center
-            - **popt2**: Lorentzian's sigma
-            - **popt3**: Lorentzian's offset
+            - **delta_frequency**: Physical detunning of the actual qubit frequency
+            - **drive_frequency**:
+            - **T2**: New qubit frequency after correcting the actual qubit frequency with the detunning calculated
+            - **popt0**: offset
+            - **popt1**: oscillation amplitude
+            - **popt2**: frequency
+            - **popt3**: phase
+            - **popt4**: T2
             - **qubit**: The qubit being tested
     """
+
     # reload instrument settings from runcard
     platform.reload_settings()
 
-    # create a sequence of pulses for the experiment:
-    # long drive probing pulse - MZ
-
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence = PulseSequence()
+    # create a sequence of pulses for the experiment
+    # RX90 - t - RX90 - MZ
     ro_pulses = {}
-    qd_pulses = {}
+    RX90_pulses1 = {}
+    RX90_pulses2 = {}
+    sequence = PulseSequence()
     for qubit in qubits:
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=0, duration=5000
+        RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
+        RX90_pulses2[qubit] = platform.create_RX90_pulse(
+            qubit, start=RX90_pulses1[qubit].finish
         )
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=5000)
-        sequence.add(qd_pulses[qubit])
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=RX90_pulses2[qubit].finish
+        )
+        sequence.add(RX90_pulses1[qubit])
+        sequence.add(RX90_pulses2[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
-    # qubit drive frequency
-    delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
+    # wait time between RX90 pulses
+    waits = np.arange(
+        delay_between_pulses_start,
+        delay_between_pulses_end,
+        delay_between_pulses_step,
+    )
 
-    # flux bias
-    sweetspot_biass = {}
-    bias_ranges = {}
-    bias_min = {}
-    bias_max = {}
-
-    if fluxlines == "qubits":
-        fluxlines = qubits
-
-    for fluxline in fluxlines:
-        # TODO: check if this is correct
-        sweetspot_biass[fluxline] = qubits[fluxline].sweetspot
-
-        bias_min[fluxline] = max(-bias_width / 2 + sweetspot_biass[fluxline], -0.03)
-        bias_max[fluxline] = min(+bias_width / 2 + sweetspot_biass[fluxline], +0.03)
-        bias_ranges[fluxline] = np.arange(
-            bias_min[fluxline], bias_max[fluxline], bias_step
-        )
+    sampling_rate = platform.sampling_rate
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
-    # additionally include qubit frequency and flux bias
+    # additionally include wait time and t_max
     data = DataUnits(
         name=f"data",
-        quantities={"frequency": "Hz", "bias": "V"},
-        options=["qubit", "fluxline", "iteration"],
+        quantities={"wait": "ns", "t_max": "ns"},
+        options=["qubit", "iteration"],
     )
 
     # repeat the experiment as many times as defined by software_averages
     count = 0
     for iteration in range(software_averages):
-        # sweep the parameters
-        for fluxline in fluxlines:
-            for bias in bias_ranges[fluxline]:
-                # set new flux bias
-                platform.set_bias(fluxline, bias)
-
-                # TODO: adjust resonator frequency if coefs available in the runcard
-                # coefs should be determined in resonator_spectroscopy_flux
-                # matrix of biass -> magnetic flux -> freq shift
-
-                for delta_freq in delta_frequency_range:
-                    # save data as often as defined by points
-                    if count % points == 0:
-                        # save data
-                        yield data
-                        # TODO: calculate and save fit
-
-                    # set new lo frequency
-                    for qubit in qubits:
-                        qd_pulses[qubit].frequency = (
-                            delta_freq + qubits[qubit].drive_frequency
-                        )
-
-                    # execute the pulse sequence
-                    result = platform.execute_pulse_sequence(sequence)
-
-                    # retrieve the results for every qubit
-                    for ro_pulse in ro_pulses.values():
-                        # average msr, phase, i and q over the number of shots defined in the runcard
-                        r = result[ro_pulse.serial].to_dict()
-                        # store the results
-                        r.update(
-                            {
-                                "frequency[Hz]": qd_pulses[ro_pulse.qubit].frequency,
-                                "bias[V]": bias,
-                                "qubit": ro_pulse.qubit,
-                                "fluxline": fluxline,
-                                "iteration": iteration,
-                            }
-                        )
-                        data.add(r)
-                    count += 1
-    # finally, save the remaining data and fits
+        # sweep the parameter
+        for wait in waits:
+            # save data as often as defined by points
+            if count % points == 0 and count > 0:
+                # save data
+                yield data
+                # calculate and save fit
+                yield ramsey_fit(
+                    data,
+                    x="wait[ns]",
+                    y="MSR[uV]",
+                    qubits=qubits,
+                    resonator_type=platform.resonator_type,
+                    qubit_freqs={
+                        qubit: qubits[qubit].drive_frequency for qubit in qubits
+                    },
+                    sampling_rate=sampling_rate,
+                    offset_freq=0,
+                    labels=[
+                        "delta_frequency",
+                        "drive_frequency",
+                        "T2",
+                    ],
+                )
+
+            for qubit in qubits:
+                RX90_pulses2[qubit].start = RX90_pulses1[qubit].finish + wait
+                ro_pulses[qubit].start = RX90_pulses2[qubit].finish
+
+            # execute the pulse sequence
+            results = platform.execute_pulse_sequence(sequence)
+
+            for ro_pulse in ro_pulses.values():
+                # average msr, phase, i and q over the number of shots defined in the runcard
+                r = results[ro_pulse.serial].average.raw
+                r.update(
+                    {
+                        "wait[ns]": wait,
+                        "t_max[ns]": delay_between_pulses_end,
+                        "qubit": ro_pulse.qubit,
+                        "iteration": iteration,
+                    }
+                )
+                data.add(r)
+            count += 1
     yield data
+    yield ramsey_fit(
+        data,
+        x="wait[ns]",
+        y="MSR[uV]",
+        qubits=qubits,
+        resonator_type=platform.resonator_type,
+        qubit_freqs={qubit: qubits[qubit].drive_frequency for qubit in qubits},
+        sampling_rate=sampling_rate,
+        offset_freq=0,
+        labels=[
+            "delta_frequency",
+            "drive_frequency",
+            "T2",
+        ],
+    )
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/rabi.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/rabi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import numpy as np
 from qibolab.platforms.abstract import AbstractPlatform
 from qibolab.pulses import PulseSequence
+from qibolab.sweeper import Parameter, Sweeper
 
 from qibocal import plots
 from qibocal.data import DataUnits
 from qibocal.decorators import plot
 from qibocal.fitting.methods import rabi_fit
 
 
 @plot("MSR vs Time", plots.time_msr_phase)
 def rabi_pulse_length(
     platform: AbstractPlatform,
     qubits: dict,
     pulse_duration_start,
     pulse_duration_end,
     pulse_duration_step,
+    nshots=1024,
     software_averages=1,
     points=10,
 ):
     r"""
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse duration
     to find the drive pulse length that creates a rotation of a desired angle.
 
@@ -104,19 +106,19 @@
                     labels=[
                         "pi_pulse_duration",
                         "pi_pulse_peak_voltage",
                     ],
                 )
 
             # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
+            results = platform.execute_pulse_sequence(sequence, nshots=nshots)
 
             for ro_pulse in ro_pulses.values():
                 # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
+                r = results[ro_pulse.serial].average.raw
                 r.update(
                     {
                         "time[ns]": duration,
                         "qubit": ro_pulse.qubit,
                         "iteration": iteration,
                     }
                 )
@@ -207,14 +209,15 @@
     data = DataUnits(
         name=f"data",
         quantities={"gain": "dimensionless"},
         options=["qubit", "iteration"],
     )
 
     count = 0
+    # TODO: add Sweeper for gain
     for iteration in range(software_averages):
         # sweep the parameter
         for gain in qd_pulse_gain_range:
             for qubit in qubits:
                 platform.set_gain(qubit, gain)
             # save data as often as defined by points
             if count % points == 0 and count > 0:
@@ -235,15 +238,15 @@
                 )
 
             # execute the pulse sequence
             results = platform.execute_pulse_sequence(sequence)
 
             for ro_pulse in ro_pulses.values():
                 # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
+                r = results[ro_pulse.serial].average.raw
                 r.update(
                     {
                         "gain[dimensionless]": gain,
                         "qubit": ro_pulse.qubit,
                         "iteration": iteration,
                     }
                 )
@@ -266,16 +269,17 @@
 @plot("MSR vs Amplitude", plots.amplitude_msr_phase)
 def rabi_pulse_amplitude(
     platform: AbstractPlatform,
     qubits: dict,
     pulse_amplitude_start,
     pulse_amplitude_end,
     pulse_amplitude_step,
+    nshots=1024,
+    relaxation_time=None,
     software_averages=1,
-    points=10,
 ):
     r"""
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse amplitude
     to find the drive pulse amplitude that creates a rotation of a desired angle.
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
@@ -325,73 +329,60 @@
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     # qubit drive pulse amplitude
     qd_pulse_amplitude_range = np.arange(
         pulse_amplitude_start, pulse_amplitude_end, pulse_amplitude_step
     )
+    sweeper = Sweeper(
+        Parameter.amplitude,
+        qd_pulse_amplitude_range,
+        [qd_pulses[qubit] for qubit in qubits],
+    )
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
     # additionally include qubit drive pulse amplitude
     data = DataUnits(
         name=f"data",
         quantities={"amplitude": "dimensionless"},
         options=["qubit", "iteration"],
     )
 
-    count = 0
     for iteration in range(software_averages):
         # sweep the parameter
-        for amplitude in qd_pulse_amplitude_range:
-            for qubit in qubits:
-                qd_pulses[qubit].amplitude = amplitude
-            # save data as often as defined by points
-            if count % points == 0 and count > 0:
-                yield data
-                # calculate and save fit
-                yield rabi_fit(
-                    data,
-                    x="amplitude[dimensionless]",
-                    y="MSR[uV]",
-                    qubits=qubits,
-                    resonator_type=platform.resonator_type,
-                    labels=[
-                        "pi_pulse_amplitude",
-                        "pi_pulse_peak_voltage",
-                    ],
-                )
-
-            # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
-
-            for ro_pulse in ro_pulses.values():
-                # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
-                r.update(
-                    {
-                        "amplitude[dimensionless]": amplitude,
-                        "qubit": ro_pulse.qubit,
-                        "iteration": iteration,
-                    }
-                )
-                data.add(r)
-            count += 1
-    yield data
-    yield rabi_fit(
-        data,
-        x="amplitude[dimensionless]",
-        y="MSR[uV]",
-        qubits=qubits,
-        resonator_type=platform.resonator_type,
-        labels=[
-            "pi_pulse_amplitude",
-            "pi_pulse_peak_voltage",
-        ],
-    )
+        results = platform.sweep(
+            sequence, sweeper, nshots=nshots, relaxation_time=relaxation_time
+        )
+        for qubit in qubits:
+            # average msr, phase, i and q over the number of shots defined in the runcard
+            result = results[ro_pulses[qubit].serial]
+            r = result.raw
+            r.update(
+                {
+                    "amplitude[dimensionless]": qd_pulse_amplitude_range,
+                    "qubit": len(qd_pulse_amplitude_range) * [qubit],
+                    "iteration": len(qd_pulse_amplitude_range) * [iteration],
+                }
+            )
+            data.add_data_from_dict(r)
+
+        yield data
+        # calculate and save fit
+        yield rabi_fit(
+            data,
+            x="amplitude[dimensionless]",
+            y="MSR[uV]",
+            qubits=qubits,
+            resonator_type=platform.resonator_type,
+            labels=[
+                "pi_pulse_amplitude",
+                "pi_pulse_peak_voltage",
+            ],
+        )
 
 
 @plot("MSR vs length and gain", plots.duration_gain_msr_phase)
 def rabi_pulse_length_and_gain(
     platform: AbstractPlatform,
     qubits: dict,
     pulse_duration_start,
@@ -461,14 +452,15 @@
     data = DataUnits(
         name=f"data",
         quantities={"duration": "ns", "gain": "dimensionless"},
         options=["qubit", "iteration"],
     )
 
     count = 0
+    # TODO: add sweeper for gain
     for iteration in range(software_averages):
         # sweep the parameters
         for duration in qd_pulse_duration_range:
             for gain in qd_pulse_gain_range:
                 for qubit in qubits:
                     qd_pulses[qubit].duration = duration
                     ro_pulses[qubit].start = duration
@@ -478,15 +470,15 @@
                     # save data
                     yield data
 
                 # execute the pulse sequence
                 results = platform.execute_pulse_sequence(sequence)
                 for ro_pulse in ro_pulses.values():
                     # average msr, phase, i and q over the number of shots defined in the runcard
-                    r = results[ro_pulse.serial].to_dict()
+                    r = results[ro_pulse.serial].average.raw
                     r.update(
                         {
                             "duration[ns]": duration,
                             "gain[dimensionless]": gain,
                             "qubit": ro_pulse.qubit,
                             "iteration": iteration,
                         }
@@ -502,14 +494,16 @@
     qubits: dict,
     pulse_duration_start,
     pulse_duration_end,
     pulse_duration_step,
     pulse_amplitude_start,
     pulse_amplitude_end,
     pulse_amplitude_step,
+    relaxation_time=None,
+    nshots=None,
     software_averages=1,
     points=10,
 ):
     r"""
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse
     combination of duration and amplitude to find the drive pulse amplitude that creates a rotation of a desired angle.
 
@@ -569,32 +563,35 @@
     data = DataUnits(
         name=f"data",
         quantities={"duration": "ns", "amplitude": "dimensionless"},
         options=["qubit", "iteration"],
     )
 
     count = 0
+    # TODO: implement Sweeper for amplitude
     for iteration in range(software_averages):
         # sweep the parameters
         for duration in qd_pulse_duration_range:
             for amplitude in qd_pulse_amplitude_range:
                 for qubit in qubits:
                     qd_pulses[qubit].duration = duration
                     ro_pulses[qubit].start = duration
                     qd_pulses[qubit].amplitude = amplitude
                 # save data as often as defined by points
                 if count % points == 0 and count > 0:
                     # save data
                     yield data
 
                 # execute the pulse sequence
-                results = platform.execute_pulse_sequence(sequence)
+                results = platform.execute_pulse_sequence(
+                    sequence, relaxation_time=relaxation_time, nshots=nshots
+                )
                 for ro_pulse in ro_pulses.values():
                     # average msr, phase, i and q over the number of shots defined in the runcard
-                    r = results[ro_pulse.serial].to_dict()
+                    r = results[ro_pulse.serial].average.raw
                     r.update(
                         {
                             "duration[ns]": duration,
                             "amplitude[dimensionless]": amplitude,
                             "qubit": ro_pulse.qubit,
                             "iteration": iteration,
                         }
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/resonator_spectroscopy.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/resonator_spectroscopy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import numpy as np
 from qibo.config import log
 from qibolab.platforms.abstract import AbstractPlatform
 from qibolab.pulses import PulseSequence
+from qibolab.sweeper import Parameter, Sweeper
 
 from qibocal import plots
-from qibocal.config import raise_error
 from qibocal.data import DataUnits
 from qibocal.decorators import plot
 from qibocal.fitting.methods import lorentzian_fit
 
 
 @plot("MSR and Phase vs Resonator Frequency", plots.frequency_msr_phase)
 def resonator_spectroscopy(
     platform: AbstractPlatform,
     qubits: dict,
-    fast_width,
-    fast_step,
-    precision_width,
-    precision_step,
-    software_averages=1,
-    points=10,
+    freq_width: int,
+    freq_step: int,
+    nshots: int = 1024,
+    relaxation_time: int = 50,
+    software_averages: int = 1,
 ):
     r"""
     Perform spectroscopies on the qubits' readout resonators.
     This routine executes an initial scan around the expected resonator frequency indicated
     in the platform runcard. After that, a final sweep with more precision is executed centered in the new
     resonator frequency found.
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
         qubits (dict): List of target qubits to perform the action
-        fast_width (int): Width frequency in HZ to perform the high resolution sweep
-        fast_step (int): Step frequency in HZ for the high resolution sweep
-        precision_width (int): Width frequency in HZ to perform the precision resolution sweep
-        precision_step (int): Step frequency in HZ for the precission resolution sweep
+        freq_width (int): Width frequency in HZ to perform the high resolution sweep
+        freq_step (int): Step frequency in HZ for the high resolution sweep
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
 
     Returns:
         - Two DataUnits objects with the raw data obtained for the fast and precision sweeps with the following keys
 
             - **MSR[V]**: Resonator signal voltage mesurement in volts
@@ -66,228 +63,230 @@
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     for qubit in qubits:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
-    # define the parameter to sweep and its range:
-
-    delta_frequency_range = np.arange(-fast_width // 2, fast_width // 2, fast_step)
-
-    # save runcard local oscillator frequencies to be able to calculate new intermediate frequencies
-    # lo_frequencies = {qubit: platform.get_lo_frequency(qubit) for qubit in qubits}
+    # define the parameter to sweep and its range resonator frequency
+    delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
+    sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        pulses=[ro_pulses[qubit] for qubit in qubits],
+    )
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
     # additionally include resonator frequency
-    fast_sweep_data = DataUnits(
-        name="fast_sweep_data",
+    data = DataUnits(
+        name="data",
         quantities={"frequency": "Hz"},
         options=["qubit", "iteration"],
     )
 
     # repeat the experiment as many times as defined by software_averages
-    count = 0
     for iteration in range(software_averages):
-        # sweep the parameter
-        for delta_freq in delta_frequency_range:
-            # save data as often as defined by points
-            if count % points == 0 and count > 0:
-                # save data
-                yield fast_sweep_data
-                # calculate and save fit
-                yield lorentzian_fit(
-                    fast_sweep_data,
-                    x="frequency[Hz]",
-                    y="MSR[uV]",
-                    qubits=qubits,
-                    resonator_type=platform.resonator_type,
-                    labels=["readout_frequency", "peak_voltage"],
-                )
-            # reconfigure the instruments based on the new resonator frequency
-            # in this case setting the local oscillators
-            # the pulse sequence does not need to be modified or recreated between executions
-            for qubit in qubits:
-                ro_pulses[qubit].frequency = (
-                    delta_freq + qubits[qubit].readout_frequency
-                )
-
-            # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
+        results = platform.sweep(
+            sequence, sweeper, nshots=nshots, relaxation_time=relaxation_time
+        )
 
-            # retrieve the results for every qubit
-            for ro_pulse in ro_pulses.values():
-                # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
-                # store the results
-                r.update(
-                    {
-                        "frequency[Hz]": ro_pulse.frequency,
-                        "qubit": ro_pulse.qubit,
-                        "iteration": iteration,
-                    }
-                )
-                fast_sweep_data.add(r)
-            count += 1
-    # finally, save the remaining data and fits
-    yield fast_sweep_data
-    yield lorentzian_fit(
-        fast_sweep_data,
-        x="frequency[Hz]",
-        y="MSR[uV]",
-        qubits=qubits,
-        resonator_type=platform.resonator_type,
-        labels=["readout_frequency", "peak_voltage"],
-    )
+        # retrieve the results for every qubit
+        for qubit in qubits:
+            # average msr, phase, i and q over the number of shots defined in the runcard
+            result = results[ro_pulses[qubit].serial]
+            # store the results
+            r = result.raw
+            r.update(
+                {
+                    "frequency[Hz]": delta_frequency_range + ro_pulses[qubit].frequency,
+                    "qubit": len(delta_frequency_range) * [qubit],
+                    "iteration": len(delta_frequency_range) * [iteration],
+                }
+            )
+            data.add_data_from_dict(r)
 
-    # store max/min peaks as new frequencies
-    for qubit in qubits:
-        qubit_data = (
-            fast_sweep_data.df[fast_sweep_data.df["qubit"] == qubit]
-            .drop(columns=["qubit", "iteration"])
-            .groupby("frequency", as_index=False)
-            .mean()
+        # finally, save the remaining data and fits
+        yield data
+        yield lorentzian_fit(
+            data,
+            x="frequency[GHz]",
+            y="MSR[uV]",
+            qubits=qubits,
+            resonator_type=platform.resonator_type,
+            labels=["readout_frequency", "peak_voltage"],
         )
-        if platform.resonator_type == "3D":
-            qubits[qubit].readout_frequency = (
-                qubit_data["frequency"][
-                    np.argmax(qubit_data["MSR"].pint.to("V").pint.magnitude)
-                ]
-                .to("Hz")
-                .magnitude
-            )
-        else:
-            qubits[qubit].readout_frequency = (
-                qubit_data["frequency"][
-                    np.argmin(qubit_data["MSR"].pint.to("V").pint.magnitude)
-                ]
-                .to("Hz")
-                .magnitude
-            )
 
-    # run a precision sweep around the newly detected frequencies
 
-    # TODO: remove it
-    # create a new sequence of pulses with adjusted frequencies
+@plot(
+    "MSR and Phase vs Resonator Frequency and Attenuation",
+    plots.frequency_attenuation_msr_phase,
+)
+@plot(
+    "Cross section at half range attenuation", plots.frequency_attenuation_msr_phase_cut
+)
+def resonator_punchout_attenuation(
+    platform: AbstractPlatform,
+    qubits: dict,
+    freq_width,
+    freq_step,
+    min_att,
+    max_att,
+    step_att,
+    relaxation_time=50,
+    nshots=1024,
+    software_averages=1,
+):
+    r"""
+    Perform spectroscopies on the qubits' readout resonators, decreasing the attenuation applied to
+    the read-out pulse, producing an increment of the power sent to the resonator.
+    That shows the two regimes of a given resonator, low and high-power regimes.
+
+    Args:
+        platform (AbstractPlatform): Qibolab platform object
+        qubits (dict): List of target qubits to perform the action
+        freq_width (int): Width frequency in HZ to perform the spectroscopy sweep
+        freq_step (int): Step frequency in HZ for the spectroscopy sweep
+        min_att (int): Minimum value in db for the attenuation sweep
+        max_att (int): Minimum value in db for the attenuation sweep
+        step_att (int): Step attenuation in db for the attenuation sweep
+        relaxation_time (int): Relaxation time between shots (ns)
+        software_averages (int): Number of executions of the routine for averaging results
+        points (int): Save data results in a file every number of points
+
+    Returns:
+        A DataUnits object with the raw data obtained with the following keys
+
+            - **MSR[V]**: Resonator signal voltage mesurement in volts
+            - **i[V]**: Resonator signal voltage mesurement for the component I in volts
+            - **q[V]**: Resonator signal voltage mesurement for the component Q in volts
+            - **phase[rad]**: Resonator signal phase mesurement in radians
+            - **frequency[Hz]**: Resonator frequency value in Hz
+            - **attenuation[dB]**: attenuation value in db applied to the flux line
+            - **qubit**: The qubit being tested
+            - **iteration**: The iteration number of the many determined by software_averages
+    """
+
+    # reload instrument settings from runcard
+    platform.reload_settings()
+
+    # create a sequence of pulses for the experiment:
+    # MZ
+
+    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
+
     ro_pulses = {}
     for qubit in qubits:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
-    delta_frequency_range = np.arange(
-        -precision_width // 2, precision_width // 2, precision_step
+    # define the parameters to sweep and their range:
+    # resonator frequency
+    delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
+    freq_sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        [ro_pulses[qubit] for qubit in qubits],
     )
 
-    # create a second DataUnits object to store the results,
-    precision_sweep_data = DataUnits(
-        name="precision_sweep_data",
-        quantities={"frequency": "Hz"},
+    # attenuation
+    attenuation_range = np.flip(np.arange(min_att, max_att, step_att))
+    att_sweeper = Sweeper(Parameter.attenuation, attenuation_range, qubits=qubits)
+
+    # create a DataUnits object to store the results,
+    # DataUnits stores by default MSR, phase, i, q
+    # additionally include resonator frequency and attenuation
+    data = DataUnits(
+        name=f"data",
+        quantities={"frequency": "Hz", "attenuation": "dB"},
         options=["qubit", "iteration"],
     )
 
     # repeat the experiment as many times as defined by software_averages
-    count = 0
+    atts = np.repeat(attenuation_range, len(delta_frequency_range))
     for iteration in range(software_averages):
-        # sweep the parameter
-        for delta_freq in delta_frequency_range:
-            # save data as often as defined by points
-            if count % points == 0 and count > 0:
-                # save data
-                yield precision_sweep_data
-                # calculate and save fit
-                yield lorentzian_fit(
-                    precision_sweep_data,
-                    x="frequency[Hz]",
-                    y="MSR[uV]",
-                    qubits=qubits,
-                    resonator_type=platform.resonator_type,
-                    labels=["readout_frequency", "peak_voltage"],
-                )
-            # reconfigure the instrument based on the new resonator frequency
-            # in this case setting the local oscillators
-            # the pulse sequence does not need to be modified between executions
-            for qubit in qubits:
-                ro_pulses[qubit].frequency = (
-                    delta_freq + qubits[qubit].readout_frequency
-                )
+        results = platform.sweep(
+            sequence,
+            att_sweeper,
+            freq_sweeper,
+            nshots=nshots,
+            relaxation_time=relaxation_time,
+        )
 
-            # execute the pulse sequence
-            results = platform.execute_pulse_sequence(sequence)
+        # retrieve the results for every qubit
+        for qubit, ro_pulse in ro_pulses.items():
+            # average msr, phase, i and q over the number of shots defined in the runcard
+            result = results[ro_pulse.serial]
+            # store the results
+            freqs = np.array(
+                len(attenuation_range)
+                * list(delta_frequency_range + ro_pulse.frequency)
+            ).flatten()
+            r = result.raw
+            r.update(
+                {
+                    "frequency[Hz]": freqs,
+                    "attenuation[dB]": atts,
+                    "qubit": len(freqs) * [qubit],
+                    "iteration": len(freqs) * [iteration],
+                }
+            )
+            data.add_data_from_dict(r)
 
-            # retrieve the results for every qubit
-            for ro_pulse in ro_pulses.values():
-                # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
-                # store the results
-                r.update(
-                    {
-                        "frequency[Hz]": ro_pulse.frequency,
-                        "qubit": ro_pulse.qubit,
-                        "iteration": iteration,
-                    }
-                )
-                precision_sweep_data.add(r)
-            count += 1
-    # finally, save the remaining data and fits
-    yield precision_sweep_data
-    yield lorentzian_fit(
-        precision_sweep_data,
-        x="frequency[Hz]",
-        y="MSR[uV]",
-        qubits=qubits,
-        resonator_type=platform.resonator_type,
-        labels=["readout_frequency", "peak_voltage"],
-    )
+        # save data
+        yield data
+        # TODO: calculate and save fit
 
 
 @plot(
-    "MSR and Phase vs Resonator Frequency and Attenuation",
-    plots.frequency_attenuation_msr_phase,
-)
-@plot(
-    "Cross section at half range attenuation", plots.frequency_attenuation_msr_phase_cut
+    "MSR and Phase vs Resonator Frequency and Amplitude",
+    plots.frequency_amplitude_msr_phase,
 )
 def resonator_punchout(
     platform: AbstractPlatform,
     qubits: dict,
     freq_width,
     freq_step,
-    min_att,
-    max_att,
-    step_att,
+    min_amp_factor,
+    max_amp_factor,
+    step_amp_factor,
+    relaxation_time=None,
+    nshots=1024,
     software_averages=1,
-    points=10,
 ):
     r"""
     Perform spectroscopies on the qubits' readout resonators, decreasing the attenuation applied to
     the read-out pulse, producing an increment of the power sent to the resonator.
     That shows the two regimes of a given resonator, low and high-power regimes.
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
         qubits (dict): List of target qubits to perform the action
         freq_width (int): Width frequency in HZ to perform the spectroscopy sweep
         freq_step (int): Step frequency in HZ for the spectroscopy sweep
-        min_att (int): Minimum value in db for the attenuation sweep
-        max_att (int): Minimum value in db for the attenuation sweep
-        step_att (int): Step attenuation in db for the attenuation sweep
+        max_amp_factor (float): Maximum value of the factor that multiplies the amplitude
+            of the readout pulse
+        min_amp_factor (float): Minimum value of the factor that multiplies the amplitude
+            of the readout pulse
+        step_amp_factor (float): Step value of the factor that multiplies the amplitude
+            of the readout pulse
+        relaxation_time (int): Relaxation time between shots (ns)
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
 
     Returns:
         A DataUnits object with the raw data obtained with the following keys
 
             - **MSR[V]**: Resonator signal voltage mesurement in volts
             - **i[V]**: Resonator signal voltage mesurement for the component I in volts
             - **q[V]**: Resonator signal voltage mesurement for the component Q in volts
             - **phase[rad]**: Resonator signal phase mesurement in radians
             - **frequency[Hz]**: Resonator frequency value in Hz
-            - **attenuation[dB]**: attenuation value in db applied to the flux line
+            - **amplitude**: amplitude value of the pulse sent
             - **qubit**: The qubit being tested
             - **iteration**: The iteration number of the many determined by software_averages
     """
 
     # reload instrument settings from runcard
     platform.reload_settings()
 
@@ -299,89 +298,87 @@
 
     ro_pulses = {}
     for qubit in qubits:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
-
-    delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step) - (
-        freq_width // 8
+    # resonator frequency
+    delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
+    freq_sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        [ro_pulses[qubit] for qubit in qubits],
     )
 
-    # attenuation
-    attenuation_range = np.flip(np.arange(min_att, max_att, step_att))
+    # amplitude
+    amplitude_range = np.arange(min_amp_factor, max_amp_factor, step_amp_factor)
+    amp_sweeper = Sweeper(
+        Parameter.amplitude, amplitude_range, [ro_pulses[qubit] for qubit in qubits]
+    )
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
     # additionally include resonator frequency and attenuation
     data = DataUnits(
         name=f"data",
-        quantities={"frequency": "Hz", "attenuation": "dB"},
+        quantities={"frequency": "Hz", "amplitude": "dimensionless"},
         options=["qubit", "iteration"],
     )
 
     # repeat the experiment as many times as defined by software_averages
-    count = 0
+    amps = np.repeat(amplitude_range, len(delta_frequency_range))
     for iteration in range(software_averages):
-        # sweep the parameters
-        for att in attenuation_range:
-            for delta_freq in delta_frequency_range:
-                # save data as often as defined by points
-                if count % points == 0:
-                    # save data
-                    yield data
-                    # TODO: calculate and save fit
-
-                # reconfigure the instrument based on the new parameters
-                # in this case setting the local oscillators and their attenuations
-                # the pulse sequence does not need to be modified between executions
-                for qubit in qubits:
-                    ro_pulses[qubit].frequency = (
-                        delta_freq + qubits[qubit].readout_frequency
-                    )
-                    platform.set_attenuation(qubit, att)
+        results = platform.sweep(
+            sequence,
+            amp_sweeper,
+            freq_sweeper,
+            nshots=nshots,
+            relaxation_time=relaxation_time,
+        )
 
-                # execute the pulse sequence
-                results = platform.execute_pulse_sequence(sequence)
+        # retrieve the results for every qubit
+        for qubit, ro_pulse in ro_pulses.items():
+            # average msr, phase, i and q over the number of shots defined in the runcard
+            result = results[ro_pulse.serial]
+            # store the results
+            freqs = np.array(
+                len(amplitude_range) * list(delta_frequency_range + ro_pulse.frequency)
+            ).flatten()
+            r = {k: v.ravel() for k, v in result.raw.items()}
+            r.update(
+                {
+                    "frequency[Hz]": freqs,
+                    "amplitude[dimensionless]": amps,
+                    "qubit": len(freqs) * [qubit],
+                    "iteration": len(freqs) * [iteration],
+                }
+            )
+            data.add_data_from_dict(r)
 
-                # retrieve the results for every qubit
-                for ro_pulse in ro_pulses.values():
-                    # average msr, phase, i and q over the number of shots defined in the runcard
-                    r = results[ro_pulse.serial].to_dict()
-                    # * (np.exp(att / 20)), # normalise the results
-                    r.update(
-                        {
-                            "frequency[Hz]": ro_pulse.frequency,
-                            "attenuation[dB]": att,
-                            "qubit": ro_pulse.qubit,
-                            "iteration": iteration,
-                        }
-                    )
-                    # store the results
-                    data.add(r)
-                count += 1
-    # finally, save the remaining data and fits
-    yield data
+        # save data
+        yield data
+        # TODO: calculate and save fit
 
 
 @plot(
-    "MSR and Phase vs Resonator Frequency and Flux Current",
+    "MSR and Phase vs Resonator Frequency and Flux",
     plots.frequency_flux_msr_phase,
 )
 def resonator_spectroscopy_flux(
     platform: AbstractPlatform,
     qubits: dict,
     freq_width,
     freq_step,
     bias_width,
     bias_step,
     fluxlines,
+    nshots=1024,
+    relaxation_time=50,
     software_averages=1,
-    points=10,
 ):
     r"""
     Perform spectroscopy on the readout resonator modifying the bias applied in the flux control line.
     This routine works for quantum devices flux controlled.
 
     Args:
         platform (AbstractPlatform): Qibolab platform object
@@ -419,84 +416,74 @@
     ro_pulses = {}
     for qubit in qubits:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
+    freq_sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        [ro_pulses[qubit] for qubit in qubits],
+    )
 
     # flux bias
-    sweetspot_biass = {}
-    bias_ranges = {}
-    bias_min = {}
-    bias_max = {}
-
     if fluxlines == "qubits":
         fluxlines = qubits
 
-    for fluxline in fluxlines:
-        sweetspot_biass[fluxline] = qubits[fluxline].sweetspot
-
-        bias_min[fluxline] = max(-bias_width / 2 + sweetspot_biass[fluxline], -0.03)
-        bias_max[fluxline] = min(+bias_width / 2 + sweetspot_biass[fluxline], +0.03)
-        bias_ranges[fluxline] = np.arange(
-            bias_min[fluxline], bias_max[fluxline], bias_step
-        )
+    delta_bias_range = np.arange(-bias_width / 2, bias_width / 2, bias_step)
+    bias_sweeper = Sweeper(Parameter.bias, delta_bias_range, qubits=fluxlines)
 
     # create a DataUnits object to store the results,
     # DataUnits stores by default MSR, phase, i, q
     # additionally include resonator frequency and flux bias
     data = DataUnits(
         name=f"data",
         quantities={"frequency": "Hz", "bias": "V"},
         options=["qubit", "fluxline", "iteration"],
     )
 
     # repeat the experiment as many times as defined by software_averages
-    count = 0
     for iteration in range(software_averages):
-        # sweep the parameters
-        for fluxline in fluxlines:
-            for bias in bias_ranges[fluxline]:
-                # set new flux bias
-                platform.set_bias(fluxline, bias)
-                for delta_freq in delta_frequency_range:
-                    # save data as often as defined by points
-                    if count % points == 0:
-                        # save data
-                        yield data
-                        # TODO: calculate and save fit
-
-                    # set new lo frequency
-                    for qubit in qubits:
-                        ro_pulses[qubit].frequency = (
-                            delta_freq + qubits[qubit].readout_frequency
-                        )
-
-                    # execute the pulse sequence
-                    results = platform.execute_pulse_sequence(sequence)
-
-                    # retrieve the results for every qubit
-                    for ro_pulse in ro_pulses.values():
-                        # average msr, phase, i and q over the number of shots defined in the runcard
-                        r = results[ro_pulse.serial].to_dict()
-                        # store the results
-                        r.update(
-                            {
-                                "frequency[Hz]": ro_pulses[qubit].frequency,
-                                "bias[V]": bias,
-                                "qubit": ro_pulse.qubit,
-                                "fluxline": fluxline,
-                                "iteration": iteration,
-                            }
-                        )
-                        data.add(r)
-                    count += 1
-    # finally, save the remaining data and fits
-    yield data
+        results = platform.sweep(
+            sequence,
+            bias_sweeper,
+            freq_sweeper,
+            nshots=nshots,
+            relaxation_time=relaxation_time,
+        )
+
+        # retrieve the results for every qubit
+        for qubit, fluxline in zip(qubits, fluxlines):
+            # TODO: Support more fluxlines for QM
+
+            result = results[ro_pulses[qubit].serial]
+
+            biases = np.repeat(
+                delta_bias_range, len(delta_frequency_range)
+            ) + platform.get_bias(fluxline)
+            freqs = np.array(
+                len(delta_bias_range)
+                * list(delta_frequency_range + ro_pulses[qubit].frequency)
+            ).flatten()
+            # store the results
+            r = {k: v.ravel() for k, v in result.raw.items()}
+            r.update(
+                {
+                    "frequency[Hz]": freqs,
+                    "bias[V]": biases,
+                    "qubit": len(freqs) * [qubit],
+                    "fluxline": len(freqs) * [fluxline],
+                    "iteration": len(freqs) * [iteration],
+                }
+            )
+            data.add_data_from_dict(r)
+
+        # save data
+        yield data
 
 
 @plot("MSR and Phase vs Resonator Frequency", plots.dispersive_frequency_msr_phase)
 def dispersive_shift(
     platform: AbstractPlatform,
     qubits: dict,
     freq_width,
@@ -523,15 +510,15 @@
             - **i[V]**: Resonator signal voltage mesurement for the component I in volts
             - **q[V]**: Resonator signal voltage mesurement for the component Q in volts
             - **phase[rad]**: Resonator signal phase mesurement in radians
             - **frequency[Hz]**: Resonator frequency value in Hz
             - **qubit**: The qubit being tested
             - **iteration**: The iteration number of the many determined by software_averages
     """
-
+    # TODO: add sweepers
     # reload instrument settings from runcard
     platform.reload_settings()
 
     # create 2 sequences of pulses for the experiment:
     # sequence_0: I  - MZ
     # sequence_1: RX - MZ
 
@@ -550,22 +537,23 @@
         sequence_1.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(-freq_width // 2, freq_width // 2, freq_step)
 
     # create a DataUnits objects to store the results
     data_0 = DataUnits(
-        name=f"data_0", quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
+        name="data_0", quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
     )
     data_1 = DataUnits(
-        name=f"data_1", quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
+        name="data_1", quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
     )
 
     # repeat the experiment as many times as defined by software_averages
     count = 0
+    # TODO: implement sweeper
     for iteration in range(software_averages):
         # sweep the parameter
         for delta_freq in delta_frequency_range:
             # save data as often as defined by points
             if count % points == 0 and count > 0:
                 # save data
                 yield data_0
@@ -602,19 +590,19 @@
             results_0 = platform.execute_pulse_sequence(sequence_0)
             results_1 = platform.execute_pulse_sequence(sequence_1)
 
             # retrieve the results for every qubit
             for data, results in list(zip([data_0, data_1], [results_0, results_1])):
                 for ro_pulse in ro_pulses.values():
                     # average msr, phase, i and q over the number of shots defined in the runcard
-                    r = results[ro_pulse.serial].to_dict()
+                    r = results[ro_pulse.serial].average.raw
                     # store the results
                     r.update(
                         {
-                            "frequency[Hz]": ro_pulses[qubit].frequency,
+                            "frequency[Hz]": ro_pulse.frequency,
                             "qubit": ro_pulse.qubit,
                             "iteration": iteration,
                         }
                     )
                     data.add(r)
             count += 1
     # finally, save the remaining data and fits
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/resonator_spectroscopy_sample.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/resonator_spectroscopy_sample.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/spin_echo.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/spin_echo.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 ro_pulses[qubit].start = RX90_pulses2[qubit].finish
 
             # execute the pulse sequence
             results = platform.execute_pulse_sequence(sequence)
 
             for ro_pulse in ro_pulses.values():
                 # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
+                r = results[ro_pulse.serial].raw
                 r.update(
                     {
                         "wait[ns]": wait,
                         "qubit": ro_pulse.qubit,
                         "iteration": iteration,
                     }
                 )
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/characterization/t1.py` & `qibocal-0.0.2/src/qibocal/calibrations/characterization/t1.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,19 @@
                 ro_pulses[qubit].start = qd_pulses[qubit].duration + wait
 
             # execute the pulse sequence
             results = platform.execute_pulse_sequence(sequence)
 
             for ro_pulse in ro_pulses.values():
                 # average msr, phase, i and q over the number of shots defined in the runcard
-                r = results[ro_pulse.serial].to_dict()
+                r = results[ro_pulse.serial].average.raw
                 r.update(
                     {
                         "wait[ns]": wait,
-                        "qubit": qubit,
+                        "qubit": ro_pulse.qubit,
                         "iteration": iteration,
                     }
                 )
                 data.add(r)
             count += 1
     yield data
     yield t1_fit(
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/XIdrb.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/XIdrb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """ This script implements an easy 1-qubit protocol with only X-gates and identities.
 It is a great example on how to write an own niGSC protocol. The single functions above have
 little descriptions for the purpose of that function and what is important to include.
 
 1. Step:
+
   Define the two module specific classes which are used in defining and executing an experiment,
   the circuit factory and experiment class.
   They can also just inherit everything from another module.
+
 2. Step:
+
   Write the sequential post processing functions.
+
 3. Step:
+
   Write the aggregational post processing function.
+
 4. Step:
+
   Write the function to build a report. When using the qq module, a plotly figure has to be returned.
 """
 
 # These libraries should be enough when starting a new protocol.
 from __future__ import annotations
 
 from collections.abc import Iterable
@@ -26,40 +33,35 @@
 from qibo.models import Circuit
 from qibo.noise import NoiseModel
 
 import qibocal.calibrations.niGSC.basics.fitting as fitting_methods
 from qibocal.calibrations.niGSC.basics.circuitfactory import CircuitFactory
 from qibocal.calibrations.niGSC.basics.experiment import Experiment
 from qibocal.calibrations.niGSC.basics.plot import Report, scatter_fit_fig
+from qibocal.calibrations.niGSC.basics.utils import number_to_str
 from qibocal.config import raise_error
 
 
 # Define the circuit factory class for this specific module.
 class ModuleFactory(CircuitFactory):
     def __init__(self, nqubits: int, depths: list, qubits: list = []) -> None:
         super().__init__(nqubits, depths, qubits)
         if not len(self.qubits) == 1:
             raise_error(
                 ValueError,
-                "This class is written for gates acting on only one qubit, not {} qubits.".format(
-                    len(self.qubits)
-                ),
+                f"This class is written for gates acting on only one qubit, not {len(self.qubits)} qubits.",
             )
         self.name = "XId"
 
     def build_circuit(self, depth: int):
         # Initiate the empty circuit from qibo with 'self.nqubits'
         # many qubits.
-        circuit = Circuit(1, density_matrix=True)
-        # There are only two gates to choose from for every qubit.
-        a = [gates.I(0), gates.X(0)]
-        # Draw sequence length many zeros and ones.
-        random_ints = np.random.randint(0, 2, size=depth)
-        # Get the Xs and Ids with random_ints as indices.
-        gate_lists = np.take(a, random_ints)
+        circuit = Circuit(1)
+        # Draw sequence length many I and X gates.
+        gate_lists = np.random.choice([gates.I(0), gates.X(0)], size=depth)
         # Add gates to circuit.
         circuit.add(gate_lists)
         circuit.add(gates.M(0))
         return circuit
 
 
 # Define the experiment class for this specific module.
@@ -68,26 +70,28 @@
         self,
         circuitfactory: Iterable,
         data: Iterable | None = None,
         nshots: int | None = None,
         noise_model: NoiseModel = None,
     ) -> None:
         super().__init__(circuitfactory, data, nshots, noise_model)
+        # Make the circuitfactory a list be able to store them using save_circuits method.
+        self.prebuild()
         self.name = "XIdRB"
 
     def execute(self, circuit: Circuit, datarow: dict) -> dict:
         datadict = super().execute(circuit, datarow)
         datadict["depth"] = circuit.ngates - 1
         # TODO change that.
-        datadict["countX"] = circuit.gate_types["x"]
+        datadict["countX"] = len(circuit.gates_of_type("x"))
         return datadict
 
 
 # Define the result class for this specific module.
-class moduleReport(Report):
+class ModuleReport(Report):
     def __init__(self) -> None:
         super().__init__()
         self.title = "X-Id Benchmarking"
 
 
 # The filter functions/post processing functions always dependent on circuit and data row!
 # It is executed row by row when used on an experiment object.
@@ -133,62 +137,50 @@
     # Compute and add the ground state probabilities row by row.
     experiment.perform(filter_sign)
 
 
 # After the row by row execution of tasks comes the aggregational task. Something like calculation
 # of means, deviations, fitting data, tasks where the whole data as to be looked at, and not just
 # one instance of circuit + other information.
-def get_aggregational_data(experiment: Experiment) -> pd.DataFrame:
+def get_aggregational_data(experiment: Experiment, ndecays: int = 2) -> pd.DataFrame:
     """Computes aggregational tasks, fits data and stores the results in a data frame.
 
     No data is manipulated in the ``experiment`` object.
 
     Args:
         experiment (Experiment): After sequential postprocessing of the experiment data.
+        ndecays (int): Number of decays to be fitted. Default is 2.
 
     Returns:
         pd.DataFrame: The summarized data.
     """
     # Has to fit the column describtion from ``filter_sign``.
     depths, ydata = experiment.extract("filter", "depth", "mean")
     _, ydata_std = experiment.extract("filter", "depth", "std")
     # Fit the filtered signal for each depth, there could be two overlaying exponential functions.
-    popt, perr = fitting_methods.fit_exp2_func(depths, ydata)
+    popt, perr = fitting_methods.fit_expn_func(depths, ydata, n=ndecays)
+    # Create dictionaries with fitting parameters and estimated errors
+    popt_keys = [f"A{k+1}" for k in range(ndecays)]
+    popt_keys += [f"p{k+1}" for k in range(ndecays)]
+    popt_dict = dict(zip(popt_keys, popt))
+    perr_keys = [f"A{k+1}_err" for k in range(ndecays)]
+    perr_keys += [f"p{k+1}_err" for k in range(ndecays)]
+    perr_dict = dict(zip(perr_keys, perr))
     # Build a list of dictionaries with the aggregational information.
     data = [
         {
             "depth": depths,  # The x-axis.
             "data": ydata,  # The filtred signal.
             "2sigma": 2 * ydata_std,  # The 2 * standard deviation error for each depth.
-            "fit_func": "exp2_func",  # Which function was used to fit.
-            "popt_real": {
-                "A1_real": np.real(
-                    popt[0]
-                ),  # The complex prefactors would lead to imaginary data.
-                "A2_real": np.real(
-                    popt[1]
-                ),  # That's why they have to be stored seperatly.
-                "p1": popt[2],
-                "p2": popt[3],
-            },  # The real fitting parameters.
-            "perr": {
-                "A1_err": perr[0],
-                "A2_err": perr[1],
-                "p1_err": perr[2],
-                "p2_err": perr[3],
-            },  # The estimated errors.
+            "fit_func": "expn_func",  # Which function was used to fit.
+            "popt": popt_dict,  # The real fitting parameters.
+            "perr": perr_dict,  # The estimated errors.
         }
     ]
-    if np.iscomplex(popt[0]) or np.iscomplex(popt[1]):
-        data[0]["popt_imag"] = {
-            "A1_imag": np.imag(popt[0]),
-            "A2_imag": np.imag(popt[1]),
-            "p1": popt[2],
-            "p2": popt[3],
-        }  # The imaginary fitting parameters.
+
     df = pd.DataFrame(data, index=["filter"])
     return df
 
 
 # This is highly individual. The only important thing for the qq module is that a plotly figure is
 # returned, if qq is not used any type of figure can be build.
 def build_report(experiment: Experiment, df_aggr: pd.DataFrame) -> Figure:
@@ -196,38 +188,32 @@
     build a report as plotly figure.
 
     Args:
         experiment (Experiment): After sequential postprocessing of the experiment data.
         df_aggr (pd.DataFrame): Normally build with ``get_aggregational_data`` function.
 
     Returns:
-        (Figure): A plotly.graphical_object.Figure object.
+        (tuple): A `plotly.graphical_object.Figure` object and a string corresponding to a table.
     """
 
     # Initiate a report object.
-    report = moduleReport()
-    # Add general information to the object.
+    report = ModuleReport()
+    # Add general information to the table.
     report.info_dict["Number of qubits"] = len(experiment.data[0]["samples"][0])
     report.info_dict["Number of shots"] = len(experiment.data[0]["samples"])
     report.info_dict["runs"] = experiment.extract("samples", "depth", "count")[1][0]
-    report.info_dict["Fitting daviations"] = "".join(
-        [
-            "{}:{:.3f} ".format(key, df_aggr.loc["filter"]["perr"][key])
-            for key in df_aggr.loc["filter"]["perr"]
-        ]
+    dfrow = df_aggr.loc["filter"]
+    popt_pairs = list(dfrow["popt"].items())[::2] + list(dfrow["popt"].items())[1::2]
+    report.info_dict["Fit"] = "".join(
+        [f"{key}={number_to_str(value)} " for key, value in popt_pairs]
+    )
+    perr_pairs = list(dfrow["perr"].items())[::2] + list(dfrow["perr"].items())[1::2]
+    report.info_dict["Fitting deviations"] = "".join(
+        [f"{key}={number_to_str(value)} " for key, value in perr_pairs]
     )
     # Use the predefined ``scatter_fit_fig`` function from ``basics.utils`` to build the wanted
     # plotly figure with the scattered filtered data along with the mean for
     # each depth and the exponential fit for the means.
-    report.all_figures.append(
-        scatter_fit_fig(
-            experiment, df_aggr, "depth", "filter", fittingparam_label="popt_real"
-        )
-    )
-    if "popt_imag" in df_aggr:
-        report.all_figures.append(
-            scatter_fit_fig(
-                experiment, df_aggr, "depth", "filter", fittingparam_label="popt_imag"
-            )
-        )
-    # Return the figure the report object builds out of all figures added to the report.
+    report.all_figures.append(scatter_fit_fig(experiment, df_aggr, "depth", "filter"))
+
+    # Return the figure of the report object and the corresponding table.
     return report.build()
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/circuitfactory.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/circuitfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import abc
+from copy import deepcopy
 
 import numpy as np
 from qibo import gates
 from qibo.models import Circuit
 from qibo.quantum_info.random_ensembles import random_clifford
 
 from qibocal.calibrations.niGSC.basics.utils import ONEQ_GATES
@@ -45,21 +46,23 @@
         Returns:
             Circuit: With specific gate distribution.
         """
 
         # Check if the stop critarion is met.
         if self.n >= len(self.depths):
             raise StopIteration
-        else:
-            circuit = self.build_circuit(self.depths[self.n])
-            self.n += 1
-            # Distribute the circuit onto the given support.
-            bigcircuit = Circuit(self.nqubits)
-            bigcircuit.add(circuit.on_qubits(*self.qubits))
-            return bigcircuit
+
+        circuit = self.build_circuit(self.depths[self.n])
+        self.n += 1
+        # Distribute the circuit onto the given support.
+        circuit_init_kwargs = deepcopy(circuit.init_kwargs)
+        circuit_init_kwargs["nqubits"] = self.nqubits
+        bigcircuit = Circuit(**circuit_init_kwargs)
+        bigcircuit.add(circuit.on_qubits(*self.qubits))
+        return bigcircuit
 
     def build_circuit(self, depth: int) -> Circuit:
         """Initiate a ``qibo.models.Circuit`` object and fill it with the wanted gates.
 
         Which gates are wanted is encoded in ``self.gates_layer()``.
         Add a measurement gate for every qubit.
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/experiment.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable
 
 import numpy as np
 import pandas as pd
 from qibo.models import Circuit
 from qibo.noise import NoiseModel
 
-from qibocal.calibrations.niGSC.basics.utils import copy_circuit, experiment_directory
+from qibocal.cli.utils import generate_output_folder
 from qibocal.config import raise_error
 
 
 class Experiment:
     """Experiment objects which holds an iterable circuit factory along with
     a simple data structure associated to each circuit.
 
@@ -35,41 +35,33 @@
         noise_model: NoiseModel | None = None,
     ) -> None:
         """ """
 
         if circuitfactory is not None and not isinstance(circuitfactory, Iterable):
             raise_error(
                 TypeError,
-                "given circuit factory has wrong type {}, must be Iterable | None.".format(
-                    type(circuitfactory)
-                ),
+                f"Invalid type {type(circuitfactory)} for CircuitFactory,  must be Iterable or None.",
             )
         self.circuitfactory = circuitfactory
         if data is not None and not isinstance(data, Iterable):
             raise_error(
                 TypeError,
-                "given data has wrong type {}, must be Iterable | None ".format(
-                    type(data)
-                ),
+                f"Invalid data type  {type(data)}. Data must be Iterable or None.",
             )
         self.data = data
         if nshots is not None and not isinstance(nshots, int):
             raise_error(
                 TypeError,
-                "given nshots has wrong type {}, must be int | None".format(
-                    type(nshots)
-                ),
+                f"Invalid nshots type {type(nshots)}. Nshots must be int or None.",
             )
         self.nshots = nshots
         if noise_model is not None and not isinstance(noise_model, NoiseModel):
             raise_error(
                 TypeError,
-                "given circuit factory has wrong type {}, must be qibo NoiseModel | None .".format(
-                    type(noise_model)
-                ),
+                f"NoiseModel has wrong type {type(noise_model)}. NoiseModel must be qibo NoiseModel or None .",
             )
         self.__noise_model = noise_model
         self.name = "Abstract"
 
     @property
     def noise_model(self):
         return self.__noise_model
@@ -84,16 +76,16 @@
 
         Args:
             path (str): The directory from where the object should be restored.
 
         Returns:
             Experiment: The object with data (and circuitfactory).
         """
-        datapath = f"{path}experiment_data.pkl"
-        circuitspath = f"{path}circuits.pkl"
+        datapath = f"{path}/experiment_data.pkl"
+        circuitspath = f"{path}/circuits.pkl"
         if isfile(datapath):
             with open(datapath, "rb") as f:
                 data = pickle.load(f)
             if isinstance(data, pd.DataFrame):  # pragma: no cover
                 data = data.to_dict("records")
             nshots = len(data[0]["samples"])
         else:
@@ -103,36 +95,48 @@
                 circuitfactory = pickle.load(f)
         else:
             circuitfactory = None
         # Initiate an instance of the experiment class.
         obj = cls(circuitfactory, data=data, nshots=nshots)
         return obj
 
-    def save(self, path: str | None = None) -> str:
-        """Creates a path if None given and pickles relevant data from ``self.data``
-        and if ``self.circuitfactory`` is a list that one too.
+    def save_circuits(self, path: str | None = None, force: bool = False) -> str:
+        """Creates a path if None given and pickles ``self.circuitfactory``
+        if it is a list.
 
         Returns:
             (str): The path of stored experiment.
         """
 
-        # Check if path to store is given, if not create one. If yes check if the last character
-        # is a /, if not add it.
+        # Check if path to store is given, if not create one.
         if path is None:
-            self.path = experiment_directory("rb")
+            self.path = generate_output_folder(path, force)
         else:
-            self.path = path if path[-1] == "/" else f"{path}/"
-        # Only if the circuit factory is a list it will be stored.
+            self.path = path
         if isinstance(self.circuitfactory, list):
-            with open(f"{self.path}circuits.pkl", "wb") as f:
+            with open(f"{self.path}/circuits.pkl", "wb") as f:
                 pickle.dump(self.circuitfactory, f)
+        return self.path
+
+    def save(self, path: str | None = None, force: bool = False) -> str:
+        """Creates a path if None given and pickles relevant data from ``self.data``.
+
+        Returns:
+            (str): The path of stored experiment.
+        """
+
+        # Check if path to store is given, if not create one.
+        if path is None:
+            self.path = generate_output_folder(path, force)
+        else:
+            self.path = path
         # And only if data is not None the data list (full of dicionaries) will be
         # stored.
         if self.data is not None:
-            with open(f"{self.path}experiment_data.pkl", "wb") as f:
+            with open(f"{self.path}/experiment_data.pkl", "wb") as f:
                 pickle.dump(self.data, f)
         # It is convenient to know the path after storing, so return it.
         return self.path
 
     def extract(
         self, output_key: str, groupby_key: str = "", agg_type: str | Callable = ""
     ) -> np.ndarray | tuple[np.ndarray, np.ndarray]:
@@ -190,28 +194,24 @@
         """
         # Either the circuit factory or the data rows can be empty.
         # If ``self.data`` is not empty the actual list element is altered without
         # storing it after alternation.
         # Both ``circuit`` and ``datarow`` can be provided:
         if self.circuitfactory is not None and self.data is not None:
             for circuit, datarow in zip(self.circuitfactory, self.data):
-                datarow = sequential_task(
-                    copy_circuit(circuit.copy(deep=True)), datarow
-                )
+                datarow = sequential_task(circuit.copy(deep=True), datarow)
         # Only``datarow`` can be provided:
         elif self.circuitfactory is None and self.data is not None:
             for datarow in self.data:
                 datarow = sequential_task(None, datarow)
         # Only ``circuit`` can be provided:
         elif self.circuitfactory is not None and self.data is None:
             newdata = []
             for circuit in self.circuitfactory:
-                newdata.append(
-                    sequential_task(copy_circuit(circuit.copy(deep=True)), {})
-                )
+                newdata.append(sequential_task(circuit.copy(deep=True), {}))
             self.data = newdata
         else:
             raise_error(ValueError, "Both attributes circuitfactory and data are None.")
 
     def execute(self, circuit: Circuit, datarow: dict) -> dict:
         """Executes a circuit, returns the single shot results in a dict.
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/fitting.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/fitting.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,17 +25,35 @@
     return A * f**x + B
 
 
 def exp2_func(x: np.ndarray, A1: float, A2: float, f1: float, f2: float) -> np.ndarray:
     """Return :math:`A_1\\cdot f_1^x+A_2\\cdot f_2^x` where ``x`` is an ``np.ndarray`` and
     ``A1``, ``f1``, ``A2``, ``f2`` are floats. There is no linear offsett B.
     """
+    x = np.array(x, dtype=complex)
     return A1 * f1**x + A2 * f2**x
 
 
+def expn_func(x: Union[np.ndarray, list], *args) -> np.ndarray:
+    """Compute the sum of exponentials :math:`\\sum A_i\\cdot f_i^x`
+
+    Args:
+        x (np.ndarray | list): list of exponents.
+        *args: Parameters of type `float` in the order
+            :math:`A_1`, :math:`A_2`, :math:`f_1`, :math:`f_2`,...
+
+    Returns:
+        The resulting sum of exponentials.
+    """
+    A_list = np.array(args[: len(args) // 2], dtype=complex)
+    f_list = np.array(args[len(args) // 2 :], dtype=complex)
+    sum_of_exponentials = np.vectorize(lambda m: np.sum(A_list * (f_list**m)))
+    return sum_of_exponentials(np.real(x))
+
+
 def esprit(
     xdata: np.ndarray,
     ydata: np.ndarray,
     num_decays: int,
     hankel_dim: Optional[int] = None,
 ) -> np.ndarray:
     """Implements the ESPRIT algorithm for peak detection.
@@ -47,18 +65,17 @@
         hankel_dim (int | None, optional): The Hankel dimension. Defaults to None.
 
     Returns:
         np.ndarray: The decay parameters.
 
     Raises:
         ValueError: When the x-labels are not equally spaced the algorithm does not work.
-
     """
-    # Check for equally spacing.
-    if not np.all(xdata[1:] - xdata[:-1] == xdata[1] - xdata[0]):
+    # Check for equal spacing.
+    if np.any(xdata[1:] - xdata[:-1] != xdata[1] - xdata[0]):
         raise_error(ValueError, "xdata has to be equally spaced.")
     sampleRate = 1 / (xdata[1] - xdata[0])
     # xdata has to be an array.
     xdata = np.array(xdata)
     # Define the Hankel dimension if not given.
     if hankel_dim is None:
         hankel_dim = int(np.round(0.5 * xdata.size))
@@ -70,15 +87,17 @@
     # Calculate nontrivial (nonzero) singular vectors of the hankel matrix.
     U, _, _ = svd(hankelMatrix, full_matrices=False)
     # Cut off the columns to the amount which is needed.
     U_signal = U[:, :num_decays]
     # Calculte the solution.
     spectralMatrix = np.linalg.pinv(U_signal[:-1,]) @ U_signal[1:,]
     # Calculate the poles/eigenvectors and space them right. Return them.
-    return np.linalg.eigvals(spectralMatrix) * sampleRate
+    decays = np.linalg.eigvals(spectralMatrix)
+    decays = np.array(decays, dtype=complex)
+    return decays**sampleRate
 
 
 def fit_exp1B_func(
     xdata: Union[np.ndarray, list], ydata: Union[np.ndarray, list], **kwargs
 ) -> Tuple[tuple, tuple]:
     """Calculate an single exponential A*p^m+B fit to the given ydata.
 
@@ -93,15 +112,15 @@
 
     # Check if all the values in ``ydata``are the same. That would make the
     # exponential fit unnecessary.
     if np.all(ydata == ydata[0]):
         popt, perr = (ydata[0], 1.0, 0), (0, 0, 0)
     else:
         # Get a guess for the exponential function.
-        guess = kwargs.get("p0", [0.5, 0.9, 0.8])
+        guess = kwargs.get("p0", (np.max(ydata) - np.mean(ydata), 0.9, np.mean(ydata)))
         # If the search for fitting parameters does not work just return
         # fixed parameters where one can see that the fit did not work
         try:
             popt, pcov = curve_fit(
                 exp1B_func,
                 xdata,
                 ydata,
@@ -148,14 +167,37 @@
             perr = tuple(np.sqrt(np.diag(pcov)))
         except:
             popt, perr = (0, 0), (0, 0)
 
     return popt, perr
 
 
+def fit_expn_func(
+    xdata: Union[np.ndarray, list], ydata: Union[np.ndarray, list], n: int = 2, **kwargs
+) -> Tuple[tuple, tuple]:
+    """Calculate n exponentials on top of each other, fit to the given ydata.
+    No linear offset, the ESPRIT algorithm is used to identify ``n`` exponential decays.
+
+    Args:
+        xdata (Union[np.ndarray, list]): The x-labels.
+        ydata (Union[np.ndarray, list]): The data to be fitted.
+        n (int): number of decays to fit. Default is 2.
+
+    Returns:
+        Tuple[tuple, tuple]: (A1, ..., An, f1, ..., fn) with f* the decay parameters.
+    """
+
+    # TODO how are the errors estimated?
+    # TODO the data has to have a sufficiently big size, check that.
+    decays = esprit(np.array(xdata), np.array(ydata), n)
+    vandermonde = np.array([decays**x for x in xdata])
+    alphas = np.linalg.pinv(vandermonde) @ np.array(ydata).reshape(-1, 1).flatten()
+    return tuple([*alphas, *decays]), (0,) * (len(alphas) + len(decays))
+
+
 def fit_exp2_func(
     xdata: Union[np.ndarray, list], ydata: Union[np.ndarray, list], **kwargs
 ) -> Tuple[tuple, tuple]:
     """Calculate 2 exponentials on top of each other, fit to the given ydata.
 
     No linear offset, the ESPRIT algorithm is used to identify the two exponential decays.
 
@@ -163,14 +205,8 @@
         xdata (Union[np.ndarray, list]): The x-labels.
         ydata (Union[np.ndarray, list]): The data to be fitted
 
     Returns:
         Tuple[tuple, tuple]: (A1, A2, f1, f2) with f* the decay parameters.
     """
 
-    # TODO how are the errors estimated?
-    # TODO the data has to have a sufficiently big size, check that.
-    decays = esprit(np.array(xdata), np.array(ydata), 2)
-    vandermonde = np.vander(decays, N=xdata[-1] + 1, increasing=True)
-    vandermonde = np.take(vandermonde, xdata, axis=1)
-    alphas = np.linalg.pinv(vandermonde.T) @ np.array(ydata).reshape(-1, 1).flatten()
-    return tuple([*alphas, *decays]), (0, 0, 0, 0)
+    return fit_expn_func(xdata, ydata, 2)
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/noisemodels.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/noisemodels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-""" Costum error models are build here for making it possible to pass
+""" Custom error models are build here for making it possible to pass
 strings describing the error model via runcards in qibocal.
 They inherit from the qibo noise NoiseModel module and are prebuild.
 """
 
 import numpy as np
 from qibo import gates
 from qibo.noise import NoiseModel, PauliError
 
 from qibocal.config import raise_error
 
 
-class PauliErrorOnUnitary(NoiseModel):
-    """Builds a noise model with pauli flips acting on unitaries.
-
+class PauliErrorOnAll(NoiseModel):
+    """Builds a noise model with pauli flips
+    acting on all gates in a Circuit.
     If no initial parameters for px, py, pz are given, random values
     are drawn (in sum not bigger than 1).
     """
 
     def __init__(self, *args) -> None:
         super().__init__()
         # Check if number of arguments is 0 or 1 and if it's equal to None
@@ -25,30 +25,27 @@
             params = np.random.uniform(0, 0.25, size=3)
         elif len(args) == 3:
             params = args
         else:
             # Raise ValueError if given paramters are wrong.
             raise_error(
                 ValueError,
-                "Wrong number of error parameters, 3 != {}.".format(len(args)),
+                f"Wrong number of error parameters, 3 != {len(args)}.",
             )
         self.build(*params)
 
     def build(self, *params):
-        # Add PauliError to gates.Unitary
-        self.add(PauliError(*params), gates.Unitary)
+        # TODO for qibo v.0.1.14 change *params to list(zip(["X", "Y", "Z"], params))
+        # Add PauliError to gates.Gate
+        self.add(PauliError(*params))
 
 
-class PauliErrorOnX(PauliErrorOnUnitary):
+class PauliErrorOnX(PauliErrorOnAll):
     """Builds a noise model with pauli flips acting on X gates.
-
-    Inherited from ``PauliErrorOnUnitary`` but the ``build`` method is
+    Inherited from ``PauliErrorOnAll`` but the ``build`` method is
     overwritten to act on X gates.
     If no initial parameters for px, py, pz are given, random values
     are drawn (in sum not bigger than 1).
     """
 
-    def __init__(self, *args) -> None:
-        super().__init__(*args)
-
     def build(self, *params):
         self.add(PauliError(*params), gates.X)
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/basics/plot.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/basics/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 import qibocal.calibrations.niGSC.basics.fitting as fitting_methods
-from qibocal.calibrations.niGSC.basics import utils
 from qibocal.calibrations.niGSC.basics.experiment import Experiment
+from qibocal.calibrations.niGSC.basics.utils import number_to_str
 
 
 def plot_qq(folder: str, routine: str, qubit, format):
-    fitting_report = ""
     """Load the module for which the plot has to be done.
 
-
     Args:
         folder (str): The folder path where the data was stored.
         routine (str): The routine name, here the module name.
         qubit (Any): Is not used here
         format (Any): Is not used here.
 
     Returns:
@@ -29,15 +27,16 @@
     module = importlib.import_module(f"qibocal.calibrations.niGSC.{routine}")
     # Load the experiment with the class method ``load``.
     experiment = module.ModuleExperiment.load(f"{folder}/data/{routine}/")
     # In this data frame the precomputed fitting parameters and other
     # parameters for fitting and plotting are stored.
     aggr_df = pd.read_pickle(f"{folder}/data/{routine}/fit_plot.pkl")
     # Build the figure/report using the responsible module.
-    plotly_figure = module.build_report(experiment, aggr_df)
+    plotly_figure, fitting_report = module.build_report(experiment, aggr_df)
+
     return [plotly_figure], fitting_report
 
 
 class Report:
     """Once initialized with the correct parameters an Report object can build
     reports to display results of a gate set characterization experiment.
     """
@@ -51,112 +50,105 @@
         l = len(self.all_figures)
         if l < 3:
             divide_by = 1
         else:
             divide_by = 2
         subplot_titles = [figdict.get("subplot_title") for figdict in self.all_figures]
         fig = make_subplots(
-            rows=int(l / divide_by) + l % divide_by + 1,
+            rows=int(l / divide_by) + l % divide_by,
             cols=1 if l == 1 else divide_by,
             subplot_titles=subplot_titles,
+            horizontal_spacing=0.1,
+            vertical_spacing=0.1,
         )
         for count, fig_dict in enumerate(self.all_figures):
             plot_list = fig_dict["figs"]
             for plot in plot_list:
                 fig.add_trace(
                     plot, row=count // divide_by + 1, col=count % divide_by + 1
                 )
 
-        fig.add_annotation(
-            dict(
-                bordercolor="black",
-                font=dict(color="black", size=16),
-                x=0.0,
-                y=1.0 / (int(l / divide_by) + l % divide_by + 1)
-                - len(self.info_dict) * 0.005,
-                showarrow=False,
-                text="<br>".join(
-                    [f"{key} : {value}\n" for key, value in self.info_dict.items()]
-                ),
-                align="left",
-                textangle=0,
-                yanchor="top",
-                xref="paper",
-                yref="paper",
-            )
-        )
         fig.update_xaxes(title_font_size=18, tickfont_size=16)
         fig.update_yaxes(title_font_size=18, tickfont_size=16)
         fig.update_layout(
             font_family="Averta",
             hoverlabel_font_family="Averta",
             title_text=self.title,
             title_font_size=24,
             legend_font_size=16,
             hoverlabel_font_size=16,
             showlegend=True,
-            height=500 * (int(l / divide_by) + l % divide_by)
-            if l > divide_by
-            else 1000,
+            height=300 * (int(l / divide_by) + l % divide_by) if l > divide_by else 500,
             width=1000,
         )
 
-        return fig
+        return fig, self.info_table()
+
+    def info_table(self):
+        return "".join(
+            [f"q/r | {key}: {value}<br>" for key, value in self.info_dict.items()]
+        )
 
 
 def scatter_fit_fig(
     experiment: Experiment,
     df_aggr: pd.DataFrame,
     xlabel: str,
     index: str,
     fittingparam_label="popt",
 ):
+    """
+    Generate a figure dictionary for plotly.
+
+    Args:
+        experiment (:class:`qibocal.calibrations.niGSC.basics.experiment.Experiment`):
+            an RB experiment that contains a dataframe with the information for the figure.
+        df_aggr (pd.DataFrame): DataFrame containing aggregational data about the RB experiment.
+        xlabel (str): key for x values in experiment.dataframe[xlabel] and df_aggr[xlabel].
+        index (str): key for y values in experiment.dataframe[index] and df_aggr[index].
+        fittingparam_label (str): key in df_aggr with a dictionary containing the parameters
+        for the dfrow["fit_func"]. Default is "popt".
+
+    Returns:
+        dict: dictionary for the plotly figure.
+    """
     fig_traces = []
     dfrow = df_aggr.loc[index]
     fig_traces.append(
         go.Scatter(
             x=experiment.dataframe[xlabel],
-            y=experiment.dataframe[index],
+            y=np.real(experiment.dataframe[index]),
             line=dict(color="#6597aa"),
             mode="markers",
             marker={"opacity": 0.2, "symbol": "square"},
             name="runs",
         )
     )
     fig_traces.append(
         go.Scatter(
             x=dfrow[xlabel],
-            y=dfrow["data"],
+            y=np.real(dfrow["data"]),
             line=dict(color="#aa6464"),
             mode="markers",
             name="average",
         )
     )
     x_fit = np.linspace(min(dfrow[xlabel]), max(dfrow[xlabel]), len(dfrow[xlabel]) * 20)
-    if "imag" in fittingparam_label:
-        y_fit = np.imag(
-            getattr(fitting_methods, dfrow["fit_func"])(
-                x_fit, *dfrow[fittingparam_label].values()
-            )
-        )
-    else:
-        y_fit = np.real(
-            getattr(fitting_methods, dfrow["fit_func"])(
-                x_fit, *dfrow[fittingparam_label].values()
-            )
+    y_fit = np.real(
+        getattr(fitting_methods, dfrow["fit_func"])(
+            x_fit, *dfrow[fittingparam_label].values()
         )
+    )
     fig_traces.append(
         go.Scatter(
             x=x_fit,
             y=y_fit,
             name="".join(
                 [
-                    "{}:{} ".format(
-                        key, utils.number_to_str(dfrow[fittingparam_label][key])
-                    )
-                    for key in dfrow[fittingparam_label]
+                    f"{key}={number_to_str(value)} "
+                    for key, value in dfrow[fittingparam_label].items()
                 ]
             ),
             line=go.scatter.Line(dash="dot"),
         )
     )
     return {"figs": fig_traces, "xlabel": xlabel, "ylabel": index}
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/simulfilteredrb.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/simulfilteredrb.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from qibo.models import Circuit
 from qibo.noise import NoiseModel
 
 import qibocal.calibrations.niGSC.basics.fitting as fitting_methods
 from qibocal.calibrations.niGSC.basics.circuitfactory import SingleCliffordsFactory
 from qibocal.calibrations.niGSC.basics.experiment import Experiment
 from qibocal.calibrations.niGSC.basics.plot import Report, scatter_fit_fig
+from qibocal.calibrations.niGSC.basics.utils import number_to_str
 
 
 class ModuleFactory(SingleCliffordsFactory):
     pass
 
 
 class ModuleExperiment(Experiment):
@@ -61,15 +62,15 @@
         datadict = super().execute(circuit, datarow)
         # Measurement gate should not contribute to depth, therefore -1.
         # Take the amount of qubits into account.
         datadict["depth"] = int((circuit.ngates - 1) / len(datadict["samples"][0]))
         return datadict
 
 
-class moduleReport(Report):
+class ModuleReport(Report):
     def __init__(self) -> None:
         super().__init__()
         self.title = "Correlated Filtered Randomized Benchmarking"
 
 
 def filter_function(circuit: Circuit, datarow: dict) -> dict:
     """Calculates the filtered signal for every crosstalk irrep.
@@ -202,32 +203,41 @@
     build a reprot as plotly figure.
 
     Args:
         experiment (Experiment): After sequential postprocessing of the experiment data.
         df_aggr (pd.DataFrame): Normally build with ``get_aggregational_data`` function.
 
     Returns:
-        (Figure): A plotly.graphical_object.Figure object.
+        (tuple): A `plotly.graphical_object.Figure` object and a string corresponding to a table.
     """
 
     # Initiate a report object.
-    report = moduleReport()
-    # Add general information to the object.
+    report = ModuleReport()
+    # Add general information to the table.
+
     report.info_dict["Number of qubits"] = len(experiment.data[0]["samples"][0])
     report.info_dict["Number of shots"] = len(experiment.data[0]["samples"])
     report.info_dict["runs"] = experiment.extract("samples", "depth", "count")[1][0]
     lambdas = iter(product([0, 1], repeat=int(report.info_dict["Number of qubits"])))
     for kk, l in enumerate(lambdas):
-        # Add the fitting errors which will be displayed in a box under the plots.
-        report.info_dict[f"Fitting daviations irrep {l}"] = "".join(
-            [
-                "{}:{:.3f} ".format(key, df_aggr.loc[f"irrep{kk}"]["perr"][key])
-                for key in df_aggr.loc[f"irrep{kk}"]["perr"]
-            ]
+        # Add the fitting parameters and  errors.
+        dfrow = df_aggr.loc[f"irrep{kk}"]
+        popt_pairs = (
+            list(dfrow["popt"].items())[::2] + list(dfrow["popt"].items())[1::2]
+        )
+        report.info_dict[f"Irrep {l} Fit"] = "".join(
+            [f"{key}={number_to_str(value)} " for key, value in popt_pairs]
+        )
+        perr_pairs = (
+            list(dfrow["perr"].items())[::2] + list(dfrow["perr"].items())[1::2]
+        )
+        report.info_dict[f"Irrep {l} Deviations"] = "".join(
+            [f"{key}={number_to_str(value)} " for key, value in perr_pairs]
         )
         # Use the predefined ``scatter_fit_fig`` function from ``basics.utils`` to build the wanted
         # plotly figure with the scattered filter function points and then mean per depth.
         figdict = scatter_fit_fig(experiment, df_aggr, "depth", f"irrep{kk}")
         # Add a subplot title for each irrep.
         figdict["subplot_title"] = f"Irrep {l}"
         report.all_figures.append(figdict)
+    # Return the figure of the report object and the corresponding table.
     return report.build()
```

### Comparing `qibocal-0.0.1/src/qibocal/calibrations/niGSC/standardrb.py` & `qibocal-0.0.2/src/qibocal/calibrations/niGSC/standardrb.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from qibo.models import Circuit
 from qibo.noise import NoiseModel
 
 import qibocal.calibrations.niGSC.basics.fitting as fitting_methods
 from qibocal.calibrations.niGSC.basics.circuitfactory import SingleCliffordsFactory
 from qibocal.calibrations.niGSC.basics.experiment import Experiment
 from qibocal.calibrations.niGSC.basics.plot import Report, scatter_fit_fig
-from qibocal.calibrations.niGSC.basics.utils import gate_fidelity
+from qibocal.calibrations.niGSC.basics.utils import gate_fidelity, number_to_str
 
 
 class ModuleFactory(SingleCliffordsFactory):
     def __init__(self, nqubits: int, depths: list, qubits: list = []) -> None:
         super().__init__(nqubits, depths, qubits)
         self.name = "SingleCliffordsInv"
 
@@ -92,15 +92,15 @@
         datarow = super().execute(circuit, datarow)
         # Substract 1 for sequence length to not count the inverse gate and
         # substract the measurement gate.
         datarow["depth"] = (circuit.depth - 2) if circuit.depth > 1 else 0
         return datarow
 
 
-class moduleReport(Report):
+class ModuleReport(Report):
     def __init__(self) -> None:
         super().__init__()
         self.title = "Standard Randomized Benchmarking"
 
 
 def groundstate_probabilities(circuit: Circuit, datarow: dict) -> dict:
     """Calculates the ground state probability with data from single shot measurements.
@@ -186,36 +186,38 @@
     build a report as plotly figure.
 
     Args:
         experiment (Experiment): After sequential postprocessing of the experiment data.
         df_aggr (pd.DataFrame): Normally build with ``get_aggregational_data`` function.
 
     Returns:
-        (Figure): A plotly.graphical_object.Figure object.
+        (tuple): A `plotly.graphical_object.Figure` object and a string corresponding to a table.
     """
 
     # Initiate a report object.
-    report = moduleReport()
-    # Add general information to the object.
+    report = ModuleReport()
+
+    # Add general information to the table.
     report.info_dict["Number of qubits"] = len(experiment.data[0]["samples"][0])
     report.info_dict["Number of shots"] = len(experiment.data[0]["samples"])
     report.info_dict["runs"] = experiment.extract("samples", "depth", "count")[1][0]
-    report.info_dict["Fitting daviations"] = "".join(
-        [
-            "{}:{:.3f} ".format(key, df_aggr.iloc[0]["perr"][key])
-            for key in df_aggr.iloc[0]["perr"]
-        ]
-    )
     report.info_dict["Gate fidelity"] = "{:.4f}".format(
         gate_fidelity(df_aggr.iloc[0]["popt"]["p"])
     )
     report.info_dict["Gate fidelity primitive"] = "{:.4f}".format(
         gate_fidelity(df_aggr.iloc[0]["popt"]["p"], primitive=True)
     )
+    dfrow = df_aggr.loc["groundstate probability"]
+    report.info_dict["Fit"] = "".join(
+        [f"{key}={number_to_str(value)} " for key, value in dfrow["popt"].items()]
+    )
+    report.info_dict["Fitting deviations"] = "".join(
+        [f"{key}={number_to_str(value)} " for key, value in dfrow["perr"].items()]
+    )
     # Use the predefined ``scatter_fit_fig`` function from ``basics.plot`` to build the wanted
     # plotly figure with the scattered ground state probability data along with the mean for
     # each depth and the exponential fit for the means.
     report.all_figures.append(
         scatter_fit_fig(experiment, df_aggr, "depth", "groundstate probability")
     )
-    # Return the figure the report object builds out of all figures added to the report.
+    # Return the figure of the report object and the corresponding table.
     return report.build()
```

### Comparing `qibocal-0.0.1/src/qibocal/cli/builders.py` & `qibocal-0.0.2/src/qibocal/cli/builders.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,19 @@
 import inspect
 import os
 import shutil
 
 import yaml
 
 from qibocal import calibrations
-from qibocal.config import log, raise_error
+from qibocal.cli.utils import generate_output_folder, load_yaml
+from qibocal.config import raise_error
 from qibocal.data import Data
 
 
-def load_yaml(path):
-    """Load yaml file from disk."""
-    with open(path) as file:
-        data = yaml.safe_load(file)
-    return data
-
-
 class ActionParser:
     """Class for parsing and executing single actions in the runcard."""
 
     def __init__(self, runcard, folder, name):
         self.runcard = runcard
         self.folder = folder
         self.func = None
@@ -34,15 +28,14 @@
 
     def build(self):
         """Load function from :func:`qibocal.characterization.calibrations` and check arguments"""
         if not os.path.exists(self.path):
             os.makedirs(self.path)
         # collect function from module
         self.func = getattr(calibrations, self.name)
-
         sig = inspect.signature(self.func)
         self.params = self.runcard["actions"][self.name]
         for param in list(sig.parameters)[2:-1]:
             if param not in self.params:
                 raise_error(AttributeError, f"Missing parameter {param} in runcard.")
 
     def execute(self, data_format, platform, qubits):
@@ -72,15 +65,15 @@
         self.nshots = self.runcard["actions"][self.name]["nshots"]
 
         from qibocal.calibrations.niGSC.basics import noisemodels
 
         try:
             self.noise_params = self.runcard["actions"][self.name]["noise_params"]
         except KeyError:
-            self.noise_params = None
+            self.noise_params = []
         try:
             self.noise_model = getattr(
                 noisemodels, self.runcard["actions"][self.name]["noise_model"]
             )(*self.noise_params)
         except:
             self.noise_model = None
 
@@ -115,14 +108,16 @@
         # Initiate the factory and the experiment.
         factory = self.module.ModuleFactory(
             self.nqubits, self.depths * self.runs, qubits=self.runcard["qubits"]
         )
         experiment = self.module.ModuleExperiment(
             factory, nshots=self.nshots, noise_model=self.noise_model
         )
+        # Store the circuits.
+        experiment.save_circuits(self.path)
         # Execute the circuits in the experiment.
         experiment.perform(experiment.execute)
         # Run the row by row postprocessing.
         self.module.post_processing_sequential(experiment)
         # Run aggregational tasks along with fitting.
         # This will return a data frame, store it right away.
         self.module.get_aggregational_data(experiment).to_pickle(
@@ -137,148 +132,125 @@
     Args:
         runcard (path): path containing the runcard.
         folder (path): path for the output folder.
         force (bool): option to overwrite the output folder if it exists already.
     """
 
     def __init__(self, runcard, folder=None, force=False):
-        path, self.folder = self._generate_output_folder(folder, force)
+        # setting output folder
+        self.folder = generate_output_folder(folder, force)
+
+        # parse runcard
         self.runcard = load_yaml(runcard)
-        # Qibolab default backend if not provided in runcard.
+
+        # backend and platform allocation
         backend_name = self.runcard.get("backend", "qibolab")
         platform_name = self.runcard.get("platform", "dummy")
         platform_runcard = self.runcard.get("runcard", None)
         self.backend, self.platform = self._allocate_backend(
-            backend_name, platform_name, path, platform_runcard
+            backend_name, platform_name, platform_runcard
         )
-        if self.platform is not None:
-            self.qubits = {
-                q: self.platform.qubits[q]
-                for q in self.runcard["qubits"]
-                if q in self.platform.qubits
-            }
+        if "qubits" in self.runcard:
+            if self.platform is not None:
+                self.qubits = {
+                    q: self.platform.qubits[q]
+                    for q in self.runcard["qubits"]
+                    if q in self.platform.qubits
+                }
+            else:
+                self.qubits = self.runcard.get("qubits")
         else:
-            self.qubits = self.runcard.get("qubits")
-        self.format = self.runcard["format"]
+            self.qubits = []
 
+        # Setting format. If absent csv is used.
+        self.format = self.runcard.get("format", "csv")
         # Saving runcard
-        shutil.copy(runcard, f"{path}/runcard.yml")
-        self.save_meta(path, self.folder)
+        shutil.copy(runcard, f"{self.folder}/runcard.yml")
+        self.save_meta()
 
-    @staticmethod
-    def _generate_output_folder(folder, force):
-        """Static method for generating the output folder.
-        Args:
-            folder (path): path for the output folder. If None it will be created a folder automatically
-            force (bool): option to overwrite the output folder if it exists already.
-        """
-        if folder is None:
-            import getpass
-
-            e = datetime.datetime.now()
-            user = getpass.getuser().replace(".", "-")
-            date = e.strftime("%Y-%m-%d")
-            folder = f"{date}-{'000'}-{user}"
-            num = 0
-            while os.path.exists(folder):
-                log.info(f"Directory {folder} already exists.")
-                num += 1
-                folder = f"{date}-{str(num).rjust(3, '0')}-{user}"
-                log.info(f"Trying to create directory {folder}")
-        elif os.path.exists(folder) and not force:
-            raise_error(RuntimeError, f"Directory {folder} already exists.")
-        elif os.path.exists(folder) and force:
-            log.warning(f"Deleting previous directory {folder}.")
-            shutil.rmtree(os.path.join(os.getcwd(), folder))
-
-        path = os.path.join(os.getcwd(), folder)
-        log.info(f"Creating directory {folder}.")
-        os.makedirs(path)
-        return path, folder
-
-    def _allocate_backend(self, backend_name, platform_name, path, platform_runcard):
+    def _allocate_backend(self, backend_name, platform_name, platform_runcard):
         """Allocate the platform using Qibolab."""
         from qibo.backends import GlobalBackend, set_backend
 
         if backend_name == "qibolab":
             if platform_runcard is None:
                 from qibolab.paths import qibolab_folder
 
                 original_runcard = qibolab_folder / "runcards" / f"{platform_name}.yml"
             else:
                 original_runcard = platform_runcard
             # copy of the original runcard that will stay unmodified
-            shutil.copy(original_runcard, f"{path}/platform.yml")
+            shutil.copy(original_runcard, f"{self.folder}/platform.yml")
             # copy of the original runcard that will be modified during calibration
             updated_runcard = f"{self.folder}/new_platform.yml"
             shutil.copy(original_runcard, updated_runcard)
             # allocate backend with updated_runcard
             set_backend(
                 backend=backend_name, platform=platform_name, runcard=updated_runcard
             )
             backend = GlobalBackend()
             return backend, backend.platform
         else:
             set_backend(backend=backend_name, platform=platform_name)
             backend = GlobalBackend()
             return backend, None
 
-    def save_meta(self, path, folder):
+    def save_meta(self):
         import qibocal
 
         e = datetime.datetime.now(datetime.timezone.utc)
         meta = {}
-        meta["title"] = folder
+        meta["title"] = self.folder
         meta["backend"] = str(self.backend)
         meta["platform"] = str(self.backend.platform)
         meta["date"] = e.strftime("%Y-%m-%d")
         meta["start-time"] = e.strftime("%H:%M:%S")
         meta["end-time"] = e.strftime("%H:%M:%S")
         meta["versions"] = self.backend.versions  # pylint: disable=E1101
         meta["versions"]["qibocal"] = qibocal.__version__
 
-        with open(f"{path}/meta.yml", "w") as file:
+        with open(f"{self.folder}/meta.yml", "w") as file:
             yaml.dump(meta, file)
 
     def execute(self):
         """Method to execute sequentially all the actions in the runcard."""
         if self.platform is not None:
             self.platform.connect()
             self.platform.setup()
             self.platform.start()
 
         actions = []
         for action in self.runcard["actions"]:
             actions.append(action)
-            try:
-                parser = niGSCactionParser(self.runcard, self.folder, action)
-                parser.build()
-                parser.execute(self.format, self.platform)
-            # TODO: find a better way to choose between the two parsers
-            except (ModuleNotFoundError, KeyError):
+            if hasattr(calibrations, action):
                 parser = ActionParser(self.runcard, self.folder, action)
                 parser.build()
                 parser.execute(self.format, self.platform, self.qubits)
-                for qubit in self.qubits:
-                    if self.platform is not None:
-                        self.update_platform_runcard(qubit, action)
+            else:
+                parser = niGSCactionParser(self.runcard, self.folder, action)
+                parser.build()
+                parser.execute(self.format, self.platform)
+
+            for qubit in self.qubits:
+                if self.platform is not None:
+                    self.update_platform_runcard(qubit, action)
             self.dump_report(actions)
 
         if self.platform is not None:
             self.platform.stop()
             self.platform.disconnect()
 
     def update_platform_runcard(self, qubit, routine):
         try:
             data_fit = Data.load_data(self.folder, "data", routine, self.format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except FileNotFoundError:
             return None
 
-        params = data_fit.df.to_dict("index")[qubit if qubit == 0 else qubit - 1]
+        params = data_fit.df[data_fit.df["qubit"] == qubit]
         settings = load_yaml(f"{self.folder}/new_platform.yml")
         for param in params:
             if param in list(self.qubits[qubit].__annotations__.keys()):
                 setattr(self.qubits[qubit], param, params[param])
                 settings["characterization"]["single_qubit"][qubit][param] = int(
                     data_fit.get_values(param)
                 )
@@ -324,23 +296,20 @@
         self.qubits = self.runcard.get("qubits")
 
         # create calibration routine objects
         # (could be incorporated to :meth:`qibocal.cli.builders.ActionBuilder._build_single_action`)
         self.routines = []
         if actions is None:
             actions = self.runcard.get("actions")
-
         for action in actions:
             if hasattr(calibrations, action):
                 routine = getattr(calibrations, action)
-            elif hasattr(calibrations.niGSC, action):
+            else:
                 routine = niGSCactionParser(self.runcard, self.path, action)
                 routine.load_plot()
-            else:
-                raise_error(ValueError, f"Undefined action {action} in report.")
 
             if not hasattr(routine, "plots"):
                 routine.plots = []
             self.routines.append(routine)
 
     def get_routine_name(self, routine):
         """Prettify routine's name for report headers."""
@@ -352,20 +321,28 @@
         Args:
             routine (Callable): Calibration method.
             method (Callable): Plot method.
             qubit (int): Qubit id.
         """
         import tempfile
 
-        figures, _ = method(self.path, routine.__name__, qubit, self.format)
+        figures, fitting_report = method(
+            self.path, routine.__name__, qubit, self.format
+        )
         with tempfile.NamedTemporaryFile(delete=False) as temp:
+            html_list = []
             for figure in figures:
                 figure.write_html(temp.name, include_plotlyjs=False, full_html=False)
+                temp.seek(0)
                 fightml = temp.read().decode("utf-8")
-        return fightml
+                html_list.append(fightml)
+
+            all_html = "".join(html_list)
+
+        return all_html, fitting_report
 
     def get_live_figure(self, routine, method, qubit):
         """Get url to dash page for live plotting.
 
         This url is used by :meth:`qibocal.web.app.get_graph`.
 
         Args:
```

### Comparing `qibocal-0.0.1/src/qibocal/config.py` & `qibocal-0.0.2/src/qibocal/config.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/data.py` & `qibocal-0.0.2/src/qibocal/data.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/decorators.py` & `qibocal-0.0.2/src/qibocal/decorators.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/fitting/methods.py` & `qibocal-0.0.2/src/qibocal/fitting/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Routine-specific method for post-processing data acquired."""
 from functools import partial
 
 import lmfit
 import numpy as np
+import pandas as pd
+import pint
 from scipy.optimize import curve_fit
 
 from qibocal.config import log
 from qibocal.data import Data
 from qibocal.fitting.utils import (
     cos,
+    cumulative,
     exp,
     flipping,
     freq_q_mathieu,
     freq_r_mathieu,
     freq_r_transmon,
     line,
     lorenzian,
     parse,
+    pint_to_float,
     rabi,
     ramsey,
 )
 
 
 def lorentzian_fit(data, x, y, qubits, resonator_type, labels, fit_file_name=None):
     r"""
@@ -159,23 +163,23 @@
             .groupby("frequency", as_index=False)
             .mean()
         )
         frequencies_keys = parse(x)
         voltages_keys = parse(y)
         frequencies = (
             qubit_data[frequencies_keys[0]].pint.to(frequencies_keys[1]).pint.magnitude
-        )
+        )  # convert frequencies to GHz for better fitting
         voltages = qubit_data[voltages_keys[0]].pint.to(voltages_keys[1]).pint.magnitude
 
         # Create a lmfit model for fitting equation defined in resonator_peak
         model_Q = lmfit.Model(lorenzian)
 
         # Guess parameters for Lorentzian max or min
         if (resonator_type == "3D" and "readout_frequency" in labels[0]) or (
-            resonator_type != "3D" and labels[0] == "drive_frequency"
+            resonator_type == "2D" and "drive_frequency" in labels[0]
         ):
             guess_center = frequencies[
                 np.argmax(voltages)
             ]  # Argmax = Returns the indices of the maximum values along an axis.
             guess_offset = np.mean(
                 voltages[np.abs(voltages - np.mean(voltages) < np.std(voltages))]
             )
@@ -200,41 +204,43 @@
         guess_parameters = model_Q.make_params()
 
         # fit the model with the data and guessed parameters
         try:
             fit_res = model_Q.fit(
                 data=voltages, frequency=frequencies, params=guess_parameters
             )
-        except:
-            log.warning("lorentzian_fit: the fitting was not successful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
+            # get the values for postprocessing and for legend.
+            f0 = fit_res.best_values["center"]
+            BW = fit_res.best_values["sigma"] * 2
+            Q = abs(f0 / BW)
+            peak_voltage = (
+                fit_res.best_values["amplitude"]
+                / (fit_res.best_values["sigma"] * np.pi)
+                + fit_res.best_values["offset"]
+            )
 
-        # get the values for postprocessing and for legend.
-        f0 = fit_res.best_values["center"]
-        BW = fit_res.best_values["sigma"] * 2
-        Q = abs(f0 / BW)
-        peak_voltage = (
-            fit_res.best_values["amplitude"] / (fit_res.best_values["sigma"] * np.pi)
-            + fit_res.best_values["offset"]
-        )
+            freq = f0 * 1e9
 
-        freq = f0
+            data_fit.add(
+                {
+                    labels[0]: freq,
+                    labels[1]: peak_voltage,
+                    "popt0": fit_res.best_values["amplitude"],
+                    "popt1": fit_res.best_values["center"],
+                    "popt2": fit_res.best_values["sigma"],
+                    "popt3": fit_res.best_values["offset"],
+                    "qubit": qubit,
+                }
+            )
+        except:
+            log.warning("lorentzian_fit: the fitting was not successful")
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-        data_fit.add(
-            {
-                labels[0]: freq,
-                labels[1]: peak_voltage,
-                "popt0": fit_res.best_values["amplitude"],
-                "popt1": fit_res.best_values["center"],
-                "popt2": fit_res.best_values["sigma"],
-                "popt3": fit_res.best_values["offset"],
-                "qubit": qubit,
-            }
-        )
     return data_fit
 
 
 def rabi_fit(data, x, y, qubits, resonator_type, labels):
     r"""
     Fitting routine for Rabi experiment. The used model is
 
@@ -262,15 +268,15 @@
             - **popt4**: T2
             - **labels[0]**: pulse parameter
             - **labels[1]**: pulse's maximum voltage
             - **qubit**: The qubit being tested
     """
 
     data_fit = Data(
-        name=f"fits",
+        name="fits",
         quantities=[
             "popt0",
             "popt1",
             "popt2",
             "popt3",
             "popt4",
             labels[0],
@@ -313,31 +319,32 @@
             popt, pcov = curve_fit(
                 rabi, parameter.values, voltages.values, p0=pguess, maxfev=10000
             )
             smooth_dataset = rabi(parameter.values, *popt)
             pi_pulse_parameter = np.abs((1.0 / popt[2]) / 2)
             pi_pulse_peak_voltage = smooth_dataset.max()
             t2 = 1.0 / popt[4]  # double check T1
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    "popt3": popt[3],
+                    "popt4": popt[4],
+                    labels[0]: pi_pulse_parameter,
+                    labels[1]: pi_pulse_peak_voltage,
+                    "qubit": qubit,
+                }
+            )
         except:
             log.warning("rabi_fit: the fitting was not succesful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-        data_fit.add(
-            {
-                "popt0": popt[0],
-                "popt1": popt[1],
-                "popt2": popt[2],
-                "popt3": popt[3],
-                "popt4": popt[4],
-                labels[0]: pi_pulse_parameter,
-                labels[1]: pi_pulse_peak_voltage,
-                "qubit": qubit,
-            }
-        )
     return data_fit
 
 
 def ramsey_fit(
     data, x, y, qubits, resonator_type, qubit_freqs, sampling_rate, offset_freq, labels
 ):
     r"""
@@ -370,15 +377,15 @@
             - **popt4**: T2
             - **labels[0]**: Physical detunning of the actual qubit frequency
             - **labels[1]**: New qubit frequency after correcting the actual qubit frequency with the detunning calculated (labels[0])
             - **labels[2]**: T2
             - **qubit**: The qubit being tested
     """
     data_fit = Data(
-        name=f"fits",
+        name="fits",
         quantities=[
             "popt0",
             "popt1",
             "popt2",
             "popt3",
             "popt4",
             labels[0],
@@ -427,32 +434,34 @@
                 popt[3] - x_min * popt[2] / (x_max - x_min),
                 popt[4] / (x_max - x_min),
             ]
             delta_fitting = popt[2] / 2 * np.pi
             delta_phys = int((delta_fitting * sampling_rate) - offset_freq)
             corrected_qubit_frequency = int(qubit_freqs[qubit] + delta_phys)
             t2 = 1.0 / popt[4]
+
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    "popt3": popt[3],
+                    "popt4": popt[4],
+                    labels[0]: delta_phys,
+                    labels[1]: corrected_qubit_frequency,
+                    labels[2]: t2,
+                    "qubit": qubit,
+                }
+            )
         except:
             log.warning("ramsey_fit: the fitting was not succesful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-        data_fit.add(
-            {
-                "popt0": popt[0],
-                "popt1": popt[1],
-                "popt2": popt[2],
-                "popt3": popt[3],
-                "popt4": popt[4],
-                labels[0]: delta_phys,
-                labels[1]: corrected_qubit_frequency,
-                labels[2]: t2,
-                "qubit": qubit,
-            }
-        )
     return data_fit
 
 
 def t1_fit(data, x, y, qubits, resonator_type, labels):
     """
     Fitting routine for T1 experiment. The used model is
 
@@ -516,29 +525,30 @@
             ]
 
         try:
             popt, pcov = curve_fit(
                 exp, times.values, voltages.values, p0=pguess, maxfev=2000000
             )
             t1 = abs(1 / popt[2])
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    labels[0]: t1,
+                    "qubit": qubit,
+                }
+            )
 
         except:
             log.warning("t1_fit: the fitting was not succesful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-    data_fit.add(
-        {
-            "popt0": popt[0],
-            "popt1": popt[1],
-            "popt2": popt[2],
-            labels[0]: t1,
-            "qubit": qubit,
-        }
-    )
     return data_fit
 
 
 def flipping_fit(data, x, y, qubits, resonator_type, pi_pulse_amplitudes, labels):
     r"""
     Fitting routine for T1 experiment. The used model is
 
@@ -603,32 +613,30 @@
         try:
             popt, pcov = curve_fit(flipping, flips, voltages, p0=pguess, maxfev=2000000)
             epsilon = -np.pi / popt[2]
             amplitude_correction_factor = np.pi / (np.pi + epsilon)
             corrected_amplitude = (
                 amplitude_correction_factor * pi_pulse_amplitudes[qubit]
             )
-            # angle = (niter * 2 * np.pi / popt[2] + popt[3]) / (1 + 4 * niter)
-            # amplitude_delta = angle * 2 / np.pi * pi_pulse_amplitude
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    "popt3": popt[3],
+                    labels[0]: amplitude_correction_factor,
+                    labels[1]: corrected_amplitude,
+                    "qubit": qubit,
+                }
+            )
         except:
             log.warning("flipping_fit: the fitting was not succesful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
-
-        data_fit.add(
-            {
-                "popt0": popt[0],
-                "popt1": popt[1],
-                "popt2": popt[2],
-                "popt3": popt[3],
-                labels[0]: amplitude_correction_factor,
-                labels[1]: corrected_amplitude,
-                "qubit": qubit,
-            }
-        )
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
     return data_fit
 
 
 def drag_tuning_fit(data: Data, x, y, qubits, labels):
     r"""
     Fitting routine for drag tunning. The used model is
@@ -692,30 +700,30 @@
             0.3,  # Phase:     p[3]
         ]
 
         try:
             popt, pcov = curve_fit(cos, beta_params.values, voltages.values)
             smooth_dataset = cos(beta_params.values, popt[0], popt[1], popt[2], popt[3])
             beta_optimal = beta_params.values[np.argmin(smooth_dataset)]
-
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    "popt3": popt[3],
+                    labels[0]: beta_optimal,
+                    "qubit": qubit,
+                }
+            )
         except:
             log.warning("drag_tuning_fit: the fitting was not succesful")
-            data_fit.add({key: 0 for key in data_fit.df.columns})
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-        data_fit.add(
-            {
-                "popt0": popt[0],
-                "popt1": popt[1],
-                "popt2": popt[2],
-                "popt3": popt[3],
-                labels[0]: beta_optimal,
-                "qubit": qubit,
-            }
-        )
     return data_fit
 
 
 def res_spectroscopy_flux_fit(data, x, y, qubit, fluxline, params_fit):
     """Fit frequency as a function of current for the flux resonator spectroscopy
         Args:
         data (DataUnits): Data file with information on the feature response at each current point.
@@ -829,15 +837,18 @@
                         "f_rs": f_rs,
                         "f_offset": f_offset,
                         "C_ii": C_ii,
                     }
                 )
         except:
             log.warning("The fitting was not successful")
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
+
     else:
         data_fit = Data(
             name=f"fit1_q{qubit}_f{fluxline}",
             quantities=[
                 "popt0",
                 "popt1",
             ],
@@ -845,33 +856,37 @@
         try:
             freq_min = np.min(freq)
             freq_max = np.max(freq)
             freq_norm = (freq - freq_min) / (freq_max - freq_min)
             popt = curve_fit(line, curr, freq_norm)[0]
             popt[0] = popt[0] * (freq_max - freq_min)
             popt[1] = popt[1] * (freq_max - freq_min) + freq_min
+            data_fit.add(
+                {
+                    "popt0": popt[0],  # C_ij
+                    "popt1": popt[1],
+                }
+            )
         except:
             log.warning("The fitting was not successful")
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-        data_fit.add(
-            {
-                "popt0": popt[0],  # C_ij
-                "popt1": popt[1],
-            }
-        )
     return data_fit
 
 
 def res_spectroscopy_flux_matrix(folder, fluxlines):
-    """Calculation of the resonator flux matrix, Mf.
+    """
+    Calculation of the resonator flux matrix, Mf.
        curr = Mf*freq + offset_c.
        Mf = Mc^-1, offset_c = -Mc^-1 * offset_f
        freq = Mc*curr + offset_f
-        Args:
+
+    Args:
         folder (str): Folder where the data files with the experimental and fit data are.
         fluxlines (list): ids of the current line used for the experiment.
 
     Returns:
         data (Data): Data file with len(fluxlines)+1 columns that contains the flux matrix (Mf) and
                      offset (offset_c) in the last column.
 
@@ -950,31 +965,33 @@
 
         try:
             popt, pcov = curve_fit(
                 exp, times.values, voltages.values, p0=pguess, maxfev=2000000
             )
             t2 = abs(1 / popt[2])
 
+            data_fit.add(
+                {
+                    "popt0": popt[0],
+                    "popt1": popt[1],
+                    "popt2": popt[2],
+                    labels[0]: t2,
+                    "qubit": qubit,
+                }
+            )
         except:
             log.warning("spin_echo_fit: the fitting was not succesful")
-            return data_fit
+            data_fit.add(
+                {key: 0 if key != "qubit" else qubit for key in data_fit.df.columns}
+            )
 
-    data_fit.add(
-        {
-            "popt0": popt[0],
-            "popt1": popt[1],
-            "popt2": popt[2],
-            labels[0]: t2,
-            "qubit": qubit,
-        }
-    )
     return data_fit
 
 
-def calibrate_qubit_states_fit(data, x, y, nshots, qubits):
+def calibrate_qubit_states_fit(data, x, y, nshots, qubits, degree=True):
     parameters = Data(
         name=f"parameters",
         quantities={
             "rotation_angle",  # in degrees
             "threshold",
             "fidelity",
             "assignment_fidelity",
@@ -1005,80 +1022,176 @@
             .pint.magnitude
             + 1.0j
             * qubit_data[qubit_data["state"] == 1][q_keys[0]]
             .pint.to(q_keys[1])
             .pint.magnitude
         )
 
-    for qubit in qubits:
-        qubit_data = data.df[data.df["qubit"] == qubit]
-
-        iq_state0 = (
-            qubit_data[qubit_data["state"] == 0][i_keys[0]]
-            .pint.to(i_keys[1])
-            .pint.magnitude
-            + 1.0j
-            * qubit_data[qubit_data["state"] == 0][q_keys[0]]
-            .pint.to(q_keys[1])
-            .pint.magnitude
-        )
-        iq_state1 = (
-            qubit_data[qubit_data["state"] == 1][i_keys[0]]
-            .pint.to(i_keys[1])
-            .pint.magnitude
-            + 1.0j
-            * qubit_data[qubit_data["state"] == 1][q_keys[0]]
-            .pint.to(q_keys[1])
-            .pint.magnitude
-        )
-
         iq_state1 = np.array(iq_state1)
         iq_state0 = np.array(iq_state0)
 
         iq_mean_state1 = np.mean(iq_state1)
         iq_mean_state0 = np.mean(iq_state0)
-        origin = iq_mean_state0
 
-        iq_state0_translated = iq_state0 - origin
-        iq_state1_translated = iq_state1 - origin
-        rotation_angle = np.angle(np.mean(iq_state1_translated))
+        rotation_angle = np.angle(iq_mean_state1 - iq_mean_state0)
 
         iq_state1_rotated = iq_state1 * np.exp(-1j * rotation_angle)
         iq_state0_rotated = iq_state0 * np.exp(-1j * rotation_angle)
 
         real_values_state1 = iq_state1_rotated.real
         real_values_state0 = iq_state0_rotated.real
 
         real_values_combined = np.concatenate((real_values_state1, real_values_state0))
         real_values_combined.sort()
 
-        cum_distribution_state1 = [
-            sum(map(lambda x: x.real >= real_value, real_values_state1))
-            for real_value in real_values_combined
-        ]
-        cum_distribution_state0 = [
-            sum(map(lambda x: x.real >= real_value, real_values_state0))
-            for real_value in real_values_combined
-        ]
+        cum_distribution_state1 = cumulative(real_values_combined, real_values_state1)
+        cum_distribution_state0 = cumulative(real_values_combined, real_values_state0)
 
         cum_distribution_diff = np.abs(
             np.array(cum_distribution_state1) - np.array(cum_distribution_state0)
         )
         argmax = np.argmax(cum_distribution_diff)
         threshold = real_values_combined[argmax]
         errors_state1 = nshots - cum_distribution_state1[argmax]
         errors_state0 = cum_distribution_state0[argmax]
         fidelity = cum_distribution_diff[argmax] / nshots
         assignment_fidelity = 1 - (errors_state1 + errors_state0) / nshots / 2
         # assignment_fidelity = 1/2 + (cum_distribution_state1[argmax] - cum_distribution_state0[argmax])/nshots/2
+        if degree:
+            rotation_angle = (-rotation_angle * 360 / (2 * np.pi)) % 360
 
         results = {
-            "rotation_angle": (-rotation_angle * 360 / (2 * np.pi)) % 360,  # in degrees
+            "rotation_angle": rotation_angle,
             "threshold": threshold,
             "fidelity": fidelity,
             "assignment_fidelity": assignment_fidelity,
             "average_state0": iq_mean_state0,
             "average_state1": iq_mean_state1,
             "qubit": qubit,
         }
         parameters.add(results)
     return parameters
+
+
+def ro_optimization_fit(data, *labels, debug=False):
+    """
+    Fit the fidelities from parameters swept as labels, and extract rotation angle and threshold
+
+    Args:
+        data (Data): data to fit
+        labels (str): variable used in the routine with format "variable_name"
+
+    Returns:
+        Data: data with the fit results
+    """
+    quantities = [
+        *labels,
+        "rotation_angle",
+        "threshold",
+        "fidelity",
+        "assignment_fidelity",
+        "average_state0",
+        "average_state1",
+    ]
+    data_fit = Data(
+        name="fit",
+        quantities=quantities,
+    )
+
+    # Create a ndarray for i and q shots for all labels
+    # shape=(i + j*q, qubit, state, label1, label2, ...)
+
+    shape = (*[len(data.df[label].unique()) for label in labels],)
+    nb_shots = len(data.df["iteration"].unique())
+
+    iq_complex = data.df["i"].pint.magnitude.to_numpy().reshape(shape) + 1j * data.df[
+        "q"
+    ].pint.magnitude.to_numpy().reshape(shape)
+
+    # Move state to 0, and iteration to -1
+    labels = list(labels)
+    iq_complex = np.moveaxis(
+        iq_complex, [labels.index("state"), labels.index("iteration")], [0, -1]
+    )
+    labels.remove("state")
+    labels.remove("iteration")
+    labels = ["state"] + labels + ["iteration"]
+
+    # Take the mean ground state
+    mean_gnd_state = np.mean(iq_complex[0, ...], axis=-1, keepdims=True)
+    mean_exc_state = np.mean(iq_complex[1, ...], axis=-1, keepdims=True)
+    angle = np.angle(mean_exc_state - mean_gnd_state)
+
+    # Rotate the data
+    iq_complex = iq_complex * np.exp(-1j * angle)
+
+    # Take the cumulative distribution of the real part of the data
+    iq_complex_sorted = np.sort(iq_complex.real, axis=-1)
+
+    def cum_dist(complex_row):
+        state0 = complex_row.real
+        state1 = complex_row.imag
+        combined = np.sort(np.concatenate((state0, state1)))
+
+        # Compute the indices where elements in state0 and state1 would be inserted in combined
+        idx_state0 = np.searchsorted(combined, state0, side="left")
+        idx_state1 = np.searchsorted(combined, state1, side="left")
+
+        # Create a combined histogram for state0 and state1
+        hist_combined = np.bincount(
+            idx_state0, minlength=len(combined)
+        ) + 1j * np.bincount(idx_state1, minlength=len(combined))
+
+        return hist_combined.cumsum()
+
+    cum_dist = (
+        np.apply_along_axis(
+            func1d=cum_dist,
+            axis=-1,
+            arr=iq_complex_sorted[0, ...] + 1j * iq_complex_sorted[1, ...],
+        )
+        / nb_shots
+    )
+
+    # Find the threshold for which the difference between the cumulative distribution of the two states is maximum
+    argmax = np.argmax(np.abs(cum_dist.real - cum_dist.imag), axis=-1, keepdims=True)
+
+    # Use np.take_along_axis to get the correct indices for the threshold calculation
+    threshold = np.take_along_axis(
+        np.concatenate((iq_complex_sorted[0, ...], iq_complex_sorted[1, ...]), axis=-1),
+        argmax,
+        axis=-1,
+    )
+
+    # Calculate the fidelity
+    fidelity = np.take_along_axis(
+        np.abs(cum_dist.real - cum_dist.imag), argmax, axis=-1
+    )
+    assignment_fidelity = (
+        1
+        - (
+            1
+            - np.take_along_axis(cum_dist.real, argmax, axis=-1)
+            + np.take_along_axis(cum_dist.imag, argmax, axis=-1)
+        )
+        / 2
+    )
+
+    # Add all the results to the data with labels as subnet without "state", "iteration"
+    data_fit.df = (
+        data.df.drop_duplicates(
+            subset=[i for i in labels if i not in ["state", "iteration"]]
+        )
+        .reset_index(drop=True)
+        .apply(pint_to_float)
+    )
+    data_fit.df["rotation_angle"] = angle.flatten()
+    data_fit.df["threshold"] = threshold.flatten()
+    data_fit.df["fidelity"] = fidelity.flatten()
+    data_fit.df["assignment_fidelity"] = assignment_fidelity.flatten()
+    data_fit.df["average_state0"] = mean_gnd_state.flatten()
+    data_fit.df["average_state1"] = mean_exc_state.flatten()
+
+    if debug:
+        return data_fit, cum_dist, iq_complex
+    else:
+        return data_fit
```

### Comparing `qibocal-0.0.1/src/qibocal/fitting/utils.py` & `qibocal-0.0.2/src/qibocal/fitting/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 
 import numpy as np
+import pandas as pd
+import pint
 from scipy.special import mathieu_a, mathieu_b
 
 
 def lorenzian(frequency, amplitude, center, sigma, offset):
     # http://openafox.com/science/peak-function-derivations.html
     return (amplitude / np.pi) * (
         sigma / ((frequency - center) ** 2 + sigma**2)
@@ -124,7 +126,33 @@
     # Charging energy E_C                                  : p[5]
     # Josephson energy E_J                                 : p[6]
     # Effective offset charge ng                           : p[7]
     G = G_f_d(x, p2, p3, p4)
     f_q = freq_q_mathieu(x, p2, p3, p4, p5, p6, p7)
     f_r = p0 + p1**2 * np.sqrt(G) / (p0 - f_q)
     return f_r
+
+
+def pint_to_float(x):
+    if isinstance(x, pd.Series):
+        return x.apply(pint_to_float)
+    elif isinstance(x, pint.Quantity):
+        return x.to(x.units).magnitude
+    else:
+        return x
+
+
+def cumulative(input_data, points):
+    r"""Evaluates in `input_data` the cumulative distribution
+    function of `points`.
+    WARNING: `input_data` and `points` should be sorted data.
+    """
+    input_data_sort = np.sort(input_data)
+    points_sort = np.sort(points)
+
+    prob = []
+    app = 0
+    for val in input_data_sort:
+        app += np.max(np.searchsorted(points_sort[app::], val), 0)
+        prob.append(app)
+
+    return np.array(prob)
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/allXY.py` & `qibocal-0.0.2/src/qibocal/plots/allXY.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import cos
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 # allXY rotations
 gatelist = [
     ["I", "I"],
     ["RX(pi)", "RX(pi)"],
     ["RY(pi)", "RY(pi)"],
     ["RX(pi)", "RY(pi)"],
@@ -28,32 +28,33 @@
     ["RX(pi)", "I"],
     ["RY(pi)", "I"],
     ["RX(pi/2)", "RX(pi/2)"],
     ["RY(pi/2)", "RY(pi/2)"],
 ]
 
 
+# allXY
 def allXY(folder, routine, qubit, format):
     figures = []
-    fitting_report = "No fitting data: -<br>No fitting data: -<br><br>"
+    fitting_report = "No fitting data"
 
     fig = make_subplots(
         rows=1,
         cols=1,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
         subplot_titles=(f"allXY",),
     )
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = Data.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = Data(
                 name="data",
                 quantities={"probability", "gateNumber", "qubit", "iteration"},
             )
         iterations = data.df["iteration"].unique()
@@ -132,30 +133,30 @@
 
     return figures, fitting_report
 
 
 # allXY
 def allXY_drag_pulse_tuning(folder, routine, qubit, format):
     figures = []
-    fitting_report = "No fitting data: -<br>No fitting data: -<br><br>"
+    fitting_report = "No fitting data"
 
     fig = make_subplots(
         rows=1,
         cols=1,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
         subplot_titles=(f"allXY",),
     )
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = Data.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = Data(
                 quantities={
                     "probability",
                     "gateNumber",
                     "beta_param",
@@ -229,111 +230,108 @@
 
     return figures, fitting_report
 
 
 # beta param tuning
 def drag_pulse_tuning(folder, routine, qubit, format):
     figures = []
-    fitting_report = "No fitting data: -<br>No fitting data: -<br><br>"
+    fitting_report = ""
 
     fig = make_subplots(
         rows=1,
         cols=1,
         horizontal_spacing=0.01,
         vertical_spacing=0.01,
     )
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
-    fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name="data",
                 quantities={"beta_param": "dimensionless"},
                 options=["qubit", "iteration"],
             )
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, "fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data()
 
         iterations = data.df["iteration"].unique()
-        beta_params = data.df["beta_param"].pint.magnitude.unique()
+        beta_params = data.df["beta_param"].unique()
 
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["beta_param"].pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["beta_param"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     mode="markers",
                     opacity=0.3,
                     name=f"q{qubit}/r{report_n}: Probability",
                     showlegend=not bool(iteration),
                     legendgroup="group1",
                 ),
                 row=1,
                 col=1,
             )
 
         fig.add_trace(
             go.Scatter(
                 x=beta_params,
-                y=data.df.groupby("beta_param", as_index=False)
-                .mean()["MSR"]  # pylint: disable=E1101
-                .pint.to("uV")
-                .pint.magnitude,
+                y=data.df.groupby("beta_param", as_index=False).mean()["MSR"]
+                * 1e6,  # pylint: disable=E1101
                 name=f"q{qubit}/r{report_n}: Average MSR",
                 marker_color=get_color(report_n),
                 mode="markers",
             ),
             row=1,
             col=1,
         )
 
         # add fitting traces
 
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             beta_range = np.linspace(
-                min(data.get_values("beta_param", "dimensionless")),
-                max(data.get_values("beta_param", "dimensionless")),
+                min(data.df["beta_param"]),
+                max(data.df["beta_param"]),
                 20,
             )
 
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
+
             fig.add_trace(
                 go.Scatter(
                     x=beta_range,
                     y=cos(
                         beta_range,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
                     ),
                     name=f"q{qubit}/r{report_n}: Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
             )
             fitting_report = fitting_report + (
-                f"q{qubit}/r{report_n} optimal_beta_param: {params['optimal_beta_param']:.4f}<br><br>"
+                f"q{qubit}/r{report_n} | optimal_beta_param: {params['optimal_beta_param']:.4f}<br><br>"
             )
-
             report_n += 1
 
     fig.update_layout(
         showlegend=True,
         uirevision="0",  # ``uirevision`` allows zooming while live plotting
         xaxis_title="Beta parameter",
         yaxis_title="MSR[uV] [Rx(pi/2) - Ry(pi)] - [Ry(pi/2) - Rx(pi)]",
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/calibrate_qubit_states.py` & `qibocal-0.0.2/src/qibocal/plots/calibrate_qubit_states.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
-from qibocal.plots.utils import get_color_state0, get_color_state1, get_data_subfolders
+from qibocal.plots.utils import (
+    get_color_state0,
+    get_color_state1,
+    get_data_subfolders,
+    load_data,
+)
 
 
 # For calibrate qubit states
 def qubit_states(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
@@ -21,98 +26,102 @@
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     max_x, max_y, min_x, min_y = 0, 0, 0, 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(options=["qubit", "iteration", "state"])
 
         try:
-            parameters = Data.load_data(
-                folder, subfolder, routine, format, "parameters"
-            )
+            parameters = load_data(folder, subfolder, routine, format, "parameters")
             parameters.df = parameters.df[parameters.df["qubit"] == qubit]
 
-            average_state0 = complex(parameters.get_values("average_state0")[0])
-            average_state1 = complex(parameters.get_values("average_state1")[0])
-            rotation_angle = parameters.get_values("rotation_angle")[0]
-            threshold = parameters.get_values("threshold")[0]
-            fidelity = parameters.get_values("fidelity")[0]
-            assignment_fidelity = parameters.get_values("assignment_fidelity")[0]
+            average_state0 = complex(parameters.df.iloc[0]["average_state0"])
+            average_state1 = complex(
+                parameters.df.iloc[0]["average_state1"]  # pylint: disable=E1101
+            )
+            rotation_angle = parameters.df.iloc[0][  # pylint: disable=E1101
+                "rotation_angle"
+            ]  # pylint: disable=E1101
+            threshold = parameters.df.iloc[0]["threshold"]  # pylint: disable=E1101
+            fidelity = parameters.df.iloc[0]["fidelity"]  # pylint: disable=E1101
+            assignment_fidelity = parameters.df.iloc[0][
+                "assignment_fidelity"
+            ]  # pylint: disable=E1101
 
         except:
             parameters = Data(
                 name=f"parameters",
                 quantities=[
-                    "rotation_angle",  # in degrees
+                    "rotation_angle",  # in rad
                     "threshold",
                     "fidelity",
                     "assignment_fidelity",
                     "average_state0",
                     "average_state1",
                     "qubit",
                 ],
             )
 
         state0_data = data.df[data.df["state"] == 0]
         state1_data = data.df[data.df["state"] == 1]
 
         fig.add_trace(
             go.Scatter(
-                x=state0_data["i"].pint.to("V").pint.magnitude,
-                y=state0_data["q"].pint.to("V").pint.magnitude,
+                x=state0_data["i"],
+                y=state0_data["q"],
                 name=f"q{qubit}/r{report_n}: state 0",
                 legendgroup=f"q{qubit}/r{report_n}: state 0",
                 mode="markers",
                 showlegend=False,
                 opacity=0.7,
                 marker=dict(size=3, color=get_color_state0(report_n)),
             ),
             row=1,
             col=1,
         )
 
         fig.add_trace(
             go.Scatter(
-                x=state1_data["i"].pint.to("V").pint.magnitude,
-                y=state1_data["q"].pint.to("V").pint.magnitude,
+                x=state1_data["i"],
+                y=state1_data["q"],
                 name=f"q{qubit}/r{report_n}: state 1",
                 legendgroup=f"q{qubit}/r{report_n}: state 1",
                 mode="markers",
                 showlegend=False,
                 opacity=0.7,
                 marker=dict(size=3, color=get_color_state1(report_n)),
             ),
             row=1,
             col=1,
         )
 
         max_x = max(
             max_x,
-            state0_data["i"].pint.to("V").pint.magnitude.max(),
-            state1_data["i"].pint.to("V").pint.magnitude.max(),
+            state0_data["i"].max(),
+            state1_data["i"].max(),
         )
         max_y = max(
             max_y,
-            state0_data["q"].pint.to("V").pint.magnitude.max(),
-            state1_data["q"].pint.to("V").pint.magnitude.max(),
+            state0_data["q"].max(),
+            state1_data["q"].max(),
         )
         min_x = min(
             min_x,
-            state0_data["i"].pint.to("V").pint.magnitude.min(),
-            state1_data["i"].pint.to("V").pint.magnitude.min(),
+            state0_data["i"].min(),
+            state1_data["i"].min(),
         )
         min_y = min(
             min_y,
-            state0_data["q"].pint.to("V").pint.magnitude.min(),
-            state1_data["q"].pint.to("V").pint.magnitude.min(),
+            state0_data["q"].min(),
+            state1_data["q"].min(),
         )
 
         fig.add_trace(
             go.Scatter(
                 x=[average_state0.real],
                 y=[average_state0.imag],
                 name=f"q{qubit}/r{report_n}: state 0",
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/flipping.py` & `qibocal-0.0.2/src/qibocal/plots/flipping.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import flipping
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # Flipping
 def flips_msr(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
@@ -21,22 +21,22 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 quantities={"flips": "dimensionless"}, options=["qubit", "iteration"]
             )
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
@@ -44,73 +44,73 @@
                     "popt4",
                     "label1",
                     "label2",
                     "qubit",
                 ]
             )
 
+        data.df = data.df.drop(columns=["i", "q", "phase", "qubit"])
         iterations = data.df["iteration"].unique()
-        flips = data.df["flips"].pint.magnitude.unique()
+        flips = data.df["flips"].unique()
 
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["flips"].pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["flips"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
 
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
                     x=flips,
-                    y=data.df.groupby("flips")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    y=data.df.groupby("flips")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             flips_range = np.linspace(
-                min(data.get_values("flips", "dimensionless")),
-                max(data.get_values("flips", "dimensionless")),
+                min(data.df["flips"]),
+                max(data.df["flips"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
             fig.add_trace(
                 go.Scatter(
                     x=flips_range,
                     y=flipping(
                         flips_range,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
                     ),
                     name=f"q{qubit}/r{report_n}: Fit MSR",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/rabi.py` & `qibocal-0.0.2/src/qibocal/plots/rabi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import rabi
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # Rabi oscillations pulse length
 def time_msr_phase(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
@@ -24,21 +24,21 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, "data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(quantities={"time": "ns"}, options=["qubit", "iteration"])
 
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
@@ -47,98 +47,96 @@
                     "label1",
                     "label2",
                     "qubit",
                 ]
             )
 
         iterations = data.df["iteration"].unique()
-        times = data.df["time"].pint.to("ns").pint.magnitude.unique()
+        times = data.df["time"].unique()
+        data.df = data.df.drop(columns=["i", "q", "qubit"])
+
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["time"].pint.to("ns").pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["time"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["time"].pint.to("ns").pint.magnitude,
-                    y=iteration_data["phase"].pint.to("rad").pint.magnitude,
+                    x=iteration_data["time"],
+                    y=iteration_data["phase"],
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=2,
             )
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
                     x=times,
-                    y=data.df.groupby("time")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    y=data.df.groupby("time")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
             fig.add_trace(
                 go.Scatter(
                     x=times,
-                    y=data.df.groupby("time")["phase"]  # pylint: disable=E1101
-                    .mean()
-                    .pint.to("rad")
-                    .pint.magnitude,
+                    y=data.df.groupby("time")["phase"].mean(),  # pylint: disable=E1101
                     marker_color=get_color(report_n),
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=2,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             timerange = np.linspace(
-                min(data.get_values("time", "ns")),
-                max(data.get_values("time", "ns")),
+                min(data.df["time"]),
+                max(data.df["time"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
             fig.add_trace(
                 go.Scatter(
                     x=timerange,
                     y=rabi(
                         timerange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
-                        data_fit.get_values("popt4"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
+                        float(data_fit.df["popt4"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
@@ -188,23 +186,23 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 quantities={"gain", "dimensionless"}, options=["qubit", "iteration"]
             )
 
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
@@ -213,98 +211,97 @@
                     "label1",
                     "label2",
                     "qubit",
                 ]
             )
 
         iterations = data.df["iteration"].unique()
-        gains = data.df["gain"].pint.to("dimensionless").pint.magnitude.unique()
+        gains = data.df["gain"].unique()
+        data.df = data.df.drop(columns=["i", "q", "qubit"])
+
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["gain"].pint.to("dimensionless").pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["gain"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["gain"].pint.to("dimensionless").pint.magnitude,
-                    y=iteration_data["phase"].pint.to("rad").pint.magnitude,
+                    x=iteration_data["gain"],
+                    y=iteration_data["phase"],
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=2,
             )
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
                     x=gains,
-                    y=data.df.groupby("gain")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    y=data.df.groupby("gain")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
+
             fig.add_trace(
                 go.Scatter(
                     x=gains,
-                    y=data.df.groupby("gain")["phase"]  # pylint: disable=E1101
-                    .mean()
-                    .pint.to("rad")
-                    .pint.magnitude,
+                    y=data.df.groupby("gain")["phase"].mean(),  # pylint: disable=E1101
                     marker_color=get_color(report_n),
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=2,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             gainrange = np.linspace(
-                min(data.get_values("gain", "dimensionless")),
-                max(data.get_values("gain", "dimensionless")),
+                min(data.df["gain"]),
+                max(data.df["gain"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
             fig.add_trace(
                 go.Scatter(
                     x=gainrange,
                     y=rabi(
                         gainrange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
-                        data_fit.get_values("popt4"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
+                        float(data_fit.df["popt4"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
@@ -353,23 +350,23 @@
     )
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 quantities={"amplitude", "dimensionless"},
                 options=["qubit", "iteration"],
             )
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
@@ -378,104 +375,101 @@
                     "label1",
                     "label2",
                     "qubit",
                 ]
             )
 
         iterations = data.df["iteration"].unique()
-        amplitudes = (
-            data.df["amplitude"].pint.to("dimensionless").pint.magnitude.unique()
-        )
+        amplitudes = data.df["amplitude"].unique()
+        data.df = data.df.drop(columns=["i", "q", "qubit"])
+
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["amplitude"]
-                    .pint.to("dimensionless")
-                    .pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["amplitude"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["amplitude"]
-                    .pint.to("dimensionless")
-                    .pint.magnitude,
-                    y=iteration_data["phase"].pint.to("rad").pint.magnitude,
+                    x=iteration_data["amplitude"],
+                    y=iteration_data["phase"],
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=2,
             )
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
                     x=amplitudes,
-                    y=data.df.groupby("amplitude")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    y=data.df.groupby("amplitude")[  # pylint: disable=E1101
+                        "MSR"
+                    ].mean()
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
+
             fig.add_trace(
                 go.Scatter(
                     x=amplitudes,
-                    y=data.df.groupby("amplitude")["phase"]  # pylint: disable=E1101
-                    .mean()
-                    .pint.to("rad")
-                    .pint.magnitude,
+                    y=data.df.groupby("amplitude")[  # pylint: disable=E1101
+                        "phase"
+                    ].mean(),
                     marker_color=get_color(report_n),
                     showlegend=False,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=2,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             amplituderange = np.linspace(
-                min(data.get_values("amplitude", "dimensionless")),
-                max(data.get_values("amplitude", "dimensionless")),
+                min(data.df["amplitude"]),
+                max(data.df["amplitude"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
             fig.add_trace(
                 go.Scatter(
                     x=amplituderange,
                     y=rabi(
                         amplituderange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
-                        data_fit.get_values("popt4"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
+                        float(data_fit.df["popt4"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color="rgb(255, 130, 67)",
                 ),
                 row=1,
                 col=1,
@@ -525,51 +519,51 @@
             "phase (rad)",
         ),
     )
 
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, f"data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"duration": "ns", "gain": "dimensionless"},
                 options=["qubit", "iteration"],
             )
 
         iterations = data.df["iteration"].unique()
-        durations = data.df["duration"].pint.to("ns").pint.magnitude.unique()
-        gains = data.df["gain"].pint.to("dimensionless").pint.magnitude.unique()
-        averaged_data = (
-            data.df.drop(columns=["qubit", "iteration"])
-            .groupby(["duration", "gain"], as_index=False)
-            .mean()
-        )
+        durations = data.df["duration"].unique()
+        gains = data.df["gain"].unique()
+
+        averaged_data = data.df.drop(columns=["i", "q", "qubit", "iteration"])
+        averaged_data = data.df.groupby(  # pylint: disable=E1101
+            ["duration", "gain"], as_index=False
+        ).mean()
 
         fig.add_trace(
             go.Heatmap(
-                x=averaged_data["duration"].pint.to("ns").pint.magnitude,
-                y=averaged_data["gain"].pint.to("dimensionless").pint.magnitude,
-                z=averaged_data["MSR"].pint.to("V").pint.magnitude,
+                x=averaged_data["duration"],
+                y=averaged_data["gain"],
+                z=averaged_data["MSR"] * 1e6,
                 colorbar_x=0.46,
             ),
             row=1 + report_n,
             col=1,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Duration (ns)", row=1 + report_n, col=1
         )
         fig.update_yaxes(title_text="Gain (dimensionless)", row=1 + report_n, col=1)
         fig.add_trace(
             go.Heatmap(
-                x=averaged_data["duration"].pint.to("ns").pint.magnitude,
-                y=averaged_data["gain"].pint.to("dimensionless").pint.magnitude,
-                z=averaged_data["phase"].pint.to("rad").pint.magnitude,
+                x=averaged_data["duration"],
+                y=averaged_data["gain"],
+                z=averaged_data["phase"],
                 colorbar_x=1.01,
             ),
             row=1 + report_n,
             col=2,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Duration (ns)", row=1 + report_n, col=2
@@ -606,55 +600,54 @@
             "phase (rad)",
         ),
     )
 
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"duration": "ns", "amplitude": "dimensionless"},
                 options=["qubit", "iteration"],
             )
 
         iterations = data.df["iteration"].unique()
-        durations = data.df["duration"].pint.to("ns").pint.magnitude.unique()
-        amplitudes = (
-            data.df["amplitude"].pint.to("dimensionless").pint.magnitude.unique()
-        )
-        averaged_data = (
-            data.df.drop(columns=["qubit", "iteration"])
-            .groupby(["duration", "amplitude"], as_index=False)
-            .mean()
-        )
+        durations = data.df["duration"].unique()
+        amplitudes = data.df["amplitude"].unique()
+
+        averaged_data = data.df.drop(columns=["i", "q", "qubit", "iteration"])
+
+        averaged_data = data.df.groupby(  # pylint: disable=E1101
+            ["duration", "amplitude"], as_index=False
+        ).mean()
 
         fig.add_trace(
             go.Heatmap(
-                x=averaged_data["duration"].pint.to("ns").pint.magnitude,
-                y=averaged_data["amplitude"].pint.to("dimensionless").pint.magnitude,
-                z=averaged_data["MSR"].pint.to("V").pint.magnitude,
+                x=averaged_data["duration"],
+                y=averaged_data["amplitude"],
+                z=averaged_data["MSR"] * 1e6,
                 colorbar_x=0.46,
             ),
             row=1 + report_n,
             col=1,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Duration (ns)", row=1 + report_n, col=1
         )
         fig.update_yaxes(
             title_text="Amplitude (dimensionless)", row=1 + report_n, col=1
         )
         fig.add_trace(
             go.Heatmap(
-                x=averaged_data["duration"].pint.to("ns").pint.magnitude,
-                y=averaged_data["amplitude"].pint.to("dimensionless").pint.magnitude,
-                z=averaged_data["phase"].pint.to("rad").pint.magnitude,
+                x=averaged_data["duration"],
+                y=averaged_data["amplitude"],
+                z=averaged_data["phase"],
                 colorbar_x=1.01,
             ),
             row=1 + report_n,
             col=2,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Duration (ns)", row=1 + report_n, col=2
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/ramsey.py` & `qibocal-0.0.2/src/qibocal/plots/ramsey.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import ramsey
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # Ramsey oscillations
 def time_msr(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
@@ -22,101 +22,101 @@
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
 
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"wait": "ns", "t_max": "ns"},
                 options=["qubit", "iteration"],
             )
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
+                    "T2",
+                    "drive_frequency",
+                    "delta_frequency",
                     "popt0",
                     "popt1",
                     "popt2",
                     "popt3",
                     "popt4",
-                    "label1",
-                    "label2",
-                    "label3",
                     "qubit",
                 ]
             )
 
         iterations = data.df["iteration"].unique()
-        waits = data.df["wait"].pint.to("ns").pint.magnitude.unique()
+        waits = data.df["wait"].unique()
+        data.df = data.df.drop(columns=["i", "q", "phase", "qubit"])
 
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["wait"].pint.to("ns").pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["wait"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
 
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
                     x=waits,
-                    y=data.df.groupby("wait")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    y=data.df.groupby("wait")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             waitrange = np.linspace(
-                min(data.get_values("wait", "ns")),
-                max(data.get_values("wait", "ns")),
+                min(data.df["wait"]),
+                max(data.df["wait"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
 
             fig.add_trace(
                 go.Scatter(
                     x=waitrange,
                     y=ramsey(
                         waitrange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
-                        data_fit.get_values("popt4"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
+                        float(data_fit.df["popt4"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
@@ -124,17 +124,17 @@
 
             fitting_report = (
                 fitting_report
                 + (
                     f"q{qubit}/r{report_n} | delta_frequency: {params['delta_frequency']:,.0f} Hz<br>"
                 )
                 + (
-                    f"q{qubit}/r{report_n} | corrected_qubit_frequency: {params['corrected_qubit_frequency']:,.0f} Hz<br>"
+                    f"q{qubit}/r{report_n} | drive_frequency: {params['drive_frequency']:,.0f} Hz<br>"
                 )
-                + (f"q{qubit}/r{report_n} | t2: {params['t2']:,.0f} ns.<br><br>")
+                + (f"q{qubit}/r{report_n} | T2: {params['T2']:,.0f} ns.<br><br>")
             )
         report_n += 1
 
     fig.update_layout(
         showlegend=True,
         uirevision="0",  # ``uirevision`` allows zooming while live plotting
         xaxis_title="Time (ns)",
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/spectroscopies.py` & `qibocal-0.0.2/src/qibocal/plots/spectroscopies.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,57 +2,46 @@
 
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import freq_r_mathieu, freq_r_transmon, line, lorenzian
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # Resonator and qubit spectroscopies
 def frequency_msr_phase(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
         subplot_titles=(
-            "MSR (V)",
+            "MSR (uV)",
             "phase (rad)",
         ),
     )
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data_fast = DataUnits.load_data(
-                folder, subfolder, routine, format, "fast_sweep_data"
-            )
-            data_fast.df = data_fast.df[data_fast.df["qubit"] == qubit]
-        except:
-            data_fast = DataUnits(
-                quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
-            )
-        try:
-            data_precision = DataUnits.load_data(
-                folder, subfolder, routine, format, f"precision_sweep_data"
-            )
-            data_precision.df = data_precision.df[data_precision.df["qubit"] == qubit]
+            data = load_data(folder, subfolder, routine, format, "data")
+            data.df = data.df[data.df["qubit"] == qubit]
         except:
-            data_precision = DataUnits(
+            data = DataUnits(
                 quantities={"frequency": "Hz"}, options=["qubit", "iteration"]
             )
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
@@ -60,99 +49,100 @@
                     "label1",
                     "label2",
                     "label3",
                     "qubit",
                 ]
             )
 
-        for i, label, data in list(
-            zip((0, 1), ("Fast", "Precision"), (data_fast, data_precision))
-        ):
-            iterations = data.df["iteration"].unique()
-            frequencies = data.df["frequency"].pint.to("Hz").pint.magnitude.unique()
-            if len(iterations) > 1:
-                opacity = 0.3
-            else:
-                opacity = 1
-            for iteration in iterations:
-                iteration_data = data.df[data.df["iteration"] == iteration]
-                fig.add_trace(
-                    go.Scatter(
-                        x=iteration_data["frequency"].pint.to("Hz").pint.magnitude,
-                        y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
-                        marker_color=get_color(2 * report_n + i),
-                        opacity=opacity,
-                        name=f"q{qubit}/r{report_n}: {label}",
-                        showlegend=not bool(iteration),
-                        legendgroup=f"q{qubit}/r{report_n}: {label}",
-                    ),
-                    row=1,
-                    col=1,
-                )
-                fig.add_trace(
-                    go.Scatter(
-                        x=iteration_data["frequency"].pint.to("Hz").pint.magnitude,
-                        y=iteration_data["phase"].pint.to("rad").pint.magnitude,
-                        marker_color=get_color(2 * report_n + i),
-                        opacity=opacity,
-                        showlegend=False,
-                        legendgroup=f"q{qubit}/r{report_n}: {label}",
-                    ),
-                    row=1,
-                    col=2,
-                )
-            if len(iterations) > 1:
-                fig.add_trace(
-                    go.Scatter(
-                        x=frequencies,
-                        y=data.df.groupby("frequency")["MSR"]
-                        .mean()
-                        .pint.to("uV")
-                        .pint.magnitude,
-                        marker_color=get_color(2 * report_n + i),
-                        name=f"q{qubit}/r{report_n}: {label} Average",
-                        showlegend=True,
-                        legendgroup=f"q{qubit}/r{report_n}: {label} Average",
-                    ),
-                    row=1,
-                    col=1,
-                )
-                fig.add_trace(
-                    go.Scatter(
-                        x=frequencies,
-                        y=data.df.groupby("frequency")["phase"]
-                        .mean()
-                        .pint.to("rad")
-                        .pint.magnitude,
-                        marker_color=get_color(2 * report_n + i),
-                        showlegend=False,
-                        legendgroup=f"q{qubit}/r{report_n}: {label} Average",
-                    ),
-                    row=1,
-                    col=2,
-                )
+        data.df = data.df.drop(columns=["i", "q", "qubit"])
+        iterations = data.df["iteration"].unique()
+        frequencies = data.df["frequency"].unique() * 1e-9
+
+        if len(iterations) > 1:
+            opacity = 0.3
+        else:
+            opacity = 1
+        for iteration in iterations:
+            iteration_data = data.df[data.df["iteration"] == iteration]
+            fig.add_trace(
+                go.Scatter(
+                    x=iteration_data["frequency"] * 1e-9,
+                    y=iteration_data["MSR"] * 1e6,
+                    marker_color=get_color(2 * report_n),
+                    opacity=opacity,
+                    name=f"q{qubit}/r{report_n}: Data",
+                    showlegend=not bool(iteration),
+                    legendgroup=f"q{qubit}/r{report_n}: Data",
+                ),
+                row=1,
+                col=1,
+            )
+            fig.add_trace(
+                go.Scatter(
+                    x=iteration_data["frequency"] * 1e-9,
+                    y=iteration_data["phase"],
+                    marker_color=get_color(2 * report_n),
+                    opacity=opacity,
+                    showlegend=False,
+                    legendgroup=f"q{qubit}/r{report_n}: Data",
+                ),
+                row=1,
+                col=2,
+            )
+        if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
+            fig.add_trace(
+                go.Scatter(
+                    x=frequencies,
+                    y=data.df.groupby("frequency")[  # pylint: disable=E1101
+                        "MSR"
+                    ].mean()
+                    * 1e6,
+                    marker_color=get_color(2 * report_n),
+                    name=f"q{qubit}/r{report_n}: Average",
+                    showlegend=True,
+                    legendgroup=f"q{qubit}/r{report_n}: Average",
+                ),
+                row=1,
+                col=1,
+            )
+
+            fig.add_trace(
+                go.Scatter(
+                    x=frequencies,
+                    y=data.df.groupby("frequency")[  # pylint: disable=E1101
+                        "phase"
+                    ].mean(),
+                    marker_color=get_color(2 * report_n),
+                    showlegend=False,
+                    legendgroup=f"q{qubit}/r{report_n}: Average",
+                ),
+                row=1,
+                col=2,
+            )
 
-        if len(data_fast) > 0 and (qubit in data_fit.df["qubit"].values):
+        if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             freqrange = np.linspace(
-                min(data_fast.get_values("frequency", "Hz")),
-                max(data_fast.get_values("frequency", "Hz")),
-                2 * len(data_fast),
+                min(frequencies),
+                max(frequencies),
+                2 * len(frequencies),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
+
             fig.add_trace(
                 go.Scatter(
                     x=freqrange,
                     y=lorenzian(
                         freqrange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
-                        data_fit.get_values("popt3"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
+                        float(data_fit.df["popt3"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
@@ -202,69 +192,157 @@
             "phase (rad)",
         ),
     )
 
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"frequency": "Hz", "attenuation": "dB"},
                 options=["qubit", "iteration"],
             )
 
         iterations = data.df["iteration"].unique()
+        frequencies = data.df["frequency"].unique()
+        attenuations = data.df["attenuation"].unique()
+        averaged_data = (
+            data.df.drop(columns=["i", "q", "qubit", "iteration"])
+            .groupby(["frequency", "attenuation"], as_index=False)
+            .mean()
+        )
+
+        def norm(x_mags):
+            return (x_mags - np.min(x_mags)) / (np.max(x_mags) - np.min(x_mags))
+
+        normalised_data = averaged_data.groupby(["attenuation"], as_index=False)[
+            ["MSR"]
+        ].transform(norm)
+
+        fig.add_trace(
+            go.Heatmap(
+                x=averaged_data["frequency"],
+                y=averaged_data["attenuation"],
+                z=normalised_data["MSR"],
+                colorbar_x=0.46,
+            ),
+            row=1 + report_n,
+            col=1,
+        )
+        fig.update_xaxes(
+            title_text=f"q{qubit}/r{report_n}: Frequency (Hz)", row=1 + report_n, col=1
+        )
+        fig.update_yaxes(title_text="Attenuation (dB)", row=1 + report_n, col=1)
+        fig.add_trace(
+            go.Heatmap(
+                x=averaged_data["frequency"],
+                y=averaged_data["attenuation"],
+                z=averaged_data["phase"],
+                colorbar_x=1.01,
+            ),
+            row=1 + report_n,
+            col=2,
+        )
+        fig.update_xaxes(
+            title_text=f"q{qubit}/r{report_n}: Frequency (Hz)", row=1 + report_n, col=2
+        )
+        fig.update_yaxes(title_text="Attenuation (dB)", row=1 + report_n, col=2)
+        fig.update_layout(
+            showlegend=False,
+            uirevision="0",  # ``uirevision`` allows zooming while live plotting
+        )
+        report_n += 1
+    if report_n > 1:
+        fig.update_traces(showscale=False)
+
+    figures.append(fig)
+
+    return figures, fitting_report
+
+
+# Punchout
+def frequency_amplitude_msr_phase(folder, routine, qubit, format):
+    figures = []
+    fitting_report = "No fitting data"
+    # iterate over multiple data folders
+    subfolders = get_data_subfolders(folder)
+
+    fig = make_subplots(
+        rows=len(subfolders),
+        cols=2,
+        horizontal_spacing=0.1,
+        vertical_spacing=0.2,
+        subplot_titles=(
+            "Normalised MSR",
+            "phase (rad)",
+        ),
+    )
+
+    report_n = 0
+    for subfolder in subfolders:
+        try:
+            data = DataUnits.load_data(folder, subfolder, routine, format, "data")
+            data.df = data.df[data.df["qubit"] == qubit]
+        except:
+            data = DataUnits(
+                name=f"data",
+                quantities={"frequency": "Hz", "amplitude": "dimensionless"},
+                options=["qubit", "iteration"],
+            )
+
+        iterations = data.df["iteration"].unique()
         frequencies = data.df["frequency"].pint.to("Hz").pint.magnitude.unique()
-        attenuations = data.df["attenuation"].pint.to("dB").pint.magnitude.unique()
+        amplitudes = (
+            data.df["amplitude"].pint.to("dimensionless").pint.magnitude.unique()
+        )
         averaged_data = (
             data.df.drop(columns=["qubit", "iteration"])
-            .groupby(["frequency", "attenuation"], as_index=False)
+            .groupby(["frequency", "amplitude"], as_index=False)
             .mean()
         )
 
         def norm(x):
             x_mags = x.pint.to("V").pint.magnitude
             return (x_mags - np.min(x_mags)) / (np.max(x_mags) - np.min(x_mags))
 
-        normalised_data = averaged_data.groupby(["attenuation"], as_index=False)[
+        normalised_data = averaged_data.groupby(["amplitude"], as_index=False)[
             ["MSR"]
         ].transform(norm)
 
         fig.add_trace(
             go.Heatmap(
                 x=averaged_data["frequency"].pint.to("Hz").pint.magnitude,
-                y=averaged_data["attenuation"].pint.to("dB").pint.magnitude,
+                y=averaged_data["amplitude"].pint.to("dimensionless").pint.magnitude,
                 z=normalised_data["MSR"],
-                # z=averaged_data["MSR"].pint.to("V").pint.magnitude,
                 colorbar_x=0.46,
             ),
             row=1 + report_n,
             col=1,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Frequency (Hz)", row=1 + report_n, col=1
         )
-        fig.update_yaxes(title_text="Attenuation (dB)", row=1 + report_n, col=1)
+        fig.update_yaxes(title_text="Amplitude", row=1 + report_n, col=1)
         fig.add_trace(
             go.Heatmap(
                 x=averaged_data["frequency"].pint.to("Hz").pint.magnitude,
-                y=averaged_data["attenuation"].pint.to("dB").pint.magnitude,
+                y=averaged_data["amplitude"].pint.to("dimensionless").pint.magnitude,
                 z=averaged_data["phase"].pint.to("rad").pint.magnitude,
                 colorbar_x=1.01,
             ),
             row=1 + report_n,
             col=2,
         )
         fig.update_xaxes(
             title_text=f"q{qubit}/r{report_n}: Frequency (Hz)", row=1 + report_n, col=2
         )
-        fig.update_yaxes(title_text="Attenuation (dB)", row=1 + report_n, col=2)
+        fig.update_yaxes(title_text="Amplitude", row=1 + report_n, col=2)
         fig.update_layout(
             showlegend=False,
             uirevision="0",  # ``uirevision`` allows zooming while live plotting
         )
         report_n += 1
     if report_n > 1:
         fig.update_traces(showscale=False)
@@ -290,43 +368,158 @@
         ),
     )
 
     subfolders = get_data_subfolders(folder)
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"frequency": "Hz", "attenuation": "dB"},
                 options=["qubit", "iteration"],
             )
         attenuations = data.df["attenuation"].unique()
         middle_attenuation = attenuations[len(attenuations) // 2]
         data.df = data.df[data.df["qubit"] == qubit][
             data.df["attenuation"] == middle_attenuation
         ].drop(columns=["attenuation"])
 
         iterations = data.df["iteration"].unique()
+        frequencies = data.df["frequency"].unique()
+        data.df = data.df.drop(columns=["i", "q", "qubit"])
+
+        if len(iterations) > 1:
+            opacity = 0.3
+        else:
+            opacity = 1
+        for iteration in iterations:
+            iteration_data = data.df[data.df["iteration"] == iteration]
+            fig.add_trace(
+                go.Scatter(
+                    x=iteration_data["frequency"],
+                    y=iteration_data["MSR"] * 1e6,
+                    marker_color=get_color(report_n),
+                    opacity=opacity,
+                    name=f"q{qubit}/r{report_n} Attenuation: {middle_attenuation} dB",
+                    showlegend=not bool(iteration),
+                    legendgroup=f"q{qubit}/r{report_n}",
+                ),
+                row=1,
+                col=1,
+            )
+            fig.add_trace(
+                go.Scatter(
+                    x=iteration_data["frequency"],
+                    y=iteration_data["phase"],
+                    marker_color=get_color(report_n),
+                    opacity=opacity,
+                    showlegend=False,
+                    legendgroup=f"q{qubit}/r{report_n}",
+                ),
+                row=1,
+                col=2,
+            )
+        if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
+            fig.add_trace(
+                go.Scatter(
+                    x=frequencies,
+                    y=data.df.groupby("frequency")[  # pylint: disable=E1101
+                        "MSR"
+                    ].mean()
+                    * 1e6,
+                    marker_color=get_color(report_n),
+                    name=f"q{qubit}/r{report_n}: Average",
+                    showlegend=True,
+                    legendgroup=f"q{qubit}/r{report_n}: Average",
+                ),
+                row=1,
+                col=1,
+            )
+
+            fig.add_trace(
+                go.Scatter(
+                    x=frequencies,
+                    y=data.df.groupby("frequency")[  # pylint: disable=E1101
+                        "phase"
+                    ].mean(),  # pylint: disable=E1101
+                    marker_color=get_color(report_n),
+                    showlegend=False,
+                    legendgroup=f"q{qubit}/r{report_n}: Average",
+                ),
+                row=1,
+                col=2,
+            )
+
+        report_n += 1
+
+    fig.update_layout(
+        showlegend=True,
+        uirevision="0",  # ``uirevision`` allows zooming while live plotting
+        xaxis_title="Frequency (Hz)",
+        yaxis_title="MSR (uV)",
+        xaxis2_title="Frequency (Hz)",
+        yaxis2_title="Phase (rad)",
+    )
+
+    figures.append(fig)
+
+    return figures, fitting_report
+
+
+# Resonator and qubit spectroscopies
+def frequency_amplitude_msr_phase_cut(folder, routine, qubit, format):
+    fig = make_subplots(
+        rows=1,
+        cols=2,
+        horizontal_spacing=0.1,
+        vertical_spacing=0.1,
+        subplot_titles=(
+            "MSR (V)",
+            "phase (rad)",
+        ),
+    )
+    fitting_report = "No fitting data"
+
+    subfolders = get_data_subfolders(folder)
+    report_n = 0
+    for subfolder in subfolders:
+        try:
+            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data.df = data.df[data.df["qubit"] == qubit]
+        except:
+            data = DataUnits(
+                name=f"data",
+                quantities={"frequency": "Hz", "amplitude": "dimensionless"},
+                options=["qubit", "iteration"],
+            )
+        amplitudes = data.df["amplitude"].unique()
+        middle_amplitude = amplitudes[len(amplitudes) // 2]
+        data.df = data.df[data.df["qubit"] == qubit][
+            data.df["amplitude"] == middle_amplitude
+        ].drop(columns=["amplitude"])
+
+        iterations = data.df["iteration"].unique()
         frequencies = data.df["frequency"].pint.to("Hz").pint.magnitude.unique()
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
                     x=iteration_data["frequency"].pint.to("Hz").pint.magnitude,
                     y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
                     marker_color=get_color(report_n),
                     opacity=opacity,
-                    name=f"q{qubit}/r{report_n} Attenuation: {middle_attenuation.to('dB').magnitude} dB",
+                    name=f"q{qubit}/r{report_n} Amplitude: {middle_amplitude.to('amplitude').magnitude}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
             fig.add_trace(
@@ -378,69 +571,67 @@
         showlegend=True,
         uirevision="0",  # ``uirevision`` allows zooming while live plotting
         xaxis_title="Frequency (Hz)",
         yaxis_title="MSR (uV)",
         xaxis2_title="Frequency (Hz)",
         yaxis2_title="Phase (rad)",
     )
-
-    figures.append(fig)
-
-    return figures, fitting_report
+    return fig, fitting_report
 
 
 # Resonator spectroscopy flux
 def frequency_flux_msr_phase(folder, routine, qubit, format):
     figures = []
     fitting_report = "No fitting data"
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
 
     report_n = 0
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"frequency": "Hz", "bias": "V"},
                 options=["qubit", "fluxline", "iteration"],
             )
 
         iterations = data.df["iteration"].unique()
         fluxlines = data.df["fluxline"].unique()
-        frequencies = data.df["frequency"].pint.to("Hz").pint.magnitude.unique()
-        biass = data.df["bias"].pint.to("V").pint.magnitude.unique()
+        frequencies = data.df["frequency"].unique()
 
         if len(fluxlines) > 1:
             fig = make_subplots(
                 rows=len(subfolders),
                 cols=len(fluxlines),
                 horizontal_spacing=0.1,
                 vertical_spacing=0.1,
                 subplot_titles=tuple(
                     [f"MSR [V] - fluxline {fluxline}" for fluxline in fluxlines]
                 ),
             )
 
             for fluxline_n, fluxline in enumerate(fluxlines):
                 fluxline_df = data.df[data.df["fluxline"] == fluxline]
-                fluxline_df = (
-                    fluxline_df.drop(columns=["qubit", "fluxline", "iteration"])
-                    .groupby(["frequency", "bias"], as_index=False)
-                    .mean()
+                fluxline_df = fluxline_df.drop(
+                    columns=["i", "q", "qubit", "fluxline", "iteration"]
                 )
 
+                fluxline_df = fluxline_df.groupby(
+                    ["frequency", "bias"], as_index=False
+                ).mean()
+
                 fig.add_trace(
                     go.Heatmap(
-                        x=fluxline_df["frequency"].pint.to("Hz").pint.magnitude,
-                        y=fluxline_df["bias"].pint.to("V").pint.magnitude,
-                        z=fluxline_df["MSR"].pint.to("V").pint.magnitude,
+                        x=fluxline_df["frequency"],
+                        y=fluxline_df["bias"],
+                        z=fluxline_df["MSR"] * 1e6,
                         showscale=False,
                     ),
                     row=1 + report_n,
                     col=1 + fluxline_n,
                 )
                 fig.update_xaxes(
                     title_text=f"q{qubit}/r{report_n}: Frequency (GHz)",
@@ -457,54 +648,56 @@
                 subplot_titles=(
                     f"MSR [V] - fluxline {fluxlines[0]}",
                     f"Phase [rad] - fluxline {fluxlines[0]}",
                 ),
             )
 
             fluxline_df = data.df[data.df["fluxline"] == fluxlines[0]]
-            fluxline_df = (
-                fluxline_df.drop(columns=["qubit", "fluxline", "iteration"])
-                .groupby(["frequency", "bias"], as_index=False)
-                .mean()
+            fluxline_df = fluxline_df.drop(
+                columns=["i", "q", "qubit", "fluxline", "iteration"]
             )
 
+            fluxline_df = fluxline_df.groupby(
+                ["frequency", "bias"], as_index=False
+            ).mean()
+
             fig.add_trace(
                 go.Heatmap(
-                    x=fluxline_df["frequency"].pint.to("Hz").pint.magnitude,
-                    y=fluxline_df["bias"].pint.to("V").pint.magnitude,
-                    z=fluxline_df["MSR"].pint.to("V").pint.magnitude,
+                    x=fluxline_df["frequency"],
+                    y=fluxline_df["bias"],
+                    z=fluxline_df["MSR"] * 1e6,
                     colorbar_x=0.46,
                 ),
                 row=1 + report_n,
                 col=1,
             )
             fig.update_xaxes(
                 title_text=f"q{qubit}/r{report_n}: Frequency (Hz)",
                 row=1 + report_n,
                 col=1,
             )
 
             fig.add_trace(
                 go.Heatmap(
-                    x=fluxline_df["frequency"].pint.to("Hz").pint.magnitude,
-                    y=fluxline_df["bias"].pint.to("V").pint.magnitude,
-                    z=fluxline_df["phase"].pint.to("rad").pint.magnitude,
+                    x=fluxline_df["frequency"],
+                    y=fluxline_df["bias"],
+                    z=fluxline_df["phase"],
                     colorbar_x=1.01,
                 ),
                 row=1 + report_n,
                 col=2,
             )
             fig.update_xaxes(
                 title_text=f"q{qubit}/r{report_n}: Frequency (Hz)",
                 row=1 + report_n,
                 col=2,
             )
-            fig.update_yaxes(title_text="Current (A)", row=1 + report_n, col=2)
+            fig.update_yaxes(title_text="Bias (V)", row=1 + report_n, col=2)
 
-        fig.update_yaxes(title_text="Current (A)", row=1 + report_n, col=1)
+        fig.update_yaxes(title_text="Bias (V)", row=1 + report_n, col=1)
         fig.update_layout(
             showlegend=False,
             uirevision="0",  # ``uirevision`` allows zooming while live plotting
         )
 
         report_n += 1
     if report_n > 1:
@@ -532,53 +725,51 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data_0 = DataUnits.load_data(folder, subfolder, routine, format, f"data_0")
+            data_0 = load_data(folder, subfolder, routine, format, "data_0")
             data_0.df = data_0.df[data_0.df["qubit"] == qubit]
         except:
             data_0 = DataUnits(
                 name=f"data_0",
                 quantities={"frequency": "Hz"},
                 options=["qubit", "shifted", "iteration"],
             )
         try:
-            data_1 = DataUnits.load_data(folder, subfolder, routine, format, f"data_1")
+            data_1 = load_data(folder, subfolder, routine, format, "data_1")
             data_1.df = data_1.df[data_1.df["qubit"] == qubit]
         except:
             data_1 = DataUnits(
                 name=f"data_1",
                 quantities={"frequency": "Hz"},
                 options=["qubit", "shifted", "iteration"],
             )
 
         try:
-            fit_data_0 = Data.load_data(
-                folder, subfolder, routine, format, f"fit_data_0"
-            )
+            fit_data_0 = load_data(folder, subfolder, routine, format, "fit_data_0")
+            fit_data_0.df = fit_data_0.df[fit_data_0.df["qubit"] == qubit]
         except:
             fit_data_0 = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
                     "popt3",
                     "label1",
                     "label2",
                     "label3",
                 ]
             )
 
         try:
-            fit_data_1 = Data.load_data(
-                folder, subfolder, routine, format, f"fit_data_1"
-            )
+            fit_data_1 = load_data(folder, subfolder, routine, format, "fit_data_1")
+            fit_data_1.df = fit_data_1.df[fit_data_1.df["qubit"] == qubit]
         except:
             fit_data_1 = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
                     "popt3",
@@ -592,96 +783,94 @@
             zip(
                 (0, 1),
                 ("Spectroscopy", "Shifted spectroscopy"),
                 (data_0, data_1),
                 (fit_data_0, fit_data_1),
             )
         ):
+            data.df = data.df.drop(columns=["i", "q", "qubit"])
             iterations = data.df["iteration"].unique()
-            frequencies = data.df["frequency"].pint.to("Hz").pint.magnitude.unique()
+            frequencies = data.df["frequency"].unique()
             if len(iterations) > 1:
                 opacity = 0.3
             else:
                 opacity = 1
             for iteration in iterations:
                 iteration_data = data.df[data.df["iteration"] == iteration]
                 fig.add_trace(
                     go.Scatter(
-                        x=iteration_data["frequency"].pint.to("Hz").pint.magnitude,
-                        y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                        x=iteration_data["frequency"],
+                        y=iteration_data["MSR"] * 1e6,
                         marker_color=get_color(2 * report_n + i),
                         opacity=opacity,
                         name=f"q{qubit}/r{report_n}: {label}",
                         showlegend=not bool(iteration),
                         legendgroup=f"q{qubit}/r{report_n}: {label}",
                     ),
                     row=1,
                     col=1,
                 )
                 fig.add_trace(
                     go.Scatter(
-                        x=iteration_data["frequency"].pint.to("Hz").pint.magnitude,
-                        y=iteration_data["phase"].pint.to("rad").pint.magnitude,
+                        x=iteration_data["frequency"],
+                        y=iteration_data["phase"],
                         marker_color=get_color(2 * report_n + i),
                         opacity=opacity,
                         showlegend=False,
                         legendgroup=f"q{qubit}/r{report_n}: {label}",
                     ),
                     row=1,
                     col=2,
                 )
             if len(iterations) > 1:
+                data.df = data.df.drop(columns=["iteration"])
                 fig.add_trace(
                     go.Scatter(
                         x=frequencies,
-                        y=data.df.groupby("frequency")["MSR"]
-                        .mean()
-                        .pint.to("uV")
-                        .pint.magnitude,
+                        y=data.df.groupby("frequency")["MSR"].mean() * 1e6,
                         marker_color=get_color(2 * report_n + i),
                         name=f"q{qubit}/r{report_n}: {label} Average",
                         showlegend=True,
                         legendgroup=f"q{qubit}/r{report_n}: {label} Average",
                     ),
                     row=1,
                     col=1,
                 )
+
                 fig.add_trace(
                     go.Scatter(
                         x=frequencies,
-                        y=data.df.groupby("frequency")["phase"]
-                        .mean()
-                        .pint.to("rad")
-                        .pint.magnitude,
+                        y=data.df.groupby("frequency")["phase"].mean(),
                         marker_color=get_color(2 * report_n + i),
                         showlegend=False,
                         legendgroup=f"q{qubit}/r{report_n}: {label} Average",
                     ),
                     row=1,
                     col=2,
                 )
 
             if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
                 freqrange = np.linspace(
-                    min(data.get_values("frequency", "Hz")),
-                    max(data.get_values("frequency", "Hz")),
+                    min(data.df["frequency"]),
+                    max(data.df["frequency"]),
                     2 * len(data),
                 )
                 params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                     orient="records"
                 )[0]
+
                 fig.add_trace(
                     go.Scatter(
                         x=freqrange,
                         y=lorenzian(
                             freqrange,
-                            data_fit.get_values("popt0"),
-                            data_fit.get_values("popt1"),
-                            data_fit.get_values("popt2"),
-                            data_fit.get_values("popt3"),
+                            float(data_fit.df["popt0"]),
+                            float(data_fit.df["popt1"]),
+                            float(data_fit.df["popt2"]),
+                            float(data_fit.df["popt3"]),
                         ),
                         name=f"q{qubit}/r{report_n}: {label} Fit",
                         line=go.scatter.Line(dash="dot"),
                         marker_color=get_color(3 * report_n + i),
                     ),
                     row=1,
                     col=1,
@@ -770,17 +959,17 @@
             y=data.get_values("attenuation", "dB"),
             name="Punchout",
         ),
         row=1,
         col=1,
     )
     if len(data1) > 0:
-        opt_f = data1.get_values("frequency", "GHz")[0]
-        opt_att = data1.get_values("attenuation", "dB")[0]
-        opt_snr = data1.get_values("snr", "dimensionless")[0]
+        opt_f = float(data1.get_values("frequency", "GHz"))
+        opt_att = float(data1.get_values("attenuation", "dB"))
+        opt_snr = float(data1.get_values("snr", "dimensionless"))
         fig.add_annotation(
             dict(
                 font=dict(color="black", size=12),
                 x=0,
                 y=-0.30,
                 showarrow=False,
                 text=f"Best response found at frequency {round(opt_f,len(str(opt_f))-3)} GHz <br> for attenuation value of {opt_att} dB with snr {opt_snr :.3e}.\n",
@@ -833,15 +1022,15 @@
     else:
         nb = len(fluxes)
     fig = make_subplots(
         rows=1,
         cols=nb,
         horizontal_spacing=0.05,
         vertical_spacing=0.1,
-        x_title="Current (A)",
+        x_title="Bias (V)",
         y_title="Frequency (GHz)",
         shared_xaxes=False,
         shared_yaxes=True,
     )
     for k, j in enumerate(fluxes):
         data_spec = DataUnits.load_data(
             folder, "data", routine, format, f"data_q{qubit}_f{j}"
@@ -867,26 +1056,26 @@
             if len(data_spec) > 0 and len(data_fit) > 0:
                 curr_range = np.linspace(
                     min(data_spec.get_values("bias", "V")),
                     max(data_spec.get_values("bias", "V")),
                     100,
                 )
                 if int(j) == int(qubit):
-                    f_qs = data_fit.get_values("f_qs")[0]
-                    f_rs = data_fit.get_values("f_rs")[0]
-                    curr_qs = data_fit.get_values("curr_sp")[0]
-                    g = data_fit.get_values("g")[0]
-                    d = data_fit.get_values("d")[0]
-                    xi = data_fit.get_values("xi")[0]
-                    C_ii = data_fit.get_values("C_ii")[0]
-                    f_offset = data_fit.get_values("f_offset")[0]
+                    f_qs = float(data_fit.get_values("f_qs"))
+                    f_rs = float(data_fit.get_values("f_rs"))
+                    curr_qs = float(data_fit.get_values("curr_sp"))
+                    g = float(data_fit.get_values("g"))
+                    d = float(data_fit.get_values("d"))
+                    xi = float(data_fit.get_values("xi"))
+                    C_ii = float(data_fit.get_values("C_ii"))
+                    f_offset = float(data_fit.get_values("f_offset"))
                     text_data = f"Fluxline: {j} <br> freq_r{qubit}_sp = {f_rs :.4e} Hz <br> freq_q{qubit}_sp = {f_qs :.4e} Hz <br> curr_{qubit}_sp = {curr_qs :.2e} A <br> g = {g :.2e} Hz <br> d = {d :.2e} <br> xi = {xi :.2e} 1/A <br> C_{qubit}{j} = {C_ii :.4e} Hz/A <br> f_offset_q{qubit} = {f_offset :.4e} Hz"
                     if len(data_fit.df.keys()) != 10:
-                        Ec = data_fit.get_values("Ec")[0]
-                        Ej = data_fit.get_values("Ej")[0]
+                        Ec = float(data_fit.get_values("Ec"))
+                        Ej = float(data_fit.get_values("Ej"))
                         text_data += f" <br> Ec = {Ec :.3e} Hz <br> Ej = {Ej :.3e} Hz"
                         freq_r_fit = freq_r_mathieu
                         params = [
                             data_fit.get_values("f_rh"),
                             data_fit.get_values("g"),
                             data_fit.get_values("curr_sp"),
                             data_fit.get_values("xi"),
@@ -941,15 +1130,15 @@
                             / 10**9,
                             name=f"Fit fluxline {j}",
                             line=go.scatter.Line(dash="dot"),
                         ),
                         row=1,
                         col=k + 1,
                     )
-                    C_ij = data_fit.get_values("popt0")[0]
+                    C_ij = float(data_fit.get_values("popt0"))
                     fig.add_annotation(
                         dict(
                             font=dict(color="black", size=12),
                             x=np.mean(curr_range),
                             y=-0.9,
                             showarrow=False,
                             text=f"Fluxline: {j} <br> C_{qubit}{j} = {C_ij :.4e} Hz/A.",
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/spin_echo.py` & `qibocal-0.0.2/src/qibocal/plots/spin_echo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import exp
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # Spin echos
 def spin_echo_time_msr(folder, routine, qubit, format):
     """Spin echo plotting routine:
     The routine plots the results of a modified Ramsey sequence with an additional Rx(pi) pulse placed symmetrically between the two Rx(pi/2) pulses.
     An exponential fit to this data gives a spin echo decay time T2.
@@ -30,95 +30,95 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"wait": "ns"},
                 options=["qubit", "iteration"],
             )
 
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
                     "label1",
                 ]
             )
 
+        data.df = data.df.drop(columns=["i", "q", "phase", "qubit"])
         iterations = data.df["iteration"].unique()
-        waits = data.df["wait"].pint.to("ns").pint.magnitude.unique()
+        waits = data.df["wait"].unique()
 
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["wait"].pint.to("ns").pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["wait"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
 
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
-                    x=waits,
-                    y=data.df.groupby("wait")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    x=waits.tolist(),
+                    y=data.df.groupby("wait")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
 
         # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             waitrange = np.linspace(
-                min(data.get_values("wait", "ns")),
-                max(data.get_values("wait", "ns")),
+                min(data.df["wait"]),
+                max(data.df["wait"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
 
             fig.add_trace(
                 go.Scatter(
                     x=waitrange,
                     y=exp(
                         waitrange,
-                        data_fit.df["popt0"][0],
-                        data_fit.df["popt1"][0],
-                        data_fit.df["popt2"][0],
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
```

### Comparing `qibocal-0.0.1/src/qibocal/plots/t1.py` & `qibocal-0.0.2/src/qibocal/plots/t1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from qibocal.data import Data, DataUnits
 from qibocal.fitting.utils import exp
-from qibocal.plots.utils import get_color, get_data_subfolders
+from qibocal.plots.utils import get_color, get_data_subfolders, load_data
 
 
 # T1
 def t1_time_msr(folder, routine, qubit, format):
     figures = []
 
     fig = make_subplots(
@@ -21,105 +21,105 @@
 
     # iterate over multiple data folders
     subfolders = get_data_subfolders(folder)
     report_n = 0
     fitting_report = ""
     for subfolder in subfolders:
         try:
-            data = DataUnits.load_data(folder, subfolder, routine, format, f"data")
+            data = load_data(folder, subfolder, routine, format, "data")
             data.df = data.df[data.df["qubit"] == qubit]
         except:
             data = DataUnits(
                 name=f"data",
                 quantities={"wait": "ns"},
                 options=["qubit", "iteration"],
             )
 
         try:
-            data_fit = Data.load_data(folder, subfolder, routine, format, f"fits")
+            data_fit = load_data(folder, subfolder, routine, format, "fits")
             data_fit.df = data_fit.df[data_fit.df["qubit"] == qubit]
         except:
             data_fit = Data(
                 quantities=[
                     "popt0",
                     "popt1",
                     "popt2",
                     "label1",
                     "qubit",
                 ]
             )
 
+        data.df = data.df.drop(columns=["i", "q", "phase", "qubit"])
         iterations = data.df["iteration"].unique()
-        waits = data.df["wait"].pint.to("ns").pint.magnitude.unique()
+        waits = data.df["wait"].unique()
 
         if len(iterations) > 1:
             opacity = 0.3
         else:
             opacity = 1
+
         for iteration in iterations:
             iteration_data = data.df[data.df["iteration"] == iteration]
             fig.add_trace(
                 go.Scatter(
-                    x=iteration_data["wait"].pint.to("ns").pint.magnitude,
-                    y=iteration_data["MSR"].pint.to("uV").pint.magnitude,
+                    x=iteration_data["wait"],
+                    y=iteration_data["MSR"] * 1e6,
                     marker_color=get_color(report_n),
                     opacity=opacity,
                     name=f"q{qubit}/r{report_n}",
                     showlegend=not bool(iteration),
                     legendgroup=f"q{qubit}/r{report_n}",
                 ),
                 row=1,
                 col=1,
             )
 
         if len(iterations) > 1:
+            data.df = data.df.drop(columns=["iteration"])  # pylint: disable=E1101
             fig.add_trace(
                 go.Scatter(
-                    x=waits,
-                    y=data.df.groupby("wait")["MSR"]
-                    .mean()
-                    .pint.to("uV")
-                    .pint.magnitude,
+                    x=waits,  # unique_waits,
+                    y=data.df.groupby("wait")["MSR"].mean()  # pylint: disable=E1101
+                    * 1e6,
                     marker_color=get_color(report_n),
                     name=f"q{qubit}/r{report_n}: Average",
                     showlegend=True,
                     legendgroup=f"q{qubit}/r{report_n}: Average",
                 ),
                 row=1,
                 col=1,
             )
 
-        # add fitting trace
+        # # add fitting trace
         if len(data) > 0 and (qubit in data_fit.df["qubit"].values):
             waitrange = np.linspace(
-                min(data.get_values("wait", "ns")),
-                max(data.get_values("wait", "ns")),
+                min(data.df["wait"]),
+                max(data.df["wait"]),
                 2 * len(data),
             )
             params = data_fit.df[data_fit.df["qubit"] == qubit].to_dict(
                 orient="records"
             )[0]
 
             fig.add_trace(
                 go.Scatter(
                     x=waitrange,
                     y=exp(
                         waitrange,
-                        data_fit.get_values("popt0"),
-                        data_fit.get_values("popt1"),
-                        data_fit.get_values("popt2"),
+                        float(data_fit.df["popt0"]),
+                        float(data_fit.df["popt1"]),
+                        float(data_fit.df["popt2"]),
                     ),
                     name=f"q{qubit}/r{report_n} Fit",
                     line=go.scatter.Line(dash="dot"),
                     marker_color=get_color(4 * report_n + 2),
                 ),
                 row=1,
                 col=1,
             )
-
             fitting_report = fitting_report + (
                 f"q{qubit}/r{report_n} | t1: {params['T1']:,.0f} ns.<br><br>"
             )
 
         report_n += 1
 
     # last part
```

### Comparing `qibocal-0.0.1/src/qibocal/web/app.py` & `qibocal-0.0.2/src/qibocal/web/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import os
 import re
 import time
 
 import pandas as pd
-import yaml
 from dash import Dash, Input, Output, dcc, html
 
 from qibocal import plots
+from qibocal.calibrations.niGSC.basics.plot import plot_qq
 from qibocal.data import DataUnits
 from qibocal.web.server import server
 
 DataUnits()  # dummy dataset call to suppress ``pint[V]`` error
 
 app = Dash(
     server=server,
@@ -31,19 +31,15 @@
                     children=[html.P("Refresh rate:")],
                 ),
                 dcc.Dropdown(
                     id="interval-refresh",
                     className="interval-refresh",
                     placeholder="Select refresh rate",
                     options=[
-                        {"label": "Auto refresh", "value": 0},
-                        {"label": "2 seconds", "value": 2},
-                        {"label": "5 seconds", "value": 5},
-                        {"label": "10 seconds", "value": 10},
-                        {"label": "20 seconds", "value": 20},
+                        {"label": "Auto", "value": 0},
                         {"label": "No refresh", "value": 3600},
                     ],
                     value=0,
                 ),
                 html.Div(
                     id="latest-timestamp",
                     className="latest-timestamp",
@@ -51,16 +47,15 @@
             ],
         ),
         html.Div(id="div-fitting", className="div-fitting"),
         html.Div(id="div-figures"),
         dcc.Location(id="url", refresh=False),
         dcc.Interval(
             id="interval",
-            # TODO: Perhaps the user should be allowed to change the refresh rate
-            interval=5 * 1000,
+            interval=160 * 1000,
             n_intervals=0,
             disabled=False,
         ),
     ]
 )
 
 
@@ -95,19 +90,24 @@
         #     params, fit = None, None
         # return getattr(plots.resonator_spectroscopy, method)(data, params, fit)
 
         # # FIXME: Temporarily hardcode the plotting method to test
         # # multiple routines with different names in one folder
         # # should be changed to:
         # # return getattr(getattr(plots, routine), method)(data)
-        figs, fitting_report = getattr(plots, method)(folder, routine, qubit, format)
+        if hasattr(plots, method):
+            figs, fitting_report = getattr(plots, method)(
+                folder, routine, qubit, format
+            )
+        else:
+            figs, fitting_report = plot_qq(folder, routine, qubit, format)
         et = time.time()
 
         if value == 0:
-            refresh_rate = (et - st) + 6
+            refresh_rate = int(et - st) + 6
         else:
             refresh_rate = value
 
         for fig in figs:
             figures.append(dcc.Graph(figure=fig))
 
         table = ""
```

### Comparing `qibocal-0.0.1/src/qibocal/web/server.py` & `qibocal-0.0.2/src/qibocal/web/server.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/web/static/styles.css` & `qibocal-0.0.2/src/qibocal/web/static/styles.css`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.1/src/qibocal/web/templates/template.html` & `qibocal-0.0.2/src/qibocal/web/templates/template.html`

 * *Files 4% similar despite different names*

```diff
@@ -182,17 +182,45 @@
                         <div id="{{ routine }}-{{ method }}" style="scroll-margin-top: 4em;">
                         {% for qubit in report.qubits %}
                           <div id="{{ routine }}-{{ method }}-{{ qubit }}" style="scroll-margin-top: 4em;">
                               <h5
                                 class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
                                 {{ header }} - Qubit {{ qubit }}</h5>
                                 {% if is_static %}
-                                  {{ report.get_figure(routine, method, qubit) }}
+                                  {% set figures, fitting_report = report.get_figure(routine, method, qubit) %}
+                                  {% if "No fitting data" not in fitting_report %}
+                                    {% set fitting_params= fitting_report.split('<br>') %}
+                                      <div class="div-fitting">
+                                        <table class="fitting-table">
+                                          <thead>
+                                            <tr>
+                                              <th class="th_styles">qubit # / report #</th>
+                                              <th class="th_styles">Fitting Parameter	</th>
+                                              <th class="th_styles">Value</th>
+                                            </tr>
+                                          </thead>
+                                          <tbody>
+                                            {% for row in fitting_params %}
+                                              {% if row != '' %}
+                                                {% set run = row.split('|') %}
+                                                {% set fparam_value = run[1].split(':') %}
+                                                <tr>
+                                                  <td class="td_styles">{{ run[0] }}</td>
+                                                  <td class="td_styles">{{ fparam_value[0] }}</td>
+                                                  <td class="td_styles">{{ fparam_value[1] }}</td>
+                                                </tr>
+                                              {% endif %}
+                                            {% endfor %}
+                                          </tbody>
+                                        </table>
+                                      </div>
+                                  {% endif %}
+                                  {{ figures }}
                                 {% else %}
-                                  <iframe src='{{ report.get_live_figure(routine, method, qubit) }}' class="gh-fit gh-fullwidth"></iframe>
+                                  <iframe src='{{ report.get_live_figure(routine, method, qubit) }}?_retry=0' class="gh-fit gh-fullwidth"></iframe>
                                 {% endif %}
                           </div>
                         {% endfor %}
                         </div>
                     {% endfor %}
                   {% else %}
                     <p>No plots available for {{ routine.__name__ }}.</p>
```

#### html2text {}

```diff
@@ -44,16 +44,21 @@
 **** Actions ****
 Please find below data generated by actions:
 {% for routine in report.routines %}
 *** {{ report.get_routine_name(routine) }} ***
 {% if routine.plots %} {% for header, method in routine.plots %}
 {% for qubit in report.qubits %}
 ** {{ header }} - Qubit {{ qubit }} **
-{% if is_static %} {{ report.get_figure(routine, method, qubit) }} {% else %}
-{% endif %}
+{% if is_static %} {% set figures, fitting_report = report.get_figure(routine,
+method, qubit) %} {% if "No fitting data" not in fitting_report %} {% set
+fitting_params= fitting_report.split('
+') %}
+qubit # / report # Fitting Parameter     Value
+{{ run[0] }}       {{ fparam_value[0] }} {{ fparam_value[1] }}
+{% endif %} {{ figures }} {% else %}  {% endif %}
 {% endfor %}
 {% endfor %} {% else %}
 No plots available for {{ routine.__name__ }}.
 {% endif %} {% endfor %}
 {% endif %} {% endfor %} {% else %} {% if error %}
 ***** Qibocal Error *****
 {{error}}
```

### Comparing `qibocal-0.0.1/PKG-INFO` & `qibocal-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,250 +1,295 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7169 626f  : 2.1.Name: qibo
 00000020: 6361 6c0a 5665 7273 696f 6e3a 2030 2e30  cal.Version: 0.0
-00000030: 2e31 0a53 756d 6d61 7279 3a20 0a48 6f6d  .1.Summary: .Hom
+00000030: 2e32 0a53 756d 6d61 7279 3a20 0a48 6f6d  .2.Summary: .Hom
 00000040: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
 00000050: 6769 7468 7562 2e63 6f6d 2f71 6962 6f74  github.com/qibot
 00000060: 6561 6d2f 7169 626f 6361 6c2f 0a4c 6963  eam/qibocal/.Lic
 00000070: 656e 7365 3a20 4170 6163 6865 2d32 2e30  ense: Apache-2.0
 00000080: 0a41 7574 686f 723a 2061 6e64 7265 612d  .Author: andrea-
 00000090: 7061 7371 7561 6c65 0a41 7574 686f 722d  pasquale.Author-
 000000a0: 656d 6169 6c3a 2061 6e64 7265 6170 6173  email: andreapas
 000000b0: 7175 616c 6539 3740 676d 6169 6c2e 636f  quale97@gmail.co
 000000c0: 6d0a 5265 7175 6972 6573 2d50 7974 686f  m.Requires-Pytho
-000000d0: 6e3a 203e 3d33 2e38 2c3c 340a 436c 6173  n: >=3.8,<4.Clas
-000000e0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-000000f0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000100: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
-00000110: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
-00000120: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000130: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000140: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
-00000150: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000170: 7974 686f 6e20 3a3a 2033 2e38 0a43 6c61  ython :: 3.8.Cla
-00000180: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000190: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001a0: 2050 7974 686f 6e20 3a3a 2033 2e39 0a43   Python :: 3.9.C
-000001b0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000001e0: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
-000001f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000200: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000210: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
-00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000240: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
-00000250: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
-00000260: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-00000270: 203a 3a20 5068 7973 6963 730a 5072 6f76   :: Physics.Prov
-00000280: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
+000000d0: 6e3a 203e 3d33 2e38 2c3c 332e 3132 0a43  n: >=3.8,<3.12.C
+000000e0: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+000000f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000100: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+00000110: 7477 6172 6520 4c69 6365 6e73 650a 436c  tware License.Cl
+00000120: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000130: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000140: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+00000150: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000160: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000170: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000180: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000190: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001a0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001b0: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+000001c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001e0: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+000001f0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000200: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000210: 3a3a 2033 2e31 310a 436c 6173 7369 6669  :: 3.11.Classifi
+00000220: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
+00000230: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000240: 696e 6720 3a3a 2050 6879 7369 6373 0a50  ing :: Physics.P
+00000250: 726f 7669 6465 732d 4578 7472 613a 2063  rovides-Extra: c
+00000260: 6c61 7373 6966 790a 5072 6f76 6964 6573  lassify.Provides
+00000270: 2d45 7874 7261 3a20 646f 6373 0a50 726f  -Extra: docs.Pro
+00000280: 7669 6465 732d 4578 7472 613a 2076 697a  vides-Extra: viz
 00000290: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 000002a0: 5069 6e74 2d50 616e 6461 7320 283e 3d30  Pint-Pandas (>=0
 000002b0: 2e33 2c3c 302e 3429 0a52 6571 7569 7265  .3,<0.4).Require
 000002c0: 732d 4469 7374 3a20 5370 6869 6e78 2028  s-Dist: Sphinx (
-000002d0: 3e3d 342e 332e 322c 3c35 2e30 2e30 2920  >=4.3.2,<5.0.0) 
+000002d0: 3e3d 352e 302e 302c 3c36 2e30 2e30 2920  >=5.0.0,<6.0.0) 
 000002e0: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
 000002f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
 00000300: 2064 6173 6820 283e 3d32 2e36 2e30 2c3c   dash (>=2.6.0,<
 00000310: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
 00000320: 4469 7374 3a20 6675 726f 2028 3e3d 3230  Dist: furo (>=20
-00000330: 3232 2e39 2e32 392c 3c32 3032 332e 302e  22.9.29,<2023.0.
+00000330: 3233 2e33 2e32 372c 3c32 3032 342e 302e  23.3.27,<2024.0.
 00000340: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
 00000350: 6f63 7322 0a52 6571 7569 7265 732d 4469  ocs".Requires-Di
-00000360: 7374 3a20 6c6d 6669 7420 283e 3d31 2e30  st: lmfit (>=1.0
-00000370: 2e33 2c3c 322e 302e 3029 0a52 6571 7569  .3,<2.0.0).Requi
-00000380: 7265 732d 4469 7374 3a20 7061 6e64 6173  res-Dist: pandas
-00000390: 2028 3e3d 312e 342e 332c 3c32 2e30 2e30   (>=1.4.3,<2.0.0
-000003a0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-000003b0: 2071 6962 6f20 283e 3d30 2e31 2e39 2c3c   qibo (>=0.1.9,<
-000003c0: 302e 322e 3029 0a52 6571 7569 7265 732d  0.2.0).Requires-
-000003d0: 4469 7374 3a20 7169 626f 6c61 6220 283e  Dist: qibolab (>
-000003e0: 3d30 2e30 2e31 2c3c 302e 302e 3229 0a52  =0.0.1,<0.0.2).R
-000003f0: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
-00000400: 636f 6d6d 6f6e 6d61 726b 2028 3e3d 302e  commonmark (>=0.
-00000410: 372e 312c 3c30 2e38 2e30 2920 3b20 6578  7.1,<0.8.0) ; ex
-00000420: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
-00000430: 7175 6972 6573 2d44 6973 743a 2073 7068  quires-Dist: sph
-00000440: 696e 785f 6d61 726b 646f 776e 5f74 6162  inx_markdown_tab
-00000450: 6c65 7320 283e 3d30 2e30 2e31 372c 3c30  les (>=0.0.17,<0
-00000460: 2e30 2e31 3829 203b 2065 7874 7261 203d  .0.18) ; extra =
-00000470: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
-00000480: 732d 4469 7374 3a20 7370 6869 6e78 636f  s-Dist: sphinxco
-00000490: 6e74 7269 622d 6269 6274 6578 2028 3e3d  ntrib-bibtex (>=
-000004a0: 322e 342e 312c 3c33 2e30 2e30 2920 3b20  2.4.1,<3.0.0) ; 
-000004b0: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
-000004c0: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
-000004d0: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
-000004e0: 2f67 6974 6875 622e 636f 6d2f 7169 626f  /github.com/qibo
-000004f0: 7465 616d 2f71 6962 6f63 616c 2f0a 4465  team/qibocal/.De
-00000500: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000510: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000520: 6b64 6f77 6e0a 0a23 2051 6962 6f63 616c  kdown..# Qibocal
-00000530: 0a21 5b54 6573 7473 5d28 6874 7470 733a  .![Tests](https:
-00000540: 2f2f 6769 7468 7562 2e63 6f6d 2f71 6962  //github.com/qib
-00000550: 6f74 6561 6d2f 7169 626f 6361 6c2f 776f  oteam/qibocal/wo
-00000560: 726b 666c 6f77 732f 5465 7374 732f 6261  rkflows/Tests/ba
-00000570: 6467 652e 7376 6729 0a5b 215b 636f 6465  dge.svg).[![code
-00000580: 636f 765d 2868 7474 7073 3a2f 2f63 6f64  cov](https://cod
-00000590: 6563 6f76 2e69 6f2f 6768 2f71 6962 6f74  ecov.io/gh/qibot
-000005a0: 6561 6d2f 7169 626f 6361 6c2f 6272 616e  eam/qibocal/bran
-000005b0: 6368 2f6d 6169 6e2f 6772 6170 682f 6261  ch/main/graph/ba
-000005c0: 6467 652e 7376 673f 746f 6b65 6e3d 3145  dge.svg?token=1E
-000005d0: 4b5a 4b56 4556 5830 295d 2868 7474 7073  KZKVEVX0)](https
-000005e0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-000005f0: 2f71 6962 6f74 6561 6d2f 7169 626f 290a  /qiboteam/qibo).
-00000600: 5b21 5b44 6f63 756d 656e 7461 7469 6f6e  [![Documentation
-00000610: 2053 7461 7475 735d 2868 7474 7073 3a2f   Status](https:/
-00000620: 2f72 6561 6474 6865 646f 6373 2e6f 7267  /readthedocs.org
-00000630: 2f70 726f 6a65 6374 732f 7169 626f 6361  /projects/qiboca
-00000640: 6c2f 6261 6467 652f 3f76 6572 7369 6f6e  l/badge/?version
-00000650: 3d6c 6174 6573 7429 5d28 6874 7470 733a  =latest)](https:
-00000660: 2f2f 7169 626f 6361 6c2e 7265 6164 7468  //qibocal.readth
-00000670: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000680: 7374 2f29 0a0a 5169 626f 6361 6c20 7072  st/)..Qibocal pr
-00000690: 6f76 6964 6573 2051 7561 6e74 756d 2043  ovides Quantum C
-000006a0: 6861 7261 6374 6572 697a 6174 696f 6e20  haracterization 
-000006b0: 5661 6c69 6461 7469 6f6e 2061 6e64 2056  Validation and V
-000006c0: 6572 6966 6963 6174 696f 6e20 7072 6f74  erification prot
-000006d0: 6f63 6f6c 7320 7573 696e 6720 5b51 6962  ocols using [Qib
-000006e0: 6f5d 2868 7474 7073 3a2f 2f67 6974 6875  o](https://githu
-000006f0: 622e 636f 6d2f 7169 626f 7465 616d 2f71  b.com/qiboteam/q
-00000700: 6962 6f29 2061 6e64 205b 5169 626f 6c61  ibo) and [Qibola
-00000710: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
-00000720: 622e 636f 6d2f 7169 626f 7465 616d 2f71  b.com/qiboteam/q
-00000730: 6962 6f6c 6162 292e 0a0a 5169 626f 6361  ibolab)...Qiboca
-00000740: 6c20 6b65 7920 6665 6174 7572 6573 3a0a  l key features:.
-00000750: 0a2d 2041 7574 6f6d 6174 697a 6174 696f  .- Automatizatio
-00000760: 6e20 6f66 2063 616c 6962 7261 7469 6f6e  n of calibration
-00000770: 2072 6f75 7469 6e65 732e 0a0a 2d20 4465   routines...- De
-00000780: 636c 6172 6174 6976 6520 696e 7075 7473  clarative inputs
-00000790: 2075 7369 6e67 2072 756e 6361 7264 2e0a   using runcard..
-000007a0: 0a2d 2047 656e 6572 6174 696f 6e20 6f66  .- Generation of
-000007b0: 2061 2072 6570 6f72 742e 0a0a 2323 2049   a report...## I
-000007c0: 6e73 7461 6c6c 6174 696f 6e0a 0a54 6865  nstallation..The
-000007d0: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
-000007e0: 696e 7374 616c 6c65 6420 6279 2073 6f75  installed by sou
-000007f0: 7263 653a 0a60 6060 7368 0a67 6974 2063  rce:.```sh.git c
-00000800: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00000810: 6875 622e 636f 6d2f 7169 626f 7465 616d  hub.com/qiboteam
-00000820: 2f71 6962 6f63 616c 2e67 6974 0a63 6420  /qibocal.git.cd 
-00000830: 7169 626f 6361 6c0a 7069 7020 696e 7374  qibocal.pip inst
-00000840: 616c 6c20 2e0a 6060 600a 0a0a 2323 2320  all ..```...### 
-00000850: 4465 7665 6c6f 7065 7220 696e 7374 7275  Developer instru
-00000860: 6374 696f 6e73 0a46 6f72 2064 6576 656c  ctions.For devel
-00000870: 6f70 6d65 6e74 206d 616b 6520 7375 7265  opment make sure
-00000880: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
-00000890: 7061 636b 6167 6520 7573 696e 6720 5b60  package using [`
-000008a0: 706f 6574 7279 605d 2868 7474 7073 3a2f  poetry`](https:/
-000008b0: 2f70 7974 686f 6e2d 706f 6574 7279 2e6f  /python-poetry.o
-000008c0: 7267 2f29 2061 6e64 2074 6f20 696e 7374  rg/) and to inst
-000008d0: 616c 6c20 7468 6520 7072 652d 636f 6d6d  all the pre-comm
-000008e0: 6974 2068 6f6f 6b73 3a0a 6060 6073 680a  it hooks:.```sh.
-000008f0: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-00000900: 2f2f 6769 7468 7562 2e63 6f6d 2f71 6962  //github.com/qib
-00000910: 6f74 6561 6d2f 7169 626f 6361 6c2e 6769  oteam/qibocal.gi
-00000920: 740a 6364 2071 6962 6f63 616c 0a70 6f65  t.cd qibocal.poe
-00000930: 7472 7920 696e 7374 616c 6c0a 7072 652d  try install.pre-
-00000940: 636f 6d6d 6974 2069 6e73 7461 6c6c 0a60  commit install.`
-00000950: 6060 0a0a 2323 204d 696e 696d 616c 2077  ``..## Minimal w
-00000960: 6f72 6b69 6e67 2065 7861 6d70 6c65 0a0a  orking example..
-00000970: 5468 6973 2073 6563 7469 6f6e 2073 686f  This section sho
-00000980: 7773 2074 6865 2073 7465 7073 2074 6f20  ws the steps to 
-00000990: 7065 7266 6f72 6d20 6120 7265 736f 6e61  perform a resona
-000009a0: 746f 7220 7370 6563 7472 6f73 636f 7079  tor spectroscopy
-000009b0: 2077 6974 6820 5169 626f 6361 6c2e 0a23   with Qibocal..#
-000009c0: 2323 2057 7269 7465 2061 2072 756e 6361  ## Write a runca
-000009d0: 7264 0a41 2072 756e 6361 7264 2063 6f6e  rd.A runcard con
-000009e0: 7461 696e 7320 616c 6c20 7468 6520 6573  tains all the es
-000009f0: 7365 6e74 6961 6c20 696e 666f 726d 6174  sential informat
-00000a00: 696f 6e20 746f 2072 756e 2061 2073 7065  ion to run a spe
-00000a10: 6369 6669 6320 7461 736b 2e0a 466f 7220  cific task..For 
-00000a20: 6f75 7220 7075 7270 6f73 6573 2c20 7765  our purposes, we
-00000a30: 2063 616e 2075 7365 2074 6865 2066 6f6c   can use the fol
-00000a40: 6c6f 7769 6e67 3a0a 6060 6079 6d6c 0a70  lowing:.```yml.p
-00000a50: 6c61 7466 6f72 6d3a 2074 6969 3171 0a0a  latform: tii1q..
-00000a60: 7175 6269 7473 3a20 5b30 5d0a 0a66 6f72  qubits: [0]..for
-00000a70: 6d61 743a 2063 7376 0a0a 6163 7469 6f6e  mat: csv..action
-00000a80: 733a 0a20 2020 7265 736f 6e61 746f 725f  s:.   resonator_
-00000a90: 7370 6563 7472 6f73 636f 7079 3a0a 2020  spectroscopy:.  
-00000aa0: 2020 206c 6f77 7265 735f 7769 6474 683a     lowres_width:
-00000ab0: 2035 5f30 3030 5f30 3030 0a20 2020 2020   5_000_000.     
-00000ac0: 6c6f 7772 6573 5f73 7465 703a 2032 5f30  lowres_step: 2_0
-00000ad0: 3030 5f30 3030 0a20 2020 2020 6869 6768  00_000.     high
-00000ae0: 7265 735f 7769 6474 683a 2031 5f35 3030  res_width: 1_500
-00000af0: 5f30 3030 0a20 2020 2020 6869 6768 7265  _000.     highre
-00000b00: 735f 7374 6570 3a20 3230 305f 3030 300a  s_step: 200_000.
-00000b10: 2020 2020 2070 7265 6369 7369 6f6e 5f77       precision_w
-00000b20: 6964 7468 3a20 315f 3530 305f 3030 300a  idth: 1_500_000.
-00000b30: 2020 2020 2070 7265 6369 7369 6f6e 5f73       precision_s
-00000b40: 7465 703a 2031 3030 5f30 3030 0a20 2020  tep: 100_000.   
-00000b50: 2020 736f 6674 7761 7265 5f61 7665 7261    software_avera
-00000b60: 6765 733a 2031 0a20 2020 2020 706f 696e  ges: 1.     poin
-00000b70: 7473 3a20 350a 6060 600a 2323 2320 5275  ts: 5.```.### Ru
-00000b80: 6e20 7468 6520 726f 7574 696e 650a 546f  n the routine.To
-00000b90: 2072 756e 2061 6c6c 2074 6865 2063 616c   run all the cal
-00000ba0: 6962 7261 7469 6f6e 2072 6f75 7469 6e65  ibration routine
-00000bb0: 7320 7370 6563 6966 6965 6420 696e 2074  s specified in t
-00000bc0: 6865 2060 6060 7275 6e63 6172 6460 6060  he ```runcard```
-00000bd0: 2c20 5169 626f 6361 6c20 7573 6573 2074  , Qibocal uses t
-00000be0: 6865 2060 7171 6020 636f 6d6d 616e 640a  he `qq` command.
-00000bf0: 6060 6073 680a 7171 203c 7275 6e63 6172  ```sh.qq <runcar
-00000c00: 643e 202d 6f20 3c6f 7574 7075 745f 666f  d> -o <output_fo
-00000c10: 6c64 6572 3e0a 6060 600a 6966 2060 6060  lder>.```.if ```
-00000c20: 3c6f 7574 7075 745f 666f 6c64 6572 3e60  <output_folder>`
-00000c30: 6060 2069 7320 7370 6563 6966 6965 642c  `` is specified,
-00000c40: 2074 6865 2072 6573 756c 7473 2077 696c   the results wil
-00000c50: 6c20 6265 2073 6176 6564 2069 6e20 6974  l be saved in it
-00000c60: 2c20 6f74 6865 7277 6973 6520 6060 6071  , otherwise ```q
-00000c70: 7160 6060 2077 696c 6c20 6175 746f 6d61  q``` will automa
-00000c80: 7469 6361 6c6c 7920 6372 6561 7465 2061  tically create a
-00000c90: 2064 6566 6175 6c74 2066 6f6c 6465 7220   default folder 
-00000ca0: 636f 6e74 6169 6e69 6e67 2074 6865 2063  containing the c
-00000cb0: 7572 7265 6e74 2064 6174 6520 616e 6420  urrent date and 
-00000cc0: 7468 6520 7573 6572 6e61 6d65 2e0a 0a23  the username...#
-00000cd0: 2323 2056 6973 7561 6c69 7a65 2074 6865  ## Visualize the
-00000ce0: 2064 6174 610a 0a51 6962 6f63 616c 2067   data..Qibocal g
-00000cf0: 6976 6573 2074 6865 2070 6f73 7369 6269  ives the possibi
-00000d00: 6c69 7479 2074 6f20 6c69 7665 2d70 6c6f  lity to live-plo
-00000d10: 7474 696e 6720 7769 7468 2074 6865 2060  tting with the `
-00000d20: 7171 2d6c 6976 6560 2063 6f6d 6d61 6e64  qq-live` command
-00000d30: 0a60 6060 7368 0a71 712d 6c69 7665 203c  .```sh.qq-live <
-00000d40: 6f75 7470 7574 5f66 6f6c 6465 723e 0a60  output_folder>.`
-00000d50: 6060 0a23 2323 2055 706c 6f61 6469 6e67  ``.### Uploading
-00000d60: 2072 6570 6f72 7473 2074 6f20 7365 7276   reports to serv
-00000d70: 6572 0a0a 496e 206f 7264 6572 2074 6f20  er..In order to 
-00000d80: 7570 6c6f 6164 2074 6865 2072 6570 6f72  upload the repor
-00000d90: 7420 746f 2061 2063 656e 7472 616c 697a  t to a centraliz
-00000da0: 6564 2073 6572 7665 722c 2073 656e 6420  ed server, send 
-00000db0: 746f 2074 6865 2073 6572 7665 7220 6164  to the server ad
-00000dc0: 6d69 6e69 7374 7261 746f 7273 2079 6f75  ministrators you
-00000dd0: 7220 7075 626c 6963 2073 7368 206b 6579  r public ssh key
-00000de0: 2028 6672 6f6d 2074 6865 206d 6163 6869   (from the machi
-00000df0: 6e65 2873 2920 796f 7520 6172 6520 706c  ne(s) you are pl
-00000e00: 616e 6e69 6e67 2074 6f20 7570 6c6f 6164  anning to upload
-00000e10: 2074 6865 2072 6570 6f72 7429 2061 6e64   the report) and
-00000e20: 2074 6865 6e20 7573 6520 7468 6520 6071   then use the `q
-00000e30: 712d 7570 6c6f 6164 203c 6f75 7470 7574  q-upload <output
-00000e40: 5f66 6f6c 6465 723e 6020 636f 6d6d 616e  _folder>` comman
-00000e50: 642e 2054 6869 7320 7072 6f67 7261 6d20  d. This program 
-00000e60: 7769 6c6c 2075 706c 6f61 6420 796f 7572  will upload your
-00000e70: 2072 6570 6f72 7420 746f 2074 6865 2073   report to the s
-00000e80: 6572 7665 7220 616e 6420 6765 6e65 7261  erver and genera
-00000e90: 7465 2061 6e20 756e 6971 7565 2055 524c  te an unique URL
-00000ea0: 2e0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-00000eb0: 6e67 0a0a 436f 6e74 7269 6275 7469 6f6e  ng..Contribution
-00000ec0: 732c 2069 7373 7565 7320 616e 6420 6665  s, issues and fe
-00000ed0: 6174 7572 6520 7265 7175 6573 7473 2061  ature requests a
-00000ee0: 7265 2077 656c 636f 6d65 210a 4665 656c  re welcome!.Feel
-00000ef0: 2066 7265 6520 746f 2063 6865 636b 0a3c   free to check.<
-00000f00: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000f10: 6769 7468 7562 2e63 6f6d 2f71 6962 6f74  github.com/qibot
-00000f20: 6561 6d2f 7169 626f 6361 6c2f 6973 7375  eam/qibocal/issu
-00000f30: 6573 223e 3c69 6d67 2061 6c74 3d22 4769  es"><img alt="Gi
-00000f40: 7448 7562 2069 7373 7565 7322 2073 7263  tHub issues" src
-00000f50: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000f60: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000f70: 6973 7375 6573 2d63 6c6f 7365 642f 7169  issues-closed/qi
-00000f80: 626f 7465 616d 2f71 6962 6f63 616c 222f  boteam/qibocal"/
-00000f90: 3e3c 2f61 3e0a 0a                        ></a>..
+00000360: 7374 3a20 6b65 7261 732d 7475 6e65 7220  st: keras-tuner 
+00000370: 283e 3d31 2e33 2e30 2c3c 312e 332e 3129  (>=1.3.0,<1.3.1)
+00000380: 203b 2028 7379 735f 706c 6174 666f 726d   ; (sys_platform
+00000390: 203d 3d20 226c 696e 7578 2220 6f72 2073   == "linux" or s
+000003a0: 7973 5f70 6c61 7466 6f72 6d20 3d3d 2022  ys_platform == "
+000003b0: 6461 7277 696e 2229 2061 6e64 2028 6578  darwin") and (ex
+000003c0: 7472 6120 3d3d 2022 636c 6173 7369 6679  tra == "classify
+000003d0: 2229 0a52 6571 7569 7265 732d 4469 7374  ").Requires-Dist
+000003e0: 3a20 6c6d 6669 7420 283e 3d31 2e30 2e33  : lmfit (>=1.0.3
+000003f0: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
+00000400: 732d 4469 7374 3a20 6d61 7470 6c6f 746c  s-Dist: matplotl
+00000410: 6962 2028 3e3d 332e 372e 302c 3c34 2e30  ib (>=3.7.0,<4.0
+00000420: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
+00000430: 636c 6173 7369 6679 220a 5265 7175 6972  classify".Requir
+00000440: 6573 2d44 6973 743a 206e 6574 776f 726b  es-Dist: network
+00000450: 7820 283e 3d33 2e30 2c3c 342e 3029 0a52  x (>=3.0,<4.0).R
+00000460: 6571 7569 7265 732d 4469 7374 3a20 7061  equires-Dist: pa
+00000470: 6e64 6173 2028 3e3d 312e 342e 332c 3c32  ndas (>=1.4.3,<2
+00000480: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000490: 6973 743a 2070 696e 7420 283e 3d30 2e32  ist: pint (>=0.2
+000004a0: 302e 312c 3c30 2e32 312e 3029 0a52 6571  0.1,<0.21.0).Req
+000004b0: 7569 7265 732d 4469 7374 3a20 7079 6461  uires-Dist: pyda
+000004c0: 6e74 6963 2028 3e3d 312e 3130 2e35 2c3c  ntic (>=1.10.5,<
+000004d0: 322e 302e 3029 0a52 6571 7569 7265 732d  2.0.0).Requires-
+000004e0: 4469 7374 3a20 7079 646f 7420 283e 3d31  Dist: pydot (>=1
+000004f0: 2e34 2e32 2c3c 322e 302e 3029 203b 2065  .4.2,<2.0.0) ; e
+00000500: 7874 7261 203d 3d20 2276 697a 220a 5265  xtra == "viz".Re
+00000510: 7175 6972 6573 2d44 6973 743a 2071 6962  quires-Dist: qib
+00000520: 6f20 283e 3d30 2e31 2e39 2c3c 302e 322e  o (>=0.1.9,<0.2.
+00000530: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000540: 3a20 7169 626f 6c61 6220 283d 3d30 2e30  : qibolab (==0.0
+00000550: 2e33 290a 5265 7175 6972 6573 2d44 6973  .3).Requires-Dis
+00000560: 743a 2072 6563 6f6d 6d6f 6e6d 6172 6b20  t: recommonmark 
+00000570: 283e 3d30 2e37 2e31 2c3c 302e 382e 3029  (>=0.7.1,<0.8.0)
+00000580: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
+00000590: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
+000005a0: 3a20 7363 696b 6974 2d6c 6561 726e 2028  : scikit-learn (
+000005b0: 3e3d 312e 322e 312c 3c32 2e30 2e30 2920  >=1.2.1,<2.0.0) 
+000005c0: 3b20 6578 7472 6120 3d3d 2022 636c 6173  ; extra == "clas
+000005d0: 7369 6679 220a 5265 7175 6972 6573 2d44  sify".Requires-D
+000005e0: 6973 743a 2073 6561 626f 726e 2028 3e3d  ist: seaborn (>=
+000005f0: 302e 3132 2e32 2c3c 302e 3133 2e30 2920  0.12.2,<0.13.0) 
+00000600: 3b20 6578 7472 6120 3d3d 2022 636c 6173  ; extra == "clas
+00000610: 7369 6679 220a 5265 7175 6972 6573 2d44  sify".Requires-D
+00000620: 6973 743a 2073 7068 696e 785f 6d61 726b  ist: sphinx_mark
+00000630: 646f 776e 5f74 6162 6c65 7320 283e 3d30  down_tables (>=0
+00000640: 2e30 2e31 372c 3c30 2e30 2e31 3829 203b  .0.17,<0.0.18) ;
+00000650: 2065 7874 7261 203d 3d20 2264 6f63 7322   extra == "docs"
+00000660: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000670: 7370 6869 6e78 636f 6e74 7269 622d 6269  sphinxcontrib-bi
+00000680: 6274 6578 2028 3e3d 322e 342e 312c 3c33  btex (>=2.4.1,<3
+00000690: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
+000006a0: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+000006b0: 2d44 6973 743a 2074 656e 736f 7266 6c6f  -Dist: tensorflo
+000006c0: 7720 283e 3d32 2e31 322e 302c 3c33 2e30  w (>=2.12.0,<3.0
+000006d0: 2e30 2920 3b20 2873 7973 5f70 6c61 7466  .0) ; (sys_platf
+000006e0: 6f72 6d20 3d3d 2022 6c69 6e75 7822 206f  orm == "linux" o
+000006f0: 7220 7379 735f 706c 6174 666f 726d 203d  r sys_platform =
+00000700: 3d20 2264 6172 7769 6e22 2920 616e 6420  = "darwin") and 
+00000710: 2865 7874 7261 203d 3d20 2263 6c61 7373  (extra == "class
+00000720: 6966 7922 290a 5072 6f6a 6563 742d 5552  ify").Project-UR
+00000730: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
+00000740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000750: 6d2f 7169 626f 7465 616d 2f71 6962 6f63  m/qiboteam/qiboc
+00000760: 616c 2f0a 4465 7363 7269 7074 696f 6e2d  al/.Description-
+00000770: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000780: 7874 2f6d 6172 6b64 6f77 6e0a 0a23 2051  xt/markdown..# Q
+00000790: 6962 6f63 616c 0a21 5b54 6573 7473 5d28  ibocal.![Tests](
+000007a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007b0: 6f6d 2f71 6962 6f74 6561 6d2f 7169 626f  om/qiboteam/qibo
+000007c0: 6361 6c2f 776f 726b 666c 6f77 732f 5465  cal/workflows/Te
+000007d0: 7374 732f 6261 6467 652e 7376 6729 0a5b  sts/badge.svg).[
+000007e0: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+000007f0: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000800: 2f71 6962 6f74 6561 6d2f 7169 626f 6361  /qiboteam/qiboca
+00000810: 6c2f 6272 616e 6368 2f6d 6169 6e2f 6772  l/branch/main/gr
+00000820: 6170 682f 6261 6467 652e 7376 673f 746f  aph/badge.svg?to
+00000830: 6b65 6e3d 3145 4b5a 4b56 4556 5830 295d  ken=1EKZKVEVX0)]
+00000840: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
+00000850: 2e69 6f2f 6768 2f71 6962 6f74 6561 6d2f  .io/gh/qiboteam/
+00000860: 7169 626f 6361 6c29 0a5b 215b 446f 6375  qibocal).[![Docu
+00000870: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000880: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
+00000890: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
+000008a0: 7473 2f71 6962 6f63 616c 2f62 6164 6765  ts/qibocal/badge
+000008b0: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
+000008c0: 295d 2868 7474 7073 3a2f 2f71 6962 6f63  )](https://qiboc
+000008d0: 616c 2e72 6561 6474 6865 646f 6373 2e69  al.readthedocs.i
+000008e0: 6f2f 656e 2f6c 6174 6573 742f 290a 5b21  o/en/latest/).[!
+000008f0: 5b44 4f49 5d28 6874 7470 733a 2f2f 7a65  [DOI](https://ze
+00000900: 6e6f 646f 2e6f 7267 2f62 6164 6765 2f44  nodo.org/badge/D
+00000910: 4f49 2f31 302e 3532 3831 2f7a 656e 6f64  OI/10.5281/zenod
+00000920: 6f2e 3736 3632 3138 352e 7376 6729 5d28  o.7662185.svg)](
+00000930: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00000940: 3130 2e35 3238 312f 7a65 6e6f 646f 2e37  10.5281/zenodo.7
+00000950: 3636 3231 3835 290a 0a51 6962 6f63 616c  662185)..Qibocal
+00000960: 2070 726f 7669 6465 7320 5175 616e 7475   provides Quantu
+00000970: 6d20 4368 6172 6163 7465 7269 7a61 7469  m Characterizati
+00000980: 6f6e 2056 616c 6964 6174 696f 6e20 616e  on Validation an
+00000990: 6420 5665 7269 6669 6361 7469 6f6e 2070  d Verification p
+000009a0: 726f 746f 636f 6c73 2075 7369 6e67 205b  rotocols using [
+000009b0: 5169 626f 5d28 6874 7470 733a 2f2f 6769  Qibo](https://gi
+000009c0: 7468 7562 2e63 6f6d 2f71 6962 6f74 6561  thub.com/qibotea
+000009d0: 6d2f 7169 626f 2920 616e 6420 5b51 6962  m/qibo) and [Qib
+000009e0: 6f6c 6162 5d28 6874 7470 733a 2f2f 6769  olab](https://gi
+000009f0: 7468 7562 2e63 6f6d 2f71 6962 6f74 6561  thub.com/qibotea
+00000a00: 6d2f 7169 626f 6c61 6229 2e0a 0a51 6962  m/qibolab)...Qib
+00000a10: 6f63 616c 206b 6579 2066 6561 7475 7265  ocal key feature
+00000a20: 733a 0a0a 2d20 4175 746f 6d61 7469 7a61  s:..- Automatiza
+00000a30: 7469 6f6e 206f 6620 6361 6c69 6272 6174  tion of calibrat
+00000a40: 696f 6e20 726f 7574 696e 6573 2e0a 0a2d  ion routines...-
+00000a50: 2044 6563 6c61 7261 7469 7665 2069 6e70   Declarative inp
+00000a60: 7574 7320 7573 696e 6720 7275 6e63 6172  uts using runcar
+00000a70: 642e 0a0a 2d20 4765 6e65 7261 7469 6f6e  d...- Generation
+00000a80: 206f 6620 6120 7265 706f 7274 2e0a 0a23   of a report...#
+00000a90: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
+00000aa0: 5468 6520 7061 636b 6167 6520 6361 6e20  The package can 
+00000ab0: 6265 2069 6e73 7461 6c6c 6564 2062 7920  be installed by 
+00000ac0: 736f 7572 6365 3a0a 6060 6073 680a 6769  source:.```sh.gi
+00000ad0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000ae0: 6769 7468 7562 2e63 6f6d 2f71 6962 6f74  github.com/qibot
+00000af0: 6561 6d2f 7169 626f 6361 6c2e 6769 740a  eam/qibocal.git.
+00000b00: 6364 2071 6962 6f63 616c 0a70 6970 2069  cd qibocal.pip i
+00000b10: 6e73 7461 6c6c 202e 0a60 6060 0a0a 0a23  nstall ..```...#
+00000b20: 2323 2044 6576 656c 6f70 6572 2069 6e73  ## Developer ins
+00000b30: 7472 7563 7469 6f6e 730a 466f 7220 6465  tructions.For de
+00000b40: 7665 6c6f 706d 656e 7420 6d61 6b65 2073  velopment make s
+00000b50: 7572 6520 746f 2069 6e73 7461 6c6c 2074  ure to install t
+00000b60: 6865 2070 6163 6b61 6765 2075 7369 6e67  he package using
+00000b70: 205b 6070 6f65 7472 7960 5d28 6874 7470   [`poetry`](http
+00000b80: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
+00000b90: 792e 6f72 672f 2920 616e 6420 746f 2069  y.org/) and to i
+00000ba0: 6e73 7461 6c6c 2074 6865 2070 7265 2d63  nstall the pre-c
+00000bb0: 6f6d 6d69 7420 686f 6f6b 733a 0a60 6060  ommit hooks:.```
+00000bc0: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
+00000bd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000be0: 7169 626f 7465 616d 2f71 6962 6f63 616c  qiboteam/qibocal
+00000bf0: 2e67 6974 0a63 6420 7169 626f 6361 6c0a  .git.cd qibocal.
+00000c00: 706f 6574 7279 2069 6e73 7461 6c6c 0a70  poetry install.p
+00000c10: 7265 2d63 6f6d 6d69 7420 696e 7374 616c  re-commit instal
+00000c20: 6c0a 6060 600a 0a23 2320 4d69 6e69 6d61  l.```..## Minima
+00000c30: 6c20 776f 726b 696e 6720 6578 616d 706c  l working exampl
+00000c40: 650a 0a54 6869 7320 7365 6374 696f 6e20  e..This section 
+00000c50: 7368 6f77 7320 7468 6520 7374 6570 7320  shows the steps 
+00000c60: 746f 2070 6572 666f 726d 2061 2072 6573  to perform a res
+00000c70: 6f6e 6174 6f72 2073 7065 6374 726f 7363  onator spectrosc
+00000c80: 6f70 7920 7769 7468 2051 6962 6f63 616c  opy with Qibocal
+00000c90: 2e0a 2323 2320 5772 6974 6520 6120 7275  ..### Write a ru
+00000ca0: 6e63 6172 640a 4120 7275 6e63 6172 6420  ncard.A runcard 
+00000cb0: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
+00000cc0: 2065 7373 656e 7469 616c 2069 6e66 6f72   essential infor
+00000cd0: 6d61 7469 6f6e 2074 6f20 7275 6e20 6120  mation to run a 
+00000ce0: 7370 6563 6966 6963 2074 6173 6b2e 0a46  specific task..F
+00000cf0: 6f72 206f 7572 2070 7572 706f 7365 732c  or our purposes,
+00000d00: 2077 6520 6361 6e20 7573 6520 7468 6520   we can use the 
+00000d10: 666f 6c6c 6f77 696e 673a 0a60 6060 796d  following:.```ym
+00000d20: 6c0a 706c 6174 666f 726d 3a20 7469 6931  l.platform: tii1
+00000d30: 710a 0a71 7562 6974 733a 205b 305d 0a0a  q..qubits: [0]..
+00000d40: 666f 726d 6174 3a20 6373 760a 0a61 6374  format: csv..act
+00000d50: 696f 6e73 3a0a 2020 2072 6573 6f6e 6174  ions:.   resonat
+00000d60: 6f72 5f73 7065 6374 726f 7363 6f70 793a  or_spectroscopy:
+00000d70: 0a20 2020 2020 6c6f 7772 6573 5f77 6964  .     lowres_wid
+00000d80: 7468 3a20 355f 3030 305f 3030 300a 2020  th: 5_000_000.  
+00000d90: 2020 206c 6f77 7265 735f 7374 6570 3a20     lowres_step: 
+00000da0: 325f 3030 305f 3030 300a 2020 2020 2068  2_000_000.     h
+00000db0: 6967 6872 6573 5f77 6964 7468 3a20 315f  ighres_width: 1_
+00000dc0: 3530 305f 3030 300a 2020 2020 2068 6967  500_000.     hig
+00000dd0: 6872 6573 5f73 7465 703a 2032 3030 5f30  hres_step: 200_0
+00000de0: 3030 0a20 2020 2020 7072 6563 6973 696f  00.     precisio
+00000df0: 6e5f 7769 6474 683a 2031 5f35 3030 5f30  n_width: 1_500_0
+00000e00: 3030 0a20 2020 2020 7072 6563 6973 696f  00.     precisio
+00000e10: 6e5f 7374 6570 3a20 3130 305f 3030 300a  n_step: 100_000.
+00000e20: 2020 2020 2073 6f66 7477 6172 655f 6176       software_av
+00000e30: 6572 6167 6573 3a20 310a 2020 2020 2070  erages: 1.     p
+00000e40: 6f69 6e74 733a 2035 0a60 6060 0a23 2323  oints: 5.```.###
+00000e50: 2052 756e 2074 6865 2072 6f75 7469 6e65   Run the routine
+00000e60: 0a54 6f20 7275 6e20 616c 6c20 7468 6520  .To run all the 
+00000e70: 6361 6c69 6272 6174 696f 6e20 726f 7574  calibration rout
+00000e80: 696e 6573 2073 7065 6369 6669 6564 2069  ines specified i
+00000e90: 6e20 7468 6520 6060 6072 756e 6361 7264  n the ```runcard
+00000ea0: 6060 602c 2051 6962 6f63 616c 2075 7365  ```, Qibocal use
+00000eb0: 7320 7468 6520 6071 7160 2063 6f6d 6d61  s the `qq` comma
+00000ec0: 6e64 0a60 6060 7368 0a71 7120 3c72 756e  nd.```sh.qq <run
+00000ed0: 6361 7264 3e20 2d6f 203c 6f75 7470 7574  card> -o <output
+00000ee0: 5f66 6f6c 6465 723e 0a60 6060 0a69 6620  _folder>.```.if 
+00000ef0: 6060 603c 6f75 7470 7574 5f66 6f6c 6465  ```<output_folde
+00000f00: 723e 6060 6020 6973 2073 7065 6369 6669  r>``` is specifi
+00000f10: 6564 2c20 7468 6520 7265 7375 6c74 7320  ed, the results 
+00000f20: 7769 6c6c 2062 6520 7361 7665 6420 696e  will be saved in
+00000f30: 2069 742c 206f 7468 6572 7769 7365 2060   it, otherwise `
+00000f40: 6060 7171 6060 6020 7769 6c6c 2061 7574  ``qq``` will aut
+00000f50: 6f6d 6174 6963 616c 6c79 2063 7265 6174  omatically creat
+00000f60: 6520 6120 6465 6661 756c 7420 666f 6c64  e a default fold
+00000f70: 6572 2063 6f6e 7461 696e 696e 6720 7468  er containing th
+00000f80: 6520 6375 7272 656e 7420 6461 7465 2061  e current date a
+00000f90: 6e64 2074 6865 2075 7365 726e 616d 652e  nd the username.
+00000fa0: 0a0a 2323 2320 5669 7375 616c 697a 6520  ..### Visualize 
+00000fb0: 7468 6520 6461 7461 0a0a 5169 626f 6361  the data..Qiboca
+00000fc0: 6c20 6769 7665 7320 7468 6520 706f 7373  l gives the poss
+00000fd0: 6962 696c 6974 7920 746f 206c 6976 652d  ibility to live-
+00000fe0: 706c 6f74 7469 6e67 2077 6974 6820 7468  plotting with th
+00000ff0: 6520 6071 712d 6c69 7665 6020 636f 6d6d  e `qq-live` comm
+00001000: 616e 640a 6060 6073 680a 7171 2d6c 6976  and.```sh.qq-liv
+00001010: 6520 3c6f 7574 7075 745f 666f 6c64 6572  e <output_folder
+00001020: 3e0a 6060 600a 2323 2320 5570 6c6f 6164  >.```.### Upload
+00001030: 696e 6720 7265 706f 7274 7320 746f 2073  ing reports to s
+00001040: 6572 7665 720a 0a49 6e20 6f72 6465 7220  erver..In order 
+00001050: 746f 2075 706c 6f61 6420 7468 6520 7265  to upload the re
+00001060: 706f 7274 2074 6f20 6120 6365 6e74 7261  port to a centra
+00001070: 6c69 7a65 6420 7365 7276 6572 2c20 7365  lized server, se
+00001080: 6e64 2074 6f20 7468 6520 7365 7276 6572  nd to the server
+00001090: 2061 646d 696e 6973 7472 6174 6f72 7320   administrators 
+000010a0: 796f 7572 2070 7562 6c69 6320 7373 6820  your public ssh 
+000010b0: 6b65 7920 2866 726f 6d20 7468 6520 6d61  key (from the ma
+000010c0: 6368 696e 6528 7329 2079 6f75 2061 7265  chine(s) you are
+000010d0: 2070 6c61 6e6e 696e 6720 746f 2075 706c   planning to upl
+000010e0: 6f61 6420 7468 6520 7265 706f 7274 2920  oad the report) 
+000010f0: 616e 6420 7468 656e 2075 7365 2074 6865  and then use the
+00001100: 2060 7171 2d75 706c 6f61 6420 3c6f 7574   `qq-upload <out
+00001110: 7075 745f 666f 6c64 6572 3e60 2063 6f6d  put_folder>` com
+00001120: 6d61 6e64 2e20 5468 6973 2070 726f 6772  mand. This progr
+00001130: 616d 2077 696c 6c20 7570 6c6f 6164 2079  am will upload y
+00001140: 6f75 7220 7265 706f 7274 2074 6f20 7468  our report to th
+00001150: 6520 7365 7276 6572 2061 6e64 2067 656e  e server and gen
+00001160: 6572 6174 6520 616e 2075 6e69 7175 6520  erate an unique 
+00001170: 5552 4c2e 0a0a 2323 2043 6f6e 7472 6962  URL...## Contrib
+00001180: 7574 696e 670a 0a43 6f6e 7472 6962 7574  uting..Contribut
+00001190: 696f 6e73 2c20 6973 7375 6573 2061 6e64  ions, issues and
+000011a0: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
+000011b0: 7320 6172 6520 7765 6c63 6f6d 6521 0a46  s are welcome!.F
+000011c0: 6565 6c20 6672 6565 2074 6f20 6368 6563  eel free to chec
+000011d0: 6b0a 3c61 2068 7265 663d 2268 7474 7073  k.<a href="https
+000011e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7169  ://github.com/qi
+000011f0: 626f 7465 616d 2f71 6962 6f63 616c 2f69  boteam/qibocal/i
+00001200: 7373 7565 7322 3e3c 696d 6720 616c 743d  ssues"><img alt=
+00001210: 2247 6974 4875 6220 6973 7375 6573 2220  "GitHub issues" 
+00001220: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00001230: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00001240: 7562 2f69 7373 7565 732d 636c 6f73 6564  ub/issues-closed
+00001250: 2f71 6962 6f74 6561 6d2f 7169 626f 6361  /qiboteam/qiboca
+00001260: 6c22 2f3e 3c2f 613e 0a0a                 l"/></a>..
```

