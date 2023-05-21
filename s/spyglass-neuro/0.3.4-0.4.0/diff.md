# Comparing `tmp/spyglass-neuro-0.3.4.tar.gz` & `tmp/spyglass-neuro-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyglass-neuro-0.3.4.tar", last modified: Fri Mar 31 00:10:43 2023, max compression
+gzip compressed data, was "spyglass-neuro-0.4.0.tar", last modified: Sun May 21 23:36:54 2023, max compression
```

## Comparing `spyglass-neuro-0.3.4.tar` & `spyglass-neuro-0.4.0.tar`

### file list

```diff
@@ -1,100 +1,122 @@
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.799068 spyglass-neuro-0.3.4/
--rw-r--r--   0 rly        (502) staff       (20)     1063 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/LICENSE
--rw-r--r--   0 rly        (502) staff       (20)       36 2022-09-22 00:46:32.000000 spyglass-neuro-0.3.4/MANIFEST.in
--rw-r--r--   0 rly        (502) staff       (20)     4874 2023-03-31 00:10:43.799197 spyglass-neuro-0.3.4/PKG-INFO
--rw-r--r--   0 rly        (502) staff       (20)     2944 2023-03-24 22:11:57.000000 spyglass-neuro-0.3.4/README.md
--rw-r--r--   0 rly        (502) staff       (20)     1666 2023-03-31 00:10:33.000000 spyglass-neuro-0.3.4/pyproject.toml
--rw-r--r--   0 rly        (502) staff       (20)      346 2023-03-31 00:10:43.799541 spyglass-neuro-0.3.4/setup.cfg
--rw-r--r--   0 rly        (502) staff       (20)       53 2022-12-17 01:24:50.000000 spyglass-neuro-0.3.4/setup.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.787336 spyglass-neuro-0.3.4/src/
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.788775 spyglass-neuro-0.3.4/src/spyglass/
--rw-r--r--   0 rly        (502) staff       (20)      349 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/__init__.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.789051 spyglass-neuro-0.3.4/src/spyglass/cli/
--rw-r--r--   0 rly        (502) staff       (20)       21 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/cli/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)    14367 2023-03-24 22:23:13.000000 spyglass-neuro-0.3.4/src/spyglass/cli/cli.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.791760 spyglass-neuro-0.3.4/src/spyglass/common/
--rw-r--r--   0 rly        (502) staff       (20)     1878 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     1381 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_backup.py
--rw-r--r--   0 rly        (502) staff       (20)     9546 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_behav.py
--rw-r--r--   0 rly        (502) staff       (20)    28298 2023-03-31 00:06:22.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_device.py
--rw-r--r--   0 rly        (502) staff       (20)     1733 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_dio.py
--rw-r--r--   0 rly        (502) staff       (20)    33832 2023-03-29 20:25:30.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_ephys.py
--rw-r--r--   0 rly        (502) staff       (20)    19206 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_filter.py
--rw-r--r--   0 rly        (502) staff       (20)    16785 2023-03-24 22:23:13.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_interval.py
--rw-r--r--   0 rly        (502) staff       (20)     5023 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_lab.py
--rw-r--r--   0 rly        (502) staff       (20)    23631 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_nwbfile.py
--rw-r--r--   0 rly        (502) staff       (20)    34091 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_position.py
--rw-r--r--   0 rly        (502) staff       (20)     1645 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_region.py
--rw-r--r--   0 rly        (502) staff       (20)    11600 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_ripple.py
--rw-r--r--   0 rly        (502) staff       (20)     1513 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_sensors.py
--rw-r--r--   0 rly        (502) staff       (20)     8934 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_session.py
--rw-r--r--   0 rly        (502) staff       (20)     1151 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_subject.py
--rw-r--r--   0 rly        (502) staff       (20)     6795 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/common_task.py
--rw-r--r--   0 rly        (502) staff       (20)       45 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/errors.py
--rw-r--r--   0 rly        (502) staff       (20)     1582 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/populate_all_common.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.792014 spyglass-neuro-0.3.4/src/spyglass/common/prepopulate/
--rw-r--r--   0 rly        (502) staff       (20)       65 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/prepopulate/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     3427 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/common/prepopulate/prepopulate.py
--rw-r--r--   0 rly        (502) staff       (20)     1544 2023-03-24 22:23:13.000000 spyglass-neuro-0.3.4/src/spyglass/common/signal_processing.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.792373 spyglass-neuro-0.3.4/src/spyglass/data_import/
--rw-r--r--   0 rly        (502) staff       (20)       91 2022-09-02 00:03:53.000000 spyglass-neuro-0.3.4/src/spyglass/data_import/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     4077 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/data_import/insert_sessions.py
--rw-r--r--   0 rly        (502) staff       (20)      449 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/data_import/storage_dirs.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.793388 spyglass-neuro-0.3.4/src/spyglass/decoding/
--rw-r--r--   0 rly        (502) staff       (20)      699 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)    27782 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/clusterless.py
--rw-r--r--   0 rly        (502) staff       (20)     2204 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/core.py
--rw-r--r--   0 rly        (502) staff       (20)     5046 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/dj_decoder_conversion.py
--rw-r--r--   0 rly        (502) staff       (20)     9364 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/sorted_spikes.py
--rw-r--r--   0 rly        (502) staff       (20)    19719 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/visualization.py
--rw-r--r--   0 rly        (502) staff       (20)     2871 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/visualization_1D_view.py
--rw-r--r--   0 rly        (502) staff       (20)    11247 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/decoding/visualization_2D_view.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.793891 spyglass-neuro-0.3.4/src/spyglass/figurl_views/
--rw-r--r--   0 rly        (502) staff       (20)     3315 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/figurl_views/SpikeSortingRecordingView.py
--rw-r--r--   0 rly        (502) staff       (20)     3353 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/figurl_views/SpikeSortingView.py
--rw-r--r--   0 rly        (502) staff       (20)      112 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/figurl_views/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)    10908 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/figurl_views/prepare_spikesortingview_data.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.794141 spyglass-neuro-0.3.4/src/spyglass/lock/
--rw-r--r--   0 rly        (502) staff       (20)       56 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/src/spyglass/lock/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     1365 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/lock/file_lock.py
--rw-r--r--   0 rly        (502) staff       (20)       31 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/settings.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.794392 spyglass-neuro-0.3.4/src/spyglass/sharing/
--rw-r--r--   0 rly        (502) staff       (20)      172 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/src/spyglass/sharing/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     9561 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/sharing/sharing_kachery.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.795555 spyglass-neuro-0.3.4/src/spyglass/spikesorting/
--rw-r--r--   0 rly        (502) staff       (20)      948 2022-12-21 21:51:14.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     7321 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/curation_figurl.py
--rw-r--r--   0 rly        (502) staff       (20)     4439 2023-03-24 22:19:44.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/merged_sorting_extractor.py
--rw-r--r--   0 rly        (502) staff       (20)     7386 2023-03-25 01:09:21.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/sortingview.py
--rw-r--r--   0 rly        (502) staff       (20)     5497 2023-03-25 01:09:21.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/sortingview_helper_fn.py
--rw-r--r--   0 rly        (502) staff       (20)    13894 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_artifact.py
--rw-r--r--   0 rly        (502) staff       (20)    37451 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_curation.py
--rw-r--r--   0 rly        (502) staff       (20)    22510 2023-03-31 00:06:22.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_recording.py
--rw-r--r--   0 rly        (502) staff       (20)    10938 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_sorting.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.795915 spyglass-neuro-0.3.4/src/spyglass/utils/
--rw-r--r--   0 rly        (502) staff       (20)        0 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/utils/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     4626 2023-03-25 07:31:17.000000 spyglass-neuro-0.3.4/src/spyglass/utils/dj_helper_fn.py
--rw-r--r--   0 rly        (502) staff       (20)    14272 2023-03-25 00:30:17.000000 spyglass-neuro-0.3.4/src/spyglass/utils/nwb_helper_fn.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.796631 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/
--rw-r--r--   0 rly        (502) staff       (20)     4874 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/PKG-INFO
--rw-r--r--   0 rly        (502) staff       (20)     2887 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/SOURCES.txt
--rw-r--r--   0 rly        (502) staff       (20)        1 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/dependency_links.txt
--rw-r--r--   0 rly        (502) staff       (20)       50 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/entry_points.txt
--rw-r--r--   0 rly        (502) staff       (20)      318 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/requires.txt
--rw-r--r--   0 rly        (502) staff       (20)        9 2023-03-31 00:10:43.000000 spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/top_level.txt
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.797737 spyglass-neuro-0.3.4/tests/
--rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/tests/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)      613 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/tests/ci_config.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.797882 spyglass-neuro-0.3.4/tests/common/
--rw-r--r--   0 rly        (502) staff       (20)      698 2022-10-26 19:03:18.000000 spyglass-neuro-0.3.4/tests/common/test_common_interval.py
--rw-r--r--   0 rly        (502) staff       (20)     3118 2023-03-24 22:07:26.000000 spyglass-neuro-0.3.4/tests/conftest.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.798167 spyglass-neuro-0.3.4/tests/data_import/
--rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/tests/data_import/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)     3255 2023-03-24 22:07:26.000000 spyglass-neuro-0.3.4/tests/data_import/test_insert_sessions.py
-drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-03-31 00:10:43.798833 spyglass-neuro-0.3.4/tests/datajoint/
--rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/tests/datajoint/__init__.py
--rw-r--r--   0 rly        (502) staff       (20)       29 2022-08-25 18:48:05.000000 spyglass-neuro-0.3.4/tests/datajoint/_config.py
--rw-r--r--   0 rly        (502) staff       (20)     2720 2023-03-24 22:11:57.000000 spyglass-neuro-0.3.4/tests/datajoint/_datajoint_server.py
--rw-r--r--   0 rly        (502) staff       (20)     3208 2023-03-25 00:00:17.000000 spyglass-neuro-0.3.4/tests/test_insert_beans.py
--rw-r--r--   0 rly        (502) staff       (20)     1816 2023-03-25 00:00:26.000000 spyglass-neuro-0.3.4/tests/test_nwb_helper_fn.py
--rw-r--r--   0 rly        (502) staff       (20)     2679 2023-03-24 22:07:26.000000 spyglass-neuro-0.3.4/tests/trim_beans.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.811668 spyglass-neuro-0.4.0/
+-rw-r--r--   0 rly        (502) staff       (20)     1063 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/LICENSE
+-rw-r--r--   0 rly        (502) staff       (20)       36 2022-09-22 00:46:32.000000 spyglass-neuro-0.4.0/MANIFEST.in
+-rw-r--r--   0 rly        (502) staff       (20)     4087 2023-05-21 23:36:54.811768 spyglass-neuro-0.4.0/PKG-INFO
+-rw-r--r--   0 rly        (502) staff       (20)     2088 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/README.md
+-rw-r--r--   0 rly        (502) staff       (20)     1952 2023-05-21 23:36:13.000000 spyglass-neuro-0.4.0/pyproject.toml
+-rw-r--r--   0 rly        (502) staff       (20)      346 2023-05-21 23:36:54.812029 spyglass-neuro-0.4.0/setup.cfg
+-rw-r--r--   0 rly        (502) staff       (20)       53 2022-12-17 01:24:50.000000 spyglass-neuro-0.4.0/setup.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.794948 spyglass-neuro-0.4.0/src/
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.796464 spyglass-neuro-0.4.0/src/spyglass/
+-rw-r--r--   0 rly        (502) staff       (20)      349 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/__init__.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.796799 spyglass-neuro-0.4.0/src/spyglass/cli/
+-rw-r--r--   0 rly        (502) staff       (20)       21 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/cli/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)    14366 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/cli/cli.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.800409 spyglass-neuro-0.4.0/src/spyglass/common/
+-rw-r--r--   0 rly        (502) staff       (20)     1888 2023-05-21 23:08:29.000000 spyglass-neuro-0.4.0/src/spyglass/common/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     1381 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_backup.py
+-rw-r--r--   0 rly        (502) staff       (20)     9546 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_behav.py
+-rw-r--r--   0 rly        (502) staff       (20)    28298 2023-03-31 00:06:22.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_device.py
+-rw-r--r--   0 rly        (502) staff       (20)     3939 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_dio.py
+-rw-r--r--   0 rly        (502) staff       (20)    33942 2023-05-21 23:08:29.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_ephys.py
+-rw-r--r--   0 rly        (502) staff       (20)    19601 2023-05-21 23:08:29.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_filter.py
+-rw-r--r--   0 rly        (502) staff       (20)    17798 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_interval.py
+-rw-r--r--   0 rly        (502) staff       (20)     5022 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_lab.py
+-rw-r--r--   0 rly        (502) staff       (20)    23632 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_nwbfile.py
+-rw-r--r--   0 rly        (502) staff       (20)    34090 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_position.py
+-rw-r--r--   0 rly        (502) staff       (20)     1645 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_region.py
+-rw-r--r--   0 rly        (502) staff       (20)    11556 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_ripple.py
+-rw-r--r--   0 rly        (502) staff       (20)     1513 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_sensors.py
+-rw-r--r--   0 rly        (502) staff       (20)     8934 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_session.py
+-rw-r--r--   0 rly        (502) staff       (20)     1151 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_subject.py
+-rw-r--r--   0 rly        (502) staff       (20)     6795 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/common_task.py
+-rw-r--r--   0 rly        (502) staff       (20)       45 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/errors.py
+-rw-r--r--   0 rly        (502) staff       (20)     1582 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/populate_all_common.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.800726 spyglass-neuro-0.4.0/src/spyglass/common/prepopulate/
+-rw-r--r--   0 rly        (502) staff       (20)       65 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/prepopulate/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     3427 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/common/prepopulate/prepopulate.py
+-rw-r--r--   0 rly        (502) staff       (20)     1544 2023-03-24 22:23:13.000000 spyglass-neuro-0.4.0/src/spyglass/common/signal_processing.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.801173 spyglass-neuro-0.4.0/src/spyglass/data_import/
+-rw-r--r--   0 rly        (502) staff       (20)       91 2022-09-02 00:03:53.000000 spyglass-neuro-0.4.0/src/spyglass/data_import/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     4077 2023-03-24 22:19:44.000000 spyglass-neuro-0.4.0/src/spyglass/data_import/insert_sessions.py
+-rw-r--r--   0 rly        (502) staff       (20)      449 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/data_import/storage_dirs.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.802609 spyglass-neuro-0.4.0/src/spyglass/decoding/
+-rw-r--r--   0 rly        (502) staff       (20)      699 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)    28409 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/clusterless.py
+-rw-r--r--   0 rly        (502) staff       (20)     5337 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/core.py
+-rw-r--r--   0 rly        (502) staff       (20)     6142 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/dj_decoder_conversion.py
+-rw-r--r--   0 rly        (502) staff       (20)    13510 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/sorted_spikes.py
+-rw-r--r--   0 rly        (502) staff       (20)    19941 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/visualization.py
+-rw-r--r--   0 rly        (502) staff       (20)     2879 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/visualization_1D_view.py
+-rw-r--r--   0 rly        (502) staff       (20)    11494 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/decoding/visualization_2D_view.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.803234 spyglass-neuro-0.4.0/src/spyglass/figurl_views/
+-rw-r--r--   0 rly        (502) staff       (20)     3315 2023-03-24 22:19:44.000000 spyglass-neuro-0.4.0/src/spyglass/figurl_views/SpikeSortingRecordingView.py
+-rw-r--r--   0 rly        (502) staff       (20)     3352 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/figurl_views/SpikeSortingView.py
+-rw-r--r--   0 rly        (502) staff       (20)      112 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/figurl_views/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)    10908 2023-03-24 22:19:44.000000 spyglass-neuro-0.4.0/src/spyglass/figurl_views/prepare_spikesortingview_data.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.794228 spyglass-neuro-0.4.0/src/spyglass/lfp/
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.803531 spyglass-neuro-0.4.0/src/spyglass/lfp/v1/
+-rw-r--r--   0 rly        (502) staff       (20)      286 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/lfp/v1/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)    36395 2023-05-21 23:08:29.000000 spyglass-neuro-0.4.0/src/spyglass/lfp/v1/lfp.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.803844 spyglass-neuro-0.4.0/src/spyglass/lock/
+-rw-r--r--   0 rly        (502) staff       (20)       56 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/src/spyglass/lock/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     1365 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/src/spyglass/lock/file_lock.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.804120 spyglass-neuro-0.4.0/src/spyglass/position/
+-rw-r--r--   0 rly        (502) staff       (20)       43 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)    15373 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/position_merge.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.807195 spyglass-neuro-0.4.0/src/spyglass/position/v1/
+-rw-r--r--   0 rly        (502) staff       (20)     1690 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)      782 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/dlc_decorators.py
+-rw-r--r--   0 rly        (502) staff       (20)     8929 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/dlc_reader.py
+-rw-r--r--   0 rly        (502) staff       (20)    41737 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/dlc_utils.py
+-rw-r--r--   0 rly        (502) staff       (20)    32834 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_centroid.py
+-rw-r--r--   0 rly        (502) staff       (20)     3182 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_cohort.py
+-rw-r--r--   0 rly        (502) staff       (20)    11813 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_model.py
+-rw-r--r--   0 rly        (502) staff       (20)     8823 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_orient.py
+-rw-r--r--   0 rly        (502) staff       (20)    11116 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_pose_estimation.py
+-rw-r--r--   0 rly        (502) staff       (20)    16122 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_position.py
+-rw-r--r--   0 rly        (502) staff       (20)    18981 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_project.py
+-rw-r--r--   0 rly        (502) staff       (20)    15801 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_selection.py
+-rw-r--r--   0 rly        (502) staff       (20)     9144 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_dlc_training.py
+-rw-r--r--   0 rly        (502) staff       (20)    21207 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/position/v1/position_trodes_position.py
+-rw-r--r--   0 rly        (502) staff       (20)       31 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/settings.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.807501 spyglass-neuro-0.4.0/src/spyglass/sharing/
+-rw-r--r--   0 rly        (502) staff       (20)      115 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/sharing/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     6942 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/sharing/sharing_kachery.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.808869 spyglass-neuro-0.4.0/src/spyglass/spikesorting/
+-rw-r--r--   0 rly        (502) staff       (20)      948 2022-12-21 21:51:14.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     7320 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/curation_figurl.py
+-rw-r--r--   0 rly        (502) staff       (20)     4439 2023-03-24 22:19:44.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/merged_sorting_extractor.py
+-rw-r--r--   0 rly        (502) staff       (20)     7386 2023-03-25 01:09:21.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/sortingview.py
+-rw-r--r--   0 rly        (502) staff       (20)     5496 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/sortingview_helper_fn.py
+-rw-r--r--   0 rly        (502) staff       (20)    14457 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_artifact.py
+-rw-r--r--   0 rly        (502) staff       (20)    37511 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_curation.py
+-rw-r--r--   0 rly        (502) staff       (20)    22509 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_recording.py
+-rw-r--r--   0 rly        (502) staff       (20)    11376 2023-05-20 06:44:06.000000 spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_sorting.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.809307 spyglass-neuro-0.4.0/src/spyglass/utils/
+-rw-r--r--   0 rly        (502) staff       (20)        0 2023-03-25 00:30:17.000000 spyglass-neuro-0.4.0/src/spyglass/utils/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     4626 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/utils/dj_helper_fn.py
+-rw-r--r--   0 rly        (502) staff       (20)    14097 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/src/spyglass/utils/nwb_helper_fn.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.810108 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/
+-rw-r--r--   0 rly        (502) staff       (20)     4087 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/PKG-INFO
+-rw-r--r--   0 rly        (502) staff       (20)     3680 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/SOURCES.txt
+-rw-r--r--   0 rly        (502) staff       (20)        1 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/dependency_links.txt
+-rw-r--r--   0 rly        (502) staff       (20)       50 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/entry_points.txt
+-rw-r--r--   0 rly        (502) staff       (20)      377 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/requires.txt
+-rw-r--r--   0 rly        (502) staff       (20)        9 2023-05-21 23:36:54.000000 spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/top_level.txt
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.810843 spyglass-neuro-0.4.0/tests/
+-rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/tests/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)      613 2022-10-26 19:03:18.000000 spyglass-neuro-0.4.0/tests/ci_config.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.810966 spyglass-neuro-0.4.0/tests/common/
+-rw-r--r--   0 rly        (502) staff       (20)     2112 2023-05-11 01:29:18.000000 spyglass-neuro-0.4.0/tests/common/test_common_interval.py
+-rw-r--r--   0 rly        (502) staff       (20)     3118 2023-03-24 22:07:26.000000 spyglass-neuro-0.4.0/tests/conftest.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.811192 spyglass-neuro-0.4.0/tests/data_import/
+-rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/tests/data_import/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)     3255 2023-03-24 22:07:26.000000 spyglass-neuro-0.4.0/tests/data_import/test_insert_sessions.py
+drwxr-xr-x   0 rly        (502) staff       (20)        0 2023-05-21 23:36:54.811549 spyglass-neuro-0.4.0/tests/datajoint/
+-rw-r--r--   0 rly        (502) staff       (20)        0 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/tests/datajoint/__init__.py
+-rw-r--r--   0 rly        (502) staff       (20)       29 2022-08-25 18:48:05.000000 spyglass-neuro-0.4.0/tests/datajoint/_config.py
+-rw-r--r--   0 rly        (502) staff       (20)     2720 2023-03-24 22:11:57.000000 spyglass-neuro-0.4.0/tests/datajoint/_datajoint_server.py
+-rw-r--r--   0 rly        (502) staff       (20)     3208 2023-03-25 00:00:17.000000 spyglass-neuro-0.4.0/tests/test_insert_beans.py
+-rw-r--r--   0 rly        (502) staff       (20)     1816 2023-03-25 00:00:26.000000 spyglass-neuro-0.4.0/tests/test_nwb_helper_fn.py
+-rw-r--r--   0 rly        (502) staff       (20)     2679 2023-03-24 22:07:26.000000 spyglass-neuro-0.4.0/tests/trim_beans.py
```

### Comparing `spyglass-neuro-0.3.4/LICENSE` & `spyglass-neuro-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/PKG-INFO` & `spyglass-neuro-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spyglass-neuro
-Version: 0.3.4
+Version: 0.4.0
 Summary: Neuroscience data analysis framework for reproducible research
-Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>
+Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>, Daniel Gramling <daniel.gramling@ucsf.edu>
 License: Copyright (c) 2020-present Loren Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -15,64 +15,28 @@
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/spyglass/issues
 Keywords: neuroscience,research,electrophysiology,reproducible,data analysis,spike sorting,spikeinterface,datajoint,nwb,kachery,sortingview
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: position
 License-File: LICENSE
 
 [![Import test](https://github.com/LorenFrankLab/spyglass/actions/workflows/workflow.yml/badge.svg)](https://github.com/LorenFrankLab/spyglass/actions/workflows/workflow.yml)
 
 # spyglass
 
 `spyglass` is a data analysis framework that facilitates the storage, analysis, visualization, and sharing of neuroscience data to support reproducible research. It is designed to be interoperable with the NWB format and integrates open-source tools into a coherent framework.
 
 Documentation can be found at - [https://lorenfranklab.github.io/spyglass/](https://lorenfranklab.github.io/spyglass/)
 
-### Installing from pip
+## Installation
 
-Install spyglass
-
-```bash
-pip install spyglass-neuro
-```
-
-Some functions may take advantage of the latest changes to spike interface, which currently has a slow release cycle. To get the latest changes:
-
-```bash
-pip install git+https://github.com/SpikeInterface/spikeinterface.git
-```
-
-The Frank Lab typically uses mountainsort, although spyglass uses spikeinterface, which allows for any spike sorter. To install mountainsort:
-
-```bash
-pip install mountainsort4
-```
-
-Spyglass uses the package `ghostipy` for filtering of signals:
-
-```bash
-pip install ghostipy
-```
-
-WARNING: If you are on an M1 Mac, you need to install pyfftw via conda BEFORE installing ghostipy
-
-```bash
-conda install -c conda-forge pyfftw
-```
-
-Finally, if you want to decode on the GPU, you must install cupy:
-```bash
-conda install -c conda-forge cupy
-```
-
-## Setup
-
-See the documentation for setup instructions - [https://lorenfranklab.github.io/spyglass/type/html/installation.html](https://lorenfranklab.github.io/spyglass/type/html/installation.html)
+For installation instructions see - [https://lorenfranklab.github.io/spyglass/type/html/installation.html](https://lorenfranklab.github.io/spyglass/type/html/installation.html)
 
 ## Tutorials
 
 The tutorials for `spyglass` is currently in the form of Jupyter Notebooks and can be found in the [notebooks](https://github.com/LorenFrankLab/spyglass/tree/master/notebooks) directory. We strongly recommend opening them in the context of `jupyterlab`.
 
 ## Contributing
```

### Comparing `spyglass-neuro-0.3.4/pyproject.toml` & `spyglass-neuro-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyglass-neuro"
-version = "0.3.4"
+version = "0.4.0"
 authors = [
     { name = "Loren Frank", email = "loren.frank@ucsf.edu" },
     { name = "Kyu Hyun Lee", email = "kyuhyun.lee@ucsf.edu" },
     { name = "Eric Denovellis", email = "eric.denovellis@ucsf.edu" },
     { name = "Ryan Ly", email = "rly@lbl.gov" },
+    { name = "Daniel Gramling", email = "daniel.gramling@ucsf.edu" },
 ]
 description = "Neuroscience data analysis framework for reproducible research"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8,<3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -41,14 +42,15 @@
     "replay_trajectory_classification",
     "ripple_detection",
     "trajectory_analysis_tools",
     "matplotlib",
     "seaborn",
     "skan",
     "bottleneck",
+    "numpy<1.24",
     "ipympl",
     "tqdm",
     "pubnub<6.4.0",
     "pynwb>=2.2.0,<3",
     "hdmf>=3.4.6",
     "datajoint>=0.13.6",
     "pymysql",
@@ -62,9 +64,16 @@
 [project.scripts]
 spyglass_cli = "spyglass.cli:cli"
 
 [project.urls]
 "Homepage" = "https://github.com/LorenFrankLab/spyglass"
 "Bug Tracker" = "https://github.com/LorenFrankLab/spyglass/issues"
 
+[project.optional-dependencies]
+position = ["ffmpeg", "numba>=0.54", "deeplabcut<2.3.0"]
 [tool.black]
 # line-length = 120
+
+[tool.codespell]
+skip = '.git,*.pdf,*.svg,*.ipynb'
+# Nevers - name in Citation
+ignore-words-list = 'nevers'
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/cli/cli.py` & `spyglass-neuro-0.4.0/src/spyglass/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 @click.command(
     help="Insert a session from a .nwb file that lives in the $SPYGLASS_BASE_DIR directory"
 )
 @click.argument("nwb_file_name")
 def insert_session(nwb_file_name: str):
-    import spyglass as nd
+    import spyglass as sg
 
-    nd.insert_sessions(nwb_file_name)
+    sg.insert_sessions(nwb_file_name)
 
 
 @click.command(help="List all sessions")
 def list_sessions():
     import spyglass.common as sgc
 
     results = sgc.Session & {}
@@ -412,15 +412,15 @@
         },
     )
 
     nds.SpikeSortingSelection.insert1(sorting_key, skip_duplicates=True)
     nds.SpikeSorting.populate([(nds.SpikeSortingSelection & sorting_key).proj()])
 
 
-@click.command(help="List spike sortings for a session.")
+@click.command(help="List spike sorting for a session.")
 @click.argument("nwb_file_name")
 def list_spike_sortings(nwb_file_name: str):
     import spyglass.spikesorting as nds
 
     results = nds.SpikeSorting & {"nwb_file_name": nwb_file_name}
     print(results)
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/__init__.py` & `spyglass-neuro-0.4.0/src/spyglass/common/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ElectrodeGroup,
     LFPBand,
     LFPBandSelection,
     LFPSelection,
     Raw,
     SampleCount,
 )
-from .common_filter import FirFilter
+from .common_filter import FirFilterParameters
 from .common_interval import (
     IntervalList,
     interval_list_censor,
     interval_list_contains,
     interval_list_contains_ind,
     interval_list_excludes,
     interval_list_excludes_ind,
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_backup.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_backup.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_behav.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_behav.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_device.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_device.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_dio.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_sensors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,43 @@
+"""Schema for headstage or other environmental sensors."""
+
 import datajoint as dj
 import pynwb
 
 from .common_ephys import Raw
 from .common_interval import IntervalList  # noqa: F401
 from .common_nwbfile import Nwbfile
 from .common_session import Session  # noqa: F401
-from ..utils.dj_helper_fn import fetch_nwb  # dj_replace
+from ..utils.dj_helper_fn import fetch_nwb
 from ..utils.nwb_helper_fn import get_data_interface, get_nwb_file
 
-schema = dj.schema("common_dio")
+schema = dj.schema("common_sensors")
 
 
 @schema
-class DIOEvents(dj.Imported):
+class SensorData(dj.Imported):
     definition = """
     -> Session
-    dio_event_name: varchar(80)   # the name assigned to this DIO event
     ---
-    dio_object_id: varchar(40)    # the object id of the data in the NWB file
-    -> IntervalList               # the list of intervals for this object
+    sensor_data_object_id: varchar(40)  # object id of the data in the NWB file
+    -> IntervalList                     # the list of intervals for this object
     """
 
     def make(self, key):
         nwb_file_name = key["nwb_file_name"]
-        nwb_file_abspath = Nwbfile.get_abs_path(nwb_file_name)
+        nwb_file_abspath = Nwbfile().get_abs_path(nwb_file_name)
         nwbf = get_nwb_file(nwb_file_abspath)
 
-        behav_events = get_data_interface(
-            nwbf, "behavioral_events", pynwb.behavior.BehavioralEvents
-        )
-        if behav_events is None:
-            print(
-                f"No conforming behavioral events data interface found in {nwb_file_name}\n"
-            )
+        sensor = get_data_interface(nwbf, "analog", pynwb.behavior.BehavioralEvents)
+        if sensor is None:
+            print(f"No conforming sensor data found in {nwb_file_name}\n")
             return
 
-        # the times for these events correspond to the valid times for the raw data
-        key["interval_list_name"] = (Raw() & {"nwb_file_name": nwb_file_name}).fetch1(
+        key["sensor_data_object_id"] = sensor.time_series["analog"].object_id
+        # the valid times for these data are the same as the valid times for the raw ephys data
+        key["interval_list_name"] = (Raw & {"nwb_file_name": nwb_file_name}).fetch1(
             "interval_list_name"
         )
-        for event_series in behav_events.time_series.values():
-            key["dio_event_name"] = event_series.name
-            key["dio_object_id"] = event_series.object_id
-            self.insert1(key, skip_duplicates=True)
+        self.insert1(key)
 
     def fetch_nwb(self, *attrs, **kwargs):
         return fetch_nwb(self, (Nwbfile, "nwb_file_abs_path"), *attrs, **kwargs)
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_ephys.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_ephys.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datajoint as dj
 import ndx_franklab_novela
 import numpy as np
 import pandas as pd
 import pynwb
 
 from .common_device import Probe  # noqa: F401
-from .common_filter import FirFilter
+from .common_filter import FirFilterParameters
 from .common_interval import (
     IntervalList,
     interval_list_censor,  # noqa: F401
     interval_list_contains_ind,
     interval_list_intersect,
 )
 from .common_nwbfile import AnalysisNwbfile, Nwbfile
@@ -358,15 +358,15 @@
 
 @schema
 class LFP(dj.Imported):
     definition = """
     -> LFPSelection
     ---
     -> IntervalList             # the valid intervals for the data
-    -> FirFilter                # the filter used for the data
+    -> FirFilterParameters                # the filter used for the data
     -> AnalysisNwbfile          # the name of the nwb file with the lfp data
     lfp_object_id: varchar(40)  # the NWB object ID for loading this object from the file
     lfp_sampling_rate: float    # the sampling rate, in HZ
     """
 
     def make(self, key):
         # get the NWB object with the data; FIX: change to fetch with additional infrastructure
@@ -395,15 +395,15 @@
         )
 
         # target 1 KHz sampling rate
         decimation = sampling_rate // 1000
 
         # get the LFP filter that matches the raw data
         filter = (
-            FirFilter()
+            FirFilterParameters()
             & {"filter_name": "LFP 0-400 Hz"}
             & {"filter_sampling_rate": sampling_rate}
         ).fetch(as_dict=True)
 
         # there should only be one filter that matches, so we take the first of the dictionaries
         key["filter_name"] = filter[0]["filter_name"]
         key["filter_sampling_rate"] = filter[0]["filter_sampling_rate"]
@@ -418,15 +418,15 @@
         electrode_keys = (LFPSelection.LFPElectrode & key).fetch("KEY")
         electrode_id_list = list(k["electrode_id"] for k in electrode_keys)
         electrode_id_list.sort()
 
         lfp_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
 
         lfp_file_abspath = AnalysisNwbfile().get_abs_path(lfp_file_name)
-        lfp_object_id, timestamp_interval = FirFilter().filter_data_nwb(
+        lfp_object_id, timestamp_interval = FirFilterParameters().filter_data_nwb(
             lfp_file_abspath,
             rawdata,
             filter_coeff,
             valid_times,
             electrode_id_list,
             decimation,
         )
@@ -477,15 +477,15 @@
         )
 
 
 @schema
 class LFPBandSelection(dj.Manual):
     definition = """
     -> LFP
-    -> FirFilter                   # the filter to use for the data
+    -> FirFilterParameters                   # the filter to use for the data
     -> IntervalList.proj(target_interval_list_name='interval_list_name')  # the original set of times to be filtered
     lfp_band_sampling_rate: int    # the sampling rate for this band
     ---
     min_interval_len = 1: float  # the minimum length of a valid interval to filter
     """
 
     class LFPBandElectrode(dj.Part):
@@ -508,15 +508,15 @@
         """
         Adds an entry for each electrode in the electrode_list with the specified filter, interval_list, and
         reference electrode.
         Also removes any entries that have the same filter, interval list and reference electrode but are not
         in the electrode_list.
         :param nwb_file_name: string - the name of the nwb file for the desired session
         :param electrode_list: list of LFP electrodes to be filtered
-        :param filter_name: the name of the filter (from the FirFilter schema)
+        :param filter_name: the name of the filter (from the FirFilterParameters schema)
         :param interval_name: the name of the interval list (from the IntervalList schema)
         :param reference_electrode_list: A single electrode id corresponding to the reference to use for all
         electrodes or a list with one element per entry in the electrode_list
         :param lfp_band_sampling_rate: The output sampling rate to be used for the filtered data; must be an
         integer divisor of the LFP sampling rate
         :return: none
         """
@@ -535,21 +535,21 @@
         decimation = lfp_sampling_rate // lfp_band_sampling_rate
         if lfp_sampling_rate // decimation != lfp_band_sampling_rate:
             raise ValueError(
                 f"lfp_band_sampling rate {lfp_band_sampling_rate} is not an integer divisor of lfp "
                 f"samping rate {lfp_sampling_rate}"
             )
         # filter
-        query = FirFilter() & {
+        query = FirFilterParameters() & {
             "filter_name": filter_name,
             "filter_sampling_rate": lfp_sampling_rate,
         }
         if not query:
             raise ValueError(
-                f"filter {filter_name}, sampling rate {lfp_sampling_rate} is not in the FirFilter table"
+                f"filter {filter_name}, sampling rate {lfp_sampling_rate} is not in the FirFilterParameters table"
             )
         # interval_list
         query = IntervalList() & {
             "nwb_file_name": nwb_file_name,
             "interval_name": interval_list_name,
         }
         if not query:
@@ -695,36 +695,36 @@
             if lfp_band_ref_id[index] != -1:
                 lfp_data[:, elect_index] = (
                     lfp_data[:, elect_index] - lfp_data[:, lfp_band_ref_index[index]]
                 )
 
         # get the LFP filter that matches the raw data
         filter = (
-            FirFilter()
+            FirFilterParameters()
             & {"filter_name": filter_name}
             & {"filter_sampling_rate": filter_sampling_rate}
         ).fetch(as_dict=True)
         if len(filter) == 0:
             raise ValueError(
                 f"Filter {filter_name} and sampling_rate {lfp_band_sampling_rate} does not exit in the "
-                "FirFilter table"
+                "FirFilterParameters table"
             )
 
         filter_coeff = filter[0]["filter_coeff"]
         if len(filter_coeff) == 0:
             print(
                 f"Error in LFPBand: no filter found with data sampling rate of {lfp_band_sampling_rate}"
             )
             return None
 
         # create the analysis nwb file to store the results.
         lfp_band_file_name = AnalysisNwbfile().create(key["nwb_file_name"])
         lfp_band_file_abspath = AnalysisNwbfile().get_abs_path(lfp_band_file_name)
         # filter the data and write to an the nwb file
-        filtered_data, new_timestamps = FirFilter().filter_data(
+        filtered_data, new_timestamps = FirFilterParameters().filter_data(
             timestamps,
             lfp_data,
             filter_coeff,
             lfp_band_valid_times,
             lfp_band_elect_index,
             decimation,
         )
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_filter.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # code to define filters that can be applied to continuous time data
+from typing import Union
 import warnings
 
 import datajoint as dj
 import matplotlib.pyplot as plt
 import numpy as np
 import psutil
 import pynwb
@@ -22,15 +23,15 @@
         raise ImportError(
             "You must install ghostipy to use filtering methods. Please note that to install ghostipy on "
             "an Mac M1, you must first install pyfftw from conda-forge."
         ) from e
 
 
 @schema
-class FirFilter(dj.Manual):
+class FirFilterParameters(dj.Manual):
     definition = """
     filter_name: varchar(80)           # descriptive name of this filter
     filter_sampling_rate: int          # sampling rate for this filter
     ---
     filter_type: enum("lowpass", "highpass", "bandpass")
     filter_low_stop = 0: float         # lowest frequency for stop band for low frequency side of filter
     filter_low_pass = 0: float         # lowest frequency for pass band of low frequency side of filter
@@ -158,14 +159,16 @@
         self,
         analysis_file_abs_path,
         eseries,
         filter_coeff,
         valid_times,
         electrode_ids,
         decimation,
+        description: str = "filtered data",
+        type: Union[None, str] = None,
     ):
         """
         :param analysis_nwb_file_name: str   full path to previously created analysis nwb file where filtered data
         should be stored. This also has the name of the original NWB file where the data will be taken from
         :param eseries: electrical series with data to be filtered
         :param filter_coeff: numpy array with filter coefficients for FIR filter
         :param valid_times: 2D numpy array with start and stop times of intervals to be filtered
@@ -249,17 +252,24 @@
             )
             eseries_name = "filtered data"
             es = pynwb.ecephys.ElectricalSeries(
                 name=eseries_name,
                 data=np.empty(tuple(output_shape_list), dtype=data_dtype),
                 electrodes=electrode_table_region,
                 timestamps=np.empty(output_shape_list[time_axis]),
+                description=description,
             )
-            # Add the electrical series to the scratch area
-            nwbf.add_scratch(es)
+            if type == "LFP":
+                lfp = pynwb.ecephys.LFP(electrical_series=es)
+                ecephys_module = nwbf.create_processing_module(
+                    name="ecephys", description=description
+                )
+                ecephys_module.add(lfp)
+            else:
+                nwbf.add_scratch(es)
             io.write(nwbf)
 
             # reload the NWB file to get the h5py objects for the data and the timestamps
             with pynwb.NWBHDF5IO(
                 path=analysis_file_abs_path, mode="a", load_namespaces=True
             ) as io:
                 nwbf = io.read()
@@ -452,9 +462,9 @@
             "standard LFP filter for 20 KHz data",
         )
         self.add_filter(
             "LFP 0-400 Hz",
             30000,
             "lowpass",
             [400, 425],
-            "standard LFP filter for 20 KHz data",
+            "standard LFP filter for 30 KHz data",
         )
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_interval.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_interval.py`

 * *Files 11% similar despite different names*

```diff
@@ -436,7 +436,47 @@
     """
     list_frames = np.unique(list_frames)
     interval_list = []
     for key, group in itertools.groupby(enumerate(list_frames), lambda t: t[1] - t[0]):
         group = list(group)
         interval_list.append([group[0][1], group[-1][1]])
     return np.asarray(interval_list)
+
+
+def interval_set_difference_inds(intervals1, intervals2):
+    """
+    e.g.
+    intervals1 = [(0, 5), (8, 10)]
+    intervals2 = [(1, 2), (3, 4), (6, 9)]
+
+    result = [(0, 1), (4, 5), (9, 10)]
+
+    Parameters
+    ----------
+    intervals1 : _type_
+        _description_
+    intervals2 : _type_
+        _description_
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    result = []
+    i = j = 0
+    while i < len(intervals1) and j < len(intervals2):
+        if intervals1[i][1] <= intervals2[j][0]:
+            result.append(intervals1[i])
+            i += 1
+        elif intervals2[j][1] <= intervals1[i][0]:
+            j += 1
+        else:
+            if intervals1[i][0] < intervals2[j][0]:
+                result.append((intervals1[i][0], intervals2[j][0]))
+            if intervals1[i][1] > intervals2[j][1]:
+                intervals1[i] = (intervals2[j][1], intervals1[i][1])
+                j += 1
+            else:
+                i += 1
+    result += intervals1[i:]
+    return result
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_lab.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_lab.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             LabMember.insert_from_name(team_member)
             query = (
                 LabMember.LabMemberInfo() & {"lab_member_name": team_member}
             ).fetch("google_user_name")
             if not len(query):
                 print(
                     f"Please add the Google user ID for {team_member} in the LabMember.LabMemberInfo table "
-                    "if you want to give them permission to manually curate sortings by this team."
+                    "if you want to give them permission to manually curate sorting by this team."
                 )
             labteammember_dict = dict()
             labteammember_dict["team_name"] = team_name
             labteammember_dict["lab_member_name"] = team_member
             cls.LabTeamMember.insert1(labteammember_dict, skip_duplicates=True)
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_nwbfile.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_nwbfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     definition = """
     # Table for holding the NWB files that contain results of analysis, such as spike sorting.
     analysis_file_name: varchar(255)               # name of the file
     ---
     -> Nwbfile                                     # name of the parent NWB file. Used for naming and metadata copy
     analysis_file_abs_path: filepath@analysis      # the full path to the file
     analysis_file_description = "": varchar(2000)  # an optional description of this analysis
-    analysis_parameters = NULL: blob               # additional relevant parmeters. Currently used only for analyses
+    analysis_parameters = NULL: blob               # additional relevant parameters. Currently used only for analyses
                                                    # that span multiple NWB files
     INDEX (analysis_file_abs_path)
     """
     # NOTE the INDEX above is implicit from filepath@... above but needs to be explicit
     # so that alter() can work
 
     def create(self, nwb_file_name):
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_position.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,15 +643,15 @@
         if is_grabbed:
             return cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
 
 
 @schema
 class PositionVideo(dj.Computed):
     """Creates a video of the computed head position and orientation as well as
-    the original LED positions overlayed on the video of the animal.
+    the original LED positions overlaid on the video of the animal.
 
     Use for debugging the effect of position extraction parameters."""
 
     definition = """
     -> IntervalPositionInfo
     ---
     """
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_region.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_region.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_ripple.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_ripple.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import datajoint as dj
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from ripple_detection import Karlsson_ripple_detector, Kay_ripple_detector
 from ripple_detection.core import gaussian_smooth, get_envelope
 from spyglass.common import (
-    Electrode,
     IntervalList,  # noqa
     IntervalPositionInfo,
-    IntervalPositionInfoSelection,
-    LFPBand,
-    LFPBandSelection,
-    Session,
 )
+from spyglass.lfp.v1 import LFPBand, LFPBandSelection
 from spyglass.common.common_nwbfile import AnalysisNwbfile
 from spyglass.utils.dj_helper_fn import fetch_nwb
 
 schema = dj.schema("common_ripple")
 
 RIPPLE_DETECTION_ALGORITHMS = {
     "Kay_ripple_detector": Kay_ripple_detector,
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_session.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_session.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_subject.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_subject.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/common_task.py` & `spyglass-neuro-0.4.0/src/spyglass/common/common_task.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/populate_all_common.py` & `spyglass-neuro-0.4.0/src/spyglass/common/populate_all_common.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/prepopulate/prepopulate.py` & `spyglass-neuro-0.4.0/src/spyglass/common/prepopulate/prepopulate.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/common/signal_processing.py` & `spyglass-neuro-0.4.0/src/spyglass/common/signal_processing.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/data_import/insert_sessions.py` & `spyglass-neuro-0.4.0/src/spyglass/data_import/insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/__init__.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/clusterless.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/clusterless.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,17 @@
 import spikeinterface as si
 import xarray as xr
 from replay_trajectory_classification.classifier import (
     _DEFAULT_CLUSTERLESS_MODEL_KWARGS,
     _DEFAULT_CONTINUOUS_TRANSITIONS,
     _DEFAULT_ENVIRONMENT,
 )
-from replay_trajectory_classification.continuous_state_transitions import (
-    RandomWalk,
-    Uniform,
-)
 from replay_trajectory_classification.discrete_state_transitions import DiagonalDiscrete
-from replay_trajectory_classification.environments import Environment
 from replay_trajectory_classification.initial_conditions import UniformInitialConditions
-from replay_trajectory_classification.observation_model import ObservationModel
+
 from ripple_detection import (
     get_multiunit_population_firing_rate,
     multiunit_HSE_detector,
 )
 from spyglass.common.common_interval import IntervalList
 from spyglass.common.common_nwbfile import AnalysisNwbfile
 from spyglass.common.common_position import IntervalPositionInfo
@@ -665,17 +660,34 @@
 
         self.insert1(key)
 
 
 def get_decoding_data_for_epoch(
     nwb_file_name: str,
     interval_list_name: str,
-    position_info_param_name="default_decoding",
-    additional_mark_keys={},
-):
+    position_info_param_name: str = "default_decoding",
+    additional_mark_keys: dict = {},
+) -> tuple[pd.DataFrame, xr.DataArray, list[slice]]:
+    """Collects necessary data for decoding.
+
+    Parameters
+    ----------
+    nwb_file_name : str
+    interval_list_name : str
+    position_info_param_name : str, optional
+    additional_mark_keys : dict, optional
+
+    Returns
+    -------
+    position_info : pd.DataFrame, shape (n_time, n_columns)
+    marks : xr.DataArray, shape (n_time, n_marks, n_electrodes)
+    valid_slices : list[slice]
+
+    """
+
     valid_ephys_position_times_by_epoch = get_valid_ephys_position_times_by_epoch(
         nwb_file_name
     )
     valid_ephys_position_times = valid_ephys_position_times_by_epoch[interval_list_name]
     valid_slices = convert_valid_times_to_slice(valid_ephys_position_times)
     position_interval_name = convert_epoch_interval_name_to_position_interval_name(
         interval_list_name
@@ -706,18 +718,35 @@
     marks = xr.concat([marks.sel(time=times) for times in valid_slices], dim="time")
 
     return position_info, marks, valid_slices
 
 
 def get_data_for_multiple_epochs(
     nwb_file_name: str,
-    epoch_names: list,
+    epoch_names: list[str],
     position_info_param_name="default_decoding",
-    additional_mark_keys={},
-):
+    additional_mark_keys: dict = {},
+) -> tuple[pd.DataFrame, xr.DataArray, dict[str, list[slice]], np.ndarray]:
+    """Collects necessary data for decoding multiple environments
+
+    Parameters
+    ----------
+    nwb_file_name : str
+    epoch_names : list[str]
+    position_info_param_name : str, optional
+    additional_mark_keys : dict, optional
+
+    Returns
+    -------
+    position_info : pd.DataFrame, shape (n_time, n_columns)
+    marks : xr.DataArray, shape (n_time, n_marks, n_electrodes)
+    valid_slices : dict[str, list[slice]]
+    environment_labels : np.ndarray, shape (n_time,)
+
+    """
     data = []
     environment_labels = []
 
     for epoch in epoch_names:
         data.append(
             get_decoding_data_for_epoch(
                 nwb_file_name,
@@ -738,41 +767,35 @@
     }
 
     assert position_info.shape[0] == marks.shape[0]
 
     return position_info, marks, valid_slices, environment_labels
 
 
-def create_model_for_multiple_epochs(epoch_names: list, env_kwargs: dict):
-    observation_models = []
-    environments = []
-    continuous_transition_types = []
-
-    for epoch in epoch_names:
-        observation_models.append(ObservationModel(epoch))
-        environments.append(Environment(epoch, **env_kwargs))
-
-    for epoch1 in epoch_names:
-        continuous_transition_types.append([])
-        for epoch2 in epoch_names:
-            if epoch1 == epoch2:
-                continuous_transition_types[-1].append(
-                    RandomWalk(epoch1, use_diffusion=True)
-                )
-            else:
-                continuous_transition_types[-1].append(Uniform(epoch1, epoch2))
-
-    return observation_models, environments, continuous_transition_types
-
-
 def populate_mark_indicators(
-    spikesorting_selection_keys: list,
-    mark_param_name="default",
-    position_info_param_name="default_decoding",
+    spikesorting_selection_keys: dict,
+    mark_param_name: str = "default",
+    position_info_param_name: str = "default_decoding",
 ):
+    """Populate mark indicators for all units in the given spike sorting selection.
+
+    This function is a way to do several pipeline steps at once. It will:
+      1. Populate the SpikeSortingSelection table
+      2. Populate the SpikeSorting table
+      3. Populate the Curation table
+      4. Populate the CuratedSpikeSortingSelection table
+      5. Populate UnitMarks
+      6. Compute UnitMarksIndicator for each position epoch
+
+    Parameters
+    ----------
+    spikesorting_selection_keys : dict
+    mark_param_name : str, optional
+    position_info_param_name : str, optional
+    """
     spikesorting_selection_keys = deepcopy(spikesorting_selection_keys)
     # Populate spike sorting
     SpikeSortingSelection().insert(
         spikesorting_selection_keys,
         skip_duplicates=True,
     )
     SpikeSorting.populate(spikesorting_selection_keys)
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/dj_decoder_conversion.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/dj_decoder_conversion.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,41 +20,66 @@
     UniformInitialConditions,
     UniformOneEnvironmentInitialConditions,
 )
 from replay_trajectory_classification.observation_model import ObservationModel
 from track_linearization import make_track_graph
 
 
-def _convert_dict_to_class(d: dict, class_conversion: dict):
+def _convert_dict_to_class(d: dict, class_conversion: dict) -> object:
+    """Converts a dictionary into a class object
+
+    Parameters
+    ----------
+    d : dict
+    class_conversion : dict
+
+    Returns
+    -------
+    class_based_on_dict : object
+
+    """
     class_name = d.pop("class_name")
     return class_conversion[class_name](**d)
 
 
-def _convert_env_dict(env_params):
+def _convert_env_dict(env_params: dict) -> Environment:
+    """If the track graph is in the environment parameters, convert it to a networkx graph
+
+    Parameters
+    ----------
+    env_params : dict
+
+    Returns
+    -------
+    environment : Environment
+    """
     if env_params["track_graph"] is not None:
         env_params["track_graph"] = make_track_graph(**env_params["track_graph"])
 
     return Environment(**env_params)
 
 
-def _to_dict(transition):
+def _to_dict(transition: object) -> dict:
+    """Helper function to convert a transition class into a dictionary"""
     parameters = vars(transition)
     parameters["class_name"] = type(transition).__name__
 
     return parameters
 
 
-def _convert_transitions_to_dict(transitions):
+def _convert_transitions_to_dict(transitions: list[list[object]]) -> list[list[dict]]:
+    """Converts a list of lists of transition classes into a list of lists of dictionaries"""
     return [
         [_to_dict(transition) for transition in transition_rows]
         for transition_rows in transitions
     ]
 
 
-def restore_classes(params):
+def restore_classes(params: dict) -> dict:
+    """Converts a dictionary of parameters into a dictionary of classes since datajoint cannot handle classes"""
     continuous_state_transition_types = {
         "RandomWalk": RandomWalk,
         "RandomWalkDirection1": RandomWalkDirection1,
         "RandomWalkDirection2": RandomWalkDirection2,
         "Uniform": Uniform,
         "Identity": Identity,
     }
@@ -93,35 +118,38 @@
             for obs in params["classifier_params"]["observation_models"]
         ]
 
     return params
 
 
 def _convert_algorithm_params(algo_params):
+    """Helper function that adds in the algorithm name to the algorithm parameters dictionary"""
     try:
         algo_params = algo_params.copy()
         algo_params["model"] = algo_params["model"].__name__
     except KeyError:
         pass
 
     return algo_params
 
 
-def _convert_environment_to_dict(env):
+def _convert_environment_to_dict(env: Environment) -> dict:
+    """Converts an Environment instance into a dictionary so that datajoint can store it"""
     if env.track_graph is not None:
         track_graph = env.track_graph
         env.track_graph = {
             "node_positions": [v["pos"] for v in dict(track_graph.nodes).values()],
             "edges": list(track_graph.edges),
         }
 
     return vars(env)
 
 
-def convert_classes_to_dict(key):
+def convert_classes_to_dict(key: dict) -> dict:
+    """Converts the classifier parameters into a dictionary so that datajoint can store it."""
     try:
         key["classifier_params"]["environments"] = [
             _convert_environment_to_dict(env)
             for env in key["classifier_params"]["environments"]
         ]
     except TypeError:
         key["classifier_params"]["environments"] = [
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/sorted_spikes.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/sorted_spikes.py`

 * *Files 21% similar despite different names*

```diff
@@ -241,44 +241,172 @@
     def insert1(self, key, **kwargs):
         super().insert1(convert_classes_to_dict(key), **kwargs)
 
     def fetch1(self, *args, **kwargs):
         return restore_classes(super().fetch1(*args, **kwargs))
 
 
+def get_spike_indicator(
+    key: dict, time_range: tuple[float, float], sampling_rate: float = 500.0
+) -> pd.DataFrame:
+    """For a given key, returns a dataframe with the spike indicator for each unit
+
+    Parameters
+    ----------
+    key : dict
+    time_range : tuple[float, float]
+        Start and end time of the spike indicator
+    sampling_rate : float, optional
+
+    Returns
+    -------
+    spike_indicator : pd.DataFrame, shape (n_time, n_units)
+        A dataframe with the spike indicator for each unit
+    """
+    start_time, end_time = time_range
+    n_samples = int(np.ceil((end_time - start_time) * sampling_rate)) + 1
+    time = np.linspace(start_time, end_time, n_samples)
+
+    spike_indicator = dict()
+    spikes_nwb_table = CuratedSpikeSorting() & key
+
+    for n_trode in spikes_nwb_table.fetch_nwb():
+        try:
+            for unit_id, unit_spike_times in n_trode["units"]["spike_times"].items():
+                unit_spike_times = unit_spike_times[
+                    (unit_spike_times > time[0]) & (unit_spike_times <= time[-1])
+                ]
+                unit_name = f'{n_trode["sort_group_id"]:04d}_{unit_id:04d}'
+                spike_indicator[unit_name] = np.bincount(
+                    np.digitize(unit_spike_times, time[1:-1]), minlength=time.shape[0]
+                )
+        except KeyError:
+            pass
+
+    return pd.DataFrame(
+        spike_indicator,
+        index=pd.Index(time, name="time"),
+    )
+
+
 def get_decoding_data_for_epoch(
     nwb_file_name: str,
     interval_list_name: str,
-    position_info_param_name="default_decoding",
-    additional_spike_keys={},
-):
+    position_info_param_name: str = "default",
+    additional_spike_keys: dict = {},
+) -> tuple[pd.DataFrame, pd.DataFrame, list[slice]]:
+    """Collects the data needed for decoding
+
+    Parameters
+    ----------
+    nwb_file_name : str
+    interval_list_name : str
+    position_info_param_name : str, optional
+    additional_spike_keys : dict, optional
+
+    Returns
+    -------
+    position_info : pd.DataFrame, shape (n_time, n_position_features)
+    spikes : pd.DataFrame, shape (n_time, n_units)
+    valid_slices : list[slice]
+
+    """
+    # valid slices
     valid_ephys_position_times_by_epoch = get_valid_ephys_position_times_by_epoch(
         nwb_file_name
     )
     valid_ephys_position_times = valid_ephys_position_times_by_epoch[interval_list_name]
     valid_slices = convert_valid_times_to_slice(valid_ephys_position_times)
+
+    # position interval
     position_interval_name = convert_epoch_interval_name_to_position_interval_name(
         interval_list_name
     )
 
+    # spikes
+    valid_times = np.asarray([(times.start, times.stop) for times in valid_slices])
+
+    curated_spikes_key = {
+        "nwb_file_name": nwb_file_name,
+        **additional_spike_keys,
+    }
+    spikes = get_spike_indicator(
+        curated_spikes_key, (valid_times.min(), valid_times.max()), sampling_rate=500
+    )
+    spikes = pd.concat([spikes.loc[times] for times in valid_slices])
+
+    # position
     position_info = (
         IntervalPositionInfo()
         & {
             "nwb_file_name": nwb_file_name,
             "interval_list_name": position_interval_name,
             "position_info_param_name": position_info_param_name,
         }
     ).fetch1_dataframe()
+    new_time = spikes.index.to_numpy()
+    new_index = pd.Index(
+        np.unique(np.concatenate((position_info.index, new_time))), name="time"
+    )
+    position_info = (
+        position_info.reindex(index=new_index)
+        .interpolate(method="linear")
+        .reindex(index=new_time)
+    )
 
-    position_info = pd.concat([position_info.loc[times] for times in valid_slices])
+    return position_info, spikes, valid_slices
 
-    spikes = (
-        SortedSpikesIndicator
-        & {
-            "nwb_file_name": nwb_file_name,
-            "interval_list_name": position_interval_name,
-            **additional_spike_keys,
-        }
-    ).fetch_dataframe()
-    spikes = pd.concat([spikes.loc[times] for times in valid_slices])
 
-    return position_info, spikes, valid_slices
+def get_data_for_multiple_epochs(
+    nwb_file_name: str,
+    epoch_names: list,
+    position_info_param_name: str = "decoding",
+    additional_spike_keys: dict = {},
+) -> tuple[pd.DataFrame, pd.DataFrame, list[slice], np.ndarray, np.ndarray]:
+    """Collects the data needed for decoding for multiple epochs
+
+    Parameters
+    ----------
+    nwb_file_name : str
+    epoch_names : list
+    position_info_param_name : str, optional
+    additional_spike_keys : dict, optional
+
+    Returns
+    -------
+    position_info : pd.DataFrame, shape (n_time, n_position_features)
+    spikes : pd.DataFrame, shape (n_time, n_units)
+    valid_slices : list[slice]
+    environment_labels : np.ndarray, shape (n_time,)
+        The environment label for each time point
+    sort_group_ids : np.ndarray, shape (n_units,)
+        The sort group of each unit
+    """
+    data = []
+    environment_labels = []
+
+    for epoch in epoch_names:
+        print(epoch)
+        data.append(
+            get_decoding_data_for_epoch(
+                nwb_file_name,
+                epoch,
+                position_info_param_name=position_info_param_name,
+                additional_spike_keys=additional_spike_keys,
+            )
+        )
+        n_time = data[-1][0].shape[0]
+        environment_labels.append([epoch] * n_time)
+
+    environment_labels = np.concatenate(environment_labels, axis=0)
+    position_info, spikes, valid_slices = list(zip(*data))
+    position_info = pd.concat(position_info, axis=0)
+    spikes = pd.concat(spikes, axis=0)
+    valid_slices = {
+        epoch: valid_slice for epoch, valid_slice in zip(epoch_names, valid_slices)
+    }
+
+    assert position_info.shape[0] == spikes.shape[0]
+
+    sort_group_ids = np.asarray([int(col.split("_")[0]) for col in spikes.columns])
+
+    return position_info, spikes, valid_slices, environment_labels, sort_group_ids
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/visualization.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import matplotlib.animation as animation
 import matplotlib.font_manager as fm
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import sortingview.views as vv
+import xarray as xr
 from mpl_toolkits.axes_grid1.anchored_artists import AnchoredSizeBar
 from ripple_detection import get_multiunit_population_firing_rate
 from tqdm.auto import tqdm
 
 from spyglass.decoding.visualization_1D_view import create_1D_decode_view
 from spyglass.decoding.visualization_2D_view import create_2D_decode_view
 
@@ -437,23 +438,23 @@
         if movie_name is not None:
             movie.save(movie_name, writer=writer, dpi=200)
 
         return fig, movie
 
 
 def create_interactive_1D_decoding_figurl(
-    position_info,
-    linear_position_info,
-    marks,
-    results,
-    position_name="linear_position",
-    speed_name="head_speed",
-    posterior_type="acausal_posterior",
-    sampling_frequency=500,
-    view_height=800,
+    position_info: pd.DataFrame,
+    linear_position_info: pd.DataFrame,
+    marks: xr.DataArray,
+    results: xr.Dataset,
+    position_name: str = "linear_position",
+    speed_name: str = "head_speed",
+    posterior_type: str = "acausal_posterior",
+    sampling_frequency: float = 500.0,
+    view_height: int = 800,
 ):
     decode_view = create_1D_decode_view(
         posterior=results[posterior_type].sum("state"),
         linear_position=linear_position_info[position_name],
     )
 
     probability_view = vv.TimeseriesGraph()
@@ -523,25 +524,25 @@
         ],
     )
 
     return view
 
 
 def create_interactive_2D_decoding_figurl(
-    position_info,
-    marks,
-    results,
-    bin_size,
-    position_name=["head_position_x", "head_position_y"],
-    head_direction_name="head_orientation",
-    speed_name="head_speed",
-    posterior_type="acausal_posterior",
-    sampling_frequency=500,
-    view_height=800,
-):
+    position_info: pd.DataFrame,
+    marks: xr.DataArray,
+    results: xr.Dataset,
+    bin_size: float,
+    position_name: list[str] = ["head_position_x", "head_position_y"],
+    head_direction_name: str = "head_orientation",
+    speed_name: str = "head_speed",
+    posterior_type: str = "acausal_posterior",
+    sampling_frequency: float = 500.0,
+    view_height: int = 800,
+) -> vv.Box:
     decode_view = create_2D_decode_view(
         position_time=position_info.index,
         position=position_info[position_name],
         posterior=results[posterior_type].sum("state"),
         bin_size=bin_size,
         head_dir=position_info[head_direction_name],
     )
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/visualization_1D_view.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/visualization_1D_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 ) -> vvf.DecodedLinearPositionData:
     """Creates a view of an interactive heatmap of position vs. time.
 
     Parameters
     ----------
     posterior : xr.DataArray, shape (n_time, n_position_bins)
     linear_position : np.ndarray, shape (n_time, ), optional
-    ref_time_sec : np.float64, optional reference time for the purpose of offsetting the start time
+    ref_time_sec : np.float64, optional
+        Reference time for the purpose of offsetting the start time
 
     Returns
     -------
     view : vvf.DecodedLinearPositionData
 
     """
     if linear_position is not None:
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/decoding/visualization_2D_view.py` & `spyglass-neuro-0.4.0/src/spyglass/decoding/visualization_2D_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,14 +287,21 @@
     head_dir : np.ndarray, optional
 
     Returns
     -------
     view : vvf.TrackPositionAnimationV1
 
     """
+    assert (
+        position_time.shape[0] == position.shape[0]
+    ), "position_time and position must have the same length"
+    assert (
+        posterior.shape[0] == position.shape[0]
+    ), "posterior and position must have the same length"
+
     position_time = np.squeeze(np.asarray(position_time)).copy()
     position = np.asarray(position)
     if head_dir is not None:
         head_dir = np.squeeze(np.asarray(head_dir))
 
     track_width, track_height, upper_left_points = make_track(
         position, bin_size=bin_size
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/figurl_views/SpikeSortingRecordingView.py` & `spyglass-neuro-0.4.0/src/spyglass/figurl_views/SpikeSortingRecordingView.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/figurl_views/SpikeSortingView.py` & `spyglass-neuro-0.4.0/src/spyglass/figurl_views/SpikeSortingView.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 schema = dj.schema("figurl_view_spike_sorting_recording")
 
 
 @schema
 class SpikeSortingView(dj.Computed):
     definition = """
-    # Schema for storing figurl views of spike sortings
+    # Schema for storing figurl views of spike sorting
     -> SpikeSorting
     ---
     figurl: varchar(10000)
     """
 
     def make(self, key):
         recording_record = (
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/figurl_views/prepare_spikesortingview_data.py` & `spyglass-neuro-0.4.0/src/spyglass/figurl_views/prepare_spikesortingview_data.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/lock/file_lock.py` & `spyglass-neuro-0.4.0/src/spyglass/lock/file_lock.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/__init__.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/__init__.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/curation_figurl.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/curation_figurl.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         recording=R,
         sorting=S,
         segment_duration_sec=60 * 20,
         snippet_len=(20, 20),
         max_num_snippets_per_segment=100,
         channel_neighborhood_size=7,
     )
-    # create a fake unit similiarity matrix (for future reference)
+    # create a fake unit similarity matrix (for future reference)
     # similarity_scores = []
     # for u1 in X.unit_ids:
     #     for u2 in X.unit_ids:
     #         similarity_scores.append(
     #             vv.UnitSimilarityScore(
     #                 unit_id1=u1,
     #                 unit_id2=u2,
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/merged_sorting_extractor.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/merged_sorting_extractor.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/sortingview.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/sortingview.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/sortingview_helper_fn.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/sortingview_helper_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         sorting=sorting,
         segment_duration_sec=60 * 20,
         snippet_len=(20, 20),
         max_num_snippets_per_segment=100,
         channel_neighborhood_size=7,
     )
 
-    # create a fake unit similiarity matrix
+    # create a fake unit similarity matrix
     # similarity_scores = []
     # for u1 in X.unit_ids:
     #     for u2 in X.unit_ids:
     #         similarity_scores.append(
     #             vv.UnitSimilarityScore(
     #                 unit_id1=u1,
     #                 unit_id2=u2,
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_artifact.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import spikeinterface as si
 from spikeinterface.core.job_tools import ChunkRecordingExecutor, ensure_n_jobs
 
 from ..common.common_interval import (
     IntervalList,
     _union_concat,
     interval_from_inds,
-    interval_list_intersect,
+    interval_set_difference_inds,
 )
 from ..utils.nwb_helper_fn import get_valid_intervals
 from .spikesorting_recording import SpikeSortingRecording
 
 schema = dj.schema("spikesorting_artifact")
 
 
@@ -241,31 +241,46 @@
 
     if len(artifact_frames) == 0:
         recording_interval = np.asarray([[valid_timestamps[0], valid_timestamps[-1]]])
         artifact_times_empty = np.asarray([])
         print("No artifacts detected.")
         return recording_interval, artifact_times_empty
 
+    # convert indices to intervals
     artifact_intervals = interval_from_inds(artifact_frames)
 
+    # convert to seconds and pad with window
     artifact_intervals_s = np.zeros((len(artifact_intervals), 2), dtype=np.float64)
     for interval_idx, interval in enumerate(artifact_intervals):
         artifact_intervals_s[interval_idx] = [
             valid_timestamps[interval[0]] - half_removal_window_s,
             valid_timestamps[interval[1]] + half_removal_window_s,
         ]
+    # make the artifact intervals disjoint
     artifact_intervals_s = reduce(_union_concat, artifact_intervals_s)
 
-    valid_intervals = get_valid_intervals(
-        valid_timestamps, recording.get_sampling_frequency(), 1.5, 0.000001
-    )
-    artifact_removed_valid_times = interval_list_intersect(
-        valid_intervals, artifact_intervals_s
+    # convert seconds back to indices
+    artifact_intervals_new = []
+    for artifact_interval_s in artifact_intervals_s:
+        artifact_intervals_new.append(
+            np.searchsorted(valid_timestamps, artifact_interval_s)
+        )
+
+    # compute set difference between intervals (of indices)
+    artifact_removed_valid_times_ind = interval_set_difference_inds(
+        [(0, len(valid_timestamps) - 1)], artifact_intervals_new
     )
 
+    # convert back to seconds
+    artifact_removed_valid_times = []
+    for i in artifact_removed_valid_times_ind:
+        artifact_removed_valid_times.append(
+            (valid_timestamps[i[0]], valid_timestamps[i[1]])
+        )
+
     return artifact_removed_valid_times, artifact_intervals_s
 
 
 def _init_artifact_worker(
     recording, zscore_thresh=None, amplitude_thresh=None, proportion_above_thresh=1.0
 ):
     # create a local dict per worker
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_curation.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     return MergedSortingExtractor(parent_sorting=sorting, merge_groups=merge_groups)
 
 
 @schema
 class Curation(dj.Manual):
     definition = """
     # Stores each spike sorting; similar to IntervalList
-    curation_id: int # a number correponding to the index of this curation
+    curation_id: int # a number corresponding to the index of this curation
     -> SpikeSorting
     ---
     parent_curation_id=-1: int
     curation_labels: blob # a dictionary of labels for the units
     merge_groups: blob # a list of merge groups for the units
     quality_metrics: blob # a list of quality metrics for the units (if available)
     description='': varchar(1000) #optional description for this curated sort
@@ -310,15 +310,15 @@
 
         sorting = Curation.get_curated_sorting(key)
 
         print("Extracting waveforms...")
         waveform_params = (WaveformParameters & key).fetch1("waveform_params")
         if "whiten" in waveform_params:
             if waveform_params.pop("whiten"):
-                recording = sp.whiten(recording)
+                recording = sp.whiten(recording, dtype=np.float16)
 
         waveform_extractor_name = self._get_waveform_extractor_name(key)
         key["waveform_extractor_path"] = str(
             Path(os.environ["SPYGLASS_WAVEFORMS_DIR"]) / Path(waveform_extractor_name)
         )
         if os.path.exists(key["waveform_extractor_path"]):
             shutil.rmtree(key["waveform_extractor_path"])
@@ -375,30 +375,32 @@
     metric_params_name: varchar(200)
     ---
     metric_params: blob
     """
     metric_default_params = {
         "snr": {
             "peak_sign": "neg",
-            "num_chunks_per_segment": 20,
-            "chunk_size": 10000,
-            "seed": 0,
+            "random_chunk_kwargs_dict": {
+                "num_chunks_per_segment": 20,
+                "chunk_size": 10000,
+                "seed": 0,
+            },
         },
         "isi_violation": {"isi_threshold_ms": 1.5, "min_isi_ms": 0.0},
         "nn_isolation": {
-            "max_spikes_for_nn": 1000,
-            "min_spikes_for_nn": 10,
+            "max_spikes": 1000,
+            "min_spikes": 10,
             "n_neighbors": 5,
             "n_components": 7,
             "radius_um": 100,
             "seed": 0,
         },
         "nn_noise_overlap": {
-            "max_spikes_for_nn": 1000,
-            "min_spikes_for_nn": 10,
+            "max_spikes": 1000,
+            "min_spikes": 10,
             "n_neighbors": 5,
             "n_components": 7,
             "radius_um": 100,
             "seed": 0,
         },
         "peak_channel": {"peak_sign": "neg"},
         "num_spikes": {},
@@ -416,15 +418,15 @@
 
     def get_metric_default_params(self, metric: str):
         "Returns default params for the given metric"
         return self.metric_default_params(metric)
 
     def insert_default(self):
         self.insert1(
-            ["franklab_default", self.metric_default_params], skip_duplicates=True
+            ["franklab_default3", self.metric_default_params], skip_duplicates=True
         )
 
     def get_available_metrics(self):
         for metric in _metric_name_to_func:
             if metric in self.available_metrics:
                 metric_doc = _metric_name_to_func[metric].__doc__.split("\n")[0]
                 metric_string = ("{metric_name} : {metric_doc}").format(
@@ -988,15 +990,15 @@
 
     def get_included_units(self, curated_sorting_key, unit_inclusion_param_name):
         """given a reference to a set of curated sorting units and the name of a unit inclusion parameter list, returns
 
         Parameters
         ----------
         curated_sorting_key : dict
-            key to select a set of curated sortings
+            key to select a set of curated sorting
         unit_inclusion_param_name : str
             name of a unit inclusion parameter entry
 
         Returns
         ------unit key
         dict
             key to select all of the included units
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_recording.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                     np.logical_and(
                         electrodes["electrode_group_name"] == e_group,
                         electrodes["probe_shank"] == shank,
                     )
                 ]
                 if (
                     omit_unitrode and len(shank_elect) == 1
-                ):  # ommit unitrodes if indicated
+                ):  # omit unitrodes if indicated
                     print(
                         f"Omitting electrode group {e_group}, shank {shank} from sort groups because unitrode."
                     )
                     continue
                 self.insert1(sg_key)
                 for elect in shank_elect:
                     sge_key["electrode_id"] = elect
@@ -284,15 +284,15 @@
         for i in range(3):
             if np.any(np.nonzero(tmp_geom[:, i])):
                 if n_found < 2:
                     geometry[:, n_found] = tmp_geom[:, i]
                     n_found += 1
                 else:
                     Warning(
-                        "Relative electrode locations have three coordinates; only two are currenlty supported"
+                        "Relative electrode locations have three coordinates; only two are currently supported"
                     )
         return np.ndarray.tolist(geometry)
 
 
 @schema
 class SortInterval(dj.Manual):
     definition = """
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/spikesorting/spikesorting_sorting.py` & `spyglass-neuro-0.4.0/src/spyglass/spikesorting/spikesorting_sorting.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 import uuid
 from pathlib import Path
 
 import datajoint as dj
 import numpy as np
 import spikeinterface as si
+import spikeinterface.preprocessing as sip
 import spikeinterface.sorters as sis
 from spikeinterface.sortingcomponents.peak_detection import detect_peaks
 
 from ..common.common_lab import LabMember, LabTeam
 from ..common.common_nwbfile import AnalysisNwbfile
 from ..utils.dj_helper_fn import fetch_nwb
 from .spikesorting_artifact import ArtifactRemovedIntervalList
@@ -32,15 +33,15 @@
     sorter_params: blob
     """
 
     def insert_default(self):
         """Default params from spike sorters available via spikeinterface"""
         sorters = sis.available_sorters()
         for sorter in sorters:
-            sorter_params = sis.get_default_params(sorter)
+            sorter_params = sis.get_default_sorter_params(sorter)
             self.insert1([sorter, "default", sorter_params], skip_duplicates=True)
 
         # Insert Frank lab defaults
         # Hippocampus tetrode default
         sorter = "mountainsort4"
         sorter_params_name = "franklab_tetrode_hippocampus_30KHz"
         sorter_params = {
@@ -165,15 +166,15 @@
                 list_triggers.append(
                     np.arange(
                         np.searchsorted(timestamps, interval[0]),
                         np.searchsorted(timestamps, interval[1]),
                     )
                 )
             list_triggers = [list(np.concatenate(list_triggers))]
-            recording = si.preprocessing.remove_artifacts(
+            recording = sip.remove_artifacts(
                 recording=recording,
                 list_triggers=list_triggers,
                 ms_before=None,
                 ms_after=None,
                 mode="zeros",
             )
 
@@ -185,24 +186,32 @@
         sorter_temp_dir = tempfile.TemporaryDirectory(
             dir=os.getenv("SPYGLASS_TEMP_DIR")
         )
         # add tempdir option for mountainsort
         sorter_params["tempdir"] = sorter_temp_dir.name
 
         if sorter == "clusterless_thresholder":
-            # Detect peaks for clusterless decoding
-            # need to remove tempdir
+            # need to remove tempdir and whiten from sorter_params
             sorter_params.pop("tempdir", None)
+            sorter_params.pop("whiten", None)
+
+            # Detect peaks for clusterless decoding
             detected_spikes = detect_peaks(recording, **sorter_params)
             sorting = si.NumpySorting.from_times_labels(
                 times_list=detected_spikes["sample_ind"],
                 labels_list=np.zeros(len(detected_spikes), dtype=np.int),
                 sampling_frequency=recording.get_sampling_frequency(),
             )
         else:
+            # whiten recording; make sure dtype is float16
+            recording = sip.whiten(recording, dtype="float16")
+            if sorter_params["whiten"] == True:
+                print(
+                    "Warning: the recording is whitened prior to sorting but the sorter param includes whitening"
+                )
             sorting = sis.run_sorter(
                 sorter,
                 recording,
                 output_folder=sorter_temp_dir.name,
                 delete_output_folder=True,
                 **sorter_params,
             )
@@ -275,11 +284,11 @@
 
     @staticmethod
     def _get_sorting_name(key):
         recording_name = SpikeSortingRecording._get_recording_name(key)
         sorting_name = recording_name + "_" + str(uuid.uuid4())[0:8] + "_spikesorting"
         return sorting_name
 
-    # TODO: write a function to import sortings done outside of dj
+    # TODO: write a function to import sorting done outside of dj
 
     def _import_sorting(self, key):
         raise NotImplementedError
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/utils/dj_helper_fn.py` & `spyglass-neuro-0.4.0/src/spyglass/utils/dj_helper_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             if "object_id" in id_attr and rec_dict[id_attr] != ""
         }
         ret.append({**rec_dict, **nwb_objs})
     return ret
 
 
 def _get_nwb_object(objects, object_id):
-    """Retreive NWB object and try to convert to dataframe if possible"""
+    """Retrieve NWB object and try to convert to dataframe if possible"""
     try:
         return objects[object_id].to_dataframe()
     except AttributeError:
         return objects[object_id]
 
 
 def get_child_tables(table):
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass/utils/nwb_helper_fn.py` & `spyglass-neuro-0.4.0/src/spyglass/utils/nwb_helper_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,20 @@
     nwb_uri = None
     nwb_raw_uri = None
     if nwbfile is None:
         # check to see if the file exists
         if not os.path.exists(nwb_file_path):
             print(f"NWB file {nwb_file_path} does not exist locally; checking kachery")
             # first try the analysis files
-            from ..sharing.sharing_kachery import AnalysisNwbfileKachery, NwbfileKachery
+            from ..sharing.sharing_kachery import AnalysisNwbfileKachery
 
             # the download functions assume just the filename, so we need to get that from the path
             if not AnalysisNwbfileKachery.download_file(
                 os.path.basename(nwb_file_path)
-            ) and not NwbfileKachery.download_file(os.path.basename(nwb_file_path)):
-                print(f"NWB file {nwb_file_path} is not available on kachery; aborting")
+            ):
                 return None
         # now open the file
         io = pynwb.NWBHDF5IO(
             path=nwb_file_path, mode="r", load_namespaces=True
         )  # keep file open
         nwbfile = io.read()
         __open_nwb_files[nwb_file_path] = (io, nwbfile)
```

### Comparing `spyglass-neuro-0.3.4/src/spyglass_neuro.egg-info/PKG-INFO` & `spyglass-neuro-0.4.0/src/spyglass_neuro.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spyglass-neuro
-Version: 0.3.4
+Version: 0.4.0
 Summary: Neuroscience data analysis framework for reproducible research
-Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>
+Author-email: Loren Frank <loren.frank@ucsf.edu>, Kyu Hyun Lee <kyuhyun.lee@ucsf.edu>, Eric Denovellis <eric.denovellis@ucsf.edu>, Ryan Ly <rly@lbl.gov>, Daniel Gramling <daniel.gramling@ucsf.edu>
 License: Copyright (c) 2020-present Loren Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -15,64 +15,28 @@
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/spyglass/issues
 Keywords: neuroscience,research,electrophysiology,reproducible,data analysis,spike sorting,spikeinterface,datajoint,nwb,kachery,sortingview
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.10,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: position
 License-File: LICENSE
 
 [![Import test](https://github.com/LorenFrankLab/spyglass/actions/workflows/workflow.yml/badge.svg)](https://github.com/LorenFrankLab/spyglass/actions/workflows/workflow.yml)
 
 # spyglass
 
 `spyglass` is a data analysis framework that facilitates the storage, analysis, visualization, and sharing of neuroscience data to support reproducible research. It is designed to be interoperable with the NWB format and integrates open-source tools into a coherent framework.
 
 Documentation can be found at - [https://lorenfranklab.github.io/spyglass/](https://lorenfranklab.github.io/spyglass/)
 
-### Installing from pip
+## Installation
 
-Install spyglass
-
-```bash
-pip install spyglass-neuro
-```
-
-Some functions may take advantage of the latest changes to spike interface, which currently has a slow release cycle. To get the latest changes:
-
-```bash
-pip install git+https://github.com/SpikeInterface/spikeinterface.git
-```
-
-The Frank Lab typically uses mountainsort, although spyglass uses spikeinterface, which allows for any spike sorter. To install mountainsort:
-
-```bash
-pip install mountainsort4
-```
-
-Spyglass uses the package `ghostipy` for filtering of signals:
-
-```bash
-pip install ghostipy
-```
-
-WARNING: If you are on an M1 Mac, you need to install pyfftw via conda BEFORE installing ghostipy
-
-```bash
-conda install -c conda-forge pyfftw
-```
-
-Finally, if you want to decode on the GPU, you must install cupy:
-```bash
-conda install -c conda-forge cupy
-```
-
-## Setup
-
-See the documentation for setup instructions - [https://lorenfranklab.github.io/spyglass/type/html/installation.html](https://lorenfranklab.github.io/spyglass/type/html/installation.html)
+For installation instructions see - [https://lorenfranklab.github.io/spyglass/type/html/installation.html](https://lorenfranklab.github.io/spyglass/type/html/installation.html)
 
 ## Tutorials
 
 The tutorials for `spyglass` is currently in the form of Jupyter Notebooks and can be found in the [notebooks](https://github.com/LorenFrankLab/spyglass/tree/master/notebooks) directory. We strongly recommend opening them in the context of `jupyterlab`.
 
 ## Contributing
```

### Comparing `spyglass-neuro-0.3.4/tests/ci_config.py` & `spyglass-neuro-0.4.0/tests/ci_config.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/conftest.py` & `spyglass-neuro-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/data_import/test_insert_sessions.py` & `spyglass-neuro-0.4.0/tests/data_import/test_insert_sessions.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/datajoint/_datajoint_server.py` & `spyglass-neuro-0.4.0/tests/datajoint/_datajoint_server.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/test_insert_beans.py` & `spyglass-neuro-0.4.0/tests/test_insert_beans.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/test_nwb_helper_fn.py` & `spyglass-neuro-0.4.0/tests/test_nwb_helper_fn.py`

 * *Files identical despite different names*

### Comparing `spyglass-neuro-0.3.4/tests/trim_beans.py` & `spyglass-neuro-0.4.0/tests/trim_beans.py`

 * *Files identical despite different names*

