# Comparing `tmp/cftsdata-0.1.1.tar.gz` & `tmp/cftsdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cftsdata-0.1.1.tar", last modified: Thu Feb 23 15:49:23 2023, max compression
+gzip compressed data, was "cftsdata-0.1.2.tar", last modified: Mon May 22 21:42:36 2023, max compression
```

## Comparing `cftsdata-0.1.1.tar` & `cftsdata-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.391490 cftsdata-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.383490 cftsdata-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.387490 cftsdata-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-23 15:49:10.000000 cftsdata-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-23 15:49:10.000000 cftsdata-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-23 15:49:10.000000 cftsdata-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-23 15:49:23.391490 cftsdata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-23 15:49:10.000000 cftsdata-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.387490 cftsdata-0.1.1/cftsdata/
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/abr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/efr.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/iec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/memr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_abr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_abr_gui.enaml
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_efr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_iec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/summarize_memr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-23 15:49:10.000000 cftsdata-0.1.1/cftsdata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.391490 cftsdata-0.1.1/cftsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 15:49:23.000000 cftsdata-0.1.1/cftsdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-23 15:49:10.000000 cftsdata-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:49:23.391490 cftsdata-0.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-02-23 15:49:10.000000 cftsdata-0.1.1/scripts/validate_abr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-23 15:49:10.000000 cftsdata-0.1.1/scripts/validate_dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 15:49:23.391490 cftsdata-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.077678 cftsdata-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.069678 cftsdata-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.069678 cftsdata-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 21:42:26.000000 cftsdata-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 21:42:26.000000 cftsdata-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 21:42:26.000000 cftsdata-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 21:42:36.077678 cftsdata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 21:42:26.000000 cftsdata-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.073678 cftsdata-0.1.2/cftsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/efr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/iec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/memr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/microphone_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_abr_gui.enaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_efr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_iec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_memr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 21:42:35.000000 cftsdata-0.1.2/cftsdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.073678 cftsdata-0.1.2/cftsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-22 21:42:26.000000 cftsdata-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.077678 cftsdata-0.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-22 21:42:26.000000 cftsdata-0.1.2/scripts/validate_abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 21:42:26.000000 cftsdata-0.1.2/scripts/validate_dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:42:36.077678 cftsdata-0.1.2/setup.cfg
```

### Comparing `cftsdata-0.1.1/.github/workflows/publish-to-pypi.yml` & `cftsdata-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/.gitignore` & `cftsdata-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/LICENSE.txt` & `cftsdata-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/PKG-INFO` & `cftsdata-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftsdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight tools for managing CFTS data
 Author-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2022 CFTS development team
```

### Comparing `cftsdata-0.1.1/cftsdata/abr.py` & `cftsdata-0.1.2/cftsdata/abr.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,67 +43,14 @@
     r'\g<experimenter> ' \
     r'\g<animal> ' \
     r'\g<ear> ' \
     r'\g<note> ' \
     r'\g<experiment>*'
 
 
-def cache(f, name=None):
-    import inspect
-    s = inspect.signature(f)
-    if name is None:
-        name = f.__code__.co_name
-
-    @wraps(f)
-    def wrapper(self, *args, bypass_cache=False, refresh_cache=False, **kwargs):
-        if bypass_cache:
-            return f(self, *args, **kwargs)
-
-        cb = kwargs.pop('cb', None)
-
-        bound_args = s.bind(self, *args, **kwargs)
-        bound_args.apply_defaults()
-        cache_kwargs = dict(bound_args.arguments)
-        cache_kwargs.pop('self')
-        cache_kwargs.pop('cb')
-
-        string = json.dumps(cache_kwargs, sort_keys=True, allow_nan=True)
-        uuid = hashlib.sha256(string.encode('utf8')).hexdigest()
-
-        cache_path = self.base_path / 'cache'
-        cache_path.mkdir(parents=True, exist_ok=True)
-        cache_file = cache_path / f'{name}-{uuid}-result.pkl'
-        kwargs_cache_file = cache_path / f'{name}-{uuid}-kwargs.pkl'
-
-        result = None
-        try:
-            if not refresh_cache and cache_file.exists():
-                result = pd.read_pickle(cache_file)
-                with open(kwargs_cache_file, 'rb') as fh:
-                    cache_kwargs = pickle.load(fh)
-                    if cache_kwargs != kwargs:
-                        raise ValueError('Cache is corrupted')
-        except:
-            # Cache is corrupted. Delete it.
-            cache_file.unlink()
-
-        if result is None:
-            result = f(self, *args, cb=cb, **kwargs)
-            try:
-                result.to_pickle(cache_file)
-                with open(kwargs_cache_file, 'wb') as fh:
-                    pickle.dump(kwargs, fh)
-            except OSError:
-                warnings.warn(f'Unable to create cache file at {cache_path}')
-
-        return result
-
-    return wrapper
-
-
 class ABRFile(Recording):
     '''
     Wrapper around an ABR file with methods for loading and querying data
 
     Parameters
     ----------
     base_path : string
@@ -150,15 +97,14 @@
         from the ABR experiment. For simplicity, all parameters beginning with
         `target_tone_` have that string removed. For example,
         `target_tone_frequency` will become `frequency`).
         '''
         data = self.__getattr__('erp_metadata')
         return data.rename(columns=lambda x: x.replace('target_tone_', ''))
 
-    @cache
     def get_epochs(self, offset=0, duration=8.5e-3, detrend='constant',
                    downsample=None, reject_threshold=None,
                    reject_mode='absolute', columns='auto', averages=None,
                    cb=None):
         '''
         Extract event-related epochs from EEG
 
@@ -170,15 +116,14 @@
         fn = self.eeg.get_epochs
         result = fn(self.erp_metadata, offset, duration, detrend,
                     downsample=downsample, columns=columns, cb=cb)
         result = self._apply_reject(result, reject_threshold, reject_mode)
         result = self._apply_n(result, averages)
         return result
 
-    @cache
     def get_random_segments(self, n, offset=0, duration=8.5e-3,
                             detrend='constant', downsample=None,
                             reject_threshold=None, reject_mode='absolute'):
         '''
         Extract random segments from filtered EEG
 
         Parameters
@@ -187,15 +132,14 @@
             Number of segments to return
         {common_docstring}
         '''
         fn = self.eeg.get_random_segments
         result = fn(n, offset, duration, detrend, downsample=downsample)
         return self._apply_reject(result, reject_threshold, reject_mode)
 
-    @cache
     def get_epochs_filtered(self, filter_lb=300, filter_ub=3000,
                             filter_order=1, offset=-1e-3, duration=10e-3,
                             detrend='constant', pad_duration=10e-3,
                             downsample=None, reject_threshold=None,
                             reject_mode='absolute', columns='auto',
                             averages=None, cb=None):
         '''
@@ -213,15 +157,14 @@
                     filter_order=filter_order, detrend=detrend,
                     pad_duration=pad_duration, downsample=downsample,
                     columns=columns, cb=cb)
         result = self._apply_reject(result, reject_threshold, reject_mode)
         result = self._apply_n(result, averages)
         return result
 
-    @cache
     def get_random_segments_filtered(self, n, filter_lb=300, filter_ub=3000,
                                      filter_order=1, offset=-1e-3,
                                      duration=10e-3, detrend='constant',
                                      pad_duration=10e-3,
                                      downsample=None,
                                      reject_threshold=None,
                                      reject_mode='absolute'):
@@ -430,20 +373,14 @@
             Columns to include
         averages : None
             Limits the number of epochs returned to the number of averages
             specified. If None, use the value stored in the file. Otherwise,
             use the provided value. To return all epochs, use `np.inf`. For
             dual-polarity data, care will be taken to ensure the number of
             trials from each polarity match (even when set to `np.inf`).
-        bypass_cache : bool
-            If true, skip cache mechanism entirely. This also prevents a cache
-            file from being saved.
-        refresh_cache : bool
-            If true, recompute from raw EEG data. If false and data has already
-            been cached, return cached results.
 '''.strip()
 
 
 def format_docstrings(klass):
     fmt = {
         'common_docstring': common_docstring,
         'filter_docstring': filter_docstring,
```

### Comparing `cftsdata-0.1.1/cftsdata/dpoae.py` & `cftsdata-0.1.2/cftsdata/dpoae.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/efr.py` & `cftsdata-0.1.2/cftsdata/efr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 from psidata.api import Recording
 
 
 class EFR(Recording):
 
     def __init__(self, filename, setting_table='analyze_efr_metadata'):
         super().__init__(filename, setting_table)
+        self.efr_type = 'ram' if self.base_path.stem.endswith('ram') else 'sam'
 
     def _get_epochs(self, signal):
         duration = self.get_setting('duration')
         offset = 0
         result = signal.get_epochs(self.analyze_efr_metadata, offset, duration)
-        return result.reset_index(['target_sam_tone_fc', 'target_sam_tone_fm'],
-                                  drop=True)
+        print(result)
+        if self.efr_type == 'sam':
+            to_drop = ['target_sam_tone_fc', 'target_sam_tone_fm']
+            return result.reset_index(to_drop, drop=True)
+        else:
+            to_drop = ['target_mod_fm', 'target_tone_frequency', 'target_mod_duty_cycle']
+        return result.reset_index(to_drop, drop=True)
 
     @property
     def mic(self):
         return self.system_microphone
 
     def get_eeg_epochs(self):
         return self._get_epochs(self.eeg)
 
     def get_mic_epochs(self):
         return self._get_epochs(self.mic)
+
+    @property
+    def level(self):
+        if self.efr_type == 'ram':
+            return self.get_setting('target_tone_level')
+        else:
+            return self.get_setting('target_sam_tone_level')
```

### Comparing `cftsdata-0.1.1/cftsdata/memr.py` & `cftsdata-0.1.2/cftsdata/memr.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/postprocess.py` & `cftsdata-0.1.2/cftsdata/postprocess.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/summarize_abr.py` & `cftsdata-0.1.2/cftsdata/summarize_abr.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import json
 from pathlib import Path
 import matplotlib.pyplot as plt
 
 import numpy as np
 import pandas as pd
 
-from psi import get_config
 from psiaudio.plot import waterfall_plot
 
 from . import abr
 
 from .util import add_default_options, DatasetManager, process_files
 
 
@@ -125,16 +124,19 @@
     return epochs.groupby(levels, group_keys=False).apply(number_trials)
 
 
 def plot_waveforms_cb(epochs_mean, filename, name):
     epochs_mean = epochs_mean.reset_index(['epoch_n', 'epoch_reject_ratio'], drop=True)
     grouped = epochs_mean.groupby('frequency')
     n_panels = len(grouped)
-    figure, axes = plt.subplots(1, n_panels, figsize=(6*n_panels, 8.5))
-    for ax, (frequency, data) in zip(axes, grouped):
+    # Normally we want a 1D array of axes, but we have to disable squeezing
+    # because if n_panels is 1, then we end up with an axes instead of a 1D
+    # array of axes. So, we get a 2D array and then extract the first row.
+    figure, axes = plt.subplots(1, n_panels, figsize=(6*n_panels, 8.5), squeeze=False)
+    for ax, (frequency, data) in zip(axes[0], grouped):
         waterfall_plot(ax, data)
         ax.set_xlabel('Time (msec)')
         ax.set_title(f'{frequency * 1e-3:0.2f} Hz')
     figure.suptitle(name)
     figure.savefig(filename)
 
 
@@ -244,89 +246,87 @@
 
     if not reprocess and manager.is_processed(files):
         return
 
     # Load the epochs. The callbacks for loading the epochs return a value in
     # the range 0 ... 1. Since this only represents "half" the total work we
     # need to do, rescale to the range 0 ... 0.5.
-    cb = manager.create_cb(cb)
-    cb(0)
+    with manager.create_cb(cb) as cb:
+        def cb_rescale(frac):
+            nonlocal cb
+            cb(frac * 0.5)
+
+        epochs = _get_epochs(fh, offset + latency_correction, duration,
+                            filter_settings, cb=cb_rescale, downsample=downsample)
+
+        if gain_correction != 1:
+            epochs = epochs * gain_correction
+
+        if latency_correction != 0:
+            new_idx = [(*r[:-1], r[-1] - latency_correction) for r in epochs.index]
+            new_idx = pd.MultiIndex.from_tuples(new_idx, names=epochs.index.names)
+            new_col = epochs.columns - latency_correction
+            epochs = pd.DataFrame(epochs.values, index=new_idx, columns=new_col)
+
+        if debug_mode:
+            return epochs
+
+        # Apply the reject
+        reject_threshold = fh.get_setting('reject_threshold')
+        m = np.abs(epochs) < reject_threshold
+        m = m.all(axis=1)
+        epochs = epochs.loc[m]
+
+        cb(0.6)
+        if n_epochs is not None:
+            n = int(np.floor(n_epochs / 2))
+            epochs = epochs.groupby(COLUMNS, group_keys=False) \
+                .apply(lambda x: x.iloc[:n])
+        cb(0.7)
+
+        epoch_mean = epochs.groupby(COLUMNS).mean().groupby(COLUMNS[:-1]).mean()
+
+        epoch_reject_ratio = 1-m.groupby(COLUMNS[:-1]).mean()
+        epoch_n = epochs.groupby(COLUMNS[:-1]).size()
+        epoch_info = pd.DataFrame({
+            'epoch_n': epoch_n,
+            'epoch_reject_ratio': epoch_reject_ratio,
+        })
+        if not np.all(epoch_mean.index == epoch_info.index):
+            raise ValueError('Programming issue. Please contact developer.')
+
+        # Merge in the N and reject ratio into the index for epoch_mean
+        epoch_info = epoch_info.set_index(['epoch_n', 'epoch_reject_ratio'],
+                                        append=True)
+        epoch_mean.index = epoch_info.index
+        epoch_mean.columns.name = 'time'
+
+        manager.get_proc_filename('processing settings.json') \
+            .write_text(json.dumps(settings, indent=2))
+        manager.get_proc_filename('experiment settings.json') \
+            .write_text(json.dumps(md, indent=2))
+
+        epoch_mean.T.to_csv(manager.get_proc_filename('average waveforms.csv'))
+        cb(0.8)
+
+        if export_single_trial:
+            epochs = add_trial(epochs)
+            epochs.columns.name = 'time'
+            epochs.T.to_csv(manager.get_proc_filename('individual waveforms.csv'))
+
+        cb(0.9)
+        if plot_waveforms_cb is not None:
+            plot_waveforms_cb(
+                epoch_mean,
+                manager.get_proc_filename('waveforms.pdf'),
+                filename.stem
+            )
 
-    def cb_rescale(frac):
-        nonlocal cb
-        cb(frac * 0.5)
-
-    epochs = _get_epochs(fh, offset + latency_correction, duration,
-                         filter_settings, cb=cb_rescale, downsample=downsample)
-
-    if gain_correction != 1:
-        epochs = epochs * gain_correction
-
-    if latency_correction != 0:
-        new_idx = [(*r[:-1], r[-1] - latency_correction) for r in epochs.index]
-        new_idx = pd.MultiIndex.from_tuples(new_idx, names=epochs.index.names)
-        new_col = epochs.columns - latency_correction
-        epochs = pd.DataFrame(epochs.values, index=new_idx, columns=new_col)
-
-    if debug_mode:
-        return epochs
-
-    # Apply the reject
-    reject_threshold = fh.get_setting('reject_threshold')
-    m = np.abs(epochs) < reject_threshold
-    m = m.all(axis=1)
-    epochs = epochs.loc[m]
-
-    cb(0.6)
-    if n_epochs is not None:
-        n = int(np.floor(n_epochs / 2))
-        epochs = epochs.groupby(COLUMNS, group_keys=False) \
-            .apply(lambda x: x.iloc[:n])
-    cb(0.7)
-
-    epoch_mean = epochs.groupby(COLUMNS).mean().groupby(COLUMNS[:-1]).mean()
-
-    epoch_reject_ratio = 1-m.groupby(COLUMNS[:-1]).mean()
-    epoch_n = epochs.groupby(COLUMNS[:-1]).size()
-    epoch_info = pd.DataFrame({
-        'epoch_n': epoch_n,
-        'epoch_reject_ratio': epoch_reject_ratio,
-    })
-    if not np.all(epoch_mean.index == epoch_info.index):
-        raise ValueError('Programming issue. Please contact developer.')
-
-    # Merge in the N and reject ratio into the index for epoch_mean
-    epoch_info = epoch_info.set_index(['epoch_n', 'epoch_reject_ratio'],
-                                      append=True)
-    epoch_mean.index = epoch_info.index
-    epoch_mean.columns.name = 'time'
-
-    manager.get_proc_filename('processing settings.json') \
-        .write_text(json.dumps(settings, indent=2))
-    manager.get_proc_filename('experiment settings.json') \
-        .write_text(json.dumps(md, indent=2))
-
-    epoch_mean.T.to_csv(manager.get_proc_filename('average waveforms.csv'))
-    cb(0.8)
-
-    if export_single_trial:
-        epochs = add_trial(epochs)
-        epochs.columns.name = 'time'
-        epochs.T.to_csv(manager.get_proc_filename('individual waveforms.csv'))
-
-    cb(0.9)
-    if plot_waveforms_cb is not None:
-        plot_waveforms_cb(
-            epoch_mean,
-            manager.get_proc_filename('waveforms.pdf'),
-            filename.stem
-        )
-
-    cb(1.0)
-    return True
+        cb(1.0)
+        plt.close('all')
 
 
 def main_file():
     parser = argparse.ArgumentParser('Filter and summarize ABR data')
 
     parser.add_argument('filenames', type=str,
                         help='Filename', nargs='+')
```

### Comparing `cftsdata-0.1.1/cftsdata/summarize_abr_gui.enaml` & `cftsdata-0.1.2/cftsdata/summarize_abr_gui.enaml`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/summarize_dpoae.py` & `cftsdata-0.1.2/cftsdata/summarize_dpoae.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,148 +80,154 @@
 
 
 def process_file(filename, cb, reprocess=False):
     manager = DatasetManager(filename)
     if not reprocess and manager.is_processed('io.csv'):
         return
     manager.clear()
-    cb = manager.create_cb(cb)
-
-    cb(0)
-    fh = DPOAEFile(filename)
-    fs = fh.system_microphone.fs
-    ramp_time = fh.get_setting('primary_tone_rise_time')
-    n_time = fh.get_setting('n_time')
-    n_fft = fh.get_setting('n_fft')
-    window = fh.get_setting('response_window')
-    f2_f1_ratio = fh.get_setting('f2_f1_ratio')
-
-    n_window = window * fs
-    n_trim = (ramp_time * 4) * fs
-    if int(n_window) != n_window:
-        raise ValueError('n_window is not an integer')
-    if int(n_trim) != n_trim:
-        raise ValueError('n_trim is not an integer')
-    n_trim = int(n_trim)
-    n_window = int(n_window)
-    resolution = fs / n_window
-
-    step = 25e-3
-    n_step = int(step * fs)
-
-    cal = fh.system_microphone.get_calibration()
-
-    psd = {}
-    measured = {}
-    f2_prev = None
-    for i, row in fh.results.iterrows():
-        cb(i / len(fh.results))
-        lb = row['dp_start']
-        ub = row['dp_end']
-        f2 = row['f2_frequency']
-        f1 = row['f1_frequency']
-        l2 = row['f2_level']
-        dp = 2 * f1 - f2
-        nf_freq = np.array([-2, -1, 1, 2]) * resolution + dp
-
-        s = fh.system_microphone.get_segment(lb, 0, ub-lb, allow_partial=True)
-        s = s.values[n_trim:]
-
-        m_set = []
-        p_set = []
-        for i in range(1):
-            n_segments, n_left = divmod(s.shape[-1], n_window)
-            s_segmented = s[:-n_left].reshape((n_segments, -1))
-            m = np.isfinite(s_segmented).all(axis=1)
-            s_segmented = s_segmented[m]
-            p = cal.get_db(util.psd_df(s_segmented.mean(axis=0), fs))
-            s = s[n_step:]
-
-            p_set.append(p)
-            m_set.append({
-                'f1_level': p[f1],
-                'f2_level': p[f2],
-                'dp_level': p[dp],
-                'dp_nf': p[nf_freq].mean(),
-                'online_dp_level': row['meas_dpoae_level'],
-                'online_dp_nf': row['dpoae_noise_floor'],
-            })
-        measured[f2, l2] = pd.DataFrame(m_set).mean(axis=0)
-        psd[f2, l2] = pd.DataFrame(p_set).mean(axis=0)
-
-    freq = fh.results['f2_frequency'].unique()
-    level = fh.results['f2_level'].unique()
-    n_freq = len(freq)
-    n_level = len(level)
-
-    measured = pd.DataFrame(
-        measured.values(),
-        index=pd.MultiIndex.from_tuples(measured.keys(), names=['f2', 'l2'])
-    )
-
-    figure, axes = plt.subplots(2, n_freq, figsize=(4 * n_freq, 8), sharex=True, sharey=True)
-    for fi, f2 in enumerate(freq):
-        col = axes[:, fi]
-        m = measured.loc[f2]
-
-        ax = col[0]
-        ax.axhline(0, ls='-', color='k')
-        ax.plot(m['f2_level'], marker='o', color='0.5')
-        ax.plot(m['f1_level'], marker='o', color='k')
-        ax.plot(m['dp_level'], marker='o', color='darkturquoise')
-        ax.plot(m['dp_nf'], marker='x', color='lightblue')
-        ax.set_title(f'{f2} Hz')
-        ax.grid()
-
-        ax = col[1]
-        ax.axhline(0, ls='-', color='k')
-        ax.plot(m['f2_level'], marker='o', color='0.5')
-        ax.plot(m['f1_level'], marker='o', color='k')
-        ax.plot(m['online_dp_level'], marker='o', color='darkorange')
-        ax.plot(m['online_dp_nf'], marker='x', color='coral')
-        ax.grid()
-        ax.set_xlabel('F2 level (dB SPL)')
-
-    for ax in axes[:, 0]:
-        ax.set_ylabel('Measured level (dB SPL)')
-
-    manager.save_fig(figure, 'io.pdf')
-
-    figure, axes = plt.subplots(n_level, n_freq, figsize=(4 * n_freq, 4 * n_level), sharex=True, sharey=True)
-    for fi, f2 in enumerate(freq):
-        for li, l2 in enumerate(level[::-1]):
-            ax = axes[li, fi]
-            f1 = f2 / f2_f1_ratio
+    with manager.create_cb(cb) as cb:
+        fh = DPOAEFile(filename)
+        fs = fh.system_microphone.fs
+        ramp_time = fh.get_setting('primary_tone_rise_time')
+        n_time = fh.get_setting('n_time')
+        n_fft = fh.get_setting('n_fft')
+        window = fh.get_setting('response_window')
+        f2_f1_ratio = fh.get_setting('f2_f1_ratio')
+
+        n_window = window * fs
+        n_trim = (ramp_time * 4) * fs
+        if int(n_window) != n_window:
+            raise ValueError('n_window is not an integer')
+        if int(n_trim) != n_trim:
+            raise ValueError('n_trim is not an integer')
+        n_trim = int(n_trim)
+        n_window = int(n_window)
+        resolution = fs / n_window
+
+        step = 25e-3
+        n_step = int(step * fs)
+
+        cal = fh.system_microphone.get_calibration()
+
+        psd = {}
+        measured = {}
+        f2_prev = None
+        for i, row in fh.results.iterrows():
+            cb(i / len(fh.results))
+            lb = row['dp_start']
+            ub = row['dp_end']
+
+            if ub < lb:
+                log.warning('Incomplete DPOAE segment')
+                continue
+
+            f2 = row['f2_frequency']
+            f1 = row['f1_frequency']
+            l2 = row['f2_level']
             dp = 2 * f1 - f2
-            ax.axvline(f2, lw=2, color='lightblue')
-            ax.axvline(f1, lw=2, color='lightblue')
-            ax.axvline(dp, lw=2, color='darkturquoise')
-            ax.axhline(0, lw=2, color='0.5')
-            ax.plot(psd[f2, l2].iloc[1:], color='k')
-
-    min_freq = min(2 * (freq / f2_f1_ratio) - freq)
-    max_freq = max(freq)
-    axes[0, 0].axis(xmin=min_freq * 0.8, xmax=max_freq / 0.8)
-    axes[0, 0].set_xscale('octave')
-
-    for ax in axes[-1]:
-        ax.set_xlabel('Frequency (kHz)')
-    for ax in axes[:, 0]:
-        ax.set_xlabel('PSD (dB)')
+            nf_freq = np.array([-2, -1, 1, 2]) * resolution + dp
 
-    manager.save_fig(figure, 'mic spectrum.pdf')
+            s = fh.system_microphone.get_segment(lb, 0, ub-lb, allow_partial=True)
+            s = s.values[n_trim:]
 
-    manager.save_dataframe(measured, 'io.csv')
+            m_set = []
+            p_set = []
+            for i in range(1):
+                n_segments, n_left = divmod(s.shape[-1], n_window)
+                if n_left != 0:
+                    s = s[:-n_left]
+                s_segmented = s.reshape((n_segments, -1))
+                m = np.isfinite(s_segmented).all(axis=1)
+                s_segmented = s_segmented[m]
+                p = cal.get_db(util.psd_df(s_segmented.mean(axis=0), fs))
+                s = s[n_step:]
+
+                p_set.append(p)
+                m_set.append({
+                    'f1_level': p[f1],
+                    'f2_level': p[f2],
+                    'dp_level': p[dp],
+                    'dp_nf': p[nf_freq].mean(),
+                    'online_dp_level': row['meas_dpoae_level'],
+                    'online_dp_nf': row['dpoae_noise_floor'],
+                })
+            measured[f2, l2] = pd.DataFrame(m_set).mean(axis=0)
+            psd[f2, l2] = pd.DataFrame(p_set).mean(axis=0)
+
+        freq = fh.results['f2_frequency'].unique()
+        level = fh.results['f2_level'].unique()
+        n_freq = len(freq)
+        n_level = len(level)
+
+        measured = pd.DataFrame(
+            measured.values(),
+            index=pd.MultiIndex.from_tuples(measured.keys(), names=['f2', 'l2'])
+        )
+
+        figure, axes = plt.subplots(2, n_freq, figsize=(4 * n_freq, 8),
+                                    sharex=True, sharey=True, squeeze=False)
+        for fi, f2 in enumerate(freq):
+            col = axes[:, fi]
+            m = measured.loc[f2]
+
+            ax = col[0]
+            ax.axhline(0, ls='-', color='k')
+            ax.plot(m['f2_level'], marker='o', color='0.5')
+            ax.plot(m['f1_level'], marker='o', color='k')
+            ax.plot(m['dp_level'], marker='o', color='darkturquoise')
+            ax.plot(m['dp_nf'], marker='x', color='lightblue')
+            ax.set_title(f'{f2} Hz')
+            ax.grid()
+
+            ax = col[1]
+            ax.axhline(0, ls='-', color='k')
+            ax.plot(m['f2_level'], marker='o', color='0.5')
+            ax.plot(m['f1_level'], marker='o', color='k')
+            ax.plot(m['online_dp_level'], marker='o', color='darkorange')
+            ax.plot(m['online_dp_nf'], marker='x', color='coral')
+            ax.grid()
+            ax.set_xlabel('F2 level (dB SPL)')
+
+        for ax in axes[:, 0]:
+            ax.set_ylabel('Measured level (dB SPL)')
+
+        manager.save_fig(figure, 'io.pdf')
+
+        figure, axes = plt.subplots(n_level, n_freq,
+                                    figsize=(4 * n_freq, 4 * n_level),
+                                    sharex=True, sharey=True, squeeze=False)
+        for fi, f2 in enumerate(freq):
+            for li, l2 in enumerate(level[::-1]):
+                ax = axes[li, fi]
+                f1 = f2 / f2_f1_ratio
+                dp = 2 * f1 - f2
+                ax.axvline(f2, lw=2, color='lightblue')
+                ax.axvline(f1, lw=2, color='lightblue')
+                ax.axvline(dp, lw=2, color='darkturquoise')
+                ax.axhline(0, lw=2, color='0.5')
+                try:
+                    ax.plot(psd[f2, l2].iloc[1:], color='k')
+                except KeyError:
+                    pass
+
+        min_freq = min(2 * (freq / f2_f1_ratio) - freq)
+        max_freq = max(freq)
+        axes[0, 0].axis(xmin=min_freq * 0.8, xmax=max_freq / 0.8)
+        axes[0, 0].set_xscale('octave')
+
+        for ax in axes[-1]:
+            ax.set_xlabel('Frequency (kHz)')
+        for ax in axes[:, 0]:
+            ax.set_xlabel('PSD (dB)')
+
+        manager.save_fig(figure, 'mic spectrum.pdf')
+        manager.save_dataframe(measured, 'io.csv')
+        plt.close('all')
 
 
 def main_folder():
     import argparse
     parser = argparse.ArgumentParser('Summarize DPOAE IO data in folder')
     add_default_options(parser)
     args = parser.parse_args()
     process_files(args.folder, '**/*dpoae_io*',
                   process_file, reprocess=args.reprocess)
-
-
-if __name__ == '__main__':
-    cb = lambda x: x
-    process_file('c:/users/mmm/projects/psi1/data/data/20230127-122543 Sean Sean left 151122 1 dpoae_io.zip', cb)
```

### Comparing `cftsdata-0.1.1/cftsdata/summarize_iec.py` & `cftsdata-0.1.2/cftsdata/summarize_iec.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/summarize_memr.py` & `cftsdata-0.1.2/cftsdata/summarize_memr.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/cftsdata/util.py` & `cftsdata-0.1.2/cftsdata/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,72 @@
 import os
 from pathlib import Path
 
-from psi import get_config
-DATA_ROOT = get_config('DATA_ROOT')
-PROCESSED_ROOT = get_config('PROCESSED_ROOT')
 
+class CallbackManager:
 
-def get_cb(cb):
+    def __init__(self, cb):
+        self._cb = cb
+
+    def __enter__(self):
+        self._cb(0)
+        return self
+
+    def __call__(self, value):
+        return self._cb(value)
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        self._cb(1)
+
+
+def get_cb(cb, suffix=None):
     # Define the callback as a no-op if not provided or sets up tqdm if requested.
     if cb is None:
         cb = lambda x: x
     elif cb == 'tqdm':
         from tqdm import tqdm
-        pbar = tqdm(total=100, bar_format='{l_bar}{bar}[{elapsed}<{remaining}]')
+        mesg = '{l_bar}{bar}[{elapsed}<{remaining}]'
+        if suffix is not None:
+            mesg = mesg + ' ' + suffix
+        pbar = tqdm(total=100, bar_format=mesg)
         def cb(frac):
             nonlocal pbar
             frac *= 100
             pbar.update(frac - pbar.n)
             if frac == 100:
                 pbar.close()
     else:
         raise ValueError(f'Unsupported callback: {cb}')
     return cb
 
 
 def add_default_options(parser):
-    parser.add_argument('-f', '--folder', type=str, help='Folder containing data', default=DATA_ROOT)
+    parser.add_argument('folder', type=str, help='Folder containing data')
     parser.add_argument('--reprocess', action='store_true', help='Reprocess all data in folder')
 
 
 def process_files(folder, glob_pattern, fn, cb='tqdm', reprocess=False,
                   halt_on_error=True):
     success = []
     errors = []
     for filename in Path(folder).glob(glob_pattern):
         if filename.suffix == '.md5':
             continue
         try:
             fn(filename, cb=cb, reprocess=reprocess)
             success.append(filename)
+        except KeyboardInterrupt:
+            # Don't capture this otherwise it just keeps continuing with the
+            # next file.
+            raise
         except Exception as e:
             if halt_on_error:
                 raise
             errors.append((filename, e))
+            print(f'Error processing {filename}')
     print(f'Successfully processed {len(success)} files with {len(errors)} errors')
 
 
 def add_trial(df, grouping):
     def _add_trial(df):
         df['trial'] = range(len(df))
         return df.set_index('trial', append=True)
@@ -66,38 +86,41 @@
                           names=['freq', 'SPL', 'phase'])
     return InterpCalibration.from_spl(cal['freq'], cal['SPL'],
                                       phase=cal['phase'])
 
 
 class DatasetManager:
 
-    def __init__(self, path, raw_dir=DATA_ROOT, proc_dir=PROCESSED_ROOT,
-                 file_template=None):
+    def __init__(self, path, raw_dir=None, proc_dir=None, file_template=None):
         '''
         Manages paths of processed files given the relative path between the
         raw and processed directory structure.
 
         Parameters
         ----------
-        raw_dir : {str, Path}
+        raw_dir : {None, str, Path}
             Base path containing raw data
-        proc_dir : {str, Path}
+        proc_dir : {None, str, Path}
             Base path containing processed data
         file_template : {None, str}
             If None, defaults to the filename stem
         '''
+        if raw_dir is None:
+            raw_dir = os.environ.get('RAW_DATA_DIR', None)
+        if proc_dir is None:
+            proc_dir = os.environ.get('PROC_DATA_DIR', None)
         self.path = Path(path)
         self.raw_dir = Path(raw_dir)
         self.proc_dir = Path(proc_dir)
         if file_template is None:
             file_template = f'{self.path.stem}'
         self.file_template = file_template
 
     def create_cb(self, cb):
-        return get_cb(cb)
+        return CallbackManager(get_cb(cb, self.path.stem))
 
     def get_proc_path(self):
         return self.proc_dir / self.path.parent.relative_to(self.raw_dir) / self.path.stem
 
     def get_proc_filename(self, suffix, mkdir=True):
         proc_path = self.get_proc_path()
         proc_path.mkdir(exist_ok=True, parents=True)
@@ -115,10 +138,12 @@
         filename = self.get_proc_filename(suffix)
         figure.savefig(filename, bbox_inches='tight')
 
     def save_dataframe(self, df, suffix):
         filename = self.get_proc_filename(suffix)
         df.to_csv(filename)
 
+    save_df = save_dataframe
+
     def clear(self):
         for filename in self.get_proc_path().iterdir():
             filename.unlink()
```

### Comparing `cftsdata-0.1.1/cftsdata.egg-info/PKG-INFO` & `cftsdata-0.1.2/cftsdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftsdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight tools for managing CFTS data
 Author-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2022 CFTS development team
```

### Comparing `cftsdata-0.1.1/cftsdata.egg-info/SOURCES.txt` & `cftsdata-0.1.2/cftsdata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .gitignore
 LICENSE.txt
 README.md
 pyproject.toml
 .github/workflows/publish-to-pypi.yml
+cftsdata/__init__.py
 cftsdata/abr.py
 cftsdata/dpoae.py
 cftsdata/efr.py
 cftsdata/iec.py
 cftsdata/memr.py
+cftsdata/microphone_calibration.py
 cftsdata/postprocess.py
 cftsdata/summarize_abr.py
 cftsdata/summarize_abr_gui.enaml
 cftsdata/summarize_dpoae.py
 cftsdata/summarize_efr.py
 cftsdata/summarize_iec.py
 cftsdata/summarize_memr.py
```

### Comparing `cftsdata-0.1.1/pyproject.toml` & `cftsdata-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/scripts/validate_abr.py` & `cftsdata-0.1.2/scripts/validate_abr.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.1/scripts/validate_dpoae.py` & `cftsdata-0.1.2/scripts/validate_dpoae.py`

 * *Files identical despite different names*

