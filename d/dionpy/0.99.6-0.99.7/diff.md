# Comparing `tmp/dionpy-0.99.6.tar.gz` & `tmp/dionpy-0.99.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dionpy-0.99.6.tar", max compression
+gzip compressed data, was "dionpy-0.99.7.tar", max compression
```

## Comparing `dionpy-0.99.6.tar` & `dionpy-0.99.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1068 2022-08-09 17:20:39.809565 dionpy-0.99.6/LICENSE
--rwxr-xr-x   0        0        0      305 2022-11-09 17:44:18.328435 dionpy-0.99.6/README.md
--rw-r--r--   0        0        0     1034 2023-03-30 18:02:10.402338 dionpy-0.99.6/pyproject.toml
--rwxr-xr-x   0        0        0     4956 2023-03-30 17:59:46.691455 dionpy-0.99.6/src/dionpy/DLayer.py
--rwxr-xr-x   0        0        0     6380 2023-03-30 17:58:25.752083 dionpy-0.99.6/src/dionpy/FLayer.py
--rwxr-xr-x   0        0        0    24032 2023-03-30 17:58:25.780082 dionpy-0.99.6/src/dionpy/IonFrame.py
--rwxr-xr-x   0        0        0     8729 2023-03-30 17:58:25.772082 dionpy-0.99.6/src/dionpy/IonLayer.py
--rwxr-xr-x   0        0        0    15937 2023-03-30 17:41:11.859808 dionpy-0.99.6/src/dionpy/IonModel.py
--rwxr-xr-x   0        0        0      189 2022-08-05 19:11:20.810361 dionpy-0.99.6/src/dionpy/__init__.py
--rwxr-xr-x   0        0        0        0 2022-07-30 19:21:54.420046 dionpy-0.99.6/src/dionpy/modules/__init__.py
--rwxr-xr-x   0        0        0      155 2022-10-08 16:14:43.272649 dionpy-0.99.6/src/dionpy/modules/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      151 2022-08-05 19:03:44.347964 dionpy-0.99.6/src/dionpy/modules/__pycache__/__init__.cpython-38.pyc
--rwxr-xr-x   0        0        0     1473 2022-10-08 16:14:43.292639 dionpy-0.99.6/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc
--rwxr-xr-x   0        0        0     1503 2022-08-22 18:27:05.149833 dionpy-0.99.6/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc
--rw-r--r--   0        0        0     6571 2023-03-30 17:44:39.398332 dionpy-0.99.6/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc
--rwxr-xr-x   0        0        0     6041 2022-08-24 17:53:23.444818 dionpy-0.99.6/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2762 2023-03-30 17:44:39.402332 dionpy-0.99.6/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc
--rwxr-xr-x   0        0        0     2404 2022-09-13 17:23:53.972099 dionpy-0.99.6/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-03-30 17:44:39.402332 dionpy-0.99.6/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc
--rwxr-xr-x   0        0        0     3325 2022-08-05 19:03:44.351964 dionpy-0.99.6/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc
--rw-r--r--   0        0        0     4451 2023-03-30 17:44:39.426332 dionpy-0.99.6/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc
--rwxr-xr-x   0        0        0     3943 2022-10-05 20:19:58.421732 dionpy-0.99.6/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc
--rwxr-xr-x   0        0        0     1166 2022-07-30 19:21:54.420046 dionpy-0.99.6/src/dionpy/modules/col_freq_agg.csv
--rwxr-xr-x   0        0        0     1214 2022-08-22 18:26:43.278932 dionpy-0.99.6/src/dionpy/modules/collision_models.py
--rwxr-xr-x   0        0        0     5890 2023-03-30 18:00:20.031196 dionpy-0.99.6/src/dionpy/modules/helpers.py
--rwxr-xr-x   0        0        0     3891 2023-03-30 18:00:20.011196 dionpy-0.99.6/src/dionpy/modules/ion_tools.py
--rwxr-xr-x   0        0        0     3802 2023-03-30 17:59:46.667455 dionpy-0.99.6/src/dionpy/modules/parallel.py
--rwxr-xr-x   0        0        0     4539 2023-03-30 17:41:52.647523 dionpy-0.99.6/src/dionpy/modules/plotting.py
--rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 dionpy-0.99.6/setup.py
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 dionpy-0.99.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2022-08-09 17:20:39.809565 dionpy-0.99.7/LICENSE
+-rwxr-xr-x   0        0        0      305 2022-11-09 17:44:18.328435 dionpy-0.99.7/README.md
+-rw-r--r--   0        0        0     1034 2023-05-22 21:14:53.954975 dionpy-0.99.7/pyproject.toml
+-rwxr-xr-x   0        0        0     4892 2023-05-05 23:38:28.402144 dionpy-0.99.7/src/dionpy/DLayer.py
+-rwxr-xr-x   0        0        0     6246 2023-05-05 23:39:53.469536 dionpy-0.99.7/src/dionpy/FLayer.py
+-rwxr-xr-x   0        0        0    23815 2023-05-05 23:38:28.378144 dionpy-0.99.7/src/dionpy/IonFrame.py
+-rwxr-xr-x   0        0        0     8643 2023-05-05 23:38:28.410144 dionpy-0.99.7/src/dionpy/IonLayer.py
+-rwxr-xr-x   0        0        0    15802 2023-05-05 23:38:28.414144 dionpy-0.99.7/src/dionpy/IonModel.py
+-rwxr-xr-x   0        0        0      189 2022-08-05 19:11:20.810361 dionpy-0.99.7/src/dionpy/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-07-30 19:21:54.420046 dionpy-0.99.7/src/dionpy/modules/__init__.py
+-rwxr-xr-x   0        0        0      155 2022-10-08 16:14:43.272649 dionpy-0.99.7/src/dionpy/modules/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      151 2022-08-05 19:03:44.347964 dionpy-0.99.7/src/dionpy/modules/__pycache__/__init__.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1473 2022-10-08 16:14:43.292639 dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1503 2022-08-22 18:27:05.149833 dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc
+-rw-r--r--   0        0        0     6015 2023-05-05 23:40:04.961453 dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc
+-rwxr-xr-x   0        0        0     6041 2022-08-24 17:53:23.444818 dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2895 2023-04-17 23:55:21.174568 dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2404 2022-09-13 17:23:53.972099 dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc
+-rw-r--r--   0        0        0     4042 2023-04-17 23:39:36.664536 dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3325 2022-08-05 19:03:44.351964 dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc
+-rw-r--r--   0        0        0     6818 2023-04-19 00:05:43.520857 dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3943 2022-10-05 20:19:58.421732 dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc
+-rwxr-xr-x   0        0        0     1166 2022-07-30 19:21:54.420046 dionpy-0.99.7/src/dionpy/modules/col_freq_agg.csv
+-rwxr-xr-x   0        0        0     1214 2022-08-22 18:26:43.278932 dionpy-0.99.7/src/dionpy/modules/collision_models.py
+-rwxr-xr-x   0        0        0     5564 2023-05-05 23:40:02.877468 dionpy-0.99.7/src/dionpy/modules/helpers.py
+-rwxr-xr-x   0        0        0     2524 2023-04-17 23:53:52.255388 dionpy-0.99.7/src/dionpy/modules/ion_tools.py
+-rwxr-xr-x   0        0        0     3802 2023-04-17 22:22:14.774661 dionpy-0.99.7/src/dionpy/modules/parallel.py
+-rwxr-xr-x   0        0        0     7308 2023-04-19 00:05:17.461073 dionpy-0.99.7/src/dionpy/modules/plotting.py
+-rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 dionpy-0.99.7/setup.py
+-rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 dionpy-0.99.7/PKG-INFO
```

### Comparing `dionpy-0.99.6/LICENSE` & `dionpy-0.99.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/pyproject.toml` & `dionpy-0.99.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dionpy"
-version = "0.99.6"
+version = "0.99.7"
 description = "Dynamic ionosphere model for global 21 cm experiments"
 authors = ["Vadym Bidula <vadym.bidula@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/lap1dem/dionpy"
 include = [
     "LICENSE",
@@ -14,15 +14,15 @@
 python = ">=3.8, <3.12"
 
 numpy = "^1.22"
 healpy = "^1.16.1"
 tqdm = "^4.64.1"
 scipy = "^1.9.3"
 matplotlib = "^3.6.0"
-pymap3d = "^2.9.1"
+pymap3d = "^3.0.1"
 h5py = "^3.7.0"
 
 echaim = "^1.0.8"
 
 pytz = "^2022.1"
 it = "^1.0.0"
 Sphinx = "^5.0.2"
```

### Comparing `dionpy-0.99.6/src/dionpy/DLayer.py` & `dionpy-0.99.7/src/dionpy/DLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             nlayers: int = 100,
             nside: int = 64,
             iriversion: int = 20,
             echaim: bool = False,
             autocalc: bool = True,
             pbar: bool = True,
             _pool: Union[Pool, None] = None,
-            _apf107_args: List | None = None,
     ):
         super().__init__(
             dt,
             position,
             hbot,
             htop,
             nlayers,
@@ -57,15 +56,14 @@
             rdeg=15,
             pbar=pbar,
             name="D layer",
             iriversion=iriversion,
             echaim=echaim,
             autocalc=autocalc,
             _pool=_pool,
-            _apf107_args=_apf107_args,
         )
 
     def atten(
             self,
             el: float | np.ndarray,
             az: float | np.ndarray,
             freq: float | np.ndarray,
@@ -101,17 +99,17 @@
         else:
             col_model = lambda h: np.float64(col_freq)
 
         heights_km = np.linspace(self.hbot, self.htop, self.nlayers)
 
         theta = np.deg2rad(90 - el)
         if troposphere:
-            dtheta = trop_refr(theta)
-            theta += dtheta
-            el -= np.rad2deg(dtheta)
+            dtheta = trop_refr(el, self.position[-1]*1e-3)
+            theta += np.deg2rad(dtheta)
+            el -= dtheta
 
         c = 2.99792458e8
 
         for i in range(self.nlayers):
             freq_c = col_model(heights_km[i])
             ded = self.ed(el, az, layer=i)
             det = self.et(el, az, layer=i)
```

### Comparing `dionpy-0.99.6/src/dionpy/FLayer.py` & `dionpy-0.99.7/src/dionpy/FLayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             nlayers: int = 100,
             nside: int = 64,
             iriversion: int = 20,
             echaim: bool = False,
             autocalc: bool = True,
             pbar: bool = True,
             _pool: Union[Pool, None] = None,
-            _apf107_args: List | None = None,
     ):
         super().__init__(
             dt,
             position,
             hbot,
             htop,
             nlayers,
@@ -56,15 +55,14 @@
             rdeg=30,
             pbar=pbar,
             name="F layer",
             iriversion=iriversion,
             echaim=echaim,
             autocalc=autocalc,
             _pool=_pool,
-            _apf107_args=_apf107_args,
         )
 
     def refr(
             self,
             el: float | np.ndarray,
             az: float | np.ndarray,
             freq: float | List | np.ndarray,
@@ -78,25 +76,23 @@
         :return: Refraction angle in [deg] at given sky coordinates, time and frequency of observation.
         """
         # TODO: Fix low frequency cutoff calculation
         freq *= 1e6
         check_elaz_shape(el, az)
         el, az = el.copy(), az.copy()
         re = 6378100.0
-        ell = Ellipsoid()
+        ell = Ellipsoid(re, re)
         f_heights = np.linspace(self.hbot, self.htop, self.nlayers) * 1e3
         delta_theta = 0 * el
         inf_theta_mask = 0 * el
         nan_theta_mask = 0 * el
 
-        theta = np.deg2rad(90 - el)
         if troposphere:
-            dtheta = trop_refr(theta)
-            theta += dtheta
-            el -= np.rad2deg(dtheta)
+            dtheta = trop_refr(el, self.position[-1]*1e-3)
+            el -= dtheta
 
         # Distance from telescope to first layer
         r_slant = srange(np.deg2rad(90 - el), f_heights[0] - self.position[2])
         # Geodetic coordinates of 'hit point' on the first layer
         lat_ray, lon_ray, _ = pm.aer2geodetic(
             az, el, r_slant, *self.position, ell=ell
         )  # arrays
```

### Comparing `dionpy-0.99.6/src/dionpy/IonFrame.py` & `dionpy-0.99.7/src/dionpy/IonFrame.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import itertools
 import os
 import shutil
 import tempfile
 from datetime import datetime
 from multiprocessing import cpu_count, Pool
-from typing import Tuple, Callable, Union, List, Sequence
+from typing import Tuple, Callable, Union, List, Sequence, Literal
 
 import h5py
-import iricore
+import iricore as iri
 import numpy as np
 import pymap3d as pm
 from tqdm import tqdm
 
 from .DLayer import DLayer
 from .FLayer import FLayer
 from .modules.helpers import none_or_array, elaz_mesh, TextColor, pic2vid, Ellipsoid
@@ -54,33 +54,32 @@
         nside: int = 64,
         dbot: float = 60,
         dtop: float = 90,
         ndlayers: int = 100,
         fbot: float = 150,
         ftop: float = 500,
         nflayers: int = 100,
-        iriversion: int = 20,
+        iriversion: Literal[16, 20] = 20,
         echaim: bool = False,
         autocalc: bool = True,
         _pbar: bool = False,
         _pool: Union[Pool, None] = None,
-        _apf107_args: List | None = None
     ):
         if isinstance(dt, datetime):
             self.dt = dt
         else:
             raise ValueError("Parameter dt must be a datetime object.")
         self.position = position
         self.nside = nside
         self.iriversion = iriversion
         self.dlayer = DLayer(
-            dt, position, dbot, dtop, ndlayers, nside, iriversion, echaim, autocalc, _pbar, _pool, _apf107_args,
+            dt, position, dbot, dtop, ndlayers, nside, iriversion, echaim, autocalc, _pbar, _pool,
         )
         self.flayer = FLayer(
-            dt, position, fbot, ftop, nflayers, nside, iriversion, echaim, autocalc, _pbar, _pool, _apf107_args,
+            dt, position, fbot, ftop, nflayers, nside, iriversion, echaim, autocalc, _pbar, _pool,
         )
 
     def calc(self, pbar: bool = False):
         """
         Calculates the model (use it if you set autocalc=False during the initialization).
 
         :param pbar: If True - a progress bar will appear.
@@ -94,24 +93,23 @@
         Sends methods either to serial or parallel calculation routines based on type of freq.
         """
         if (isinstance(freq, list) or isinstance(freq, np.ndarray)) and len(freq) > 1:
             return calc_refatt_par(func, el, az, freq, pbar_desc, **kwargs)
         else:
             return calc_refatt(func, el, az, freq, **kwargs)
 
-    @staticmethod
-    def troprefr(el: float | np.ndarray) -> float | np.ndarray:
+    def troprefr(self, el: float | np.ndarray) -> float | np.ndarray:
         """
         Approximation of the refraction in the troposphere recommended by the ITU-R:
         https://www.itu.int/dms_pubrec/itu-r/rec/p/R-REC-P.834-9-201712-I!!PDF-E.pdf
 
         :param el: Elevation of observation(s) in [deg].
         :return: Refraction in the troposphere in [deg].
         """
-        return np.rad2deg(trop_refr(np.deg2rad(90 - el)))
+        return trop_refr(el, self.position[2]*1e-3)
 
     def refr(
             self,
             el: float | np.ndarray,
             az: float | np.ndarray,
             freq: float | np.ndarray,
             troposphere: bool = True,
@@ -169,15 +167,15 @@
         :param dec: Declination in [deg].
         :return: [alt, az], both in [deg]
         """
         from astropy.coordinates import EarthLocation, SkyCoord, AltAz
         from astropy.time import Time
         from astropy import units as u
 
-        location = EarthLocation(lat=self.position[0], lon=self.position[0], height=self.position[2] * u.m)
+        location = EarthLocation(lat=self.position[0], lon=self.position[1], height=self.position[2] * u.m)
         time = Time(self.dt)
         altaz_cs = AltAz(location=location, obstime=time)
         skycoord = SkyCoord(ra * u.deg, dec * u.deg)
         aa_coord = skycoord.transform_to(altaz_cs)
         return aa_coord.alt.value, aa_coord.az.value
 
     def stec(self, alt: float, az: float, hbot: float = 90, htop: float = 2000, npoints: int = 500) -> float:
@@ -187,26 +185,15 @@
         :param alt: Altitude angle.
         :param az: Azimuth angle.
         :param hbot: Bottom height limit for integration.
         :param htop: Top height limit for integration.
         :param npoints: Number of points to integrate.
         :return: Total electron content along the line of sight in TECU (10^16 m-2).
         """
-        hstep = (htop - hbot) / npoints
-        heights = np.linspace(hbot, htop, npoints)
-        rslant = srange(np.deg2rad(90 - alt), heights * 1e3)
-        ell = Ellipsoid()
-        slat, slon, _ = pm.aer2geodetic(az, alt, rslant, *self.position, ell=ell)
-        ne = iricore.STEC(self.dt, heights, slat, slon, version=self.iriversion)
-        ne = np.where(np.isnan(ne), 0, ne)
-        ne = np.where(np.isinf(ne), 0, ne)
-        ne_ = ne - np.roll(ne, -1)
-        ne = np.where(ne_ > 1e3, np.roll(ne, 1), ne)
-        res = np.sum(ne) * hstep * 1e3 * 1e-16
-        return res
+        return iri.stec(alt, az, self.dt, self.position, version=self.iriversion)
 
     def stec_echaim(self, alt: float, az: float, hbot: float = 90, htop: float = 2000, npoints: int = 500) -> float:
         """
         Calculates slant tec in a given direction using the E-CHAIM model.
 
         :param alt: Altitude angle.
         :param az: Azimuth angle.
@@ -304,96 +291,104 @@
                     + "Consider reading it with IonModel class."
                 )
 
             grp = file[groups[0]]
             obj = cls.read_self_from_file(grp)
         return obj
 
-    def plot_ded(self, gridsize: int = 200, layer: int | None = None, **kwargs):
+    def plot_ded(self, gridsize: int = 200, layer: int | None = None, cmap='plasma', **kwargs):
         """
         Visualize electron density in the D layer.
 
         :param gridsize: Grid resolution of the plot.
         :param layer: A specfic layer to plot. If None - an average of all layers is calculated.
+        :param cmap: A colormap to use in the plot.
         :param kwargs: See `dionpy.plot_kwargs`.
         :return: A matplotlib figure.
         """
         barlabel = r"$m^{-3}$"
         el, az = elaz_mesh(gridsize)
         ded = self.dlayer.ed(el, az, layer)
         return polar_plot(
             (np.deg2rad(az), 90 - el, ded),
             dt=self.dt,
             pos=self.position,
             barlabel=barlabel,
+            cmap=cmap,
             **kwargs,
         )
 
-    def plot_det(self, gridsize: int = 200, layer: int | None = None, **kwargs):
+    def plot_det(self, gridsize: int = 200, layer: int | None = None, cmap='viridis', **kwargs):
         """
         Visualize electron temperature in the D layer.
 
         :param gridsize: Grid resolution of the plot.
         :param layer: A specfic layer to plot. If None - an average of all layers is calculated.
+        :param cmap: A colormap to use in the plot.
         :param kwargs: See `dionpy.plot_kwargs`.
         :return: A matplotlib figure.
         """
-        barlabel = r"$K^\circ$"
+        barlabel = "K"
         el, az = elaz_mesh(gridsize)
         det = self.dlayer.et(el, az, layer)
         return polar_plot(
             (np.deg2rad(az), 90 - el, det),
             dt=self.dt,
             pos=self.position,
             barlabel=barlabel,
+            cmap=cmap,
             **kwargs,
         )
 
-    def plot_fed(self, gridsize: int = 200, layer: int | None = None, **kwargs):
+    def plot_fed(self, gridsize: int = 200, layer: int | None = None, cmap='plasma', **kwargs):
         """
         Visualize electron density in the F layer.
 
         :param gridsize: Grid resolution of the plot.
         :param layer: A specfic layer to plot. If None - an average of all layers is calculated.
+        :param cmap: A colormap to use in the plot.
         :param kwargs: See `dionpy.plot_kwargs`.
         :return: A matplotlib figure.
         """
         barlabel = r"$m^{-3}$"
         el, az = elaz_mesh(gridsize)
         fed = self.flayer.ed(el, az, layer)
         return polar_plot(
             (np.deg2rad(az), 90 - el, fed),
             dt=self.dt,
             pos=self.position,
             barlabel=barlabel,
+            cmap=cmap,
             **kwargs,
         )
 
-    def plot_fet(self, gridsize: int = 200, layer: int | None = None, **kwargs):
+    def plot_fet(self, gridsize: int = 200, layer: int | None = None, cmap='viridis', **kwargs):
         """
         Visualize electron temperature in the F layer.
 
         :param gridsize: Grid resolution of the plot.
         :param layer: A specfic layer to plot. If None - an average of all layers is calculated.
+        :param cmap: A colormap to use in the plot.
         :param kwargs: See `dionpy.plot_kwargs`.
         :return: A matplotlib figure.
         """
-        barlabel = r"$K^\circ$"
+        barlabel = r"K"
         el, az = elaz_mesh(gridsize)
         fet = self.flayer.et(el, az, layer)
         return polar_plot(
             (np.deg2rad(az), 90 - el, fet),
             dt=self.dt,
             pos=self.position,
             barlabel=barlabel,
+            cmap=cmap,
             **kwargs,
         )
 
     def plot_atten(
-        self, freq: float, troposphere: bool = True, gridsize: int = 200, cmap='viridis', cblim=None,  **kwargs
+        self, freq: float, troposphere: bool = True, gridsize: int = 200, cmap='Purples_r', cblim=None,  **kwargs
     ):
         """
         Visualize ionospheric attenuation.
 
         :param freq: Frequency of observation in [Hz].
         :param troposphere: If True - the troposphere refraction correction will be applied before calculation.
         :param gridsize: Grid resolution of the plot.
@@ -414,15 +409,15 @@
             freq=freq,
             cmap=cmap,
             cblim=cblim,
             **kwargs,
         )
 
     def plot_emiss(
-        self, freq: float, troposphere: bool = True, gridsize: int = 200, cmap='viridis', cblim=None, **kwargs
+        self, freq: float, troposphere: bool = True, gridsize: int = 200, cmap='Oranges', cblim=None, **kwargs
     ):
         """
         Visualize ionospheric attenuation.
 
         :param freq: Frequency of observation in [Hz].
         :param troposphere: If True - the troposphere refraction correction will be applied before calculation.
         :param gridsize: Grid resolution of the plot.
@@ -447,15 +442,15 @@
         )
 
     def plot_refr(
         self,
         freq: float,
         troposphere: bool = True,
         gridsize: int = 200,
-        cmap: str = 'viridis_r',
+        cmap: str = 'Greens',
         cblim=None,
         **kwargs,
     ):
         """
         Visualize ionospheric refraction.
 
         :param freq: Frequency of observation in [Hz].
@@ -477,15 +472,15 @@
             freq=freq,
             barlabel=barlabel,
             cmap=cmap,
             cblim=cblim,
             **kwargs,
         )
 
-    def plot_troprefr(self, gridsize=200, cmap="viridis_r", cblim=None, **kwargs):
+    def plot_troprefr(self, gridsize=200, cmap="Greens", cblim=None, **kwargs):
         """
         Visualize tropospheric refraction.
 
         :param gridsize: Grid resolution of the plot.
         :param cmap: A colormap to use in the plot.
         :param cblim: Colorbar limits.
         :param kwargs: See `dionpy.plot_kwargs`.
```

### Comparing `dionpy-0.99.6/src/dionpy/IonLayer.py` & `dionpy-0.99.7/src/dionpy/IonLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import itertools
 from datetime import datetime
 from multiprocessing import cpu_count, Pool
 from typing import List, Union, Sequence
 
 import healpy as hp
-import iricore
+import iricore as iri
 import numpy as np
 from tqdm import tqdm
 
 from .modules.helpers import eval_layer
 from .modules.parallel import iri_star, echaim_star
 
 
@@ -45,15 +45,14 @@
             rdeg: float = 20,
             pbar: bool = True,
             name: str | None = None,
             iriversion: int = 20,
             autocalc: bool = True,
             echaim: bool = False,
             _pool: Union[Pool, None] = None,
-            _apf107_args: List | None = None,
     ):
         self.hbot = hbot
         self.htop = htop
         self.nlayers = nlayers
         self.dt = dt
         self.position = position
         self.name = name
@@ -69,58 +68,58 @@
         self._obs_lons, self._obs_lats = hp.pix2ang(
             self.nside, self._obs_pixels, lonlat=True
         )
         self.edens = np.zeros((len(self._obs_pixels), nlayers))
         self.etemp = np.zeros((len(self._obs_pixels), nlayers))
 
         if autocalc:
-            self._calc(pbar=pbar, _pool=_pool, _apf107_args=_apf107_args)
+            self._calc(pbar=pbar, _pool=_pool)
 
     def _batch_split(self, batch):
         nbatches = len(self._obs_pixels) // batch + 1
         nproc = np.min([cpu_count(), nbatches])
         blat = np.array_split(self._obs_lats, nbatches)
         blon = np.array_split(self._obs_lons, nbatches)
         return nbatches, nproc, blat, blon
 
-    def _calc(self, pbar=True, _pool: Union[Pool, None] = None, _apf107_args: List | None = None):
+    def _calc(self, pbar=True, _pool: Union[Pool, None] = None):
         """
         Makes several calls to iricore in parallel requesting electron density and
         electron temperature for future use in attenuation modeling.
         """
 
         nbatches, nproc, blat, blon = self._batch_split(200)
 
         heights = (
             self.hbot,
             self.htop,
             (self.htop - self.hbot) / (self.nlayers - 1) - 1e-6,
         )
 
-        if _apf107_args is None:
-            aap, af107, nlines = iricore.readapf107(self.iriversion)
-        else:
-            aap, af107, nlines = _apf107_args
+        # if _apf107_args is None:
+        #     aap, af107, nlines = iricore.readapf107(self.iriversion)
+        # else:
+        #     aap, af107, nlines = _apf107_args
 
         # nproc=4
         pool = Pool(processes=nproc) if _pool is None else _pool
         res = list(
             tqdm(
                 pool.imap(
                     iri_star,
                     zip(
                         itertools.repeat(self.dt),
                         itertools.repeat(heights),
                         blat,
                         blon,
                         itertools.repeat(0.0),
                         itertools.repeat(self.iriversion),
-                        itertools.repeat(aap),
-                        itertools.repeat(af107),
-                        itertools.repeat(nlines),
+                        # itertools.repeat(aap),
+                        # itertools.repeat(af107),
+                        # itertools.repeat(nlines),
                     ),
                 ),
                 total=nbatches,
                 disable=not pbar,
                 desc=self.name,
             )
         )
```

### Comparing `dionpy-0.99.6/src/dionpy/IonModel.py` & `dionpy-0.99.7/src/dionpy/IonModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import tempfile
 from datetime import datetime, timedelta
 from multiprocessing import Pool, cpu_count
 from typing import List, Callable, Sequence
 import warnings
 
 import numpy as np
-from iricore import readapf107
 from numpy import ndarray
 from tqdm import tqdm
 
 from .IonFrame import IonFrame
 from .modules.helpers import elaz_mesh, TextColor, pic2vid, get_atten_from_frame, get_refr_from_frame
 from .modules.parallel import calc_interp_val_par, calc_interp_val, interp_val
 from .modules.plotting import polar_plot_star
@@ -90,15 +89,14 @@
         self.iriversion = iriversion
         self.models = []
 
         if autocalc:
             nproc = np.min([cpu_count(), nmodels])
             # nproc = 1
             pool = Pool(processes=nproc)
-            apf107_args = readapf107(self.iriversion)
 
             for dt in tqdm(self._dts, desc="Calculating time frames"):
                 self.models.append(
                     IonFrame(
                         dt,
                         position,
                         nside,
@@ -109,15 +107,14 @@
                         ftop,
                         nflayers,
                         iriversion,
                         echaim=echaim,
                         autocalc=autocalc,
                         _pbar=False,
                         _pool=pool,
-                        _apf107_args=apf107_args,
                     )
                 )
             pool.close()
 
     def save(self, saveto: str = "./ionmodel"):
         """
         Save the model to a file.
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/collision_models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 17:26:42 2023 UTC, .py size: 5900 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,411 +1,376 @@
-00000000: 6f0d 0d0a 0000 0000 52c6 2564 0c17 0000  o.......R.%d....
+00000000: 6f0d 0d0a 0000 0000 d293 5564 bc15 0000  o.........Ud....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0173 f200 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0173 de00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
-00000050: 6d06 5a06 6d07 5a07 0100 6400 6402 6c08  m.Z.m.Z...d.d.l.
-00000060: 5a09 6400 6402 6c0a 5a0b 6400 6404 6c0c  Z.d.d.l.Z.d.d.l.
-00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000080: 6d10 5a11 0100 6400 6406 6c12 6d12 5a12  m.Z...d.d.l.m.Z.
-00000090: 0100 6407 6408 6c13 6d14 5a14 0100 4700  ..d.d.l.m.Z...G.
-000000a0: 6409 640a 8400 640a 8302 5a15 4700 640b  d.d...d...Z.G.d.
-000000b0: 640c 8400 640c 6511 8303 5a10 6442 6411  d...d.e...Z.dBd.
-000000c0: 6412 8404 5a16 6413 6414 8400 5a17 6443  d...Z.d.d...Z.dC
-000000d0: 6418 6419 8404 5a18 6444 641f 6420 8404  d.d...Z.dDd.d ..
-000000e0: 5a19 6445 6424 6425 8404 5a1a 0902 6446  Z.dEd$d%..Z...dF
-000000f0: 6447 6431 6432 8405 5a1b 0933 0902 0934  dGd1d2..Z..3...4
-00000100: 6448 6449 643c 643d 8405 5a1c 643e 643f  dHdId<d=..Z.d>d?
-00000110: 8400 5a1d 6440 6441 8400 5a1e 6402 5300  ..Z.d@dA..Z.d.S.
-00000120: 294a e900 0000 0029 01da 0b61 6e6e 6f74  )J.....)...annot
-00000130: 6174 696f 6e73 4e29 04da 0554 7570 6c65  ationsN)...Tuple
-00000140: da08 4974 6572 6162 6c65 da04 4c69 7374  ..Iterable..List
-00000150: da08 5365 7175 656e 6365 2901 da0e 4666  ..Sequence)...Ff
-00000160: 6d70 6567 5072 6f67 7265 7373 2902 da0c  mpegProgress)...
-00000170: 6165 7232 6765 6f64 6574 6963 da09 456c  aer2geodetic..El
-00000180: 6c69 7073 6f69 6429 01da 0474 7164 6de9  lipsoid)...tqdm.
-00000190: 0100 0000 2901 da06 7372 616e 6765 6300  ....)...srangec.
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000001b0: 0000 0040 0000 0173 3800 0000 6500 5a01  ...@...s8...e.Z.
-000001c0: 6400 5a02 6401 5a03 6402 5a04 6403 5a05  d.Z.d.Z.d.Z.d.Z.
-000001d0: 6404 5a06 6405 5a07 6406 5a08 6407 5a09  d.Z.d.Z.d.Z.d.Z.
-000001e0: 6408 5a0a 6409 5a0b 640a 5a0c 640b 5a0d  d.Z.d.Z.d.Z.d.Z.
-000001f0: 640c 5300 290d da09 5465 7874 436f 6c6f  d.S.)...TextColo
-00000200: 727a 390a 2020 2020 5072 6f76 6964 6573  rz9.    Provides
-00000210: 2066 6f72 6d61 7474 6572 7320 666f 7220   formatters for 
-00000220: 7465 726d 696e 616c 2074 6578 7420 636f  terminal text co
-00000230: 6c6f 7269 6e67 2e0a 2020 2020 7a05 1b5b  loring..    z..[
-00000240: 3935 6d7a 051b 5b39 366d 7a05 1b5b 3336  95mz..[96mz..[36
-00000250: 6d7a 051b 5b39 346d 7a05 1b5b 3932 6d7a  mz..[94mz..[92mz
-00000260: 051b 5b39 336d 7a05 1b5b 3931 6d7a 041b  ..[93mz..[91mz..
-00000270: 5b31 6d7a 041b 5b34 6d7a 041b 5b30 6d4e  [1mz..[4mz..[0mN
-00000280: 290e da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000290: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000002a0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-000002b0: 0650 5552 504c 45da 0443 5941 4eda 0844  .PURPLE..CYAN..D
-000002c0: 4152 4b43 5941 4eda 0442 4c55 45da 0547  ARKCYAN..BLUE..G
-000002d0: 5245 454e da06 5945 4c4c 4f57 da03 5245  REEN..YELLOW..RE
-000002e0: 44da 0442 4f4c 44da 0955 4e44 4552 4c49  D..BOLD..UNDERLI
-000002f0: 4e45 da03 454e 44a9 0072 1c00 0000 721c  NE..END..r....r.
-00000300: 0000 00fa 3d2f 686f 6d65 2f6c 6170 3164  ....=/home/lap1d
-00000310: 656d 2f64 6576 2d70 7974 686f 6e2f 6469  em/dev-python/di
-00000320: 6f6e 7079 2f73 7263 2f64 696f 6e70 792f  onpy/src/dionpy/
-00000330: 6d6f 6475 6c65 732f 6865 6c70 6572 732e  modules/helpers.
-00000340: 7079 720d 0000 000f 0000 0073 1800 0000  pyr........s....
-00000350: 0800 0401 0404 0401 0401 0401 0401 0401  ................
-00000360: 0401 0401 0401 0801 720d 0000 0063 0000  ........r....c..
-00000370: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000380: 0000 0000 0001 7320 0000 0065 005a 0164  ......s ...e.Z.d
-00000390: 005a 0264 015a 0387 0066 0164 0264 0384  .Z.d.Z...f.d.d..
-000003a0: 085a 0487 0004 005a 0553 0029 0472 0900  .Z.....Z.S.).r..
-000003b0: 0000 7a4b 0a20 2020 2043 7573 746f 6d20  ..zK.    Custom 
-000003c0: 656c 6c69 7073 6f69 6420 666f 7220 7079  ellipsoid for py
-000003d0: 6d61 7033 6420 7061 636b 6167 652e 2049  map3d package. I
-000003e0: 6d70 6c65 6d65 6e74 7320 6120 7369 6d70  mplements a simp
-000003f0: 6c65 2073 7068 6572 652e 0a20 2020 2063  le sphere..    c
-00000400: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000410: 0200 0000 0300 0001 732c 0000 0074 0083  ........s,...t..
-00000420: 00a0 01a1 0001 0064 017c 005f 0264 017c  .......d.|._.d.|
-00000430: 005f 0364 027c 005f 0464 027c 005f 0564  ._.d.|._.d.|._.d
-00000440: 027c 005f 0664 0053 0029 034e 6700 0000  .|._.d.S.).Ng...
-00000450: 009d 5458 4167 0000 0000 0000 0000 2907  ..TXAg........).
-00000460: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-00000470: 5fda 0e73 656d 696d 616a 6f72 5f61 7869  _..semimajor_axi
-00000480: 73da 0e73 656d 696d 696e 6f72 5f61 7869  s..semiminor_axi
-00000490: 73da 0a66 6c61 7474 656e 696e 67da 0f74  s..flattening..t
-000004a0: 6869 7264 666c 6174 7465 6e69 6e67 da0c  hirdflattening..
-000004b0: 6563 6365 6e74 7269 6369 7479 2901 da04  eccentricity)...
-000004c0: 7365 6c66 a901 da09 5f5f 636c 6173 735f  self....__class_
-000004d0: 5f72 1c00 0000 721d 0000 0072 1f00 0000  _r....r....r....
-000004e0: 2500 0000 730c 0000 000a 0106 0106 0106  %...s...........
-000004f0: 0106 010a 017a 1245 6c6c 6970 736f 6964  .....z.Ellipsoid
-00000500: 2e5f 5f69 6e69 745f 5f29 0672 0e00 0000  .__init__).r....
-00000510: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000520: 1f00 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00000530: 6c5f 5f72 1c00 0000 721c 0000 0072 2600  l__r....r....r&.
-00000540: 0000 721d 0000 0072 0900 0000 2000 0000  ..r....r.... ...
-00000550: 7306 0000 0008 0004 0114 0472 0900 0000  s..........r....
-00000560: da04 7661 6c73 fa0f 4e6f 6e65 207c 2049  ..vals..None | I
-00000570: 7465 7261 626c 65da 0672 6574 7572 6efa  terable..return.
-00000580: 116e 702e 6e64 6172 7261 7920 7c20 4e6f  .np.ndarray | No
-00000590: 6e65 6301 0000 0000 0000 0000 0000 0001  nec.............
-000005a0: 0000 0003 0000 0043 0000 0173 1600 0000  .......C...s....
-000005b0: 7c00 6401 7500 7206 6401 5300 7400 a001  |.d.u.r.d.S.t...
-000005c0: 7c00 a101 5300 2902 7a56 0a20 2020 2055  |...S.).zV.    U
-000005d0: 7365 6420 666f 7220 6461 7461 206c 6f61  sed for data loa
-000005e0: 6469 6e67 2066 726f 6d20 4844 4620 6669  ding from HDF fi
-000005f0: 6c65 732e 2043 6f6e 7665 7274 7320 6e6f  les. Converts no
-00000600: 7420 4e6f 6e65 2076 616c 7565 7320 746f  t None values to
-00000610: 206e 702e 6172 7261 7973 2e0a 2020 2020   np.arrays..    
-00000620: 4e29 02da 026e 70da 0561 7272 6179 2901  N)...np..array).
-00000630: 7229 0000 0072 1c00 0000 721c 0000 0072  r)...r....r....r
-00000640: 1d00 0000 da0d 6e6f 6e65 5f6f 725f 6172  ......none_or_ar
-00000650: 7261 792e 0000 0073 0600 0000 0804 0401  ray....s........
-00000660: 0a01 722f 0000 0063 0100 0000 0000 0000  ..r/...c........
-00000670: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-00000680: 731e 0000 0074 007c 0074 0183 0273 0b74  s....t.|.t...s.t
-00000690: 007c 0074 026a 0383 0272 0d64 0153 0064  .|.t.j...r.d.S.d
-000006a0: 0253 0029 034e 5446 2904 da0a 6973 696e  .S.).NTF)...isin
-000006b0: 7374 616e 6365 da04 6c69 7374 722d 0000  stance..listr-..
-000006c0: 00da 076e 6461 7272 6179 2901 da01 7872  ...ndarray)...xr
-000006d0: 1c00 0000 721c 0000 0072 1d00 0000 da0b  ....r....r......
-000006e0: 6973 5f69 7465 7261 626c 6537 0000 0073  is_iterable7...s
-000006f0: 0600 0000 1601 0401 0401 7234 0000 00da  ..........r4....
-00000700: 0265 6cfa 1266 6c6f 6174 207c 206e 702e  .el..float | np.
-00000710: 6e64 6172 7261 79da 0261 7a63 0200 0000  ndarray..azc....
-00000720: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000730: 4300 0001 7354 0000 0074 007c 0074 0183  C...sT...t.|.t..
-00000740: 0273 2674 007c 0174 0183 0273 2874 007c  .s&t.|.t...s(t.|
-00000750: 0074 026a 0383 0272 2274 007c 0074 026a  .t.j...r"t.|.t.j
-00000760: 0383 0272 227c 006a 047c 016a 046b 0273  ...r"|.j.|.j.k.s
-00000770: 2074 0564 0183 0182 0164 0353 0074 0564   t.d.....d.S.t.d
-00000780: 0283 0182 0164 0353 0064 0353 0029 047a  .....d.S.d.S.).z
-00000790: 3f0a 2020 2020 4368 6563 6b73 2073 6861  ?.    Checks sha
-000007a0: 7065 2061 6e64 2074 7970 6520 6f66 2069  pe and type of i
-000007b0: 6e70 7574 2065 6c65 7661 7469 6f6e 2061  nput elevation a
-000007c0: 6e64 2061 7a69 6d75 7468 2e0a 2020 2020  nd azimuth..    
-000007d0: 7a2e 456c 6576 6174 696f 6e20 616e 6420  z.Elevation and 
-000007e0: 617a 696d 7574 6820 6d75 7374 2062 6520  azimuth must be 
-000007f0: 7468 6520 7361 6d65 206c 656e 6774 682e  the same length.
-00000800: 7a3c 456c 6576 6174 696f 6e20 616e 6420  z<Elevation and 
-00000810: 617a 696d 7574 6820 6d75 7374 2062 6520  azimuth must be 
-00000820: 6569 7468 6572 2066 6c6f 6174 7320 6f72  either floats or
-00000830: 206e 756d 7079 2061 7272 6179 732e 4e29   numpy arrays.N)
-00000840: 0672 3000 0000 da05 666c 6f61 7472 2d00  .r0.....floatr-.
-00000850: 0000 7232 0000 00da 0573 6861 7065 da0a  ..r2.....shape..
-00000860: 5661 6c75 6545 7272 6f72 2902 7235 0000  ValueError).r5..
-00000870: 0072 3700 0000 721c 0000 0072 1c00 0000  .r7...r....r....
-00000880: 721d 0000 00da 1063 6865 636b 5f65 6c61  r......check_ela
-00000890: 7a5f 7368 6170 653d 0000 0073 1200 0000  z_shape=...s....
-000008a0: 1404 1801 0c01 0801 04ff 0203 0201 04ff  ................
-000008b0: 08fb 723b 0000 00da 0668 6569 6768 7472  ..r;.....heightr
-000008c0: 3800 0000 da03 706f 73fa 1a54 7570 6c65  8.....pos..Tuple
-000008d0: 5b66 6c6f 6174 2c20 666c 6f61 742c 2066  [float, float, f
-000008e0: 6c6f 6174 5dfa 285b 666c 6f61 7420 7c20  loat].([float | 
-000008f0: 6e70 2e6e 6461 7272 6179 2c20 666c 6f61  np.ndarray, floa
-00000900: 7420 7c20 6e70 2e6e 6461 7272 6179 5d63  t | np.ndarray]c
-00000910: 0400 0000 0000 0000 0000 0000 0800 0000  ................
-00000920: 0500 0000 4300 0001 7342 0000 0074 0074  ....C...sB...t.t
-00000930: 01a0 0264 017c 0018 00a1 017c 0264 0214  ...d.|.....|.d..
-00000940: 0083 027d 0474 037c 017c 007c 0467 037c  ...}.t.|.|.|.g.|
-00000950: 03a2 0152 0064 0374 0483 0069 018e 015c  ...R.d.t...i...\
-00000960: 037d 057d 067d 077c 057c 0666 0253 0029  .}.}.}.|.|.f.S.)
-00000970: 0461 9601 0000 0a20 2020 2043 6f6e 7665  .a.....    Conve
-00000980: 7274 7320 7669 7369 626c 6520 656c 6576  rts visible elev
-00000990: 6174 696f 6e20 616e 6420 617a 696d 7574  ation and azimut
-000009a0: 6820 746f 2067 656f 6772 6170 6869 6320  h to geographic 
-000009b0: 636f 6f72 6469 6e61 7465 7320 7769 7468  coordinates with
-000009c0: 2067 6976 656e 2068 6569 6768 7420 6f66   given height of
-000009d0: 2074 6865 2076 6973 6962 6c65 2070 6f69   the visible poi
-000009e0: 6e74 2e0a 0a20 2020 203a 7061 7261 6d20  nt...    :param 
-000009f0: 656c 3a20 456c 6576 6174 696f 6e20 6f66  el: Elevation of
-00000a00: 206f 6273 6572 7661 7469 6f6e 2873 2920   observation(s) 
-00000a10: 696e 2064 6567 2e0a 2020 2020 3a70 6172  in deg..    :par
-00000a20: 616d 2061 7a3a 2041 7a69 6d75 7468 206f  am az: Azimuth o
-00000a30: 6620 6f62 7365 7276 6174 696f 6e28 7329  f observation(s)
-00000a40: 2069 6e20 6465 672e 0a20 2020 203a 7061   in deg..    :pa
-00000a50: 7261 6d20 6865 6967 6874 3a20 4865 6967  ram height: Heig
-00000a60: 6874 206f 6620 6f62 7365 7276 6162 6c65  ht of observable
-00000a70: 2070 6f69 6e74 2873 2920 696e 206b 6d2e   point(s) in km.
-00000a80: 0a20 2020 203a 7061 7261 6d20 706f 733a  .    :param pos:
-00000a90: 2047 656f 6772 6170 6869 6361 6c20 636f   Geographical co
-00000aa0: 6f72 6469 6e61 7465 7320 616e 6420 6865  ordinates and he
-00000ab0: 6967 6874 2069 6e20 6d20 6f66 2074 6865  ight in m of the
-00000ac0: 2074 656c 6573 636f 7065 0a20 2020 203a   telescope.    :
-00000ad0: 7265 7475 726e 3a20 4f62 7365 7276 6162  return: Observab
-00000ae0: 6c65 2067 656f 6772 6170 6869 6361 6c20  le geographical 
-00000af0: 6c61 7469 7475 6465 2061 6e64 206c 6f6e  latitude and lon
-00000b00: 6769 7475 6465 2e0a 2020 2020 e95a 0000  gitude..    .Z..
-00000b10: 0067 0000 0000 0040 8f40 da03 656c 6c29  .g.....@.@..ell)
-00000b20: 0572 0c00 0000 722d 0000 00da 0764 6567  .r....r-.....deg
-00000b30: 3272 6164 7208 0000 0072 0900 0000 2908  2radr....r....).
-00000b40: 7235 0000 0072 3700 0000 723c 0000 0072  r5...r7...r<...r
-00000b50: 3d00 0000 da08 645f 7372 616e 6765 da07  =.....d_srange..
-00000b60: 6f62 735f 6c61 74da 076f 6273 5f6c 6f6e  obs_lat..obs_lon
-00000b70: da01 5f72 1c00 0000 721c 0000 0072 1d00  .._r....r....r..
-00000b80: 0000 da06 736b 7932 6c6c 4b00 0000 7306  ....sky2llK...s.
-00000b90: 0000 0018 0f22 0108 0172 4700 0000 da08  ....."...rG.....
-00000ba0: 6772 6964 7369 7a65 da03 696e 74fa 185b  gridsize..int..[
-00000bb0: 6e70 2e6e 6461 7272 6179 2c20 6e70 2e6e  np.ndarray, np.n
-00000bc0: 6461 7272 6179 5d63 0100 0000 0000 0000  darray]c........
-00000bd0: 0000 0000 0500 0000 0600 0000 4300 0001  ............C...
-00000be0: 7338 0000 0074 006a 0164 0164 027c 0064  s8...t.j.d.d.|.d
-00000bf0: 0364 048d 047d 0174 00a0 0164 0164 057c  .d...}.t...d.d.|
-00000c00: 00a1 037d 0274 00a0 027c 017c 02a1 025c  ...}.t...|.|...\
-00000c10: 027d 037d 047c 037c 0466 0253 0029 067a  .}.}.|.|.f.S.).z
-00000c20: 6f0a 2020 2020 3a70 6172 616d 2067 7269  o.    :param gri
-00000c30: 6473 697a 653a 2047 7269 6420 7265 736f  dsize: Grid reso
-00000c40: 6c75 7469 6f6e 2e0a 2020 2020 3a72 6574  lution..    :ret
-00000c50: 7572 6e3a 204d 6573 6867 7269 6420 6f66  urn: Meshgrid of
-00000c60: 2065 6c65 7661 7469 6f6e 2061 6e64 2061   elevation and a
-00000c70: 7a69 6d75 7468 2066 6f72 2061 6c6c 2076  zimuth for all v
-00000c80: 6973 6962 6c65 2073 6b79 2e0a 2020 2020  isible sky..    
-00000c90: 7201 0000 0072 4000 0000 5429 01da 0865  r....r@...T)...e
-00000ca0: 6e64 706f 696e 7469 6801 0000 2903 722d  ndpointih...).r-
-00000cb0: 0000 00da 086c 696e 7370 6163 65da 086d  .....linspace..m
-00000cc0: 6573 6867 7269 6429 0572 4800 0000 7235  eshgrid).rH...r5
-00000cd0: 0000 0072 3700 0000 da03 656c 73da 0361  ...r7.....els..a
-00000ce0: 7a73 721c 0000 0072 1c00 0000 721d 0000  zsr....r....r...
-00000cf0: 00da 0965 6c61 7a5f 6d65 7368 5f00 0000  ...elaz_mesh_...
-00000d00: 7308 0000 0012 050e 0110 0108 0172 5000  s............rP.
-00000d10: 0000 da05 6e73 6964 65da 0870 6f73 6974  ....nside..posit
-00000d20: 696f 6efa 1d53 6571 7565 6e63 655b 666c  ion..Sequence[fl
-00000d30: 6f61 742c 2066 6c6f 6174 2c20 666c 6f61  oat, float, floa
-00000d40: 745d da04 6862 6f74 da04 6874 6f70 da07  t]..hbot..htop..
-00000d50: 6e6c 6179 6572 73da 0a6f 6273 5f70 6978  nlayers..obs_pix
-00000d60: 656c 73fa 0d53 6571 7565 6e63 655b 696e  els..Sequence[in
-00000d70: 745d da04 6461 7461 da05 6c61 7965 72fa  t]..data..layer.
-00000d80: 0a69 6e74 207c 204e 6f6e 6563 0a00 0000  .int | Nonec....
-00000d90: 0000 0000 0000 0000 1000 0000 0700 0000  ................
-00000da0: 4300 0001 7322 0100 0074 007c 007c 0183  C...s"...t.|.|..
-00000db0: 0201 0074 01a0 027c 047c 057c 06a1 037d  ...t...|.|.|...}
-00000dc0: 0a74 01a0 0374 04a0 057c 02a1 01a1 0174  .t...t...|.....t
-00000dd0: 046a 0617 007d 0b7c 0964 0175 0072 5b74  .j...}.|.d.u.r[t
-00000de0: 01a0 0767 007c 006a 08a2 017c 0691 0152  ...g.|.j...|...R
-00000df0: 00a1 017d 0c74 097c 0683 0144 005d 2a7d  ...}.t.|...D.]*}
-00000e00: 0d7c 0864 0164 0185 027c 0d66 0219 007c  .|.d.d...|.f...|
-00000e10: 0b7c 073c 0074 0a7c 007c 017c 0a7c 0d19  .|.<.t.|.|.|.|..
-00000e20: 007c 0383 045c 027d 0e7d 0f74 046a 0b6a  .|...\.}.}.t.j.j
-00000e30: 0c7c 0b7c 0f7c 0e64 0264 038d 047c 0c64  .|.|.|.d.d...|.d
-00000e40: 0164 0185 0264 0164 0185 027c 0d66 033c  .d...d.d...|.f.<
-00000e50: 0071 2a7c 0c6a 0d64 0464 058d 0153 0074  .q*|.j.d.d...S.t
-00000e60: 0e7c 0974 0f83 0272 877c 097c 0664 0617  .|.t...r.|.|.d..
-00000e70: 006b 0072 877c 0864 0164 0185 027c 0966  .k.r.|.d.d...|.f
-00000e80: 0219 007c 0b7c 073c 0074 0a7c 007c 017c  ...|.|.<.t.|.|.|
-00000e90: 0a7c 0919 007c 0383 045c 027d 0e7d 0f74  .|...|...\.}.}.t
-00000ea0: 046a 0b6a 0c7c 0b7c 0f7c 0e64 0264 038d  .j.j.|.|.|.d.d..
-00000eb0: 047d 0c7c 0c53 0074 1064 077c 0664 0618  .}.|.S.t.d.|.d..
-00000ec0: 009b 0064 089d 0383 0182 0129 0961 b202  ...d.......).a..
-00000ed0: 0000 0a20 2020 2043 616c 6375 6c61 7465  ...    Calculate
-00000ee0: 7320 696e 7465 7270 6f6c 6174 6564 2076  s interpolated v
-00000ef0: 616c 7565 7320 6f6e 2068 6561 6c70 6978  alues on healpix
-00000f00: 2067 7269 642e 0a0a 2020 2020 3a70 6172   grid...    :par
-00000f10: 616d 2065 6c3a 2045 6c65 7661 7469 6f6e  am el: Elevation
-00000f20: 2e0a 2020 2020 3a70 6172 616d 2061 7a3a  ..    :param az:
-00000f30: 2041 7a69 6d75 7468 2e0a 2020 2020 3a70   Azimuth..    :p
-00000f40: 6172 616d 206e 7369 6465 3a20 5265 736f  aram nside: Reso
-00000f50: 6c75 7469 6f6e 206f 6620 6865 616c 7069  lution of healpi
-00000f60: 7820 6772 6964 2e0a 2020 2020 3a70 6172  x grid..    :par
-00000f70: 616d 2070 6f73 6974 696f 6e3a 0a20 2020  am position:.   
-00000f80: 203a 7061 7261 6d20 6862 6f74 3a20 4c6f   :param hbot: Lo
-00000f90: 7765 7220 6c69 6d69 7420 696e 205b 6b6d  wer limit in [km
-00000fa0: 5d20 6f66 2074 6865 206c 6179 6572 2e0a  ] of the layer..
-00000fb0: 2020 2020 3a70 6172 616d 2068 746f 703a      :param htop:
-00000fc0: 2055 7070 6572 206c 696d 6974 2069 6e20   Upper limit in 
-00000fd0: 5b6b 6d5d 206f 6620 7468 6520 6c61 7965  [km] of the laye
-00000fe0: 722e 0a20 2020 203a 7061 7261 6d20 6e6c  r..    :param nl
-00000ff0: 6179 6572 733a 204e 756d 6265 7220 6f66  ayers: Number of
-00001000: 2073 7562 2d6c 6179 6572 7320 7573 6564   sub-layers used
-00001010: 2066 6f72 2069 6e74 6572 6d65 6469 6174   for intermediat
-00001020: 6520 6361 6c63 756c 6174 696f 6e73 2e0a  e calculations..
-00001030: 2020 2020 3a70 6172 616d 206f 6273 5f70      :param obs_p
-00001040: 6978 656c 733a 204c 6973 7420 6f66 2070  ixels: List of p
-00001050: 6978 656c 2069 6e64 6963 6573 2069 6e73  ixel indices ins
-00001060: 6964 6520 7468 6520 7669 7369 626c 6520  ide the visible 
-00001070: 6469 736b 206f 6e20 6865 616c 7069 7820  disk on healpix 
-00001080: 7370 6865 7265 2e0a 2020 2020 3a70 6172  sphere..    :par
-00001090: 616d 2064 6174 613a 2041 2064 6174 6120  am data: A data 
-000010a0: 746f 2069 6e74 6572 706f 6c61 7465 2e0a  to interpolate..
-000010b0: 2020 2020 3a70 6172 616d 206c 6179 6572      :param layer
-000010c0: 3a20 4e75 6d62 6572 206f 6620 7375 626c  : Number of subl
-000010d0: 6179 6572 2066 726f 6d20 7468 6520 7072  ayer from the pr
-000010e0: 6563 616c 6375 6c61 7465 6420 7375 626c  ecalculated subl
-000010f0: 6179 6572 732e 0a20 2020 2020 2020 2020  ayers..         
-00001100: 2020 2020 2020 2020 2049 6620 4e6f 6e65           If None
-00001110: 202d 2061 6e20 6176 6572 6167 6520 6f76   - an average ov
-00001120: 6572 2061 6c6c 206c 6179 6572 7320 6973  er all layers is
-00001130: 2072 6574 7572 6e65 642e 0a20 2020 203a   returned..    :
-00001140: 7265 7475 726e 3a20 496e 7465 7270 6f6c  return: Interpol
-00001150: 6174 6564 2076 616c 7565 7320 6174 2073  ated values at s
-00001160: 7065 6369 6669 6564 2065 6c65 7661 7469  pecified elevati
-00001170: 6f6e 2061 6e64 2061 7a69 6d75 7468 2e0a  on and azimuth..
-00001180: 2020 2020 4e54 2901 da06 6c6f 6e6c 6174      NT)...lonlat
-00001190: e902 0000 0029 01da 0461 7869 7372 0b00  .....)...axisr..
-000011a0: 0000 7a34 5468 6520 6c61 7965 7220 7661  ..z4The layer va
-000011b0: 6c75 6520 6d75 7374 2062 6520 696e 7465  lue must be inte
-000011c0: 6765 7220 616e 6420 6265 2069 6e20 7261  ger and be in ra
-000011d0: 6e67 6520 5b30 2c20 fa01 5d29 1172 3b00  nge [0, ..]).r;.
-000011e0: 0000 722d 0000 0072 4c00 0000 da05 7a65  ..r-...rL.....ze
-000011f0: 726f 73da 0268 70da 0a6e 7369 6465 326e  ros..hp..nside2n
-00001200: 7069 78da 0655 4e53 4545 4eda 0565 6d70  pix..UNSEEN..emp
-00001210: 7479 7239 0000 00da 0572 616e 6765 7247  tyr9.....rangerG
-00001220: 0000 00da 0970 6978 656c 6675 6e63 da0e  .....pixelfunc..
-00001230: 6765 745f 696e 7465 7270 5f76 616c da04  get_interp_val..
-00001240: 6d65 616e 7230 0000 0072 4900 0000 723a  meanr0...rI...r:
-00001250: 0000 0029 1072 3500 0000 7237 0000 0072  ...).r5...r7...r
-00001260: 5100 0000 7252 0000 0072 5400 0000 7255  Q...rR...rT...rU
-00001270: 0000 0072 5600 0000 7257 0000 0072 5900  ...rV...rW...rY.
-00001280: 0000 725a 0000 00da 0768 6569 6768 7473  ..rZ.....heights
-00001290: da04 6d61 705f da03 7265 73da 0169 7244  ..map_..res..irD
-000012a0: 0000 0072 4500 0000 721c 0000 0072 1c00  ...rE...r....r..
-000012b0: 0000 721d 0000 00da 0a65 7661 6c5f 6c61  ..r......eval_la
-000012c0: 7965 726a 0000 0073 2800 0000 0a1c 0e01  yerj...s(.......
-000012d0: 1601 0801 1601 0c01 1401 1601 0601 0801  ................
-000012e0: 1aff 0c03 1601 1401 1601 1401 0401 0202  ................
-000012f0: 0e01 04ff 726d 0000 00e9 1400 0000 da07  ....rm..........
-00001300: 6c69 6278 3236 34da 0569 6d64 6972 da03  libx264..imdir..
-00001310: 7374 72da 0673 6176 6574 6fda 0366 7073  str..saveto..fps
-00001320: da04 6465 7363 fa0a 7374 7220 7c20 4e6f  ..desc..str | No
-00001330: 6e65 da05 636f 6465 6363 0500 0000 0000  ne..codecc......
-00001340: 0000 0000 0000 0900 0000 0900 0000 4300  ..............C.
-00001350: 0001 7398 0000 007c 01a0 0064 01a1 0173  ..s....|...d...s
-00001360: 097c 0164 0137 007d 017c 0370 0c64 027d  .|.d.7.}.|.p.d.}
-00001370: 0364 0364 047c 029b 0064 0574 016a 02a0  .d.d.|...d.t.j..
-00001380: 037c 0064 06a1 0264 077c 0464 087c 0167  .|.d...d.|.d.|.g
-00001390: 097d 0574 047c 0583 017d 0674 0564 0964  .}.t.|...}.t.d.d
-000013a0: 0a7c 0364 0b64 0c8d 048f 187d 077c 06a0  .|.d.d.....}.|..
-000013b0: 06a1 0044 005d 0a7d 087c 07a0 077c 087c  ...D.].}.|...|.|
-000013c0: 076a 0818 00a1 0101 0071 2f57 0064 0d04  .j.......q/W.d..
-000013d0: 0004 0083 0301 0064 0d53 0031 0073 4577  .......d.S.1.sEw
-000013e0: 0101 0001 0001 0059 0001 0064 0d53 0029  .......Y...d.S.)
-000013f0: 0e61 5501 0000 0a20 2020 2052 656e 6465  .aU....    Rende
-00001400: 7273 2065 7869 7374 696e 6720 7365 7420  rs existing set 
-00001410: 6f66 2070 6963 7475 7265 7320 746f 206d  of pictures to m
-00001420: 7034 2076 6964 656f 2e0a 2020 2020 3a70  p4 video..    :p
-00001430: 6172 616d 2069 6d64 6972 3a20 4c6f 6361  aram imdir: Loca
-00001440: 7469 6f6e 206f 6620 696d 6167 6573 2e0a  tion of images..
-00001450: 2020 2020 3a70 6172 616d 2073 6176 6574      :param savet
-00001460: 6f3a 2050 6174 6820 7769 7468 206e 616d  o: Path with nam
-00001470: 6520 746f 2077 6865 7265 2073 6176 6520  e to where save 
-00001480: 7468 6520 6669 6c65 2e0a 2020 2020 3a70  the file..    :p
-00001490: 6172 616d 2066 7073 3a20 4672 616d 6572  aram fps: Framer
-000014a0: 6174 6520 2d20 6672 616d 6573 2070 6572  ate - frames per
-000014b0: 2073 6563 6f6e 642e 0a20 2020 203a 7061   second..    :pa
-000014c0: 7261 6d20 6465 7363 3a20 4465 7363 7269  ram desc: Descri
-000014d0: 7074 696f 6e20 6f66 2061 2070 726f 6772  ption of a progr
-000014e0: 6573 7362 6172 2e20 4966 204e 6f6e 6520  essbar. If None 
-000014f0: 2d20 7468 6520 7072 6f67 7265 7373 6261  - the progressba
-00001500: 7220 7769 6c6c 206e 6f74 2061 7070 6561  r will not appea
-00001510: 722e 0a20 2020 203a 7061 7261 6d20 636f  r..    :param co
-00001520: 6465 633a 2043 6f64 6563 2074 6f20 7573  dec: Codec to us
-00001530: 6520 666f 7220 7669 6465 6f20 7265 6e64  e for video rend
-00001540: 6572 696e 672e 0a20 2020 207a 042e 6d70  ering..    z..mp
-00001550: 347a 0f52 656e 6465 7269 6e67 2076 6964  4z.Rendering vid
-00001560: 656f da06 6666 6d70 6567 7a02 2d72 7a02  eo..ffmpegz.-rz.
-00001570: 2d69 7a08 2530 3664 2e70 6e67 7a07 2d76  -iz.%06d.pngz.-v
-00001580: 636f 6465 637a 022d 79e9 6400 0000 7201  codecz.-y.d...r.
-00001590: 0000 0054 2904 da05 746f 7461 6c72 5200  ...T)...totalrR.
-000015a0: 0000 7274 0000 00da 056c 6561 7665 4e29  ..rt.....leaveN)
-000015b0: 09da 0865 6e64 7377 6974 68da 026f 73da  ...endswith..os.
-000015c0: 0470 6174 68da 046a 6f69 6e72 0700 0000  .path..joinr....
-000015d0: 720a 0000 00da 1972 756e 5f63 6f6d 6d61  r......run_comma
-000015e0: 6e64 5f77 6974 685f 7072 6f67 7265 7373  nd_with_progress
-000015f0: da06 7570 6461 7465 da01 6e29 0972 7000  ..update..n).rp.
-00001600: 0000 7272 0000 0072 7300 0000 7274 0000  ..rr...rs...rt..
-00001610: 0072 7600 0000 da03 636d 64da 0266 66da  .rv.....cmd..ff.
-00001620: 0470 6261 72da 0870 726f 6772 6573 7372  .pbar..progressr
-00001630: 1c00 0000 721c 0000 0072 1d00 0000 da07  ....r....r......
-00001640: 7069 6332 7669 649d 0000 0073 2600 0000  pic2vid....s&...
-00001650: 0a0f 0801 0801 0202 0201 0401 0201 0c01  ................
-00001660: 0201 0201 0201 0201 04f7 080b 1201 0c01  ................
-00001670: 1201 02ff 22ff 7286 0000 0063 0100 0000  ....".r....c....
-00001680: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00001690: 4300 0001 f316 0000 007c 0064 0119 006a  C........|.d...j
-000016a0: 007c 0064 0264 0085 0219 008e 0053 00a9  .|.d.d.......S..
-000016b0: 034e 7201 0000 0072 0b00 0000 2901 da05  .Nr....r....)...
-000016c0: 6174 7465 6ea9 01da 0461 7267 7372 1c00  atten....argsr..
-000016d0: 0000 721c 0000 0072 1d00 0000 da14 6765  ..r....r......ge
-000016e0: 745f 6174 7465 6e5f 6672 6f6d 5f66 7261  t_atten_from_fra
-000016f0: 6d65 c000 0000 f302 0000 0016 0172 8c00  me...........r..
-00001700: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001710: 0000 0004 0000 0043 0000 0172 8700 0000  .......C...r....
-00001720: 7288 0000 0029 01da 0472 6566 7272 8a00  r....)...refrr..
-00001730: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00001740: 00da 1367 6574 5f72 6566 725f 6672 6f6d  ...get_refr_from
-00001750: 5f66 7261 6d65 c400 0000 728d 0000 0072  _frame....r....r
-00001760: 8f00 0000 2904 7229 0000 0072 2a00 0000  ....).r)...r*...
-00001770: 722b 0000 0072 2c00 0000 2904 7235 0000  r+...r,...).r5..
-00001780: 0072 3600 0000 7237 0000 0072 3600 0000  .r6...r7...r6...
-00001790: 290a 7235 0000 0072 3600 0000 7237 0000  ).r5...r6...r7..
-000017a0: 0072 3600 0000 723c 0000 0072 3800 0000  .r6...r<...r8...
-000017b0: 723d 0000 0072 3e00 0000 722b 0000 0072  r=...r>...r+...r
-000017c0: 3f00 0000 2904 7248 0000 0072 4900 0000  ?...).rH...rI...
-000017d0: 722b 0000 0072 4a00 0000 2901 4e29 1472  r+...rJ...).N).r
-000017e0: 3500 0000 7236 0000 0072 3700 0000 7236  5...r6...r7...r6
-000017f0: 0000 0072 5100 0000 7249 0000 0072 5200  ...rQ...rI...rR.
-00001800: 0000 7253 0000 0072 5400 0000 7238 0000  ..rS...rT...r8..
-00001810: 0072 5500 0000 7238 0000 0072 5600 0000  .rU...r8...rV...
-00001820: 7249 0000 0072 5700 0000 7258 0000 0072  rI...rW...rX...r
-00001830: 5900 0000 7236 0000 0072 5a00 0000 725b  Y...r6...rZ...r[
-00001840: 0000 0029 0372 6e00 0000 4e72 6f00 0000  ...).rn...Nro...
-00001850: 290a 7270 0000 0072 7100 0000 7272 0000  ).rp...rq...rr..
-00001860: 0072 7100 0000 7273 0000 0072 4900 0000  .rq...rs...rI...
-00001870: 7274 0000 0072 7500 0000 7276 0000 0072  rt...ru...rv...r
-00001880: 7100 0000 291f da0a 5f5f 6675 7475 7265  q...)...__future
-00001890: 5f5f 7202 0000 0072 7c00 0000 da06 7479  __r....r|.....ty
-000018a0: 7069 6e67 7203 0000 0072 0400 0000 7205  pingr....r....r.
-000018b0: 0000 0072 0600 0000 da06 6865 616c 7079  ...r......healpy
-000018c0: 7261 0000 00da 056e 756d 7079 722d 0000  ra.....numpyr-..
-000018d0: 00da 1566 666d 7065 675f 7072 6f67 7265  ...ffmpeg_progre
-000018e0: 7373 5f79 6965 6c64 7207 0000 00da 0770  ss_yieldr......p
-000018f0: 796d 6170 3364 7208 0000 0072 0900 0000  ymap3dr....r....
-00001900: da0b 706d 456c 6c69 7073 6f69 6472 0a00  ..pmEllipsoidr..
-00001910: 0000 da09 696f 6e5f 746f 6f6c 7372 0c00  ....ion_toolsr..
-00001920: 0000 720d 0000 0072 2f00 0000 7234 0000  ..r....r/...r4..
-00001930: 0072 3b00 0000 7247 0000 0072 5000 0000  .r;...rG...rP...
-00001940: 726d 0000 0072 8600 0000 728c 0000 0072  rm...r....r....r
-00001950: 8f00 0000 721c 0000 0072 1c00 0000 721c  ....r....r....r.
-00001960: 0000 0072 1d00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001970: 653e 0100 0000 7330 0000 000c 0008 0218  e>....s0........
-00001980: 0108 0208 010c 0110 010c 010c 020e 0310  ................
-00001990: 110a 0e08 090a 060a 0e0a 1402 150c f602  ................
-000019a0: 3602 0102 010c fb08 230c 04              6.......#..
+00000050: 0100 6400 6402 6c06 5a07 6400 6402 6c08  ..d.d.l.Z.d.d.l.
+00000060: 5a09 6400 6404 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
+00000070: 6405 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6400  d.l.m.Z.m.Z...d.
+00000080: 6406 6c0f 6d0f 5a0f 0100 6407 6408 6c10  d.l.m.Z...d.d.l.
+00000090: 6d11 5a11 0100 6409 5a12 4700 640a 640b  m.Z...d.Z.G.d.d.
+000000a0: 8400 640b 8302 5a13 6440 6410 6411 8404  ..d...Z.d@d.d...
+000000b0: 5a14 6412 6413 8400 5a15 6441 6417 6418  Z.d.d...Z.dAd.d.
+000000c0: 8404 5a16 6442 641e 641f 8404 5a17 6443  ..Z.dBd.d...Z.dC
+000000d0: 6423 6424 8404 5a18 0902 6444 6445 642f  d#d$..Z...dDdEd/
+000000e0: 6430 8405 5a19 0931 0902 0932 6446 6447  d0..Z..1...2dFdG
+000000f0: 643a 643b 8405 5a1a 643c 643d 8400 5a1b  d:d;..Z.d<d=..Z.
+00000100: 643e 643f 8400 5a1c 6402 5300 2948 e900  d>d?..Z.d.S.)H..
+00000110: 0000 0029 01da 0b61 6e6e 6f74 6174 696f  ...)...annotatio
+00000120: 6e73 4e29 02da 0849 7465 7261 626c 65da  nsN)...Iterable.
+00000130: 0853 6571 7565 6e63 6529 01da 0e46 666d  .Sequence)...Ffm
+00000140: 7065 6750 726f 6772 6573 7329 02da 0c61  pegProgress)...a
+00000150: 6572 3267 656f 6465 7469 63da 0945 6c6c  er2geodetic..Ell
+00000160: 6970 736f 6964 2901 da04 7471 646d e901  ipsoid)...tqdm..
+00000170: 0000 0029 01da 0673 7261 6e67 6567 0000  ...)...srangeg..
+00000180: 0000 9d54 5841 6300 0000 0000 0000 0000  ...TXAc.........
+00000190: 0000 0000 0000 0001 0000 0040 0000 0173  ...........@...s
+000001a0: 3800 0000 6500 5a01 6400 5a02 6401 5a03  8...e.Z.d.Z.d.Z.
+000001b0: 6402 5a04 6403 5a05 6404 5a06 6405 5a07  d.Z.d.Z.d.Z.d.Z.
+000001c0: 6406 5a08 6407 5a09 6408 5a0a 6409 5a0b  d.Z.d.Z.d.Z.d.Z.
+000001d0: 640a 5a0c 640b 5a0d 640c 5300 290d da09  d.Z.d.Z.d.S.)...
+000001e0: 5465 7874 436f 6c6f 727a 390a 2020 2020  TextColorz9.    
+000001f0: 5072 6f76 6964 6573 2066 6f72 6d61 7474  Provides formatt
+00000200: 6572 7320 666f 7220 7465 726d 696e 616c  ers for terminal
+00000210: 2074 6578 7420 636f 6c6f 7269 6e67 2e0a   text coloring..
+00000220: 2020 2020 7a05 1b5b 3935 6d7a 051b 5b39      z..[95mz..[9
+00000230: 366d 7a05 1b5b 3336 6d7a 051b 5b39 346d  6mz..[36mz..[94m
+00000240: 7a05 1b5b 3932 6d7a 051b 5b39 336d 7a05  z..[92mz..[93mz.
+00000250: 1b5b 3931 6d7a 041b 5b31 6d7a 041b 5b34  .[91mz..[1mz..[4
+00000260: 6d7a 041b 5b30 6d4e 290e da08 5f5f 6e61  mz..[0mN)...__na
+00000270: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000280: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000290: 5f5f 646f 635f 5fda 0650 5552 504c 45da  __doc__..PURPLE.
+000002a0: 0443 5941 4eda 0844 4152 4b43 5941 4eda  .CYAN..DARKCYAN.
+000002b0: 0442 4c55 45da 0547 5245 454e da06 5945  .BLUE..GREEN..YE
+000002c0: 4c4c 4f57 da03 5245 44da 0442 4f4c 44da  LLOW..RED..BOLD.
+000002d0: 0955 4e44 4552 4c49 4e45 da03 454e 44a9  .UNDERLINE..END.
+000002e0: 0072 1a00 0000 721a 0000 00fa 3d2f 686f  .r....r.....=/ho
+000002f0: 6d65 2f6c 6170 3164 656d 2f64 6576 2d70  me/lap1dem/dev-p
+00000300: 7974 686f 6e2f 6469 6f6e 7079 2f73 7263  ython/dionpy/src
+00000310: 2f64 696f 6e70 792f 6d6f 6475 6c65 732f  /dionpy/modules/
+00000320: 6865 6c70 6572 732e 7079 720b 0000 0011  helpers.pyr.....
+00000330: 0000 0073 1800 0000 0800 0401 0404 0401  ...s............
+00000340: 0401 0401 0401 0401 0401 0401 0401 0801  ................
+00000350: 720b 0000 00da 0476 616c 73fa 0f4e 6f6e  r......vals..Non
+00000360: 6520 7c20 4974 6572 6162 6c65 da06 7265  e | Iterable..re
+00000370: 7475 726e fa11 6e70 2e6e 6461 7272 6179  turn..np.ndarray
+00000380: 207c 204e 6f6e 6563 0100 0000 0000 0000   | Nonec........
+00000390: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
+000003a0: 7316 0000 007c 0064 0175 0072 0664 0153  s....|.d.u.r.d.S
+000003b0: 0074 00a0 017c 00a1 0153 0029 027a 560a  .t...|...S.).zV.
+000003c0: 2020 2020 5573 6564 2066 6f72 2064 6174      Used for dat
+000003d0: 6120 6c6f 6164 696e 6720 6672 6f6d 2048  a loading from H
+000003e0: 4446 2066 696c 6573 2e20 436f 6e76 6572  DF files. Conver
+000003f0: 7473 206e 6f74 204e 6f6e 6520 7661 6c75  ts not None valu
+00000400: 6573 2074 6f20 6e70 2e61 7272 6179 732e  es to np.arrays.
+00000410: 0a20 2020 204e 2902 da02 6e70 da05 6172  .    N)...np..ar
+00000420: 7261 7929 0172 1c00 0000 721a 0000 0072  ray).r....r....r
+00000430: 1a00 0000 721b 0000 00da 0d6e 6f6e 655f  ....r......none_
+00000440: 6f72 5f61 7272 6179 2100 0000 7306 0000  or_array!...s...
+00000450: 0008 0404 010a 0172 2200 0000 6301 0000  .......r"...c...
+00000460: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000470: 0043 0000 0173 1e00 0000 7400 7c00 7401  .C...s....t.|.t.
+00000480: 8302 730b 7400 7c00 7402 6a03 8302 720d  ..s.t.|.t.j...r.
+00000490: 6401 5300 6402 5300 2903 4e54 4629 04da  d.S.d.S.).NTF)..
+000004a0: 0a69 7369 6e73 7461 6e63 65da 046c 6973  .isinstance..lis
+000004b0: 7472 2000 0000 da07 6e64 6172 7261 7929  tr .....ndarray)
+000004c0: 01da 0178 721a 0000 0072 1a00 0000 721b  ...xr....r....r.
+000004d0: 0000 00da 0b69 735f 6974 6572 6162 6c65  .....is_iterable
+000004e0: 2a00 0000 7306 0000 0016 0104 0104 0172  *...s..........r
+000004f0: 2700 0000 da02 656c fa12 666c 6f61 7420  '.....el..float 
+00000500: 7c20 6e70 2e6e 6461 7272 6179 da02 617a  | np.ndarray..az
+00000510: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00000520: 0003 0000 0043 0000 0173 5400 0000 7400  .....C...sT...t.
+00000530: 7c00 7401 8302 7326 7400 7c01 7401 8302  |.t...s&t.|.t...
+00000540: 7328 7400 7c00 7402 6a03 8302 7222 7400  s(t.|.t.j...r"t.
+00000550: 7c00 7402 6a03 8302 7222 7c00 6a04 7c01  |.t.j...r"|.j.|.
+00000560: 6a04 6b02 7320 7405 6401 8301 8201 6403  j.k.s t.d.....d.
+00000570: 5300 7405 6402 8301 8201 6403 5300 6403  S.t.d.....d.S.d.
+00000580: 5300 2904 7a3f 0a20 2020 2043 6865 636b  S.).z?.    Check
+00000590: 7320 7368 6170 6520 616e 6420 7479 7065  s shape and type
+000005a0: 206f 6620 696e 7075 7420 656c 6576 6174   of input elevat
+000005b0: 696f 6e20 616e 6420 617a 696d 7574 682e  ion and azimuth.
+000005c0: 0a20 2020 207a 2e45 6c65 7661 7469 6f6e  .    z.Elevation
+000005d0: 2061 6e64 2061 7a69 6d75 7468 206d 7573   and azimuth mus
+000005e0: 7420 6265 2074 6865 2073 616d 6520 6c65  t be the same le
+000005f0: 6e67 7468 2e7a 3c45 6c65 7661 7469 6f6e  ngth.z<Elevation
+00000600: 2061 6e64 2061 7a69 6d75 7468 206d 7573   and azimuth mus
+00000610: 7420 6265 2065 6974 6865 7220 666c 6f61  t be either floa
+00000620: 7473 206f 7220 6e75 6d70 7920 6172 7261  ts or numpy arra
+00000630: 7973 2e4e 2906 7223 0000 00da 0566 6c6f  ys.N).r#.....flo
+00000640: 6174 7220 0000 0072 2500 0000 da05 7368  atr ...r%.....sh
+00000650: 6170 65da 0a56 616c 7565 4572 726f 7229  ape..ValueError)
+00000660: 0272 2800 0000 722a 0000 0072 1a00 0000  .r(...r*...r....
+00000670: 721a 0000 0072 1b00 0000 da10 6368 6563  r....r......chec
+00000680: 6b5f 656c 617a 5f73 6861 7065 3000 0000  k_elaz_shape0...
+00000690: 7312 0000 0014 0418 010c 0108 0104 ff02  s...............
+000006a0: 0302 0104 ff08 fb72 2e00 0000 da06 6865  .......r......he
+000006b0: 6967 6874 722b 0000 00da 0370 6f73 fa1d  ightr+.....pos..
+000006c0: 5365 7175 656e 6365 5b66 6c6f 6174 2c20  Sequence[float, 
+000006d0: 666c 6f61 742c 2066 6c6f 6174 5dfa 285b  float, float].([
+000006e0: 666c 6f61 7420 7c20 6e70 2e6e 6461 7272  float | np.ndarr
+000006f0: 6179 2c20 666c 6f61 7420 7c20 6e70 2e6e  ay, float | np.n
+00000700: 6461 7272 6179 5d63 0400 0000 0000 0000  darray]c........
+00000710: 0000 0000 0800 0000 0600 0000 4300 0001  ............C...
+00000720: 7346 0000 0074 0074 01a0 0264 017c 0018  sF...t.t...d.|..
+00000730: 00a1 017c 0264 0214 0083 027d 0474 037c  ...|.d.....}.t.|
+00000740: 017c 007c 0467 037c 03a2 0152 0064 0374  .|.|.g.|...R.d.t
+00000750: 0474 0574 0583 0269 018e 015c 037d 057d  .t.t...i...\.}.}
+00000760: 067d 077c 057c 0666 0253 0029 0461 9601  .}.|.|.f.S.).a..
+00000770: 0000 0a20 2020 2043 6f6e 7665 7274 7320  ...    Converts 
+00000780: 7669 7369 626c 6520 656c 6576 6174 696f  visible elevatio
+00000790: 6e20 616e 6420 617a 696d 7574 6820 746f  n and azimuth to
+000007a0: 2067 656f 6772 6170 6869 6320 636f 6f72   geographic coor
+000007b0: 6469 6e61 7465 7320 7769 7468 2067 6976  dinates with giv
+000007c0: 656e 2068 6569 6768 7420 6f66 2074 6865  en height of the
+000007d0: 2076 6973 6962 6c65 2070 6f69 6e74 2e0a   visible point..
+000007e0: 0a20 2020 203a 7061 7261 6d20 656c 3a20  .    :param el: 
+000007f0: 456c 6576 6174 696f 6e20 6f66 206f 6273  Elevation of obs
+00000800: 6572 7661 7469 6f6e 2873 2920 696e 2064  ervation(s) in d
+00000810: 6567 2e0a 2020 2020 3a70 6172 616d 2061  eg..    :param a
+00000820: 7a3a 2041 7a69 6d75 7468 206f 6620 6f62  z: Azimuth of ob
+00000830: 7365 7276 6174 696f 6e28 7329 2069 6e20  servation(s) in 
+00000840: 6465 672e 0a20 2020 203a 7061 7261 6d20  deg..    :param 
+00000850: 6865 6967 6874 3a20 4865 6967 6874 206f  height: Height o
+00000860: 6620 6f62 7365 7276 6162 6c65 2070 6f69  f observable poi
+00000870: 6e74 2873 2920 696e 206b 6d2e 0a20 2020  nt(s) in km..   
+00000880: 203a 7061 7261 6d20 706f 733a 2047 656f   :param pos: Geo
+00000890: 6772 6170 6869 6361 6c20 636f 6f72 6469  graphical coordi
+000008a0: 6e61 7465 7320 616e 6420 6865 6967 6874  nates and height
+000008b0: 2069 6e20 6d20 6f66 2074 6865 2074 656c   in m of the tel
+000008c0: 6573 636f 7065 0a20 2020 203a 7265 7475  escope.    :retu
+000008d0: 726e 3a20 4f62 7365 7276 6162 6c65 2067  rn: Observable g
+000008e0: 656f 6772 6170 6869 6361 6c20 6c61 7469  eographical lati
+000008f0: 7475 6465 2061 6e64 206c 6f6e 6769 7475  tude and longitu
+00000900: 6465 2e0a 2020 2020 e95a 0000 0067 0000  de..    .Z...g..
+00000910: 0000 0040 8f40 da03 656c 6c29 0672 0a00  ...@.@..ell).r..
+00000920: 0000 7220 0000 00da 0764 6567 3272 6164  ..r .....deg2rad
+00000930: 7206 0000 0072 0700 0000 da07 525f 4541  r....r......R_EA
+00000940: 5254 4829 0872 2800 0000 722a 0000 0072  RTH).r(...r*...r
+00000950: 2f00 0000 7230 0000 00da 0864 5f73 7261  /...r0.....d_sra
+00000960: 6e67 65da 076f 6273 5f6c 6174 da07 6f62  nge..obs_lat..ob
+00000970: 735f 6c6f 6eda 015f 721a 0000 0072 1a00  s_lon.._r....r..
+00000980: 0000 721b 0000 00da 0673 6b79 326c 6c3e  ..r......sky2ll>
+00000990: 0000 0073 0600 0000 180f 2601 0801 723b  ...s......&...r;
+000009a0: 0000 00da 0867 7269 6473 697a 65da 0369  .....gridsize..i
+000009b0: 6e74 fa18 5b6e 702e 6e64 6172 7261 792c  nt..[np.ndarray,
+000009c0: 206e 702e 6e64 6172 7261 795d 6301 0000   np.ndarray]c...
+000009d0: 0000 0000 0000 0000 0005 0000 0006 0000  ................
+000009e0: 0043 0000 0173 3800 0000 7400 6a01 6401  .C...s8...t.j.d.
+000009f0: 6402 7c00 6403 6404 8d04 7d01 7400 a001  d.|.d.d...}.t...
+00000a00: 6401 6405 7c00 a103 7d02 7400 a002 7c01  d.d.|...}.t...|.
+00000a10: 7c02 a102 5c02 7d03 7d04 7c03 7c04 6602  |...\.}.}.|.|.f.
+00000a20: 5300 2906 7a6f 0a20 2020 203a 7061 7261  S.).zo.    :para
+00000a30: 6d20 6772 6964 7369 7a65 3a20 4772 6964  m gridsize: Grid
+00000a40: 2072 6573 6f6c 7574 696f 6e2e 0a20 2020   resolution..   
+00000a50: 203a 7265 7475 726e 3a20 4d65 7368 6772   :return: Meshgr
+00000a60: 6964 206f 6620 656c 6576 6174 696f 6e20  id of elevation 
+00000a70: 616e 6420 617a 696d 7574 6820 666f 7220  and azimuth for 
+00000a80: 616c 6c20 7669 7369 626c 6520 736b 792e  all visible sky.
+00000a90: 0a20 2020 2072 0100 0000 7233 0000 0054  .    r....r3...T
+00000aa0: 2901 da08 656e 6470 6f69 6e74 6968 0100  )...endpointih..
+00000ab0: 0029 0372 2000 0000 da08 6c69 6e73 7061  .).r .....linspa
+00000ac0: 6365 da08 6d65 7368 6772 6964 2905 723c  ce..meshgrid).r<
+00000ad0: 0000 0072 2800 0000 722a 0000 00da 0365  ...r(...r*.....e
+00000ae0: 6c73 da03 617a 7372 1a00 0000 721a 0000  ls..azsr....r...
+00000af0: 0072 1b00 0000 da09 656c 617a 5f6d 6573  .r......elaz_mes
+00000b00: 6852 0000 0073 0800 0000 1205 0e01 1001  hR...s..........
+00000b10: 0801 7244 0000 00da 056e 7369 6465 da08  ..rD.....nside..
+00000b20: 706f 7369 7469 6f6e da04 6862 6f74 da04  position..hbot..
+00000b30: 6874 6f70 da07 6e6c 6179 6572 73da 0a6f  htop..nlayers..o
+00000b40: 6273 5f70 6978 656c 73fa 0d53 6571 7565  bs_pixels..Seque
+00000b50: 6e63 655b 696e 745d da04 6461 7461 da05  nce[int]..data..
+00000b60: 6c61 7965 72fa 0a69 6e74 207c 204e 6f6e  layer..int | Non
+00000b70: 6563 0a00 0000 0000 0000 0000 0000 1000  ec..............
+00000b80: 0000 0700 0000 4300 0001 7322 0100 0074  ......C...s"...t
+00000b90: 007c 007c 0183 0201 0074 01a0 027c 047c  .|.|.....t...|.|
+00000ba0: 057c 06a1 037d 0a74 01a0 0374 04a0 057c  .|...}.t...t...|
+00000bb0: 02a1 01a1 0174 046a 0617 007d 0b7c 0964  .....t.j...}.|.d
+00000bc0: 0175 0072 5b74 01a0 0767 007c 006a 08a2  .u.r[t...g.|.j..
+00000bd0: 017c 0691 0152 00a1 017d 0c74 097c 0683  .|...R...}.t.|..
+00000be0: 0144 005d 2a7d 0d7c 0864 0164 0185 027c  .D.]*}.|.d.d...|
+00000bf0: 0d66 0219 007c 0b7c 073c 0074 0a7c 007c  .f...|.|.<.t.|.|
+00000c00: 017c 0a7c 0d19 007c 0383 045c 027d 0e7d  .|.|...|...\.}.}
+00000c10: 0f74 046a 0b6a 0c7c 0b7c 0f7c 0e64 0264  .t.j.j.|.|.|.d.d
+00000c20: 038d 047c 0c64 0164 0185 0264 0164 0185  ...|.d.d...d.d..
+00000c30: 027c 0d66 033c 0071 2a7c 0c6a 0d64 0464  .|.f.<.q*|.j.d.d
+00000c40: 058d 0153 0074 0e7c 0974 0f83 0272 877c  ...S.t.|.t...r.|
+00000c50: 097c 0664 0617 006b 0072 877c 0864 0164  .|.d...k.r.|.d.d
+00000c60: 0185 027c 0966 0219 007c 0b7c 073c 0074  ...|.f...|.|.<.t
+00000c70: 0a7c 007c 017c 0a7c 0919 007c 0383 045c  .|.|.|.|...|...\
+00000c80: 027d 0e7d 0f74 046a 0b6a 0c7c 0b7c 0f7c  .}.}.t.j.j.|.|.|
+00000c90: 0e64 0264 038d 047d 0c7c 0c53 0074 1064  .d.d...}.|.S.t.d
+00000ca0: 077c 0664 0618 009b 0064 089d 0383 0182  .|.d.....d......
+00000cb0: 0129 0961 b202 0000 0a20 2020 2043 616c  .).a.....    Cal
+00000cc0: 6375 6c61 7465 7320 696e 7465 7270 6f6c  culates interpol
+00000cd0: 6174 6564 2076 616c 7565 7320 6f6e 2068  ated values on h
+00000ce0: 6561 6c70 6978 2067 7269 642e 0a0a 2020  ealpix grid...  
+00000cf0: 2020 3a70 6172 616d 2065 6c3a 2045 6c65    :param el: Ele
+00000d00: 7661 7469 6f6e 2e0a 2020 2020 3a70 6172  vation..    :par
+00000d10: 616d 2061 7a3a 2041 7a69 6d75 7468 2e0a  am az: Azimuth..
+00000d20: 2020 2020 3a70 6172 616d 206e 7369 6465      :param nside
+00000d30: 3a20 5265 736f 6c75 7469 6f6e 206f 6620  : Resolution of 
+00000d40: 6865 616c 7069 7820 6772 6964 2e0a 2020  healpix grid..  
+00000d50: 2020 3a70 6172 616d 2070 6f73 6974 696f    :param positio
+00000d60: 6e3a 0a20 2020 203a 7061 7261 6d20 6862  n:.    :param hb
+00000d70: 6f74 3a20 4c6f 7765 7220 6c69 6d69 7420  ot: Lower limit 
+00000d80: 696e 205b 6b6d 5d20 6f66 2074 6865 206c  in [km] of the l
+00000d90: 6179 6572 2e0a 2020 2020 3a70 6172 616d  ayer..    :param
+00000da0: 2068 746f 703a 2055 7070 6572 206c 696d   htop: Upper lim
+00000db0: 6974 2069 6e20 5b6b 6d5d 206f 6620 7468  it in [km] of th
+00000dc0: 6520 6c61 7965 722e 0a20 2020 203a 7061  e layer..    :pa
+00000dd0: 7261 6d20 6e6c 6179 6572 733a 204e 756d  ram nlayers: Num
+00000de0: 6265 7220 6f66 2073 7562 2d6c 6179 6572  ber of sub-layer
+00000df0: 7320 7573 6564 2066 6f72 2069 6e74 6572  s used for inter
+00000e00: 6d65 6469 6174 6520 6361 6c63 756c 6174  mediate calculat
+00000e10: 696f 6e73 2e0a 2020 2020 3a70 6172 616d  ions..    :param
+00000e20: 206f 6273 5f70 6978 656c 733a 204c 6973   obs_pixels: Lis
+00000e30: 7420 6f66 2070 6978 656c 2069 6e64 6963  t of pixel indic
+00000e40: 6573 2069 6e73 6964 6520 7468 6520 7669  es inside the vi
+00000e50: 7369 626c 6520 6469 736b 206f 6e20 6865  sible disk on he
+00000e60: 616c 7069 7820 7370 6865 7265 2e0a 2020  alpix sphere..  
+00000e70: 2020 3a70 6172 616d 2064 6174 613a 2041    :param data: A
+00000e80: 2064 6174 6120 746f 2069 6e74 6572 706f   data to interpo
+00000e90: 6c61 7465 2e0a 2020 2020 3a70 6172 616d  late..    :param
+00000ea0: 206c 6179 6572 3a20 4e75 6d62 6572 206f   layer: Number o
+00000eb0: 6620 7375 626c 6179 6572 2066 726f 6d20  f sublayer from 
+00000ec0: 7468 6520 7072 6563 616c 6375 6c61 7465  the precalculate
+00000ed0: 6420 7375 626c 6179 6572 732e 0a20 2020  d sublayers..   
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000ef0: 6620 4e6f 6e65 202d 2061 6e20 6176 6572  f None - an aver
+00000f00: 6167 6520 6f76 6572 2061 6c6c 206c 6179  age over all lay
+00000f10: 6572 7320 6973 2072 6574 7572 6e65 642e  ers is returned.
+00000f20: 0a20 2020 203a 7265 7475 726e 3a20 496e  .    :return: In
+00000f30: 7465 7270 6f6c 6174 6564 2076 616c 7565  terpolated value
+00000f40: 7320 6174 2073 7065 6369 6669 6564 2065  s at specified e
+00000f50: 6c65 7661 7469 6f6e 2061 6e64 2061 7a69  levation and azi
+00000f60: 6d75 7468 2e0a 2020 2020 4e54 2901 da06  muth..    NT)...
+00000f70: 6c6f 6e6c 6174 e902 0000 0029 01da 0461  lonlat.....)...a
+00000f80: 7869 7372 0900 0000 7a34 5468 6520 6c61  xisr....z4The la
+00000f90: 7965 7220 7661 6c75 6520 6d75 7374 2062  yer value must b
+00000fa0: 6520 696e 7465 6765 7220 616e 6420 6265  e integer and be
+00000fb0: 2069 6e20 7261 6e67 6520 5b30 2c20 fa01   in range [0, ..
+00000fc0: 5d29 1172 2e00 0000 7220 0000 0072 4000  ]).r....r ...r@.
+00000fd0: 0000 da05 7a65 726f 73da 0268 70da 0a6e  ....zeros..hp..n
+00000fe0: 7369 6465 326e 7069 78da 0655 4e53 4545  side2npix..UNSEE
+00000ff0: 4eda 0565 6d70 7479 722c 0000 00da 0572  N..emptyr,.....r
+00001000: 616e 6765 723b 0000 00da 0970 6978 656c  anger;.....pixel
+00001010: 6675 6e63 da0e 6765 745f 696e 7465 7270  func..get_interp
+00001020: 5f76 616c da04 6d65 616e 7223 0000 0072  _val..meanr#...r
+00001030: 3d00 0000 722d 0000 0029 1072 2800 0000  =...r-...).r(...
+00001040: 722a 0000 0072 4500 0000 7246 0000 0072  r*...rE...rF...r
+00001050: 4700 0000 7248 0000 0072 4900 0000 724a  G...rH...rI...rJ
+00001060: 0000 0072 4c00 0000 724d 0000 00da 0768  ...rL...rM.....h
+00001070: 6569 6768 7473 da04 6d61 705f da03 7265  eights..map_..re
+00001080: 73da 0169 7238 0000 0072 3900 0000 721a  s..ir8...r9...r.
+00001090: 0000 0072 1a00 0000 721b 0000 00da 0a65  ...r....r......e
+000010a0: 7661 6c5f 6c61 7965 725d 0000 0073 2800  val_layer]...s(.
+000010b0: 0000 0a1c 0e01 1601 0801 1601 0c01 1401  ................
+000010c0: 1601 0601 0801 1aff 0c03 1601 1401 1601  ................
+000010d0: 1401 0401 0202 0e01 04ff 7260 0000 00e9  ..........r`....
+000010e0: 1400 0000 da07 6c69 6278 3236 34da 0569  ......libx264..i
+000010f0: 6d64 6972 da03 7374 72da 0673 6176 6574  mdir..str..savet
+00001100: 6fda 0366 7073 da04 6465 7363 fa0a 7374  o..fps..desc..st
+00001110: 7220 7c20 4e6f 6e65 da05 636f 6465 6363  r | None..codecc
+00001120: 0500 0000 0000 0000 0000 0000 0900 0000  ................
+00001130: 0900 0000 4300 0001 7398 0000 007c 01a0  ....C...s....|..
+00001140: 0064 01a1 0173 097c 0164 0137 007d 017c  .d...s.|.d.7.}.|
+00001150: 0370 0c64 027d 0364 0364 047c 029b 0064  .p.d.}.d.d.|...d
+00001160: 0574 016a 02a0 037c 0064 06a1 0264 077c  .t.j...|.d...d.|
+00001170: 0464 087c 0167 097d 0574 047c 0583 017d  .d.|.g.}.t.|...}
+00001180: 0674 0564 0964 0a7c 0364 0b64 0c8d 048f  .t.d.d.|.d.d....
+00001190: 187d 077c 06a0 06a1 0044 005d 0a7d 087c  .}.|.....D.].}.|
+000011a0: 07a0 077c 087c 076a 0818 00a1 0101 0071  ...|.|.j.......q
+000011b0: 2f57 0064 0d04 0004 0083 0301 0064 0d53  /W.d.........d.S
+000011c0: 0031 0073 4577 0101 0001 0001 0059 0001  .1.sEw.......Y..
+000011d0: 0064 0d53 0029 0e61 5501 0000 0a20 2020  .d.S.).aU....   
+000011e0: 2052 656e 6465 7273 2065 7869 7374 696e   Renders existin
+000011f0: 6720 7365 7420 6f66 2070 6963 7475 7265  g set of picture
+00001200: 7320 746f 206d 7034 2076 6964 656f 2e0a  s to mp4 video..
+00001210: 2020 2020 3a70 6172 616d 2069 6d64 6972      :param imdir
+00001220: 3a20 4c6f 6361 7469 6f6e 206f 6620 696d  : Location of im
+00001230: 6167 6573 2e0a 2020 2020 3a70 6172 616d  ages..    :param
+00001240: 2073 6176 6574 6f3a 2050 6174 6820 7769   saveto: Path wi
+00001250: 7468 206e 616d 6520 746f 2077 6865 7265  th name to where
+00001260: 2073 6176 6520 7468 6520 6669 6c65 2e0a   save the file..
+00001270: 2020 2020 3a70 6172 616d 2066 7073 3a20      :param fps: 
+00001280: 4672 616d 6572 6174 6520 2d20 6672 616d  Framerate - fram
+00001290: 6573 2070 6572 2073 6563 6f6e 642e 0a20  es per second.. 
+000012a0: 2020 203a 7061 7261 6d20 6465 7363 3a20     :param desc: 
+000012b0: 4465 7363 7269 7074 696f 6e20 6f66 2061  Description of a
+000012c0: 2070 726f 6772 6573 7362 6172 2e20 4966   progressbar. If
+000012d0: 204e 6f6e 6520 2d20 7468 6520 7072 6f67   None - the prog
+000012e0: 7265 7373 6261 7220 7769 6c6c 206e 6f74  ressbar will not
+000012f0: 2061 7070 6561 722e 0a20 2020 203a 7061   appear..    :pa
+00001300: 7261 6d20 636f 6465 633a 2043 6f64 6563  ram codec: Codec
+00001310: 2074 6f20 7573 6520 666f 7220 7669 6465   to use for vide
+00001320: 6f20 7265 6e64 6572 696e 672e 0a20 2020  o rendering..   
+00001330: 207a 042e 6d70 347a 0f52 656e 6465 7269   z..mp4z.Renderi
+00001340: 6e67 2076 6964 656f da06 6666 6d70 6567  ng video..ffmpeg
+00001350: 7a02 2d72 7a02 2d69 7a08 2530 3664 2e70  z.-rz.-iz.%06d.p
+00001360: 6e67 7a07 2d76 636f 6465 637a 022d 79e9  ngz.-vcodecz.-y.
+00001370: 6400 0000 7201 0000 0054 2904 da05 746f  d...r....T)...to
+00001380: 7461 6c72 4600 0000 7267 0000 00da 056c  talrF...rg.....l
+00001390: 6561 7665 4e29 09da 0865 6e64 7377 6974  eaveN)...endswit
+000013a0: 68da 026f 73da 0470 6174 68da 046a 6f69  h..os..path..joi
+000013b0: 6e72 0500 0000 7208 0000 00da 1972 756e  nr....r......run
+000013c0: 5f63 6f6d 6d61 6e64 5f77 6974 685f 7072  _command_with_pr
+000013d0: 6f67 7265 7373 da06 7570 6461 7465 da01  ogress..update..
+000013e0: 6e29 0972 6300 0000 7265 0000 0072 6600  n).rc...re...rf.
+000013f0: 0000 7267 0000 0072 6900 0000 da03 636d  ..rg...ri.....cm
+00001400: 64da 0266 66da 0470 6261 72da 0870 726f  d..ff..pbar..pro
+00001410: 6772 6573 7372 1a00 0000 721a 0000 0072  gressr....r....r
+00001420: 1b00 0000 da07 7069 6332 7669 6490 0000  ......pic2vid...
+00001430: 0073 2600 0000 0a0f 0801 0801 0202 0201  .s&.............
+00001440: 0401 0201 0c01 0201 0201 0201 0201 04f7  ................
+00001450: 080b 1201 0c01 1201 02ff 22ff 7279 0000  ..........".ry..
+00001460: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001470: 0000 0400 0000 4300 0001 f316 0000 007c  ......C........|
+00001480: 0064 0119 006a 007c 0064 0264 0085 0219  .d...j.|.d.d....
+00001490: 008e 0053 00a9 034e 7201 0000 0072 0900  ...S...Nr....r..
+000014a0: 0000 2901 da05 6174 7465 6ea9 01da 0461  ..)...atten....a
+000014b0: 7267 7372 1a00 0000 721a 0000 0072 1b00  rgsr....r....r..
+000014c0: 0000 da14 6765 745f 6174 7465 6e5f 6672  ....get_atten_fr
+000014d0: 6f6d 5f66 7261 6d65 b300 0000 f302 0000  om_frame........
+000014e0: 0016 0172 7f00 0000 6301 0000 0000 0000  ...r....c.......
+000014f0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001500: 0172 7a00 0000 727b 0000 0029 01da 0472  .rz...r{...)...r
+00001510: 6566 7272 7d00 0000 721a 0000 0072 1a00  efrr}...r....r..
+00001520: 0000 721b 0000 00da 1367 6574 5f72 6566  ..r......get_ref
+00001530: 725f 6672 6f6d 5f66 7261 6d65 b700 0000  r_from_frame....
+00001540: 7280 0000 0072 8200 0000 2904 721c 0000  r....r....).r...
+00001550: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00001560: 2904 7228 0000 0072 2900 0000 722a 0000  ).r(...r)...r*..
+00001570: 0072 2900 0000 290a 7228 0000 0072 2900  .r)...).r(...r).
+00001580: 0000 722a 0000 0072 2900 0000 722f 0000  ..r*...r)...r/..
+00001590: 0072 2b00 0000 7230 0000 0072 3100 0000  .r+...r0...r1...
+000015a0: 721e 0000 0072 3200 0000 2904 723c 0000  r....r2...).r<..
+000015b0: 0072 3d00 0000 721e 0000 0072 3e00 0000  .r=...r....r>...
+000015c0: 2901 4e29 1472 2800 0000 7229 0000 0072  ).N).r(...r)...r
+000015d0: 2a00 0000 7229 0000 0072 4500 0000 723d  *...r)...rE...r=
+000015e0: 0000 0072 4600 0000 7231 0000 0072 4700  ...rF...r1...rG.
+000015f0: 0000 722b 0000 0072 4800 0000 722b 0000  ..r+...rH...r+..
+00001600: 0072 4900 0000 723d 0000 0072 4a00 0000  .rI...r=...rJ...
+00001610: 724b 0000 0072 4c00 0000 7229 0000 0072  rK...rL...r)...r
+00001620: 4d00 0000 724e 0000 0029 0372 6100 0000  M...rN...).ra...
+00001630: 4e72 6200 0000 290a 7263 0000 0072 6400  Nrb...).rc...rd.
+00001640: 0000 7265 0000 0072 6400 0000 7266 0000  ..re...rd...rf..
+00001650: 0072 3d00 0000 7267 0000 0072 6800 0000  .r=...rg...rh...
+00001660: 7269 0000 0072 6400 0000 291d da0a 5f5f  ri...rd...)...__
+00001670: 6675 7475 7265 5f5f 7202 0000 0072 6f00  future__r....ro.
+00001680: 0000 da06 7479 7069 6e67 7203 0000 0072  ....typingr....r
+00001690: 0400 0000 da06 6865 616c 7079 7254 0000  ......healpyrT..
+000016a0: 00da 056e 756d 7079 7220 0000 00da 1566  ...numpyr .....f
+000016b0: 666d 7065 675f 7072 6f67 7265 7373 5f79  fmpeg_progress_y
+000016c0: 6965 6c64 7205 0000 00da 0770 796d 6170  ieldr......pymap
+000016d0: 3364 7206 0000 0072 0700 0000 7208 0000  3dr....r....r...
+000016e0: 00da 0969 6f6e 5f74 6f6f 6c73 720a 0000  ...ion_toolsr...
+000016f0: 0072 3600 0000 720b 0000 0072 2200 0000  .r6...r....r"...
+00001700: 7227 0000 0072 2e00 0000 723b 0000 0072  r'...r....r;...r
+00001710: 4400 0000 7260 0000 0072 7900 0000 727f  D...r`...ry...r.
+00001720: 0000 0072 8200 0000 721a 0000 0072 1a00  ...r....r....r..
+00001730: 0000 721a 0000 0072 1b00 0000 da08 3c6d  ..r....r......<m
+00001740: 6f64 756c 653e 0100 0000 7330 0000 000c  odule>....s0....
+00001750: 0008 0210 0108 0208 010c 0110 010c 010c  ................
+00001760: 0204 020e 030a 1008 090a 060a 0e0a 1402  ................
+00001770: 150c f602 3602 0102 010c fb08 230c 04    ....6.......#..
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 17:32:33 2023 UTC, .py size: 3870 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-00000000: 6f0d 0d0a 0000 0000 b1c7 2564 1e0f 0000  o.........%d....
+00000000: 6f0d 0d0a 0000 0000 10dc 3d64 dc09 0000  o.........=d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6503 6a04 6403 6404 8d01 0100 0905  Z.e.j.d.d.......
-00000050: 641b 641c 640c 640d 8405 5a05 641d 640f  d.d.d.d...Z.d.d.
-00000060: 6410 8404 5a06 641e 6412 6413 8404 5a07  d...Z.d.d.d...Z.
-00000070: 641f 6417 6418 8404 5a08 6420 6419 641a  d.d.d...Z.d d.d.
-00000080: 8404 5a09 6402 5300 2921 e900 0000 0029  ..Z.d.S.)!.....)
+00000050: 641d 641e 640c 640d 8405 5a05 641f 640f  d.d.d.d...Z.d.d.
+00000060: 6410 8404 5a06 6420 6412 6413 8404 5a07  d...Z.d d.d...Z.
+00000070: 6421 6417 6418 8404 5a08 6422 641b 641c  d!d.d...Z.d"d.d.
+00000080: 8404 5a09 6402 5300 2923 e900 0000 0029  ..Z.d.S.)#.....)
 00000090: 01da 0b61 6e6e 6f74 6174 696f 6e73 4eda  ...annotationsN.
 000000a0: 0669 676e 6f72 6529 01da 0769 6e76 616c  .ignore)...inval
 000000b0: 6964 e974 5261 00da 0574 6865 7461 fa12  id.tRa...theta..
 000000c0: 666c 6f61 7420 7c20 6e70 2e6e 6461 7272  float | np.ndarr
 000000d0: 6179 da03 616c 74da 0272 65da 0566 6c6f  ay..alt..re..flo
 000000e0: 6174 da06 7265 7475 726e 6303 0000 0000  at..returnc.....
 000000f0: 0000 0000 0000 0004 0000 0007 0000 0043  ...............C
@@ -118,56 +118,64 @@
 00000750: 2069 6e20 5b72 6164 5d2e 0a20 2020 203a   in [rad]..    :
 00000760: 7265 7475 726e 3a20 4f75 7463 6f6d 696e  return: Outcomin
 00000770: 6720 616e 676c 6520 696e 205b 7261 645d  g angle in [rad]
 00000780: 2e0a 2020 2020 2903 720e 0000 00da 0661  ..    ).r......a
 00000790: 7263 7369 6eda 0373 696e 2903 7222 0000  rcsin..sin).r"..
 000007a0: 0072 2300 0000 7224 0000 0072 1400 0000  .r#...r$...r....
 000007b0: 7214 0000 0072 1500 0000 da0a 7265 6672  r....r......refr
-000007c0: 5f61 6e67 6c65 3500 0000 7302 0000 0018  _angle5...s.....
-000007d0: 0d72 2700 0000 6301 0000 0000 0000 0000  .r'...c.........
-000007e0: 0000 0004 0000 0005 0000 0043 0000 0173  ...........C...s
-000007f0: 2800 0000 6401 7d01 6402 7d02 6403 7d03  (...d.}.d.}.d.}.
-00000800: 6404 7c01 7c02 7c00 1400 1700 7c03 7c00  d.|.|.|.....|.|.
-00000810: 6405 1300 1400 1700 1b00 5300 2906 6127  d.........S.).a'
-00000820: 0100 000a 2020 2020 4170 7072 6f78 696d  ....    Approxim
-00000830: 6174 696f 6e20 6f66 2074 6865 2072 6566  ation of the ref
-00000840: 7261 6374 696f 6e20 696e 2074 6865 2074  raction in the t
-00000850: 726f 706f 7370 6865 7265 2072 6563 6f6d  roposphere recom
-00000860: 6d65 6e64 6564 2062 7920 7468 6520 4954  mended by the IT
-00000870: 552d 523a 0a20 2020 2068 7474 7073 3a2f  U-R:.    https:/
-00000880: 2f77 7777 2e69 7475 2e69 6e74 2f64 6d73  /www.itu.int/dms
-00000890: 5f70 7562 7265 632f 6974 752d 722f 7265  _pubrec/itu-r/re
-000008a0: 632f 702f 522d 5245 432d 502e 3833 342d  c/p/R-REC-P.834-
-000008b0: 392d 3230 3137 3132 2d49 2121 5044 462d  9-201712-I!!PDF-
-000008c0: 452e 7064 660a 0a20 2020 203a 7061 7261  E.pdf..    :para
-000008d0: 6d20 7468 6574 613a 205a 656e 6974 6820  m theta: Zenith 
-000008e0: 616e 676c 6520 696e 2072 6164 6961 6e73  angle in radians
-000008f0: 2e0a 2020 2020 3a72 6574 7572 6e3a 2043  ..    :return: C
-00000900: 6861 6e67 6520 6f66 2074 6865 2061 6e67  hange of the ang
-00000910: 6c65 2074 6865 7461 2064 7565 2074 6f20  le theta due to 
-00000920: 7472 6f70 6f73 7068 6572 6963 2072 6566  tropospheric ref
-00000930: 7261 6374 696f 6e20 2869 6e20 7261 6469  raction (in radi
-00000940: 616e 7329 2e0a 2020 2020 673d 0ad7 a360  ans)..    g=...`
-00000950: 51d0 4067 0ad7 a370 8d9e d2c0 67ae 47e1  Q.@g...p....g.G.
-00000960: 7a54 14b5 4072 1800 0000 720c 0000 0072  zT..@r....r....r
-00000970: 1400 0000 2904 7206 0000 00da 0161 da01  ....).r......a..
-00000980: 62da 0163 7214 0000 0072 1400 0000 7215  b..cr....r....r.
-00000990: 0000 00da 0974 726f 705f 7265 6672 4500  .....trop_refrE.
-000009a0: 0000 7308 0000 0004 0804 0104 011c 0172  ..s............r
-000009b0: 2b00 0000 2901 7205 0000 0029 0872 0600  +...).r....).r..
-000009c0: 0000 7207 0000 0072 0800 0000 7207 0000  ..r....r....r...
-000009d0: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-000009e0: 7207 0000 0029 0472 1700 0000 7207 0000  r....).r....r...
-000009f0: 0072 0b00 0000 7207 0000 0029 0472 1700  .r....r....).r..
-00000a00: 0000 7207 0000 0072 1f00 0000 720a 0000  ..r....r....r...
-00000a10: 0029 0872 2200 0000 7207 0000 0072 2300  .).r"...r....r#.
-00000a20: 0000 7207 0000 0072 2400 0000 7207 0000  ..r....r$...r...
-00000a30: 0072 0b00 0000 7207 0000 0029 0472 0600  .r....r....).r..
-00000a40: 0000 7207 0000 0072 0b00 0000 7207 0000  ..r....r....r...
-00000a50: 0029 0ada 0a5f 5f66 7574 7572 655f 5f72  .)...__future__r
-00000a60: 0200 0000 da05 6e75 6d70 7972 0e00 0000  ......numpyr....
-00000a70: da06 7365 7465 7272 7216 0000 0072 1e00  ..seterrr....r..
-00000a80: 0000 7221 0000 0072 2700 0000 722b 0000  ..r!...r'...r+..
-00000a90: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
-00000aa0: 7215 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000ab0: 0000 0073 1200 0000 0c00 0802 0c02 0204  ...s............
-00000ac0: 0cff 0a11 0a10 0a0c 0e10                 ..........
+000007c0: 5f61 6e67 6c65 3400 0000 7302 0000 0018  _angle4...s.....
+000007d0: 0d72 2700 0000 da02 656c da01 6863 0200  .r'.....el..hc..
+000007e0: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+000007f0: 0000 4300 0001 734c 0000 0064 0164 027c  ..C...sL...d.d.|
+00000800: 0014 0017 0064 037c 0064 0413 0014 0017  .....d.|.d......
+00000810: 007d 0264 0564 067c 0014 0017 0064 077c  .}.d.d.|.....d.|
+00000820: 0064 0413 0014 0017 007d 0364 087c 027c  .d.......}.d.|.|
+00000830: 017c 0314 0017 007c 0164 0413 0064 0914  .|.....|.d...d..
+00000840: 0017 001b 0053 0029 0a61 5101 0000 0a20  .....S.).aQ.... 
+00000850: 2020 2041 7070 726f 7869 6d61 7469 6f6e     Approximation
+00000860: 206f 6620 7468 6520 7265 6672 6163 7469   of the refracti
+00000870: 6f6e 2069 6e20 7468 6520 7472 6f70 6f73  on in the tropos
+00000880: 7068 6572 6520 7265 636f 6d6d 656e 6465  phere recommende
+00000890: 6420 6279 2074 6865 2049 5455 2d52 3a0a  d by the ITU-R:.
+000008a0: 2020 2020 6874 7470 733a 2f2f 7777 772e      https://www.
+000008b0: 6974 752e 696e 742f 646d 735f 7075 6272  itu.int/dms_pubr
+000008c0: 6563 2f69 7475 2d72 2f72 6563 2f70 2f52  ec/itu-r/rec/p/R
+000008d0: 2d52 4543 2d50 2e38 3334 2d39 2d32 3031  -REC-P.834-9-201
+000008e0: 3731 322d 4921 2150 4446 2d45 2e70 6466  712-I!!PDF-E.pdf
+000008f0: 0a0a 2020 2020 3a70 6172 616d 2065 6c3a  ..    :param el:
+00000900: 2045 6c65 7661 7469 6f6e 2061 6e67 6c65   Elevation angle
+00000910: 2069 6e20 5b64 6567 5d2e 0a20 2020 203a   in [deg]..    :
+00000920: 7061 7261 6d20 683a 2048 6569 6768 7420  param h: Height 
+00000930: 6f66 2069 6e73 7472 756d 656e 7420 696e  of instrument in
+00000940: 205b 6b6d 5d2e 0a20 2020 203a 7265 7475   [km]..    :retu
+00000950: 726e 3a20 4368 616e 6765 206f 6620 7468  rn: Change of th
+00000960: 6520 616e 676c 6520 7468 6574 6120 6475  e angle theta du
+00000970: 6520 746f 2074 726f 706f 7370 6865 7269  e to tropospheri
+00000980: 6320 7265 6672 6163 7469 6f6e 2028 696e  c refraction (in
+00000990: 2072 6164 6961 6e73 292e 0a20 2020 2067   radians)..    g
+000009a0: a01a 2fdd 2406 f53f 6729 ed0d be30 99e4  ../.$..?g)...0..
+000009b0: 3f67 e292 e34e e960 9d3f 720c 0000 0067  ?g...N.`.?r....g
+000009c0: 1b2f dd24 0681 cd3f 67a6 b8aa ecbb 22b8  ./.$...?g.....".
+000009d0: 3f67 5166 834c 3272 863f 7218 0000 0067  ?gQf.L2r.?r....g
+000009e0: 9b03 0473 f4f8 b53f 7214 0000 0029 0472  ...s...?r....).r
+000009f0: 2800 0000 7229 0000 00da 0274 31da 0274  (...r).....t1..t
+00000a00: 3272 1400 0000 7214 0000 0072 1500 0000  2r....r....r....
+00000a10: da09 7472 6f70 5f72 6566 7244 0000 0073  ..trop_refrD...s
+00000a20: 0600 0000 1809 1801 1c01 722c 0000 0029  ..........r,...)
+00000a30: 0172 0500 0000 2908 7206 0000 0072 0700  .r....).r....r..
+00000a40: 0000 7208 0000 0072 0700 0000 7209 0000  ..r....r....r...
+00000a50: 0072 0a00 0000 720b 0000 0072 0700 0000  .r....r....r....
+00000a60: 2904 7217 0000 0072 0700 0000 720b 0000  ).r....r....r...
+00000a70: 0072 0700 0000 2904 7217 0000 0072 0700  .r....).r....r..
+00000a80: 0000 721f 0000 0072 0a00 0000 2908 7222  ..r....r....).r"
+00000a90: 0000 0072 0700 0000 7223 0000 0072 0700  ...r....r#...r..
+00000aa0: 0000 7224 0000 0072 0700 0000 720b 0000  ..r$...r....r...
+00000ab0: 0072 0700 0000 2906 7228 0000 0072 0700  .r....).r(...r..
+00000ac0: 0000 7229 0000 0072 0a00 0000 720b 0000  ..r)...r....r...
+00000ad0: 0072 0700 0000 290a da0a 5f5f 6675 7475  .r....)...__futu
+00000ae0: 7265 5f5f 7202 0000 00da 056e 756d 7079  re__r......numpy
+00000af0: 720e 0000 00da 0673 6574 6572 7272 1600  r......seterrr..
+00000b00: 0000 721e 0000 0072 2100 0000 7227 0000  ..r....r!...r'..
+00000b10: 0072 2c00 0000 7214 0000 0072 1400 0000  .r,...r....r....
+00000b20: 7214 0000 0072 1500 0000 da08 3c6d 6f64  r....r......<mod
+00000b30: 756c 653e 0100 0000 7312 0000 000c 0008  ule>....s.......
+00000b40: 020c 0202 040c ff0a 110a 100a 0b0e 10    ...............
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/ion_tools.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 17:26:42 2023 UTC, .py size: 3816 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,254 +1,253 @@
-00000000: 6f0d 0d0a 0000 0000 52c6 2564 e80e 0000  o.......R.%d....
+00000000: 6f0d 0d0a 0000 0000 96c6 3d64 da0e 0000  o.........=d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 6400  m.Z...d.d.l.Z.d.
-00000050: 6401 6c05 5a05 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6401 6c06 5a07 6400 6403 6c08 6d09 5a09  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6400 6404 6c0a 6d0a 5a0a 0100 6405  ..d.d.l.m.Z...d.
-00000080: 6406 8400 5a0b 6407 6408 8400 5a0c 6409  d...Z.d.d...Z.d.
-00000090: 640a 8400 5a0d 640b 640c 8400 5a0e 640d  d...Z.d.d...Z.d.
-000000a0: 640e 8400 5a0f 640f 6410 8400 5a10 6411  d...Z.d.d...Z.d.
-000000b0: 6412 8400 5a11 6413 6414 8400 5a12 6415  d...Z.d.d...Z.d.
-000000c0: 6416 8400 5a13 6417 6418 8400 5a14 6419  d...Z.d.d...Z.d.
-000000d0: 641a 8400 5a15 641b 641c 8400 5a16 6401  d...Z.d.d...Z.d.
-000000e0: 5300 291d e900 0000 004e 2902 da09 6370  S.)......N)...cp
-000000f0: 755f 636f 756e 74da 0450 6f6f 6c29 01da  u_count..Pool)..
-00000100: 0869 6e74 6572 7031 6429 01da 0474 7164  .interp1d)...tqd
-00000110: 6d63 0100 0000 0000 0000 0000 0000 0100  mc..............
-00000120: 0000 0200 0000 4300 0000 f30a 0000 0074  ......C........t
-00000130: 006a 017c 008e 0053 00a9 014e 2902 da07  .j.|...S...N)...
-00000140: 6972 6963 6f72 65da 0349 5249 a901 da04  iricore..IRI....
-00000150: 7061 7273 a900 720c 0000 00fa 3e2f 686f  pars..r.....>/ho
-00000160: 6d65 2f6c 6170 3164 656d 2f64 6576 2d70  me/lap1dem/dev-p
-00000170: 7974 686f 6e2f 6469 6f6e 7079 2f73 7263  ython/dionpy/src
-00000180: 2f64 696f 6e70 792f 6d6f 6475 6c65 732f  /dionpy/modules/
-00000190: 7061 7261 6c6c 656c 2e70 79da 0869 7269  parallel.py..iri
-000001a0: 5f73 7461 720c 0000 00f3 0200 0000 0a01  _star...........
-000001b0: 720e 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000001c0: 0000 0100 0000 0200 0000 4300 0000 7206  ..........C...r.
-000001d0: 0000 0072 0700 0000 2902 da06 6563 6861  ...r....)...echa
-000001e0: 696d da0f 6465 6e73 6974 795f 7072 6f66  im..density_prof
-000001f0: 696c 6572 0a00 0000 720c 0000 0072 0c00  iler....r....r..
-00000200: 0000 720d 0000 00da 0b65 6368 6169 6d5f  ..r......echaim_
-00000210: 7374 6172 1000 0000 720f 0000 0072 1200  star....r....r..
-00000220: 0000 6305 0000 0000 0000 0000 0000 0009  ..c.............
-00000230: 0000 0005 0000 0043 0000 0073 5200 0000  .......C...sR...
-00000240: 7c02 7c03 6b02 7206 7c00 5300 7400 a001  |.|.k.r.|.S.t...
-00000250: 6401 7c03 7c02 1800 a002 a100 6702 a101  d.|.|.......g...
-00000260: 7d05 7400 a001 7c00 7c01 6702 a101 7d06  }.t...|.|.g...}.
-00000270: 7403 7c05 7c06 6401 6402 8d03 7d07 7c04  t.|.|.d.d...}.|.
-00000280: 7c02 1800 a002 a100 7d08 7c07 7c08 8301  |.......}.|.|...
-00000290: 5300 2903 7a60 0a20 2020 204c 696e 6561  S.).z`.    Linea
-000002a0: 7220 696e 7465 7270 6f6c 6174 696f 6e20  r interpolation 
-000002b0: 6f66 2076 616c 7565 2873 2920 6265 7477  of value(s) betw
-000002c0: 6565 6e20 7477 6f20 6461 7461 2070 6f69  een two data poi
-000002d0: 6e74 732f 6172 7261 7973 2067 6976 656e  nts/arrays given
-000002e0: 2074 6865 6972 2064 6174 6574 696d 6573   their datetimes
-000002f0: 2e0a 2020 2020 7201 0000 0029 01da 0461  ..    r....)...a
-00000300: 7869 7329 04da 026e 70da 0761 7361 7272  xis)...np..asarr
-00000310: 6179 da0d 746f 7461 6c5f 7365 636f 6e64  ay..total_second
-00000320: 7372 0400 0000 2909 da05 6461 7461 31da  sr....)...data1.
-00000330: 0564 6174 6132 da03 6474 31da 0364 7432  .data2..dt1..dt2
-00000340: da02 6474 da01 78da 0179 da06 6c69 6e6d  ..dt..x..y..linm
-00000350: 6f64 da04 785f 696e 720c 0000 0072 0c00  od..x_inr....r..
-00000360: 0000 720d 0000 00da 0a69 6e74 6572 705f  ..r......interp_
-00000370: 7661 6c18 0000 0073 0e00 0000 0804 0401  val....s........
-00000380: 1602 0e01 0e01 0c01 0801 7220 0000 0063  ..........r ...c
-00000390: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000003a0: 0200 0000 4300 0000 7308 0000 0074 007c  ....C...s....t.|
-000003b0: 008e 0053 0072 0700 0000 a901 7220 0000  ...S.r......r ..
-000003c0: 0072 0a00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000003d0: 720d 0000 00da 0f69 6e74 6572 705f 7661  r......interp_va
-000003e0: 6c5f 7374 6172 2600 0000 7302 0000 0008  l_star&...s.....
-000003f0: 0172 2200 0000 6304 0000 0000 0000 0000  .r"...c.........
-00000400: 0000 0005 0000 0004 0000 004b 0000 0073  ...........K...s
-00000410: 1400 0000 7c00 7c01 7c02 7c03 6603 6900  ....|.|.|.|.f.i.
-00000420: 7c04 a401 8e01 5300 2901 7a68 0a20 2020  |.....S.).zh.   
-00000430: 204f 7574 7369 6465 2063 6c61 7373 2066   Outside class f
-00000440: 756e 6374 696f 6e20 746f 206d 616b 6520  unction to make 
-00000450: 6361 6c63 756c 6174 696f 6e20 6f66 2061  calculation of a
-00000460: 7474 656e 7561 7469 6f6e 2061 6e64 2072  ttenuation and r
-00000470: 6566 7261 6374 696f 6e20 706f 7373 6962  efraction possib
-00000480: 6c65 2069 6e20 7061 7261 6c6c 656c 2e0a  le in parallel..
-00000490: 2020 2020 720c 0000 0029 05da 0466 756e      r....)...fun
-000004a0: 63da 0265 6cda 0261 7ada 0466 7265 71da  c..el..az..freq.
-000004b0: 066b 7761 7267 7372 0c00 0000 720c 0000  .kwargsr....r...
-000004c0: 0072 0d00 0000 da0b 6361 6c63 5f72 6566  .r......calc_ref
-000004d0: 6174 742a 0000 0073 0200 0000 1404 7228  att*...s......r(
-000004e0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000004f0: 0100 0000 0500 0000 4300 0000 731a 0000  ........C...s...
-00000500: 0074 007c 0064 0064 0185 0219 0069 007c  .t.|.d.d.....i.|
-00000510: 0064 0119 00a4 018e 0153 0029 024e e9ff  .d.......S.).N..
-00000520: ffff ff29 0172 2800 0000 720a 0000 0072  ...).r(...r....r
-00000530: 0c00 0000 720c 0000 0072 0d00 0000 da10  ....r....r......
-00000540: 6361 6c63 5f72 6566 6174 745f 7374 6172  calc_refatt_star
-00000550: 3100 0000 7302 0000 001a 0172 2a00 0000  1...s......r*...
-00000560: 6305 0000 0000 0000 0000 0000 000b 0000  c...............
-00000570: 000c 0000 000b 0000 0073 b000 0000 7400  .........s....t.
-00000580: a001 7402 8300 7403 7c03 8301 6702 a101  ..t...t.|...g...
-00000590: 7d06 7c04 6401 7500 7210 6402 6e01 6403  }.|.d.u.r.d.n.d.
-000005a0: 7d07 8700 6601 6404 6405 8408 7404 7403  }...f.d.d...t.t.
-000005b0: 7c03 8301 8301 4400 8301 7d08 7405 7c06  |.....D...}.t.|.
-000005c0: 6406 8d01 8f27 7d09 7406 7407 7c09 a008  d....'}.t.t.|...
-000005d0: 7409 740a 740b a00c 7c00 a101 740b a00c  t.t.t...|...t...
-000005e0: 7c01 a101 740b a00c 7c02 a101 7c03 7c08  |...t...|...|.|.
-000005f0: 8305 a102 7403 7c03 8301 7c07 7c04 6407  ....t.|...|.|.d.
-00000600: 8d04 8301 7d0a 5700 6401 0400 0400 8303  ....}.W.d.......
-00000610: 0100 6e08 3100 734e 7701 0100 0100 0100  ..n.1.sNw.......
-00000620: 5900 0100 7400 a00d 7c0a a101 5300 2908  Y...t...|...S.).
-00000630: 7a44 0a20 2020 2049 6d70 6c65 6d65 6e74  zD.    Implement
-00000640: 7320 7061 7261 6c6c 656c 2063 616c 6375  s parallel calcu
-00000650: 6c61 7469 6f6e 206f 6620 7265 6672 6163  lation of refrac
-00000660: 7469 6f6e 2f61 7474 656e 7561 7469 6f6e  tion/attenuation
-00000670: 2e0a 2020 2020 4e54 4663 0100 0000 0000  ..    NTFc......
-00000680: 0000 0000 0000 0200 0000 0300 0000 1300  ................
-00000690: 0000 f310 0000 0067 007c 005d 047d 0188  .......g.|.].}..
-000006a0: 0091 0271 0253 0072 0c00 0000 720c 0000  ...q.S.r....r...
-000006b0: 00a9 02da 022e 30da 015f a901 7227 0000  ......0.._..r'..
-000006c0: 0072 0c00 0000 720d 0000 00da 0a3c 6c69  .r....r......<li
-000006d0: 7374 636f 6d70 3e3b 0000 00f3 0200 0000  stcomp>;........
-000006e0: 1000 7a23 6361 6c63 5f72 6566 6174 745f  ..z#calc_refatt_
-000006f0: 7061 722e 3c6c 6f63 616c 733e 2e3c 6c69  par.<locals>.<li
-00000700: 7374 636f 6d70 3ea9 01da 0970 726f 6365  stcomp>....proce
-00000710: 7373 6573 a903 da05 746f 7461 6cda 0764  sses....total..d
-00000720: 6973 6162 6c65 da04 6465 7363 290e 7214  isable..desc).r.
-00000730: 0000 00da 036d 696e 7202 0000 00da 036c  .....minr......l
-00000740: 656e da05 7261 6e67 6572 0300 0000 da04  en..ranger......
-00000750: 6c69 7374 7205 0000 00da 0469 6d61 7072  listr......imapr
-00000760: 2a00 0000 da03 7a69 70da 0969 7465 7274  *.....zip..itert
-00000770: 6f6f 6c73 da06 7265 7065 6174 da05 6172  ools..repeat..ar
-00000780: 7261 7929 0b72 2300 0000 7224 0000 0072  ray).r#...r$...r
-00000790: 2500 0000 da05 6672 6571 73da 0970 6261  %.....freqs..pba
-000007a0: 725f 6465 7363 7227 0000 00da 056e 7072  r_descr'.....npr
-000007b0: 6f63 7236 0000 00da 0a72 6570 5f6b 7761  ocr6.....rep_kwa
-000007c0: 7267 73da 0470 6f6f 6cda 0372 6573 720c  rgs..pool..resr.
-000007d0: 0000 0072 2f00 0000 720d 0000 00da 0f63  ...r/...r......c
-000007e0: 616c 635f 7265 6661 7474 5f70 6172 3500  alc_refatt_par5.
-000007f0: 0000 732e 0000 0014 0410 011a 010c 0102  ..s.............
-00000800: 0102 0104 0102 0102 0108 0108 0108 0102  ................
-00000810: 0102 0102 fb02 fe06 0a02 0102 0104 f306  ................
-00000820: ff1c ff0a 1272 4700 0000 6301 0000 0000  .....rG...c.....
-00000830: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000840: 0000 0072 0600 0000 7207 0000 0029 0272  ...r....r....).r
-00000850: 1000 0000 da0c 6465 6e73 6974 795f 7061  ......density_pa
-00000860: 7468 720a 0000 0072 0c00 0000 720c 0000  thr....r....r...
-00000870: 0072 0d00 0000 da18 6563 6861 696d 5f64  .r......echaim_d
-00000880: 656e 7369 7479 5f70 6174 685f 7374 6172  ensity_path_star
-00000890: 5100 0000 720f 0000 0072 4900 0000 6304  Q...r....rI...c.
-000008a0: 0000 0000 0000 0000 0000 000b 0000 000c  ................
-000008b0: 0000 0043 0000 0073 8200 0000 7400 8300  ...C...s....t...
-000008c0: 7d04 7c04 7d05 7401 a002 7c00 7c05 a102  }.|.}.t...|.|...
-000008d0: 7d06 7401 a002 7c01 7c05 a102 7d07 7401  }.t...|.|...}.t.
-000008e0: a002 7c02 7c05 a102 7d08 7403 7c04 6401  ..|.|...}.t.|.d.
-000008f0: 8d01 8f18 7d09 7404 7c09 a005 7406 7407  ....}.t.|...t.t.
-00000900: 7c06 7c07 7c08 7408 a009 7c03 a101 8304  |.|.|.t...|.....
-00000910: a102 8301 7d0a 5700 6400 0400 0400 8303  ....}.W.d.......
-00000920: 0100 6e08 3100 7337 7701 0100 0100 0100  ..n.1.s7w.......
-00000930: 5900 0100 7401 a00a 7c0a a101 5300 2902  Y...t...|...S.).
-00000940: 4e72 3200 0000 290b 7202 0000 0072 1400  Nr2...).r....r..
-00000950: 0000 da0b 6172 7261 795f 7370 6c69 7472  ....array_splitr
-00000960: 0300 0000 723b 0000 0072 3c00 0000 7249  ....r;...r<...rI
-00000970: 0000 0072 3d00 0000 723e 0000 0072 3f00  ...r=...r>...r?.
-00000980: 0000 da06 6873 7461 636b 290b da04 736c  ....hstack)...sl
-00000990: 6174 da04 736c 6f6e da07 6865 6967 6874  at..slon..height
-000009a0: 7372 1b00 0000 7243 0000 00da 086e 6261  sr....rC.....nba
-000009b0: 7463 6865 73da 0462 6c61 74da 0462 6c6f  tches..blat..blo
-000009c0: 6eda 0862 6865 6967 6874 7372 4500 0000  n..bheightsrE...
-000009d0: 7246 0000 0072 0c00 0000 720c 0000 0072  rF...r....r....r
-000009e0: 0d00 0000 da1c 7061 7261 6c6c 656c 5f65  ......parallel_e
-000009f0: 6368 6169 6d5f 6465 6e73 6974 795f 7061  chaim_density_pa
-00000a00: 7468 5500 0000 7318 0000 0006 0104 010c  thU...s.........
-00000a10: 010c 010c 010c 0106 0102 0112 0108 fe1c  ................
-00000a20: ff0a 0572 5300 0000 6304 0000 0000 0000  ...rS...c.......
-00000a30: 0000 0000 0008 0000 0004 0000 004f 0000  .............O..
-00000a40: 0073 4a00 0000 7c02 6401 1900 7c00 7c01  .sJ...|.d...|.|.
-00000a50: 6702 7c04 a201 5200 6900 7c05 a401 8e01  g.|...R.i.|.....
-00000a60: 7d06 7c02 6402 1900 7c00 7c01 6702 7c04  }.|.d...|.|.g.|.
-00000a70: a201 5200 6900 7c05 a401 8e01 7d07 7400  ..R.i.|.....}.t.
-00000a80: 7c06 7c07 6702 7c03 a201 5200 8e00 5300  |.|.g.|...R...S.
-00000a90: 2903 7a56 0a20 2020 2046 6972 7374 2063  ).zV.    First c
-00000aa0: 616c 6375 6c61 7465 2064 6174 6120 6672  alculate data fr
-00000ab0: 6f6d 2070 726f 7669 6465 6420 6675 6e63  om provided func
-00000ac0: 7469 6f6e 732c 2074 6865 6e20 7065 7266  tions, then perf
-00000ad0: 6f72 6d20 616e 2069 6e74 6572 706f 6c61  orm an interpola
-00000ae0: 7469 6f6e 2e0a 2020 2020 7201 0000 00e9  tion..    r.....
-00000af0: 0100 0000 7221 0000 0029 0872 2400 0000  ....r!...).r$...
-00000b00: 7225 0000 00da 0566 756e 6373 da03 6474  r%.....funcs..dt
-00000b10: 73da 0461 7267 7372 2700 0000 7217 0000  s..argsr'...r...
-00000b20: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000b30: 720d 0000 00da 0f63 616c 635f 696e 7465  r......calc_inte
-00000b40: 7270 5f76 616c 6300 0000 7306 0000 001c  rp_valc...s.....
-00000b50: 041c 0112 0172 5800 0000 6301 0000 0000  .....rX...c.....
-00000b60: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000b70: 0000 0073 2800 0000 7400 6700 7c00 6400  ...s(...t.g.|.d.
-00000b80: 6401 8502 1900 a201 7c00 6401 1900 a201  d.......|.d.....
-00000b90: 5200 6900 7c00 6402 1900 a401 8e01 5300  R.i.|.d.......S.
-00000ba0: 2903 4ee9 feff ffff 7229 0000 0029 0172  ).N.....r)...).r
-00000bb0: 5800 0000 720a 0000 0072 0c00 0000 720c  X...r....r....r.
-00000bc0: 0000 0072 0d00 0000 da14 6361 6c63 5f69  ...r......calc_i
-00000bd0: 6e74 6572 705f 7661 6c5f 7374 6172 6c00  nterp_val_starl.
-00000be0: 0000 7302 0000 0028 0172 5a00 0000 6305  ..s....(.rZ...c.
-00000bf0: 0000 0000 0000 0000 0000 000d 0000 000d  ................
-00000c00: 0000 000f 0000 0073 c600 0000 7400 a001  .......s....t...
-00000c10: 7402 8300 7403 7c02 8301 6702 a101 7d07  t...t.|...g...}.
-00000c20: 7c04 6401 7500 7210 6402 6e01 6403 7d08  |.d.u.r.d.n.d.}.
-00000c30: 8700 6601 6404 6405 8408 7404 7403 7c03  ..f.d.d...t.t.|.
-00000c40: 8301 8301 4400 8301 7d09 8701 6601 6406  ....D...}...f.d.
-00000c50: 6405 8408 7404 7403 7c03 8301 8301 4400  d...t.t.|.....D.
-00000c60: 8301 7d0a 7405 7c07 6407 8d01 8f25 7d0b  ..}.t.|.d....%}.
-00000c70: 7406 7407 7c0b a008 7409 740a 740b a00c  t.t.|...t.t.t...
-00000c80: 7c00 a101 740b a00c 7c01 a101 7c02 7c03  |...t...|...|.|.
-00000c90: 7c09 7c0a 8306 a102 7403 7c03 8301 7c08  |.|.....t.|...|.
-00000ca0: 7c04 6408 8d04 8301 7d0c 5700 6401 0400  |.d.....}.W.d...
-00000cb0: 0400 8303 0100 6e08 3100 7359 7701 0100  ......n.1.sYw...
-00000cc0: 0100 0100 5900 0100 7400 a00d 7c0c a101  ....Y...t...|...
-00000cd0: 5300 2909 7a57 0a20 2020 2049 6d70 6c65  S.).zW.    Imple
-00000ce0: 6d65 6e74 7320 7061 7261 6c6c 656c 2063  ments parallel c
-00000cf0: 616c 6375 6c61 7469 6f6e 2061 6e64 2069  alculation and i
-00000d00: 6e74 6572 706f 6c61 7469 6f6e 206f 6620  nterpolation of 
-00000d10: 6461 7461 2061 7420 6769 7665 6e20 6461  data at given da
-00000d20: 7465 7469 6d65 732e 0a20 2020 204e 5446  tetimes..    NTF
-00000d30: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000d40: 0003 0000 0013 0000 0072 2b00 0000 720c  .........r+...r.
-00000d50: 0000 0072 0c00 0000 722c 0000 0029 0172  ...r....r,...).r
-00000d60: 5700 0000 720c 0000 0072 0d00 0000 7230  W...r....r....r0
-00000d70: 0000 0076 0000 0072 3100 0000 7a27 6361  ...v...r1...z'ca
-00000d80: 6c63 5f69 6e74 6572 705f 7661 6c5f 7061  lc_interp_val_pa
-00000d90: 722e 3c6c 6f63 616c 733e 2e3c 6c69 7374  r.<locals>.<list
-00000da0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00000db0: 0000 0200 0000 0300 0000 1300 0000 722b  ..............r+
-00000dc0: 0000 0072 0c00 0000 720c 0000 0072 2c00  ...r....r....r,.
-00000dd0: 0000 722f 0000 0072 0c00 0000 720d 0000  ..r/...r....r...
-00000de0: 0072 3000 0000 7700 0000 7231 0000 0072  .r0...w...r1...r
-00000df0: 3200 0000 7234 0000 0029 0e72 1400 0000  2...r4...).r....
-00000e00: 7238 0000 0072 0200 0000 7239 0000 0072  r8...r....r9...r
-00000e10: 3a00 0000 7203 0000 0072 3b00 0000 7205  :...r....r;...r.
-00000e20: 0000 0072 3c00 0000 725a 0000 0072 3d00  ...r<...rZ...r=.
-00000e30: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
-00000e40: 0029 0d72 2400 0000 7225 0000 0072 5500  .).r$...r%...rU.
-00000e50: 0000 7256 0000 0072 4200 0000 7257 0000  ..rV...rB...rW..
-00000e60: 0072 2700 0000 7243 0000 0072 3600 0000  .r'...rC...r6...
-00000e70: da08 7265 705f 6172 6773 7244 0000 0072  ..rep_argsrD...r
-00000e80: 4500 0000 7246 0000 0072 0c00 0000 2902  E...rF...r....).
-00000e90: 7257 0000 0072 2700 0000 720d 0000 00da  rW...r'...r.....
-00000ea0: 1363 616c 635f 696e 7465 7270 5f76 616c  .calc_interp_val
-00000eb0: 5f70 6172 7000 0000 7332 0000 0014 0410  _parp...s2......
-00000ec0: 011a 011a 010c 0102 0102 0104 0102 0102  ................
-00000ed0: 0108 0108 0102 0102 0102 0102 0102 fa02  ................
-00000ee0: fe06 0b02 0102 0104 f206 ff1c ff0a 1372  ...............r
-00000ef0: 5c00 0000 2917 723e 0000 00da 0f6d 756c  \...).r>.....mul
-00000f00: 7469 7072 6f63 6573 7369 6e67 7202 0000  tiprocessingr...
-00000f10: 0072 0300 0000 7210 0000 0072 0800 0000  .r....r....r....
-00000f20: da05 6e75 6d70 7972 1400 0000 da11 7363  ..numpyr......sc
-00000f30: 6970 792e 696e 7465 7270 6f6c 6174 6572  ipy.interpolater
-00000f40: 0400 0000 7205 0000 0072 0e00 0000 7212  ....r....r....r.
-00000f50: 0000 0072 2000 0000 7222 0000 0072 2800  ...r ...r"...r(.
-00000f60: 0000 722a 0000 0072 4700 0000 7249 0000  ..r*...rG...rI..
-00000f70: 0072 5300 0000 7258 0000 0072 5a00 0000  .rS...rX...rZ...
-00000f80: 725c 0000 0072 0c00 0000 720c 0000 0072  r\...r....r....r
-00000f90: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
-00000fa0: 6c65 3e01 0000 0073 2800 0000 0800 1001  le>....s(.......
-00000fb0: 0802 0801 0801 0801 0c01 0c01 0803 0804  ................
-00000fc0: 0808 080e 0804 0807 0804 081c 0804 080e  ................
-00000fd0: 0809 0c04                                ....
+00000050: 6401 6c05 5a05 6400 6401 6c06 5a07 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6405 6406 8400 5a0b 6407  m.Z...d.d...Z.d.
+00000080: 6408 8400 5a0c 6409 640a 8400 5a0d 640b  d...Z.d.d...Z.d.
+00000090: 640c 8400 5a0e 640d 640e 8400 5a0f 640f  d...Z.d.d...Z.d.
+000000a0: 6410 8400 5a10 6411 6412 8400 5a11 6413  d...Z.d.d...Z.d.
+000000b0: 6414 8400 5a12 6415 6416 8400 5a13 6417  d...Z.d.d...Z.d.
+000000c0: 6418 8400 5a14 6419 641a 8400 5a15 641b  d...Z.d.d...Z.d.
+000000d0: 641c 8400 5a16 6401 5300 291d e900 0000  d...Z.d.S.).....
+000000e0: 004e 2902 da09 6370 755f 636f 756e 74da  .N)...cpu_count.
+000000f0: 0450 6f6f 6c29 01da 0869 6e74 6572 7031  .Pool)...interp1
+00000100: 6429 01da 0474 7164 6d63 0100 0000 0000  d)...tqdmc......
+00000110: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00000120: 0000 f30a 0000 0074 006a 017c 008e 0053  .......t.j.|...S
+00000130: 00a9 014e 2902 da07 6972 6963 6f72 65da  ...N)...iricore.
+00000140: 0349 5249 a901 da04 7061 7273 a900 720c  .IRI....pars..r.
+00000150: 0000 00fa 3e2f 686f 6d65 2f6c 6170 3164  ....>/home/lap1d
+00000160: 656d 2f64 6576 2d70 7974 686f 6e2f 6469  em/dev-python/di
+00000170: 6f6e 7079 2f73 7263 2f64 696f 6e70 792f  onpy/src/dionpy/
+00000180: 6d6f 6475 6c65 732f 7061 7261 6c6c 656c  modules/parallel
+00000190: 2e70 79da 0869 7269 5f73 7461 720b 0000  .py..iri_star...
+000001a0: 00f3 0200 0000 0a01 720e 0000 0063 0100  ........r....c..
+000001b0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000001c0: 0000 4300 0000 7206 0000 0072 0700 0000  ..C...r....r....
+000001d0: 2902 da06 6563 6861 696d da0f 6465 6e73  )...echaim..dens
+000001e0: 6974 795f 7072 6f66 696c 6572 0a00 0000  ity_profiler....
+000001f0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000200: 0b65 6368 6169 6d5f 7374 6172 0f00 0000  .echaim_star....
+00000210: 720f 0000 0072 1200 0000 6305 0000 0000  r....r....c.....
+00000220: 0000 0000 0000 0009 0000 0005 0000 0043  ...............C
+00000230: 0000 0073 5200 0000 7c02 7c03 6b02 7206  ...sR...|.|.k.r.
+00000240: 7c00 5300 7400 a001 6401 7c03 7c02 1800  |.S.t...d.|.|...
+00000250: a002 a100 6702 a101 7d05 7400 a001 7c00  ....g...}.t...|.
+00000260: 7c01 6702 a101 7d06 7403 7c05 7c06 6401  |.g...}.t.|.|.d.
+00000270: 6402 8d03 7d07 7c04 7c02 1800 a002 a100  d...}.|.|.......
+00000280: 7d08 7c07 7c08 8301 5300 2903 7a60 0a20  }.|.|...S.).z`. 
+00000290: 2020 204c 696e 6561 7220 696e 7465 7270     Linear interp
+000002a0: 6f6c 6174 696f 6e20 6f66 2076 616c 7565  olation of value
+000002b0: 2873 2920 6265 7477 6565 6e20 7477 6f20  (s) between two 
+000002c0: 6461 7461 2070 6f69 6e74 732f 6172 7261  data points/arra
+000002d0: 7973 2067 6976 656e 2074 6865 6972 2064  ys given their d
+000002e0: 6174 6574 696d 6573 2e0a 2020 2020 7201  atetimes..    r.
+000002f0: 0000 0029 01da 0461 7869 7329 04da 026e  ...)...axis)...n
+00000300: 70da 0761 7361 7272 6179 da0d 746f 7461  p..asarray..tota
+00000310: 6c5f 7365 636f 6e64 7372 0400 0000 2909  l_secondsr....).
+00000320: da05 6461 7461 31da 0564 6174 6132 da03  ..data1..data2..
+00000330: 6474 31da 0364 7432 da02 6474 da01 78da  dt1..dt2..dt..x.
+00000340: 0179 da06 6c69 6e6d 6f64 da04 785f 696e  .y..linmod..x_in
+00000350: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000360: 0a69 6e74 6572 705f 7661 6c17 0000 0073  .interp_val....s
+00000370: 0e00 0000 0804 0401 1602 0e01 0e01 0c01  ................
+00000380: 0801 7220 0000 0063 0100 0000 0000 0000  ..r ...c........
+00000390: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+000003a0: 7308 0000 0074 007c 008e 0053 0072 0700  s....t.|...S.r..
+000003b0: 0000 a901 7220 0000 0072 0a00 0000 720c  ....r ...r....r.
+000003c0: 0000 0072 0c00 0000 720d 0000 00da 0f69  ...r....r......i
+000003d0: 6e74 6572 705f 7661 6c5f 7374 6172 2500  nterp_val_star%.
+000003e0: 0000 7302 0000 0008 0172 2200 0000 6304  ..s......r"...c.
+000003f0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00000400: 0000 004b 0000 0073 1400 0000 7c00 7c01  ...K...s....|.|.
+00000410: 7c02 7c03 6603 6900 7c04 a401 8e01 5300  |.|.f.i.|.....S.
+00000420: 2901 7a68 0a20 2020 204f 7574 7369 6465  ).zh.    Outside
+00000430: 2063 6c61 7373 2066 756e 6374 696f 6e20   class function 
+00000440: 746f 206d 616b 6520 6361 6c63 756c 6174  to make calculat
+00000450: 696f 6e20 6f66 2061 7474 656e 7561 7469  ion of attenuati
+00000460: 6f6e 2061 6e64 2072 6566 7261 6374 696f  on and refractio
+00000470: 6e20 706f 7373 6962 6c65 2069 6e20 7061  n possible in pa
+00000480: 7261 6c6c 656c 2e0a 2020 2020 720c 0000  rallel..    r...
+00000490: 0029 05da 0466 756e 63da 0265 6cda 0261  .)...func..el..a
+000004a0: 7ada 0466 7265 71da 066b 7761 7267 7372  z..freq..kwargsr
+000004b0: 0c00 0000 720c 0000 0072 0d00 0000 da0b  ....r....r......
+000004c0: 6361 6c63 5f72 6566 6174 7429 0000 0073  calc_refatt)...s
+000004d0: 0200 0000 1404 7228 0000 0063 0100 0000  ......r(...c....
+000004e0: 0000 0000 0000 0000 0100 0000 0500 0000  ................
+000004f0: 4300 0000 731a 0000 0074 007c 0064 0064  C...s....t.|.d.d
+00000500: 0185 0219 0069 007c 0064 0119 00a4 018e  .....i.|.d......
+00000510: 0153 0029 024e e9ff ffff ff29 0172 2800  .S.).N.....).r(.
+00000520: 0000 720a 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000530: 0072 0d00 0000 da10 6361 6c63 5f72 6566  .r......calc_ref
+00000540: 6174 745f 7374 6172 3000 0000 7302 0000  att_star0...s...
+00000550: 001a 0172 2a00 0000 6305 0000 0000 0000  ...r*...c.......
+00000560: 0000 0000 000b 0000 000c 0000 000b 0000  ................
+00000570: 0073 b000 0000 7400 a001 7402 8300 7403  .s....t...t...t.
+00000580: 7c03 8301 6702 a101 7d06 7c04 6401 7500  |...g...}.|.d.u.
+00000590: 7210 6402 6e01 6403 7d07 8700 6601 6404  r.d.n.d.}...f.d.
+000005a0: 6405 8408 7404 7403 7c03 8301 8301 4400  d...t.t.|.....D.
+000005b0: 8301 7d08 7405 7c06 6406 8d01 8f27 7d09  ..}.t.|.d....'}.
+000005c0: 7406 7407 7c09 a008 7409 740a 740b a00c  t.t.|...t.t.t...
+000005d0: 7c00 a101 740b a00c 7c01 a101 740b a00c  |...t...|...t...
+000005e0: 7c02 a101 7c03 7c08 8305 a102 7403 7c03  |...|.|.....t.|.
+000005f0: 8301 7c07 7c04 6407 8d04 8301 7d0a 5700  ..|.|.d.....}.W.
+00000600: 6401 0400 0400 8303 0100 6e08 3100 734e  d.........n.1.sN
+00000610: 7701 0100 0100 0100 5900 0100 7400 a00d  w.......Y...t...
+00000620: 7c0a a101 5300 2908 7a44 0a20 2020 2049  |...S.).zD.    I
+00000630: 6d70 6c65 6d65 6e74 7320 7061 7261 6c6c  mplements parall
+00000640: 656c 2063 616c 6375 6c61 7469 6f6e 206f  el calculation o
+00000650: 6620 7265 6672 6163 7469 6f6e 2f61 7474  f refraction/att
+00000660: 656e 7561 7469 6f6e 2e0a 2020 2020 4e54  enuation..    NT
+00000670: 4663 0100 0000 0000 0000 0000 0000 0200  Fc..............
+00000680: 0000 0300 0000 1300 0000 f310 0000 0067  ...............g
+00000690: 007c 005d 047d 0188 0091 0271 0253 0072  .|.].}.....q.S.r
+000006a0: 0c00 0000 720c 0000 00a9 02da 022e 30da  ....r.........0.
+000006b0: 015f a901 7227 0000 0072 0c00 0000 720d  ._..r'...r....r.
+000006c0: 0000 00da 0a3c 6c69 7374 636f 6d70 3e3a  .....<listcomp>:
+000006d0: 0000 00f3 0200 0000 1000 7a23 6361 6c63  ..........z#calc
+000006e0: 5f72 6566 6174 745f 7061 722e 3c6c 6f63  _refatt_par.<loc
+000006f0: 616c 733e 2e3c 6c69 7374 636f 6d70 3ea9  als>.<listcomp>.
+00000700: 01da 0970 726f 6365 7373 6573 a903 da05  ...processes....
+00000710: 746f 7461 6cda 0764 6973 6162 6c65 da04  total..disable..
+00000720: 6465 7363 290e 7214 0000 00da 036d 696e  desc).r......min
+00000730: 7202 0000 00da 036c 656e da05 7261 6e67  r......len..rang
+00000740: 6572 0300 0000 da04 6c69 7374 7205 0000  er......listr...
+00000750: 00da 0469 6d61 7072 2a00 0000 da03 7a69  ...imapr*.....zi
+00000760: 70da 0969 7465 7274 6f6f 6c73 da06 7265  p..itertools..re
+00000770: 7065 6174 da05 6172 7261 7929 0b72 2300  peat..array).r#.
+00000780: 0000 7224 0000 0072 2500 0000 da05 6672  ..r$...r%.....fr
+00000790: 6571 73da 0970 6261 725f 6465 7363 7227  eqs..pbar_descr'
+000007a0: 0000 00da 056e 7072 6f63 7236 0000 00da  .....nprocr6....
+000007b0: 0a72 6570 5f6b 7761 7267 73da 0470 6f6f  .rep_kwargs..poo
+000007c0: 6cda 0372 6573 720c 0000 0072 2f00 0000  l..resr....r/...
+000007d0: 720d 0000 00da 0f63 616c 635f 7265 6661  r......calc_refa
+000007e0: 7474 5f70 6172 3400 0000 732e 0000 0014  tt_par4...s.....
+000007f0: 0410 011a 010c 0102 0102 0104 0102 0102  ................
+00000800: 0108 0108 0108 0102 0102 0102 fb02 fe06  ................
+00000810: 0a02 0102 0104 f306 ff1c ff0a 1272 4700  .............rG.
+00000820: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000830: 0000 0002 0000 0043 0000 0072 0600 0000  .......C...r....
+00000840: 7207 0000 0029 0272 1000 0000 da0c 6465  r....).r......de
+00000850: 6e73 6974 795f 7061 7468 720a 0000 0072  nsity_pathr....r
+00000860: 0c00 0000 720c 0000 0072 0d00 0000 da18  ....r....r......
+00000870: 6563 6861 696d 5f64 656e 7369 7479 5f70  echaim_density_p
+00000880: 6174 685f 7374 6172 5000 0000 720f 0000  ath_starP...r...
+00000890: 0072 4900 0000 6304 0000 0000 0000 0000  .rI...c.........
+000008a0: 0000 000b 0000 000c 0000 0043 0000 0073  ...........C...s
+000008b0: 8200 0000 7400 8300 7d04 7c04 7d05 7401  ....t...}.|.}.t.
+000008c0: a002 7c00 7c05 a102 7d06 7401 a002 7c01  ..|.|...}.t...|.
+000008d0: 7c05 a102 7d07 7401 a002 7c02 7c05 a102  |...}.t...|.|...
+000008e0: 7d08 7403 7c04 6401 8d01 8f18 7d09 7404  }.t.|.d.....}.t.
+000008f0: 7c09 a005 7406 7407 7c06 7c07 7c08 7408  |...t.t.|.|.|.t.
+00000900: a009 7c03 a101 8304 a102 8301 7d0a 5700  ..|.........}.W.
+00000910: 6400 0400 0400 8303 0100 6e08 3100 7337  d.........n.1.s7
+00000920: 7701 0100 0100 0100 5900 0100 7401 a00a  w.......Y...t...
+00000930: 7c0a a101 5300 2902 4e72 3200 0000 290b  |...S.).Nr2...).
+00000940: 7202 0000 0072 1400 0000 da0b 6172 7261  r....r......arra
+00000950: 795f 7370 6c69 7472 0300 0000 723b 0000  y_splitr....r;..
+00000960: 0072 3c00 0000 7249 0000 0072 3d00 0000  .r<...rI...r=...
+00000970: 723e 0000 0072 3f00 0000 da06 6873 7461  r>...r?.....hsta
+00000980: 636b 290b da04 736c 6174 da04 736c 6f6e  ck)...slat..slon
+00000990: da07 6865 6967 6874 7372 1b00 0000 7243  ..heightsr....rC
+000009a0: 0000 00da 086e 6261 7463 6865 73da 0462  .....nbatches..b
+000009b0: 6c61 74da 0462 6c6f 6eda 0862 6865 6967  lat..blon..bheig
+000009c0: 6874 7372 4500 0000 7246 0000 0072 0c00  htsrE...rF...r..
+000009d0: 0000 720c 0000 0072 0d00 0000 da1c 7061  ..r....r......pa
+000009e0: 7261 6c6c 656c 5f65 6368 6169 6d5f 6465  rallel_echaim_de
+000009f0: 6e73 6974 795f 7061 7468 5400 0000 7318  nsity_pathT...s.
+00000a00: 0000 0006 0104 010c 010c 010c 010c 0106  ................
+00000a10: 0102 0112 0108 fe1c ff0a 0572 5300 0000  ...........rS...
+00000a20: 6304 0000 0000 0000 0000 0000 0008 0000  c...............
+00000a30: 0004 0000 004f 0000 0073 4a00 0000 7c02  .....O...sJ...|.
+00000a40: 6401 1900 7c00 7c01 6702 7c04 a201 5200  d...|.|.g.|...R.
+00000a50: 6900 7c05 a401 8e01 7d06 7c02 6402 1900  i.|.....}.|.d...
+00000a60: 7c00 7c01 6702 7c04 a201 5200 6900 7c05  |.|.g.|...R.i.|.
+00000a70: a401 8e01 7d07 7400 7c06 7c07 6702 7c03  ....}.t.|.|.g.|.
+00000a80: a201 5200 8e00 5300 2903 7a56 0a20 2020  ..R...S.).zV.   
+00000a90: 2046 6972 7374 2063 616c 6375 6c61 7465   First calculate
+00000aa0: 2064 6174 6120 6672 6f6d 2070 726f 7669   data from provi
+00000ab0: 6465 6420 6675 6e63 7469 6f6e 732c 2074  ded functions, t
+00000ac0: 6865 6e20 7065 7266 6f72 6d20 616e 2069  hen perform an i
+00000ad0: 6e74 6572 706f 6c61 7469 6f6e 2e0a 2020  nterpolation..  
+00000ae0: 2020 7201 0000 00e9 0100 0000 7221 0000    r.........r!..
+00000af0: 0029 0872 2400 0000 7225 0000 00da 0566  .).r$...r%.....f
+00000b00: 756e 6373 da03 6474 73da 0461 7267 7372  uncs..dts..argsr
+00000b10: 2700 0000 7217 0000 0072 1800 0000 720c  '...r....r....r.
+00000b20: 0000 0072 0c00 0000 720d 0000 00da 0f63  ...r....r......c
+00000b30: 616c 635f 696e 7465 7270 5f76 616c 6200  alc_interp_valb.
+00000b40: 0000 7306 0000 001c 041c 0112 0172 5800  ..s..........rX.
+00000b50: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000b60: 0000 0005 0000 0043 0000 0073 2800 0000  .......C...s(...
+00000b70: 7400 6700 7c00 6400 6401 8502 1900 a201  t.g.|.d.d.......
+00000b80: 7c00 6401 1900 a201 5200 6900 7c00 6402  |.d.....R.i.|.d.
+00000b90: 1900 a401 8e01 5300 2903 4ee9 feff ffff  ......S.).N.....
+00000ba0: 7229 0000 0029 0172 5800 0000 720a 0000  r)...).rX...r...
+00000bb0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000bc0: da14 6361 6c63 5f69 6e74 6572 705f 7661  ..calc_interp_va
+00000bd0: 6c5f 7374 6172 6b00 0000 7302 0000 0028  l_stark...s....(
+00000be0: 0172 5a00 0000 6305 0000 0000 0000 0000  .rZ...c.........
+00000bf0: 0000 000d 0000 000d 0000 000f 0000 0073  ...............s
+00000c00: c600 0000 7400 a001 7402 8300 7403 7c02  ....t...t...t.|.
+00000c10: 8301 6702 a101 7d07 7c04 6401 7500 7210  ..g...}.|.d.u.r.
+00000c20: 6402 6e01 6403 7d08 8700 6601 6404 6405  d.n.d.}...f.d.d.
+00000c30: 8408 7404 7403 7c03 8301 8301 4400 8301  ..t.t.|.....D...
+00000c40: 7d09 8701 6601 6406 6405 8408 7404 7403  }...f.d.d...t.t.
+00000c50: 7c03 8301 8301 4400 8301 7d0a 7405 7c07  |.....D...}.t.|.
+00000c60: 6407 8d01 8f25 7d0b 7406 7407 7c0b a008  d....%}.t.t.|...
+00000c70: 7409 740a 740b a00c 7c00 a101 740b a00c  t.t.t...|...t...
+00000c80: 7c01 a101 7c02 7c03 7c09 7c0a 8306 a102  |...|.|.|.|.....
+00000c90: 7403 7c03 8301 7c08 7c04 6408 8d04 8301  t.|...|.|.d.....
+00000ca0: 7d0c 5700 6401 0400 0400 8303 0100 6e08  }.W.d.........n.
+00000cb0: 3100 7359 7701 0100 0100 0100 5900 0100  1.sYw.......Y...
+00000cc0: 7400 a00d 7c0c a101 5300 2909 7a57 0a20  t...|...S.).zW. 
+00000cd0: 2020 2049 6d70 6c65 6d65 6e74 7320 7061     Implements pa
+00000ce0: 7261 6c6c 656c 2063 616c 6375 6c61 7469  rallel calculati
+00000cf0: 6f6e 2061 6e64 2069 6e74 6572 706f 6c61  on and interpola
+00000d00: 7469 6f6e 206f 6620 6461 7461 2061 7420  tion of data at 
+00000d10: 6769 7665 6e20 6461 7465 7469 6d65 732e  given datetimes.
+00000d20: 0a20 2020 204e 5446 6301 0000 0000 0000  .    NTFc.......
+00000d30: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+00000d40: 0072 2b00 0000 720c 0000 0072 0c00 0000  .r+...r....r....
+00000d50: 722c 0000 0029 0172 5700 0000 720c 0000  r,...).rW...r...
+00000d60: 0072 0d00 0000 7230 0000 0075 0000 0072  .r....r0...u...r
+00000d70: 3100 0000 7a27 6361 6c63 5f69 6e74 6572  1...z'calc_inter
+00000d80: 705f 7661 6c5f 7061 722e 3c6c 6f63 616c  p_val_par.<local
+00000d90: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00000da0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00000db0: 0000 1300 0000 722b 0000 0072 0c00 0000  ......r+...r....
+00000dc0: 720c 0000 0072 2c00 0000 722f 0000 0072  r....r,...r/...r
+00000dd0: 0c00 0000 720d 0000 0072 3000 0000 7600  ....r....r0...v.
+00000de0: 0000 7231 0000 0072 3200 0000 7234 0000  ..r1...r2...r4..
+00000df0: 0029 0e72 1400 0000 7238 0000 0072 0200  .).r....r8...r..
+00000e00: 0000 7239 0000 0072 3a00 0000 7203 0000  ..r9...r:...r...
+00000e10: 0072 3b00 0000 7205 0000 0072 3c00 0000  .r;...r....r<...
+00000e20: 725a 0000 0072 3d00 0000 723e 0000 0072  rZ...r=...r>...r
+00000e30: 3f00 0000 7240 0000 0029 0d72 2400 0000  ?...r@...).r$...
+00000e40: 7225 0000 0072 5500 0000 7256 0000 0072  r%...rU...rV...r
+00000e50: 4200 0000 7257 0000 0072 2700 0000 7243  B...rW...r'...rC
+00000e60: 0000 0072 3600 0000 da08 7265 705f 6172  ...r6.....rep_ar
+00000e70: 6773 7244 0000 0072 4500 0000 7246 0000  gsrD...rE...rF..
+00000e80: 0072 0c00 0000 2902 7257 0000 0072 2700  .r....).rW...r'.
+00000e90: 0000 720d 0000 00da 1363 616c 635f 696e  ..r......calc_in
+00000ea0: 7465 7270 5f76 616c 5f70 6172 6f00 0000  terp_val_paro...
+00000eb0: 7332 0000 0014 0410 011a 011a 010c 0102  s2..............
+00000ec0: 0102 0104 0102 0102 0108 0108 0102 0102  ................
+00000ed0: 0102 0102 0102 fa02 fe06 0b02 0102 0104  ................
+00000ee0: f206 ff1c ff0a 1372 5c00 0000 2917 723e  .......r\...).r>
+00000ef0: 0000 00da 0f6d 756c 7469 7072 6f63 6573  .....multiproces
+00000f00: 7369 6e67 7202 0000 0072 0300 0000 7208  singr....r....r.
+00000f10: 0000 0072 1000 0000 da05 6e75 6d70 7972  ...r......numpyr
+00000f20: 1400 0000 da11 7363 6970 792e 696e 7465  ......scipy.inte
+00000f30: 7270 6f6c 6174 6572 0400 0000 7205 0000  rpolater....r...
+00000f40: 0072 0e00 0000 7212 0000 0072 2000 0000  .r....r....r ...
+00000f50: 7222 0000 0072 2800 0000 722a 0000 0072  r"...r(...r*...r
+00000f60: 4700 0000 7249 0000 0072 5300 0000 7258  G...rI...rS...rX
+00000f70: 0000 0072 5a00 0000 725c 0000 0072 0c00  ...rZ...r\...r..
+00000f80: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000f90: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000fa0: 2600 0000 0800 1001 0802 0801 0801 0c01  &...............
+00000fb0: 0c01 0803 0804 0808 080e 0804 0807 0804  ................
+00000fc0: 081c 0804 080e 0809 0c04                 ..........
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/parallel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/__pycache__/plotting.cpython-310.pyc` & `dionpy-0.99.7/src/dionpy/modules/__pycache__/plotting.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 17:41:52 2023 UTC, .py size: 4539 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,279 +1,247 @@
-00000000: 6f0d 0d0a 0000 0000 e0c9 2564 bb11 0000  o.........%d....
+00000000: 550d 0d0a 0000 0000 ece6 3d63 7710 0000  U.........=cw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000f 0000 0040 0000 0173 b200 0000 6400  .....@...s....d.
+00000020: 0011 0000 0040 0000 0173 aa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d03 5a03 6d04 5a04  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6402 6c07 5a08 6400 6405 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6400 6406 6c09 6d0b 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6407 6c0d 6d0e 5a0e 0100 6408 6409 640a  d.l.m.Z...d.d.d.
-00000090: 640b 640c 640d 640e 640f 6410 6411 6412  d.d.d.d.d.d.d.d.
-000000a0: 6413 6414 6415 6416 9c0e 5a0f 0902 0902  d.d.d.d...Z.....
-000000b0: 0902 0902 0902 0902 0902 0902 0917 0918  ................
-000000c0: 0902 0919 091a 0902 6437 6438 6433 6434  ........d7d8d3d4
-000000d0: 8405 5a10 6435 6436 8400 5a11 6402 5300  ..Z.d5d6..Z.d.S.
-000000e0: 2939 e900 0000 0029 01da 0b61 6e6e 6f74  )9.....)...annot
-000000f0: 6174 696f 6e73 4e29 02da 0864 6174 6574  ationsN)...datet
-00000100: 696d 65da 0974 696d 6564 656c 7461 2901  ime..timedelta).
-00000110: da08 5365 7175 656e 6365 2901 da09 636f  ..Sequence)...co
-00000120: 6c6f 726d 6170 7329 01da 0670 7970 6c6f  lormaps)...pyplo
-00000130: 7429 01da 0d46 756e 6346 6f72 6d61 7474  t)...FuncFormatt
-00000140: 6572 7a62 4461 7465 7469 6d65 206f 626a  erzbDatetime obj
-00000150: 6563 7420 7265 7072 6573 656e 7469 6e67  ect representing
-00000160: 2061 2074 696d 6520 6f66 2061 6e20 6f62   a time of an ob
-00000170: 7365 7276 6174 696f 6e2e 2049 6620 4e6f  servation. If No
-00000180: 6e65 202d 2077 696c 6c20 6e6f 7420 6265  ne - will not be
-00000190: 2073 7065 6369 6669 6564 2075 6e64 6572   specified under
-000001a0: 2070 6c6f 742e 7aa2 4c69 7374 2063 6f6e   plot.z.List con
-000001b0: 7461 696e 696e 6720 6765 6f67 7261 7068  taining geograph
-000001c0: 6963 616c 206c 6174 6974 7564 6520 5b64  ical latitude [d
-000001d0: 6567 5d2c 206c 6f6e 6769 7475 6465 5b64  eg], longitude[d
-000001e0: 6567 5d20 616e 6420 616c 7469 7475 6465  eg] and altitude
-000001f0: 5b6d 5d20 7265 7072 6573 656e 7469 6e67  [m] representing
-00000200: 2061 2070 6f73 6974 696f 6e20 6f66 2020   a position of  
-00000210: 616e 2069 6e73 7472 756d 656e 742e 2049  an instrument. I
-00000220: 6620 4e6f 6e65 202d 2077 696c 6c20 6e6f  f None - will no
-00000230: 7420 6265 2073 7065 6369 6669 6564 2075  t be specified u
-00000240: 6e64 6572 2070 6c6f 742e 7a5d 466c 6f61  nder plot.z]Floa
-00000250: 7420 7265 7072 6573 656e 7469 6e67 2061  t representing a
-00000260: 2066 7265 7175 656e 6379 206f 6620 616e   frequency of an
-00000270: 206f 6273 6572 7661 7469 6f6e 2e20 4966   observation. If
-00000280: 204e 6f6e 6520 2d20 7769 6c6c 206e 6f74   None - will not
-00000290: 2062 6520 7370 6563 6966 6965 6420 756e   be specified un
-000002a0: 6465 7220 706c 6f74 2e7a 1154 6974 6c65  der plot.z.Title
-000002b0: 206f 6620 7468 6520 706c 6f74 7a3c 4c61   of the plotz<La
-000002c0: 6265 6c20 6e65 6172 2063 6f6c 6f72 6261  bel near colorba
-000002d0: 722e 204d 6f73 7420 6675 6e63 7469 6f6e  r. Most function
-000002e0: 7320 6f76 6572 7269 6465 2074 6869 7320  s override this 
-000002f0: 7061 7261 6d65 7465 722e 7a57 4c61 6265  parameter.zWLabe
-00000300: 6c20 756e 6465 7220 706c 6f74 2e20 5573  l under plot. Us
-00000310: 7561 6c6c 7920 696e 636c 7564 6573 2064  ually includes d
-00000320: 6174 652f 7469 6d65 2c20 6c6f 6361 7469  ate/time, locati
-00000330: 6f6e 2061 6e64 2066 7265 7175 656e 6379  on and frequency
-00000340: 206f 6620 616e 206f 6273 6572 7661 7469   of an observati
-00000350: 6f6e 2e7a 8154 7570 6c65 2063 6f6e 7461  on.z.Tuple conta
-00000360: 696e 696e 6720 6d69 6e20 616e 6420 6d61  ining min and ma
-00000370: 7820 7661 6c75 6573 206f 6620 7468 6520  x values of the 
-00000380: 636f 6c6f 7262 6172 2073 6361 6c65 2e20  colorbar scale. 
-00000390: 4966 2061 6e79 206f 6620 6c69 6d69 7473  If any of limits
-000003a0: 2069 7320 4e6f 6e65 202d 206d 6178 2f6d   is None - max/m
-000003b0: 696e 2076 616c 7565 7320 6973 2061 7574  in values is aut
-000003c0: 6f6d 6174 6963 616c 6c79 2063 616c 6375  omatically calcu
-000003d0: 6c61 7465 642e 7a58 5061 7468 2074 6f20  lated.zXPath to 
-000003e0: 7361 7665 2074 6865 2070 6c6f 742e 204d  save the plot. M
-000003f0: 7573 7420 696e 636c 7564 6520 6e61 6d65  ust include name
-00000400: 2e20 4966 206e 6f74 2073 7065 6369 6669  . If not specifi
-00000410: 6564 202d 2074 6865 2070 6c6f 7420 7769  ed - the plot wi
-00000420: 6c6c 206e 6f74 2062 6520 7361 7665 642e  ll not be saved.
-00000430: 7a11 496d 6167 6520 7265 736f 6c75 7469  z.Image resoluti
-00000440: 6f6e 2e7a 1e41 2063 6f6c 6f72 6d61 7020  on.z.A colormap 
-00000450: 746f 2075 7365 2069 6e20 7468 6520 706c  to use in the pl
-00000460: 6f74 2e7a 2b46 6f72 6d61 7474 6572 206f  ot.z+Formatter o
-00000470: 6620 6e75 6d62 6572 7320 6f6e 2074 6865  f numbers on the
-00000480: 2063 6f6c 6f72 6261 7220 7363 616c 652e   colorbar scale.
-00000490: 7a23 4120 636f 6c6f 7220 746f 2066 696c  z#A color to fil
-000004a0: 6c20 6e70 2e6e 616e 2069 6e20 7468 6520  l np.nan in the 
-000004b0: 706c 6f74 2e7a 2341 2063 6f6c 6f72 2074  plot.z#A color t
-000004c0: 6f20 6669 6c6c 206e 702e 696e 6620 696e  o fill np.inf in
-000004d0: 2074 6865 2070 6c6f 742e 7a58 4469 6666   the plot.zXDiff
-000004e0: 6572 656e 6365 2062 6574 7765 656e 206c  erence between l
-000004f0: 6f63 616c 2074 696d 6520 616e 6420 5554  ocal time and UT
-00000500: 432e 2049 6620 7370 6563 6966 6965 6420  C. If specified 
-00000510: 2d20 6c6f 6361 6c20 7469 6d65 2069 7320  - local time is 
-00000520: 7368 6f77 6e20 696e 7374 6561 6420 6f66  shown instead of
-00000530: 2055 5443 290e da02 6474 da03 706f 73da   UTC)...dt..pos.
-00000540: 0466 7265 71da 0574 6974 6c65 da08 6261  .freq..title..ba
-00000550: 726c 6162 656c da09 706c 6f74 6c61 6265  rlabel..plotlabe
-00000560: 6cda 0563 626c 696d da06 7361 7665 746f  l..cblim..saveto
-00000570: da03 6470 69da 0463 6d61 70da 0863 6266  ..dpi..cmap..cbf
-00000580: 6f72 6d61 74da 086e 616e 636f 6c6f 72da  ormat..nancolor.
-00000590: 0869 6e66 636f 6c6f 72da 0a6c 6f63 616c  .infcolor..local
-000005a0: 5f74 696d 65e9 2c01 0000 da07 7669 7269  _time.,.....viri
-000005b0: 6469 73da 0562 6c61 636b da05 7768 6974  dis..black..whit
-000005c0: 65da 0464 6174 61fa 2c53 6571 7565 6e63  e..data.,Sequenc
-000005d0: 655b 6e70 2e6e 6461 7272 6179 2c20 6e70  e[np.ndarray, np
-000005e0: 2e6e 6461 7272 6179 2c20 6e70 2e6e 6461  .ndarray, np.nda
-000005f0: 7272 6179 5d72 0900 0000 fa0f 6461 7465  rray]r......date
-00000600: 7469 6d65 207c 204e 6f6e 6572 0a00 0000  time | Noner....
-00000610: fa24 5365 7175 656e 6365 5b66 6c6f 6174  .$Sequence[float
-00000620: 2c20 666c 6f61 742c 2066 6c6f 6174 5d20  , float, float] 
-00000630: 7c20 4e6f 6e65 720b 0000 00fa 0c66 6c6f  | Noner......flo
-00000640: 6174 207c 204e 6f6e 6572 0c00 0000 fa0a  at | Noner......
-00000650: 7374 7220 7c20 4e6f 6e65 720d 0000 0072  str | Noner....r
-00000660: 0e00 0000 720f 0000 00fa 1653 6571 7565  ....r......Seque
-00000670: 6e63 655b 666c 6f61 742c 2066 6c6f 6174  nce[float, float
-00000680: 5d72 1000 0000 7211 0000 00da 0369 6e74  ]r....r......int
-00000690: 7212 0000 00da 0373 7472 7213 0000 0072  r......strr....r
-000006a0: 1400 0000 7215 0000 0072 1600 0000 fa0a  ....r....r......
-000006b0: 696e 7420 7c20 4e6f 6e65 630f 0000 0000  int | Nonec.....
-000006c0: 0000 0000 0000 0017 0000 0009 0000 0043  ...............C
-000006d0: 0000 0173 ac02 0000 7c06 6401 7500 7253  ...s....|.d.u.rS
-000006e0: 6402 7d06 7c02 6401 7501 721b 7c06 6403  d.}.|.d.u.r.|.d.
-000006f0: 7c02 6404 1900 6405 9b04 6406 7c02 6407  |.d...d...d.|.d.
-00000700: 1900 6405 9b04 6408 9d05 3700 7d06 7c01  ..d...d...7.}.|.
-00000710: 6401 7501 7246 7c0e 6401 7500 7230 7c06  d.u.rF|.d.u.r0|.
-00000720: 6409 7400 a001 7c01 640a a102 1700 6408  d.t...|.d.....d.
-00000730: 1700 3700 7d06 6e16 7402 7c0e 7403 8302  ..7.}.n.t.|.t...
-00000740: 7246 7c06 640b 7400 a001 7c01 7404 7c0e  rF|.d.t...|.t.|.
-00000750: 640c 8d01 1700 640a a102 1700 640d 1700  d.....d.....d...
-00000760: 3700 7d06 7c03 6401 7501 7253 7c06 640e  7.}.|.d.u.rS|.d.
-00000770: 7c03 640f 9b04 6410 9d03 3700 7d06 7c07  |.d...d...7.}.|.
-00000780: 7058 6401 6401 6702 7d07 7c07 6404 1900  pXd.d.g.}.|.d...
-00000790: 6401 7500 7270 7405 a006 7c00 6411 1900  d.u.rpt...|.d...
-000007a0: 7c00 6411 1900 7405 6a07 0b00 6b03 1900  |.d...t.j...k...
-000007b0: a101 7c07 6404 3c00 7c07 6407 1900 6401  ..|.d.<.|.d...d.
-000007c0: 7500 728a 7c07 6407 1900 7087 7405 a008  u.r.|.d...p.t...
-000007d0: 7c00 6411 1900 7c00 6411 1900 7405 6a07  |.d...|.d...t.j.
-000007e0: 6b03 1900 a101 7c07 6407 3c00 7405 a009  k.....|.d.<.t...
-000007f0: 7405 a00a 7c00 6411 1900 a101 7c07 6407  t...|.d.....|.d.
-00000800: 1900 6412 1700 7c00 6411 1900 a103 7d0f  ..d...|.d.....}.
-00000810: 7402 7c0a 740b 8302 72a5 740c 7c0a 1900  t.|.t...r.t.|...
-00000820: 7d0a 7c0a a00d 7c0c a101 0100 7c0a a00e  }.|...|.....|...
-00000830: 7c0d a101 0100 7405 6a0f 6a10 7c0f 7405  |.....t.j.j.|.t.
-00000840: a011 7c0f a101 6413 8d02 7d10 7412 6a13  ..|...d...}.t.j.
-00000850: 6414 6415 8d01 7d11 7c11 6a14 6416 6417  d.d...}.|.j.d.d.
-00000860: 6418 8d02 7d12 7c12 6a15 7c00 6404 1900  d...}.|.j.|.d...
-00000870: 7c00 6407 1900 7c10 7c0a 7c07 6404 1900  |.d...|.|.|.d...
-00000880: 7c07 6407 1900 6419 641a 8d07 7d13 7c12  |.d...d.d...}.|.
-00000890: 6a16 641b 641c 641d 8d02 0100 7c12 a017  j.d.d.d.....|...
-000008a0: 641e a101 0100 641f 6420 8400 7d14 7c12  d.....d.d ..}.|.
-000008b0: 6a18 a019 741a 7c14 8301 a101 0100 7c12  j...t.|.......|.
-000008c0: a01b 6421 a101 0100 7c12 6a1c 6422 6423  ..d!....|.j.d"d#
-000008d0: 6424 6425 8d03 0100 7c12 6a1c 6426 6423  d$d%....|.j.d&d#
-000008e0: 641b 6427 8d03 0100 7412 6a1d 7c13 6428  d.d'....t.j.|.d(
-000008f0: 6429 7c0b 642a 8d04 6a1e 7c05 642b 642c  d)|.d*..j.|.d+d,
-00000900: 8d02 0100 7412 6a1f 7c04 642d 642e 642f  ....t.j.|.d-d.d/
-00000910: 8d03 0100 7412 6a20 7c06 642b 6430 8d02  ....t.j |.d+d0..
-00000920: 0100 7c08 6401 7501 9001 7254 7421 6a22  ..|.d.u...rTt!j"
-00000930: a023 7c08 a101 5c02 7d15 7d16 7421 6a22  .#|...\.}.}.t!j"
-00000940: a024 7c15 a101 9001 7345 7425 7c15 8301  .$|.....sEt%|...
-00000950: 6404 6b04 9001 7245 7421 a026 7c15 a101  d.k...rEt!.&|...
-00000960: 0100 7412 6a27 7c08 7c09 6431 6432 8d03  ..t.j'|.|.d1d2..
-00000970: 0100 7412 a028 7c11 a101 0100 6401 5300  ..t..(|.....d.S.
-00000980: 7c11 5300 2933 7aa8 0a20 2020 2041 2063  |.S.)3z..    A c
-00000990: 6f72 6520 6675 6e63 7469 6f6e 2066 6f72  ore function for
-000009a0: 2067 7261 7068 6963 2067 656e 6572 6174   graphic generat
-000009b0: 696f 6e20 6f6e 2074 6865 2076 6973 6962  ion on the visib
-000009c0: 6c65 2073 6b79 2066 6965 6c64 2e0a 2020  le sky field..  
-000009d0: 2020 5365 6520 616c 6c20 6176 6169 6c61    See all availa
-000009e0: 626c 6520 6f70 7469 6f6e 206c 6973 7465  ble option liste
-000009f0: 6420 696e 2064 696f 6e70 792e 706c 6f74  d in dionpy.plot
-00000a00: 5f6b 7761 7267 732e 0a0a 2020 2020 3a72  _kwargs...    :r
-00000a10: 6574 7572 6e3a 2041 206d 6174 706c 6f74  eturn: A matplot
-00000a20: 6c69 6220 6669 6775 7265 2e0a 2020 2020  lib figure..    
-00000a30: 4eda 007a 0e50 6f73 6974 696f 6e3a 206c  N..z.Position: l
-00000a40: 6174 3d72 0100 0000 7a03 2e33 667a 062c  at=r....z..3fz.,
-00000a50: 206c 6f6e 3de9 0100 0000 da01 0a7a 0a55   lon=........z.U
-00000a60: 5443 2074 696d 653a 207a 0e25 592d 256d  TC time: z.%Y-%m
-00000a70: 2d25 6420 2548 3a25 4d7a 0c4c 6f63 616c  -%d %H:%Mz.Local
-00000a80: 2074 696d 653a 2029 01da 0568 6f75 7273   time: )...hours
-00000a90: 7a02 0a20 7a0b 4672 6571 7565 6e63 793a  z.. z.Frequency:
-00000aa0: 207a 032e 3166 7a04 204d 487a e902 0000   z..1fz. MHz....
-00000ab0: 0067 0000 0000 84d7 9741 2901 da04 6d61  .g.......A)...ma
-00000ac0: 736b 2902 e908 0000 0072 2b00 0000 2901  sk)......r+...).
-00000ad0: da07 6669 6773 697a 65e9 6f00 0000 da05  ..figsize.o.....
-00000ae0: 706f 6c61 7229 01da 0a70 726f 6a65 6374  polar)...project
-00000af0: 696f 6eda 0461 7574 6f29 0472 1200 0000  ion..auto).r....
-00000b00: da04 766d 696e da04 766d 6178 da07 7368  ..vmin..vmax..sh
-00000b10: 6164 696e 67da 0467 7261 79fa 013a 2902  ading..gray..:).
-00000b20: da05 636f 6c6f 72da 096c 696e 6573 7479  ..color..linesty
-00000b30: 6c65 da01 4e63 0200 0000 0000 0000 0000  le..Nc..........
-00000b40: 0000 0200 0000 0200 0000 5300 0001 730c  ..........S...s.
-00000b50: 0000 007c 0064 019b 0464 029d 0253 0029  ...|.d...d...S.)
-00000b60: 034e 7a03 2e30 66f5 0200 0000 c2b0 a900  .Nz..0f.........
-00000b70: 2902 da02 785f da01 5f72 3a00 0000 723a  )...x_.._r:...r:
-00000b80: 0000 00fa 3e2f 686f 6d65 2f6c 6170 3164  ....>/home/lap1d
-00000b90: 656d 2f64 6576 2d70 7974 686f 6e2f 6469  em/dev-python/di
-00000ba0: 6f6e 7079 2f73 7263 2f64 696f 6e70 792f  onpy/src/dionpy/
-00000bb0: 6d6f 6475 6c65 732f 706c 6f74 7469 6e67  modules/plotting
-00000bc0: 2e70 79da 083c 6c61 6d62 6461 3e66 0000  .py..<lambda>f..
-00000bd0: 0073 0200 0000 0c00 7a1c 706f 6c61 725f  .s......z.polar_
-00000be0: 706c 6f74 2e3c 6c6f 6361 6c73 3e2e 3c6c  plot.<locals>.<l
-00000bf0: 616d 6264 613e e9ff ffff ffda 0462 6f74  ambda>.......bot
-00000c00: 68da 056d 616a 6f72 e90b 0000 0029 03da  h..major.....)..
-00000c10: 0461 7869 73da 0577 6869 6368 da09 6c61  .axis..which..la
-00000c20: 6265 6c73 697a 65da 0179 2903 7243 0000  belsize..y).rC..
-00000c30: 0072 4400 0000 da0a 6c61 6265 6c63 6f6c  .rD.....labelcol
-00000c40: 6f72 671b 2fdd 2406 81a5 3f67 7b14 ae47  org./.$...?g{..G
-00000c50: e17a b43f 2903 da08 6672 6163 7469 6f6e  .z.?)...fraction
-00000c60: da03 7061 64da 0666 6f72 6d61 74e9 0a00  ..pad..format...
-00000c70: 0000 2902 da05 6c61 6265 6cda 0473 697a  ..)...label..siz
-00000c80: 65e9 0e00 0000 e914 0000 0029 02da 0866  e..........)...f
-00000c90: 6f6e 7473 697a 6572 4900 0000 2901 7250  ontsizerI...).rP
-00000ca0: 0000 00da 0574 6967 6874 2902 7211 0000  .....tight).r...
-00000cb0: 00da 0b62 626f 785f 696e 6368 6573 2929  ...bbox_inches))
-00000cc0: 7203 0000 00da 0873 7472 6674 696d 65da  r......strftime.
-00000cd0: 0a69 7369 6e73 7461 6e63 6572 2200 0000  .isinstancer"...
-00000ce0: 7204 0000 00da 026e 70da 066e 616e 6d69  r......np..nanmi
-00000cf0: 6eda 0369 6e66 da06 6e61 6e6d 6178 da05  n..inf..nanmax..
-00000d00: 7768 6572 65da 0569 7369 6e66 7223 0000  where..isinfr#..
-00000d10: 0072 0600 0000 da07 7365 745f 6261 64da  .r......set_bad.
-00000d20: 0873 6574 5f6f 7665 72da 026d 61da 0561  .set_over..ma..a
-00000d30: 7272 6179 da05 6973 6e61 6eda 0370 6c74  rray..isnan..plt
-00000d40: da06 6669 6775 7265 da0b 6164 645f 7375  ..figure..add_su
-00000d50: 6270 6c6f 74da 0a70 636f 6c6f 726d 6573  bplot..pcolormes
-00000d60: 68da 0467 7269 64da 1773 6574 5f74 6865  h..grid..set_the
-00000d70: 7461 5f7a 6572 6f5f 6c6f 6361 7469 6f6e  ta_zero_location
-00000d80: da05 7961 7869 73da 1373 6574 5f6d 616a  ..yaxis..set_maj
-00000d90: 6f72 5f66 6f72 6d61 7474 6572 7208 0000  or_formatterr...
-00000da0: 00da 1373 6574 5f74 6865 7461 5f64 6972  ...set_theta_dir
-00000db0: 6563 7469 6f6e da0b 7469 636b 5f70 6172  ection..tick_par
-00000dc0: 616d 73da 0863 6f6c 6f72 6261 72da 0973  ams..colorbar..s
-00000dd0: 6574 5f6c 6162 656c 720c 0000 00da 0678  et_labelr......x
-00000de0: 6c61 6265 6cda 026f 73da 0470 6174 68da  label..os..path.
-00000df0: 0573 706c 6974 da06 6578 6973 7473 da03  .split..exists..
-00000e00: 6c65 6eda 086d 616b 6564 6972 73da 0773  len..makedirs..s
-00000e10: 6176 6566 6967 da05 636c 6f73 6529 1772  avefig..close).r
-00000e20: 1b00 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-00000e30: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000e40: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000e50: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000e60: 7215 0000 0072 1600 0000 da09 706c 6f74  r....r......plot
-00000e70: 5f64 6174 61da 0b6d 6173 6b65 645f 6461  _data..masked_da
-00000e80: 7461 da03 6669 67da 0261 78da 0369 6d67  ta..fig..ax..img
-00000e90: da04 7266 6d74 da04 6865 6164 da04 7461  ..rfmt..head..ta
-00000ea0: 696c 723a 0000 0072 3a00 0000 723d 0000  ilr:...r:...r=..
-00000eb0: 00da 0a70 6f6c 6172 5f70 6c6f 7420 0000  ...polar_plot ..
-00000ec0: 0073 7e00 0000 0817 0401 0801 2201 0801  .s~........."...
-00000ed0: 0801 0201 1201 06ff 0a03 0201 0201 0401  ................
-00000ee0: 0e01 02ff 02ff 0204 02fc 04ff 0807 1201  ................
-00000ef0: 0c02 0c01 2201 0c01 2801 2402 0a01 0801  ...."...(.$.....
-00000f00: 0a01 0a01 1602 0c02 0e01 0401 0601 0601  ................
-00000f10: 0201 0201 0601 0601 0201 06f9 0e09 0a01  ................
-00000f20: 0801 1001 0a01 1002 1001 1201 0401 06ff  ................
-00000f30: 1003 0e01 0a01 1001 1c01 0a01 1001 0a01  ................
-00000f40: 0401 0401 727d 0000 0063 0100 0000 0000  ....r}...c......
-00000f50: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000f60: 0001 7308 0000 0074 007c 008e 0053 0029  ..s....t.|...S.)
-00000f70: 014e 2901 727d 0000 0029 01da 0470 6172  .N).r}...)...par
-00000f80: 7372 3a00 0000 723a 0000 0072 3d00 0000  sr:...r:...r=...
-00000f90: da0f 706f 6c61 725f 706c 6f74 5f73 7461  ..polar_plot_sta
-00000fa0: 727b 0000 0073 0200 0000 0801 727f 0000  r{...s......r...
-00000fb0: 0029 0e4e 4e4e 4e4e 4e4e 4e72 1700 0000  .).NNNNNNNNr....
-00000fc0: 7218 0000 004e 7219 0000 0072 1a00 0000  r....Nr....r....
-00000fd0: 4e29 1e72 1b00 0000 721c 0000 0072 0900  N).r....r....r..
-00000fe0: 0000 721d 0000 0072 0a00 0000 721e 0000  ..r....r....r...
-00000ff0: 0072 0b00 0000 721f 0000 0072 0c00 0000  .r....r....r....
-00001000: 7220 0000 0072 0d00 0000 7220 0000 0072  r ...r....r ...r
-00001010: 0e00 0000 7220 0000 0072 0f00 0000 7221  ....r ...r....r!
-00001020: 0000 0072 1000 0000 7220 0000 0072 1100  ...r....r ...r..
-00001030: 0000 7222 0000 0072 1200 0000 7223 0000  ..r"...r....r#..
-00001040: 0072 1300 0000 7223 0000 0072 1400 0000  .r....r#...r....
-00001050: 7223 0000 0072 1500 0000 7223 0000 0072  r#...r....r#...r
-00001060: 1600 0000 7224 0000 0029 12da 0a5f 5f66  ....r$...)...__f
-00001070: 7574 7572 655f 5f72 0200 0000 726d 0000  uture__r....rm..
-00001080: 0072 0300 0000 7204 0000 00da 0674 7970  .r....r......typ
-00001090: 696e 6772 0500 0000 da05 6e75 6d70 7972  ingr......numpyr
-000010a0: 5500 0000 da0a 6d61 7470 6c6f 746c 6962  U.....matplotlib
-000010b0: 7206 0000 0072 0700 0000 7260 0000 00da  r....r....r`....
-000010c0: 116d 6174 706c 6f74 6c69 622e 7469 636b  .matplotlib.tick
-000010d0: 6572 7208 0000 00da 0b70 6c6f 745f 6b77  err......plot_kw
-000010e0: 6172 6773 727d 0000 0072 7f00 0000 723a  argsr}...r....r:
-000010f0: 0000 0072 3a00 0000 723a 0000 0072 3d00  ...r:...r:...r=.
-00001100: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001110: 734e 0000 000c 0008 0210 010c 0108 020c  sN..............
-00001120: 010c 010c 0102 0302 0102 0202 0102 0102  ................
-00001130: 0102 0102 0202 0102 0102 0102 0102 0102  ................
-00001140: 0106 f002 1602 0102 0102 0102 0102 0102  ................
-00001150: 0102 0102 0102 0102 0102 0102 0102 010c  ................
-00001160: f10c 5b                                  ..[
+00000070: 0100 6400 6406 6c09 6d0b 5a0c 0100 6407  ..d.d.l.m.Z...d.
+00000080: 6408 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
+00000090: 6410 6411 6412 6413 6414 6415 9c0e 5a0d  d.d.d.d.d.d...Z.
+000000a0: 6428 641a 641b 641c 641d 641e 641e 641e  d(d.d.d.d.d.d.d.
+000000b0: 641f 641e 6420 6421 6421 6421 6421 6422  d.d.d d!d!d!d!d"
+000000c0: 6423 9c0f 6424 6425 8405 5a0e 6426 6427  d#..d$d%..Z.d&d'
+000000d0: 8400 5a0f 6402 5300 2929 e900 0000 0029  ..Z.d.S.)).....)
+000000e0: 01da 0b61 6e6e 6f74 6174 696f 6e73 4e29  ...annotationsN)
+000000f0: 02da 0864 6174 6574 696d 65da 0974 696d  ...datetime..tim
+00000100: 6564 656c 7461 2901 da05 5475 706c 6529  edelta)...Tuple)
+00000110: 01da 0963 6f6c 6f72 6d61 7073 2901 da06  ...colormaps)...
+00000120: 7079 706c 6f74 7a62 4461 7465 7469 6d65  pyplotzbDatetime
+00000130: 206f 626a 6563 7420 7265 7072 6573 656e   object represen
+00000140: 7469 6e67 2061 2074 696d 6520 6f66 2061  ting a time of a
+00000150: 6e20 6f62 7365 7276 6174 696f 6e2e 2049  n observation. I
+00000160: 6620 4e6f 6e65 202d 2077 696c 6c20 6e6f  f None - will no
+00000170: 7420 6265 2073 7065 6369 6669 6564 2075  t be specified u
+00000180: 6e64 6572 2070 6c6f 742e 7aa2 4c69 7374  nder plot.z.List
+00000190: 2063 6f6e 7461 696e 696e 6720 6765 6f67   containing geog
+000001a0: 7261 7068 6963 616c 206c 6174 6974 7564  raphical latitud
+000001b0: 6520 5b64 6567 5d2c 206c 6f6e 6769 7475  e [deg], longitu
+000001c0: 6465 5b64 6567 5d20 616e 6420 616c 7469  de[deg] and alti
+000001d0: 7475 6465 5b6d 5d20 7265 7072 6573 656e  tude[m] represen
+000001e0: 7469 6e67 2061 2070 6f73 6974 696f 6e20  ting a position 
+000001f0: 6f66 2020 616e 2069 6e73 7472 756d 656e  of  an instrumen
+00000200: 742e 2049 6620 4e6f 6e65 202d 2077 696c  t. If None - wil
+00000210: 6c20 6e6f 7420 6265 2073 7065 6369 6669  l not be specifi
+00000220: 6564 2075 6e64 6572 2070 6c6f 742e 7a5d  ed under plot.z]
+00000230: 466c 6f61 7420 7265 7072 6573 656e 7469  Float representi
+00000240: 6e67 2061 2066 7265 7175 656e 6379 206f  ng a frequency o
+00000250: 6620 616e 206f 6273 6572 7661 7469 6f6e  f an observation
+00000260: 2e20 4966 204e 6f6e 6520 2d20 7769 6c6c  . If None - will
+00000270: 206e 6f74 2062 6520 7370 6563 6966 6965   not be specifie
+00000280: 6420 756e 6465 7220 706c 6f74 2e7a 1154  d under plot.z.T
+00000290: 6974 6c65 206f 6620 7468 6520 706c 6f74  itle of the plot
+000002a0: 7a3c 4c61 6265 6c20 6e65 6172 2063 6f6c  z<Label near col
+000002b0: 6f72 6261 722e 204d 6f73 7420 6675 6e63  orbar. Most func
+000002c0: 7469 6f6e 7320 6f76 6572 7269 6465 2074  tions override t
+000002d0: 6869 7320 7061 7261 6d65 7465 722e 7a57  his parameter.zW
+000002e0: 4c61 6265 6c20 756e 6465 7220 706c 6f74  Label under plot
+000002f0: 2e20 5573 7561 6c6c 7920 696e 636c 7564  . Usually includ
+00000300: 6573 2064 6174 652f 7469 6d65 2c20 6c6f  es date/time, lo
+00000310: 6361 7469 6f6e 2061 6e64 2066 7265 7175  cation and frequ
+00000320: 656e 6379 206f 6620 616e 206f 6273 6572  ency of an obser
+00000330: 7661 7469 6f6e 2e7a 3a54 7570 6c65 2063  vation.z:Tuple c
+00000340: 6f6e 7461 696e 696e 6720 6d69 6e20 616e  ontaining min an
+00000350: 6420 6d61 7820 7661 6c75 6573 206f 6620  d max values of 
+00000360: 7468 6520 636f 6c6f 7262 6172 2073 6361  the colorbar sca
+00000370: 6c65 2e7a 5850 6174 6820 746f 2073 6176  le.zXPath to sav
+00000380: 6520 7468 6520 706c 6f74 2e20 4d75 7374  e the plot. Must
+00000390: 2069 6e63 6c75 6465 206e 616d 652e 2049   include name. I
+000003a0: 6620 6e6f 7420 7370 6563 6966 6965 6420  f not specified 
+000003b0: 2d20 7468 6520 706c 6f74 2077 696c 6c20  - the plot will 
+000003c0: 6e6f 7420 6265 2073 6176 6564 2e7a 1149  not be saved.z.I
+000003d0: 6d61 6765 2072 6573 6f6c 7574 696f 6e2e  mage resolution.
+000003e0: 7a1e 4120 636f 6c6f 726d 6170 2074 6f20  z.A colormap to 
+000003f0: 7573 6520 696e 2074 6865 2070 6c6f 742e  use in the plot.
+00000400: 7a2b 466f 726d 6174 7465 7220 6f66 206e  z+Formatter of n
+00000410: 756d 6265 7273 206f 6e20 7468 6520 636f  umbers on the co
+00000420: 6c6f 7262 6172 2073 6361 6c65 2e7a 2341  lorbar scale.z#A
+00000430: 2063 6f6c 6f72 2074 6f20 6669 6c6c 206e   color to fill n
+00000440: 702e 6e61 6e20 696e 2074 6865 2070 6c6f  p.nan in the plo
+00000450: 742e 7a23 4120 636f 6c6f 7220 746f 2066  t.z#A color to f
+00000460: 696c 6c20 6e70 2e69 6e66 2069 6e20 7468  ill np.inf in th
+00000470: 6520 706c 6f74 2e7a 5844 6966 6665 7265  e plot.zXDiffere
+00000480: 6e63 6520 6265 7477 6565 6e20 6c6f 6361  nce between loca
+00000490: 6c20 7469 6d65 2061 6e64 2055 5443 2e20  l time and UTC. 
+000004a0: 4966 2073 7065 6369 6669 6564 202d 206c  If specified - l
+000004b0: 6f63 616c 2074 696d 6520 6973 2073 686f  ocal time is sho
+000004c0: 776e 2069 6e73 7465 6164 206f 6620 5554  wn instead of UT
+000004d0: 4329 0eda 0264 74da 0370 6f73 da04 6672  C)...dt..pos..fr
+000004e0: 6571 da05 7469 746c 65da 0862 6172 6c61  eq..title..barla
+000004f0: 6265 6cda 0970 6c6f 746c 6162 656c da05  bel..plotlabel..
+00000500: 6362 6c69 6dda 0673 6176 6574 6fda 0364  cblim..saveto..d
+00000510: 7069 da04 636d 6170 da08 6362 666f 726d  pi..cmap..cbform
+00000520: 6174 da08 6e61 6e63 6f6c 6f72 da08 696e  at..nancolor..in
+00000530: 6663 6f6c 6f72 da0a 6c6f 6361 6c5f 7469  fcolor..local_ti
+00000540: 6d65 e92c 0100 00da 0776 6972 6964 6973  me.,.....viridis
+00000550: da05 626c 6163 6bda 0577 6869 7465 7a29  ..black..whitez)
+00000560: 5475 706c 655b 6e70 2e6e 6461 7272 6179  Tuple[np.ndarray
+00000570: 2c20 6e70 2e6e 6461 7272 6179 2c20 6e70  , np.ndarray, np
+00000580: 2e6e 6461 7272 6179 5d7a 0f64 6174 6574  .ndarray]z.datet
+00000590: 696d 6520 7c20 4e6f 6e65 7a21 5475 706c  ime | Nonez!Tupl
+000005a0: 655b 666c 6f61 742c 2066 6c6f 6174 2c20  e[float, float, 
+000005b0: 666c 6f61 745d 207c 204e 6f6e 657a 0c66  float] | Nonez.f
+000005c0: 6c6f 6174 207c 204e 6f6e 657a 0a73 7472  loat | Nonez.str
+000005d0: 207c 204e 6f6e 657a 1a54 7570 6c65 5b66   | Nonez.Tuple[f
+000005e0: 6c6f 6174 2c20 666c 6f61 745d 207c 204e  loat, float] | N
+000005f0: 6f6e 65da 0369 6e74 da03 7374 727a 0a69  one..int..strz.i
+00000600: 6e74 207c 204e 6f6e 6529 0fda 0464 6174  nt | None)...dat
+00000610: 6172 0800 0000 7209 0000 0072 0a00 0000  ar....r....r....
+00000620: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000630: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00000640: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00000650: 0000 7215 0000 0063 0f00 0000 0000 0000  ..r....c........
+00000660: 0000 0000 1600 0000 0900 0000 4300 0001  ............C...
+00000670: 7372 0200 007c 0664 016b 0872 a664 027d  sr...|.d.k.r.d.}
+00000680: 067c 0264 016b 0972 367c 0664 037c 0264  .|.d.k.r6|.d.|.d
+00000690: 0419 0064 059b 0464 067c 0264 0719 0064  ...d...d.|.d...d
+000006a0: 059b 0464 089d 0537 007d 067c 0164 016b  ...d...7.}.|.d.k
+000006b0: 0972 8c7c 0e64 016b 0872 607c 0664 0974  .r.|.d.k.r`|.d.t
+000006c0: 00a0 017c 0164 0aa1 0217 0064 0817 0037  ...|.d.....d...7
+000006d0: 007d 066e 2c74 027c 0e74 0383 0272 8c7c  .}.n,t.|.t...r.|
+000006e0: 0664 0b74 00a0 017c 0174 047c 0e64 0c8d  .d.t...|.t.|.d..
+000006f0: 0117 0064 0aa1 0217 0064 0d17 0037 007d  ...d.....d...7.}
+00000700: 067c 0364 016b 0972 a67c 0664 0e7c 0364  .|.d.k.r.|.d.|.d
+00000710: 0f9b 0464 109d 0337 007d 067c 0770 e274  ...d...7.}.|.p.t
+00000720: 05a0 067c 0064 1119 007c 0064 1119 0074  ...|.d...|.d...t
+00000730: 056a 070b 006b 0319 00a1 0174 05a0 087c  .j...k.....t...|
+00000740: 0064 1119 007c 0064 1119 0074 056a 076b  .d...|.d...t.j.k
+00000750: 0319 00a1 0166 027d 0774 05a0 0974 05a0  .....f.}.t...t..
+00000760: 0a7c 0064 1119 00a1 017c 0764 0719 0064  .|.d.....|.d...d
+00000770: 1217 007c 0064 1119 00a1 037d 0f74 027c  ...|.d.....}.t.|
+00000780: 0a74 0b83 0290 0172 1c74 0c7c 0a19 007d  .t.....r.t.|...}
+00000790: 0a7c 0aa0 0d7c 0ca1 0101 007c 0aa0 0e7c  .|...|.....|...|
+000007a0: 0da1 0101 0074 056a 0f6a 107c 0f74 05a0  .....t.j.j.|.t..
+000007b0: 117c 0fa1 0164 138d 027d 1074 126a 1364  .|...d...}.t.j.d
+000007c0: 1464 158d 017d 117c 116a 1464 1664 1764  .d...}.|.j.d.d.d
+000007d0: 188d 027d 127c 126a 157c 0064 0419 007c  ...}.|.j.|.d...|
+000007e0: 0064 0719 007c 107c 0a7c 0764 0419 007c  .d...|.|.|.d...|
+000007f0: 0764 0719 0064 1964 1a8d 077d 137c 126a  .d...d.d...}.|.j
+00000800: 1664 1b64 1c64 1d8d 0201 007c 12a0 1764  .d.d.d.....|...d
+00000810: 1ea1 0101 007c 126a 1864 1f64 2064 2164  .....|.j.d.d d!d
+00000820: 0467 0464 2164 228d 0201 007c 126a 1964  .g.d!d"....|.j.d
+00000830: 2364 2464 2564 268d 0301 007c 126a 1964  #d$d%d&....|.j.d
+00000840: 2764 2464 1b64 288d 0301 0074 126a 1a7c  'd$d.d(....t.j.|
+00000850: 1364 2964 2a7c 0b64 2b8d 046a 1b7c 0564  .d)d*|.d+..j.|.d
+00000860: 2c64 2d8d 0201 0074 126a 1c7c 0464 2e64  ,d-....t.j.|.d.d
+00000870: 2f64 308d 0301 0074 126a 1d7c 0664 2c64  /d0....t.j.|.d,d
+00000880: 318d 0201 007c 0864 016b 0990 0272 6e74  1....|.d.k...rnt
+00000890: 1e6a 1fa0 207c 08a1 015c 027d 147d 1574  .j.. |...\.}.}.t
+000008a0: 1e6a 1fa0 217c 14a1 0190 0273 5074 227c  .j..!|.....sPt"|
+000008b0: 1483 0164 046b 0490 0272 5074 1ea0 237c  ...d.k...rPt..#|
+000008c0: 14a1 0101 0074 126a 247c 087c 0964 3264  .....t.j$|.|.d2d
+000008d0: 338d 0301 0074 12a0 257c 11a1 0101 0064  3....t..%|.....d
+000008e0: 0153 007c 1153 0029 347a a80a 2020 2020  .S.|.S.)4z..    
+000008f0: 4120 636f 7265 2066 756e 6374 696f 6e20  A core function 
+00000900: 666f 7220 6772 6170 6869 6320 6765 6e65  for graphic gene
+00000910: 7261 7469 6f6e 206f 6e20 7468 6520 7669  ration on the vi
+00000920: 7369 626c 6520 736b 7920 6669 656c 642e  sible sky field.
+00000930: 0a20 2020 2053 6565 2061 6c6c 2061 7661  .    See all ava
+00000940: 696c 6162 6c65 206f 7074 696f 6e20 6c69  ilable option li
+00000950: 7374 6564 2069 6e20 6469 6f6e 7079 2e70  sted in dionpy.p
+00000960: 6c6f 745f 6b77 6172 6773 2e0a 0a20 2020  lot_kwargs...   
+00000970: 203a 7265 7475 726e 3a20 4120 6d61 7470   :return: A matp
+00000980: 6c6f 746c 6962 2066 6967 7572 652e 0a20  lotlib figure.. 
+00000990: 2020 204e da00 7a0e 506f 7369 7469 6f6e     N..z.Position
+000009a0: 3a20 6c61 743d 7201 0000 007a 032e 3366  : lat=r....z..3f
+000009b0: 7a06 2c20 6c6f 6e3d e901 0000 00da 010a  z., lon=........
+000009c0: 7a0a 5554 4320 7469 6d65 3a20 7a0e 2559  z.UTC time: z.%Y
+000009d0: 2d25 6d2d 2564 2025 483a 254d 7a0c 4c6f  -%m-%d %H:%Mz.Lo
+000009e0: 6361 6c20 7469 6d65 3a20 2901 da05 686f  cal time: )...ho
+000009f0: 7572 737a 020a 207a 0b46 7265 7175 656e  ursz.. z.Frequen
+00000a00: 6379 3a20 7a03 2e31 667a 0420 4d48 7ae9  cy: z..1fz. MHz.
+00000a10: 0200 0000 6700 0000 0084 d797 4129 01da  ....g.......A)..
+00000a20: 046d 6173 6b29 02e9 0800 0000 7223 0000  .mask)......r#..
+00000a30: 0029 01da 0766 6967 7369 7a65 e96f 0000  .)...figsize.o..
+00000a40: 00da 0570 6f6c 6172 2901 da0a 7072 6f6a  ...polar)...proj
+00000a50: 6563 7469 6f6e da04 6175 746f 2904 7211  ection..auto).r.
+00000a60: 0000 00da 0476 6d69 6eda 0476 6d61 78da  .....vmin..vmax.
+00000a70: 0773 6861 6469 6e67 da04 6772 6179 fa01  .shading..gray..
+00000a80: 3a29 02da 0563 6f6c 6f72 da09 6c69 6e65  :)...color..line
+00000a90: 7374 796c 65da 0153 e95a 0000 00e9 3c00  style..S.Z....<.
+00000aa0: 0000 e91e 0000 0029 015a 0846 6f6e 7473  .......).Z.Fonts
+00000ab0: 697a 65da 0462 6f74 68da 056d 616a 6f72  ize..both..major
+00000ac0: e90b 0000 0029 03da 0461 7869 73da 0577  .....)...axis..w
+00000ad0: 6869 6368 da09 6c61 6265 6c73 697a 65da  hich..labelsize.
+00000ae0: 0179 2903 7237 0000 0072 3800 0000 da0a  .y).r7...r8.....
+00000af0: 6c61 6265 6c63 6f6c 6f72 671b 2fdd 2406  labelcolorg./.$.
+00000b00: 81a5 3f67 7b14 ae47 e17a b43f 2903 da08  ..?g{..G.z.?)...
+00000b10: 6672 6163 7469 6f6e da03 7061 64da 0666  fraction..pad..f
+00000b20: 6f72 6d61 74e9 0a00 0000 2902 da05 6c61  ormat.....)...la
+00000b30: 6265 6cda 0473 697a 65e9 0e00 0000 e914  bel..size.......
+00000b40: 0000 0029 02da 0866 6f6e 7473 697a 6572  ...)...fontsizer
+00000b50: 3d00 0000 2901 7244 0000 00da 0574 6967  =...).rD.....tig
+00000b60: 6874 2902 7210 0000 00da 0b62 626f 785f  ht).r......bbox_
+00000b70: 696e 6368 6573 2926 7203 0000 00da 0873  inches)&r......s
+00000b80: 7472 6674 696d 65da 0a69 7369 6e73 7461  trftime..isinsta
+00000b90: 6e63 6572 1a00 0000 7204 0000 00da 026e  ncer....r......n
+00000ba0: 70da 066e 616e 6d69 6eda 0369 6e66 da06  p..nanmin..inf..
+00000bb0: 6e61 6e6d 6178 da05 7768 6572 65da 0569  nanmax..where..i
+00000bc0: 7369 6e66 721b 0000 0072 0600 0000 da07  sinfr....r......
+00000bd0: 7365 745f 6261 64da 0873 6574 5f6f 7665  set_bad..set_ove
+00000be0: 72da 026d 61da 0561 7272 6179 da05 6973  r..ma..array..is
+00000bf0: 6e61 6eda 0370 6c74 da06 6669 6775 7265  nan..plt..figure
+00000c00: da0b 6164 645f 7375 6270 6c6f 74da 0a70  ..add_subplot..p
+00000c10: 636f 6c6f 726d 6573 68da 0467 7269 64da  colormesh..grid.
+00000c20: 1773 6574 5f74 6865 7461 5f7a 6572 6f5f  .set_theta_zero_
+00000c30: 6c6f 6361 7469 6f6e da0a 7365 745f 7274  location..set_rt
+00000c40: 6963 6b73 da0b 7469 636b 5f70 6172 616d  icks..tick_param
+00000c50: 73da 0863 6f6c 6f72 6261 72da 0973 6574  s..colorbar..set
+00000c60: 5f6c 6162 656c 720b 0000 00da 0678 6c61  _labelr......xla
+00000c70: 6265 6cda 026f 73da 0470 6174 68da 0573  bel..os..path..s
+00000c80: 706c 6974 da06 6578 6973 7473 da03 6c65  plit..exists..le
+00000c90: 6eda 086d 616b 6564 6972 73da 0773 6176  n..makedirs..sav
+00000ca0: 6566 6967 da05 636c 6f73 6529 1672 1c00  efig..close).r..
+00000cb0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000cc0: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000cd0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000ce0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+00000cf0: 0000 0072 1500 0000 da09 706c 6f74 5f64  ...r......plot_d
+00000d00: 6174 615a 0b6d 6173 6b65 645f 6461 7461  ataZ.masked_data
+00000d10: da03 6669 67da 0261 78da 0369 6d67 da04  ..fig..ax..img..
+00000d20: 6865 6164 da04 7461 696c a900 726d 0000  head..tail..rm..
+00000d30: 00fa 3e2f 686f 6d65 2f6c 6170 3164 656d  ..>/home/lap1dem
+00000d40: 2f64 6576 2d70 7974 686f 6e2f 6469 6f6e  /dev-python/dion
+00000d50: 7079 2f73 7263 2f64 696f 6e70 792f 6d6f  py/src/dionpy/mo
+00000d60: 6475 6c65 732f 706c 6f74 7469 6e67 2e70  dules/plotting.p
+00000d70: 79da 0a70 6f6c 6172 5f70 6c6f 741e 0000  y..polar_plot...
+00000d80: 0073 7600 0000 0017 0801 0401 0801 2201  .sv...........".
+00000d90: 0801 0801 0201 12ff 0603 0a01 0201 0201  ................
+00000da0: 0401 0c00 02ff 02ff 0204 02fc 02ff 0407  ................
+00000db0: 0801 1202 3e01 2401 0c01 0801 0a01 0a02  ....>.$.........
+00000dc0: 1602 0c01 0e01 0401 0601 0601 0201 0201  ................
+00000dd0: 0601 0601 02f9 0609 0e01 0a01 1601 1001  ................
+00000de0: 1001 1201 0200 02ff 0603 1001 0e01 0a01  ................
+00000df0: 1001 1c01 0a01 1001 0a01 0401 726f 0000  ............ro..
+00000e00: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000e10: 0000 0200 0000 4300 0001 7308 0000 0074  ......C...s....t
+00000e20: 007c 008e 0053 0029 014e 2901 726f 0000  .|...S.).N).ro..
+00000e30: 0029 01da 0470 6172 7372 6d00 0000 726d  .)...parsrm...rm
+00000e40: 0000 0072 6e00 0000 da0f 706f 6c61 725f  ...rn.....polar_
+00000e50: 706c 6f74 5f73 7461 7271 0000 0073 0200  plot_starq...s..
+00000e60: 0000 0001 7271 0000 0029 0e4e 4e4e 4e4e  ....rq...).NNNNN
+00000e70: 4e4e 4e72 1600 0000 7217 0000 004e 7218  NNNr....r....Nr.
+00000e80: 0000 0072 1900 0000 4e29 10da 0a5f 5f66  ...r....N)...__f
+00000e90: 7574 7572 655f 5f72 0200 0000 725f 0000  uture__r....r_..
+00000ea0: 0072 0300 0000 7204 0000 00da 0674 7970  .r....r......typ
+00000eb0: 696e 6772 0500 0000 da05 6e75 6d70 7972  ingr......numpyr
+00000ec0: 4900 0000 da0a 6d61 7470 6c6f 746c 6962  I.....matplotlib
+00000ed0: 7206 0000 0072 0700 0000 7254 0000 00da  r....r....rT....
+00000ee0: 0b70 6c6f 745f 6b77 6172 6773 726f 0000  .plot_kwargsro..
+00000ef0: 0072 7100 0000 726d 0000 0072 6d00 0000  .rq...rm...rm...
+00000f00: 726d 0000 0072 6e00 0000 da08 3c6d 6f64  rm...rn.....<mod
+00000f10: 756c 653e 0100 0000 734a 0000 000c 0208  ule>....sJ......
+00000f20: 0110 010c 0208 010c 010c 0302 0102 0202  ................
+00000f30: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000f40: 0102 0102 0102 f106 1500 0100 0100 0100  ................
+00000f50: 0100 0100 0100 0100 0100 0100 0100 0100  ................
+00000f60: 0100 0100 f12c 53                        .....,S
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/col_freq_agg.csv` & `dionpy-0.99.7/src/dionpy/modules/col_freq_agg.csv`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/collision_models.py` & `dionpy-0.99.7/src/dionpy/modules/collision_models.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/src/dionpy/modules/helpers.py` & `dionpy-0.99.7/src/dionpy/modules/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import os
 from typing import Iterable, Sequence
 
 import healpy as hp
 import numpy as np
 from ffmpeg_progress_yield import FfmpegProgress
-from pymap3d import aer2geodetic, Ellipsoid as pmEllipsoid
+from pymap3d import aer2geodetic, Ellipsoid
 from tqdm import tqdm
 
 from .ion_tools import srange
 
+R_EARTH = 6378100.0
+
 
 class TextColor:
     """
     Provides formatters for terminal text coloring.
     """
 
     PURPLE = "\033[95m"
@@ -24,29 +26,14 @@
     GREEN = "\033[92m"
     YELLOW = "\033[93m"
     RED = "\033[91m"
     BOLD = "\033[1m"
     UNDERLINE = "\033[4m"
     END = "\033[0m"
 
-
-class Ellipsoid(pmEllipsoid):
-    """
-    Custom ellipsoid for pymap3d package. Implements a simple sphere.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.semimajor_axis = 6378100.0
-        self.semiminor_axis = 6378100.0
-        self.flattening = 0.0
-        self.thirdflattening = 0.0
-        self.eccentricity = 0.0
-
-
 def none_or_array(vals: None | Iterable) -> np.ndarray | None:
     """
     Used for data loading from HDF files. Converts not None values to np.arrays.
     """
     if vals is None:
         return None
     return np.array(vals)
@@ -84,15 +71,15 @@
     :param el: Elevation of observation(s) in deg.
     :param az: Azimuth of observation(s) in deg.
     :param height: Height of observable point(s) in km.
     :param pos: Geographical coordinates and height in m of the telescope
     :return: Observable geographical latitude and longitude.
     """
     d_srange = srange(np.deg2rad(90 - el), height * 1e3)
-    obs_lat, obs_lon, _ = aer2geodetic(az, el, d_srange, *pos, ell=Ellipsoid())
+    obs_lat, obs_lon, _ = aer2geodetic(az, el, d_srange, *pos, ell=Ellipsoid(R_EARTH, R_EARTH))
     return obs_lat, obs_lon
 
 
 def elaz_mesh(gridsize: int) -> [np.ndarray, np.ndarray]:
     """
     :param gridsize: Grid resolution.
     :return: Meshgrid of elevation and azimuth for all visible sky.
```

### Comparing `dionpy-0.99.6/src/dionpy/modules/parallel.py` & `dionpy-0.99.7/src/dionpy/modules/parallel.py`

 * *Files identical despite different names*

### Comparing `dionpy-0.99.6/setup.py` & `dionpy-0.99.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,26 +16,26 @@
  'ffmpeg-progress-yield>=0.3.0,<0.4.0',
  'h5py>=3.7.0,<4.0.0',
  'healpy>=1.16.1,<2.0.0',
  'iricore>=1.3.1,<2.0.0',
  'it>=1.0.0,<2.0.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.22,<2.0',
- 'pymap3d>=2.9.1,<3.0.0',
+ 'pymap3d>=3.0.1,<4.0.0',
  'pytz>=2022.1,<2023.0',
  'scipy>=1.9.3,<2.0.0',
  'setuptools>=67.6.1,<68.0.0',
  'sphinx-autodoc-typehints>=1.19.1,<2.0.0',
  'sphinx-rtd-theme>=1.0.0,<2.0.0',
  'sphinxcontrib-bibtex>=2.5.0,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'dionpy',
-    'version': '0.99.6',
+    'version': '0.99.7',
     'description': 'Dynamic ionosphere model for global 21 cm experiments',
     'long_description': '[//]: # (![]&#40;docs/images/logos/logo_wide.png&#41;)\n\n# DIonPy\nThe `dionpy` package provides model of ionosphere refraction and attenuation based on the \n[IRI2020 Ionosphere Model](https://irimodel.org/).\n\nMore details are available at our [documentation page](https://dionpy.readthedocs.io/en/latest/).',
     'author': 'Vadym Bidula',
     'author_email': 'vadym.bidula@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lap1dem/dionpy',
```

### Comparing `dionpy-0.99.6/PKG-INFO` & `dionpy-0.99.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dionpy
-Version: 0.99.6
+Version: 0.99.7
 Summary: Dynamic ionosphere model for global 21 cm experiments
 Home-page: https://github.com/lap1dem/dionpy
 License: MIT
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: ffmpeg-progress-yield (>=0.3.0,<0.4.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: healpy (>=1.16.1,<2.0.0)
 Requires-Dist: iricore (>=1.3.1,<2.0.0)
 Requires-Dist: it (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: numpy (>=1.22,<2.0)
-Requires-Dist: pymap3d (>=2.9.1,<3.0.0)
+Requires-Dist: pymap3d (>=3.0.1,<4.0.0)
 Requires-Dist: pytz (>=2022.1,<2023.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0)
 Requires-Dist: sphinxcontrib-bibtex (>=2.5.0,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
```

