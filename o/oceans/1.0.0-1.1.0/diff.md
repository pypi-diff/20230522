# Comparing `tmp/oceans-1.0.0.tar.gz` & `tmp/oceans-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceans-1.0.0.tar", last modified: Fri Mar 10 21:19:58 2023, max compression
+gzip compressed data, was "oceans-1.1.0.tar", last modified: Mon May 22 13:19:38 2023, max compression
```

## Comparing `oceans-1.0.0.tar` & `oceans-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.182378 oceans-1.0.0/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1987 2023-03-03 16:45:47.000000 oceans-1.0.0/CHANGES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1487 2023-03-03 16:45:47.000000 oceans-1.0.0/LICENSE.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      302 2023-03-03 16:46:15.000000 oceans-1.0.0/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2627 2023-03-10 21:19:58.182378 oceans-1.0.0/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      561 2023-03-03 16:46:15.000000 oceans-1.0.0/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.178378 oceans-1.0.0/oceans/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    11855 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/RPSstuff.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       91 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/__init__.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.178378 oceans-1.0.0/oceans/cmap_data/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      896 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/cbathy.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3584 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/coolavhrrmap.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      924 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/ctopo.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1582 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/odv.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3556 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/redblue_dark.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1316 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/redblue_light.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3570 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/redgreen.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3570 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/cmap_data/rscolmap.dat
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4140 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/colormaps.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    10485 2023-03-10 21:19:08.000000 oceans-1.0.0/oceans/datasets.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    20140 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/filters.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21378 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/ocfis.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    12006 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/plotting.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.178378 oceans-1.0.0/oceans/sandbox/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.178378 oceans-1.0.0/oceans/sandbox/data/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    19192 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/sandbox/data/testdata.npz
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     7259 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/sandbox/lines.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.182378 oceans-1.0.0/oceans/sw_extras/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      784 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/sw_extras/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    17317 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/sw_extras/gamma_GP_from_SP_pt.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    29750 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/sw_extras/sw_extras.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4934 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/sw_extras/waves.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2839 2023-03-03 16:46:15.000000 oceans-1.0.0/oceans/synop.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1072 2023-03-03 16:45:47.000000 oceans-1.0.0/oceans/utilities.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-03-10 21:19:58.182378 oceans-1.0.0/oceans.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      689 2023-03-10 21:19:58.000000 oceans-1.0.0/oceans.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1777 2023-03-03 16:46:15.000000 oceans-1.0.0/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      120 2023-03-10 21:19:08.000000 oceans-1.0.0/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       77 2023-03-10 21:19:08.000000 oceans-1.0.0/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2023-03-10 21:19:58.182378 oceans-1.0.0/setup.cfg
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1987 2023-03-03 16:45:47.000000 oceans-1.1.0/CHANGES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1487 2023-03-03 16:45:47.000000 oceans-1.1.0/LICENSE.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      302 2023-03-03 16:46:15.000000 oceans-1.1.0/MANIFEST.in
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2889 2023-05-22 13:19:38.607519 oceans-1.1.0/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      561 2023-03-03 16:46:15.000000 oceans-1.1.0/README.md
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    11855 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/RPSstuff.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       91 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/__init__.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans/cmap_data/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      896 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/cbathy.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3584 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/coolavhrrmap.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      924 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/ctopo.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1582 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/odv.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3556 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/redblue_dark.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1316 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/redblue_light.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3570 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/redgreen.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3570 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/cmap_data/rscolmap.dat
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     4140 2023-05-22 12:55:46.000000 oceans-1.1.0/oceans/colormaps.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    10511 2023-05-22 13:12:10.000000 oceans-1.1.0/oceans/datasets.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    21078 2023-05-22 13:12:10.000000 oceans-1.1.0/oceans/filters.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    21392 2023-05-22 13:12:10.000000 oceans-1.1.0/oceans/ocfis.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    12007 2023-05-22 13:12:10.000000 oceans-1.1.0/oceans/plotting.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans/sandbox/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans/sandbox/data/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    19192 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/sandbox/data/testdata.npz
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     7259 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/sandbox/lines.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans/sw_extras/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      784 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/sw_extras/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    17317 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/sw_extras/gamma_GP_from_SP_pt.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    29750 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/sw_extras/sw_extras.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     4934 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/sw_extras/waves.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2839 2023-03-03 16:46:15.000000 oceans-1.1.0/oceans/synop.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1072 2023-03-03 16:45:47.000000 oceans-1.1.0/oceans/utilities.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-05-22 13:19:38.607519 oceans-1.1.0/oceans.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      689 2023-05-22 13:19:38.000000 oceans-1.1.0/oceans.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2284 2023-05-22 13:12:10.000000 oceans-1.1.0/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      120 2023-03-10 21:19:08.000000 oceans-1.1.0/requirements-dev.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       77 2023-03-10 21:19:08.000000 oceans-1.1.0/requirements.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2023-05-22 13:19:38.607519 oceans-1.1.0/setup.cfg
```

### Comparing `oceans-1.0.0/CHANGES.txt` & `oceans-1.1.0/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/LICENSE.txt` & `oceans-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/PKG-INFO` & `oceans-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: oceans
-Version: 1.0.0
+Version: 1.1.0
 Summary: Misc functions for oceanographic data analysis
-Author: André Palóczy, Arnaldo Russo, Filipe Fernandes
+Maintainer: André Palóczy, Arnaldo Russo, Filipe Fernandes
 License: Copyright (c) 2016, Filipe Fernandes
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         
@@ -15,14 +15,19 @@
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: documentation, https://pyoceans.github.io/python-oceans/
 Project-URL: homepage, https://pypi.python.org/pypi/oceans/
 Project-URL: repository, https://github.com/pyoceans/python-oceans
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 License-File: LICENSE.txt
 
 [![PyPI Package](https://img.shields.io/pypi/v/oceans.svg)](https://pypi.org/project/oceans/)
 [![Tests](https://github.com/pyoceans/python-oceans/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/pyoceans/python-oceans/actions/workflows/tests.yml)
```

### Comparing `oceans-1.0.0/README.md` & `oceans-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/RPSstuff.py` & `oceans-1.1.0/oceans/RPSstuff.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/cbathy.dat` & `oceans-1.1.0/oceans/cmap_data/cbathy.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/coolavhrrmap.dat` & `oceans-1.1.0/oceans/cmap_data/coolavhrrmap.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/ctopo.dat` & `oceans-1.1.0/oceans/cmap_data/ctopo.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/odv.dat` & `oceans-1.1.0/oceans/cmap_data/odv.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/redblue_dark.dat` & `oceans-1.1.0/oceans/cmap_data/redblue_dark.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/redblue_light.dat` & `oceans-1.1.0/oceans/cmap_data/redblue_light.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/redgreen.dat` & `oceans-1.1.0/oceans/cmap_data/redgreen.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/cmap_data/rscolmap.dat` & `oceans-1.1.0/oceans/cmap_data/rscolmap.dat`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/colormaps.py` & `oceans-1.1.0/oceans/colormaps.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/datasets.py` & `oceans-1.1.0/oceans/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     v = _woa_variable(variable)
 
     if variable not in ["salinity", "temperature"]:
         pref = "woa09"
         warnings.warn(
             f'The variable "{variable}" is only available at 1 degree resolution, '
             f'annual time period, and "{pref}".',
+            stacklevel=2,
         )
         return f"{base}/" f"{pref}/" f"{variable}_annual_1deg.nc"
     else:
         dddd = "decav"
         pref = "woa18"
 
     grids = {
```

### Comparing `oceans-1.0.0/oceans/filters.py` & `oceans-1.1.0/oceans/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -460,15 +460,15 @@
         raise ValueError(msg(xin.ndim))
 
     xout = np.zeros_like(xin) + np.NaN
 
     Lwing = (L - 1) // 2
 
     # NOTE: Use np.ndenumerate in case I expand to +1D case
-    for i, xi in enumerate(xin):
+    for i, _xi in enumerate(xin):
         if i < Lwing:  # Left boundary.
             xout[i] = np.median(xin[0 : i + Lwing + 1])  # (0 to i + Lwing)
         elif i >= N - Lwing:  # Right boundary.
             xout[i] = np.median(xin[i - Lwing : N])  # (i-Lwing to N-1)
         else:  # Middle (N-2*Lwing input vector and filter window overlap).
             xout[i] = np.median(xin[i - Lwing : i + Lwing + 1])
             # (i-Lwing to i+Lwing)
@@ -578,14 +578,18 @@
 
     The PL33 filter is described on p. 21, Rosenfeld (1983), WHOI
     Technical Report 85-35.  Filter half amplitude period = 33 hrs.,
     half power period = 38 hrs.  The time series x is folded over
     and cosine tapered at each end to return a filtered time series
     xf of the same length.  Assumes length of x greater than 67.
 
+    Can input a DataArray and use dask-supported for lazy execution. In that
+    use case, dt is ignored and calculated from the input DataArray.
+    cf-xarray is also required.
+
     Examples
     --------
     >>> from oceans.filters import pl33tn
     >>> import matplotlib.pyplot as plt
     >>> t = np.arange(500)  # Time in hours.
     >>> x = 2.5 * np.sin(2 * np.pi * t / 12.42)
     >>> x += 1.5 * np.sin(2 * np.pi * t / 12.0)
@@ -599,14 +603,24 @@
     >>> pad = [np.NaN] * 17
     >>> (l3,) = ax.plot(t, np.r_[pad, filtered_33d3, pad], label="3 days")
     >>> legend = ax.legend()
 
 
     """
 
+    import cf_xarray  # noqa: F401
+    import xarray as xr
+
+    if isinstance(x, xr.Dataset):
+        raise TypeError("Input a DataArray not a Dataset.")
+
+    if isinstance(x, xr.DataArray):
+        # find dt in units of hours
+        dt = (x.cf["T"][1] - x.cf["T"][0]) * 1e-9 / 3600
+
     pl33 = np.array(
         [
             -0.00027,
             -0.00114,
             -0.00211,
             -0.00317,
             -0.00427,
@@ -682,9 +696,26 @@
     filter_time = np.arange(0.0, 33.0, dt, dtype="d")
     # N = len(filter_time)
     filter_time = np.hstack((-filter_time[-1:0:-1], filter_time))
 
     pl33 = np.interp(filter_time, _dt, pl33)
     pl33 /= pl33.sum()
 
-    xf = np.convolve(x, pl33, mode=mode)
+    if isinstance(x, xr.DataArray):
+        weight = xr.DataArray(pl33, dims=["window"])
+        xf = (
+            x.rolling({x.cf["T"].name: len(pl33)}, center=True)
+            .construct({x.cf["T"].name: "window"})
+            .dot(weight)
+        )
+        # update attrs
+        attrs = {
+            key: f"{value}, filtered"
+            for key, value in x.attrs.items()
+            if key != "units"
+        }
+        xf.attrs = attrs
+
+    else:  # use numpy
+        xf = np.convolve(x, pl33, mode=mode)
+
     return xf
```

### Comparing `oceans-1.0.0/oceans/ocfis.py` & `oceans-1.1.0/oceans/ocfis.py`

 * *Files 1% similar despite different names*

```diff
@@ -764,15 +764,15 @@
             xi.max() > x.max(),
             yi.min() < y.min(),
             yi.max() > y.max(),
         ],
     )
 
     if conditions.any():
-        warnings.warn("Warning! Extrapolation!!")
+        warnings.warn("Warning! Extrapolation!!", stacklevel=2)
 
     dx = x[0, 1] - x[0, 0]
     dy = y[1, 0] - y[0, 0]
 
     jvals = (xi - x[0, 0]) / dx
     ivals = (yi - y[0, 0]) / dy
```

### Comparing `oceans-1.0.0/oceans/plotting.py` & `oceans-1.1.0/oceans/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
                 self.points.set_ydata(y)
                 self.line.set_data(self.points.get_data())
         elif event.key == "i":
             if self.verbose:
                 print("Insert point")  # noqa
             xs = self.points.get_xdata()
             ex, ey = event.xdata, event.ydata
-            for i in range(len(xs) - 1):
+            for _i in range(len(xs) - 1):
                 self.points.set_xdata(np.r_[self.points.get_xdata(), ex])
                 self.points.set_ydata(np.r_[self.points.get_ydata(), ey])
                 self.line.set_data(self.points.get_data())
                 if self.verbose:
                     print(f"\nInserting: ({ex}, {ey})")  # noqa
                 break
```

### Comparing `oceans-1.0.0/oceans/sandbox/data/testdata.npz` & `oceans-1.1.0/oceans/sandbox/data/testdata.npz`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/sandbox/lines.py` & `oceans-1.1.0/oceans/sandbox/lines.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/sw_extras/__init__.py` & `oceans-1.1.0/oceans/sw_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/sw_extras/gamma_GP_from_SP_pt.py` & `oceans-1.1.0/oceans/sw_extras/gamma_GP_from_SP_pt.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/sw_extras/sw_extras.py` & `oceans-1.1.0/oceans/sw_extras/sw_extras.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/sw_extras/waves.py` & `oceans-1.1.0/oceans/sw_extras/waves.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/synop.py` & `oceans-1.1.0/oceans/synop.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans/utilities.py` & `oceans-1.1.0/oceans/utilities.py`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/oceans.egg-info/SOURCES.txt` & `oceans-1.1.0/oceans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oceans-1.0.0/pyproject.toml` & `oceans-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -7,18 +7,27 @@
 ]
 
 [project]
 name = "oceans"
 description = "Misc functions for oceanographic data analysis"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
-authors = [
-    {name = "André Palóczy, Arnaldo Russo, Filipe Fernandes"},
+maintainers = [
+    {name = "André Palóczy"},
+    {name = "Arnaldo Russo"},
+    {name = "Filipe Fernandes"},
 ]
 requires-python = ">=3.8"
+classifiers = [
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
 dynamic = [
   "version",
 ]
 dependencies = [
   "contourpy",
   "gsw",
   "matplotlib>=3.6",
@@ -54,33 +63,41 @@
 [tool.pytest.ini_options]
 markers = [
   "web: marks tests require connection (deselect with '-m \"not web\"')"
   ]
 
 [tool.ruff]
 select = [
+    "A", # flake8-builtins
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
     "F", # flakes
     "I", # import sorting
-    "U", # upgrade
+    "T20", # flake8-print
+    "UP", # upgrade
 ]
 target-version = "py311"
 line-length = 79
+ignore = [
+    "B905",  # zip ztrict arg, enable only for py310
+]
 
 [tool.ruff.per-file-ignores]
-"docs/conf.py" = ["E402"]
+"docs/source/conf.py" = ["E402", "A001"]
+"oceans/plotting.py" = ["T201"]  # `print` found
 
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-module = false
 fail-under = 95
-exclude = ["setup.py", "docs", "tests"]
+exclude = ["docs", "tests"]
 verbose = 1
 quiet = false
 color = true
 
 [tool.check-manifest]
 ignore = [
     ".coveragerc",
```

