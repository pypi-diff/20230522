# Comparing `tmp/physiofit-3.0.4.tar.gz` & `tmp/physiofit-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physiofit-3.0.4.tar", max compression
+gzip compressed data, was "physiofit-3.0.6.tar", max compression
```

## Comparing `physiofit-3.0.4.tar` & `physiofit-3.0.6.tar`

### file list

```diff
@@ -1,198 +1,34 @@
--rw-r--r--   0        0        0    35821 2022-11-29 10:25:21.371451 physiofit-3.0.4/LICENSE
--rw-r--r--   0        0        0       82 2023-02-01 14:58:37.438522 physiofit-3.0.4/physiofit/__init__.py
--rw-r--r--   0        0        0     1002 2023-02-01 14:58:37.440522 physiofit-3.0.4/physiofit/__main__.py
--rw-r--r--   0        0        0        0 2022-11-29 10:25:21.440048 physiofit-3.0.4/physiofit/base/__init__.py
--rw-r--r--   0        0        0      161 2022-11-30 16:31:31.859179 physiofit-3.0.4/physiofit/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    14169 2023-02-09 08:51:28.199278 physiofit-3.0.4/physiofit/base/__pycache__/fitter.cpython-39.pyc
--rw-r--r--   0        0        0    17360 2023-02-14 10:13:03.843325 physiofit-3.0.4/physiofit/base/__pycache__/io.cpython-39.pyc
--rw-r--r--   0        0        0    19509 2023-04-20 13:16:32.187271 physiofit-3.0.4/physiofit/base/fitter.py
--rw-r--r--   0        0        0    22770 2023-02-14 10:13:02.721663 physiofit-3.0.4/physiofit/base/io.py
--rw-r--r--   0        0        0      289 2023-04-18 08:44:18.750842 physiofit-3.0.4/physiofit/data/data_example.tsv
--rw-r--r--   0        0        0    22336 2023-02-01 13:49:50.075127 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/Ace.svg
--rw-r--r--   0        0        0      584 2023-02-01 13:49:50.720116 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/config_file.yml
--rw-r--r--   0        0        0      931 2023-02-01 13:49:49.903129 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/flux_results.tsv
--rw-r--r--   0        0        0    23387 2023-02-01 13:49:50.048128 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/Glc.svg
--rw-r--r--   0        0        0    16910 2023-02-01 13:49:50.717126 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/plots.pdf
--rw-r--r--   0        0        0      382 2023-02-01 13:49:49.907131 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/stat_results.tsv
--rw-r--r--   0        0        0    22911 2023-02-01 13:49:50.021129 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_1_res/X.svg
--rw-r--r--   0        0        0      764 2018-03-21 12:21:04.318182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_2.tsv
--rw-r--r--   0        0        0      765 2018-03-21 12:21:05.726182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_3.tsv
--rw-r--r--   0        0        0      752 2018-03-21 12:21:07.124182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_4.tsv
--rw-r--r--   0        0        0      738 2018-03-21 12:21:08.511182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_5.tsv
--rw-r--r--   0        0        0      761 2018-03-21 12:21:09.862182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_6.tsv
--rw-r--r--   0        0        0      754 2018-03-21 12:21:11.418182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_7.tsv
--rw-r--r--   0        0        0      766 2018-03-21 12:21:12.868182 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/KEIO_ROBOT6_8.tsv
--rw-r--r--   0        0        0     1183 2023-01-25 14:00:50.317662 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/KEIO_ROBOT_multiple.tsv
--rw-r--r--   0        0        0    12944 2023-01-25 15:16:24.069591 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Lindsay_test.tsv
--rw-r--r--   0        0        0    39193 2023-01-13 14:54:11.449831 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Lindsay_test.xlsx
--rw-r--r--   0        0        0      771 2023-01-17 09:22:17.441749 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Lindsay_test_unique.tsv
--rw-r--r--   0        0        0    25021 2023-01-30 15:32:42.796621 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Alanine.svg
--rw-r--r--   0        0        0     1872 2023-01-30 15:31:30.200123 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/config_file.yml
--rw-r--r--   0        0        0    26542 2023-01-30 15:32:42.825618 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Ethanol.svg
--rw-r--r--   0        0        0     3729 2023-01-30 15:32:42.375687 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/flux_results.tsv
--rw-r--r--   0        0        0    26951 2023-01-30 15:32:42.856632 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Glucose.svg
--rw-r--r--   0        0        0    25723 2023-01-30 15:32:42.885621 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Glutamine.svg
--rw-r--r--   0        0        0    27987 2023-01-30 15:32:42.915630 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Isoleucine.svg
--rw-r--r--   0        0        0    25309 2023-01-30 15:32:42.945620 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Lactate.svg
--rw-r--r--   0        0        0    25539 2023-01-30 15:32:42.975620 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Leucine.svg
--rw-r--r--   0        0        0    27171 2023-01-30 15:32:43.045619 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Methionine.svg
--rw-r--r--   0        0        0    29132 2023-01-30 15:32:43.076801 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Phenylalanine.svg
--rw-r--r--   0        0        0    43219 2023-01-30 15:31:30.195122 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/plots.pdf
--rw-r--r--   0        0        0    28319 2023-01-30 15:32:43.106711 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Pyruvate.svg
--rw-r--r--   0        0        0      382 2023-01-30 15:32:42.378685 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/stat_results.tsv
--rw-r--r--   0        0        0    26868 2023-01-30 15:32:43.137710 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Threonine.svg
--rw-r--r--   0        0        0    27106 2023-01-30 15:32:43.375799 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Tyrosine.svg
--rw-r--r--   0        0        0    24137 2023-01-30 15:32:43.402799 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/Valine.svg
--rw-r--r--   0        0        0    24115 2023-01-30 15:32:42.769621 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_1/X.svg
--rw-r--r--   0        0        0    27297 2023-01-30 15:32:13.615715 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Alanine.svg
--rw-r--r--   0        0        0    26452 2023-01-30 15:32:13.708739 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Ethanol.svg
--rw-r--r--   0        0        0     3651 2023-01-30 15:32:09.185716 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/flux_results.tsv
--rw-r--r--   0        0        0    26952 2023-01-30 15:32:13.767797 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Glucose.svg
--rw-r--r--   0        0        0    28005 2023-01-30 15:32:13.827789 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Glutamine.svg
--rw-r--r--   0        0        0    26356 2023-01-30 15:32:13.893737 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Isoleucine.svg
--rw-r--r--   0        0        0    25320 2023-01-30 15:32:13.951791 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Lactate.svg
--rw-r--r--   0        0        0    25552 2023-01-30 15:32:14.009748 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Leucine.svg
--rw-r--r--   0        0        0    27175 2023-01-30 15:32:14.079701 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Methionine.svg
--rw-r--r--   0        0        0    29177 2023-01-30 15:32:14.146701 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Phenylalanine.svg
--rw-r--r--   0        0        0    27496 2023-01-30 15:32:14.214789 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Pyruvate.svg
--rw-r--r--   0        0        0      387 2023-01-30 15:32:09.190750 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/stat_results.tsv
--rw-r--r--   0        0        0    27806 2023-01-30 15:32:14.284703 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Threonine.svg
--rw-r--r--   0        0        0    27107 2023-01-30 15:32:14.350716 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Tyrosine.svg
--rw-r--r--   0        0        0    24681 2023-01-30 15:32:14.411735 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/Valine.svg
--rw-r--r--   0        0        0    24118 2023-01-30 15:32:13.521796 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/P53cKO_2/X.svg
--rw-r--r--   0        0        0    24269 2023-01-30 15:33:11.010310 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Alanine.svg
--rw-r--r--   0        0        0     1871 2023-01-30 15:32:17.611786 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/config_file.yml
--rw-r--r--   0        0        0    24124 2023-01-30 15:33:11.038310 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Ethanol.svg
--rw-r--r--   0        0        0     3934 2023-01-30 15:33:10.596214 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/flux_results.tsv
--rw-r--r--   0        0        0    25846 2023-01-30 15:33:11.067225 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Glucose.svg
--rw-r--r--   0        0        0    26904 2023-01-30 15:33:11.096225 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Glutamine.svg
--rw-r--r--   0        0        0    25255 2023-01-30 15:33:11.124215 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Isoleucine.svg
--rw-r--r--   0        0        0    22371 2023-01-30 15:33:11.151338 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Lactate.svg
--rw-r--r--   0        0        0    24444 2023-01-30 15:33:11.181210 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Leucine.svg
--rw-r--r--   0        0        0    23915 2023-01-30 15:33:11.208229 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Methionine.svg
--rw-r--r--   0        0        0    26158 2023-01-30 15:33:11.238228 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Phenylalanine.svg
--rw-r--r--   0        0        0    42004 2023-01-30 15:32:17.605793 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/plots.pdf
--rw-r--r--   0        0        0    25551 2023-01-30 15:33:11.268342 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Pyruvate.svg
--rw-r--r--   0        0        0      387 2023-01-30 15:33:10.599213 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/stat_results.tsv
--rw-r--r--   0        0        0    25822 2023-01-30 15:33:11.298248 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Threonine.svg
--rw-r--r--   0        0        0    24576 2023-01-30 15:33:11.327313 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Tyrosine.svg
--rw-r--r--   0        0        0    25225 2023-01-30 15:33:11.356342 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/Valine.svg
--rw-r--r--   0        0        0    24640 2023-01-30 15:33:10.982309 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_1/X.svg
--rw-r--r--   0        0        0    26361 2023-01-30 15:32:28.820724 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Alanine.svg
--rw-r--r--   0        0        0     1871 2023-01-30 15:32:32.204715 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/config_file.yml
--rw-r--r--   0        0        0    24825 2023-01-30 15:32:28.850427 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Ethanol.svg
--rw-r--r--   0        0        0     3681 2023-01-30 15:32:28.394745 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/flux_results.tsv
--rw-r--r--   0        0        0    24768 2023-01-30 15:32:28.879427 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Glucose.svg
--rw-r--r--   0        0        0    26404 2023-01-30 15:32:28.908427 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Glutamine.svg
--rw-r--r--   0        0        0    26721 2023-01-30 15:32:28.936426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Isoleucine.svg
--rw-r--r--   0        0        0    22746 2023-01-30 15:32:28.963426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Lactate.svg
--rw-r--r--   0        0        0    25423 2023-01-30 15:32:28.991426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Leucine.svg
--rw-r--r--   0        0        0    24902 2023-01-30 15:32:29.020426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Methionine.svg
--rw-r--r--   0        0        0    27343 2023-01-30 15:32:29.049426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Phenylalanine.svg
--rw-r--r--   0        0        0    41848 2023-01-30 15:32:32.198716 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/plots.pdf
--rw-r--r--   0        0        0    24849 2023-01-30 15:32:29.077426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Pyruvate.svg
--rw-r--r--   0        0        0      382 2023-01-30 15:32:28.398697 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/stat_results.tsv
--rw-r--r--   0        0        0    25175 2023-01-30 15:32:29.106426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Threonine.svg
--rw-r--r--   0        0        0    24785 2023-01-30 15:32:29.133426 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Tyrosine.svg
--rw-r--r--   0        0        0    25229 2023-01-30 15:32:29.171425 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/Valine.svg
--rw-r--r--   0        0        0    24132 2023-01-30 15:32:28.790746 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOT6_1/Multiple_Conds_Test/Multiple_Conds_Test_res/WT_5/X.svg
--rw-r--r--   0        0        0     7871 2023-01-25 15:47:49.445918 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all.tsv
--rw-r--r--   0        0        0    24467 2023-04-13 09:49:54.149282 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:49:55.923204 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/config_file.yml
--rw-r--r--   0        0        0      762 2023-04-13 09:49:53.627776 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/flux_results.tsv
--rw-r--r--   0        0        0    24751 2023-04-13 09:49:54.080178 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/Glc.svg
--rw-r--r--   0        0        0    18264 2023-04-13 09:49:55.852410 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/plots.pdf
--rw-r--r--   0        0        0      375 2023-04-13 09:49:53.638242 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/stat_results.tsv
--rw-r--r--   0        0        0    24983 2023-04-13 09:49:53.994579 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_1/X.svg
--rw-r--r--   0        0        0    24466 2023-04-13 09:50:01.795547 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:03.681370 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/config_file.yml
--rw-r--r--   0        0        0      776 2023-04-13 09:50:01.452003 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/flux_results.tsv
--rw-r--r--   0        0        0    24749 2023-04-13 09:50:01.746685 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/Glc.svg
--rw-r--r--   0        0        0    18302 2023-04-13 09:50:03.251832 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/plots.pdf
--rw-r--r--   0        0        0      374 2023-04-13 09:50:01.461306 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/stat_results.tsv
--rw-r--r--   0        0        0    25446 2023-04-13 09:50:01.700544 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_2/X.svg
--rw-r--r--   0        0        0    24469 2023-04-13 09:50:08.370779 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:09.870561 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/config_file.yml
--rw-r--r--   0        0        0      764 2023-04-13 09:50:07.980393 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/flux_results.tsv
--rw-r--r--   0        0        0    24755 2023-04-13 09:50:08.302410 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/Glc.svg
--rw-r--r--   0        0        0    18289 2023-04-13 09:50:09.862559 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/plots.pdf
--rw-r--r--   0        0        0      373 2023-04-13 09:50:07.990877 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/stat_results.tsv
--rw-r--r--   0        0        0    24951 2023-04-13 09:50:08.240795 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_3/X.svg
--rw-r--r--   0        0        0    22339 2023-04-13 09:50:15.982090 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:17.432734 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/config_file.yml
--rw-r--r--   0        0        0      776 2023-04-13 09:50:15.685783 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/flux_results.tsv
--rw-r--r--   0        0        0    24753 2023-04-13 09:50:15.935228 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/Glc.svg
--rw-r--r--   0        0        0    18214 2023-04-13 09:50:17.426620 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/plots.pdf
--rw-r--r--   0        0        0      375 2023-04-13 09:50:15.695034 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/stat_results.tsv
--rw-r--r--   0        0        0    25444 2023-04-13 09:50:15.877111 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_4/X.svg
--rw-r--r--   0        0        0    24472 2023-04-13 09:50:22.854713 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:24.244858 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/config_file.yml
--rw-r--r--   0        0        0      774 2023-04-13 09:50:22.360436 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/flux_results.tsv
--rw-r--r--   0        0        0    24760 2023-04-13 09:50:22.788809 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/Glc.svg
--rw-r--r--   0        0        0    18311 2023-04-13 09:50:24.237858 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/plots.pdf
--rw-r--r--   0        0        0      374 2023-04-13 09:50:22.370716 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/stat_results.tsv
--rw-r--r--   0        0        0    25446 2023-04-13 09:50:22.726135 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_5/X.svg
--rw-r--r--   0        0        0    24472 2023-04-13 09:50:29.356681 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:30.783268 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/config_file.yml
--rw-r--r--   0        0        0      775 2023-04-13 09:50:28.866853 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/flux_results.tsv
--rw-r--r--   0        0        0    24754 2023-04-13 09:50:29.286510 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/Glc.svg
--rw-r--r--   0        0        0    18307 2023-04-13 09:50:30.774981 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/plots.pdf
--rw-r--r--   0        0        0      374 2023-04-13 09:50:28.876119 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/stat_results.tsv
--rw-r--r--   0        0        0    25447 2023-04-13 09:50:29.198368 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_6/X.svg
--rw-r--r--   0        0        0    24464 2023-04-13 09:50:36.190955 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:37.654052 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/config_file.yml
--rw-r--r--   0        0        0      768 2023-04-13 09:50:35.715161 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/flux_results.tsv
--rw-r--r--   0        0        0    24714 2023-04-13 09:50:36.130812 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/Glc.svg
--rw-r--r--   0        0        0    17285 2023-04-13 09:50:37.646886 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/plots.pdf
--rw-r--r--   0        0        0      375 2023-04-13 09:50:35.725375 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/stat_results.tsv
--rw-r--r--   0        0        0    22881 2023-04-13 09:50:36.071033 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_7/X.svg
--rw-r--r--   0        0        0    24464 2023-04-13 09:50:44.355834 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/Ace.svg
--rw-r--r--   0        0        0      474 2023-04-13 09:50:46.061901 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/config_file.yml
--rw-r--r--   0        0        0      776 2023-04-13 09:50:43.913737 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/flux_results.tsv
--rw-r--r--   0        0        0    24719 2023-04-13 09:50:44.284134 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/Glc.svg
--rw-r--r--   0        0        0    17383 2023-04-13 09:50:46.054783 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/plots.pdf
--rw-r--r--   0        0        0      375 2023-04-13 09:50:43.923058 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/stat_results.tsv
--rw-r--r--   0        0        0    23867 2023-04-13 09:50:44.222875 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/KEIO_ROBOT_6_8/X.svg
--rw-r--r--   0        0        0     6611 2023-04-13 09:50:46.070035 physiofit-3.0.4/physiofit/data/KEIO_test_data/KEIO_ROBOTS_all/KEIO_ROBOTS_all_res/recap.csv
--rw-r--r--   0        0        0      397 2023-02-13 15:43:01.367237 physiofit-3.0.4/physiofit/data/KEIO_test_data/ode_test/KEIO_ROBOT6_1.tsv
--rw-r--r--   0        0        0      470 2023-01-31 11:06:34.673766 physiofit-3.0.4/physiofit/data/yaml_test/config_file.yml
--rw-r--r--   0        0        0      389 2023-03-09 10:14:14.790040 physiofit-3.0.4/physiofit/example_yaml.yml
--rw-r--r--   0        0        0        0 2023-02-01 14:58:37.464523 physiofit-3.0.4/physiofit/models/__init__.py
--rw-r--r--   0        0        0      182 2023-04-18 08:44:18.165843 physiofit-3.0.4/physiofit/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      163 2023-02-01 14:59:03.907410 physiofit-3.0.4/physiofit/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6252 2023-04-18 08:44:18.172841 physiofit-3.0.4/physiofit/models/__pycache__/base_model.cpython-310.pyc
--rw-r--r--   0        0        0     6172 2023-02-01 14:59:03.911431 physiofit-3.0.4/physiofit/models/__pycache__/base_model.cpython-39.pyc
--rw-r--r--   0        0        0     2831 2023-04-18 08:44:18.175840 physiofit-3.0.4/physiofit/models/__pycache__/model_1.cpython-310.pyc
--rw-r--r--   0        0        0     2768 2023-04-18 08:58:53.071930 physiofit-3.0.4/physiofit/models/__pycache__/model_1.cpython-39.pyc
--rw-r--r--   0        0        0     2126 2023-04-18 08:44:18.180844 physiofit-3.0.4/physiofit/models/__pycache__/model_2.cpython-310.pyc
--rw-r--r--   0        0        0     2073 2023-04-18 08:58:53.078928 physiofit-3.0.4/physiofit/models/__pycache__/model_2.cpython-39.pyc
--rw-r--r--   0        0        0     2417 2023-04-18 08:44:18.183841 physiofit-3.0.4/physiofit/models/__pycache__/model_3.cpython-310.pyc
--rw-r--r--   0        0        0     2378 2023-04-18 08:58:53.085929 physiofit-3.0.4/physiofit/models/__pycache__/model_3.cpython-39.pyc
--rw-r--r--   0        0        0     1817 2023-04-18 08:44:18.188841 physiofit-3.0.4/physiofit/models/__pycache__/model_4.cpython-310.pyc
--rw-r--r--   0        0        0     1764 2023-04-18 08:58:53.092927 physiofit-3.0.4/physiofit/models/__pycache__/model_4.cpython-39.pyc
--rw-r--r--   0        0        0     3188 2023-04-18 08:44:18.194842 physiofit-3.0.4/physiofit/models/__pycache__/model_5.cpython-310.pyc
--rw-r--r--   0        0        0     3125 2023-04-18 08:58:53.098944 physiofit-3.0.4/physiofit/models/__pycache__/model_5.cpython-39.pyc
--rw-r--r--   0        0        0     3196 2023-04-18 08:44:18.196843 physiofit-3.0.4/physiofit/models/__pycache__/model_6.cpython-310.pyc
--rw-r--r--   0        0        0     6423 2023-02-01 14:58:37.465522 physiofit-3.0.4/physiofit/models/base_model.py
--rw-r--r--   0        0        0     3323 2023-04-18 08:44:18.203845 physiofit-3.0.4/physiofit/models/model_1.py
--rw-r--r--   0        0        0     2645 2023-04-18 08:44:18.211840 physiofit-3.0.4/physiofit/models/model_2.py
--rw-r--r--   0        0        0     2427 2023-04-18 08:44:18.218845 physiofit-3.0.4/physiofit/models/model_3.py
--rw-r--r--   0        0        0     1876 2023-04-18 08:44:18.226844 physiofit-3.0.4/physiofit/models/model_4.py
--rw-r--r--   0        0        0     4152 2023-04-18 08:44:18.233867 physiofit-3.0.4/physiofit/models/model_5.py
--rw-r--r--   0        0        0      113 2023-02-01 14:58:37.479523 physiofit-3.0.4/physiofit/models/template.py
--rw-r--r--   0        0        0        0 2022-11-29 10:25:21.440048 physiofit-3.0.4/physiofit/tests/__init__.py
--rw-r--r--   0        0        0      162 2023-04-18 08:54:16.321541 physiofit-3.0.4/physiofit/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2023-04-18 09:01:57.707951 physiofit-3.0.4/physiofit/tests/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1838 2023-04-18 09:01:59.335013 physiofit-3.0.4/physiofit/tests/__pycache__/test_fitter.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      701 2023-04-18 09:01:49.684145 physiofit-3.0.4/physiofit/tests/conftest.py
--rw-r--r--   0        0        0      697 2023-04-18 09:11:25.010201 physiofit-3.0.4/physiofit/tests/test_fitter.py
--rw-r--r--   0        0        0        0 2022-11-29 10:25:21.440048 physiofit-3.0.4/physiofit/ui/__init__.py
--rw-r--r--   0        0        0      159 2022-11-30 16:31:31.843638 physiofit-3.0.4/physiofit/ui/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5084 2023-02-01 14:59:02.295516 physiofit-3.0.4/physiofit/ui/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0        0        0    13526 2023-03-09 08:43:00.438611 physiofit-3.0.4/physiofit/ui/__pycache__/gui.cpython-39.pyc
--rw-r--r--   0        0        0     6704 2023-02-01 14:58:37.485521 physiofit-3.0.4/physiofit/ui/cli.py
--rw-r--r--   0        0        0    24811 2023-04-18 08:44:18.242842 physiofit-3.0.4/physiofit/ui/gui.py
--rw-r--r--   0        0        0      875 2023-05-12 08:48:26.921779 physiofit-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     3668 2023-03-13 10:44:58.031633 physiofit-3.0.4/README.md
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 physiofit-3.0.4/setup.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 physiofit-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-05-22 08:54:39.415783 physiofit-3.0.6/LICENSE
+-rw-r--r--   0        0        0     3577 2023-05-22 08:54:39.415783 physiofit-3.0.6/README.md
+-rw-r--r--   0        0        0       80 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/__init__.py
+-rw-r--r--   0        0        0      966 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/__init__.py
+-rw-r--r--   0        0        0    18990 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/fitter.py
+-rw-r--r--   0        0        0    22161 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/base/io.py
+-rw-r--r--   0        0        0      272 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/data/data_example.tsv
+-rw-r--r--   0        0        0      366 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/example_yaml.yml
+-rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6252 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/base_model.cpython-310.pyc
+-rw-r--r--   0        0        0     2831 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2126 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_2.cpython-310.pyc
+-rw-r--r--   0        0        0     2417 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_3.cpython-310.pyc
+-rw-r--r--   0        0        0     1817 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_4.cpython-310.pyc
+-rw-r--r--   0        0        0     3188 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_5.cpython-310.pyc
+-rw-r--r--   0        0        0     3196 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/__pycache__/model_6.cpython-310.pyc
+-rw-r--r--   0        0        0     6220 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/base_model.py
+-rw-r--r--   0        0        0     3218 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_1.py
+-rw-r--r--   0        0        0     2558 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_2.py
+-rw-r--r--   0        0        0     2346 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_3.py
+-rw-r--r--   0        0        0     1811 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_4.py
+-rw-r--r--   0        0        0     4012 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/model_5.py
+-rw-r--r--   0        0        0      101 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/models/template.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/__init__.py
+-rw-r--r--   0        0        0     1670 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/conftest.py
+-rw-r--r--   0        0        0     3252 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/tests/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/__init__.py
+-rw-r--r--   0        0        0     6499 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/cli.py
+-rw-r--r--   0        0        0    24255 2023-05-22 08:54:39.419783 physiofit-3.0.6/physiofit/ui/gui.py
+-rw-r--r--   0        0        0      854 2023-05-22 08:54:39.423783 physiofit-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 physiofit-3.0.6/setup.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 physiofit-3.0.6/PKG-INFO
```

### Comparing `physiofit-3.0.4/LICENSE` & `physiofit-3.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `physiofit-3.0.4/physiofit/__main__.py` & `physiofit-3.0.6/physiofit/__main__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from subprocess import run
-import sys
-from pathlib import Path
-
-from threading import Thread
-import requests
-
-import physiofit
-import physiofit.ui.cli
-
-
-def get_last_version():
-    """Get last Physiofit version."""
-    try:
-        pf_path = Path(physiofit.__file__).parent
-        # Get the version from pypi
-        response = requests.get(f'https://pypi.org/pypi/physiofit/json')
-        latest_version = response.json()['info']['version']
-        with open(str(Path(pf_path, "last_version.txt")), "w") as f:
-            f.write(latest_version)
-    except Exception:
-        pass
-
-def main():
-    """The main routine"""
-
-    if len(sys.argv) > 1:
-        physiofit.ui.cli.main()
-    else:
-        thread = Thread(target=get_last_version)
-        thread.start()
-        path_to_app = Path(physiofit.__file__).parent
-        path_to_app = path_to_app / "ui/gui.py"
-        run(["streamlit", "run", str(path_to_app)])
-
-if __name__ == "__main__":
+from subprocess import run
+import sys
+from pathlib import Path
+
+from threading import Thread
+import requests
+
+import physiofit
+import physiofit.ui.cli
+
+
+def get_last_version():
+    """Get last Physiofit version."""
+    try:
+        pf_path = Path(physiofit.__file__).parent
+        # Get the version from pypi
+        response = requests.get(f'https://pypi.org/pypi/physiofit/json')
+        latest_version = response.json()['info']['version']
+        with open(str(Path(pf_path, "last_version.txt")), "w") as f:
+            f.write(latest_version)
+    except Exception:
+        pass
+
+def main():
+    """The main routine"""
+
+    if len(sys.argv) > 1:
+        physiofit.ui.cli.main()
+    else:
+        thread = Thread(target=get_last_version)
+        thread.start()
+        path_to_app = Path(physiofit.__file__).parent
+        path_to_app = path_to_app / "ui/gui.py"
+        run(["streamlit", "run", str(path_to_app)])
+
+if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `physiofit-3.0.4/physiofit/base/fitter.py` & `physiofit-3.0.6/physiofit/base/fitter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,519 +1,519 @@
-"""
-PhysioFit software main module
-"""
-
-import logging
-
-import numpy as np
-from pandas import DataFrame
-from scipy.optimize import minimize, differential_evolution
-from scipy.stats import chi2
-
-from physiofit.models.base_model import Model
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
-
-
-# TODO: add estimate deg function (eq 6) with plot of best fit and measured values
-
-
-class PhysioFitter:
-    """
-    This class is responsible for most of Physiofit's heavy lifting. Features included are:
-
-        * loading of data from **csv** or **tsv** file
-        * **equation system initialization** using the following analytical functions (in absence of lag and
-          degradation:
-
-            X(t) = X0 * exp(mu * t)
-            Mi(t) = qMi * (X0 / mu) * (exp(mu * t) - 1) + Mi0
-
-        * **simulation of data points** from given initial parameters
-        * **cost calculation** using the equation:
-
-            residuum = sum((sim - meas) / sd)²
-
-        * **optimization of the initial parameters** using `scipy.optimize.minimize ('Differential evolution', with polish with 'L-BFGS-B' method) <https://docs.scipy.org/doc/scipy/reference/optimize.minimize-lbfgsb.html#optimize-minimize-lbfgsb>`_
-        * **sensitivity analysis, khi2 tests and plotting**
-
-    :param data: DataFrame containing data and passed by IOstream object
-    :type data: class: pandas.DataFrame
-    :param model: Model to initialize parameters and optimize
-    :type model: physiofit.models.base_model.Model
-    :param mc: Should Monte-Carlo sensitivity analysis be performed (default=True)
-    :type mc: Boolean
-    :param iterations: number of iterations for Monte-Carlo simulation (default=50)
-    :type iterations: int
-    :param sd: sd matrix used for residuum calculations. Can be:
-
-                * a matrix with the same dimensions as the measurements matrix (but without the time column)
-                * a named vector containing sds for all the metabolites provided in the input file
-                * 0  in which case the matrix is automatically constructed from default values
-                * a dictionary with the data column headers as keys and the associated value as a scalar or list
-
-    :type sd: int, float, list, dict or ndarray
-    """
-
-    def __init__(
-            self,
-            data,
-            model,
-            mc=True,
-            iterations=100,
-            sd=None,
-            debug_mode=False
-    ):
-
-        self.data = data
-        self.model = model
-        self.mc = mc
-        self.iterations = iterations
-        self.sd = sd
-        self.debug_mode = debug_mode
-        self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
-
-        self.simulated_matrix = None
-        self.simulated_data = None
-        self.optimize_results = None
-        self.simulate = None
-        self.parameter_stats = None
-        self.opt_params_sds = None
-        self.matrices_ci = None
-        self.opt_conf_ints = None
-        self.khi2_res = None
-
-    def verify_attrs(self):
-        """Check that attributes are valid"""
-
-        if type(self.iterations) is not int:
-            raise TypeError(
-                f"Number of monte carlo iterations must be an "
-                f"integer, and not of type {type(self.iterations)}"
-            )
-
-        allowed_sds = [int, float, list, np.ndarray]
-        if type(self.sd) not in allowed_sds:
-            raise TypeError(
-                f"sds is not in the right format ({type(self.sd)}. "
-                f"Compatible formats are:\n{allowed_sds}"
-            )
-
-    def _sd_dict_to_matrix(self):
-        """Convert sd dictionary to matrix/vector"""
-
-        logger.debug("Initializing sd matrix from dict")
-        # Perform checks
-        for key in self.sd.keys():
-            if key not in self.model.name_vector:
-                raise KeyError(
-                    f"The key {key} is not part of the data headers"
-                )
-        for name in self.model.name_vector:
-            if name not in self.sd.keys():
-                raise KeyError(
-                    f"The key {name} is missing from the sds dict"
-                )
-
-        # Get lengths of each sd entry
-        sd_lengths = [
-            len(self.sd[key]) if type(self.sd[key]) not in [float, int] else 1
-            for key in self.sd.keys()
-        ]
-
-        # Make sure that lengths are the same
-        if not all(elem == sd_lengths[0] for elem in sd_lengths):
-            raise ValueError("All sd vectors must have the same length")
-
-        # Build matrix/vector
-        if sd_lengths[0] == 1:
-            self.sd = [self.sd[name] for name in self.model.name_vector]
-        else:
-            columns = (self.sd[name] for name in self.model.name_vector)
-            matrix = np.column_stack(columns)
-            self.sd = matrix
-
-        logger.debug(f"SD object type: {type(self.sd)}")
-        logger.debug(f"Array built from dict:\n{self.sd}")
-
-    def initialize_sd_matrix(self):
-        """
-        Initialize the sd matrix from different types of inputs: single value,
-        vector or matrix.
-
-        :return: None
-        """
-
-        # This function can be optimized, if the input is a matrix we should
-        # detect it directly
-        logger.info("Initializing sd matrix...\n")
-
-        # If sd is None, we generate the default matrix
-        if self.sd is None or self.sd == {}:
-            try:
-                self.sd = {"X": 0.2}
-                for col in self.data.columns[2:]:
-                    self.sd.update({col: 0.5})
-            except Exception:
-                raise
-
-        if isinstance(self.sd, dict):
-            self._sd_dict_to_matrix()
-        # When sd is a single value, we build a sd matrix containing the value
-        # in all positions
-        if isinstance(self.sd, int) or isinstance(self.sd, float):
-            self._build_sd_matrix()
-            logger.debug(f"SD matrix: {self.sd}\n")
-            return
-        if not isinstance(self.sd, np.ndarray) and not isinstance(self.sd,
-                                                                  list):
-            raise TypeError(
-                f"Cannot coerce SD to array. Please check that a list or array "
-                f"is given as input.\nCurrent input: \n{self.sd}"
-            )
-        else:
-            self.sd = np.array(self.sd)
-        if not np.issubdtype(self.sd.dtype, np.number):
-            try:
-                self.sd = self.sd.astype(float)
-            except ValueError:
-                raise ValueError(
-                    f"The sd vector/matrix contains values that are not "
-                    f"numeric. \nCurrent sd vector/matrix: \n{self.sd}"
-                )
-            except Exception as e:
-                raise RuntimeError(f"Unknown error: {e}")
-        else:
-            # If the array is not the right shape, we assume it is a vector
-            # that needs to be tiled into a matrix
-
-            logger.debug(f"SD matrix: {self.sd}\n")
-            logger.debug(f"Type of SD matrix: {type(self.sd)}")
-
-            if self.sd.shape != self.experimental_matrix.shape:
-                try:
-                    self._build_sd_matrix()
-                except ValueError:
-                    raise
-                except RuntimeError:
-                    raise
-            else:
-                logger.debug(f"sd matrix: {self.sd}\n")
-                return
-        logger.info(f"sd Matrix:\n{self.sd}\n")
-
-    def _build_sd_matrix(self):
-        """
-        Build the sd matrix from different input types
-
-        :return: None
-        """
-
-        # First condition: the sds are in a 1D array
-        if isinstance(self.sd, np.ndarray):
-            # We first check that the sd vector is as long as the
-            # experimental matrix on the row axis
-            if self.sd.size != self.experimental_matrix[0].size:
-                raise ValueError("sd vector not of right size")
-            else:
-                # We duplicate the vector column-wise to build a matrix of
-                # duplicated sd vectors
-                self.sd = np.tile(self.sd, (len(self.experimental_matrix), 1))
-
-        # Second condition: the sd is a scalar and must be broadcast to a
-        # matrix with same shape as the data
-        elif isinstance(self.sd, int) or isinstance(self.sd, float):
-            self.sd = np.full(self.experimental_matrix.shape, self.sd)
-        else:
-            raise RuntimeError("Unknown error")
-
-    def _get_default_sds(self):
-        """
-        Build a default sd matrix. Default values:
-            * Biomass: 0.2
-            * Metabolites: 0.5
-        :return: None
-        """
-
-        sds = [0.2]
-        for name in range(len(self.model.name_vector) - 1):
-            sds.append(0.5)
-        self.sd = np.array(sds)
-        self._build_sd_matrix()
-
-    def optimize(self):
-        """
-        Run optimization and build the simulated matrix
-        from the optimized parameters
-        """
-
-        logger.info("\nRunning optimization...\n")
-        bounds = self.model.bounds()
-        parameters = [param for param in self.model.parameters_to_estimate.values()]
-        logger.debug(f"Simulate function = {self.model.simulate}")
-        self.optimize_results = self._run_optimization(
-            params=parameters,
-            func=self.model.simulate,
-            exp_data_matrix=self.experimental_matrix,
-            time_vector=self.model.time_vector,
-            non_opt_params=self.model.fixed_parameters,
-            sd_matrix=self.sd,
-            bounds=bounds,
-            method="differential_evolution"
-        )
-        self.parameter_stats = {
-            "optimal": self.optimize_results.x
-        }
-        logger.info(f"Optimization results: \n{self.optimize_results}\n")
-        for i, param in zip(
-                self.model.parameters_to_estimate, self.optimize_results.x
-        ):
-            logger.info(f"\n{i} = {param}\n")
-        self.simulated_matrix = self.model.simulate(
-            self.optimize_results.x,
-            self.experimental_matrix,
-            self.model.time_vector,
-            self.model.fixed_parameters
-        )
-        logger.debug(f"simulated_matrix:\n{self.simulated_matrix}")
-        nan_sim_mat = np.copy(self.simulated_matrix)
-        nan_sim_mat[np.isnan(self.experimental_matrix)] = np.nan
-        self.simulated_data = DataFrame(
-            data=nan_sim_mat,
-            index=self.model.time_vector,
-            columns=self.model.name_vector
-        )
-        self.simulated_data.index.name = "Time"
-        logger.info(f"Final Simulated Data: \n{self.simulated_data}\n")
-
-    @staticmethod
-    def _calculate_cost(
-            params, func, exp_data_matrix, time_vector, non_opt_params,
-            sd_matrix
-    ):
-        """
-        Calculate the cost (residue) using the square of
-        simulated-experimental over the SDs
-        """
-
-        simulated_matrix = func(params, exp_data_matrix, time_vector,
-                                non_opt_params)
-        cost_val = np.square((simulated_matrix - exp_data_matrix) / sd_matrix)
-        residuum = np.nansum(cost_val)
-        return residuum
-
-    @staticmethod
-    def _run_optimization(
-            params: list,
-            func: Model.simulate,
-            exp_data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            non_opt_params: dict,
-            sd_matrix: np.ndarray,
-            bounds: tuple,
-            method: str
-    ):
-        """
-        Run the optimization on input parameters using the cost function and
-        Scipy minimize (L-BFGS-B method that is deterministic and uses the
-        gradient method for optimizing)
-        """
-
-        if method == "differential_evolution":
-            logger.debug(f"Optimization method = {method}")
-            optimize_results = differential_evolution(
-                PhysioFitter._calculate_cost, bounds=bounds,
-                args=(
-                func, exp_data_matrix, time_vector, non_opt_params, sd_matrix),
-                polish=True, x0=np.array(params)
-            )
-        elif method == "L-BFGS-B":
-            logger.debug(f"Optimization method = {method}")
-            optimize_results = minimize(
-                PhysioFitter._calculate_cost, x0=np.array(params),
-                args=(
-                func, exp_data_matrix, time_vector, non_opt_params, sd_matrix),
-                method="L-BFGS-B", bounds=bounds, options={'maxcor': 30}
-            )
-        else:
-            raise ValueError(f"{method} is not implemented")
-
-        return optimize_results
-
-    def monte_carlo_analysis(self):
-        """
-        Run a monte carlo analysis to calculate optimization standard
-        deviations on parameters and simulated data points
-        """
-
-        if not self.optimize_results:
-            raise RuntimeError(
-                "Running Monte Carlo simulation without having run the "
-                "optimization is impossible as best fit results are needed to "
-                "generate the initial simulated matrix"
-            )
-
-        logger.info(
-            f"Running monte carlo analysis. Number of iterations: "
-            f"{self.iterations}\n"
-        )
-
-        # Store the optimized results in variable that will be overridden on
-        # every pass
-        opt_res = self.optimize_results
-        opt_params_list = []
-        matrices = []
-
-        for _ in range(self.iterations):
-            new_matrix = self._apply_noise()
-
-            # We optimise the parameters using the noisy matrix as input
-            opt_res = PhysioFitter._run_optimization(
-                opt_res.x, self.model.simulate, new_matrix, self.model.time_vector,
-                self.model.fixed_parameters, self.sd, self.model.bounds(),
-                "L-BFGS-B"
-            )
-
-            # Store the new simulated matrix in list for later use
-            matrices.append(
-                self.model.simulate(
-                    opt_res.x, new_matrix, self.model.time_vector,
-                    self.model.fixed_parameters
-                )
-            )
-
-            # Store the new optimised parameters in list for later use
-            opt_params_list.append(opt_res.x)
-
-        # Build a 3D array from all the simulated matrices to get standard
-        # deviation on each data point
-        matrices = np.array(matrices)
-        self.matrices_ci = {
-            "lower_ci": np.percentile(matrices, 2.5, axis=0),
-            "higher_ci": np.percentile(matrices, 97.5, axis=0)
-        }
-
-        # Compute the statistics on the list of parameters: means, sds,
-        # medians and confidence interval
-        self._compute_parameter_stats(opt_params_list)
-        logger.info(f"Optimized parameters statistics:")
-        for key, value in self.parameter_stats.items():
-            logger.info(f"{key}: {value}")
-
-        # Apply nan mask to be coherent with the experimental matrix
-        nan_lower_ci = np.copy(self.matrices_ci['lower_ci'])
-        nan_higher_ci = np.copy(self.matrices_ci['higher_ci'])
-        nan_lower_ci[np.isnan(self.experimental_matrix)] = np.nan
-        nan_higher_ci[np.isnan(self.experimental_matrix)] = np.nan
-
-        logger.info(
-            f"Simulated matrix lower confidence interval:\n{nan_lower_ci}\n"
-        )
-        logger.info(
-            f"Simulated matrix higher confidence interval:\n{nan_higher_ci}\n"
-        )
-        return
-
-    def _compute_parameter_stats(self, opt_params_list):
-        """
-        Compute statistics on the optimized parameters from the monte carlo
-        analysis.
-
-        :param opt_params_list: list of optimized parameter arrays generated
-                                during the monte carlo analysis
-        :return: parameter stats attribute containing means, sds, medians, low
-                 and high CI
-        """
-
-        opt_params_means = np.mean(np.array(opt_params_list), 0)
-        opt_params_sds = np.std(np.array(opt_params_list), 0)
-        opt_params_meds = np.median(np.array(opt_params_list), 0)
-        conf_ints = np.column_stack((
-            np.percentile(opt_params_list, 2.5, 0),
-            np.percentile(opt_params_list, 97.5, 0)
-        ))
-
-        self.parameter_stats.update({
-            "mean": opt_params_means,
-            "sd": opt_params_sds,
-            "median": opt_params_meds,
-            "CI_2.5": conf_ints[:, 0],
-            "CI_97.5": conf_ints[:, 1]
-        })
-
-        # self.parameter_stats_df = DataFrame()
-
-    def khi2_test(self):
-
-        number_measurements = np.count_nonzero(
-            ~np.isnan(self.experimental_matrix)
-        )
-        number_params = len(self.model.parameters_to_estimate)
-        dof = number_measurements - number_params
-        cost = self._calculate_cost(
-            self.optimize_results.x, self.model.simulate, self.experimental_matrix,
-            self.model.time_vector, self.model.fixed_parameters, self.sd
-        )
-        p_val = chi2.cdf(cost, dof)
-
-        khi2_res = {
-            "khi2_value": cost,
-            "number_of_measurements": number_measurements,
-            "number_of_params": number_params,
-            "Degrees_of_freedom": dof,
-            "p_val": p_val
-        }
-        self.khi2_res = DataFrame.from_dict(
-            khi2_res, "index", columns=["Values"]
-        )
-
-        logger.info(f"khi2 test results:\n"
-                     f"khi2 value: {cost}\n"
-                     f"Number of measurements: {number_measurements}\n"
-                     f"Number of parameters to fit: {number_params}\n"
-                     f"Degrees of freedom: {dof}\n"
-                     f"p-value = {p_val}\n"
-                    )
-
-        if p_val < 0.95:
-            logger.info(
-                f"At level of 95% confidence, the model fits the data good "
-                f"enough with respect to the provided measurement SD. "
-                f"Value: {p_val}"
-            )
-
-        else:
-            logger.info(
-                f"At level of 95% confidence, the model does not fit the data "
-                f"good enough with respect to the provided measurement SD. "
-                f"Value: {p_val}\n"
-            )
-
-    @staticmethod
-    def _add_noise(vector, sd):
-        """
-        Add random noise to a given array using input standard deviations.
-
-        :param vector: input array on which to apply noise
-        :type vector: class: numpy.ndarray
-        :param sd: standard deviation to apply to the input array
-        :type sd: class: numpy.ndarray
-        :return: noisy ndarray
-        """
-
-        output = np.random.default_rng().normal(
-            loc=vector, scale=sd, size=vector.size
-        )
-        return output
-
-    def _apply_noise(self):
-        """
-        Apply noise to the simulated matrix obtained using optimized
-        parameters. SDs are obtained from the sd matrix
-        """
-
-        new_matrix = np.array([
-            PhysioFitter._add_noise(self.simulated_matrix[idx, :], sd)
-            for idx, sd in enumerate(self.sd)
-        ])
-        return new_matrix
+"""
+PhysioFit software main module
+"""
+
+import logging
+
+import numpy as np
+from pandas import DataFrame
+from scipy.optimize import minimize, differential_evolution
+from scipy.stats import chi2
+
+from physiofit.models.base_model import Model
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+
+
+# TODO: add estimate deg function (eq 6) with plot of best fit and measured values
+
+
+class PhysioFitter:
+    """
+    This class is responsible for most of Physiofit's heavy lifting. Features included are:
+
+        * loading of data from **csv** or **tsv** file
+        * **equation system initialization** using the following analytical functions (in absence of lag and
+          degradation:
+
+            X(t) = X0 * exp(mu * t)
+            Mi(t) = qMi * (X0 / mu) * (exp(mu * t) - 1) + Mi0
+
+        * **simulation of data points** from given initial parameters
+        * **cost calculation** using the equation:
+
+            residuum = sum((sim - meas) / sd)²
+
+        * **optimization of the initial parameters** using `scipy.optimize.minimize ('Differential evolution', with polish with 'L-BFGS-B' method) <https://docs.scipy.org/doc/scipy/reference/optimize.minimize-lbfgsb.html#optimize-minimize-lbfgsb>`_
+        * **sensitivity analysis, khi2 tests and plotting**
+
+    :param data: DataFrame containing data and passed by IOstream object
+    :type data: class: pandas.DataFrame
+    :param model: Model to initialize parameters and optimize
+    :type model: physiofit.models.base_model.Model
+    :param mc: Should Monte-Carlo sensitivity analysis be performed (default=True)
+    :type mc: Boolean
+    :param iterations: number of iterations for Monte-Carlo simulation (default=50)
+    :type iterations: int
+    :param sd: sd matrix used for residuum calculations. Can be:
+
+                * a matrix with the same dimensions as the measurements matrix (but without the time column)
+                * a named vector containing sds for all the metabolites provided in the input file
+                * 0  in which case the matrix is automatically constructed from default values
+                * a dictionary with the data column headers as keys and the associated value as a scalar or list
+
+    :type sd: int, float, list, dict or ndarray
+    """
+
+    def __init__(
+            self,
+            data,
+            model,
+            mc=True,
+            iterations=100,
+            sd=None,
+            debug_mode=False
+    ):
+
+        self.data = data
+        self.model = model
+        self.mc = mc
+        self.iterations = iterations
+        self.sd = sd
+        self.debug_mode = debug_mode
+        self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
+
+        self.simulated_matrix = None
+        self.simulated_data = None
+        self.optimize_results = None
+        self.simulate = None
+        self.parameter_stats = None
+        self.opt_params_sds = None
+        self.matrices_ci = None
+        self.opt_conf_ints = None
+        self.khi2_res = None
+
+    def verify_attrs(self):
+        """Check that attributes are valid"""
+
+        if type(self.iterations) is not int:
+            raise TypeError(
+                f"Number of monte carlo iterations must be an "
+                f"integer, and not of type {type(self.iterations)}"
+            )
+
+        allowed_sds = [int, float, list, np.ndarray]
+        if type(self.sd) not in allowed_sds:
+            raise TypeError(
+                f"sds is not in the right format ({type(self.sd)}. "
+                f"Compatible formats are:\n{allowed_sds}"
+            )
+
+    def _sd_dict_to_matrix(self):
+        """Convert sd dictionary to matrix/vector"""
+
+        logger.debug("Initializing sd matrix from dict")
+        # Perform checks
+        for key in self.sd.keys():
+            if key not in self.model.name_vector:
+                raise KeyError(
+                    f"The key {key} is not part of the data headers"
+                )
+        for name in self.model.name_vector:
+            if name not in self.sd.keys():
+                raise KeyError(
+                    f"The key {name} is missing from the sds dict"
+                )
+
+        # Get lengths of each sd entry
+        sd_lengths = [
+            len(self.sd[key]) if type(self.sd[key]) not in [float, int] else 1
+            for key in self.sd.keys()
+        ]
+
+        # Make sure that lengths are the same
+        if not all(elem == sd_lengths[0] for elem in sd_lengths):
+            raise ValueError("All sd vectors must have the same length")
+
+        # Build matrix/vector
+        if sd_lengths[0] == 1:
+            self.sd = [self.sd[name] for name in self.model.name_vector]
+        else:
+            columns = (self.sd[name] for name in self.model.name_vector)
+            matrix = np.column_stack(columns)
+            self.sd = matrix
+
+        logger.debug(f"SD object type: {type(self.sd)}")
+        logger.debug(f"Array built from dict:\n{self.sd}")
+
+    def initialize_sd_matrix(self):
+        """
+        Initialize the sd matrix from different types of inputs: single value,
+        vector or matrix.
+
+        :return: None
+        """
+
+        # This function can be optimized, if the input is a matrix we should
+        # detect it directly
+        logger.info("Initializing sd matrix...\n")
+
+        # If sd is None, we generate the default matrix
+        if self.sd is None or self.sd == {}:
+            try:
+                self.sd = {"X": 0.2}
+                for col in self.data.columns[2:]:
+                    self.sd.update({col: 0.5})
+            except Exception:
+                raise
+
+        if isinstance(self.sd, dict):
+            self._sd_dict_to_matrix()
+        # When sd is a single value, we build a sd matrix containing the value
+        # in all positions
+        if isinstance(self.sd, int) or isinstance(self.sd, float):
+            self._build_sd_matrix()
+            logger.debug(f"SD matrix: {self.sd}\n")
+            return
+        if not isinstance(self.sd, np.ndarray) and not isinstance(self.sd,
+                                                                  list):
+            raise TypeError(
+                f"Cannot coerce SD to array. Please check that a list or array "
+                f"is given as input.\nCurrent input: \n{self.sd}"
+            )
+        else:
+            self.sd = np.array(self.sd)
+        if not np.issubdtype(self.sd.dtype, np.number):
+            try:
+                self.sd = self.sd.astype(float)
+            except ValueError:
+                raise ValueError(
+                    f"The sd vector/matrix contains values that are not "
+                    f"numeric. \nCurrent sd vector/matrix: \n{self.sd}"
+                )
+            except Exception as e:
+                raise RuntimeError(f"Unknown error: {e}")
+        else:
+            # If the array is not the right shape, we assume it is a vector
+            # that needs to be tiled into a matrix
+
+            logger.debug(f"SD matrix: {self.sd}\n")
+            logger.debug(f"Type of SD matrix: {type(self.sd)}")
+
+            if self.sd.shape != self.experimental_matrix.shape:
+                try:
+                    self._build_sd_matrix()
+                except ValueError:
+                    raise
+                except RuntimeError:
+                    raise
+            else:
+                logger.debug(f"sd matrix: {self.sd}\n")
+                return
+        logger.info(f"sd Matrix:\n{self.sd}\n")
+
+    def _build_sd_matrix(self):
+        """
+        Build the sd matrix from different input types
+
+        :return: None
+        """
+
+        # First condition: the sds are in a 1D array
+        if isinstance(self.sd, np.ndarray):
+            # We first check that the sd vector is as long as the
+            # experimental matrix on the row axis
+            if self.sd.size != self.experimental_matrix[0].size:
+                raise ValueError("sd vector not of right size")
+            else:
+                # We duplicate the vector column-wise to build a matrix of
+                # duplicated sd vectors
+                self.sd = np.tile(self.sd, (len(self.experimental_matrix), 1))
+
+        # Second condition: the sd is a scalar and must be broadcast to a
+        # matrix with same shape as the data
+        elif isinstance(self.sd, int) or isinstance(self.sd, float):
+            self.sd = np.full(self.experimental_matrix.shape, self.sd)
+        else:
+            raise RuntimeError("Unknown error")
+
+    def _get_default_sds(self):
+        """
+        Build a default sd matrix. Default values:
+            * Biomass: 0.2
+            * Metabolites: 0.5
+        :return: None
+        """
+
+        sds = [0.2]
+        for name in range(len(self.model.name_vector) - 1):
+            sds.append(0.5)
+        self.sd = np.array(sds)
+        self._build_sd_matrix()
+
+    def optimize(self):
+        """
+        Run optimization and build the simulated matrix
+        from the optimized parameters
+        """
+
+        logger.info("\nRunning optimization...\n")
+        bounds = self.model.bounds()
+        parameters = [param for param in self.model.parameters_to_estimate.values()]
+        logger.debug(f"Simulate function = {self.model.simulate}")
+        self.optimize_results = self._run_optimization(
+            params=parameters,
+            func=self.model.simulate,
+            exp_data_matrix=self.experimental_matrix,
+            time_vector=self.model.time_vector,
+            non_opt_params=self.model.fixed_parameters,
+            sd_matrix=self.sd,
+            bounds=bounds,
+            method="differential_evolution"
+        )
+        self.parameter_stats = {
+            "optimal": self.optimize_results.x
+        }
+        logger.info(f"Optimization results: \n{self.optimize_results}\n")
+        for i, param in zip(
+                self.model.parameters_to_estimate, self.optimize_results.x
+        ):
+            logger.info(f"\n{i} = {param}\n")
+        self.simulated_matrix = self.model.simulate(
+            self.optimize_results.x,
+            self.experimental_matrix,
+            self.model.time_vector,
+            self.model.fixed_parameters
+        )
+        logger.debug(f"simulated_matrix:\n{self.simulated_matrix}")
+        nan_sim_mat = np.copy(self.simulated_matrix)
+        nan_sim_mat[np.isnan(self.experimental_matrix)] = np.nan
+        self.simulated_data = DataFrame(
+            data=nan_sim_mat,
+            index=self.model.time_vector,
+            columns=self.model.name_vector
+        )
+        self.simulated_data.index.name = "Time"
+        logger.info(f"Final Simulated Data: \n{self.simulated_data}\n")
+
+    @staticmethod
+    def _calculate_cost(
+            params, func, exp_data_matrix, time_vector, non_opt_params,
+            sd_matrix
+    ):
+        """
+        Calculate the cost (residue) using the square of
+        simulated-experimental over the SDs
+        """
+
+        simulated_matrix = func(params, exp_data_matrix, time_vector,
+                                non_opt_params)
+        cost_val = np.square((simulated_matrix - exp_data_matrix) / sd_matrix)
+        residuum = np.nansum(cost_val)
+        return residuum
+
+    @staticmethod
+    def _run_optimization(
+            params: list,
+            func: Model.simulate,
+            exp_data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            non_opt_params: dict,
+            sd_matrix: np.ndarray,
+            bounds: tuple,
+            method: str
+    ):
+        """
+        Run the optimization on input parameters using the cost function and
+        Scipy minimize (L-BFGS-B method that is deterministic and uses the
+        gradient method for optimizing)
+        """
+
+        if method == "differential_evolution":
+            logger.debug(f"Optimization method = {method}")
+            optimize_results = differential_evolution(
+                PhysioFitter._calculate_cost, bounds=bounds,
+                args=(
+                func, exp_data_matrix, time_vector, non_opt_params, sd_matrix),
+                polish=True, x0=np.array(params)
+            )
+        elif method == "L-BFGS-B":
+            logger.debug(f"Optimization method = {method}")
+            optimize_results = minimize(
+                PhysioFitter._calculate_cost, x0=np.array(params),
+                args=(
+                func, exp_data_matrix, time_vector, non_opt_params, sd_matrix),
+                method="L-BFGS-B", bounds=bounds, options={'maxcor': 30}
+            )
+        else:
+            raise ValueError(f"{method} is not implemented")
+
+        return optimize_results
+
+    def monte_carlo_analysis(self):
+        """
+        Run a monte carlo analysis to calculate optimization standard
+        deviations on parameters and simulated data points
+        """
+
+        if not self.optimize_results:
+            raise RuntimeError(
+                "Running Monte Carlo simulation without having run the "
+                "optimization is impossible as best fit results are needed to "
+                "generate the initial simulated matrix"
+            )
+
+        logger.info(
+            f"Running monte carlo analysis. Number of iterations: "
+            f"{self.iterations}\n"
+        )
+
+        # Store the optimized results in variable that will be overridden on
+        # every pass
+        opt_res = self.optimize_results
+        opt_params_list = []
+        matrices = []
+
+        for _ in range(self.iterations):
+            new_matrix = self._apply_noise()
+
+            # We optimise the parameters using the noisy matrix as input
+            opt_res = PhysioFitter._run_optimization(
+                opt_res.x, self.model.simulate, new_matrix, self.model.time_vector,
+                self.model.fixed_parameters, self.sd, self.model.bounds(),
+                "L-BFGS-B"
+            )
+
+            # Store the new simulated matrix in list for later use
+            matrices.append(
+                self.model.simulate(
+                    opt_res.x, new_matrix, self.model.time_vector,
+                    self.model.fixed_parameters
+                )
+            )
+
+            # Store the new optimised parameters in list for later use
+            opt_params_list.append(opt_res.x)
+
+        # Build a 3D array from all the simulated matrices to get standard
+        # deviation on each data point
+        matrices = np.array(matrices)
+        self.matrices_ci = {
+            "lower_ci": np.percentile(matrices, 2.5, axis=0),
+            "higher_ci": np.percentile(matrices, 97.5, axis=0)
+        }
+
+        # Compute the statistics on the list of parameters: means, sds,
+        # medians and confidence interval
+        self._compute_parameter_stats(opt_params_list)
+        logger.info(f"Optimized parameters statistics:")
+        for key, value in self.parameter_stats.items():
+            logger.info(f"{key}: {value}")
+
+        # Apply nan mask to be coherent with the experimental matrix
+        nan_lower_ci = np.copy(self.matrices_ci['lower_ci'])
+        nan_higher_ci = np.copy(self.matrices_ci['higher_ci'])
+        nan_lower_ci[np.isnan(self.experimental_matrix)] = np.nan
+        nan_higher_ci[np.isnan(self.experimental_matrix)] = np.nan
+
+        logger.info(
+            f"Simulated matrix lower confidence interval:\n{nan_lower_ci}\n"
+        )
+        logger.info(
+            f"Simulated matrix higher confidence interval:\n{nan_higher_ci}\n"
+        )
+        return
+
+    def _compute_parameter_stats(self, opt_params_list):
+        """
+        Compute statistics on the optimized parameters from the monte carlo
+        analysis.
+
+        :param opt_params_list: list of optimized parameter arrays generated
+                                during the monte carlo analysis
+        :return: parameter stats attribute containing means, sds, medians, low
+                 and high CI
+        """
+
+        opt_params_means = np.mean(np.array(opt_params_list), 0)
+        opt_params_sds = np.std(np.array(opt_params_list), 0)
+        opt_params_meds = np.median(np.array(opt_params_list), 0)
+        conf_ints = np.column_stack((
+            np.percentile(opt_params_list, 2.5, 0),
+            np.percentile(opt_params_list, 97.5, 0)
+        ))
+
+        self.parameter_stats.update({
+            "mean": opt_params_means,
+            "sd": opt_params_sds,
+            "median": opt_params_meds,
+            "CI_2.5": conf_ints[:, 0],
+            "CI_97.5": conf_ints[:, 1]
+        })
+
+        # self.parameter_stats_df = DataFrame()
+
+    def khi2_test(self):
+
+        number_measurements = np.count_nonzero(
+            ~np.isnan(self.experimental_matrix)
+        )
+        number_params = len(self.model.parameters_to_estimate)
+        dof = number_measurements - number_params
+        cost = self._calculate_cost(
+            self.optimize_results.x, self.model.simulate, self.experimental_matrix,
+            self.model.time_vector, self.model.fixed_parameters, self.sd
+        )
+        p_val = chi2.cdf(cost, dof)
+
+        khi2_res = {
+            "khi2_value": cost,
+            "number_of_measurements": number_measurements,
+            "number_of_params": number_params,
+            "Degrees_of_freedom": dof,
+            "p_val": p_val
+        }
+        self.khi2_res = DataFrame.from_dict(
+            khi2_res, "index", columns=["Values"]
+        )
+
+        logger.info(f"khi2 test results:\n"
+                     f"khi2 value: {cost}\n"
+                     f"Number of measurements: {number_measurements}\n"
+                     f"Number of parameters to fit: {number_params}\n"
+                     f"Degrees of freedom: {dof}\n"
+                     f"p-value = {p_val}\n"
+                    )
+
+        if p_val < 0.95:
+            logger.info(
+                f"At level of 95% confidence, the model fits the data good "
+                f"enough with respect to the provided measurement SD. "
+                f"Value: {p_val}"
+            )
+
+        else:
+            logger.info(
+                f"At level of 95% confidence, the model does not fit the data "
+                f"good enough with respect to the provided measurement SD. "
+                f"Value: {p_val}\n"
+            )
+
+    @staticmethod
+    def _add_noise(vector, sd):
+        """
+        Add random noise to a given array using input standard deviations.
+
+        :param vector: input array on which to apply noise
+        :type vector: class: numpy.ndarray
+        :param sd: standard deviation to apply to the input array
+        :type sd: class: numpy.ndarray
+        :return: noisy ndarray
+        """
+
+        output = np.random.default_rng().normal(
+            loc=vector, scale=sd, size=vector.size
+        )
+        return output
+
+    def _apply_noise(self):
+        """
+        Apply noise to the simulated matrix obtained using optimized
+        parameters. SDs are obtained from the sd matrix
+        """
+
+        new_matrix = np.array([
+            PhysioFitter._add_noise(self.simulated_matrix[idx, :], sd)
+            for idx, sd in enumerate(self.sd)
+        ])
+        return new_matrix
```

### Comparing `physiofit-3.0.4/physiofit/base/io.py` & `physiofit-3.0.6/physiofit/base/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,653 +1,653 @@
-"""Module to handle inputs and outputs for PhysioFit"""
-
-from __future__ import annotations
-import importlib
-import logging
-import os
-import sys
-from pathlib import Path
-from io import BytesIO
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-# Switch matplotlib logger to higher level to not get debug logs in root logger
-logging.getLogger("matplotlib").setLevel(logging.WARNING)
-
-from matplotlib.backends.backend_pdf import PdfPages
-from pandas import DataFrame, read_csv, concat
-import yaml
-
-from physiofit import __file__
-from physiofit.base.fitter import PhysioFitter
-from physiofit.models.base_model import StandardDevs, Bounds
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
-
-class IoHandler:
-    """
-    Input/Output class that handles the former and initializes the
-    PhysioFitter component object. It is the preferred interface for
-    interacting with the PhysioFit package.
-
-    """
-
-    allowed_keys = {
-        "sd", "model", "iterations", "mc", "debug_mode"
-    }
-
-    def __init__(self):
-
-        self._output_type = []
-        self.figures = []
-        self.models = []
-        self.fitter = None
-        self.output = None
-        self.data = None
-        self.names = None
-        self.simulated_data_sds = None
-        self.simulated_data = None
-        self.experimental_data = None
-        self.home_path = None
-        self.data_path = None
-        self.res_path = None
-        self.has_config_been_read = False
-        self.experiments = None
-        self.multiple_experiments = False
-
-    @staticmethod
-    def read_data(data: str) -> DataFrame:
-        """
-        Read initial data file (csv or tsv)
-
-        :param data: str containing the relative or
-                             absolute path to the data
-        :return: pandas DataFrame containing the data
-        """
-        try:
-            if isinstance(data, str):
-                data_path = Path(data).resolve()
-            # .dat file type for galaxy implementation
-                if data_path.suffix in [".txt", ".tsv", ".dat"]:
-                    data = read_csv(str(data_path), sep="\t")
-                elif data_path.suffix == ".csv":
-                    data = read_csv(str(data_path), sep=";")
-                else:
-                    if not data_path.exists():
-                        raise ValueError(f"{data_path} is not a valid file")
-                    else:
-                        raise TypeError(
-                            f"{data_path} is not a valid format. "
-                            f"Accepted formats are .csv, .txt or .tsv"
-                        )
-            elif issubclass(type(data), BytesIO):
-                data = read_csv(data, sep="\t")
-            else:
-                raise TypeError(f"Input data file is not of right type. Accepted types: file-like (bytes) or string")
-        except Exception:
-            logger.exception("There was an error while reading the data")
-            raise IOError(
-                "Error while reading data. Please ensure you have the right file format (txt, tsv or bytes)"
-            )
-
-        IoHandler._verify_data(data)
-        return data
-
-    def select_model(self, model_name, data=None):
-        """
-        Select a model from the list of models in the model folder of the package src directory
-        """
-
-        self.get_models(data)
-        for x in self.models:
-            if x.model_name == model_name:
-                model = x
-        return model
-
-    def read_model(self, model_file):
-        """
-        Import and return the model class from .py file containing the model.
-
-        .. warning: ONLY USE THIS FUNCTION ON TRUSTED PYTHON FILES. Reading code from untrusted sources can lead to
-                    propagation of viruses and compromised security.
-
-        :param model_file: path to the model.py file to import
-        """
-
-        if not Path(model_file).is_file() or Path(model_file).suffix != ".py":
-            raise ValueError(
-                "The given path is not valid. The path must point to a .py file containing the module "
-                "from which the model will be loaded."
-            )
-
-        spec = importlib.util.spec_from_file_location("module_to_import", fr"{model_file}")
-        module = importlib.util.module_from_spec(spec)
-        sys.modules["module_to_import"] = module
-        spec.loader.exec_module(module)
-        model_class = getattr(module, "ChildModel")
-
-        return model_class
-
-
-    @staticmethod
-    def _verify_data(data: DataFrame):
-        """
-        Perform checks on DataFrame returned by the _read_data function
-
-        :param data: pandas DataFrame containing the data
-        :return: None
-        """
-
-        if not isinstance(data, DataFrame):
-            raise TypeError(
-                "There was an error reading the data: "
-                "DataFrame has not been generated"
-            )
-
-        for x in ["time", "X"]:
-            if x not in data.columns:
-                raise ValueError(f"Column {x} is missing from the dataset")
-
-        if "experiment" in data.columns:
-            if len(data.columns) <= 3:
-                raise ValueError(f"Data does not contain any metabolite columns")
-        else:
-            if len(data.columns) <= 2:
-                raise ValueError(f"Data does not contain any metabolite columns")
-
-        for x in data.columns:
-            if x != "experiments" and data[x].dtypes != np.int64 and data[x].dtypes != np.float64:
-                raise ValueError(
-                    f"Column {x} has values that are not of numeric type"
-                )
-            if all(data[x].isnull()) or all(data[x].isna()):
-                raise ValueError(
-                f"The column {x} contains only null or NA values"
-            )
-
-    @staticmethod
-    def get_model_list():
-        model_dir = Path(__file__).parent / "models"
-        # Make fake dataframe
-        df = DataFrame(
-            columns=["time", "X"],
-        )
-        for file in os.listdir(str(model_dir)):
-            if "model_" in file:
-                module = importlib.import_module(
-                    f"physiofit.models.{file[:-3]}"
-                )
-                model_class = getattr(module, "ChildModel")
-                model = model_class(df)
-                print(model.model_name)
-        return
-        
-    def get_models(self, data=None):
-        """
-        Read modules containing the different models and add them to models attribute
-
-        :return: list containing the different model objects
-        """
-
-        model_dir = Path(__file__).parent / "models"
-        for file in os.listdir(str(model_dir)):
-            if "model_" in file:
-                module = importlib.import_module(
-                    f"physiofit.models.{file[:-3]}"
-                )
-                model_class = getattr(module, "ChildModel")
-                if data is not None:
-                    self.models.append(model_class(data))
-                else:
-                    self.models.append(model_class(self.data))
-
-    @staticmethod
-    def read_yaml(yaml_file: str | bytes) -> ConfigParser:
-
-        """
-        Import raml configuration file and parse keyword arguments
-
-        :param yaml_file: path to the yaml file or json file
-        :return config_parser: Dictionary containing arguments parsed from yaml file
-        """
-
-        # Load config file
-        try:
-            if isinstance(yaml_file, str) or issubclass(type(yaml_file), BytesIO):
-                config_parser = ConfigParser.from_file(yaml_file)
-            else:
-                raise TypeError(
-                    f"Trying to read object that is not a file or path to file: {yaml_file}"
-                )
-        except Exception as e:
-            raise IOError(
-                f"Error while reading yaml configuration file {yaml_file}. "
-                f"\nTraceback:\n\n{e}"
-                )
-        return config_parser
-
-    def initialize_fitter(self, data, **kwargs):
-        """
-        Initialize a PhysioFitter object
-
-        :param kwargs: Keyword arguments for fitter initialization
-        :return: None
-        """
-
-        wrong_keys = []
-
-        # Initialize fitter
-        fitter = PhysioFitter(
-            data=data,
-            model=kwargs["model"],
-            mc=kwargs["mc"] if "mc" in kwargs else True,
-            iterations=kwargs["iterations"] if "iterations" in kwargs else 100,
-            sd=kwargs["sd"] if "sd" in kwargs else StandardDevs(),
-            debug_mode=kwargs["debug_mode"] if "debug_mode" in kwargs else False
-        )
-
-        if "sd" not in kwargs:
-            fitter.sd.update(
-                {"X" : 0.2}
-            )
-            for col in self.data.columns[2:]:
-                fitter.sd.update(
-                    {col : 0.2}
-                )
-
-        fitter.initialize_sd_matrix()
-        fitter.verify_attrs()
-        logger.debug(
-            f"Fitter attribute dictionary:\n{fitter.__dict__}"
-        )
-
-        return fitter
-
-
-    def output_pdf(self, fitter, export_path: str | Path = None):
-        """
-        Handle the creation and output of a pdf file containing fit results as
-        a plot
-
-        :param export_path: Path to exported pdf. In local mode, it is sent to
-                            the _res directory
-        :return: None
-        """
-
-        if not self.figures:
-            self.plot_data(fitter)
-
-        try:
-            with PdfPages(rf"{export_path}\plots.pdf") as pdf:
-                for fig in self.figures:
-                    pdf.savefig(fig[1])
-        except Exception as e:
-            raise IOError(f"Error while generating pdf:\n{e}")
-
-    def output_plots(self, fitter, export_path):
-        """
-        Handle the creation and export of the different plots in svg format
-        :return: None
-        """
-
-        if not self.figures:
-            self.plot_data(fitter)
-
-        try:
-            for fig in self.figures:
-                fig[1].savefig(rf"{export_path}\{fig[0]}.svg")
-        except Exception:
-            raise RuntimeError("Unknown error while generating output")
-
-    def output_recap(self, export_path: str):
-
-        if not isinstance(self.multiple_experiments, list):
-            raise TypeError(
-                "The multiple experiments attribute must be a list"
-            )
-        if not self.multiple_experiments:
-            raise ValueError(
-                f"It seems that the multiple experiments list is empty: {self.multiple_experiments}"
-            )
-        for idx, element in enumerate(self.multiple_experiments):
-            if not isinstance(element, DataFrame):
-                raise TypeError(
-                    f"All the elements of multiple_experiments must be DataFrames. Wrong element type"
-                    f"detected at indice {idx}"
-                )
-        final_df = concat(self.multiple_experiments)
-        final_df.to_csv(f"{str(Path(export_path))}/recap.csv")
-
-
-
-    def output_report(self, fitter, export_path: str |list = None):
-        """
-        Handle creation and export of the report containing stats from monte
-        carlo analysis of optimization parameters
-
-        :param export_paths: list of paths to export the stats and fluxes. [0]
-                             is for stats and [1] for fluxes.
-        """
-
-        if isinstance(export_path, list):
-            if len(export_path) != 2:
-                raise ValueError(
-                    f"Expected only 2 export paths and {len(export_path)}"
-                    f" were detected"
-                )
-            stat_path = export_path[0]
-            flux_path = export_path[1]
-        else:
-            flux_path = fr"{export_path}\flux_results.tsv"
-            stat_path = fr"{export_path}\stat_results.tsv"
-
-        logger.debug(
-            f"Parameter Stats:\n{fitter.parameter_stats}"
-        )
-
-        # Get optimization results as dataframe
-        opt_data = DataFrame.from_dict(fitter.parameter_stats,
-                                       orient="columns")
-
-        # Use IDs to clarify which parameter is described on each line
-        opt_data.index = [param for param in fitter.model.parameters_to_estimate.keys()]
-        opt_data.to_csv(flux_path, sep="\t")
-
-        if isinstance(fitter.khi2_res, DataFrame):
-            with open(stat_path, "w+") as stat_out:
-                stat_out.write("==================\n"
-                               "Khi² test results\n"
-                               "==================\n\n")
-                stat_out.write(
-                    fitter.khi2_res.to_string(
-                        header=False, justify="center"
-                    )
-                )
-                if fitter.khi2_res.at["p_val", "Values"] < 0.95:
-                    stat_out.write(
-                        f"\n\nAt level of 95% confidence, the model fits the "
-                        f"data good enough with respect to the provided "
-                        f"measurement SD. Value: "
-                        f"{fitter.khi2_res.at['p_val', 'Values']}"
-                    )
-
-                else:
-                    stat_out.write(
-                        f"\n\nAt level of 95% confidence, the model does not "
-                        f"fit the data good enough with respect to the "
-                        f"provided measurement SD. Value: "
-                        f"{fitter.khi2_res.at['p_val', 'Values']}\n"
-                    )
-
-    def _get_plot_data(self, fitter):
-        """
-        Prepare data for plotting
-        """
-
-        # Initialize vectors and data for plotting
-        if fitter.model.time_vector is not None:
-            x = fitter.model.time_vector
-        else:
-            raise ValueError(
-                "PhysioFitter model time_vector has not been initialized. "
-                "Have you loaded in the data correctly?"
-            )
-        if fitter.experimental_matrix is not None:
-            exp_mat = fitter.experimental_matrix
-        else:
-            raise ValueError(
-                "PhysioFitter object does not have experimental data loaded in"
-            )
-        if fitter.simulated_matrix is not None:
-            sim_mat = fitter.simulated_matrix
-        else:
-            raise ValueError("PhysioFitter simulated data does not exist yet")
-        if fitter.matrices_ci is not None:
-            sim_mat_ci = fitter.matrices_ci
-            self.simulated_data_low_ci = DataFrame(
-                columns=fitter.model.name_vector,
-                index=x,
-                data=sim_mat_ci["lower_ci"]
-            )
-            self.simulated_data_high_ci = DataFrame(
-                columns=fitter.model.name_vector,
-                index=x,
-                data=sim_mat_ci["higher_ci"]
-            )
-        else:
-            logger.warning(
-                "Monte Carlo analysis has not been done, "
-                "confidence intervals will not be computed"
-            )
-
-        self.experimental_data = DataFrame(
-            columns=fitter.model.name_vector,
-            index=x,
-            data=exp_mat
-        ).sort_index(level=0)
-        self.simulated_data = DataFrame(
-            columns=fitter.model.name_vector,
-            index=x,
-            data=sim_mat
-        ).sort_index(level=0)
-
-    def plot_data(self, fitter, display: bool = False):
-        """
-        Plot the data
-
-        :param display: should plots be displayed
-        """
-
-        self._get_plot_data(fitter)
-        self._draw_plots(fitter, display)
-
-    def _draw_plots(self, fitter, display: bool):
-        """
-        Draw plots and assign them to the _figures attribute for later access
-        in pdf and plot generation functions
-
-        :param display: Should plots be displayed or not on creation
-        """
-
-        for element in fitter.model.name_vector:
-
-            # Initialize figure object
-            fig, ax = plt.subplots()
-            fig.set_size_inches(9, 5)
-
-            # Draw experimental points onto the Axe
-            exp = ax.scatter(
-                self.experimental_data.index,
-                self.experimental_data[element],
-                marker='o',
-                color="orange"
-            )
-            exp.set_label(f"Exp {element}")
-
-            # Draw the simulated line onto the Axe
-            sim_line, = ax.plot(
-                self.simulated_data.index,
-                self.simulated_data[element],
-                linestyle='--'
-            )
-            sim_line.set_label(f"Sim {element}")
-
-            # If monte carlo analysis has been done add the
-            # corresponding sd to the plot as a red area
-            if fitter.matrices_ci is not None:
-                ax = self._add_sd_area(element, ax)
-
-            # Finishing touches
-            ax.set(xlim=0, ylim=0)
-            ax.set_xlabel("Time", fontsize=21)
-            ax.set_ylabel("Concentration", fontsize=21)
-            ax.legend(prop={"size": 18})
-            ax.set_title(f"{element}", fontsize=23)
-            ax.tick_params(axis='both', which='major', labelsize=18)
-            fig.tight_layout()
-
-            # Add the figure with the metabolite name as index
-            # to the _figures attribute for later use
-            self.figures.append((element, fig))
-
-        if display:
-            for _ in self.figures:
-                plt.show()
-        plt.close()
-
-    def _add_sd_area(self, element: str, ax: plt.Axes):
-        """
-        Draw red area around the fitting line to show confidence intervals
-
-        :param element: Which variable is being plotted
-        :param ax: axes on which to draw the area before
-                   returning to mother function
-        """
-
-        y1 = self.simulated_data_low_ci[element].to_numpy()
-        y2 = self.simulated_data_high_ci[element].to_numpy()
-        x = self.simulated_data.index
-        ax.fill_between(x, y1, y2, alpha=.3, linewidth=0, color="red")
-        return ax
-
-
-class ConfigParser:
-
-    allowed_keys = ["model", "sds", "mc", "iterations"]
-
-    def __init__(
-            self,
-            selected_model,
-            sds,
-            mc,
-            iterations,
-            path_to_data=None
-    ):
-
-        self.path_to_data = path_to_data
-        self.model = selected_model
-        self.sds = StandardDevs(sds)
-        self.mc = mc
-        self.iterations = iterations
-
-        if not isinstance(self.mc, bool):
-            raise TypeError(
-                f"The MonteCarlo option must be given as a boolean (True or False). Detected input: {self.mc}, "
-                f"type: {type(self.mc)}"
-            )
-        if not isinstance(self.iterations, int):
-            raise TypeError(
-                f"Number of iterations must be an integer: Detected input: {self.mc}, type: {type(self.iterations)}"
-            )
-
-
-    @classmethod
-    def from_file(cls, yaml_file):
-
-        if isinstance(yaml_file, str):
-            with open(yaml_file, 'r') as file:
-                data = yaml.safe_load(file)
-        else:
-            data = yaml.safe_load(yaml_file)
-        data_keys = [key for key in data.keys()]
-        for key in cls.allowed_keys:
-            if key not in data_keys:
-                raise ValueError(
-                    f"The key {key} is missing from the input config file"
-                )
-
-        try:
-            return ConfigParser(
-                path_to_data=data["path_to_data"],
-                selected_model=data["model"],
-                sds = data["sds"],
-                mc = data["mc"],
-                iterations = data["iterations"]
-            )
-        except KeyError:
-            return ConfigParser(
-                selected_model=data["model"],
-                sds=data["sds"],
-                mc=data["mc"],
-                iterations=data["iterations"]
-            )
-
-    @classmethod
-    def from_galaxy(cls, galaxy_yaml):
-        pass
-
-    def get_kwargs(self):
-        return  {
-            "path_to_data" : self.path_to_data,
-            "model" : self.model,
-            "mc" : self.mc,
-            "iterations" : self.iterations,
-            "sd" : self.sds
-            }
-
-    def update_model(self, model):
-
-        if self.model["parameters_to_estimate"] is not None:
-            model.parameters_to_estimate.update(self.model["parameters_to_estimate"])
-        if self.model["bounds"] is not None:
-            model.bounds.update(Bounds(self.model["bounds"]))
-        return model
-
-    def export_config(self, export_path):
-
-        with open(fr"{export_path}/config_file.yml", "w") as file:
-            data = {
-                "model" : {
-                    "model_name" : self.model.model_name,
-                    "parameters_to_estimate" : self.model.parameters_to_estimate,
-                    "bounds" : {name : f"{bounds[0], bounds[1]}" for name, bounds in self.model.bounds.items()}
-                },
-                "sds" : dict(self.sds),
-                "mc" : self.mc,
-                "iterations" : self.iterations,
-                "path_to_data" : str(self.path_to_data)
-            }
-            yaml.safe_dump(
-                data,
-                file
-            )
-
-
-if __name__ == "__main__":
-    import pandas as pd
-
-    io_handler = IoHandler()
-    data_file = pd.read_csv(
-        r"C:\Users\legregam\Documents\Projets\PhysioFit\data\KEIO_test_data"
-        r"\KEIO_ROBOT6_1\KEIO_ROBOT6_1.tsv",
-        sep="\t"
-    )
-    io_handler.data = data_file
-    io_handler.data = io_handler.data.sort_values(
-        "time",
-        ignore_index=True
-    )
-    io_handler.get_models()
-    try:
-        sd = {"X": 0.}
-        for col in io_handler.data.columns[2:]:
-            sd.update({col: 0.5})
-    except Exception:
-        raise
-    io_handler.names = io_handler.data.columns[1:].to_list()
-    model = io_handler.models[-1]
-    model.get_params()
-    print(model)
-    keywargs = {
-        "sd": sd,
-        "model": model,
-        "mc": True,
-        "iterations": 100,
-        "debug_mode": True,
-    }
-    io_handler.res_path = Path(
-        r"C:\Users\legregam\Documents\Projets\PhysioFit\data\KEIO_test_data"
-        r"\KEIO_ROBOT6_1")
-    io_handler.initialize_fitter(kwargs=keywargs)
-    io_handler.fitter.optimize()
+"""Module to handle inputs and outputs for PhysioFit"""
+
+from __future__ import annotations
+import importlib
+import logging
+import os
+import sys
+from pathlib import Path
+from io import BytesIO
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+# Switch matplotlib logger to higher level to not get debug logs in root logger
+logging.getLogger("matplotlib").setLevel(logging.WARNING)
+
+from matplotlib.backends.backend_pdf import PdfPages
+from pandas import DataFrame, read_csv, concat
+import yaml
+
+from physiofit import __file__
+from physiofit.base.fitter import PhysioFitter
+from physiofit.models.base_model import StandardDevs, Bounds
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+class IoHandler:
+    """
+    Input/Output class that handles the former and initializes the
+    PhysioFitter component object. It is the preferred interface for
+    interacting with the PhysioFit package.
+
+    """
+
+    allowed_keys = {
+        "sd", "model", "iterations", "mc", "debug_mode"
+    }
+
+    def __init__(self):
+
+        self._output_type = []
+        self.figures = []
+        self.models = []
+        self.fitter = None
+        self.output = None
+        self.data = None
+        self.names = None
+        self.simulated_data_sds = None
+        self.simulated_data = None
+        self.experimental_data = None
+        self.home_path = None
+        self.data_path = None
+        self.res_path = None
+        self.has_config_been_read = False
+        self.experiments = None
+        self.multiple_experiments = False
+
+    @staticmethod
+    def read_data(data: str) -> DataFrame:
+        """
+        Read initial data file (csv or tsv)
+
+        :param data: str containing the relative or
+                             absolute path to the data
+        :return: pandas DataFrame containing the data
+        """
+        try:
+            if isinstance(data, str):
+                data_path = Path(data).resolve()
+            # .dat file type for galaxy implementation
+                if data_path.suffix in [".txt", ".tsv", ".dat"]:
+                    data = read_csv(str(data_path), sep="\t")
+                elif data_path.suffix == ".csv":
+                    data = read_csv(str(data_path), sep=";")
+                else:
+                    if not data_path.exists():
+                        raise ValueError(f"{data_path} is not a valid file")
+                    else:
+                        raise TypeError(
+                            f"{data_path} is not a valid format. "
+                            f"Accepted formats are .csv, .txt or .tsv"
+                        )
+            elif issubclass(type(data), BytesIO):
+                data = read_csv(data, sep="\t")
+            else:
+                raise TypeError(f"Input data file is not of right type. Accepted types: file-like (bytes) or string")
+        except Exception:
+            logger.exception("There was an error while reading the data")
+            raise IOError(
+                "Error while reading data. Please ensure you have the right file format (txt, tsv or bytes)"
+            )
+
+        IoHandler._verify_data(data)
+        return data
+
+    def select_model(self, model_name, data=None):
+        """
+        Select a model from the list of models in the model folder of the package src directory
+        """
+
+        self.get_models(data)
+        for x in self.models:
+            if x.model_name == model_name:
+                model = x
+        return model
+
+    def read_model(self, model_file):
+        """
+        Import and return the model class from .py file containing the model.
+
+        .. warning: ONLY USE THIS FUNCTION ON TRUSTED PYTHON FILES. Reading code from untrusted sources can lead to
+                    propagation of viruses and compromised security.
+
+        :param model_file: path to the model.py file to import
+        """
+
+        if not Path(model_file).is_file() or Path(model_file).suffix != ".py":
+            raise ValueError(
+                "The given path is not valid. The path must point to a .py file containing the module "
+                "from which the model will be loaded."
+            )
+
+        spec = importlib.util.spec_from_file_location("module_to_import", fr"{model_file}")
+        module = importlib.util.module_from_spec(spec)
+        sys.modules["module_to_import"] = module
+        spec.loader.exec_module(module)
+        model_class = getattr(module, "ChildModel")
+
+        return model_class
+
+
+    @staticmethod
+    def _verify_data(data: DataFrame):
+        """
+        Perform checks on DataFrame returned by the _read_data function
+
+        :param data: pandas DataFrame containing the data
+        :return: None
+        """
+
+        if not isinstance(data, DataFrame):
+            raise TypeError(
+                "There was an error reading the data: "
+                "DataFrame has not been generated"
+            )
+
+        for x in ["time", "X"]:
+            if x not in data.columns:
+                raise ValueError(f"Column {x} is missing from the dataset")
+
+        if "experiment" in data.columns:
+            if len(data.columns) <= 3:
+                raise ValueError(f"Data does not contain any metabolite columns")
+        else:
+            if len(data.columns) <= 2:
+                raise ValueError(f"Data does not contain any metabolite columns")
+
+        for x in data.columns:
+            if x != "experiments" and data[x].dtypes != np.int64 and data[x].dtypes != np.float64:
+                raise ValueError(
+                    f"Column {x} has values that are not of numeric type"
+                )
+            if all(data[x].isnull()) or all(data[x].isna()):
+                raise ValueError(
+                f"The column {x} contains only null or NA values"
+            )
+
+    @staticmethod
+    def get_model_list():
+        model_dir = Path(__file__).parent / "models"
+        # Make fake dataframe
+        df = DataFrame(
+            columns=["time", "X"],
+        )
+        for file in os.listdir(str(model_dir)):
+            if "model_" in file:
+                module = importlib.import_module(
+                    f"physiofit.models.{file[:-3]}"
+                )
+                model_class = getattr(module, "ChildModel")
+                model = model_class(df)
+                print(model.model_name)
+        return
+        
+    def get_models(self, data=None):
+        """
+        Read modules containing the different models and add them to models attribute
+
+        :return: list containing the different model objects
+        """
+
+        model_dir = Path(__file__).parent / "models"
+        for file in os.listdir(str(model_dir)):
+            if "model_" in file:
+                module = importlib.import_module(
+                    f"physiofit.models.{file[:-3]}"
+                )
+                model_class = getattr(module, "ChildModel")
+                if data is not None:
+                    self.models.append(model_class(data))
+                else:
+                    self.models.append(model_class(self.data))
+
+    @staticmethod
+    def read_yaml(yaml_file: str | bytes) -> ConfigParser:
+
+        """
+        Import raml configuration file and parse keyword arguments
+
+        :param yaml_file: path to the yaml file or json file
+        :return config_parser: Dictionary containing arguments parsed from yaml file
+        """
+
+        # Load config file
+        try:
+            if isinstance(yaml_file, str) or issubclass(type(yaml_file), BytesIO):
+                config_parser = ConfigParser.from_file(yaml_file)
+            else:
+                raise TypeError(
+                    f"Trying to read object that is not a file or path to file: {yaml_file}"
+                )
+        except Exception as e:
+            raise IOError(
+                f"Error while reading yaml configuration file {yaml_file}. "
+                f"\nTraceback:\n\n{e}"
+                )
+        return config_parser
+
+    def initialize_fitter(self, data, **kwargs):
+        """
+        Initialize a PhysioFitter object
+
+        :param data: input data
+        :param kwargs: Keyword arguments for fitter initialization
+        :return: None
+        """
+        #
+        # wrong_keys = []
+
+        # Initialize fitter
+        fitter = PhysioFitter(
+            data=data,
+            model=kwargs["model"],
+            mc=kwargs["mc"] if "mc" in kwargs else True,
+            iterations=kwargs["iterations"] if "iterations" in kwargs else 100,
+            sd=kwargs["sd"] if "sd" in kwargs else StandardDevs(),
+            debug_mode=kwargs["debug_mode"] if "debug_mode" in kwargs else False
+        )
+
+        if "sd" not in kwargs:
+            fitter.sd.update(
+                {"X" : 0.2}
+            )
+            for col in self.data.columns[2:]:
+                fitter.sd.update(
+                    {col : 0.2}
+                )
+
+        fitter.initialize_sd_matrix()
+        fitter.verify_attrs()
+        logger.debug(
+            f"Fitter attribute dictionary:\n{fitter.__dict__}"
+        )
+
+        return fitter
+
+
+    def output_pdf(self, fitter, export_path: str | Path = None):
+        """
+        Handle the creation and output of a pdf file containing fit results as
+        a plot
+
+        :param export_path: Path to exported pdf. In local mode, it is sent to
+                            the _res directory
+        :return: None
+        """
+
+        if not self.figures:
+            self.plot_data(fitter)
+
+        try:
+            with PdfPages(rf"{export_path}\plots.pdf") as pdf:
+                for fig in self.figures:
+                    pdf.savefig(fig[1])
+        except Exception as e:
+            raise IOError(f"Error while generating pdf:\n{e}")
+
+    def output_plots(self, fitter, export_path):
+        """
+        Handle the creation and export of the different plots in svg format
+        :return: None
+        """
+
+        if not self.figures:
+            self.plot_data(fitter)
+
+        try:
+            for fig in self.figures:
+                fig[1].savefig(rf"{export_path}\{fig[0]}.svg")
+        except Exception:
+            raise RuntimeError("Unknown error while generating output")
+
+    def output_recap(self, export_path: str):
+
+        if not isinstance(self.multiple_experiments, list):
+            raise TypeError(
+                "The multiple experiments attribute must be a list"
+            )
+        if not self.multiple_experiments:
+            raise ValueError(
+                f"It seems that the multiple experiments list is empty: {self.multiple_experiments}"
+            )
+        for idx, element in enumerate(self.multiple_experiments):
+            if not isinstance(element, DataFrame):
+                raise TypeError(
+                    f"All the elements of multiple_experiments must be DataFrames. Wrong element type"
+                    f"detected at indice {idx}"
+                )
+        final_df = concat(self.multiple_experiments)
+        final_df.to_csv(f"{str(Path(export_path))}/summary.csv")
+
+
+    def output_report(self, fitter, export_path: str |list = None):
+        """
+        Handle creation and export of the report containing stats from monte
+        carlo analysis of optimization parameters
+
+        :param export_paths: list of paths to export the stats and fluxes. [0]
+                             is for stats and [1] for fluxes.
+        """
+
+        if isinstance(export_path, list):
+            if len(export_path) != 2:
+                raise ValueError(
+                    f"Expected only 2 export paths and {len(export_path)}"
+                    f" were detected"
+                )
+            stat_path = export_path[0]
+            flux_path = export_path[1]
+        else:
+            flux_path = fr"{export_path}\flux_results.tsv"
+            stat_path = fr"{export_path}\stat_results.tsv"
+
+        logger.debug(
+            f"Parameter Stats:\n{fitter.parameter_stats}"
+        )
+
+        # Get optimization results as dataframe
+        opt_data = DataFrame.from_dict(fitter.parameter_stats,
+                                       orient="columns")
+
+        # Use IDs to clarify which parameter is described on each line
+        opt_data.index = [param for param in fitter.model.parameters_to_estimate.keys()]
+        opt_data.to_csv(flux_path, sep="\t")
+
+        if isinstance(fitter.khi2_res, DataFrame):
+            with open(stat_path, "w+") as stat_out:
+                stat_out.write("==================\n"
+                               "Khi² test results\n"
+                               "==================\n\n")
+                stat_out.write(
+                    fitter.khi2_res.to_string(
+                        header=False, justify="center"
+                    )
+                )
+                if fitter.khi2_res.at["p_val", "Values"] < 0.95:
+                    stat_out.write(
+                        f"\n\nAt level of 95% confidence, the model fits the "
+                        f"data good enough with respect to the provided "
+                        f"measurement SD. Value: "
+                        f"{fitter.khi2_res.at['p_val', 'Values']}"
+                    )
+
+                else:
+                    stat_out.write(
+                        f"\n\nAt level of 95% confidence, the model does not "
+                        f"fit the data good enough with respect to the "
+                        f"provided measurement SD. Value: "
+                        f"{fitter.khi2_res.at['p_val', 'Values']}\n"
+                    )
+
+    def _get_plot_data(self, fitter):
+        """
+        Prepare data for plotting
+        """
+
+        # Initialize vectors and data for plotting
+        if fitter.model.time_vector is not None:
+            x = fitter.model.time_vector
+        else:
+            raise ValueError(
+                "PhysioFitter model time_vector has not been initialized. "
+                "Have you loaded in the data correctly?"
+            )
+        if fitter.experimental_matrix is not None:
+            exp_mat = fitter.experimental_matrix
+        else:
+            raise ValueError(
+                "PhysioFitter object does not have experimental data loaded in"
+            )
+        if fitter.simulated_matrix is not None:
+            sim_mat = fitter.simulated_matrix
+        else:
+            raise ValueError("PhysioFitter simulated data does not exist yet")
+        if fitter.matrices_ci is not None:
+            sim_mat_ci = fitter.matrices_ci
+            self.simulated_data_low_ci = DataFrame(
+                columns=fitter.model.name_vector,
+                index=x,
+                data=sim_mat_ci["lower_ci"]
+            )
+            self.simulated_data_high_ci = DataFrame(
+                columns=fitter.model.name_vector,
+                index=x,
+                data=sim_mat_ci["higher_ci"]
+            )
+        else:
+            logger.warning(
+                "Monte Carlo analysis has not been done, "
+                "confidence intervals will not be computed"
+            )
+
+        self.experimental_data = DataFrame(
+            columns=fitter.model.name_vector,
+            index=x,
+            data=exp_mat
+        ).sort_index(level=0)
+        self.simulated_data = DataFrame(
+            columns=fitter.model.name_vector,
+            index=x,
+            data=sim_mat
+        ).sort_index(level=0)
+
+    def plot_data(self, fitter, display: bool = False):
+        """
+        Plot the data
+
+        :param display: should plots be displayed
+        """
+
+        self._get_plot_data(fitter)
+        self._draw_plots(fitter, display)
+
+    def _draw_plots(self, fitter, display: bool):
+        """
+        Draw plots and assign them to the _figures attribute for later access
+        in pdf and plot generation functions
+
+        :param display: Should plots be displayed or not on creation
+        """
+
+        for element in fitter.model.name_vector:
+
+            # Initialize figure object
+            fig, ax = plt.subplots()
+            fig.set_size_inches(9, 5)
+
+            # Draw experimental points onto the Axe
+            exp = ax.scatter(
+                self.experimental_data.index,
+                self.experimental_data[element],
+                marker='o',
+                color="orange"
+            )
+            exp.set_label(f"Exp {element}")
+
+            # Draw the simulated line onto the Axe
+            sim_line, = ax.plot(
+                self.simulated_data.index,
+                self.simulated_data[element],
+                linestyle='--'
+            )
+            sim_line.set_label(f"Sim {element}")
+
+            # If monte carlo analysis has been done add the
+            # corresponding sd to the plot as a red area
+            if fitter.matrices_ci is not None:
+                ax = self._add_sd_area(element, ax)
+
+            # Finishing touches
+            ax.set(xlim=0, ylim=0)
+            ax.set_xlabel("Time", fontsize=21)
+            ax.set_ylabel("Concentration", fontsize=21)
+            ax.legend(prop={"size": 18})
+            ax.set_title(f"{element}", fontsize=23)
+            ax.tick_params(axis='both', which='major', labelsize=18)
+            fig.tight_layout()
+
+            # Add the figure with the metabolite name as index
+            # to the _figures attribute for later use
+            self.figures.append((element, fig))
+
+        if display:
+            for _ in self.figures:
+                plt.show()
+        plt.close()
+
+    def _add_sd_area(self, element: str, ax: plt.Axes):
+        """
+        Draw red area around the fitting line to show confidence intervals
+
+        :param element: Which variable is being plotted
+        :param ax: axes on which to draw the area before
+                   returning to mother function
+        """
+
+        y1 = self.simulated_data_low_ci[element].to_numpy()
+        y2 = self.simulated_data_high_ci[element].to_numpy()
+        x = self.simulated_data.index
+        ax.fill_between(x, y1, y2, alpha=.3, linewidth=0, color="red")
+        return ax
+
+
+class ConfigParser:
+
+    allowed_keys = ["model", "sds", "mc", "iterations"]
+
+    def __init__(
+            self,
+            selected_model,
+            sds,
+            mc,
+            iterations,
+            path_to_data=None
+    ):
+
+        self.path_to_data = path_to_data
+        self.model = selected_model
+        self.sds = StandardDevs(sds)
+        self.mc = mc
+        self.iterations = iterations
+
+        if not isinstance(self.mc, bool):
+            raise TypeError(
+                f"The MonteCarlo option must be given as a boolean (True or False). Detected input: {self.mc}, "
+                f"type: {type(self.mc)}"
+            )
+        if not isinstance(self.iterations, int):
+            raise TypeError(
+                f"Number of iterations must be an integer: Detected input: {self.mc}, type: {type(self.iterations)}"
+            )
+
+
+    @classmethod
+    def from_file(cls, yaml_file):
+
+        if isinstance(yaml_file, str):
+            with open(yaml_file, 'r') as file:
+                data = yaml.safe_load(file)
+        else:
+            data = yaml.safe_load(yaml_file)
+        data_keys = [key for key in data.keys()]
+        for key in cls.allowed_keys:
+            if key not in data_keys:
+                raise ValueError(
+                    f"The key {key} is missing from the input config file"
+                )
+
+        try:
+            return ConfigParser(
+                path_to_data=data["path_to_data"],
+                selected_model=data["model"],
+                sds = data["sds"],
+                mc = data["mc"],
+                iterations = data["iterations"]
+            )
+        except KeyError:
+            return ConfigParser(
+                selected_model=data["model"],
+                sds=data["sds"],
+                mc=data["mc"],
+                iterations=data["iterations"]
+            )
+
+    @classmethod
+    def from_galaxy(cls, galaxy_yaml):
+        pass
+
+    def get_kwargs(self):
+        return  {
+            "path_to_data" : self.path_to_data,
+            "model" : self.model,
+            "mc" : self.mc,
+            "iterations" : self.iterations,
+            "sd" : self.sds
+            }
+
+    def update_model(self, model):
+
+        if self.model["parameters_to_estimate"] is not None:
+            model.parameters_to_estimate.update(self.model["parameters_to_estimate"])
+        if self.model["bounds"] is not None:
+            model.bounds.update(Bounds(self.model["bounds"]))
+        return model
+
+    def export_config(self, export_path):
+
+        with open(fr"{export_path}/config_file.yml", "w") as file:
+            data = {
+                "model" : {
+                    "model_name" : self.model.model_name,
+                    "parameters_to_estimate" : self.model.parameters_to_estimate,
+                    "bounds" : {name : f"{bounds[0], bounds[1]}" for name, bounds in self.model.bounds.items()}
+                },
+                "sds" : dict(self.sds),
+                "mc" : self.mc,
+                "iterations" : self.iterations,
+                "path_to_data" : str(self.path_to_data)
+            }
+            yaml.safe_dump(
+                data,
+                file
+            )
+
+
+if __name__ == "__main__":
+    import pandas as pd
+
+    io_handler = IoHandler()
+    data_file = pd.read_csv(
+        r"C:\Users\legregam\Documents\Projets\PhysioFit\data\KEIO_test_data"
+        r"\KEIO_ROBOT6_1\KEIO_ROBOT6_1.tsv",
+        sep="\t"
+    )
+    io_handler.data = data_file
+    io_handler.data = io_handler.data.sort_values(
+        "time",
+        ignore_index=True
+    )
+    io_handler.get_models()
+    try:
+        sd = {"X": 0.}
+        for col in io_handler.data.columns[2:]:
+            sd.update({col: 0.5})
+    except Exception:
+        raise
+    io_handler.names = io_handler.data.columns[1:].to_list()
+    model = io_handler.models[-1]
+    model.get_params()
+    print(model)
+    keywargs = {
+        "sd": sd,
+        "model": model,
+        "mc": True,
+        "iterations": 100,
+        "debug_mode": True,
+    }
+    io_handler.res_path = Path(
+        r"C:\Users\legregam\Documents\Projets\PhysioFit\data\KEIO_test_data"
+        r"\KEIO_ROBOT6_1")
+    io_handler.initialize_fitter(kwargs=keywargs)
+    io_handler.fitter.optimize()
```

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/base_model.cpython-310.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/base_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_1.cpython-310.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_1.cpython-39.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_5.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 18 08:44:18 2023 UTC, .py size: 3323 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,200 @@
-00000000: 610d 0d0a 0000 0000 6258 3e64 fb0c 0000  a.......bX>d....
+00000000: 6f0d 0d0a 0000 0000 88c9 1d64 3810 0000  o..........d8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0173 6a00 0000 6400  .....@...sj...d.
+00000020: 0006 0000 0040 0000 0173 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 5a04 6401 6403 6c05 5a06 6401  d.l.Z.d.d.l.Z.d.
-00000050: 6404 6c07 6d08 5a08 6d09 5a09 0100 4700  d.l.m.Z.m.Z...G.
-00000060: 6405 6406 8400 6406 6508 8303 5a0a 650b  d.d...d.e...Z.e.
-00000070: 6407 6b02 7266 650a 6506 6a0c 6408 6409  d.k.rfe.e.j.d.d.
-00000080: 640a 8d02 8301 5a0d 650e 650f 650d 8301  d.....Z.e.e.e...
-00000090: 8301 0100 6403 5300 290b 7a32 0a4d 6f64  ....d.S.).z2.Mod
-000000a0: 756c 6520 636f 6e74 6169 6e69 6e67 2074  ule containing t
-000000b0: 6865 206d 6574 686f 6473 2075 7365 6420  he methods used 
-000000c0: 6279 2050 6879 7369 6f46 6974 2e0a e900  by PhysioFit....
-000000d0: 0000 0029 01da 0b61 6e6e 6f74 6174 696f  ...)...annotatio
-000000e0: 6e73 4e29 02da 054d 6f64 656c da06 426f  nsN)...Model..Bo
-000000f0: 756e 6473 6300 0000 0000 0000 0000 0000  undsc...........
-00000100: 0000 0000 0006 0000 0000 0000 0173 3c00  .............s<.
-00000110: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
-00000120: 6402 8408 5a03 6403 6404 8400 5a04 6505  d...Z.d.d...Z.e.
-00000130: 6405 6406 6406 6407 6408 9c04 6409 640a  d.d.d.d.d...d.d.
-00000140: 8404 8301 5a06 8700 0400 5a07 5300 290b  ....Z.....Z.S.).
-00000150: da0a 4368 696c 644d 6f64 656c 6302 0000  ..ChildModelc...
-00000160: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000170: 0003 0000 0173 2800 0000 7400 8300 a001  .....s(...t.....
-00000180: 7c01 a101 0100 6401 7c00 5f02 6402 7c00  |.....d.|._.d.|.
-00000190: 5f03 6400 7c00 5f04 6400 7c00 5f05 6400  _.d.|._.d.|._.d.
-000001a0: 5300 2903 4e7a 4753 7465 6164 792d 7374  S.).NzGSteady-st
-000001b0: 6174 6520 6261 7463 6820 6d6f 6465 6c20  ate batch model 
-000001c0: 7769 7468 206c 6167 2070 6861 7365 2061  with lag phase a
-000001d0: 6e64 2064 6567 7261 6461 7469 6f6e 206f  nd degradation o
-000001e0: 6620 6d65 7461 626f 6c69 7465 7320 e901  f metabolites ..
-000001f0: 0000 0029 06da 0573 7570 6572 da08 5f5f  ...)...super..__
-00000200: 696e 6974 5f5f da0a 6d6f 6465 6c5f 6e61  init__..model_na
-00000210: 6d65 da04 7669 6e69 da16 7061 7261 6d65  me..vini..parame
-00000220: 7465 7273 5f74 6f5f 6573 7469 6d61 7465  ters_to_estimate
-00000230: da10 6669 7865 645f 7061 7261 6d65 7465  ..fixed_paramete
-00000240: 7273 2902 da04 7365 6c66 da04 6461 7461  rs)...self..data
-00000250: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000260: 4743 3a5c 5573 6572 735c 6c65 6772 6567  GC:\Users\legreg
-00000270: 616d 5c50 7963 6861 726d 5072 6f6a 6563  am\PycharmProjec
-00000280: 7473 5c50 6879 7369 6f46 6974 5c70 6879  ts\PhysioFit\phy
-00000290: 7369 6f66 6974 5c6d 6f64 656c 735c 6d6f  siofit\models\mo
-000002a0: 6465 6c5f 312e 7079 7208 0000 000d 0000  del_1.pyr.......
-000002b0: 0073 0a00 0000 0002 0c01 0602 0601 0601  .s..............
-000002c0: 7a13 4368 696c 644d 6f64 656c 2e5f 5f69  z.ChildModel.__i
-000002d0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-000002e0: 0000 0200 0000 0700 0000 4300 0001 739c  ..........C...s.
-000002f0: 0000 007c 006a 007c 006a 007c 006a 0064  ...|.j.|.j.|.j.d
-00000300: 019c 037c 005f 0174 0264 0264 0364 0464  ...|._.t.d.d.d.d
-00000310: 057c 006a 03a0 04a1 0014 0066 0264 018d  .|.j.......f.d..
-00000320: 037c 005f 057c 006a 0644 005d 487d 017c  .|._.|.j.D.]H}.|
-00000330: 006a 01a0 077c 019b 0064 069d 027c 006a  .j...|...d...|.j
-00000340: 007c 019b 0064 079d 027c 006a 0069 02a1  .|...d...|.j.i..
-00000350: 0101 007c 006a 05a0 077c 019b 0064 069d  ...|.j...|...d..
-00000360: 0264 087c 019b 0064 079d 0264 0969 02a1  .d.|...d...d.i..
-00000370: 0101 0071 3864 0a64 0b64 0c84 007c 006a  ...q8d.d.d...|.j
-00000380: 0644 0083 0169 017c 005f 0864 0053 0029  .D...i.|._.d.S.)
-00000390: 0d4e 2903 5a03 585f 30da 026d 75da 0574  .N).Z.X_0..mu..t
-000003a0: 5f6c 6167 2902 e7fc a9f1 d24d 6250 3fe9  _lag)......MbP?.
-000003b0: 0a00 0000 2902 7215 0000 00e9 0300 0000  ....).r.........
-000003c0: 7201 0000 0067 0000 0000 0000 e03f da02  r....g.......?..
-000003d0: 5f71 5a03 5f4d 3029 0269 ceff ffff e932  _qZ._M0).i.....2
-000003e0: 0000 0029 0267 8ded b5a0 f7c6 b03e 7219  ...).g.......>r.
-000003f0: 0000 00da 0b44 6567 7261 6461 7469 6f6e  .....Degradation
-00000400: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000410: 0004 0000 0053 0000 0173 1200 0000 6900  .....S...s....i.
-00000420: 7c00 5d0a 7d01 7c01 6400 9302 7104 5300  |.].}.|.d...q.S.
-00000430: 2901 7201 0000 0072 1100 0000 2902 da02  ).r....r....)...
-00000440: 2e30 5a03 6d65 7472 1100 0000 7211 0000  .0Z.metr....r...
-00000450: 0072 1200 0000 da0a 3c64 6963 7463 6f6d  .r......<dictcom
-00000460: 703e 3000 0000 7302 0000 0006 017a 2943  p>0...s......z)C
-00000470: 6869 6c64 4d6f 6465 6c2e 6765 745f 7061  hildModel.get_pa
-00000480: 7261 6d73 2e3c 6c6f 6361 6c73 3e2e 3c64  rams.<locals>.<d
-00000490: 6963 7463 6f6d 703e 2909 720a 0000 0072  ictcomp>).r....r
-000004a0: 0b00 0000 7204 0000 00da 0b74 696d 655f  ....r......time_
-000004b0: 7665 6374 6f72 da03 6d61 78da 0662 6f75  vector..max..bou
-000004c0: 6e64 73da 0b6d 6574 6162 6f6c 6974 6573  nds..metabolites
-000004d0: da06 7570 6461 7465 720c 0000 0029 0272  ..updater....).r
-000004e0: 0d00 0000 5a0a 6d65 7461 626f 6c69 7465  ....Z.metabolite
-000004f0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000500: 0a67 6574 5f70 6172 616d 7316 0000 0073  .get_params....s
-00000510: 2e00 0000 0003 0401 0401 04fd 0805 0201  ................
-00000520: 0201 0201 10fd 0805 0a01 0602 0c01 0cfe  ................
-00000530: 02ff 0406 0602 0a01 0afe 02ff 0607 0801  ................
-00000540: 04ff 7a15 4368 696c 644d 6f64 656c 2e67  ..z.ChildModel.g
-00000550: 6574 5f70 6172 616d 73da 046c 6973 747a  et_params..listz
-00000560: 0a6e 702e 6e64 6172 7261 79da 0464 6963  .np.ndarray..dic
-00000570: 7429 04da 0b70 6172 616d 735f 6f70 7469  t)...params_opti
-00000580: da0b 6461 7461 5f6d 6174 7269 7872 1d00  ..data_matrixr..
-00000590: 0000 da0f 7061 7261 6d73 5f6e 6f6e 5f6f  ....params_non_o
-000005a0: 7074 6963 0400 0000 0000 0000 0000 0000  ptic............
-000005b0: 1100 0000 0800 0000 4300 0001 736a 0100  ........C...sj..
-000005c0: 0074 00a0 017c 01a1 017d 047c 0064 0119  .t...|...}.|.d..
-000005d0: 007d 057c 0064 0219 007d 067c 0064 0319  .}.|.d...}.|.d..
-000005e0: 007d 0774 00a0 027c 027c 076b 00a1 017d  .}.t...|.|.k...}
-000005f0: 0874 00a0 0374 047c 0883 0164 0218 0066  .t...t.|...d...f
-00000600: 017c 05a1 027d 097c 0574 00a0 057c 067c  .|...}.|.t...|.|
-00000610: 0274 047c 0883 0164 0218 0064 0085 0219  .t.|...d...d....
-00000620: 007c 0718 0014 00a1 0114 007d 0a74 006a  .|.........}.t.j
-00000630: 067c 097c 0a66 0264 0064 048d 027c 0464  .|.|.f.d.d...|.d
-00000640: 0064 0085 0264 0166 023c 0064 0564 0684  .d...d.f.<.d.d..
-00000650: 007c 0364 0719 00a0 07a1 0044 0083 017d  .|.d.......D...}
-00000660: 0b74 0864 0274 0974 047c 0083 0164 031b  .t.d.t.t.|...d..
-00000670: 0083 0183 0244 005d ae7d 0c7c 007c 0c64  .....D.].}.|.|.d
-00000680: 0314 0064 0217 0019 007d 0d7c 007c 0c64  ...d.....}.|.|.d
-00000690: 0314 0064 0317 0019 007d 0e7c 0b7c 0c64  ...d.....}.|.|.d
-000006a0: 0218 0019 007d 0f74 00a0 0374 047c 0883  .....}.t...t.|..
-000006b0: 0164 0218 0066 017c 0ea1 027d 107c 0d7c  .d...f.|...}.|.|
-000006c0: 057c 067c 0f17 001b 0014 0074 00a0 057c  .|.|.......t...|
-000006d0: 067c 027c 0718 0014 00a1 0174 00a0 057c  .|.|.......t...|
-000006e0: 0f0b 007c 027c 0718 0014 00a1 0118 0014  ...|.|..........
-000006f0: 007c 0e74 00a0 057c 0f0b 007c 0214 00a1  .|.t...|...|....
-00000700: 0114 0017 007d 0a74 006a 067c 107c 0a66  .....}.t.j.|.|.f
-00000710: 0264 0064 048d 027c 0464 0064 0085 027c  .d.d...|.d.d...|
-00000720: 0c66 023c 0071 b67c 0453 0029 084e 7201  .f.<.q.|.S.).Nr.
-00000730: 0000 0072 0600 0000 e902 0000 0029 01da  ...r.........)..
-00000740: 0461 7869 7363 0100 0000 0000 0000 0000  .axisc..........
-00000750: 0000 0200 0000 0300 0000 5300 0001 7310  ..........S...s.
-00000760: 0000 0067 007c 005d 087d 017c 0191 0271  ...g.|.].}.|...q
-00000770: 0453 0072 1100 0000 7211 0000 0029 0272  .S.r....r....).r
-00000780: 1b00 0000 da05 7661 6c75 6572 1100 0000  ......valuer....
-00000790: 7211 0000 0072 1200 0000 da0a 3c6c 6973  r....r......<lis
-000007a0: 7463 6f6d 703e 4e00 0000 f300 0000 007a  tcomp>N........z
-000007b0: 2743 6869 6c64 4d6f 6465 6c2e 7369 6d75  'ChildModel.simu
-000007c0: 6c61 7465 2e3c 6c6f 6361 6c73 3e2e 3c6c  late.<locals>.<l
-000007d0: 6973 7463 6f6d 703e 721a 0000 0029 0ada  istcomp>r....)..
-000007e0: 026e 70da 0a65 6d70 7479 5f6c 696b 65da  .np..empty_like.
-000007f0: 076e 6f6e 7a65 726f da04 6675 6c6c da03  .nonzero..full..
-00000800: 6c65 6eda 0365 7870 da0b 636f 6e63 6174  len..exp..concat
-00000810: 656e 6174 65da 0676 616c 7565 73da 0572  enate..values..r
-00000820: 616e 6765 da03 696e 7429 1172 2500 0000  ange..int).r%...
-00000830: 7226 0000 0072 1d00 0000 7227 0000 00da  r&...r....r'....
-00000840: 1073 696d 756c 6174 6564 5f6d 6174 7269  .simulated_matri
-00000850: 785a 0378 5f30 7213 0000 0072 1400 0000  xZ.x_0r....r....
-00000860: da03 6964 785a 0778 5f74 5f6c 6167 5a0c  ..idxZ.x_t_lagZ.
-00000870: 6d75 6c74 5f62 795f 7469 6d65 da0c 6669  mult_by_time..fi
-00000880: 7865 645f 7061 7261 6d73 da01 69da 0171  xed_params..i..q
-00000890: 5a03 6d5f 30da 016b 5a07 6d5f 745f 6c61  Z.m_0..kZ.m_t_la
-000008a0: 6772 1100 0000 7211 0000 0072 1200 0000  gr....r....r....
-000008b0: da08 7369 6d75 6c61 7465 3500 0000 733c  ..simulate5...s<
-000008c0: 0000 0000 080a 0308 0108 0108 030e 0316  ................
-000008d0: 0326 010a 0102 ff12 0216 021a 0110 0110  .&..............
-000008e0: 010c 0116 0112 010a ff02 0212 fe04 0206  ................
-000008f0: 0108 ff04 fe04 0504 0106 0102 fe14 057a  ...............z
-00000900: 1343 6869 6c64 4d6f 6465 6c2e 7369 6d75  .ChildModel.simu
-00000910: 6c61 7465 2908 da08 5f5f 6e61 6d65 5f5f  late)...__name__
-00000920: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000930: 7175 616c 6e61 6d65 5f5f 7208 0000 0072  qualname__r....r
-00000940: 2200 0000 da0c 7374 6174 6963 6d65 7468  ".....staticmeth
-00000950: 6f64 723d 0000 00da 0d5f 5f63 6c61 7373  odr=.....__class
-00000960: 6365 6c6c 5f5f 7211 0000 0072 1100 0000  cell__r....r....
-00000970: 720f 0000 0072 1200 0000 7205 0000 000b  r....r....r.....
-00000980: 0000 0073 0800 0000 0802 0c09 081f 0201  ...s............
-00000990: 7205 0000 00da 085f 5f6d 6169 6e5f 5f7a  r......__main__z
-000009a0: 6143 3a5c 5573 6572 735c 6c65 6772 6567  aC:\Users\legreg
-000009b0: 616d 5c44 6f63 756d 656e 7473 5c50 726f  am\Documents\Pro
-000009c0: 6a65 7473 5c50 6879 7369 6f46 6974 5c64  jets\PhysioFit\d
-000009d0: 6174 615c 4b45 494f 5f74 6573 745f 6461  ata\KEIO_test_da
-000009e0: 7461 5c4b 4549 4f5f 524f 424f 5436 5f31  ta\KEIO_ROBOT6_1
-000009f0: 5c4b 4549 4f5f 524f 424f 5436 5f31 2e74  \KEIO_ROBOT6_1.t
-00000a00: 7376 fa01 0929 01da 0373 6570 2910 da07  sv...)...sep)...
-00000a10: 5f5f 646f 635f 5fda 0a5f 5f66 7574 7572  __doc__..__futur
-00000a20: 655f 5f72 0200 0000 da05 6e75 6d70 7972  e__r......numpyr
-00000a30: 2d00 0000 da06 7061 6e64 6173 da02 7064  -.....pandas..pd
-00000a40: da1b 7068 7973 696f 6669 742e 6d6f 6465  ..physiofit.mode
-00000a50: 6c73 2e62 6173 655f 6d6f 6465 6c72 0300  ls.base_modelr..
-00000a60: 0000 7204 0000 0072 0500 0000 723e 0000  ..r....r....r>..
-00000a70: 00da 0872 6561 645f 6373 76da 056d 6f64  ...read_csv..mod
-00000a80: 656c da05 7072 696e 74da 0474 7970 6572  el..print..typer
-00000a90: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000aa0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000ab0: 0073 1a00 0000 0403 0c02 0801 0802 1002  .s..............
-00000ac0: 1057 0801 0201 0401 0202 02fd 04ff 0406  .W..............
+00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
+00000060: 0100 4700 6406 6407 8400 6407 6508 8303  ..G.d.d...d.e...
+00000070: 5a0a 650b 6408 6b02 726a 6401 6409 6c0c  Z.e.d.k.rjd.d.l.
+00000080: 6d0d 5a0d 0100 650d 8300 5a0e 650e a00f  m.Z...e...Z.e...
+00000090: 640a a101 5a10 6510 a011 640b a101 5a10  d...Z.e...d...Z.
+000000a0: 650a 6510 8301 5a12 6512 a013 a100 0100  e.e...Z.e.......
+000000b0: 640c 640d 8400 6512 6a14 a015 a100 4400  d.d...e.j.....D.
+000000c0: 8301 5a16 650a a017 6516 6512 6a10 6512  ..Z.e...e.e.j.e.
+000000d0: 6a18 6403 a104 5a19 651a 640e 6519 6a1b  j.d...Z.e.d.e.j.
+000000e0: 9b00 9d02 8301 0100 651a 640f 6504 a01c  ........e.d.e...
+000000f0: 6519 6a1d a101 9b00 9d02 8301 0100 6403  e.j...........d.
+00000100: 5300 6403 5300 2910 7a3e 0a4d 6f64 756c  S.d.S.).z>.Modul
+00000110: 6520 636f 6e74 6169 6e69 6e67 2061 2064  e containing a d
+00000120: 796e 616d 6963 2067 726f 7774 6820 616e  ynamic growth an
+00000130: 6420 666c 7578 2065 7374 696d 6174 696f  d flux estimatio
+00000140: 6e20 6d6f 6465 6c0a e900 0000 0029 01da  n model......)..
+00000150: 0b61 6e6e 6f74 6174 696f 6e73 4e29 01da  .annotationsN)..
+00000160: 0973 6f6c 7665 5f69 7670 2902 da05 4d6f  .solve_ivp)...Mo
+00000170: 6465 6cda 0642 6f75 6e64 7363 0000 0000  del..Boundsc....
+00000180: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000190: 0000 0001 7332 0000 0065 005a 0164 005a  ....s2...e.Z.d.Z
+000001a0: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
+000001b0: 0484 005a 0465 0564 0e64 0c64 0d84 0483  ...Z.e.d.d.d....
+000001c0: 015a 0687 0004 005a 0753 0029 0fda 0a43  .Z.....Z.S.)...C
+000001d0: 6869 6c64 4d6f 6465 6c63 0200 0000 0000  hildModelc......
+000001e0: 0000 0000 0000 0200 0000 0300 0000 0300  ................
+000001f0: 0001 7322 0000 0074 0083 00a0 017c 01a1  ..s"...t.....|..
+00000200: 0101 0064 017c 005f 0264 027c 005f 0364  ...d.|._.d.|._.d
+00000210: 007c 005f 0464 0053 0029 034e 7a2c 4479  .|._.d.S.).Nz,Dy
+00000220: 6e61 6d69 6320 4d6f 6e6f 6420 6d6f 6465  namic Monod mode
+00000230: 6c20 2831 2073 7562 7374 7261 7465 2c20  l (1 substrate, 
+00000240: 3120 7072 6f64 7563 7429 e901 0000 0029  1 product).....)
+00000250: 05da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
+00000260: 5f5f da0a 6d6f 6465 6c5f 6e61 6d65 da04  __..model_name..
+00000270: 7669 6e69 da16 7061 7261 6d65 7465 7273  vini..parameters
+00000280: 5f74 6f5f 6573 7469 6d61 7465 2902 da04  _to_estimate)...
+00000290: 7365 6c66 da04 6461 7461 a901 da09 5f5f  self..data....__
+000002a0: 636c 6173 735f 5fa9 00fa 5843 3a5c 5573  class__...XC:\Us
+000002b0: 6572 735c 6d69 6c6c 6172 645c 446f 6375  ers\millard\Docu
+000002c0: 6d65 6e74 735c 4749 545c 5068 7973 696f  ments\GIT\Physio
+000002d0: 4669 745c 5068 7973 696f 4669 745c 5068  Fit\PhysioFit\Ph
+000002e0: 7973 696f 4669 745c 7068 7973 696f 6669  ysioFit\physiofi
+000002f0: 745c 6d6f 6465 6c73 5c6d 6f64 656c 5f35  t\models\model_5
+00000300: 2e70 7972 0900 0000 0d00 0000 7308 0000  .pyr........s...
+00000310: 000c 0206 0106 010a 017a 1343 6869 6c64  .........z.Child
+00000320: 4d6f 6465 6c2e 5f5f 696e 6974 5f5f 6301  Model.__init__c.
+00000330: 0000 0000 0000 0000 0000 0002 0000 0009  ................
+00000340: 0000 0043 0000 0173 0601 0000 7c00 6a00  ...C...s....|.j.
+00000350: 7c00 6a00 6401 9c02 7c00 5f01 7402 6402  |.j.d...|._.t.d.
+00000360: 6403 6401 8d02 7c00 5f03 7c00 6a04 4400  d.d...|._.|.j.D.
+00000370: 5d35 7d01 7c01 a005 6404 a101 7247 7c00  ]5}.|...d...rG|.
+00000380: 6a01 a006 7c01 9b00 6405 9d02 7c00 6a00  j...|...d...|.j.
+00000390: 7c01 9b00 6406 9d02 7c00 6a00 7c01 9b00  |...d...|.j.|...
+000003a0: 6407 9d02 6408 6903 a101 0100 7c00 6a03  d...d.i.....|.j.
+000003b0: a006 7c01 9b00 6405 9d02 6409 7c01 9b00  ..|...d...d.|...
+000003c0: 6406 9d02 6409 7c01 9b00 6407 9d02 6409  d...d.|...d...d.
+000003d0: 6903 a101 0100 0100 7148 7112 7c00 6a04  i.......qHq.|.j.
+000003e0: 4400 5d2a 7d01 7c01 a005 640a a101 7275  D.]*}.|...d...ru
+000003f0: 7c00 6a01 a006 7c01 9b00 640b 9d02 7c00  |.j...|...d...|.
+00000400: 6a00 7c01 9b00 640c 9d02 6408 6902 a101  j.|...d...d.i...
+00000410: 0100 7c00 6a03 a006 7c01 9b00 640b 9d02  ..|.j...|...d...
+00000420: 6409 7c01 9b00 640c 9d02 6409 6902 a101  d.|...d...d.i...
+00000430: 0100 0100 7176 714b 7407 7c00 6a01 8301  ....qvqKt.|.j...
+00000440: 640d 6b03 7281 7408 640e 8301 8201 6400  d.k.r.t.d.....d.
+00000450: 5300 290f 4e29 02da 0358 5f30 da04 795f  S.).N)...X_0..y_
+00000460: 424d 2902 e7fc a9f1 d24d 6250 3fe9 0a00  BM)......MbP?...
+00000470: 0000 2902 7215 0000 00e9 0300 0000 5a02  ..).r.........Z.
+00000480: 535f 5a03 5f6b 6d5a 065f 7173 6d61 785a  S_Z._kmZ._qsmaxZ
+00000490: 045f 735f 30e9 6400 0000 2902 678d edb5  ._s_0.d...).g...
+000004a0: a0f7 c6b0 3e72 1800 0000 5a02 505f 5a04  ....>r....Z.P_Z.
+000004b0: 5f79 5f50 5a04 5f70 5f30 e907 0000 007a  _y_PZ._p_0.....z
+000004c0: 8854 6869 7320 6d6f 6465 6c20 6578 7065  .This model expe
+000004d0: 6374 7320 3220 6d65 7461 626f 6c69 7465  cts 2 metabolite
+000004e0: 7320 696e 2074 6865 2064 6174 6120 6669  s in the data fi
+000004f0: 6c65 2028 3120 7375 6273 7472 6174 6520  le (1 substrate 
+00000500: 7769 7468 206e 616d 6520 7374 6172 7469  with name starti
+00000510: 6e67 2077 6974 6820 2753 5f27 2061 6e64  ng with 'S_' and
+00000520: 2031 2070 726f 6475 6374 2077 6974 6820   1 product with 
+00000530: 6e61 6d65 2073 7461 7274 696e 6720 7769  name starting wi
+00000540: 7468 2027 505f 2729 2e29 0972 0b00 0000  th 'P_').).r....
+00000550: 720c 0000 0072 0500 0000 da06 626f 756e  r....r......boun
+00000560: 6473 da0b 6d65 7461 626f 6c69 7465 73da  ds..metabolites.
+00000570: 0a73 7461 7274 7377 6974 68da 0675 7064  .startswith..upd
+00000580: 6174 65da 036c 656e da0a 5661 6c75 6545  ate..len..ValueE
+00000590: 7272 6f72 2902 720d 0000 00da 0a6d 6574  rror).r......met
+000005a0: 6162 6f6c 6974 6572 1100 0000 7211 0000  aboliter....r...
+000005b0: 0072 1200 0000 da0a 6765 745f 7061 7261  .r......get_para
+000005c0: 6d73 1400 0000 7350 0000 0004 0304 0108  ms....sP........
+000005d0: fe02 0502 0102 0108 fe0a 050a 0106 010c  ................
+000005e0: 020c 010a 0102 fd04 ff06 070a 020a 010a  ................
+000005f0: 0102 fd04 ff04 0702 f10a 110a 0106 010c  ................
+00000600: 020a 0102 fe04 ff06 070a 020a 0102 fe04  ................
+00000610: ff04 0602 f20e 1008 0104 ff7a 1543 6869  ...........z.Chi
+00000620: 6c64 4d6f 6465 6c2e 6765 745f 7061 7261  ldModel.get_para
+00000630: 6d73 da0b 7061 7261 6d73 5f6f 7074 69da  ms..params_opti.
+00000640: 046c 6973 74da 0b64 6174 615f 6d61 7472  .list..data_matr
+00000650: 6978 fa0a 6e70 2e6e 6461 7272 6179 da0b  ix..np.ndarray..
+00000660: 7469 6d65 5f76 6563 746f 72da 0f70 6172  time_vector..par
+00000670: 616d 735f 6e6f 6e5f 6f70 7469 da04 6469  ams_non_opti..di
+00000680: 6374 6304 0000 0000 0000 0000 0000 000f  ctc.............
+00000690: 0000 0008 0000 0043 0000 0173 8600 0000  .......C...s....
+000006a0: 7c00 6401 1900 7d04 7c00 6402 1900 7d05  |.d...}.|.d...}.
+000006b0: 7c00 6403 1900 7d06 7c00 6404 1900 7d07  |.d...}.|.d...}.
+000006c0: 7c00 6405 1900 7d08 7c00 6406 1900 7d09  |.d...}.|.d...}.
+000006d0: 7c00 6407 1900 7d0a 7c05 7c09 7c06 7c07  |.d...}.|.|.|.|.
+000006e0: 6604 7d0b 7c04 7c08 7c0a 6703 7d0c 6408  f.}.|.|.|.g.}.d.
+000006f0: 6409 8400 7d0d 7400 7c0d 7401 a002 7c02  d...}.t.|.t...|.
+00000700: a101 7401 a003 7c02 a101 6602 7c0c 7c0b  ..t...|...f.|.|.
+00000710: 640a 7404 7c02 8301 640b 8d06 7d0e 7c0e  d.t.|...d...}.|.
+00000720: 6a05 6a06 5300 290c 4e72 0100 0000 7207  j.j.S.).Nr....r.
+00000730: 0000 00e9 0200 0000 7217 0000 00e9 0400  ........r.......
+00000740: 0000 e905 0000 00e9 0600 0000 6306 0000  ............c...
+00000750: 0000 0000 0000 0000 000e 0000 0004 0000  ................
+00000760: 0053 0000 0173 5400 0000 7c01 6401 1900  .S...sT...|.d...
+00000770: 7d06 7c01 6402 1900 7d07 7c05 7c06 7c04  }.|.d...}.|.|.|.
+00000780: 7c06 1700 1b00 1400 7d08 7c02 7c08 1400  |.......}.|.|...
+00000790: 7d09 7c03 7c08 1400 7d0a 7c09 7c07 1400  }.|.|...}.|.|...
+000007a0: 7d0b 7c08 0b00 7c07 1400 7d0c 7c0a 7c07  }.|...|...}.|.|.
+000007b0: 1400 7d0d 7c0b 7c0c 7c0d 6603 5300 2903  ..}.|.|.|.f.S.).
+000007c0: 4e72 0100 0000 7207 0000 0072 1100 0000  Nr....r....r....
+000007d0: 290e da01 74da 0573 7461 7465 7214 0000  )...t..stater...
+000007e0: 00da 0379 5f50 da02 6b6d da05 7173 6d61  ...y_P..km..qsma
+000007f0: 785a 0373 5f74 5a03 785f 745a 0471 735f  xZ.s_tZ.x_tZ.qs_
+00000800: 745a 046d 755f 745a 0471 705f 74da 0264  tZ.mu_tZ.qp_t..d
+00000810: 78da 0264 73da 0264 7072 1100 0000 7211  x..ds..dpr....r.
+00000820: 0000 0072 1200 0000 da14 6361 6c63 756c  ...r......calcul
+00000830: 6174 655f 6465 7269 7661 7469 7665 5c00  ate_derivative\.
+00000840: 0000 7312 0000 0008 0308 0110 0308 0108  ..s.............
+00000850: 0108 030a 0108 010a 027a 3143 6869 6c64  .........z1Child
+00000860: 4d6f 6465 6c2e 7369 6d75 6c61 7465 2e3c  Model.simulate.<
+00000870: 6c6f 6361 6c73 3e2e 6361 6c63 756c 6174  locals>.calculat
+00000880: 655f 6465 7269 7661 7469 7665 da05 4c53  e_derivative..LS
+00000890: 4f44 4129 06da 0366 756e da06 745f 7370  ODA)...fun..t_sp
+000008a0: 616e da02 7930 da04 6172 6773 da06 6d65  an..y0..args..me
+000008b0: 7468 6f64 da06 745f 6576 616c 2907 7203  thod..t_eval).r.
+000008c0: 0000 00da 026e 70da 036d 696e da03 6d61  .....np..min..ma
+000008d0: 7872 2300 0000 da01 79da 0154 290f 7222  xr#.....y..T).r"
+000008e0: 0000 0072 2400 0000 7226 0000 0072 2700  ...r$...r&...r'.
+000008f0: 0000 da03 785f 3072 1400 0000 7230 0000  ....x_0r....r0..
+00000900: 0072 3100 0000 5a03 735f 3072 2f00 0000  .r1...Z.s_0r/...
+00000910: 5a03 705f 30da 0670 6172 616d 7372 2e00  Z.p_0..paramsr..
+00000920: 0000 7235 0000 00da 0373 6f6c 7211 0000  ..r5.....solr...
+00000930: 0072 1100 0000 7212 0000 00da 0873 696d  .r....r......sim
+00000940: 756c 6174 6547 0000 0073 2600 0000 0809  ulateG...s&.....
+00000950: 0801 0801 0801 0801 0801 0801 0c01 0a03  ................
+00000960: 0802 0213 0201 1201 0201 0201 0201 0601  ................
+00000970: 06fa 0809 7a13 4368 696c 644d 6f64 656c  ....z.ChildModel
+00000980: 2e73 696d 756c 6174 6529 0872 2200 0000  .simulate).r"...
+00000990: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+000009a0: 2600 0000 7225 0000 0072 2700 0000 7228  &...r%...r'...r(
+000009b0: 0000 0029 08da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+000009c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000009d0: 7561 6c6e 616d 655f 5f72 0900 0000 7221  ualname__r....r!
+000009e0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
+000009f0: 6472 4500 0000 da0d 5f5f 636c 6173 7363  drE.....__classc
+00000a00: 656c 6c5f 5f72 1100 0000 7211 0000 0072  ell__r....r....r
+00000a10: 0f00 0000 7212 0000 0072 0600 0000 0b00  ....r....r......
+00000a20: 0000 730a 0000 0008 000c 0208 0702 3314  ..s...........3.
+00000a30: 0172 0600 0000 da08 5f5f 6d61 696e 5f5f  .r......__main__
+00000a40: 2901 da09 496f 4861 6e64 6c65 727a 5a43  )...IoHandlerzZC
+00000a50: 3a5c 5573 6572 735c 6c65 6772 6567 616d  :\Users\legregam
+00000a60: 5c50 7963 6861 726d 5072 6f6a 6563 7473  \PycharmProjects
+00000a70: 5c50 6879 7369 6f46 6974 5c64 6174 615c  \PhysioFit\data\
+00000a80: 4b45 494f 5f74 6573 745f 6461 7461 5c6f  KEIO_test_data\o
+00000a90: 6465 5f74 6573 745c 4b45 494f 5f52 4f42  de_test\KEIO_ROB
+00000aa0: 4f54 365f 312e 7473 76da 0474 696d 6563  OT6_1.tsv..timec
+00000ab0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000ac0: 0300 0000 4300 0001 7310 0000 0067 007c  ....C...s....g.|
+00000ad0: 005d 047d 017c 0191 0271 0253 0072 1100  .].}.|...q.S.r..
+00000ae0: 0000 7211 0000 0029 02da 022e 30da 0570  ..r....)....0..p
+00000af0: 6172 616d 7211 0000 0072 1100 0000 7212  aramr....r....r.
+00000b00: 0000 00da 0a3c 6c69 7374 636f 6d70 3e84  .....<listcomp>.
+00000b10: 0000 0073 0200 0000 1000 7250 0000 007a  ...s......rP...z
+00000b20: 0754 696d 6573 3a20 7a08 5661 6c75 6573  .Times: z.Values
+00000b30: 3a20 291e da07 5f5f 646f 635f 5fda 0a5f  : )...__doc__.._
+00000b40: 5f66 7574 7572 655f 5f72 0200 0000 da05  _future__r......
+00000b50: 6e75 6d70 7972 3d00 0000 da0f 7363 6970  numpyr=.....scip
+00000b60: 792e 696e 7465 6772 6174 6572 0300 0000  y.integrater....
+00000b70: da1b 7068 7973 696f 6669 742e 6d6f 6465  ..physiofit.mode
+00000b80: 6c73 2e62 6173 655f 6d6f 6465 6c72 0400  ls.base_modelr..
+00000b90: 0000 7205 0000 0072 0600 0000 7246 0000  ..r....r....rF..
+00000ba0: 00da 1170 6879 7369 6f66 6974 2e62 6173  ...physiofit.bas
+00000bb0: 652e 696f 724c 0000 00da 0269 6fda 0972  e.iorL.....io..r
+00000bc0: 6561 645f 6461 7461 720e 0000 00da 0b73  ead_datar......s
+00000bd0: 6f72 745f 7661 6c75 6573 da05 6d6f 6465  ort_values..mode
+00000be0: 6c72 2100 0000 720c 0000 00da 0676 616c  lr!...r......val
+00000bf0: 7565 7372 4300 0000 7245 0000 0072 2600  uesrC...rE...r&.
+00000c00: 0000 7244 0000 00da 0570 7269 6e74 722d  ..rD.....printr-
+00000c10: 0000 00da 0561 7272 6179 7240 0000 0072  .....arrayr@...r
+00000c20: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00000c30: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000c40: 0073 2e00 0000 0400 0c03 0802 0c01 1002  .s..............
+00000c50: 1002 086f 0c02 0602 0a01 0a01 0802 0801  ...o............
+00000c60: 1401 0401 0201 0401 0401 0201 04fc 1006  ................
+00000c70: 1a01 04ee                                ....
```

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_2.cpython-310.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_2.cpython-39.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_3.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 18 08:44:18 2023 UTC, .py size: 2645 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,152 @@
-00000000: 610d 0d0a 0000 0000 6258 3e64 550a 0000  a.......bX>dU...
+00000000: 6f0d 0d0a 0000 0000 b081 1d64 7b09 0000  o..........d{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6506 8303 5a08 6403 5300 2907 7a32 0a4d  e...Z.d.S.).z2.M
 00000070: 6f64 756c 6520 636f 6e74 6169 6e69 6e67  odule containing
 00000080: 2074 6865 206d 6574 686f 6473 2075 7365   the methods use
 00000090: 6420 6279 2050 6879 7369 6f46 6974 2e0a  d by PhysioFit..
 000000a0: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
 000000b0: 696f 6e73 4e29 02da 054d 6f64 656c da06  ionsN)...Model..
 000000c0: 426f 756e 6473 6300 0000 0000 0000 0000  Boundsc.........
-000000d0: 0000 0000 0000 0006 0000 0000 0000 0173  ...............s
-000000e0: 3c00 0000 6500 5a01 6400 5a02 8700 6601  <...e.Z.d.Z...f.
+000000d0: 0000 0000 0000 0004 0000 0000 0000 0173  ...............s
+000000e0: 3200 0000 6500 5a01 6400 5a02 8700 6601  2...e.Z.d.Z...f.
 000000f0: 6401 6402 8408 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00000100: 6505 6405 6406 6406 6407 6408 9c04 6409  e.d.d.d.d.d...d.
-00000110: 640a 8404 8301 5a06 8700 0400 5a07 5300  d.....Z.....Z.S.
-00000120: 290b da0a 4368 696c 644d 6f64 656c 6302  )...ChildModelc.
-00000130: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000140: 0000 0003 0000 0173 2800 0000 7400 8300  .......s(...t...
-00000150: a001 7c01 a101 0100 6401 7c00 5f02 6402  ..|.....d.|._.d.
-00000160: 7c00 5f03 6400 7c00 5f04 6400 7c00 5f05  |._.d.|._.d.|._.
-00000170: 6400 5300 2903 4e7a 2753 7465 6164 792d  d.S.).Nz'Steady-
-00000180: 7374 6174 6520 6261 7463 6820 6d6f 6465  state batch mode
-00000190: 6c20 7769 7468 206c 6167 2070 6861 7365  l with lag phase
-000001a0: e901 0000 0029 06da 0573 7570 6572 da08  .....)...super..
-000001b0: 5f5f 696e 6974 5f5f da0a 6d6f 6465 6c5f  __init__..model_
-000001c0: 6e61 6d65 da04 7669 6e69 da16 7061 7261  name..vini..para
-000001d0: 6d65 7465 7273 5f74 6f5f 6573 7469 6d61  meters_to_estima
-000001e0: 7465 da10 6669 7865 645f 7061 7261 6d65  te..fixed_parame
-000001f0: 7465 7273 2902 da04 7365 6c66 da04 6461  ters)...self..da
-00000200: 7461 a901 da09 5f5f 636c 6173 735f 5fa9  ta....__class__.
-00000210: 00fa 4743 3a5c 5573 6572 735c 6c65 6772  ..GC:\Users\legr
-00000220: 6567 616d 5c50 7963 6861 726d 5072 6f6a  egam\PycharmProj
-00000230: 6563 7473 5c50 6879 7369 6f46 6974 5c70  ects\PhysioFit\p
-00000240: 6879 7369 6f66 6974 5c6d 6f64 656c 735c  hysiofit\models\
-00000250: 6d6f 6465 6c5f 322e 7079 7208 0000 000d  model_2.pyr.....
-00000260: 0000 0073 0a00 0000 0002 0c01 0601 0601  ...s............
-00000270: 0601 7a13 4368 696c 644d 6f64 656c 2e5f  ..z.ChildModel._
-00000280: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000290: 0000 0000 0200 0000 0700 0000 4300 0001  ............C...
-000002a0: 7384 0000 007c 006a 007c 006a 007c 006a  s....|.j.|.j.|.j
-000002b0: 0064 019c 037c 005f 0174 0264 0264 0364  .d...|._.t.d.d.d
-000002c0: 0464 057c 006a 03a0 04a1 0014 0066 0264  .d.|.j.......f.d
-000002d0: 019c 0383 017c 005f 057c 006a 0644 005d  .....|._.|.j.D.]
-000002e0: 447d 017c 006a 01a0 077c 019b 0064 069d  D}.|.j...|...d..
-000002f0: 0264 077c 019b 0064 089d 0264 0769 02a1  .d.|...d...d.i..
-00000300: 0101 007c 006a 05a0 077c 019b 0064 069d  ...|.j...|...d..
-00000310: 0264 097c 019b 0064 089d 0264 0a69 02a1  .d.|...d...d.i..
-00000320: 0101 0071 3a64 0053 0029 0b4e 2903 da03  ...q:d.S.).N)...
-00000330: 585f 30da 026d 75da 0574 5f6c 6167 2902  X_0..mu..t_lag).
-00000340: e7fc a9f1 d24d 6250 3fe9 0a00 0000 2902  .....MbP?.....).
-00000350: 7216 0000 00e9 0300 0000 7201 0000 0067  r.........r....g
-00000360: 0000 0000 0000 e03f da02 5f71 7206 0000  .......?.._qr...
-00000370: 00da 035f 4d30 2902 69ce ffff ffe9 3200  ..._M0).i.....2.
-00000380: 0000 2902 678d edb5 a0f7 c6b0 3e72 1b00  ..).g.......>r..
-00000390: 0000 2908 720a 0000 0072 0b00 0000 7204  ..).r....r....r.
-000003a0: 0000 00da 0b74 696d 655f 7665 6374 6f72  .....time_vector
-000003b0: da03 6d61 78da 0662 6f75 6e64 73da 0b6d  ..max..bounds..m
-000003c0: 6574 6162 6f6c 6974 6573 da06 7570 6461  etabolites..upda
-000003d0: 7465 2902 720d 0000 00da 0a6d 6574 6162  te).r......metab
-000003e0: 6f6c 6974 6572 1100 0000 7211 0000 0072  oliter....r....r
-000003f0: 1200 0000 da0a 6765 745f 7061 7261 6d73  ......get_params
-00000400: 1500 0000 7328 0000 0000 0304 0104 0104  ....s(..........
-00000410: fd08 0502 0102 0102 0110 fd0a 050a 0106  ................
-00000420: 020a 010a fe02 ff04 0606 020a 010a fe02  ................
-00000430: ff7a 1543 6869 6c64 4d6f 6465 6c2e 6765  .z.ChildModel.ge
-00000440: 745f 7061 7261 6d73 da04 6c69 7374 7a0a  t_params..listz.
-00000450: 6e70 2e6e 6461 7272 6179 7a0b 6469 6374  np.ndarrayz.dict
-00000460: 207c 206c 6973 7429 04da 0b70 6172 616d   | list)...param
-00000470: 735f 6f70 7469 da0b 6461 7461 5f6d 6174  s_opti..data_mat
-00000480: 7269 7872 1c00 0000 da0f 7061 7261 6d73  rixr......params
-00000490: 5f6e 6f6e 5f6f 7074 6963 0400 0000 0000  _non_optic......
-000004a0: 0000 0000 0000 1000 0000 0700 0000 4300  ..............C.
-000004b0: 0001 7328 0100 0074 00a0 017c 01a1 017d  ..s(...t...|...}
-000004c0: 047c 0064 0119 007d 057c 0064 0219 007d  .|.d...}.|.d...}
-000004d0: 067c 0064 0319 007d 0774 00a0 027c 027c  .|.d...}.t...|.|
-000004e0: 076b 00a1 017d 0874 00a0 0374 047c 0883  .k...}.t...t.|..
-000004f0: 0164 0218 0066 017c 05a1 027d 097c 0574  .d...f.|...}.|.t
-00000500: 00a0 057c 067c 0274 047c 0883 0164 0218  ...|.|.t.|...d..
-00000510: 0064 0085 0219 007c 0718 0014 00a1 0114  .d.....|........
-00000520: 007d 0a74 006a 067c 097c 0a66 0264 0064  .}.t.j.|.|.f.d.d
-00000530: 048d 027c 0464 0064 0085 0264 0166 023c  ...|.d.d...d.f.<
-00000540: 0074 00a0 057c 067c 027c 0718 0014 00a1  .t...|.|.|......
-00000550: 0164 0218 007d 0b74 0764 0274 0874 047c  .d...}.t.d.t.t.|
-00000560: 0083 0164 031b 0083 0183 0244 005d 6c7d  ...d.......D.]l}
-00000570: 0c7c 007c 0c64 0314 0064 0217 0019 007d  .|.|.d...d.....}
-00000580: 0d7c 007c 0c64 0314 0064 0317 0019 007d  .|.|.d...d.....}
-00000590: 0e74 00a0 0374 047c 0883 0164 0218 0066  .t...t.|...d...f
-000005a0: 017c 0ea1 027d 0f7c 0d7c 057c 061b 0014  .|...}.|.|.|....
-000005b0: 007c 0b14 007c 0e17 007d 0a74 006a 067c  .|...|...}.t.j.|
-000005c0: 0f7c 0a66 0264 0064 048d 027c 0464 0064  .|.f.d.d...|.d.d
-000005d0: 0085 027c 0c66 023c 0071 b67c 0453 0029  ...|.f.<.q.|.S.)
-000005e0: 054e 7201 0000 0072 0600 0000 e902 0000  .Nr....r........
-000005f0: 0029 01da 0461 7869 7329 09da 026e 70da  .)...axis)...np.
-00000600: 0a65 6d70 7479 5f6c 696b 65da 076e 6f6e  .empty_like..non
-00000610: 7a65 726f da04 6675 6c6c da03 6c65 6eda  zero..full..len.
-00000620: 0365 7870 da0b 636f 6e63 6174 656e 6174  .exp..concatenat
-00000630: 65da 0572 616e 6765 da03 696e 7429 1072  e..range..int).r
-00000640: 2400 0000 7225 0000 0072 1c00 0000 7226  $...r%...r....r&
-00000650: 0000 00da 1073 696d 756c 6174 6564 5f6d  .....simulated_m
-00000660: 6174 7269 78da 0378 5f30 7214 0000 0072  atrix..x_0r....r
-00000670: 1500 0000 da03 6964 78da 0778 5f74 5f6c  ......idx..x_t_l
-00000680: 6167 da0c 6d75 6c74 5f62 795f 7469 6d65  ag..mult_by_time
-00000690: 5a0c 6578 705f 6d75 5f74 5f6c 6167 da01  Z.exp_mu_t_lag..
-000006a0: 69da 0171 da03 6d5f 30da 076d 5f74 5f6c  i..q..m_0..m_t_l
-000006b0: 6167 7211 0000 0072 1100 0000 7212 0000  agr....r....r...
-000006c0: 00da 0873 696d 756c 6174 652f 0000 0073  ...simulate/...s
-000006d0: 2c00 0000 0008 0a01 0801 0801 0803 0e03  ,...............
-000006e0: 1603 2604 0401 0601 02fe 1204 1602 1a01  ..&.............
-000006f0: 1001 1001 1601 1401 0401 0601 02fe 1405  ................
-00000700: 7a13 4368 696c 644d 6f64 656c 2e73 696d  z.ChildModel.sim
-00000710: 756c 6174 6529 08da 085f 5f6e 616d 655f  ulate)...__name_
-00000720: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000730: 5f71 7561 6c6e 616d 655f 5f72 0800 0000  _qualname__r....
-00000740: 7222 0000 00da 0c73 7461 7469 636d 6574  r".....staticmet
-00000750: 686f 6472 3b00 0000 da0d 5f5f 636c 6173  hodr;.....__clas
-00000760: 7363 656c 6c5f 5f72 1100 0000 7211 0000  scell__r....r...
-00000770: 0072 0f00 0000 7212 0000 0072 0500 0000  .r....r....r....
-00000780: 0b00 0000 7308 0000 0008 020c 0808 1a02  ....s...........
-00000790: 0172 0500 0000 2909 da07 5f5f 646f 635f  .r....)...__doc_
-000007a0: 5fda 0a5f 5f66 7574 7572 655f 5f72 0200  _..__future__r..
-000007b0: 0000 da05 6e75 6d70 7972 2900 0000 da1b  ....numpyr).....
-000007c0: 7068 7973 696f 6669 742e 6d6f 6465 6c73  physiofit.models
-000007d0: 2e62 6173 655f 6d6f 6465 6c72 0300 0000  .base_modelr....
-000007e0: 7204 0000 0072 0500 0000 7211 0000 0072  r....r....r....r
-000007f0: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
-00000800: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000810: 0004 040c 0108 0210 03                   .........
+00000100: 6505 640e 640c 640d 8404 8301 5a06 8700  e.d.d.d.....Z...
+00000110: 0400 5a07 5300 290f da0a 4368 696c 644d  ..Z.S.)...ChildM
+00000120: 6f64 656c 6302 0000 0000 0000 0000 0000  odelc...........
+00000130: 0002 0000 0003 0000 0003 0000 0173 2800  .............s(.
+00000140: 0000 7400 8300 a001 7c01 a101 0100 6401  ..t.....|.....d.
+00000150: 7c00 5f02 6402 7c00 5f03 6400 7c00 5f04  |._.d.|._.d.|._.
+00000160: 6400 7c00 5f05 6400 5300 2903 4e7a 3853  d.|._.d.S.).Nz8S
+00000170: 7465 6164 792d 7374 6174 6520 6261 7463  teady-state batc
+00000180: 6820 6d6f 6465 6c20 7769 7468 2064 6567  h model with deg
+00000190: 7261 6461 7469 6f6e 206f 6620 6d65 7461  radation of meta
+000001a0: 626f 6c69 7465 73e9 0100 0000 2906 da05  bolites.....)...
+000001b0: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
+000001c0: 0a6d 6f64 656c 5f6e 616d 65da 0476 696e  .model_name..vin
+000001d0: 69da 1670 6172 616d 6574 6572 735f 746f  i..parameters_to
+000001e0: 5f65 7374 696d 6174 65da 1066 6978 6564  _estimate..fixed
+000001f0: 5f70 6172 616d 6574 6572 7329 02da 0473  _parameters)...s
+00000200: 656c 66da 0464 6174 61a9 01da 095f 5f63  elf..data....__c
+00000210: 6c61 7373 5f5f a900 fa58 433a 5c55 7365  lass__...XC:\Use
+00000220: 7273 5c6d 696c 6c61 7264 5c44 6f63 756d  rs\millard\Docum
+00000230: 656e 7473 5c47 4954 5c50 6879 7369 6f46  ents\GIT\PhysioF
+00000240: 6974 5c50 6879 7369 6f46 6974 5c50 6879  it\PhysioFit\Phy
+00000250: 7369 6f46 6974 5c70 6879 7369 6f66 6974  sioFit\physiofit
+00000260: 5c6d 6f64 656c 735c 6d6f 6465 6c5f 332e  \models\model_3.
+00000270: 7079 7208 0000 000d 0000 0073 0a00 0000  pyr........s....
+00000280: 0c02 0601 0601 0601 0a01 7a13 4368 696c  ..........z.Chil
+00000290: 644d 6f64 656c 2e5f 5f69 6e69 745f 5f63  dModel.__init__c
+000002a0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000002b0: 0700 0000 4300 0001 73a0 0000 007c 006a  ....C...s....|.j
+000002c0: 007c 006a 0064 019c 027c 005f 0164 0264  .|.j.d...|._.d.d
+000002d0: 0364 0484 007c 006a 0244 0083 0169 017c  .d...|.j.D...i.|
+000002e0: 005f 0374 0464 0564 0664 079c 0283 017c  ._.t.d.d.d.....|
+000002f0: 005f 057c 006a 0244 005d 2f7d 017c 006a  ._.|.j.D.]/}.|.j
+00000300: 01a0 067c 019b 0064 089d 027c 006a 007c  ...|...d...|.j.|
+00000310: 019b 0064 099d 027c 006a 0069 02a1 0101  ...d...|.j.i....
+00000320: 007c 006a 05a0 067c 019b 0064 089d 0264  .|.j...|...d...d
+00000330: 0a7c 019b 0064 099d 0264 0b69 02a1 0101  .|...d...d.i....
+00000340: 0064 0264 0c64 0484 007c 006a 0244 0083  .d.d.d...|.j.D..
+00000350: 0169 017c 005f 0371 1e64 0053 0029 0d4e  .i.|._.q.d.S.).N
+00000360: 2902 5a03 585f 4fda 026d 75da 0b44 6567  ).Z.X_O..mu..Deg
+00000370: 7261 6461 7469 6f6e 6301 0000 0000 0000  radationc.......
+00000380: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00000390: 01f3 1200 0000 6900 7c00 5d05 7d01 7c01  ......i.|.].}.|.
+000003a0: 6400 9302 7102 5300 a901 7201 0000 0072  d...q.S...r....r
+000003b0: 1100 0000 a902 da02 2e30 da03 6d65 7472  .........0..metr
+000003c0: 1100 0000 7211 0000 0072 1200 0000 da0a  ....r....r......
+000003d0: 3c64 6963 7463 6f6d 703e 1b00 0000 f306  <dictcomp>......
+000003e0: 0000 0006 0006 0106 ff7a 2943 6869 6c64  .........z)Child
+000003f0: 4d6f 6465 6c2e 6765 745f 7061 7261 6d73  Model.get_params
+00000400: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00000410: 6f6d 703e 2902 e7fc a9f1 d24d 6250 3fe9  omp>)......MbP?.
+00000420: 0a00 0000 2902 721c 0000 00e9 0300 0000  ....).r.........
+00000430: 2902 da03 585f 3072 1300 0000 da02 5f71  )...X_0r......_q
+00000440: da03 5f4d 3029 0269 ceff ffff e932 0000  .._M0).i.....2..
+00000450: 0029 0267 8ded b5a0 f7c6 b03e 7222 0000  .).g.......>r"..
+00000460: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000470: 0000 0400 0000 5300 0001 7215 0000 0072  ......S...r....r
+00000480: 1600 0000 7211 0000 0072 1700 0000 7211  ....r....r....r.
+00000490: 0000 0072 1100 0000 7212 0000 0072 1a00  ...r....r....r..
+000004a0: 0000 3000 0000 721b 0000 0029 0772 0a00  ..0...r....).r..
+000004b0: 0000 720b 0000 00da 0b6d 6574 6162 6f6c  ..r......metabol
+000004c0: 6974 6573 720c 0000 0072 0400 0000 da06  itesr....r......
+000004d0: 626f 756e 6473 da06 7570 6461 7465 2902  bounds..update).
+000004e0: 720d 0000 00da 0a6d 6574 6162 6f6c 6974  r......metabolit
+000004f0: 6572 1100 0000 7211 0000 0072 1200 0000  er....r....r....
+00000500: da0a 6765 745f 7061 7261 6d73 1500 0000  ..get_params....
+00000510: 7332 0000 0004 0304 0108 fe08 0404 010a  s2..............
+00000520: ff02 0402 0102 010a fe0a 0406 010c 020c  ................
+00000530: 0102 fe04 ff06 060a 020a 0102 fe04 ff08  ................
+00000540: 0604 010c ff04 f37a 1543 6869 6c64 4d6f  .......z.ChildMo
+00000550: 6465 6c2e 6765 745f 7061 7261 6d73 da0b  del.get_params..
+00000560: 7061 7261 6d73 5f6f 7074 69da 046c 6973  params_opti..lis
+00000570: 74da 0b64 6174 615f 6d61 7472 6978 fa0a  t..data_matrix..
+00000580: 6e70 2e6e 6461 7272 6179 da0b 7469 6d65  np.ndarray..time
+00000590: 5f76 6563 746f 72da 0f70 6172 616d 735f  _vector..params_
+000005a0: 6e6f 6e5f 6f70 7469 fa0b 6469 6374 207c  non_opti..dict |
+000005b0: 206c 6973 7463 0400 0000 0000 0000 0000   listc..........
+000005c0: 0000 0e00 0000 0500 0000 4300 0001 73d6  ..........C...s.
+000005d0: 0000 0074 00a0 017c 01a1 017d 047c 0064  ...t...|...}.|.d
+000005e0: 0119 007d 057c 0064 0219 007d 0674 00a0  ...}.|.d...}.t..
+000005f0: 027c 067c 0214 00a1 017d 077c 057c 0714  .|.|.....}.|.|..
+00000600: 007c 0464 0064 0085 0264 0166 023c 0064  .|.d.d...d.f.<.d
+00000610: 0364 0484 007c 0364 0519 00a0 03a1 0044  .d...|.d.......D
+00000620: 0083 017d 0874 0464 0274 0574 067c 0083  ...}.t.d.t.t.|..
+00000630: 0164 061b 0083 0183 0244 005d 347d 097c  .d.......D.]4}.|
+00000640: 007c 0964 0614 0019 007d 0a7c 007c 0964  .|.d.....}.|.|.d
+00000650: 0614 0064 0217 0019 007d 0b7c 087c 0964  ...d.....}.|.|.d
+00000660: 0218 0019 007d 0c74 00a0 027c 0c0b 007c  .....}.t...|...|
+00000670: 0214 00a1 017d 0d7c 0a7c 057c 067c 0c17  .....}.|.|.|.|..
+00000680: 001b 0014 007c 077c 0d18 0014 007c 0b7c  .....|.|.....|.|
+00000690: 0d14 0017 007c 0464 0064 0085 027c 0966  .....|.d.d...|.f
+000006a0: 023c 0071 347c 0453 0029 074e 7201 0000  .<.q4|.S.).Nr...
+000006b0: 0072 0600 0000 6301 0000 0000 0000 0000  .r....c.........
+000006c0: 0000 0002 0000 0003 0000 0053 0000 0173  ...........S...s
+000006d0: 1000 0000 6700 7c00 5d04 7d01 7c01 9102  ....g.|.].}.|...
+000006e0: 7102 5300 7211 0000 0072 1100 0000 2902  q.S.r....r....).
+000006f0: 7218 0000 00da 0576 616c 7565 7211 0000  r......valuer...
+00000700: 0072 1100 0000 7212 0000 00da 0a3c 6c69  .r....r......<li
+00000710: 7374 636f 6d70 3e46 0000 0073 0200 0000  stcomp>F...s....
+00000720: 1000 7a27 4368 696c 644d 6f64 656c 2e73  ..z'ChildModel.s
+00000730: 696d 756c 6174 652e 3c6c 6f63 616c 733e  imulate.<locals>
+00000740: 2e3c 6c69 7374 636f 6d70 3e72 1400 0000  .<listcomp>r....
+00000750: e902 0000 0029 07da 026e 70da 0a65 6d70  .....)...np..emp
+00000760: 7479 5f6c 696b 65da 0365 7870 da06 7661  ty_like..exp..va
+00000770: 6c75 6573 da05 7261 6e67 65da 0369 6e74  lues..range..int
+00000780: da03 6c65 6e29 0e72 2800 0000 722a 0000  ..len).r(...r*..
+00000790: 0072 2c00 0000 722d 0000 00da 1073 696d  .r,...r-.....sim
+000007a0: 756c 6174 6564 5f6d 6174 7269 78da 0378  ulated_matrix..x
+000007b0: 5f30 7213 0000 005a 0865 7870 5f6d 755f  _0r....Z.exp_mu_
+000007c0: 74da 0c66 6978 6564 5f70 6172 616d 73da  t..fixed_params.
+000007d0: 0169 da01 71da 036d 5f30 da01 6b5a 0765  .i..q..m_0..kZ.e
+000007e0: 7870 5f6b 5f74 7211 0000 0072 1100 0000  xp_k_tr....r....
+000007f0: 7212 0000 00da 0873 696d 756c 6174 6535  r......simulate5
+00000800: 0000 0073 2200 0000 0a08 0803 0801 0e03  ...s"...........
+00000810: 1401 1601 1a02 0c01 1001 0c01 1001 0e01  ................
+00000820: 0601 02ff 0602 12fe 0404 7a13 4368 696c  ..........z.Chil
+00000830: 644d 6f64 656c 2e73 696d 756c 6174 6529  dModel.simulate)
+00000840: 0872 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00000850: 722b 0000 0072 2c00 0000 722b 0000 0072  r+...r,...r+...r
+00000860: 2d00 0000 722e 0000 0029 08da 085f 5f6e  -...r....)...__n
+00000870: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000880: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000890: 0800 0000 7227 0000 00da 0c73 7461 7469  ....r'.....stati
+000008a0: 636d 6574 686f 6472 4000 0000 da0d 5f5f  cmethodr@.....__
+000008b0: 636c 6173 7363 656c 6c5f 5f72 1100 0000  classcell__r....
+000008c0: 7211 0000 0072 0f00 0000 7212 0000 0072  r....r....r....r
+000008d0: 0500 0000 0b00 0000 730a 0000 0008 000c  ........s.......
+000008e0: 0208 0802 2014 0172 0500 0000 2909 da07  .... ..r....)...
+000008f0: 5f5f 646f 635f 5fda 0a5f 5f66 7574 7572  __doc__..__futur
+00000900: 655f 5f72 0200 0000 da05 6e75 6d70 7972  e__r......numpyr
+00000910: 3200 0000 da1b 7068 7973 696f 6669 742e  2.....physiofit.
+00000920: 6d6f 6465 6c73 2e62 6173 655f 6d6f 6465  models.base_mode
+00000930: 6c72 0300 0000 7204 0000 0072 0500 0000  lr....r....r....
+00000940: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000950: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000960: 0000 730a 0000 0004 000c 0408 0110 0214  ..s.............
+00000970: 03                                       .
```

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_3.cpython-39.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_4.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 18 08:44:18 2023 UTC, .py size: 2427 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,149 +1,114 @@
-00000000: 610d 0d0a 0000 0000 6258 3e64 7b09 0000  a.......bX>d{...
+00000000: 6f0d 0d0a 0000 0000 ac81 1d64 5407 0000  o..........dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 6506 8303 5a08 6403 5300 2907 7a32 0a4d  e...Z.d.S.).z2.M
 00000070: 6f64 756c 6520 636f 6e74 6169 6e69 6e67  odule containing
 00000080: 2074 6865 206d 6574 686f 6473 2075 7365   the methods use
 00000090: 6420 6279 2050 6879 7369 6f46 6974 2e0a  d by PhysioFit..
 000000a0: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
 000000b0: 696f 6e73 4e29 02da 054d 6f64 656c da06  ionsN)...Model..
 000000c0: 426f 756e 6473 6300 0000 0000 0000 0000  Boundsc.........
-000000d0: 0000 0000 0000 0006 0000 0000 0000 0173  ...............s
-000000e0: 3c00 0000 6500 5a01 6400 5a02 8700 6601  <...e.Z.d.Z...f.
+000000d0: 0000 0000 0000 0004 0000 0000 0000 0173  ...............s
+000000e0: 3200 0000 6500 5a01 6400 5a02 8700 6601  2...e.Z.d.Z...f.
 000000f0: 6401 6402 8408 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00000100: 6505 6405 6406 6406 6407 6408 9c04 6409  e.d.d.d.d.d...d.
-00000110: 640a 8404 8301 5a06 8700 0400 5a07 5300  d.....Z.....Z.S.
-00000120: 290b da0a 4368 696c 644d 6f64 656c 6302  )...ChildModelc.
-00000130: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000140: 0000 0003 0000 0173 2800 0000 7400 8300  .......s(...t...
-00000150: a001 7c01 a101 0100 6401 7c00 5f02 6402  ..|.....d.|._.d.
-00000160: 7c00 5f03 6400 7c00 5f04 6400 7c00 5f05  |._.d.|._.d.|._.
-00000170: 6400 5300 2903 4e7a 3853 7465 6164 792d  d.S.).Nz8Steady-
-00000180: 7374 6174 6520 6261 7463 6820 6d6f 6465  state batch mode
-00000190: 6c20 7769 7468 2064 6567 7261 6461 7469  l with degradati
-000001a0: 6f6e 206f 6620 6d65 7461 626f 6c69 7465  on of metabolite
-000001b0: 73e9 0100 0000 2906 da05 7375 7065 72da  s.....)...super.
-000001c0: 085f 5f69 6e69 745f 5fda 0a6d 6f64 656c  .__init__..model
-000001d0: 5f6e 616d 65da 0476 696e 69da 1670 6172  _name..vini..par
-000001e0: 616d 6574 6572 735f 746f 5f65 7374 696d  ameters_to_estim
-000001f0: 6174 65da 1066 6978 6564 5f70 6172 616d  ate..fixed_param
-00000200: 6574 6572 7329 02da 0473 656c 66da 0464  eters)...self..d
-00000210: 6174 61a9 01da 095f 5f63 6c61 7373 5f5f  ata....__class__
-00000220: a900 fa47 433a 5c55 7365 7273 5c6c 6567  ...GC:\Users\leg
-00000230: 7265 6761 6d5c 5079 6368 6172 6d50 726f  regam\PycharmPro
-00000240: 6a65 6374 735c 5068 7973 696f 4669 745c  jects\PhysioFit\
-00000250: 7068 7973 696f 6669 745c 6d6f 6465 6c73  physiofit\models
-00000260: 5c6d 6f64 656c 5f33 2e70 7972 0800 0000  \model_3.pyr....
-00000270: 0d00 0000 730a 0000 0000 020c 0106 0106  ....s...........
-00000280: 0106 017a 1343 6869 6c64 4d6f 6465 6c2e  ...z.ChildModel.
-00000290: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-000002a0: 0000 0000 0002 0000 0007 0000 0043 0000  .............C..
-000002b0: 0173 a000 0000 7c00 6a00 7c00 6a00 6401  .s....|.j.|.j.d.
-000002c0: 9c02 7c00 5f01 6402 6403 6404 8400 7c00  ..|._.d.d.d...|.
-000002d0: 6a02 4400 8301 6901 7c00 5f03 7404 6405  j.D...i.|._.t.d.
-000002e0: 6406 6407 9c02 8301 7c00 5f05 7c00 6a02  d.d.....|._.|.j.
-000002f0: 4400 5d5e 7d01 7c00 6a01 a006 7c01 9b00  D.]^}.|.j...|...
-00000300: 6408 9d02 7c00 6a00 7c01 9b00 6409 9d02  d...|.j.|...d...
-00000310: 7c00 6a00 6902 a101 0100 7c00 6a05 a006  |.j.i.....|.j...
-00000320: 7c01 9b00 6408 9d02 640a 7c01 9b00 6409  |...d...d.|...d.
-00000330: 9d02 640b 6902 a101 0100 6402 640c 6404  ..d.i.....d.d.d.
-00000340: 8400 7c00 6a02 4400 8301 6901 7c00 5f03  ..|.j.D...i.|._.
-00000350: 713c 6400 5300 290d 4e29 025a 0358 5f4f  q<d.S.).N).Z.X_O
-00000360: da02 6d75 da0b 4465 6772 6164 6174 696f  ..mu..Degradatio
-00000370: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
-00000380: 0000 0400 0000 5300 0001 7312 0000 0069  ......S...s....i
-00000390: 007c 005d 0a7d 017c 0164 0093 0271 0453  .|.].}.|.d...q.S
-000003a0: 00a9 0172 0100 0000 7211 0000 00a9 02da  ...r....r.......
-000003b0: 022e 30da 036d 6574 7211 0000 0072 1100  ..0..metr....r..
-000003c0: 0000 7212 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
-000003d0: 6d70 3e1b 0000 0073 0200 0000 0601 7a29  mp>....s......z)
-000003e0: 4368 696c 644d 6f64 656c 2e67 6574 5f70  ChildModel.get_p
-000003f0: 6172 616d 732e 3c6c 6f63 616c 733e 2e3c  arams.<locals>.<
-00000400: 6469 6374 636f 6d70 3e29 02e7 fca9 f1d2  dictcomp>)......
-00000410: 4d62 503f e90a 0000 0029 0272 1a00 0000  MbP?.....).r....
-00000420: e903 0000 0029 02da 0358 5f30 7213 0000  .....)...X_0r...
-00000430: 00da 025f 71da 035f 4d30 2902 69ce ffff  ..._q.._M0).i...
-00000440: ffe9 3200 0000 2902 678d edb5 a0f7 c6b0  ..2...).g.......
-00000450: 3e72 2000 0000 6301 0000 0000 0000 0000  >r ...c.........
-00000460: 0000 0002 0000 0004 0000 0053 0000 0173  ...........S...s
-00000470: 1200 0000 6900 7c00 5d0a 7d01 7c01 6400  ....i.|.].}.|.d.
-00000480: 9302 7104 5300 7215 0000 0072 1100 0000  ..q.S.r....r....
-00000490: 7216 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-000004a0: 1200 0000 7219 0000 0030 0000 0073 0200  ....r....0...s..
-000004b0: 0000 0601 2907 720a 0000 0072 0b00 0000  ....).r....r....
-000004c0: da0b 6d65 7461 626f 6c69 7465 7372 0c00  ..metabolitesr..
-000004d0: 0000 7204 0000 00da 0662 6f75 6e64 73da  ..r......bounds.
-000004e0: 0675 7064 6174 6529 0272 0d00 0000 da0a  .update).r......
-000004f0: 6d65 7461 626f 6c69 7465 7211 0000 0072  metaboliter....r
-00000500: 1100 0000 7212 0000 00da 0a67 6574 5f70  ....r......get_p
-00000510: 6172 616d 7315 0000 0073 3000 0000 0003  arams....s0.....
-00000520: 0401 04fe 0804 0801 04ff 0a04 0201 0201  ................
-00000530: 02fe 0a04 0a01 0602 0c01 0cfe 02ff 0406  ................
-00000540: 0602 0a01 0afe 02ff 0406 0801 04ff 7a15  ..............z.
-00000550: 4368 696c 644d 6f64 656c 2e67 6574 5f70  ChildModel.get_p
-00000560: 6172 616d 73da 046c 6973 747a 0a6e 702e  arams..listz.np.
-00000570: 6e64 6172 7261 797a 0b64 6963 7420 7c20  ndarrayz.dict | 
-00000580: 6c69 7374 2904 da0b 7061 7261 6d73 5f6f  list)...params_o
-00000590: 7074 69da 0b64 6174 615f 6d61 7472 6978  pti..data_matrix
-000005a0: da0b 7469 6d65 5f76 6563 746f 72da 0f70  ..time_vector..p
-000005b0: 6172 616d 735f 6e6f 6e5f 6f70 7469 6304  arams_non_optic.
-000005c0: 0000 0000 0000 0000 0000 000e 0000 0005  ................
-000005d0: 0000 0043 0000 0173 d600 0000 7400 a001  ...C...s....t...
-000005e0: 7c01 a101 7d04 7c00 6401 1900 7d05 7c00  |...}.|.d...}.|.
-000005f0: 6402 1900 7d06 7400 a002 7c06 7c02 1400  d...}.t...|.|...
-00000600: a101 7d07 7c05 7c07 1400 7c04 6400 6400  ..}.|.|...|.d.d.
-00000610: 8502 6401 6602 3c00 6403 6404 8400 7c03  ..d.f.<.d.d...|.
-00000620: 6405 1900 a003 a100 4400 8301 7d08 7404  d.......D...}.t.
-00000630: 6402 7405 7406 7c00 8301 6406 1b00 8301  d.t.t.|...d.....
-00000640: 8302 4400 5d68 7d09 7c00 7c09 6406 1400  ..D.]h}.|.|.d...
-00000650: 1900 7d0a 7c00 7c09 6406 1400 6402 1700  ..}.|.|.d...d...
-00000660: 1900 7d0b 7c08 7c09 6402 1800 1900 7d0c  ..}.|.|.d.....}.
-00000670: 7400 a002 7c0c 0b00 7c02 1400 a101 7d0d  t...|...|.....}.
-00000680: 7c0a 7c05 7c06 7c0c 1700 1b00 1400 7c07  |.|.|.|.......|.
-00000690: 7c0d 1800 1400 7c0b 7c0d 1400 1700 7c04  |.....|.|.....|.
-000006a0: 6400 6400 8502 7c09 6602 3c00 7168 7c04  d.d...|.f.<.qh|.
-000006b0: 5300 2907 4e72 0100 0000 7206 0000 0063  S.).Nr....r....c
-000006c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000006d0: 0300 0000 5300 0001 7310 0000 0067 007c  ....S...s....g.|
-000006e0: 005d 087d 017c 0191 0271 0453 0072 1100  .].}.|...q.S.r..
-000006f0: 0000 7211 0000 0029 0272 1700 0000 da05  ..r....).r......
-00000700: 7661 6c75 6572 1100 0000 7211 0000 0072  valuer....r....r
-00000710: 1200 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-00000720: 4600 0000 f300 0000 007a 2743 6869 6c64  F........z'Child
-00000730: 4d6f 6465 6c2e 7369 6d75 6c61 7465 2e3c  Model.simulate.<
-00000740: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000750: 703e 7214 0000 00e9 0200 0000 2907 da02  p>r.........)...
-00000760: 6e70 da0a 656d 7074 795f 6c69 6b65 da03  np..empty_like..
-00000770: 6578 70da 0676 616c 7565 73da 0572 616e  exp..values..ran
-00000780: 6765 da03 696e 74da 036c 656e 290e 7227  ge..int..len).r'
-00000790: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-000007a0: 0000 da10 7369 6d75 6c61 7465 645f 6d61  ....simulated_ma
-000007b0: 7472 6978 da03 785f 3072 1300 0000 5a08  trix..x_0r....Z.
-000007c0: 6578 705f 6d75 5f74 da0c 6669 7865 645f  exp_mu_t..fixed_
-000007d0: 7061 7261 6d73 da01 69da 0171 da03 6d5f  params..i..q..m_
-000007e0: 30da 016b 5a07 6578 705f 6b5f 7472 1100  0..kZ.exp_k_tr..
-000007f0: 0000 7211 0000 0072 1200 0000 da08 7369  ..r....r......si
-00000800: 6d75 6c61 7465 3500 0000 7322 0000 0000  mulate5...s"....
-00000810: 080a 0308 0108 030e 0114 0116 021a 010c  ................
-00000820: 0110 010c 0110 010e 0106 ff02 0206 fe12  ................
-00000830: 047a 1343 6869 6c64 4d6f 6465 6c2e 7369  .z.ChildModel.si
-00000840: 6d75 6c61 7465 2908 da08 5f5f 6e61 6d65  mulate)...__name
-00000850: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000860: 5f5f 7175 616c 6e61 6d65 5f5f 7208 0000  __qualname__r...
-00000870: 0072 2500 0000 da0c 7374 6174 6963 6d65  .r%.....staticme
-00000880: 7468 6f64 723d 0000 00da 0d5f 5f63 6c61  thodr=.....__cla
-00000890: 7373 6365 6c6c 5f5f 7211 0000 0072 1100  sscell__r....r..
-000008a0: 0000 720f 0000 0072 1200 0000 7205 0000  ..r....r....r...
-000008b0: 000b 0000 0073 0800 0000 0802 0c08 0820  .....s......... 
-000008c0: 0201 7205 0000 0029 09da 075f 5f64 6f63  ..r....)...__doc
-000008d0: 5f5f da0a 5f5f 6675 7475 7265 5f5f 7202  __..__future__r.
-000008e0: 0000 00da 056e 756d 7079 722f 0000 00da  .....numpyr/....
-000008f0: 1b70 6879 7369 6f66 6974 2e6d 6f64 656c  .physiofit.model
-00000900: 732e 6261 7365 5f6d 6f64 656c 7203 0000  s.base_modelr...
-00000910: 0072 0400 0000 7205 0000 0072 1100 0000  .r....r....r....
-00000920: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000930: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000940: 0000 0404 0c01 0802 1003                 ..........
+00000100: 6505 640e 640c 640d 8404 8301 5a06 8700  e.d.d.d.....Z...
+00000110: 0400 5a07 5300 290f da0a 4368 696c 644d  ..Z.S.)...ChildM
+00000120: 6f64 656c 6302 0000 0000 0000 0000 0000  odelc...........
+00000130: 0002 0000 0003 0000 0003 0000 0173 2800  .............s(.
+00000140: 0000 7400 8300 a001 7c01 a101 0100 6401  ..t.....|.....d.
+00000150: 7c00 5f02 6402 7c00 5f03 6400 7c00 5f04  |._.d.|._.d.|._.
+00000160: 6400 7c00 5f05 6400 5300 2903 4e7a 1853  d.|._.d.S.).Nz.S
+00000170: 7465 6164 792d 7374 6174 6520 6261 7463  teady-state batc
+00000180: 6820 6d6f 6465 6ce9 0100 0000 2906 da05  h model.....)...
+00000190: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
+000001a0: 0a6d 6f64 656c 5f6e 616d 65da 0476 696e  .model_name..vin
+000001b0: 69da 1670 6172 616d 6574 6572 735f 746f  i..parameters_to
+000001c0: 5f65 7374 696d 6174 65da 1066 6978 6564  _estimate..fixed
+000001d0: 5f70 6172 616d 6574 6572 7329 02da 0473  _parameters)...s
+000001e0: 656c 66da 0464 6174 61a9 01da 095f 5f63  elf..data....__c
+000001f0: 6c61 7373 5f5f a900 fa58 433a 5c55 7365  lass__...XC:\Use
+00000200: 7273 5c6d 696c 6c61 7264 5c44 6f63 756d  rs\millard\Docum
+00000210: 656e 7473 5c47 4954 5c50 6879 7369 6f46  ents\GIT\PhysioF
+00000220: 6974 5c50 6879 7369 6f46 6974 5c50 6879  it\PhysioFit\Phy
+00000230: 7369 6f46 6974 5c70 6879 7369 6f66 6974  sioFit\physiofit
+00000240: 5c6d 6f64 656c 735c 6d6f 6465 6c5f 342e  \models\model_4.
+00000250: 7079 7208 0000 000d 0000 0073 0a00 0000  pyr........s....
+00000260: 0c02 0601 0601 0601 0a01 7a13 4368 696c  ..........z.Chil
+00000270: 644d 6f64 656c 2e5f 5f69 6e69 745f 5f63  dModel.__init__c
+00000280: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000290: 0700 0000 4300 0001 7374 0000 007c 006a  ....C...st...|.j
+000002a0: 007c 006a 0064 019c 027c 005f 0174 0264  .|.j.d...|._.t.d
+000002b0: 0264 0364 019c 0283 017c 005f 037c 006a  .d.d.....|._.|.j
+000002c0: 0444 005d 247d 017c 006a 01a0 057c 019b  .D.]$}.|.j...|..
+000002d0: 0064 049d 027c 006a 007c 019b 0064 059d  .d...|.j.|...d..
+000002e0: 027c 006a 0069 02a1 0101 007c 006a 03a0  .|.j.i.....|.j..
+000002f0: 057c 019b 0064 049d 0264 067c 019b 0064  .|...d...d.|...d
+00000300: 059d 0264 0769 02a1 0101 0071 1364 0053  ...d.i.....q.d.S
+00000310: 0029 084e 2902 da03 585f 30da 026d 7529  .).N)...X_0..mu)
+00000320: 02e7 fca9 f1d2 4d62 503f e90a 0000 0029  ......MbP?.....)
+00000330: 0272 1500 0000 e903 0000 00da 025f 71da  .r..........._q.
+00000340: 035f 4d30 2902 69ce ffff ffe9 3200 0000  ._M0).i.....2...
+00000350: 2902 678d edb5 a0f7 c6b0 3e72 1a00 0000  ).g.......>r....
+00000360: 2906 720a 0000 0072 0b00 0000 7204 0000  ).r....r....r...
+00000370: 00da 0662 6f75 6e64 73da 0b6d 6574 6162  ...bounds..metab
+00000380: 6f6c 6974 6573 da06 7570 6461 7465 2902  olites..update).
+00000390: 720d 0000 00da 0a6d 6574 6162 6f6c 6974  r......metabolit
+000003a0: 6572 1100 0000 7211 0000 0072 1200 0000  er....r....r....
+000003b0: da0a 6765 745f 7061 7261 6d73 1500 0000  ..get_params....
+000003c0: 7326 0000 0004 0304 0108 fe02 0402 0102  s&..............
+000003d0: 010a fe0a 0406 010c 020c 0102 fe04 ff06  ................
+000003e0: 060a 020a 0102 fe06 ff04 f97a 1543 6869  ...........z.Chi
+000003f0: 6c64 4d6f 6465 6c2e 6765 745f 7061 7261  ldModel.get_para
+00000400: 6d73 da0b 7061 7261 6d73 5f6f 7074 69da  ms..params_opti.
+00000410: 046c 6973 74da 0b64 6174 615f 6d61 7472  .list..data_matr
+00000420: 6978 fa0a 6e70 2e6e 6461 7272 6179 da0b  ix..np.ndarray..
+00000430: 7469 6d65 5f76 6563 746f 72da 0f70 6172  time_vector..par
+00000440: 616d 735f 6e6f 6e5f 6f70 7469 fa0b 6469  ams_non_opti..di
+00000450: 6374 207c 206c 6973 7463 0400 0000 0000  ct | listc......
+00000460: 0000 0000 0000 0b00 0000 0500 0000 4300  ..............C.
+00000470: 0001 739c 0000 0074 00a0 017c 01a1 017d  ..s....t...|...}
+00000480: 047c 0064 0119 007d 057c 0064 0219 007d  .|.d...}.|.d...}
+00000490: 0674 00a0 027c 067c 0214 00a1 017d 077c  .t...|.|.....}.|
+000004a0: 057c 0714 007c 0464 0064 0085 0264 0166  .|...|.d.d...d.f
+000004b0: 023c 0074 0364 0274 0474 057c 0083 0164  .<.t.d.t.t.|...d
+000004c0: 031b 0083 0183 0244 005d 227d 087c 007c  .......D.]"}.|.|
+000004d0: 0864 0314 0019 007d 097c 007c 0864 0314  .d.....}.|.|.d..
+000004e0: 0064 0217 0019 007d 0a7c 097c 057c 061b  .d.....}.|.|.|..
+000004f0: 0014 007c 0764 0218 0014 007c 0a17 007c  ...|.d.....|...|
+00000500: 0464 0064 0085 027c 0866 023c 0071 297c  .d.d...|.f.<.q)|
+00000510: 0453 0029 044e 7201 0000 0072 0600 0000  .S.).Nr....r....
+00000520: e902 0000 0029 06da 026e 70da 0a65 6d70  .....)...np..emp
+00000530: 7479 5f6c 696b 65da 0365 7870 da05 7261  ty_like..exp..ra
+00000540: 6e67 65da 0369 6e74 da03 6c65 6e29 0b72  nge..int..len).r
+00000550: 2000 0000 7222 0000 0072 2400 0000 7225   ...r"...r$...r%
+00000560: 0000 00da 1073 696d 756c 6174 6564 5f6d  .....simulated_m
+00000570: 6174 7269 78da 0378 5f30 7214 0000 00da  atrix..x_0r.....
+00000580: 0865 7870 5f6d 755f 74da 0169 da01 71da  .exp_mu_t..i..q.
+00000590: 036d 5f30 7211 0000 0072 1100 0000 7212  .m_0r....r....r.
+000005a0: 0000 00da 0873 696d 756c 6174 652d 0000  .....simulate-..
+000005b0: 0073 1c00 0000 0a08 0801 0801 0e01 1401  .s..............
+000005c0: 1a01 0c01 1001 0a01 0601 02ff 0202 12fe  ................
+000005d0: 0404 7a13 4368 696c 644d 6f64 656c 2e73  ..z.ChildModel.s
+000005e0: 696d 756c 6174 6529 0872 2000 0000 7221  imulate).r ...r!
+000005f0: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
+00000600: 0000 7223 0000 0072 2500 0000 7226 0000  ..r#...r%...r&..
+00000610: 0029 08da 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00000620: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000630: 6c6e 616d 655f 5f72 0800 0000 721f 0000  lname__r....r...
+00000640: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
+00000650: 3400 0000 da0d 5f5f 636c 6173 7363 656c  4.....__classcel
+00000660: 6c5f 5f72 1100 0000 7211 0000 0072 0f00  l__r....r....r..
+00000670: 0000 7212 0000 0072 0500 0000 0b00 0000  ..r....r........
+00000680: 730a 0000 0008 000c 0208 0802 1814 0172  s..............r
+00000690: 0500 0000 2909 da07 5f5f 646f 635f 5fda  ....)...__doc__.
+000006a0: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
+000006b0: da05 6e75 6d70 7972 2800 0000 da1b 7068  ..numpyr(.....ph
+000006c0: 7973 696f 6669 742e 6d6f 6465 6c73 2e62  ysiofit.models.b
+000006d0: 6173 655f 6d6f 6465 6c72 0300 0000 7204  ase_modelr....r.
+000006e0: 0000 0072 0500 0000 7211 0000 0072 1100  ...r....r....r..
+000006f0: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
+00000700: 6f64 756c 653e 0100 0000 730a 0000 0004  odule>....s.....
+00000710: 000c 0408 0110 0214 03                   .........
```

### Comparing `physiofit-3.0.4/physiofit/models/__pycache__/model_5.cpython-310.pyc` & `physiofit-3.0.6/physiofit/models/__pycache__/model_6.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 24 16:02:16 2023 UTC, .py size: 4152 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 88c9 1d64 3810 0000  o..........d8...
+00000000: 6f0d 0d0a 0000 0000 6dae 1d64 580f 0000  o.......m..dX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 d800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 0100 4700 6406 6407 8400 6407 6508 8303  ..G.d.d...d.e...
 00000070: 5a0a 650b 6408 6b02 726a 6401 6409 6c0c  Z.e.d.k.rjd.d.l.
@@ -27,174 +27,174 @@
 000001a0: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
 000001b0: 0484 005a 0465 0564 0e64 0c64 0d84 0483  ...Z.e.d.d.d....
 000001c0: 015a 0687 0004 005a 0753 0029 0fda 0a43  .Z.....Z.S.)...C
 000001d0: 6869 6c64 4d6f 6465 6c63 0200 0000 0000  hildModelc......
 000001e0: 0000 0000 0000 0200 0000 0300 0000 0300  ................
 000001f0: 0001 7322 0000 0074 0083 00a0 017c 01a1  ..s"...t.....|..
 00000200: 0101 0064 017c 005f 0264 027c 005f 0364  ...d.|._.d.|._.d
-00000210: 007c 005f 0464 0053 0029 034e 7a2c 4479  .|._.d.S.).Nz,Dy
-00000220: 6e61 6d69 6320 4d6f 6e6f 6420 6d6f 6465  namic Monod mode
-00000230: 6c20 2831 2073 7562 7374 7261 7465 2c20  l (1 substrate, 
-00000240: 3120 7072 6f64 7563 7429 e901 0000 0029  1 product).....)
-00000250: 05da 0573 7570 6572 da08 5f5f 696e 6974  ...super..__init
-00000260: 5f5f da0a 6d6f 6465 6c5f 6e61 6d65 da04  __..model_name..
-00000270: 7669 6e69 da16 7061 7261 6d65 7465 7273  vini..parameters
-00000280: 5f74 6f5f 6573 7469 6d61 7465 2902 da04  _to_estimate)...
-00000290: 7365 6c66 da04 6461 7461 a901 da09 5f5f  self..data....__
-000002a0: 636c 6173 735f 5fa9 00fa 5843 3a5c 5573  class__...XC:\Us
-000002b0: 6572 735c 6d69 6c6c 6172 645c 446f 6375  ers\millard\Docu
-000002c0: 6d65 6e74 735c 4749 545c 5068 7973 696f  ments\GIT\Physio
-000002d0: 4669 745c 5068 7973 696f 4669 745c 5068  Fit\PhysioFit\Ph
-000002e0: 7973 696f 4669 745c 7068 7973 696f 6669  ysioFit\physiofi
-000002f0: 745c 6d6f 6465 6c73 5c6d 6f64 656c 5f35  t\models\model_5
-00000300: 2e70 7972 0900 0000 0d00 0000 7308 0000  .pyr........s...
-00000310: 000c 0206 0106 010a 017a 1343 6869 6c64  .........z.Child
-00000320: 4d6f 6465 6c2e 5f5f 696e 6974 5f5f 6301  Model.__init__c.
-00000330: 0000 0000 0000 0000 0000 0002 0000 0009  ................
-00000340: 0000 0043 0000 0173 0601 0000 7c00 6a00  ...C...s....|.j.
-00000350: 7c00 6a00 6401 9c02 7c00 5f01 7402 6402  |.j.d...|._.t.d.
-00000360: 6403 6401 8d02 7c00 5f03 7c00 6a04 4400  d.d...|._.|.j.D.
-00000370: 5d35 7d01 7c01 a005 6404 a101 7247 7c00  ]5}.|...d...rG|.
-00000380: 6a01 a006 7c01 9b00 6405 9d02 7c00 6a00  j...|...d...|.j.
-00000390: 7c01 9b00 6406 9d02 7c00 6a00 7c01 9b00  |...d...|.j.|...
-000003a0: 6407 9d02 6408 6903 a101 0100 7c00 6a03  d...d.i.....|.j.
-000003b0: a006 7c01 9b00 6405 9d02 6409 7c01 9b00  ..|...d...d.|...
-000003c0: 6406 9d02 6409 7c01 9b00 6407 9d02 6409  d...d.|...d...d.
-000003d0: 6903 a101 0100 0100 7148 7112 7c00 6a04  i.......qHq.|.j.
-000003e0: 4400 5d2a 7d01 7c01 a005 640a a101 7275  D.]*}.|...d...ru
-000003f0: 7c00 6a01 a006 7c01 9b00 640b 9d02 7c00  |.j...|...d...|.
-00000400: 6a00 7c01 9b00 640c 9d02 6408 6902 a101  j.|...d...d.i...
-00000410: 0100 7c00 6a03 a006 7c01 9b00 640b 9d02  ..|.j...|...d...
-00000420: 6409 7c01 9b00 640c 9d02 6409 6902 a101  d.|...d...d.i...
-00000430: 0100 0100 7176 714b 7407 7c00 6a01 8301  ....qvqKt.|.j...
-00000440: 640d 6b03 7281 7408 640e 8301 8201 6400  d.k.r.t.d.....d.
-00000450: 5300 290f 4e29 02da 0358 5f30 da04 795f  S.).N)...X_0..y_
-00000460: 424d 2902 e7fc a9f1 d24d 6250 3fe9 0a00  BM)......MbP?...
-00000470: 0000 2902 7215 0000 00e9 0300 0000 5a02  ..).r.........Z.
-00000480: 535f 5a03 5f6b 6d5a 065f 7173 6d61 785a  S_Z._kmZ._qsmaxZ
-00000490: 045f 735f 30e9 6400 0000 2902 678d edb5  ._s_0.d...).g...
-000004a0: a0f7 c6b0 3e72 1800 0000 5a02 505f 5a04  ....>r....Z.P_Z.
-000004b0: 5f79 5f50 5a04 5f70 5f30 e907 0000 007a  _y_PZ._p_0.....z
-000004c0: 8854 6869 7320 6d6f 6465 6c20 6578 7065  .This model expe
-000004d0: 6374 7320 3220 6d65 7461 626f 6c69 7465  cts 2 metabolite
-000004e0: 7320 696e 2074 6865 2064 6174 6120 6669  s in the data fi
-000004f0: 6c65 2028 3120 7375 6273 7472 6174 6520  le (1 substrate 
-00000500: 7769 7468 206e 616d 6520 7374 6172 7469  with name starti
-00000510: 6e67 2077 6974 6820 2753 5f27 2061 6e64  ng with 'S_' and
-00000520: 2031 2070 726f 6475 6374 2077 6974 6820   1 product with 
-00000530: 6e61 6d65 2073 7461 7274 696e 6720 7769  name starting wi
-00000540: 7468 2027 505f 2729 2e29 0972 0b00 0000  th 'P_').).r....
-00000550: 720c 0000 0072 0500 0000 da06 626f 756e  r....r......boun
-00000560: 6473 da0b 6d65 7461 626f 6c69 7465 73da  ds..metabolites.
-00000570: 0a73 7461 7274 7377 6974 68da 0675 7064  .startswith..upd
-00000580: 6174 65da 036c 656e da0a 5661 6c75 6545  ate..len..ValueE
-00000590: 7272 6f72 2902 720d 0000 00da 0a6d 6574  rror).r......met
-000005a0: 6162 6f6c 6974 6572 1100 0000 7211 0000  aboliter....r...
-000005b0: 0072 1200 0000 da0a 6765 745f 7061 7261  .r......get_para
-000005c0: 6d73 1400 0000 7350 0000 0004 0304 0108  ms....sP........
-000005d0: fe02 0502 0102 0108 fe0a 050a 0106 010c  ................
-000005e0: 020c 010a 0102 fd04 ff06 070a 020a 010a  ................
-000005f0: 0102 fd04 ff04 0702 f10a 110a 0106 010c  ................
-00000600: 020a 0102 fe04 ff06 070a 020a 0102 fe04  ................
-00000610: ff04 0602 f20e 1008 0104 ff7a 1543 6869  ...........z.Chi
-00000620: 6c64 4d6f 6465 6c2e 6765 745f 7061 7261  ldModel.get_para
-00000630: 6d73 da0b 7061 7261 6d73 5f6f 7074 69da  ms..params_opti.
-00000640: 046c 6973 74da 0b64 6174 615f 6d61 7472  .list..data_matr
-00000650: 6978 fa0a 6e70 2e6e 6461 7272 6179 da0b  ix..np.ndarray..
-00000660: 7469 6d65 5f76 6563 746f 72da 0f70 6172  time_vector..par
-00000670: 616d 735f 6e6f 6e5f 6f70 7469 da04 6469  ams_non_opti..di
-00000680: 6374 6304 0000 0000 0000 0000 0000 000f  ctc.............
-00000690: 0000 0008 0000 0043 0000 0173 8600 0000  .......C...s....
-000006a0: 7c00 6401 1900 7d04 7c00 6402 1900 7d05  |.d...}.|.d...}.
-000006b0: 7c00 6403 1900 7d06 7c00 6404 1900 7d07  |.d...}.|.d...}.
-000006c0: 7c00 6405 1900 7d08 7c00 6406 1900 7d09  |.d...}.|.d...}.
-000006d0: 7c00 6407 1900 7d0a 7c05 7c09 7c06 7c07  |.d...}.|.|.|.|.
-000006e0: 6604 7d0b 7c04 7c08 7c0a 6703 7d0c 6408  f.}.|.|.|.g.}.d.
-000006f0: 6409 8400 7d0d 7400 7c0d 7401 a002 7c02  d...}.t.|.t...|.
-00000700: a101 7401 a003 7c02 a101 6602 7c0c 7c0b  ..t...|...f.|.|.
-00000710: 640a 7404 7c02 8301 640b 8d06 7d0e 7c0e  d.t.|...d...}.|.
-00000720: 6a05 6a06 5300 290c 4e72 0100 0000 7207  j.j.S.).Nr....r.
-00000730: 0000 00e9 0200 0000 7217 0000 00e9 0400  ........r.......
-00000740: 0000 e905 0000 00e9 0600 0000 6306 0000  ............c...
-00000750: 0000 0000 0000 0000 000e 0000 0004 0000  ................
-00000760: 0053 0000 0173 5400 0000 7c01 6401 1900  .S...sT...|.d...
-00000770: 7d06 7c01 6402 1900 7d07 7c05 7c06 7c04  }.|.d...}.|.|.|.
-00000780: 7c06 1700 1b00 1400 7d08 7c02 7c08 1400  |.......}.|.|...
-00000790: 7d09 7c03 7c08 1400 7d0a 7c09 7c07 1400  }.|.|...}.|.|...
-000007a0: 7d0b 7c08 0b00 7c07 1400 7d0c 7c0a 7c07  }.|...|...}.|.|.
-000007b0: 1400 7d0d 7c0b 7c0c 7c0d 6603 5300 2903  ..}.|.|.|.f.S.).
-000007c0: 4e72 0100 0000 7207 0000 0072 1100 0000  Nr....r....r....
-000007d0: 290e da01 74da 0573 7461 7465 7214 0000  )...t..stater...
-000007e0: 00da 0379 5f50 da02 6b6d da05 7173 6d61  ...y_P..km..qsma
-000007f0: 785a 0373 5f74 5a03 785f 745a 0471 735f  xZ.s_tZ.x_tZ.qs_
-00000800: 745a 046d 755f 745a 0471 705f 74da 0264  tZ.mu_tZ.qp_t..d
-00000810: 78da 0264 73da 0264 7072 1100 0000 7211  x..ds..dpr....r.
-00000820: 0000 0072 1200 0000 da14 6361 6c63 756c  ...r......calcul
-00000830: 6174 655f 6465 7269 7661 7469 7665 5c00  ate_derivative\.
-00000840: 0000 7312 0000 0008 0308 0110 0308 0108  ..s.............
-00000850: 0108 030a 0108 010a 027a 3143 6869 6c64  .........z1Child
-00000860: 4d6f 6465 6c2e 7369 6d75 6c61 7465 2e3c  Model.simulate.<
-00000870: 6c6f 6361 6c73 3e2e 6361 6c63 756c 6174  locals>.calculat
-00000880: 655f 6465 7269 7661 7469 7665 da05 4c53  e_derivative..LS
-00000890: 4f44 4129 06da 0366 756e da06 745f 7370  ODA)...fun..t_sp
-000008a0: 616e da02 7930 da04 6172 6773 da06 6d65  an..y0..args..me
-000008b0: 7468 6f64 da06 745f 6576 616c 2907 7203  thod..t_eval).r.
-000008c0: 0000 00da 026e 70da 036d 696e da03 6d61  .....np..min..ma
-000008d0: 7872 2300 0000 da01 79da 0154 290f 7222  xr#.....y..T).r"
-000008e0: 0000 0072 2400 0000 7226 0000 0072 2700  ...r$...r&...r'.
-000008f0: 0000 da03 785f 3072 1400 0000 7230 0000  ....x_0r....r0..
-00000900: 0072 3100 0000 5a03 735f 3072 2f00 0000  .r1...Z.s_0r/...
-00000910: 5a03 705f 30da 0670 6172 616d 7372 2e00  Z.p_0..paramsr..
-00000920: 0000 7235 0000 00da 0373 6f6c 7211 0000  ..r5.....solr...
-00000930: 0072 1100 0000 7212 0000 00da 0873 696d  .r....r......sim
-00000940: 756c 6174 6547 0000 0073 2600 0000 0809  ulateG...s&.....
-00000950: 0801 0801 0801 0801 0801 0801 0c01 0a03  ................
-00000960: 0802 0213 0201 1201 0201 0201 0201 0601  ................
-00000970: 06fa 0809 7a13 4368 696c 644d 6f64 656c  ....z.ChildModel
-00000980: 2e73 696d 756c 6174 6529 0872 2200 0000  .simulate).r"...
-00000990: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
-000009a0: 2600 0000 7225 0000 0072 2700 0000 7228  &...r%...r'...r(
-000009b0: 0000 0029 08da 085f 5f6e 616d 655f 5fda  ...)...__name__.
-000009c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000009d0: 7561 6c6e 616d 655f 5f72 0900 0000 7221  ualname__r....r!
-000009e0: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
-000009f0: 6472 4500 0000 da0d 5f5f 636c 6173 7363  drE.....__classc
-00000a00: 656c 6c5f 5f72 1100 0000 7211 0000 0072  ell__r....r....r
-00000a10: 0f00 0000 7212 0000 0072 0600 0000 0b00  ....r....r......
-00000a20: 0000 730a 0000 0008 000c 0208 0702 3314  ..s...........3.
-00000a30: 0172 0600 0000 da08 5f5f 6d61 696e 5f5f  .r......__main__
-00000a40: 2901 da09 496f 4861 6e64 6c65 727a 5a43  )...IoHandlerzZC
-00000a50: 3a5c 5573 6572 735c 6c65 6772 6567 616d  :\Users\legregam
-00000a60: 5c50 7963 6861 726d 5072 6f6a 6563 7473  \PycharmProjects
-00000a70: 5c50 6879 7369 6f46 6974 5c64 6174 615c  \PhysioFit\data\
-00000a80: 4b45 494f 5f74 6573 745f 6461 7461 5c6f  KEIO_test_data\o
-00000a90: 6465 5f74 6573 745c 4b45 494f 5f52 4f42  de_test\KEIO_ROB
-00000aa0: 4f54 365f 312e 7473 76da 0474 696d 6563  OT6_1.tsv..timec
-00000ab0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000ac0: 0300 0000 4300 0001 7310 0000 0067 007c  ....C...s....g.|
-00000ad0: 005d 047d 017c 0191 0271 0253 0072 1100  .].}.|...q.S.r..
-00000ae0: 0000 7211 0000 0029 02da 022e 30da 0570  ..r....)....0..p
-00000af0: 6172 616d 7211 0000 0072 1100 0000 7212  aramr....r....r.
-00000b00: 0000 00da 0a3c 6c69 7374 636f 6d70 3e84  .....<listcomp>.
-00000b10: 0000 0073 0200 0000 1000 7250 0000 007a  ...s......rP...z
-00000b20: 0754 696d 6573 3a20 7a08 5661 6c75 6573  .Times: z.Values
-00000b30: 3a20 291e da07 5f5f 646f 635f 5fda 0a5f  : )...__doc__.._
-00000b40: 5f66 7574 7572 655f 5f72 0200 0000 da05  _future__r......
-00000b50: 6e75 6d70 7972 3d00 0000 da0f 7363 6970  numpyr=.....scip
-00000b60: 792e 696e 7465 6772 6174 6572 0300 0000  y.integrater....
-00000b70: da1b 7068 7973 696f 6669 742e 6d6f 6465  ..physiofit.mode
-00000b80: 6c73 2e62 6173 655f 6d6f 6465 6c72 0400  ls.base_modelr..
-00000b90: 0000 7205 0000 0072 0600 0000 7246 0000  ..r....r....rF..
-00000ba0: 00da 1170 6879 7369 6f66 6974 2e62 6173  ...physiofit.bas
-00000bb0: 652e 696f 724c 0000 00da 0269 6fda 0972  e.iorL.....io..r
-00000bc0: 6561 645f 6461 7461 720e 0000 00da 0b73  ead_datar......s
-00000bd0: 6f72 745f 7661 6c75 6573 da05 6d6f 6465  ort_values..mode
-00000be0: 6c72 2100 0000 720c 0000 00da 0676 616c  lr!...r......val
-00000bf0: 7565 7372 4300 0000 7245 0000 0072 2600  uesrC...rE...r&.
-00000c00: 0000 7244 0000 00da 0570 7269 6e74 722d  ..rD.....printr-
-00000c10: 0000 00da 0561 7272 6179 7240 0000 0072  .....arrayr@...r
-00000c20: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000c30: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000c40: 0073 2e00 0000 0400 0c03 0802 0c01 1002  .s..............
-00000c50: 1002 086f 0c02 0602 0a01 0a01 0802 0801  ...o............
-00000c60: 1401 0401 0201 0401 0401 0201 04fc 1006  ................
-00000c70: 1a01 04ee                                ....
+00000210: 007c 005f 0464 0053 0029 034e 7a25 4d6f  .|._.d.S.).Nz%Mo
+00000220: 6e6f 6420 6d6f 6465 6c62 2028 3120 7375  nod modelb (1 su
+00000230: 6273 7472 6174 652c 2031 2070 726f 6475  bstrate, 1 produ
+00000240: 6374 29e9 0100 0000 2905 da05 7375 7065  ct).....)...supe
+00000250: 72da 085f 5f69 6e69 745f 5fda 0a6d 6f64  r..__init__..mod
+00000260: 656c 5f6e 616d 65da 0476 696e 69da 1670  el_name..vini..p
+00000270: 6172 616d 6574 6572 735f 746f 5f65 7374  arameters_to_est
+00000280: 696d 6174 6529 02da 0473 656c 66da 0464  imate)...self..d
+00000290: 6174 61a9 01da 095f 5f63 6c61 7373 5f5f  ata....__class__
+000002a0: a900 fa58 433a 5c55 7365 7273 5c6d 696c  ...XC:\Users\mil
+000002b0: 6c61 7264 5c44 6f63 756d 656e 7473 5c47  lard\Documents\G
+000002c0: 4954 5c50 6879 7369 6f46 6974 5c50 6879  IT\PhysioFit\Phy
+000002d0: 7369 6f46 6974 5c50 6879 7369 6f46 6974  sioFit\PhysioFit
+000002e0: 5c70 6879 7369 6f66 6974 5c6d 6f64 656c  \physiofit\model
+000002f0: 735c 6d6f 6465 6c5f 362e 7079 7209 0000  s\model_6.pyr...
+00000300: 000d 0000 0073 0800 0000 0c02 0601 0601  .....s..........
+00000310: 0a01 7a13 4368 696c 644d 6f64 656c 2e5f  ..z.ChildModel._
+00000320: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000330: 0000 0000 0200 0000 0900 0000 4300 0001  ............C...
+00000340: 7306 0100 007c 006a 007c 006a 0064 019c  s....|.j.|.j.d..
+00000350: 027c 005f 0174 0264 0264 0364 018d 027c  .|._.t.d.d.d...|
+00000360: 005f 037c 006a 0444 005d 357d 017c 01a0  ._.|.j.D.]5}.|..
+00000370: 0564 04a1 0172 477c 006a 01a0 067c 019b  .d...rG|.j...|..
+00000380: 0064 059d 027c 006a 007c 019b 0064 069d  .d...|.j.|...d..
+00000390: 027c 006a 007c 019b 0064 079d 0264 0869  .|.j.|...d...d.i
+000003a0: 03a1 0101 007c 006a 03a0 067c 019b 0064  .....|.j...|...d
+000003b0: 059d 0264 097c 019b 0064 069d 0264 097c  ...d.|...d...d.|
+000003c0: 019b 0064 079d 0264 0a69 03a1 0101 0001  ...d...d.i......
+000003d0: 0071 4871 127c 006a 0444 005d 2a7d 017c  .qHq.|.j.D.]*}.|
+000003e0: 01a0 0564 0ba1 0172 757c 006a 01a0 067c  ...d...ru|.j...|
+000003f0: 019b 0064 0c9d 027c 006a 007c 019b 0064  ...d...|.j.|...d
+00000400: 0d9d 0264 0869 02a1 0101 007c 006a 03a0  ...d.i.....|.j..
+00000410: 067c 019b 0064 0c9d 0264 097c 019b 0064  .|...d...d.|...d
+00000420: 0d9d 0264 0a69 02a1 0101 0001 0071 7671  ...d.i.......qvq
+00000430: 4b74 077c 006a 0183 0164 0e6b 0372 8174  Kt.|.j...d.k.r.t
+00000440: 0864 0f83 0182 0164 0053 0029 104e 2902  .d.....d.S.).N).
+00000450: da03 585f 30da 0679 6c64 5f42 4d29 02e7  ..X_0..yld_BM)..
+00000460: fca9 f1d2 4d62 503f e90a 0000 0029 0272  ....MbP?.....).r
+00000470: 1500 0000 e903 0000 00da 0253 5fda 035f  ...........S_.._
+00000480: 6b6d da06 5f71 736d 6178 da04 5f73 5f30  km.._qsmax.._s_0
+00000490: e964 0000 0029 02e7 8ded b5a0 f7c6 b03e  .d...).........>
+000004a0: e932 0000 0029 0272 1d00 0000 e996 0000  .2...).r........
+000004b0: 00da 0250 5fda 065f 796c 645f 50da 045f  ...P_.._yld_P.._
+000004c0: 705f 30e9 0700 0000 7a86 5468 6973 206d  p_0.....z.This m
+000004d0: 6f64 656c 2065 7870 6563 7420 3220 6d65  odel expect 2 me
+000004e0: 7461 626f 6c69 7465 7320 696e 2074 6865  tabolites in the
+000004f0: 2064 6174 6166 696c 6520 2831 2073 7562   datafile (1 sub
+00000500: 7374 7261 7465 2077 6974 6820 6e61 6d65  strate with name
+00000510: 2073 7461 7274 696e 6720 7769 7468 2027   starting with '
+00000520: 535f 2720 616e 6420 3120 7072 6f64 7563  S_' and 1 produc
+00000530: 7420 7769 7468 206e 616d 6520 7374 6172  t with name star
+00000540: 7469 6e67 2077 6974 6820 2750 5f27 292e  ting with 'P_').
+00000550: 2909 720b 0000 0072 0c00 0000 7205 0000  ).r....r....r...
+00000560: 00da 0662 6f75 6e64 73da 0b6d 6574 6162  ...bounds..metab
+00000570: 6f6c 6974 6573 da0a 7374 6172 7473 7769  olites..startswi
+00000580: 7468 da06 7570 6461 7465 da03 6c65 6eda  th..update..len.
+00000590: 0a56 616c 7565 4572 726f 7229 0272 0d00  .ValueError).r..
+000005a0: 0000 da0a 6d65 7461 626f 6c69 7465 7211  ....metaboliter.
+000005b0: 0000 0072 1100 0000 7212 0000 00da 0a67  ...r....r......g
+000005c0: 6574 5f70 6172 616d 7314 0000 0073 5000  et_params....sP.
+000005d0: 0000 0403 0401 08fe 0205 0201 0201 08fe  ................
+000005e0: 0a05 0a01 0601 0c02 0c01 0a01 02fd 04ff  ................
+000005f0: 0607 0a02 0a01 0a01 02fd 04ff 0407 02f1  ................
+00000600: 0a11 0a01 0601 0c02 0a01 02fe 04ff 0607  ................
+00000610: 0a02 0a01 02fe 04ff 0406 02f2 0e10 0801  ................
+00000620: 04ff 7a15 4368 696c 644d 6f64 656c 2e67  ..z.ChildModel.g
+00000630: 6574 5f70 6172 616d 73da 0b70 6172 616d  et_params..param
+00000640: 735f 6f70 7469 da04 6c69 7374 da0b 6461  s_opti..list..da
+00000650: 7461 5f6d 6174 7269 78fa 0a6e 702e 6e64  ta_matrix..np.nd
+00000660: 6172 7261 79da 0b74 696d 655f 7665 6374  array..time_vect
+00000670: 6f72 da0f 7061 7261 6d73 5f6e 6f6e 5f6f  or..params_non_o
+00000680: 7074 69da 0464 6963 7463 0400 0000 0000  pti..dictc......
+00000690: 0000 0000 0000 0f00 0000 0800 0000 4300  ..............C.
+000006a0: 0001 7386 0000 007c 0064 0119 007d 047c  ..s....|.d...}.|
+000006b0: 0064 0219 007d 057c 0064 0319 007d 067c  .d...}.|.d...}.|
+000006c0: 0064 0419 007d 077c 0064 0519 007d 087c  .d...}.|.d...}.|
+000006d0: 0064 0619 007d 097c 0064 0719 007d 0a7c  .d...}.|.d...}.|
+000006e0: 047c 087c 0a67 037d 0b7c 057c 097c 067c  .|.|.g.}.|.|.|.|
+000006f0: 0766 047d 0c64 0864 0984 007d 0d74 007c  .f.}.d.d...}.t.|
+00000700: 0d74 01a0 027c 02a1 0174 01a0 037c 02a1  .t...|...t...|..
+00000710: 0166 027c 0b7c 0c64 0a74 047c 0283 0164  .f.|.|.d.t.|...d
+00000720: 0b8d 067d 0e7c 0e6a 056a 0653 0029 0c4e  ...}.|.j.j.S.).N
+00000730: 7201 0000 0072 0700 0000 e902 0000 0072  r....r.........r
+00000740: 1700 0000 e904 0000 00e9 0500 0000 e906  ................
+00000750: 0000 0063 0600 0000 0000 0000 0000 0000  ...c............
+00000760: 0e00 0000 0400 0000 5300 0001 7354 0000  ........S...sT..
+00000770: 007c 0164 0119 007d 067c 0164 0219 007d  .|.d...}.|.d...}
+00000780: 077c 057c 067c 047c 0617 001b 0014 007d  .|.|.|.|.......}
+00000790: 087c 087c 021b 007d 097c 037c 0814 007d  .|.|...}.|.|...}
+000007a0: 0a7c 087c 0714 007d 0b7c 090b 007c 0714  .|.|...}.|...|..
+000007b0: 007d 0c7c 0a7c 0714 007d 0d7c 0b7c 0c7c  .}.|.|...}.|.|.|
+000007c0: 0d66 0353 0029 034e 7201 0000 0072 0700  .f.S.).Nr....r..
+000007d0: 0000 7211 0000 0029 0eda 0174 da05 7374  ..r....)...t..st
+000007e0: 6174 65da 0379 6c64 da04 796c 6450 da02  ate..yld..yldP..
+000007f0: 6b6d da05 7173 6d61 78da 0373 5f74 da03  km..qsmax..s_t..
+00000800: 785f 74da 0471 735f 74da 046d 755f 74da  x_t..qs_t..mu_t.
+00000810: 0471 705f 74da 0264 78da 0264 73da 0264  .qp_t..dx..ds..d
+00000820: 7072 1100 0000 7211 0000 0072 1200 0000  pr....r....r....
+00000830: da14 6361 6c63 756c 6174 655f 6465 7269  ..calculate_deri
+00000840: 7661 7469 7665 5a00 0000 7312 0000 0008  vativeZ...s.....
+00000850: 0208 0110 0108 0108 0108 020a 0108 010a  ................
+00000860: 027a 3143 6869 6c64 4d6f 6465 6c2e 7369  .z1ChildModel.si
+00000870: 6d75 6c61 7465 2e3c 6c6f 6361 6c73 3e2e  mulate.<locals>.
+00000880: 6361 6c63 756c 6174 655f 6465 7269 7661  calculate_deriva
+00000890: 7469 7665 da05 4c53 4f44 4129 06da 0366  tive..LSODA)...f
+000008a0: 756e da06 745f 7370 616e da02 7930 da04  un..t_span..y0..
+000008b0: 6172 6773 da06 6d65 7468 6f64 da06 745f  args..method..t_
+000008c0: 6576 616c 2907 7203 0000 00da 026e 70da  eval).r......np.
+000008d0: 036d 696e da03 6d61 7872 2d00 0000 da01  .min..maxr-.....
+000008e0: 79da 0154 290f 722c 0000 0072 2e00 0000  y..T).r,...r....
+000008f0: 7230 0000 0072 3100 0000 da03 785f 3072  r0...r1.....x_0r
+00000900: 3900 0000 723b 0000 0072 3c00 0000 da03  9...r;...r<.....
+00000910: 735f 3072 3a00 0000 da03 705f 3072 3800  s_0r:.....p_0r8.
+00000920: 0000 da06 7061 7261 6d73 7245 0000 00da  ....paramsrE....
+00000930: 0373 6f6c 7211 0000 0072 1100 0000 7212  .solr....r....r.
+00000940: 0000 00da 0873 696d 756c 6174 6547 0000  .....simulateG..
+00000950: 0073 2600 0000 0809 0801 0801 0801 0801  .s&.............
+00000960: 0801 0801 0a01 0c01 0802 020e 0201 1201  ................
+00000970: 0201 0201 0201 0601 06fa 0809 7a13 4368  ............z.Ch
+00000980: 696c 644d 6f64 656c 2e73 696d 756c 6174  ildModel.simulat
+00000990: 6529 0872 2c00 0000 722d 0000 0072 2e00  e).r,...r-...r..
+000009a0: 0000 722f 0000 0072 3000 0000 722f 0000  ..r/...r0...r/..
+000009b0: 0072 3100 0000 7232 0000 0029 08da 085f  .r1...r2...)..._
+000009c0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000009d0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000009e0: 5f72 0900 0000 722b 0000 00da 0c73 7461  _r....r+.....sta
+000009f0: 7469 636d 6574 686f 6472 5700 0000 da0d  ticmethodrW.....
+00000a00: 5f5f 636c 6173 7363 656c 6c5f 5f72 1100  __classcell__r..
+00000a10: 0000 7211 0000 0072 0f00 0000 7212 0000  ..r....r....r...
+00000a20: 0072 0600 0000 0b00 0000 730a 0000 0008  .r........s.....
+00000a30: 000c 0208 0702 3314 0172 0600 0000 da08  ......3..r......
+00000a40: 5f5f 6d61 696e 5f5f 2901 da09 496f 4861  __main__)...IoHa
+00000a50: 6e64 6c65 727a 5a43 3a5c 5573 6572 735c  ndlerzZC:\Users\
+00000a60: 6c65 6772 6567 616d 5c50 7963 6861 726d  legregam\Pycharm
+00000a70: 5072 6f6a 6563 7473 5c50 6879 7369 6f46  Projects\PhysioF
+00000a80: 6974 5c64 6174 615c 4b45 494f 5f74 6573  it\data\KEIO_tes
+00000a90: 745f 6461 7461 5c6f 6465 5f74 6573 745c  t_data\ode_test\
+00000aa0: 4b45 494f 5f52 4f42 4f54 365f 312e 7473  KEIO_ROBOT6_1.ts
+00000ab0: 76da 0474 696d 6563 0100 0000 0000 0000  v..timec........
+00000ac0: 0000 0000 0200 0000 0300 0000 4300 0001  ............C...
+00000ad0: 7310 0000 0067 007c 005d 047d 017c 0191  s....g.|.].}.|..
+00000ae0: 0271 0253 0072 1100 0000 7211 0000 0029  .q.S.r....r....)
+00000af0: 02da 022e 30da 0570 6172 616d 7211 0000  ....0..paramr...
+00000b00: 0072 1100 0000 7212 0000 00da 0a3c 6c69  .r....r......<li
+00000b10: 7374 636f 6d70 3e7d 0000 0073 0200 0000  stcomp>}...s....
+00000b20: 1000 7262 0000 007a 0754 696d 6573 3a20  ..rb...z.Times: 
+00000b30: 7a08 5661 6c75 6573 3a20 291e da07 5f5f  z.Values: )...__
+00000b40: 646f 635f 5fda 0a5f 5f66 7574 7572 655f  doc__..__future_
+00000b50: 5f72 0200 0000 da05 6e75 6d70 7972 4d00  _r......numpyrM.
+00000b60: 0000 da0f 7363 6970 792e 696e 7465 6772  ....scipy.integr
+00000b70: 6174 6572 0300 0000 da1b 7068 7973 696f  ater......physio
+00000b80: 6669 742e 6d6f 6465 6c73 2e62 6173 655f  fit.models.base_
+00000b90: 6d6f 6465 6c72 0400 0000 7205 0000 0072  modelr....r....r
+00000ba0: 0600 0000 7258 0000 00da 1170 6879 7369  ....rX.....physi
+00000bb0: 6f66 6974 2e62 6173 652e 696f 725e 0000  ofit.base.ior^..
+00000bc0: 00da 0269 6fda 0972 6561 645f 6461 7461  ...io..read_data
+00000bd0: 720e 0000 00da 0b73 6f72 745f 7661 6c75  r......sort_valu
+00000be0: 6573 da05 6d6f 6465 6c72 2b00 0000 720c  es..modelr+...r.
+00000bf0: 0000 00da 0676 616c 7565 7372 5500 0000  .....valuesrU...
+00000c00: 7257 0000 0072 3000 0000 7256 0000 00da  rW...r0...rV....
+00000c10: 0570 7269 6e74 7237 0000 00da 0561 7272  .printr7.....arr
+00000c20: 6179 7250 0000 0072 1100 0000 7211 0000  ayrP...r....r...
+00000c30: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
+00000c40: 6475 6c65 3e01 0000 0073 2e00 0000 0400  dule>....s......
+00000c50: 0c03 0802 0c01 1002 1002 0868 0c02 0602  ...........h....
+00000c60: 0a01 0a01 0802 0801 1401 0401 0201 0401  ................
+00000c70: 0401 0201 04fc 1006 1a01 04ee            ............
```

### Comparing `physiofit-3.0.4/physiofit/models/base_model.py` & `physiofit-3.0.6/physiofit/models/base_model.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from ast import literal_eval
-
-import pandas as pd
-import numpy as np
-
-
-# Initialization: nom des métabolites en entrée
-
-# Get les parametres en fonction du modèle: retourne les noms des paramètres
-# (optimisables et non),leurs valeurs initiales et les bounds pour ceux qui
-# sont optimisables
-
-# Besoin d'une fonction simulate propre au modèle qui prends les temps,
-# les paramètres optimisables optimisables et non optimisables
-
-
-class Model(ABC):
-
-    def __init__(self, data: pd.DataFrame):
-        self.data = data
-        self.time_vector = self.data.time.to_numpy()
-        if "time" in self.data.columns and "experiments" in self.data.columns:
-            self.name_vector = self.data.drop(["time", "experiments"], axis=1).columns.to_list()
-        elif "time" in self.data.columns:
-            self.name_vector = self.data.drop(["time"], axis=1).columns.to_list()
-        else:
-            raise ValueError(
-                "Couldn't get column names from data. Is data loaded in properly and well formatted?"
-            )
-        self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
-        self.metabolites = self.name_vector[1:]
-        self.model_name = None
-        self.parameters_to_estimate = None
-        self.fixed_parameters = None
-        self.bounds = None
-
-
-    def __repr__(self):
-        return f"Selected model: {self.model_name}\n" \
-               f"Model data: \n{self.data}\n" \
-               f"Experimental matrix: \n{self.experimental_matrix}\n" \
-               f"Time vector: {self.time_vector}\n" \
-               f"Name vector: {self.name_vector}\n" \
-               f"Metabolites: {self.metabolites}\n" \
-               f"Parameters to estimate: {self.parameters_to_estimate}\n" \
-               f"Fixed parameters: {self.fixed_parameters}\n" \
-               f"Bounds: {self.bounds}\n"
-
-    def __setattr__(self, key, value):
-        if key == "data":
-            self.__dict__["data"] = value
-            self.time_vector = self.data.time.to_numpy()
-            self.name_vector = self.data.drop("time", axis=1).columns.to_list()
-            self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
-            self.metabolites = self.name_vector[1:]
-        else:
-            self.__dict__[key] = value
-
-    @ abstractmethod
-    def get_params(self):
-        """
-
-        :return params_to_estimate: List of parameters to estimate
-        :return fixed_parameters: dict of constant parameters
-        :return bounds: dict of upper and lower bounds
-        :return default_init_values: dict containing default initial values for
-                                    params
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def simulate(
-            params_opti: list,
-            data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            params_non_opti: dict | list
-    ):
-        pass
-
-
-class Bounds(dict):
-
-    def __init__(self, mapping=None, **kwargs):
-
-        if mapping is None:
-            mapping = {}
-        if kwargs:
-            mapping.update(
-                {key: value for key, value in kwargs.items()}
-            )
-
-        for key, value in mapping.items():
-            key, value = self._check_bounds(key, value)
-            mapping[key] = value
-
-        super().__init__(mapping)
-
-    def __call__(self):
-
-        tuples = tuple(value for value in self.values())
-        return tuples
-
-    def __setitem__(self, key, value):
-
-        key, value = self._check_bounds(key, value)
-        super().__setitem__(key, value)
-
-    @staticmethod
-    def _check_bounds(key, value):
-
-        if not isinstance(value, tuple):
-            if isinstance(value, str):
-                try:
-                    value = literal_eval(value)
-                except Exception:
-                    raise TypeError(
-                        f"Could not coerce {value} into string"
-                    )
-        for x in value:
-            if not isinstance(x, int) and not isinstance(x, float):
-                raise TypeError(
-                    "Individual bound values must be numbers"
-                )
-        if value[0] >= value[1]:
-            raise ValueError(
-                "Lower bound cannot be higher than upper bound. "
-            )
-        if len(value) != 2:
-            raise ValueError(
-                "Bounds can only have two values. Number of values detected: "
-                f"{len(value)}"
-            )
-        if not isinstance(key, str):
-            raise TypeError(
-                "Name for bounds must be strings"
-            )
-        return key, value
-
-
-class StandardDevs(dict):
-
-    def __init__(self, mapping=None, **kwargs):
-
-        self._vector = None
-
-        if mapping is None:
-            mapping = {}
-        if kwargs:
-            mapping.update(
-                {key: value for key, value in kwargs.items()}
-            )
-
-        for key, value in mapping.items():
-            self._check_sd(key, value)
-
-        super().__init__(mapping)
-
-    @staticmethod
-    def _check_sd(key, value):
-
-        if not isinstance(key, str):
-            raise TypeError(
-                f"SD name field can only contain strings. Detected type {type(key)} for {key}"
-            )
-        if not isinstance(value, int) and not isinstance(value, float):
-            try:
-                value = float(value)
-            except Exception:
-                raise TypeError(
-                    f"SD value must be a number. Detected type: {type(value)} for {key}"
-                )
-        if value <= 0:
-            raise ValueError(
-                f"SD value must be superior to 0. Detected value: {value} for {key}"
-            )
-
-    def __setitem__(self, key, value):
-
-        self._check_sd(key, value)
-        super().__setitem__(key, value)
-
-    @property
-    def vector(self):
-
-        if self._vector is not None:
-            return self._vector
-        self._vector = np.array([value for value in self.values])
-        return self._vector
-
-class ModelError(Exception):
-    pass
-
-
-if __name__ == "__main__":
-    bounds = Bounds(
-        X_0=(1e-3, 10),
-        mu=(1e-3, 3)
-    )
-    print(bounds())
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from ast import literal_eval
+
+import pandas as pd
+import numpy as np
+
+
+# Initialization: nom des métabolites en entrée
+
+# Get les parametres en fonction du modèle: retourne les noms des paramètres
+# (optimisables et non),leurs valeurs initiales et les bounds pour ceux qui
+# sont optimisables
+
+# Besoin d'une fonction simulate propre au modèle qui prends les temps,
+# les paramètres optimisables optimisables et non optimisables
+
+
+class Model(ABC):
+
+    def __init__(self, data: pd.DataFrame):
+        self.data = data
+        self.time_vector = self.data.time.to_numpy()
+        if "time" in self.data.columns and "experiments" in self.data.columns:
+            self.name_vector = self.data.drop(["time", "experiments"], axis=1).columns.to_list()
+        elif "time" in self.data.columns:
+            self.name_vector = self.data.drop(["time"], axis=1).columns.to_list()
+        else:
+            raise ValueError(
+                "Couldn't get column names from data. Is data loaded in properly and well formatted?"
+            )
+        self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
+        self.metabolites = self.name_vector[1:]
+        self.model_name = None
+        self.parameters_to_estimate = None
+        self.fixed_parameters = None
+        self.bounds = None
+
+
+    def __repr__(self):
+        return f"Selected model: {self.model_name}\n" \
+               f"Model data: \n{self.data}\n" \
+               f"Experimental matrix: \n{self.experimental_matrix}\n" \
+               f"Time vector: {self.time_vector}\n" \
+               f"Name vector: {self.name_vector}\n" \
+               f"Metabolites: {self.metabolites}\n" \
+               f"Parameters to estimate: {self.parameters_to_estimate}\n" \
+               f"Fixed parameters: {self.fixed_parameters}\n" \
+               f"Bounds: {self.bounds}\n"
+
+    def __setattr__(self, key, value):
+        if key == "data":
+            self.__dict__["data"] = value
+            self.time_vector = self.data.time.to_numpy()
+            self.name_vector = self.data.drop("time", axis=1).columns.to_list()
+            self.experimental_matrix = self.data.drop("time", axis=1).to_numpy()
+            self.metabolites = self.name_vector[1:]
+        else:
+            self.__dict__[key] = value
+
+    @ abstractmethod
+    def get_params(self):
+        """
+
+        :return params_to_estimate: List of parameters to estimate
+        :return fixed_parameters: dict of constant parameters
+        :return bounds: dict of upper and lower bounds
+        :return default_init_values: dict containing default initial values for
+                                    params
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def simulate(
+            params_opti: list,
+            data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            params_non_opti: dict | list
+    ):
+        pass
+
+
+class Bounds(dict):
+
+    def __init__(self, mapping=None, **kwargs):
+
+        if mapping is None:
+            mapping = {}
+        if kwargs:
+            mapping.update(
+                {key: value for key, value in kwargs.items()}
+            )
+
+        for key, value in mapping.items():
+            key, value = self._check_bounds(key, value)
+            mapping[key] = value
+
+        super().__init__(mapping)
+
+    def __call__(self):
+
+        tuples = tuple(value for value in self.values())
+        return tuples
+
+    def __setitem__(self, key, value):
+
+        key, value = self._check_bounds(key, value)
+        super().__setitem__(key, value)
+
+    @staticmethod
+    def _check_bounds(key, value):
+
+        if not isinstance(value, tuple):
+            if isinstance(value, str):
+                try:
+                    value = literal_eval(value)
+                except Exception:
+                    raise TypeError(
+                        f"Could not coerce {value} into string"
+                    )
+        for x in value:
+            if not isinstance(x, int) and not isinstance(x, float):
+                raise TypeError(
+                    "Individual bound values must be numbers"
+                )
+        if value[0] >= value[1]:
+            raise ValueError(
+                "Lower bound cannot be higher than upper bound. "
+            )
+        if len(value) != 2:
+            raise ValueError(
+                "Bounds can only have two values. Number of values detected: "
+                f"{len(value)}"
+            )
+        if not isinstance(key, str):
+            raise TypeError(
+                "Name for bounds must be strings"
+            )
+        return key, value
+
+
+class StandardDevs(dict):
+
+    def __init__(self, mapping=None, **kwargs):
+
+        self._vector = None
+
+        if mapping is None:
+            mapping = {}
+        if kwargs:
+            mapping.update(
+                {key: value for key, value in kwargs.items()}
+            )
+
+        for key, value in mapping.items():
+            self._check_sd(key, value)
+
+        super().__init__(mapping)
+
+    @staticmethod
+    def _check_sd(key, value):
+
+        if not isinstance(key, str):
+            raise TypeError(
+                f"SD name field can only contain strings. Detected type {type(key)} for {key}"
+            )
+        if not isinstance(value, int) and not isinstance(value, float):
+            try:
+                value = float(value)
+            except Exception:
+                raise TypeError(
+                    f"SD value must be a number. Detected type: {type(value)} for {key}"
+                )
+        if value <= 0:
+            raise ValueError(
+                f"SD value must be superior to 0. Detected value: {value} for {key}"
+            )
+
+    def __setitem__(self, key, value):
+
+        self._check_sd(key, value)
+        super().__setitem__(key, value)
+
+    @property
+    def vector(self):
+
+        if self._vector is not None:
+            return self._vector
+        self._vector = np.array([value for value in self.values])
+        return self._vector
+
+class ModelError(Exception):
+    pass
+
+
+if __name__ == "__main__":
+    bounds = Bounds(
+        X_0=(1e-3, 10),
+        mu=(1e-3, 3)
+    )
+    print(bounds())
```

### Comparing `physiofit-3.0.4/physiofit/models/model_2.py` & `physiofit-3.0.6/physiofit/models/model_1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,105 @@
-"""
-Module containing the methods used by PhysioFit.
-"""
-
-from __future__ import annotations
-import numpy as np
-
-from physiofit.models.base_model import Model, Bounds
-
-
-class ChildModel(Model):
-
-    def __init__(self, data):
-
-        super().__init__(data)
-        self.model_name = "Steady-state batch model with lag phase"
-        self.vini = 1
-        self.parameters_to_estimate = None
-        self.fixed_parameters = None
-
-    def get_params(self):
-
-        self.parameters_to_estimate = {
-            "X_0" : self.vini,
-            "mu" : self.vini,
-            "t_lag" : self.vini
-        }
-        self.bounds = Bounds({
-            "X_0": (1e-3, 10),
-            "mu": (1e-3, 3),
-            "t_lag": (0, 0.5 * self.time_vector.max()),
-        })
-        for metabolite in self.metabolites:
-            self.parameters_to_estimate.update(
-                {
-                    f"{metabolite}_q" : 1,
-                    f"{metabolite}_M0" : 1
-                }
-            )
-            self.bounds.update(
-                {
-                    f"{metabolite}_q": (-50, 50),
-                    f"{metabolite}_M0": (1e-6, 50)
-                }
-            )
-
-    @staticmethod
-    def simulate(
-            params_opti: list,
-            data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            params_non_opti: dict | list
-    ):
-        # Get end shape
-        simulated_matrix = np.empty_like(data_matrix)
-        x_0 = params_opti[0]
-        mu = params_opti[1]
-        t_lag = params_opti[2]
-
-        # We get indices in time vector where time < t_lag
-        idx = np.nonzero(time_vector < t_lag)
-
-        # Fill at those indices with x_0
-        x_t_lag = np.full((len(idx) - 1,), x_0)
-
-        # The rest of the biomass points are calculated as usual
-        mult_by_time = x_0 * np.exp(mu * (time_vector[len(idx) - 1:] - t_lag))
-
-        # Concatenate both vectors and transfer to X_t column of the
-        # simulated matrix
-        simulated_matrix[:, 0] = np.concatenate(
-            (x_t_lag, mult_by_time),
-            axis=None
-        )
-        exp_mu_t_lag = np.exp(mu * (time_vector - t_lag)) - 1
-
-        for i in range(1, int(len(params_opti) / 2)):
-            q = params_opti[i * 2 + 1]
-            m_0 = params_opti[i * 2 + 2]
-            m_t_lag = np.full((len(idx) - 1,), m_0)
-            mult_by_time = q * (x_0 / mu) * exp_mu_t_lag + m_0
-            simulated_matrix[:, i] = np.concatenate(
-                (m_t_lag, mult_by_time),
-                axis=None
-            )
-
-        return simulated_matrix
+"""
+Module containing the methods used by PhysioFit.
+"""
+from __future__ import annotations
+
+import numpy as np
+import pandas as pd
+
+from physiofit.models.base_model import Model, Bounds
+
+class ChildModel(Model):
+
+    def __init__(self, data):
+
+        super().__init__(data)
+        self.model_name = "Steady-state batch model with lag phase and " \
+                          "degradation of metabolites "
+        self.vini = 1
+        self.parameters_to_estimate = None
+        self.fixed_parameters = None
+
+    def get_params(self):
+
+        self.parameters_to_estimate = {
+            "X_0" : self.vini,
+            "mu" : self.vini,
+            "t_lag" : self.vini
+        }
+        self.bounds = Bounds(
+            X_0=(1e-3, 10),
+            mu=(1e-3, 3),
+            t_lag = (0, 0.5*self.time_vector.max())
+        )
+        for metabolite in self.metabolites:
+            self.parameters_to_estimate.update(
+                {
+                    f"{metabolite}_q" : self.vini,
+                    f"{metabolite}_M0" : self.vini
+                }
+            )
+            self.bounds.update(
+                {
+                    f"{metabolite}_q": (-50, 50),
+                    f"{metabolite}_M0": (1e-6, 50)
+                }
+            )
+
+        self.fixed_parameters = {"Degradation": {
+            met: 0 for met in self.metabolites
+            }
+        }
+
+    @staticmethod
+    def simulate(
+            params_opti: list,
+            data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            params_non_opti: dict
+    ):
+        # Get end shape
+        simulated_matrix = np.empty_like(data_matrix)
+
+        # Get initial params
+        x_0 = params_opti[0]
+        mu = params_opti[1]
+        t_lag = params_opti[2]
+
+        # We get indices in time vector where time < t_lag
+        idx = np.nonzero(time_vector < t_lag)
+
+        # Fill at those indices with x_0
+        x_t_lag = np.full((len(idx) - 1,), x_0)
+
+        # The rest of the biomass points are calculated as usual
+        mult_by_time = x_0 * np.exp(mu * (time_vector[len(idx) - 1:] - t_lag))
+        simulated_matrix[:, 0] = np.concatenate((x_t_lag, mult_by_time),
+                                                axis=None)
+        fixed_params = [value for value in params_non_opti["Degradation"].values()]
+
+        for i in range(1, int(len(params_opti) / 2)):
+            q = params_opti[i * 2 + 1]
+            m_0 = params_opti[i * 2 + 2]
+            k = fixed_params[i - 1]
+            m_t_lag = np.full((len(idx) - 1,), m_0)
+            mult_by_time = q * (x_0 / (mu + k)) * (np.exp(
+                mu * (time_vector - t_lag)
+            ) - np.exp(-k * (time_vector - t_lag))) + (m_0 * np.exp(
+                -k * time_vector)
+                                                       )
+            simulated_matrix[:, i] = np.concatenate(
+                (m_t_lag, mult_by_time),
+                axis=None
+            )
+
+        return simulated_matrix
+
+
+if __name__ == "__main__":
+    model = ChildModel(
+        pd.read_csv(
+            r"C:\Users\legregam\Documents\Projets\PhysioFit\data"
+            r"\KEIO_test_data\KEIO_ROBOT6_1\KEIO_ROBOT6_1.tsv",
+            sep='\t')
+    )
+    print(type(model))
```

### Comparing `physiofit-3.0.4/physiofit/models/model_3.py` & `physiofit-3.0.6/physiofit/models/model_3.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""
-Module containing the methods used by PhysioFit.
-"""
-
-from __future__ import annotations
-import numpy as np
-
-from physiofit.models.base_model import Model, Bounds
-
-
-class ChildModel(Model):
-
-    def __init__(self, data):
-
-        super().__init__(data)
-        self.model_name = "Steady-state batch model with degradation of metabolites"
-        self.vini = 1
-        self.parameters_to_estimate = None
-        self.fixed_parameters = None
-
-    def get_params(self):
-
-        self.parameters_to_estimate = {
-            "X_O" : self.vini,
-            "mu" : self.vini
-        }
-        self.fixed_parameters = {"Degradation": {
-            met: 0 for met in self.metabolites
-            }
-        }
-        self.bounds = Bounds({
-            "X_0": (1e-3, 10),
-            "mu": (1e-3, 3),
-        })
-        for metabolite in self.metabolites:
-            self.parameters_to_estimate.update(
-                {
-                    f"{metabolite}_q": self.vini,
-                    f"{metabolite}_M0": self.vini
-                }
-            )
-            self.bounds.update(
-                {
-                    f"{metabolite}_q": (-50, 50),
-                    f"{metabolite}_M0": (1e-6, 50)
-                }
-            )
-            self.fixed_parameters = {"Degradation": {
-                met: 0 for met in self.metabolites
-                }
-            }
-
-    @staticmethod
-    def simulate(
-            params_opti: list,
-            data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            params_non_opti: dict | list
-    ):
-        # Get end shape
-        simulated_matrix = np.empty_like(data_matrix)
-
-        # Get initial params
-        x_0 = params_opti[0]
-        mu = params_opti[1]
-
-        # Get X_0 values
-        exp_mu_t = np.exp(mu * time_vector)
-        simulated_matrix[:, 0] = x_0 * exp_mu_t
-        fixed_params = [value for value in params_non_opti["Degradation"].values()]
-
-        for i in range(1, int(len(params_opti) / 2)):
-            q = params_opti[i * 2]
-            m_0 = params_opti[i * 2 + 1]
-            k = fixed_params[i - 1]
-            exp_k_t = np.exp(-k * time_vector)
-            simulated_matrix[:, i] = q * (x_0 / (mu + k)) \
-                                     * (exp_mu_t - exp_k_t) \
-                                     + m_0 * exp_k_t
-
-        return simulated_matrix
+"""
+Module containing the methods used by PhysioFit.
+"""
+
+from __future__ import annotations
+import numpy as np
+
+from physiofit.models.base_model import Model, Bounds
+
+
+class ChildModel(Model):
+
+    def __init__(self, data):
+
+        super().__init__(data)
+        self.model_name = "Steady-state batch model with degradation of metabolites"
+        self.vini = 1
+        self.parameters_to_estimate = None
+        self.fixed_parameters = None
+
+    def get_params(self):
+
+        self.parameters_to_estimate = {
+            "X_O" : self.vini,
+            "mu" : self.vini
+        }
+        self.fixed_parameters = {"Degradation": {
+            met: 0 for met in self.metabolites
+            }
+        }
+        self.bounds = Bounds({
+            "X_0": (1e-3, 10),
+            "mu": (1e-3, 3),
+        })
+        for metabolite in self.metabolites:
+            self.parameters_to_estimate.update(
+                {
+                    f"{metabolite}_q": self.vini,
+                    f"{metabolite}_M0": self.vini
+                }
+            )
+            self.bounds.update(
+                {
+                    f"{metabolite}_q": (-50, 50),
+                    f"{metabolite}_M0": (1e-6, 50)
+                }
+            )
+            self.fixed_parameters = {"Degradation": {
+                met: 0 for met in self.metabolites
+                }
+            }
+
+    @staticmethod
+    def simulate(
+            params_opti: list,
+            data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            params_non_opti: dict | list
+    ):
+        # Get end shape
+        simulated_matrix = np.empty_like(data_matrix)
+
+        # Get initial params
+        x_0 = params_opti[0]
+        mu = params_opti[1]
+
+        # Get X_0 values
+        exp_mu_t = np.exp(mu * time_vector)
+        simulated_matrix[:, 0] = x_0 * exp_mu_t
+        fixed_params = [value for value in params_non_opti["Degradation"].values()]
+
+        for i in range(1, int(len(params_opti) / 2)):
+            q = params_opti[i * 2]
+            m_0 = params_opti[i * 2 + 1]
+            k = fixed_params[i - 1]
+            exp_k_t = np.exp(-k * time_vector)
+            simulated_matrix[:, i] = q * (x_0 / (mu + k)) \
+                                     * (exp_mu_t - exp_k_t) \
+                                     + m_0 * exp_k_t
+
+        return simulated_matrix
```

### Comparing `physiofit-3.0.4/physiofit/models/model_4.py` & `physiofit-3.0.6/physiofit/models/model_4.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-Module containing the methods used by PhysioFit.
-"""
-
-from __future__ import annotations
-import numpy as np
-
-from physiofit.models.base_model import Model, Bounds
-
-
-class ChildModel(Model):
-
-    def __init__(self, data):
-
-        super().__init__(data)
-        self.model_name = "Steady-state batch model"
-        self.vini = 1
-        self.parameters_to_estimate = None
-        self.fixed_parameters = None
-
-    def get_params(self):
-
-        self.parameters_to_estimate = {
-            "X_0" : self.vini,
-            "mu" : self.vini
-        }
-        self.bounds = Bounds({
-            "X_0": (1e-3, 10),
-            "mu": (1e-3, 3)
-        })
-        for metabolite in self.metabolites:
-            self.parameters_to_estimate.update(
-                {
-                    f"{metabolite}_q" : self.vini,
-                    f"{metabolite}_M0" : self.vini
-                }
-            )
-            self.bounds.update(
-                {
-                    f"{metabolite}_q": (-50, 50),
-                    f"{metabolite}_M0": (1e-6, 50)
-                }
-            )
-
-    @staticmethod
-    def simulate(
-            params_opti: list,
-            data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            params_non_opti: dict | list
-    ):
-        # Get end shape
-        simulated_matrix = np.empty_like(data_matrix)
-        x_0 = params_opti[0]
-        mu = params_opti[1]
-        exp_mu_t = np.exp(mu * time_vector)
-        simulated_matrix[:, 0] = x_0 * exp_mu_t
-        for i in range(1, int(len(params_opti) / 2)):
-            q = params_opti[i * 2]
-            m_0 = params_opti[i * 2 + 1]
-            simulated_matrix[:, i] = q * (x_0 / mu) \
-                                     * (exp_mu_t - 1) \
-                                     + m_0
-
-        return simulated_matrix
+"""
+Module containing the methods used by PhysioFit.
+"""
+
+from __future__ import annotations
+import numpy as np
+
+from physiofit.models.base_model import Model, Bounds
+
+
+class ChildModel(Model):
+
+    def __init__(self, data):
+
+        super().__init__(data)
+        self.model_name = "Steady-state batch model"
+        self.vini = 1
+        self.parameters_to_estimate = None
+        self.fixed_parameters = None
+
+    def get_params(self):
+
+        self.parameters_to_estimate = {
+            "X_0" : self.vini,
+            "mu" : self.vini
+        }
+        self.bounds = Bounds({
+            "X_0": (1e-3, 10),
+            "mu": (1e-3, 3)
+        })
+        for metabolite in self.metabolites:
+            self.parameters_to_estimate.update(
+                {
+                    f"{metabolite}_q" : self.vini,
+                    f"{metabolite}_M0" : self.vini
+                }
+            )
+            self.bounds.update(
+                {
+                    f"{metabolite}_q": (-50, 50),
+                    f"{metabolite}_M0": (1e-6, 50)
+                }
+            )
+
+    @staticmethod
+    def simulate(
+            params_opti: list,
+            data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            params_non_opti: dict | list
+    ):
+        # Get end shape
+        simulated_matrix = np.empty_like(data_matrix)
+        x_0 = params_opti[0]
+        mu = params_opti[1]
+        exp_mu_t = np.exp(mu * time_vector)
+        simulated_matrix[:, 0] = x_0 * exp_mu_t
+        for i in range(1, int(len(params_opti) / 2)):
+            q = params_opti[i * 2]
+            m_0 = params_opti[i * 2 + 1]
+            simulated_matrix[:, i] = q * (x_0 / mu) \
+                                     * (exp_mu_t - 1) \
+                                     + m_0
+
+        return simulated_matrix
```

### Comparing `physiofit-3.0.4/physiofit/models/model_5.py` & `physiofit-3.0.6/physiofit/models/model_5.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-"""
-Module containing a dynamic growth and flux estimation model
-"""
-from __future__ import annotations
-
-import numpy as np
-from scipy.integrate import solve_ivp
-
-from physiofit.models.base_model import Model, Bounds
-
-class ChildModel(Model):
-
-    def __init__(self, data):
-
-        super().__init__(data)
-        self.model_name = "Dynamic Monod model (1 substrate, 1 product)"
-        self.vini = 1
-        self.parameters_to_estimate = None
-
-    def get_params(self):
-
-        self.parameters_to_estimate = {
-            "X_0": self.vini,
-            "y_BM": self.vini
-        }
-
-        self.bounds = Bounds(
-            X_0=(1e-3, 10),
-            y_BM=(1e-3, 3)
-        )
-
-        for metabolite in self.metabolites:
-            if metabolite.startswith("S_"):
-                self.parameters_to_estimate.update(
-                    {
-                        f"{metabolite}_km": self.vini,
-                        f"{metabolite}_qsmax": self.vini,
-                        f"{metabolite}_s_0": 100
-                    }
-                )
-                self.bounds.update(
-                    {
-                        f"{metabolite}_km": (1e-6, 100),
-                        f"{metabolite}_qsmax": (1e-6, 100),
-                        f"{metabolite}_s_0": (1e-6, 100)
-                    }
-                )
-                break
-                
-        for metabolite in self.metabolites:
-            if metabolite.startswith("P_"):
-                self.parameters_to_estimate.update(
-                    {
-                        f"{metabolite}_y_P": self.vini,
-                        f"{metabolite}_p_0": 100
-                    }
-
-                )
-                self.bounds.update(
-                    {
-                        f"{metabolite}_y_P": (1e-6, 100),
-                        f"{metabolite}_p_0": (1e-6, 100)
-                    }
-                )
-                break
-
-        if len(self.parameters_to_estimate) != 7:
-            raise ValueError("This model expects 2 metabolites in the data file (1 substrate with name starting with 'S_' and 1 product with name starting with 'P_').")
-
-
-    @staticmethod
-    def simulate(
-            params_opti: list,
-            data_matrix: np.ndarray,
-            time_vector: np.ndarray,
-            params_non_opti: dict
-    ):
-
-        # Get parameters
-        x_0 = params_opti[0]
-        y_BM = params_opti[1]
-        km = params_opti[2]
-        qsmax = params_opti[3]
-        s_0 = params_opti[4]
-        y_P = params_opti[5]
-        p_0 = params_opti[6]
-        params = (y_BM, y_P, km, qsmax)
-
-        # initialize variables at t=0
-        state = [x_0, s_0, p_0]
-        
-        def calculate_derivative(t, state, y_BM, y_P, km, qsmax):
-            
-            # get substrate and biomass concentrations
-            s_t = state[0]
-            x_t = state[1]
-
-            # calculate fluxes
-            qs_t = qsmax * (s_t / (km + s_t))
-            mu_t = y_BM * qs_t
-            qp_t = y_P * qs_t
-
-            # calculate derivatives
-            dx = mu_t * x_t
-            ds = -qs_t * x_t
-            dp = qp_t * x_t
-
-            return dx, ds, dp
-
-        # simulate time-course concentrations
-        sol = solve_ivp(
-            fun=calculate_derivative,
-            t_span=(np.min(time_vector), np.max(time_vector)),
-            y0 = state,
-            args=params,
-            method="LSODA",
-            t_eval = list(time_vector)
-        )
-
-        return sol.y.T
-
-if __name__ == "__main__":
-
-    from physiofit.base.io import IoHandler
-
-    io = IoHandler()
-    data = io.read_data(r"C:\Users\legregam\PycharmProjects\PhysioFit\data\KEIO_test_data\ode_test\KEIO_ROBOT6_1.tsv")
-    data = data.sort_values("time")
-
-    model = ChildModel(data)
-    model.get_params()
-    params = [param for param in model.parameters_to_estimate.values()]
-    sol = ChildModel.simulate(
-        params,
-        model.data,
-        model.time_vector,
-        None
-    )
-    print(f"Times: {sol.t}")
-    print(f"Values: {np.array(sol.y)}")
+"""
+Module containing a dynamic growth and flux estimation model
+"""
+from __future__ import annotations
+
+import numpy as np
+from scipy.integrate import solve_ivp
+
+from physiofit.models.base_model import Model, Bounds
+
+class ChildModel(Model):
+
+    def __init__(self, data):
+
+        super().__init__(data)
+        self.model_name = "Dynamic Monod model (1 substrate, 1 product)"
+        self.vini = 1
+        self.parameters_to_estimate = None
+
+    def get_params(self):
+
+        self.parameters_to_estimate = {
+            "X_0": self.vini,
+            "y_BM": self.vini
+        }
+
+        self.bounds = Bounds(
+            X_0=(1e-3, 10),
+            y_BM=(1e-3, 3)
+        )
+
+        for metabolite in self.metabolites:
+            if metabolite.startswith("S_"):
+                self.parameters_to_estimate.update(
+                    {
+                        f"{metabolite}_km": self.vini,
+                        f"{metabolite}_qsmax": self.vini,
+                        f"{metabolite}_s_0": 100
+                    }
+                )
+                self.bounds.update(
+                    {
+                        f"{metabolite}_km": (1e-6, 100),
+                        f"{metabolite}_qsmax": (1e-6, 100),
+                        f"{metabolite}_s_0": (1e-6, 100)
+                    }
+                )
+                break
+                
+        for metabolite in self.metabolites:
+            if metabolite.startswith("P_"):
+                self.parameters_to_estimate.update(
+                    {
+                        f"{metabolite}_y_P": self.vini,
+                        f"{metabolite}_p_0": 100
+                    }
+
+                )
+                self.bounds.update(
+                    {
+                        f"{metabolite}_y_P": (1e-6, 100),
+                        f"{metabolite}_p_0": (1e-6, 100)
+                    }
+                )
+                break
+
+        if len(self.parameters_to_estimate) != 7:
+            raise ValueError("This model expects 2 metabolites in the data file (1 substrate with name starting with 'S_' and 1 product with name starting with 'P_').")
+
+
+    @staticmethod
+    def simulate(
+            params_opti: list,
+            data_matrix: np.ndarray,
+            time_vector: np.ndarray,
+            params_non_opti: dict
+    ):
+
+        # Get parameters
+        x_0 = params_opti[0]
+        y_BM = params_opti[1]
+        km = params_opti[2]
+        qsmax = params_opti[3]
+        s_0 = params_opti[4]
+        y_P = params_opti[5]
+        p_0 = params_opti[6]
+        params = (y_BM, y_P, km, qsmax)
+
+        # initialize variables at t=0
+        state = [x_0, s_0, p_0]
+        
+        def calculate_derivative(t, state, y_BM, y_P, km, qsmax):
+            
+            # get substrate and biomass concentrations
+            s_t = state[0]
+            x_t = state[1]
+
+            # calculate fluxes
+            qs_t = qsmax * (s_t / (km + s_t))
+            mu_t = y_BM * qs_t
+            qp_t = y_P * qs_t
+
+            # calculate derivatives
+            dx = mu_t * x_t
+            ds = -qs_t * x_t
+            dp = qp_t * x_t
+
+            return dx, ds, dp
+
+        # simulate time-course concentrations
+        sol = solve_ivp(
+            fun=calculate_derivative,
+            t_span=(np.min(time_vector), np.max(time_vector)),
+            y0 = state,
+            args=params,
+            method="LSODA",
+            t_eval = list(time_vector)
+        )
+
+        return sol.y.T
+
+if __name__ == "__main__":
+
+    from physiofit.base.io import IoHandler
+
+    io = IoHandler()
+    data = io.read_data(r"C:\Users\legregam\PycharmProjects\PhysioFit\data\KEIO_test_data\ode_test\KEIO_ROBOT6_1.tsv")
+    data = data.sort_values("time")
+
+    model = ChildModel(data)
+    model.get_params()
+    params = [param for param in model.parameters_to_estimate.values()]
+    sol = ChildModel.simulate(
+        params,
+        model.data,
+        model.time_vector,
+        None
+    )
+    print(f"Times: {sol.t}")
+    print(f"Values: {np.array(sol.y)}")
```

### Comparing `physiofit-3.0.4/physiofit/ui/cli.py` & `physiofit-3.0.6/physiofit/ui/cli.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-"""
-Module containing the Command-Line Interface control logic.
-"""
-import argparse
-import logging
-from pathlib import Path
-import sys
-
-from physiofit.base.io import IoHandler, StandardDevs, ConfigParser
-
-def args_parse():
-    """
-    Parse arguments from user input.
-    :return: Argument Parser object
-    :rtype: class: argparse.ArgumentParser
-    """
-
-    parser = argparse.ArgumentParser(
-        "Physiofit: Extracellular flux estimation software"
-    )
-
-    # Parse data arguments (tsv + json)
-    parser.add_argument(
-        "-d", "--data", type=str,
-        help="Path to data file in tabulated format (txt or tsv)"
-    )
-    parser.add_argument(
-        "-c", "--config", type=str,
-        help="Path to config file in yaml format"
-    )
-    parser.add_argument(
-        "-m", "--model", type=str,
-        help="Which model should be chosen. Useful only if generating related config file"
-    )
-
-    # Parse developer arguments
-    parser.add_argument(
-        "-g", "--galaxy", action="store_true",
-        help="Is the CLI being used on the galaxy platform"
-    )
-    parser.add_argument(
-        "--list", action="store_true",
-        help="Return the list of models in model folder"
-    )
-    parser.add_argument(
-        "-v", "--debug_mode", action="store_true",
-        help="Activate the debug logs"
-    )
-
-    # Parse selective output path arguments (for galaxy implementation mostly)
-    parser.add_argument(
-        "-op", "--output_pdf", type=str,
-        help="Path to output the pdf file containing plots"
-    )
-    parser.add_argument(
-        "-of", "--output_fluxes", type=str,
-        help="Path to output the flux results"
-    )
-    parser.add_argument(
-        "-os", "--output_stats", type=str,
-        help="Path to output the khi² test"
-    )
-    parser.add_argument(
-        "-oc", "--output_config", type=str,
-        help="Path to output the yaml config file"
-    )
-
-    return parser
-
-def run(data, args, logger, exp=None):
-
-    io = IoHandler()
-    logger.info(f"Input Data: \n{io.data}")
-    io.home_path = Path(args.data).parent
-    logger.info(f"Home path: {io.home_path}")
-    logger.info(f"Reading configuration file at {args.config}")
-    io.configparser = io.read_yaml(args.config)
-    logger.info(f"Config File:\n{io.configparser}")
-    model = io.select_model(io.configparser.model["model_name"], data)
-    model.get_params()
-    logger.info(f"Selected Model:\n{model}")
-    model = io.configparser.update_model(model)
-    logger.info(f"Updated Model: \n{model}")
-    logger.info(f"Model Data: \n{model.data}")
-    fitter = io.initialize_fitter(
-        model.data,
-        model=model,
-        mc=io.configparser.mc,
-        iterations=io.configparser.iterations,
-        sd=io.configparser.sds,
-        debug_mode=args.debug_mode
-    )
-    fitter.optimize()
-    if fitter.mc:
-        fitter.monte_carlo_analysis()
-    fitter.khi2_test()
-    if exp is not None:
-        res_path = io.home_path / (io.home_path.name + "_res") / exp
-    else:
-        res_path = io.home_path / (io.home_path.name + "_res")
-    if not res_path.is_dir():
-        res_path.mkdir(parents=True)
-    io.output_report(fitter, res_path)
-    io.output_plots(fitter, res_path)
-    io.output_pdf(fitter, res_path)
-    io.figures = []
-
-def generate_config(args, data, logger):
-
-    logger.info("Launching in configuration file generator mode")
-    # Run checks
-    if args.model is None:
-        # Must be path to model.py file or name of a model
-        raise ValueError(
-            f"Please select a model to generate the associated configuration file"
-        )
-    if args.output_config is None:
-        raise ValueError(
-            "Please select an output directory for the configuration file"
-        )
-    try:
-        io = IoHandler()
-        if Path(args.model).is_file():
-            model_class = io.read_model(args.model)
-            model = model_class(data)
-            model.get_params()
-
-        else:
-            model = io.select_model(args.model, data)
-            model.get_params()
-    except Exception:
-        logger.error("There was an error while initialising the model")
-        raise
-
-    # Build config parser and export configuration file
-    default_sds = StandardDevs({col: 0.2 for col in model.name_vector})
-    configparser = ConfigParser(
-        path_to_data=args.data,
-        selected_model=model,
-        sds=default_sds,
-        mc=True,
-        iterations=100
-    )
-    configparser.export_config(args.output_config)
-    logger.info(f"Finished exporting the configuration file to {args.output_config}")
-    sys.exit()
-
-def process(args):
-
-    logger = logging.getLogger()
-    logger.setLevel(logging.DEBUG)
-    out_stream = logging.StreamHandler()
-    formatter = logging.Formatter()
-    out_stream.setFormatter(formatter)
-    if args.debug_mode:
-        out_stream.setLevel(logging.DEBUG)
-    else:
-        out_stream.setLevel(logging.INFO)
-    logger.addHandler(out_stream)
-
-    if args.list:
-        IoHandler.get_model_list()
-        sys.exit()
-
-    if args.data is None:
-        raise ValueError("A path towards the data must be given")
-
-    # Ensure that the path to data is correct
-    path_to_data = Path(args.data)
-    if not path_to_data.is_file():
-        raise ValueError(
-            f"The data path is not correct. Please check and try again. Input data path: \n{args.data}"
-        )
-    # Ensure that the input file is a tsv
-    if not path_to_data.suffix in [".tsv", ".txt"]:
-        raise TypeError(
-            f"The input data must be in tsv/txt format. Detected format: {path_to_data.suffix}"
-        )
-
-    # Read & check data
-    data = IoHandler.read_data(str(path_to_data))
-
-    # If no configuration file is present we assume the user wants to generate a default one
-    if args.config is None:
-        generate_config(args, data, logger)
-
-    # If configuration file is present we launch the optimization
-    if "experiments" in data.columns:
-        experiments = list(data["experiments"].unique())
-        data = data.set_index("experiments")
-        for exp in experiments:
-            logger.info(f"Running optimization for {exp}")
-            run_data = data.loc[exp, :].sort_values("time").copy()
-            run(run_data, args, logger, exp)
-    else:
-        logger.info("Running optimization")
-        run_data = data.sort_values("time")
-        run(run_data, args, logger)
-    logger.info("Done!")
-    sys.exit()
-
-def main():
-    parser = args_parse()
-    args = parser.parse_args()
-    process(args)
+"""
+Module containing the Command-Line Interface control logic.
+"""
+import argparse
+import logging
+from pathlib import Path
+import sys
+
+from physiofit.base.io import IoHandler, StandardDevs, ConfigParser
+
+def args_parse():
+    """
+    Parse arguments from user input.
+    :return: Argument Parser object
+    :rtype: class: argparse.ArgumentParser
+    """
+
+    parser = argparse.ArgumentParser(
+        "Physiofit: Extracellular flux estimation software"
+    )
+
+    # Parse data arguments (tsv + json)
+    parser.add_argument(
+        "-d", "--data", type=str,
+        help="Path to data file in tabulated format (txt or tsv)"
+    )
+    parser.add_argument(
+        "-c", "--config", type=str,
+        help="Path to config file in yaml format"
+    )
+    parser.add_argument(
+        "-m", "--model", type=str,
+        help="Which model should be chosen. Useful only if generating related config file"
+    )
+
+    # Parse developer arguments
+    parser.add_argument(
+        "-g", "--galaxy", action="store_true",
+        help="Is the CLI being used on the galaxy platform"
+    )
+    parser.add_argument(
+        "--list", action="store_true",
+        help="Return the list of models in model folder"
+    )
+    parser.add_argument(
+        "-v", "--debug_mode", action="store_true",
+        help="Activate the debug logs"
+    )
+
+    # Parse selective output path arguments (for galaxy implementation mostly)
+    parser.add_argument(
+        "-op", "--output_pdf", type=str,
+        help="Path to output the pdf file containing plots"
+    )
+    parser.add_argument(
+        "-of", "--output_fluxes", type=str,
+        help="Path to output the flux results"
+    )
+    parser.add_argument(
+        "-os", "--output_stats", type=str,
+        help="Path to output the khi² test"
+    )
+    parser.add_argument(
+        "-oc", "--output_config", type=str,
+        help="Path to output the yaml config file"
+    )
+
+    return parser
+
+def run(data, args, logger, exp=None):
+
+    io = IoHandler()
+    logger.info(f"Input Data: \n{io.data}")
+    io.home_path = Path(args.data).parent
+    logger.info(f"Home path: {io.home_path}")
+    logger.info(f"Reading configuration file at {args.config}")
+    io.configparser = io.read_yaml(args.config)
+    logger.info(f"Config File:\n{io.configparser}")
+    model = io.select_model(io.configparser.model["model_name"], data)
+    model.get_params()
+    logger.info(f"Selected Model:\n{model}")
+    model = io.configparser.update_model(model)
+    logger.info(f"Updated Model: \n{model}")
+    logger.info(f"Model Data: \n{model.data}")
+    fitter = io.initialize_fitter(
+        model.data,
+        model=model,
+        mc=io.configparser.mc,
+        iterations=io.configparser.iterations,
+        sd=io.configparser.sds,
+        debug_mode=args.debug_mode
+    )
+    fitter.optimize()
+    if fitter.mc:
+        fitter.monte_carlo_analysis()
+    fitter.khi2_test()
+    if exp is not None:
+        res_path = io.home_path / (io.home_path.name + "_res") / exp
+    else:
+        res_path = io.home_path / (io.home_path.name + "_res")
+    if not res_path.is_dir():
+        res_path.mkdir(parents=True)
+    io.output_report(fitter, res_path)
+    io.output_plots(fitter, res_path)
+    io.output_pdf(fitter, res_path)
+    io.figures = []
+
+def generate_config(args, data, logger):
+
+    logger.info("Launching in configuration file generator mode")
+    # Run checks
+    if args.model is None:
+        # Must be path to model.py file or name of a model
+        raise ValueError(
+            f"Please select a model to generate the associated configuration file"
+        )
+    if args.output_config is None:
+        raise ValueError(
+            "Please select an output directory for the configuration file"
+        )
+    try:
+        io = IoHandler()
+        if Path(args.model).is_file():
+            model_class = io.read_model(args.model)
+            model = model_class(data)
+            model.get_params()
+
+        else:
+            model = io.select_model(args.model, data)
+            model.get_params()
+    except Exception:
+        logger.error("There was an error while initialising the model")
+        raise
+
+    # Build config parser and export configuration file
+    default_sds = StandardDevs({col: 0.2 for col in model.name_vector})
+    configparser = ConfigParser(
+        path_to_data=args.data,
+        selected_model=model,
+        sds=default_sds,
+        mc=True,
+        iterations=100
+    )
+    configparser.export_config(args.output_config)
+    logger.info(f"Finished exporting the configuration file to {args.output_config}")
+    sys.exit()
+
+def process(args):
+
+    logger = logging.getLogger()
+    logger.setLevel(logging.DEBUG)
+    out_stream = logging.StreamHandler()
+    formatter = logging.Formatter()
+    out_stream.setFormatter(formatter)
+    if args.debug_mode:
+        out_stream.setLevel(logging.DEBUG)
+    else:
+        out_stream.setLevel(logging.INFO)
+    logger.addHandler(out_stream)
+
+    if args.list:
+        IoHandler.get_model_list()
+        sys.exit()
+
+    if args.data is None:
+        raise ValueError("A path towards the data must be given")
+
+    # Ensure that the path to data is correct
+    path_to_data = Path(args.data)
+    if not path_to_data.is_file():
+        raise ValueError(
+            f"The data path is not correct. Please check and try again. Input data path: \n{args.data}"
+        )
+    # Ensure that the input file is a tsv
+    if not path_to_data.suffix in [".tsv", ".txt"]:
+        raise TypeError(
+            f"The input data must be in tsv/txt format. Detected format: {path_to_data.suffix}"
+        )
+
+    # Read & check data
+    data = IoHandler.read_data(str(path_to_data))
+
+    # If no configuration file is present we assume the user wants to generate a default one
+    if args.config is None:
+        generate_config(args, data, logger)
+
+    # If configuration file is present we launch the optimization
+    if "experiments" in data.columns:
+        experiments = list(data["experiments"].unique())
+        data = data.set_index("experiments")
+        for exp in experiments:
+            logger.info(f"Running optimization for {exp}")
+            run_data = data.loc[exp, :].sort_values("time").copy()
+            run(run_data, args, logger, exp)
+    else:
+        logger.info("Running optimization")
+        run_data = data.sort_values("time")
+        run(run_data, args, logger)
+    logger.info("Done!")
+    sys.exit()
+
+def main():
+    parser = args_parse()
+    args = parser.parse_args()
+    process(args)
```

### Comparing `physiofit-3.0.4/pyproject.toml` & `physiofit-3.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-[tool.poetry]
-name = "physiofit"
-version = "3.0.4"
-description = "Calculate extracellular fluxes from metabolite concentrations and biomass data"
-authors = ["llegregam <legregam@insa-toulouse.fr>"]
-license = "GNU General Public License (GPL)"
-readme = "README.md"
-
-[tool.poetry.scripts]
-physiofit = 'physiofit.__main__:main'
-
-[tool.poetry.dependencies]
-python = ">=3.8,<3.9.7 || >3.9.7,<3.12"
-pandas = "^1.5.3"
-numpy = "^1.24.2"
-scipy = "^1.10.1"
-streamlit = "^1.20.0"
-matplotlib = "^3.7.1"
-openpyxl = "^3.1.2"
-pyyaml = "^6.0"
-
-[tool.poetry.group.dev.dependencies]
-ipykernel = "^6.21.3"
-nbsphinx = "^0.9.1"
-pandoc = "^2.3"
-Sphinx = "^6.1.3"
-sphinx-argparse = "^0.4.0"
-sphinx-rtd-theme = "^1.2.0"
-
-
-[tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "physiofit"
+version = "3.0.6"
+description = "Calculate extracellular fluxes from metabolite concentrations and biomass data"
+authors = ["llegregam <legregam@insa-toulouse.fr>"]
+license = "GNU General Public License (GPL)"
+readme = "README.md"
+
+[tool.poetry.scripts]
+physiofit = 'physiofit.__main__:main'
+
+[tool.poetry.dependencies]
+python = ">=3.8,<3.9.7 || >3.9.7,<3.12"
+pandas = "^2.0.1"
+numpy = "^1.24.2"
+scipy = "^1.10.1"
+streamlit = "^1.20.0"
+matplotlib = "^3.7.1"
+openpyxl = "^3.1.2"
+pyyaml = "^6.0"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.21.3"
+nbsphinx = "^0.9.1"
+pandoc = "^2.3"
+Sphinx = "^6.1.3"
+sphinx-argparse = "^0.4.0"
+sphinx-rtd-theme = "^1.2.0"
+
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.3.1"
+tox = "^4.5.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `physiofit-3.0.4/README.md` & `physiofit-3.0.6/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# PhysioFit
-
-[![PyPI version](https://badge.fury.io/py/physiofit.svg)](https://badge.fury.io/py/physiofit)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/physiofit.svg)](https://pypi.python.org/pypi/physiofit/)
-[![Documentation Status](https://readthedocs.org/projects/physiofit/badge/?version=latest)](http://physiofit.readthedocs.io/?badge=latest)
-
-
-## What is PhysioFit?
-**PhysioFit is a scientific tool designed to quantify cell growth parameters and uptake & production fluxes**
-
-Fluxes are estimated using various mathematical models by fitting time-course measurements of the concentration of
-cells and extracellular substrates and products. PhysioFit v3 includes by default the most common growth models, and
-additional models can be implemented by users.
-
-It is one of the routine tools that we use at the [MetaSys team](http://www.lisbp.fr/en/research/molecular-physiology-and-metabolism/metasys.html) 
-and [MetaToul platform](http://www.metatoul.fr) in functional studies of metabolic systems.
-
-The code is open-source, and available under a GPLv3 license. Additional information can be found in the following 
-[publication](https://doi.org/10.1128/aem.00768-19).
-
-Detailed documentation can be found online at Read the Docs 
-([https://physiofit.readthedocs.io/](https://physiofit.readthedocs.io/)).
-
-## Key features
-   * **calculation of growth rate and extracellular (uptake and production) fluxes**,
-   * default models for quantifying parameters in steady-state conditions (with and without lag & metabolite degradation
-     over time),
-   * **user-defined growth models**,
-   * Monte-Carlo sensitivity analysis to **estimate the precision of the calculated fluxes**,
-   * **evaluation of the goodness of fit and visual inspection of the fitted curves**,
-   * shipped as a **library** with both a **graphical** and **command line** interface,
-   * open-source, free and easy to install everywhere where Python 3 and pip run,
-   * **biologist-friendly**.
-
-## Quick-start
-PhysioFit requires Python 3.7 or higher and run on all platforms.
-Please check [the documentation](https://physiofit.readthedocs.io/en/latest/quickstart.html) for complete
-installation and usage instructions.
-
-Use `pip` to **install PhysioFit from PyPi**:
-
-```bash
-$ pip install physiofit
-```
-
-Then, start the graphical interface with:
-
-```bash
-$ physiofit
-```
-
-PhysioFit is also available directly from command-line and as a Python library.
-
-## Bug and feature requests
-If you have an idea on how we could improve PhysioFit please submit a new *issue*
-to [our GitHub issue tracker](https://github.com/MetaSys-LISBP/PhysioFit/issues).
-
-
-## Developers guide
-### Contributions
-Contributions are very welcome! :heart:
-
-Please work on your own fork,
-follow [PEP8](https://www.python.org/dev/peps/pep-0008/) style guide,
-and make sure you pass all the tests before a pull request.
-
-### Local install with pip
-In development mode, do a `pip install -e /path/to/PhysioFit` to install
-locally the development version.
-
-### Build the documentation locally
-Build the HTML documentation with:
-
-```bash
-$ cd doc
-$ make html
-```
-
-The PDF documentation can be built locally by replacing `html` by `latexpdf`
-in the command above. You will need a recent latex installation.
-
-## How to cite
-PhysioFit: quantifying cell growth parameters and uptake and production fluxes.
-Le Grégam L., Guitton Y., Bellvert F., Jourdan F., Portais J.C., Millard P.
-In preparation for publication
-
-## Authors
-Loïc Le Grégam, Pierre Millard
-
-## Contact
-:email: legregam@insa-toulouse.fr, millard@insa-toulouse.fr
+# PhysioFit
+
+[![PyPI version](https://badge.fury.io/py/physiofit.svg)](https://badge.fury.io/py/physiofit)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/physiofit.svg)](https://pypi.python.org/pypi/physiofit/)
+[![Documentation Status](https://readthedocs.org/projects/physiofit/badge/?version=latest)](http://physiofit.readthedocs.io/?badge=latest)
+
+
+## What is PhysioFit?
+**PhysioFit is a scientific tool designed to quantify cell growth parameters and uptake & production fluxes**
+
+Fluxes are estimated using various mathematical models by fitting time-course measurements of the concentration of
+cells and extracellular substrates and products. PhysioFit v3 includes by default the most common growth models, and
+additional models can be implemented by users.
+
+It is one of the routine tools that we use at the [MetaSys team](http://www.lisbp.fr/en/research/molecular-physiology-and-metabolism/metasys.html) 
+and [MetaToul platform](http://www.metatoul.fr) in functional studies of metabolic systems.
+
+The code is open-source, and available under a GPLv3 license. Additional information can be found in the following 
+[publication](https://doi.org/10.1128/aem.00768-19).
+
+Detailed documentation can be found online at Read the Docs 
+([https://physiofit.readthedocs.io/](https://physiofit.readthedocs.io/)).
+
+## Key features
+   * **calculation of growth rate and extracellular (uptake and production) fluxes**,
+   * default models for quantifying parameters in steady-state conditions (with and without lag & metabolite degradation
+     over time),
+   * **user-defined growth models**,
+   * Monte-Carlo sensitivity analysis to **estimate the precision of the calculated fluxes**,
+   * **evaluation of the goodness of fit and visual inspection of the fitted curves**,
+   * shipped as a **library** with both a **graphical** and **command line** interface,
+   * open-source, free and easy to install everywhere where Python 3 and pip run,
+   * **biologist-friendly**.
+
+## Quick-start
+PhysioFit requires Python 3.7 or higher and run on all platforms.
+Please check [the documentation](https://physiofit.readthedocs.io/en/latest/quickstart.html) for complete
+installation and usage instructions.
+
+Use `pip` to **install PhysioFit from PyPi**:
+
+```bash
+$ pip install physiofit
+```
+
+Then, start the graphical interface with:
+
+```bash
+$ physiofit
+```
+
+PhysioFit is also available directly from command-line and as a Python library.
+
+## Bug and feature requests
+If you have an idea on how we could improve PhysioFit please submit a new *issue*
+to [our GitHub issue tracker](https://github.com/MetaSys-LISBP/PhysioFit/issues).
+
+
+## Developers guide
+### Contributions
+Contributions are very welcome! :heart:
+
+Please work on your own fork,
+follow [PEP8](https://www.python.org/dev/peps/pep-0008/) style guide,
+and make sure you pass all the tests before a pull request.
+
+### Local install with pip
+In development mode, do a `pip install -e /path/to/PhysioFit` to install
+locally the development version.
+
+### Build the documentation locally
+Build the HTML documentation with:
+
+```bash
+$ cd doc
+$ make html
+```
+
+The PDF documentation can be built locally by replacing `html` by `latexpdf`
+in the command above. You will need a recent latex installation.
+
+## How to cite
+PhysioFit: quantifying cell growth parameters and uptake and production fluxes.
+Le Grégam L., Guitton Y., Bellvert F., Jourdan F., Portais J.C., Millard P.
+In preparation for publication
+
+## Authors
+Loïc Le Grégam, Pierre Millard
+
+## Contact
+:email: legregam@insa-toulouse.fr, millard@insa-toulouse.fr
```

### Comparing `physiofit-3.0.4/PKG-INFO` & `physiofit-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: physiofit
-Version: 3.0.4
+Version: 3.0.6
 Summary: Calculate extracellular fluxes from metabolite concentrations and biomass data
 License: GNU General Public License (GPL)
 Author: llegregam
 Author-email: legregam@insa-toulouse.fr
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: streamlit (>=1.20.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PhysioFit
```

