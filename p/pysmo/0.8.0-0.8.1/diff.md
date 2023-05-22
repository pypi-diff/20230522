# Comparing `tmp/pysmo-0.8.0.tar.gz` & `tmp/pysmo-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmo-0.8.0.tar", max compression
+gzip compressed data, was "pysmo-0.8.1.tar", max compression
```

## Comparing `pysmo-0.8.0.tar` & `pysmo-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0    35147 2018-08-08 15:25:14.222828 pysmo-0.8.0/LICENSE
--rw-r--r--   0        0        0      619 2021-08-23 10:42:00.514598 pysmo-0.8.0/README.md
--rw-r--r--   0        0        0      823 2021-08-23 10:42:00.516598 pysmo-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      402 2019-01-11 00:33:10.486265 pysmo-0.8.0/pysmo/__init__.py
--rw-r--r--   0        0        0      335 2019-01-11 00:33:10.486265 pysmo-0.8.0/pysmo/core/__init__.py
--rw-r--r--   0        0        0      282 2019-01-11 00:33:10.486265 pysmo-0.8.0/pysmo/core/sac/__init__.py
--rw-r--r--   0        0        0     8479 2020-12-10 22:01:18.587487 pysmo-0.8.0/pysmo/core/sac/sacfunc.py
--rw-r--r--   0        0        0    10065 2021-06-29 14:16:59.369675 pysmo-0.8.0/pysmo/core/sac/sacheader.py
--rw-r--r--   0        0        0    18220 2021-06-29 14:16:59.370675 pysmo-0.8.0/pysmo/core/sac/sacheader.yml
--rw-r--r--   0        0        0    16405 2021-08-23 10:42:00.516598 pysmo-0.8.0/pysmo/core/sac/sacio.py
--rw-r--r--   0        0        0     1603 2020-12-10 22:01:18.587487 pysmo-0.8.0/pysmo/core/sac/sacmeth.py
--rw-r--r--   0        0        0     1585 2019-10-01 15:21:39.778629 pysmo-0.8.0/pysmo/core/timeseries.py
--rw-r--r--   0        0        0      113 2019-01-11 00:33:10.487265 pysmo-0.8.0/pysmo/tools/__init__.py
--rw-r--r--   0        0        0      384 2018-09-28 14:27:50.983507 pysmo-0.8.0/pysmo/tools/noise/__init__.py
--rw-r--r--   0        0        0     4102 2019-01-11 00:33:10.504265 pysmo-0.8.0/pysmo/tools/noise/peterson.py
--rw-r--r--   0        0        0     1483 2021-08-23 10:45:52.849299 pysmo-0.8.0/setup.py
--rw-r--r--   0        0        0     1659 2021-08-23 10:45:52.849626 pysmo-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-05-19 23:31:41.963627 pysmo-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1587 2023-05-22 12:23:35.953666 pysmo-0.8.1/README.md
+-rw-r--r--   0        0        0      990 2023-05-22 12:42:40.771632 pysmo-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-05-22 12:23:36.411661 pysmo-0.8.1/pysmo/__init__.py
+-rw-r--r--   0        0        0      380 2023-05-22 12:23:36.444660 pysmo-0.8.1/pysmo/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-22 12:23:36.478660 pysmo-0.8.1/pysmo/core/sac/__init__.py
+-rw-r--r--   0        0        0     8500 2023-05-22 12:23:36.511659 pysmo-0.8.1/pysmo/core/sac/sacfunc.py
+-rw-r--r--   0        0        0    10065 2023-05-22 12:23:36.556659 pysmo-0.8.1/pysmo/core/sac/sacheader.py
+-rw-r--r--   0        0        0    18220 2023-05-22 12:23:36.601658 pysmo-0.8.1/pysmo/core/sac/sacheader.yml
+-rw-r--r--   0        0        0    16547 2023-05-22 12:23:36.646658 pysmo-0.8.1/pysmo/core/sac/sacio.py
+-rw-r--r--   0        0        0      113 2022-05-19 23:31:41.968627 pysmo-0.8.1/pysmo/tools/__init__.py
+-rw-r--r--   0        0        0      417 2022-05-19 23:31:41.969627 pysmo-0.8.1/pysmo/tools/noise/__init__.py
+-rw-r--r--   0        0        0     4122 2023-05-22 12:23:36.691657 pysmo-0.8.1/pysmo/tools/noise/peterson.py
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 pysmo-0.8.1/setup.py
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 pysmo-0.8.1/PKG-INFO
```

### Comparing `pysmo-0.8.0/LICENSE` & `pysmo-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.0/pyproject.toml` & `pysmo-0.8.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "pysmo"
-version = "0.8.0"
+version = "0.8.1"
 description = "Python module to read/write/manipulate SAC (Seismic Analysis Code) files"
 readme = "README.md"
 authors = ["Simon M. Lloyd <simon@slloyd.net>"]
 license = "GPL-3.0-or-later"
+documentation = "https://pysmo.readthedocs.io"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "<3.12,>=3.8"
 scipy = "^1.5.4"
 numpy = "^1.19.4"
 matplotlib = "^3.3.3"
 pyproj = "^3.0.0"
 PyYAML = "^5.3.1"
 requests = "^2.25.1"
 
@@ -25,12 +27,13 @@
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 Sphinx = "^3.3.1"
 sphinx-rtd-theme = "^0.5.0"
 pytest-mpl = "^0.12"
 pytest-cov = "^2.10.1"
 pytest-depends = "^1.0.1"
+flake8 = "^3.9.2"
 
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pysmo-0.8.0/pysmo/core/sac/sacfunc.py` & `pysmo-0.8.1/pysmo/core/sac/sacfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 # along with pysmo.  If not, see <http://www.gnu.org/licenses/>.
 ###
 
 """
 Useful functions to use with SacIO objects.
 """
 
-__copyright__ = """
-Copyright (c) 2012 Simon Lloyd
-"""
+__author__ = "Simon Lloyd"
+__copyright__ = "Copyright (c) 2012 Simon Lloyd"
 
 
 def sac2xy(name, retarray=False):
     """
     Return time and amplitude from a SacIO object.
 
     :param name: Name of the SacIO object passed to this function.
```

### Comparing `pysmo-0.8.0/pysmo/core/sac/sacheader.py` & `pysmo-0.8.1/pysmo/core/sac/sacheader.py`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.0/pysmo/core/sac/sacheader.yml` & `pysmo-0.8.1/pysmo/core/sac/sacheader.yml`

 * *Files identical despite different names*

### Comparing `pysmo-0.8.0/pysmo/core/sac/sacio.py` & `pysmo-0.8.1/pysmo/core/sac/sacio.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 # along with pysmo.  If not, see <http://www.gnu.org/licenses/>.
 ###
 
 """
 Python module for reading/writing SAC files using the :class:`SacIO` class.
 """
 
+__author__ = "Simon Lloyd"
+__copyright__ = "Copyright (c) 2012 Simon Lloyd"
+
 import struct
 import datetime
 import io
 import requests
 import urllib.parse
 import zipfile
 from contextlib import contextmanager
 from .sacheader import SacHeader, _HEADER_FIELDS
 
-__copyright__ = """
-Copyright (c) 2012 Simon Lloyd
-"""
-
 
 class SacIO():
     """
     The :class:`SacIO` class reads and writes data and header values to and
     from a SAC file. Additonal class attributes may be set, but are not written
     to a SAC file (because there is no space reserved for them there). Class
     attributes with corresponding header fields in a SAC file (for example the
@@ -60,17 +59,14 @@
     Change the sampling rate::
 
         >>> newdelta = 0.05
         >>> my_sac.delta = newdelta
         >>> my_sac.delta
         0.05
 
-    There are a lot of header fields in a SAC file, which are all called the
-    same way when using :class:`SacIO`. They are all listed below.
-
     Read from IRIS services::
 
         >>> from pysmo import SacIO
         >>> my_sac = SacIO.from_iris(
         >>>             net="C1",
         >>>             sta="VA01",
         >>>             cha="BHZ",
@@ -79,14 +75,16 @@
         >>>             duration=1 * 60 * 60,
         >>>             scale="AUTO",
         >>>             demean="true",
         >>>             force_single_result=True)
         >>> my_sac.npts
         144001
 
+    There are a lot of header fields in a SAC file, which are all called the
+    same way when using :class:`SacIO`. They are all listed below.
     """
 
     # Descriptors for all header fields
     delta = SacHeader("delta")
     depmin = SacHeader("depmin")
     depmax = SacHeader("depmax")
     scale = SacHeader("scale")
@@ -311,23 +309,25 @@
             raise EOFError()
 
         content = buffer[start1:end1]
         data1 = struct.unpack(data_format, content)
 
         # Try reading second data block and combine both blocks
         # to a list of tuples. If it fails return only the first
-        # data block as a list
+        # data block as a list.
+        # NOTE: I've never encountered such a file in
+        # the wild, and this is somewhat untested...
         try:
             content = buffer[start1+length:end1+length]
             data2 = struct.unpack(data_format, content)
             data = []
             for x1, x2 in zip(data1, data2):
                 data.append((x1, x2))
             self._data = data
-        except:
+        except:  # noqa: E722
             self._data = list(data1)
             if self.depmen is None:
                 self.depmen = sum(data1)/self.npts
 
         if self.depmin is None:
             self.depmin = min(data1)
```

### Comparing `pysmo-0.8.0/pysmo/tools/noise/peterson.py` & `pysmo-0.8.1/pysmo/tools/noise/peterson.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 # You should have received a copy of the GNU General Public License
 # along with pysmo.  If not, see <http://www.gnu.org/licenses/>.
 ###
 
 """
 """
 
-__copyright__ = """
-Copyright (c) 2013 Simon Lloyd
-"""
+__copyright__ = "Copyright (c) 2012 Simon Lloyd"
+
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.integrate import cumtrapz
 
 NLNM = dict(dB=np.array([-168.0, -166.7, -166.7, -169.2, -163.7,
                          -148.6, -141.1, -141.1, -149.0, -163.8,
@@ -39,23 +38,26 @@
 NHNM = dict(dB=np.array([-91.5, -97.4, -110.5, -120.0, -98.0,
                          -96.5, -101.0, -113.5, -120.0, -138.5,
                          -126.0, -80.1, -48.5]),
             T=np.array([0.10, 0.22, 0.32, 0.80, 3.80, 4.60,
                         6.30, 7.90, 15.40, 20.00, 354.80,
                         10**4, 10**5]))
 
+
 def _genNoise(delta, npts, NM, velocity):
     """
     Helper function for calculating random noise from noise model NM.
     """
     delta = float(delta)
-    Fnyq = 0.5/delta 
-    f = interp1d(NM['T'], NM['dB'], kind='linear', bounds_error=False, fill_value=-200)
-    NPTS = int(2**np.ceil(np.ceil(np.log2(npts)+1))) # make it longer than necessary so we can cut out middle bit
-    freqs = np.linspace(1./NPTS/delta,Fnyq,NPTS-1)
+    Fnyq = 0.5/delta
+    f = interp1d(NM['T'], NM['dB'], kind='linear', bounds_error=False,
+                 fill_value=-200)
+    # make it longer than necessary so we can cut out middle bit
+    NPTS = int(2**np.ceil(np.ceil(np.log2(npts)+1)))
+    freqs = np.linspace(1./NPTS/delta, Fnyq, NPTS-1)
     Pxx = f(1/freqs)
     spectrum = np.zeros(NPTS)
     spectrum[1:NPTS] = np.sqrt(10**(Pxx/10) * NPTS / delta * 2)
 
     # phase is randomly generated
     phase = (np.random.rand(NPTS) - 0.5) * np.pi * 2
 
@@ -69,14 +71,15 @@
         velocity = velocity[start:end]
         velocity = velocity - np.mean(velocity)
         return velocity
     acceleration = acceleration[start:end]
     acceleration = acceleration - np.mean(acceleration)
     return acceleration
 
+
 def genNoiseNLNM(delta, npts, velocity=False):
     """
     Generate a random signal that matches Peterson's
     new low noise model NLNM.
 
     :param delta: Sampling rate of generated noise
     :type delta: float
@@ -91,14 +94,15 @@
         >>> import pysmo.tools.noise as noise
         >>> delta = 0.05
         >>> npts = 5000
         >>> low_noise = noise.genNoiseNLNM(delta, npts)
     """
     return _genNoise(delta, npts, NLNM, velocity)
 
+
 def genNoiseNHNM(delta, npts, velocity=False):
     """
     Generate a random signal that matches Peterson's
     new high noise model NHNM.
 
     :param delta: Sampling rate of generated noise
     :type delta: float
```

