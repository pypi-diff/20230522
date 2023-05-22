# Comparing `tmp/colorsysx-1.0a1.tar.gz` & `tmp/colorsysx-1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-1.0a1.tar", last modified: Thu May 18 12:42:45 2023, max compression
+gzip compressed data, was "colorsysx-1.1a1.tar", last modified: Mon May 22 17:10:44 2023, max compression
```

## Comparing `colorsysx-1.0a1.tar` & `colorsysx-1.1a1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      506 2023-05-13 17:41:09.960408 colorsysx-1.0a1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-05-11 22:49:25.520127 colorsysx-1.0a1/.gitignore
--rw-r--r--   0        0        0     1082 2023-05-15 12:35:15.890023 colorsysx-1.0a1/LICENSE
--rw-r--r--   0        0        0     3186 2023-05-17 15:23:29.534628 colorsysx-1.0a1/README.md
--rw-r--r--   0        0        0     1448 2023-05-18 12:41:04.379228 colorsysx-1.0a1/colorsysx/__init__.py
--rw-r--r--   0        0        0     5566 2023-05-18 12:01:21.430173 colorsysx-1.0a1/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4482 2023-05-18 12:00:28.891978 colorsysx-1.0a1/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-11 02:07:41.913560 colorsysx-1.0a1/colorsysx/_helpers.py
--rw-r--r--   0        0        0      741 2023-05-13 16:25:55.939388 colorsysx-1.0a1/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2771 2023-05-18 11:59:52.814338 colorsysx-1.0a1/colorsysx/_yuv.py
--rw-r--r--   0        0        0     2569 2023-05-18 12:10:16.947498 colorsysx-1.0a1/colorsysx/weights.py
--rw-r--r--   0        0        0      819 2023-05-17 13:04:58.016321 colorsysx-1.0a1/pyproject.toml
--rw-r--r--   0        0        0     1261 2023-05-17 13:04:58.016321 colorsysx-1.0a1/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-13 01:06:47.992623 colorsysx-1.0a1/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-13 01:01:00.825464 colorsysx-1.0a1/tests/context.py
--rw-r--r--   0        0        0     5822 2023-05-18 12:07:06.124196 colorsysx-1.0a1/tests/test_glhs.py
--rw-r--r--   0        0        0     2710 2023-05-18 12:06:33.075493 colorsysx-1.0a1/tests/test_hcy.py
--rw-r--r--   0        0        0      592 2023-05-13 16:25:28.626827 colorsysx-1.0a1/tests/test_swizzle.py
--rw-r--r--   0        0        0      860 2023-05-18 12:09:20.418639 colorsysx-1.0a1/tests/test_weights.py
--rw-r--r--   0        0        0     1706 2023-05-18 12:07:20.784493 colorsysx-1.0a1/tests/test_yuv.py
--rw-r--r--   0        0        0     1030 2023-05-18 12:41:04.371228 colorsysx-1.0a1/tox.ini
--rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 colorsysx-1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-05-22 16:10:46.352674 colorsysx-1.1a1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       53 2023-05-22 16:10:46.352674 colorsysx-1.1a1/.gitignore
+-rw-r--r--   0        0        0     1082 2023-05-22 16:10:46.352674 colorsysx-1.1a1/LICENSE
+-rw-r--r--   0        0        0     3186 2023-05-22 16:10:46.416675 colorsysx-1.1a1/README.md
+-rw-r--r--   0        0        0     1448 2023-05-22 16:40:25.210787 colorsysx-1.1a1/colorsysx/__init__.py
+-rw-r--r--   0        0        0     6421 2023-05-22 16:59:01.212529 colorsysx-1.1a1/colorsysx/_glhs.py
+-rw-r--r--   0        0        0     4717 2023-05-22 16:35:31.724434 colorsysx-1.1a1/colorsysx/_hcy.py
+-rw-r--r--   0        0        0      379 2023-05-22 16:12:08.181596 colorsysx-1.1a1/colorsysx/_helpers.py
+-rw-r--r--   0        0        0     1246 2023-05-22 16:12:08.185596 colorsysx-1.1a1/colorsysx/_swizzle.py
+-rw-r--r--   0        0        0     3248 2023-05-22 16:59:34.920828 colorsysx-1.1a1/colorsysx/_yuv.py
+-rw-r--r--   0        0        0     2929 2023-05-22 16:46:12.301566 colorsysx-1.1a1/colorsysx/weights.py
+-rw-r--r--   0        0        0      819 2023-05-22 16:10:46.352674 colorsysx-1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1261 2023-05-22 16:10:46.416675 colorsysx-1.1a1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-22 16:12:08.185596 colorsysx-1.1a1/tests/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-22 16:12:08.189596 colorsysx-1.1a1/tests/context.py
+-rw-r--r--   0        0        0     1438 2023-05-22 16:57:48.499880 colorsysx-1.1a1/tests/test_deprecations.py
+-rw-r--r--   0        0        0     5806 2023-05-22 16:36:45.793029 colorsysx-1.1a1/tests/test_glhs.py
+-rw-r--r--   0        0        0     2734 2023-05-22 16:24:40.122637 colorsysx-1.1a1/tests/test_hcy.py
+-rw-r--r--   0        0        0      584 2023-05-22 16:31:57.978708 colorsysx-1.1a1/tests/test_swizzle.py
+-rw-r--r--   0        0        0      815 2023-05-22 16:12:08.185596 colorsysx-1.1a1/tests/test_weights.py
+-rw-r--r--   0        0        0     1724 2023-05-22 16:28:20.952886 colorsysx-1.1a1/tests/test_yuv.py
+-rw-r--r--   0        0        0     1030 2023-05-22 16:10:46.372674 colorsysx-1.1a1/tox.ini
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 colorsysx-1.1a1/PKG-INFO
```

### Comparing `colorsysx-1.0a1/LICENSE` & `colorsysx-1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0a1/README.md` & `colorsysx-1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0a1/colorsysx/__init__.py` & `colorsysx-1.1a1/colorsysx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "1.0a1"
+__version__ = "1.1a1"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
```

### Comparing `colorsysx-1.0a1/colorsysx/_hcy.py` & `colorsysx-1.1a1/colorsysx/_hcy.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,40 +33,42 @@
 from . import weights
 from ._helpers import clamp
 from . import _swizzle
 
 
 # Default values::
 
-DEFAULT_WEIGHTS = weights.ComponentWeights.REC709
+DEFAULT_WEIGHTS = weights.RGBWeights.REC709
 
 
 # Conversion functions::
 
-def rgb_to_hcy(r, g, b, w_rgb=None):
+def rgb_to_hcy(r, g, b, weights_rgb=None, w_rgb=None):
     """Converts from RGB to HCY.
 
-    The r, g, and b parameters are floats between 0 and 1 inclusive.  If
-    given, w_rgb specifies the luma weighting coefficients for the r, g,
-    and b components, in that order. It must be a tuple of 3 floats that
-    sum to 1, but this is not enforced. The default is
-    colorsysx.weights.W_RGB_REC709.
+    The "r", "g", and "b" parameters are floats between 0 and 1
+    inclusive. If given, "weights_rgb specifies the luma weighting
+    coefficients for the r, g, and b components, in that order. It must
+    be a tuple of 3 floats that sum to 1, but this is not enforced. The
+    default is colorsysx.weights.RGBWeights.REC709.
 
     Returns a tuple (h, c, y).
 
     """
 
+    weights_rgb = w_rgb or weights_rgb  # FIXME: remove in 2.0
+
     # Luma is a weighted sum of the three components.
-    if w_rgb is None:
-        w_rgb = DEFAULT_WEIGHTS
+    if weights_rgb is None:
+        weights_rgb = DEFAULT_WEIGHTS
 
     # Hue. First pick a sector based on the greatest RGB component, then add
     # the scaled difference of the other two RGB components.
     (comp_min, w_min), (comp_mid, w_mid), (comp_max, w_max) \
-        = sorted(zip([r, g, b], w_rgb))
+        = sorted(zip([r, g, b], weights_rgb))
 
     if comp_max == comp_min:
         return (0.0, 0.0, comp_max)
 
     # Compute hue
     mid_minus_min = comp_mid - comp_min
     max_minus_min = comp_max - comp_min
@@ -101,27 +103,30 @@
         c = (y - comp_min) / y
     else:
         c = (comp_max - y) / (1.0 - y)
 
     return (h, c, y)
 
 
-def hcy_to_rgb(h, c, y, w_rgb=None):
+def hcy_to_rgb(h, c, y, weights_rgb=None, w_rgb=None):
     """Converts from HCY to RGB.
 
-    The h, c, and y parameters are floats between 0 and 1 inclusive.
-    w_rgb has the same meaning and default value as in rgb_to_hcy().
+    The "h", "c", and "y" parameters are floats between 0 and 1 inclusive.
+    "weights_rgb" has the same meaning and default value as it does in
+    "rgb_to_hcy()".
 
     Returns a tuple of floats in the form (r, g, b), where each
     component is between 0 and 1 inclusive.
 
     """
 
-    if w_rgb is None:
-        w_rgb = DEFAULT_WEIGHTS
+    weights_rgb = w_rgb or weights_rgb  # FIXME: remove in 2.0
+
+    if weights_rgb is None:
+        weights_rgb = DEFAULT_WEIGHTS
 
     # Achromatic case
     if c == 0:
         return tuple(clamp(c, 0.0, 1.0) for c in (y, y, y))
 
     # Pick a sector based on the hue angle.
     # This determines the order in which {r, g, b} are selected from
@@ -131,28 +136,28 @@
     f = ((h % 1.0) * 6.0) - sector
     if (sector % 2) == 0:
         ff = f
     else:
         ff = 1.0 - f
 
     # Put the weights in min-to-max order.
-    mapping_indices = _swizzle.FROM_RGB_TO_MIN2MAX[sector]
-    w_min, w_mid, w_max = (w_rgb[i] for i in mapping_indices)
+    mapping_indices = _swizzle.FROM_RGB_TO_SORTED[sector]
+    w_min, w_mid, w_max = (weights_rgb[i] for i in mapping_indices)
 
     # Calculate the RGB components in min-to-max order.
     y_q = (w_mid * ff) + w_max
     if y <= y_q:
         comp_max = y + y*c*(1-y_q)/y_q
         comp_mid = y + y*c*(ff-y_q)/y_q
         comp_min = y - (y*c)
     else:
         comp_max = y + (1-y)*c
         comp_mid = y + (1-y)*c*(ff-y_q)/(1-y_q)
         comp_min = y - (1-y)*c*y_q/(1-y_q)
 
     # Back to RGB order
-    comps_min2max = (comp_min, comp_mid, comp_max)
+    comps_sorted = (comp_min, comp_mid, comp_max)
     comps_rgb = [
-        clamp(comps_min2max[i], 0.0, 1.0)
-        for i in _swizzle.FROM_MIN2MAX_TO_RGB[sector]
+        clamp(comps_sorted[i], 0.0, 1.0)
+        for i in _swizzle.FROM_SORTED_TO_RGB[sector]
     ]
     return comps_rgb
```

### Comparing `colorsysx-1.0a1/colorsysx/weights.py` & `colorsysx-1.1a1/colorsysx/weights.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,33 @@
 
 Each set of weights is a tuple of three floats that sum to exactly 1.
 They are used for calculating lightness terms by this package's colour
 conversion functions.
 
 """
 
+# Imports::
+
 import sys
 
 if sys.version_info >= (3, 11):
     import enum
 
     class _EnumBase (tuple, enum.ReprEnum):
         pass
 
 else:
 
     class _EnumBase (object):
         pass
 
 
-class ComponentWeights (_EnumBase):
+# Const namespaces::
+
+class RGBWeights (_EnumBase):
     """Weights for each RGB component, in typical red-green-blue order.
 
     These weighting tuples are appropriate for conversions which use a
     weighted sum of the individual colour components. The ones given
     here correspond to broadcast TV standards from different ages.
 
     * REC601: ITU-R Recommendation BT.601 (a.k.a. BT.470), as used in SDTV.
@@ -32,28 +36,31 @@
     * REC709: ITU-R Recommendation BT.709, as used in HDTV.
 
     * REC2020: ITU-R Recommendation BT.2020, as used in UHDTV.
 
     These weightings are appropriate for use with both the YUV and the
     GLHS pairs of conversion functions.
 
+    ("ComponentWeights" is a deprecated alias for this class name. It
+    will be removed in v2.0.)
+
     """
     # (R, G, B)
     REC601 = (0.299, 0.587, 0.114)
     REC709 = (0.2126, 0.7152, 0.0722)
     REC2020 = (0.2627, 0.678, 0.0593)
 
 
-class SortedComponentWeights (_EnumBase):
+class SortedWeights (_EnumBase):
     """Weights for RGB components when sorted by ascending numeric value.
 
     These weighting tuples are appropriate for the GLHS conversion
-    functions, where using different weights for the w_min2max parameter
-    makes the conversion operate like other well known cylindrical
-    lighness/hue/saturation models.
+    functions, where using different weights for the "weights_sorted"
+    parameter makes the conversion operate like other well known
+    cylindrical lighness/hue/saturation models.
 
     The weights are used to make a weighted sum of the three RGB
     components ordered by their numeric value, lowest first.
 
     * HSI: Weighting coefficients for the HSI model.
 
       For this model, the Intensity (or lightness) term is the
@@ -72,12 +79,21 @@
       valued RGB component. This produces the same results as
       colorsys.rgb_to_hls() and its inverse.
 
     References:
 
     * https://doi.org/10.1006/cgip.1993.1019
 
+    ("SortedComponentWeights" is a deprecated alias for this class name.
+    It will be removed in v2.0.)
+
     """
     # (Min, Mid, Max)
     HSI = (1/3, 1/3, 1/3)
     HSV = (0, 0, 1)
     HLS = (1/2, 0, 1/2)
+
+
+# Deprecated aliases, to be removed in version 2.0::
+
+ComponentWeights = RGBWeights
+SortedComponentWeights = SortedWeights
```

### Comparing `colorsysx-1.0a1/pyproject.toml` & `colorsysx-1.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0a1/requirements.txt` & `colorsysx-1.1a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0a1/tests/test_glhs.py` & `colorsysx-1.1a1/tests/test_glhs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,56 +8,56 @@
 from sys import float_info
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
-WEIGHTS_MIN2MAX = (
-    colorsysx.weights.SortedComponentWeights.HSI,
-    colorsysx.weights.SortedComponentWeights.HSV,
-    colorsysx.weights.SortedComponentWeights.HLS,
+WEIGHTS_SORTED = (
+    colorsysx.weights.SortedWeights.HSI,
+    colorsysx.weights.SortedWeights.HSV,
+    colorsysx.weights.SortedWeights.HLS,
 )
 WEIGHTS_RGB = (
-    colorsysx.weights.ComponentWeights.REC601,
-    colorsysx.weights.ComponentWeights.REC709,
-    colorsysx.weights.ComponentWeights.REC2020,
+    colorsysx.weights.RGBWeights.REC601,
+    colorsysx.weights.RGBWeights.REC709,
+    colorsysx.weights.RGBWeights.REC2020,
 )
 
 
 # Test funcs::
 
-def test_grey_is_grey_min2max():
+def test_grey_is_grey_sorted():
     """Neutral grey is always neutral grey."""
-    for w in WEIGHTS_MIN2MAX:
-        l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, w_min2max=w)
+    for w in WEIGHTS_SORTED:
+        l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, weights_sorted=w)
         assert abs(l - 0.5) <= EPSILON
         assert h <= EPSILON
         assert s <= EPSILON  # just a convention
 
 
 def test_grey_is_grey_rgb():
     """Neutral grey is always neutral grey."""
     for w in WEIGHTS_RGB:
-        l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, w_rgb=w)
+        l, h, s = colorsysx.rgb_to_glhs(0.5, 0.5, 0.5, weights_rgb=w)
         assert abs(l - 0.5) <= EPSILON
         assert h <= EPSILON
         assert s <= EPSILON  # just a convention
 
 
-def test_ranges_min2max():
+def test_ranges_sorted():
     """Output should lie within the stated bounds, and cover that range"""
     n = 16
     min_l, max_l = [1, 0]
     min_h, max_h = [1, 0]
     min_s, max_s = [1, 0]
-    for w in WEIGHTS_MIN2MAX:
+    for w in WEIGHTS_SORTED:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_min2max=w)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, weights_sorted=w)
             assert 0-EPSILON <= l <= 1+EPSILON
             assert 0-EPSILON <= h <= 1+EPSILON
             assert 0-EPSILON <= s <= 1+EPSILON
             min_l, max_l = min(l, min_l), max(l, max_l)
             min_h, max_h = min(h, min_h), max(h, max_h)
             min_s, max_s = min(s, min_s), max(s, max_s)
     assert min_l < EPSILON
@@ -73,39 +73,39 @@
     n = 16
     min_l, max_l = [1, 0]
     min_h, max_h = [1, 0]
     min_s, max_s = [1, 0]
     for w in WEIGHTS_RGB:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_rgb=w)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, weights_rgb=w)
             assert 0-EPSILON <= l <= 1+EPSILON
             assert 0-EPSILON <= h <= 1+EPSILON
             assert 0-EPSILON <= s <= 1+EPSILON
             min_l, max_l = min(l, min_l), max(l, max_l)
             min_h, max_h = min(h, min_h), max(h, max_h)
             min_s, max_s = min(s, min_s), max(s, max_s)
     assert min_l < EPSILON
     assert max_l > 1-EPSILON
     assert min_h < 1/12
     assert max_h > 1 - 1/12
     assert min_s < EPSILON
     assert max_s > 1-EPSILON
 
 
-def test_round_trips_min2max():
+def test_round_trips_sorted():
     """Should be able to convert to GHLS and back to RGB accurately."""
     n = 16
 
-    for w in WEIGHTS_MIN2MAX:
+    for w in WEIGHTS_SORTED:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_min2max=w)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, weights_sorted=w)
             assert 0 <= l <= 1
-            r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, w_min2max=w)
+            r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, weights_sorted=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
 
             fudge = 4
             assert abs(r1 - r0) <= EPSILON*fudge
             assert abs(g1 - g0) <= EPSILON*fudge
@@ -115,17 +115,17 @@
 def test_round_trips_rgb():
     """Should be able to convert to GHLS and back to RGB accurately."""
     n = 16
 
     for w in WEIGHTS_RGB:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, w_rgb=w)
+            l, h, s = colorsysx.rgb_to_glhs(r0, g0, b0, weights_rgb=w)
             assert 0 <= l <= 1
-            r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, w_rgb=w)
+            r1, g1, b1 = colorsysx.glhs_to_rgb(l, h, s, weights_rgb=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
 
             # Fudge factor seems pretty high.
             fudge = 20
             # Perhaps I should just be testing that 16bpc linear colour
@@ -141,36 +141,36 @@
     fudge = 1
     for rn, gn, bn in itertools.product(range(n+1), repeat=3):
         r, g, b = (rn/n, gn/n, bn/n)
 
         # "HLS" double hexcone model
         (gl1, gh1, gs1) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_min2max=colorsysx.weights.SortedComponentWeights.HLS,
+            weights_sorted=colorsysx.weights.SortedWeights.HLS,
         )
         (h1, l1, s1) = colorsys.rgb_to_hls(r, g, b)
         assert abs(gl1 - l1) <= EPSILON*fudge
         assert abs(gs1 - s1) <= EPSILON*fudge
         assert abs(gh1 - h1) <= EPSILON*fudge
 
         # "HSV" hexcone model
         (gl2, gh2, gs2) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_min2max=colorsysx.weights.SortedComponentWeights.HSV,
+            weights_sorted=colorsysx.weights.SortedWeights.HSV,
         )
         (h2, s2, v2) = colorsys.rgb_to_hsv(r, g, b)
         assert abs(gl2 - v2) <= EPSILON*fudge
         assert abs(gs2 - s2) <= EPSILON*fudge
         assert abs(gh2 - h2) <= EPSILON*fudge
 
         # "HCY" luma-based model
         (gl3, gh3, gs3) = colorsysx.rgb_to_glhs(
             r, g, b,
-            w_rgb=colorsysx.weights.ComponentWeights.REC709,
+            weights_rgb=colorsysx.weights.RGBWeights.REC709,
         )
         (h3, c3, y3) = colorsysx.rgb_to_hcy(
             r, g, b,
-            w_rgb=colorsysx.weights.ComponentWeights.REC709,
+            weights_rgb=colorsysx.weights.RGBWeights.REC709,
         )
         assert abs(gl3 - y3) <= EPSILON*fudge
         assert abs(gs3 - c3) <= EPSILON*fudge
         assert abs(gh3 - h3) <= EPSILON*fudge
```

### Comparing `colorsysx-1.0a1/tests/test_hcy.py` & `colorsysx-1.1a1/tests/test_hcy.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,53 +8,53 @@
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
 WEIGHTS = (
-    colorsysx.weights.ComponentWeights.REC601,
-    colorsysx.weights.ComponentWeights.REC709,
-    colorsysx.weights.ComponentWeights.REC2020,
+    colorsysx.weights.RGBWeights.REC601,
+    colorsysx.weights.RGBWeights.REC709,
+    colorsysx.weights.RGBWeights.REC2020,
 )
 
 
 # Test funcs::
 
 def test_grey_is_grey():
     """Neutral grey is always neutral grey."""
     for w in WEIGHTS:
-        h, c, y = colorsysx.rgb_to_hcy(0.5, 0.5, 0.5, w_rgb=w)
+        h, c, y = colorsysx.rgb_to_hcy(0.5, 0.5, 0.5, weights_rgb=w)
         assert abs(y - 0.5) <= EPSILON
         assert c <= EPSILON
         assert h <= EPSILON  # just a convention
 
 
 def test_pure_components_match_weights():
     """Pure r, g, and b produce the corresponding weight value in y."""
     for w in WEIGHTS:
         wr, wg, wb = w
-        h, c, y = colorsysx.rgb_to_hcy(1, 0, 0, w_rgb=w)
+        h, c, y = colorsysx.rgb_to_hcy(1, 0, 0, weights_rgb=w)
         assert abs(y - wr) <= EPSILON
-        h, c, y = colorsysx.rgb_to_hcy(0, 1, 0, w_rgb=w)
+        h, c, y = colorsysx.rgb_to_hcy(0, 1, 0, weights_rgb=w)
         assert abs(y - wg) <= EPSILON
-        h, c, y = colorsysx.rgb_to_hcy(0, 0, 1, w_rgb=w)
+        h, c, y = colorsysx.rgb_to_hcy(0, 0, 1, weights_rgb=w)
         assert abs(y - wb) <= EPSILON
 
 
 def test_ranges():
     """Output should lie within the stated bounds, and cover that range"""
     n = 16
     min_h, max_h = [1, 0]
     min_c, max_c = [1, 0]
     min_y, max_y = [1, 0]
     for w in WEIGHTS:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            h, c, y = colorsysx.rgb_to_hcy(r0, g0, b0, w_rgb=w)
+            h, c, y = colorsysx.rgb_to_hcy(r0, g0, b0, weights_rgb=w)
             assert 0-EPSILON <= h <= 1+EPSILON
             assert 0-EPSILON <= c <= 1+EPSILON
             assert 0-EPSILON <= y <= 1+EPSILON
             min_h, max_h = min(h, min_h), max(h, max_h)
             min_c, max_c = min(c, min_c), max(c, max_c)
             min_y, max_y = min(y, min_y), max(y, max_y)
     assert min_h < 1/12
@@ -67,17 +67,17 @@
 
 def test_round_trips():
     """Should be able to convert to GHLS and back to RGB accurately."""
     n = 16
     for w in WEIGHTS:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            h, c, y = colorsysx.rgb_to_hcy(r0, g0, b0, w_rgb=w)
+            h, c, y = colorsysx.rgb_to_hcy(r0, g0, b0, weights_rgb=w)
             assert 0 <= y <= 1
-            r1, g1, b1 = colorsysx.hcy_to_rgb(h, c, y, w_rgb=w)
+            r1, g1, b1 = colorsysx.hcy_to_rgb(h, c, y, weights_rgb=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
 
             # Oddly, the current GLHS implementation is worse (20×Epsilon)
             # for the same 3 sets of coefficients.
             fudge = 9
```

### Comparing `colorsysx-1.0a1/tests/test_swizzle.py` & `colorsysx-1.1a1/tests/test_swizzle.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from colorsysx import _swizzle
 
 
 def test_swizzle_pairs_are_inverses():
     """The sectoral swizzles must be reverse mappings of each other"""
 
-    from_min2max_to_rgb_generated = [
+    from_sorted_to_rgb_generated = [
         tuple(s.index(i) for i in (0, 1, 2))
-        for s in _swizzle.FROM_RGB_TO_MIN2MAX
+        for s in _swizzle.FROM_RGB_TO_SORTED
     ]
-    assert _swizzle.FROM_MIN2MAX_TO_RGB == from_min2max_to_rgb_generated
+    assert _swizzle.FROM_SORTED_TO_RGB == from_sorted_to_rgb_generated
 
-    from_rgb_to_min2max_generated = [
+    from_rgb_to_sorted_generated = [
         tuple(s.index(i) for i in (0, 1, 2))
-        for s in _swizzle.FROM_MIN2MAX_TO_RGB
+        for s in _swizzle.FROM_SORTED_TO_RGB
     ]
-    assert _swizzle.FROM_RGB_TO_MIN2MAX == from_rgb_to_min2max_generated
+    assert _swizzle.FROM_RGB_TO_SORTED == from_rgb_to_sorted_generated
```

### Comparing `colorsysx-1.0a1/tests/test_weights.py` & `colorsysx-1.1a1/tests/test_deprecations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-"""Test colorsysx.weights"""
+"""Reminder to remove deprecations at the promised version."""
 
-# Imports::
+from packaging.version import Version
 
 from .context import colorsysx
 
-from sys import float_info
 
-
-# Module vars::
-
-EPSILON = float_info.epsilon
-
-
-# Test funcs::
-
-def test_comp_weights():
-    weights = (
-        colorsysx.weights.ComponentWeights.REC601,
-        colorsysx.weights.ComponentWeights.REC709,
-        colorsysx.weights.ComponentWeights.REC2020,
-    )
-    for w in weights:
-        assert len(w) == 3
-        assert abs(1.0 - sum(w)) <= EPSILON
-        wr, rg, wb = w
-        assert abs(1.0 - (1.0*wr + 1.0*rg + 1.0*wb)) <= EPSILON
-
-
-def test_sorted_comp_weights():
-    weights = (
-        colorsysx.weights.SortedComponentWeights.HSI,
-        colorsysx.weights.SortedComponentWeights.HSV,
-        colorsysx.weights.SortedComponentWeights.HLS,
+def test_v2_deprecation_aliases():
+    # Test that the aliases are being respected
+    # This is fairly pathological code, don't copy this!
+    w_min2max_funcs = [
+        # These should accept the old "w_min2max" parameter,
+        # and convert it to "weights_sorted"
+        colorsysx.rgb_to_glhs,
+        colorsysx.glhs_to_rgb,
+    ]
+    w_rgb_funcs = [
+        # These should accept the old "w_rgb" parameter,
+        # and convert it to "weights_rgb"
+        colorsysx.rgb_to_hcy,
+        colorsysx.hcy_to_rgb,
+        colorsysx.rgb_to_glhs,
+        colorsysx.glhs_to_rgb,
+        colorsysx.rgb_to_yuv,
+        colorsysx.yuv_to_rgb,
+    ]
+    x, y, z = (0.5, 0.6, 0.7)
+    weights = (0.3, 0.5, 0.7)
+    for func in w_min2max_funcs:
+        res_w_min2max = func(x, y, z, w_min2max=weights)
+        res_weights_sorted = func(x, y, z, weights_sorted=weights)
+        assert res_w_min2max == res_weights_sorted
+    for func in w_rgb_funcs:
+        res_w_rgb = func(x, y, z, w_rgb=weights)
+        res_weights_rgb = func(x, y, z, weights_rgb=weights)
+        assert res_w_rgb == res_weights_rgb
+
+
+def test_v2_deprecations():
+    assert Version(colorsysx.__version__) < Version("2.0"), (
+        "v2.0+: remove w_rgb and w_min2max parameters, "
+        "and the old aliases in colorsysx.weights"
     )
-    for w in weights:
-        assert len(w) == 3
-        assert abs(1.0 - sum(w)) <= EPSILON
```

### Comparing `colorsysx-1.0a1/tests/test_yuv.py` & `colorsysx-1.1a1/tests/test_yuv.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,51 +8,51 @@
 import itertools
 
 
 # Module vars::
 
 EPSILON = float_info.epsilon
 WEIGHTS = (
-    colorsysx.weights.ComponentWeights.REC601,
-    colorsysx.weights.ComponentWeights.REC709,
-    colorsysx.weights.ComponentWeights.REC2020,
+    colorsysx.weights.RGBWeights.REC601,
+    colorsysx.weights.RGBWeights.REC709,
+    colorsysx.weights.RGBWeights.REC2020,
 )
 
 
 # Test funcs::
 
 def test_grey_is_grey():
     """Neutral grey is always neutral grey."""
     for w in WEIGHTS:
-        y, u, v = colorsysx.rgb_to_yuv(0.5, 0.5, 0.5, w_rgb=w)
+        y, u, v = colorsysx.rgb_to_yuv(0.5, 0.5, 0.5, weights_rgb=w)
         assert abs(y - 0.5) <= EPSILON
         assert u <= EPSILON
         assert v <= EPSILON
 
 
 def test_pure_components_match_weights():
     """Pure r, g, and b produce the corresponding weight value in y."""
     for w in WEIGHTS:
         wr, wg, wb = w
-        y, u, v = colorsysx.rgb_to_yuv(1, 0, 0, w_rgb=w)
+        y, u, v = colorsysx.rgb_to_yuv(1, 0, 0, weights_rgb=w)
         assert abs(y - wr) <= EPSILON
-        y, u, v = colorsysx.rgb_to_yuv(0, 1, 0, w_rgb=w)
+        y, u, v = colorsysx.rgb_to_yuv(0, 1, 0, weights_rgb=w)
         assert abs(y - wg) <= EPSILON
-        y, u, v = colorsysx.rgb_to_yuv(0, 0, 1, w_rgb=w)
+        y, u, v = colorsysx.rgb_to_yuv(0, 0, 1, weights_rgb=w)
         assert abs(y - wb) <= EPSILON
 
 
 def test_round_trips():
     """Should be able to convert to GHLS and back to RGB accurately."""
     n = 16
     for w in WEIGHTS:
         for rn, gn, bn in itertools.product(range(n+1), repeat=3):
             r0, g0, b0 = (rn/n, gn/n, bn/n)
-            y, u, v = colorsysx.rgb_to_yuv(r0, g0, b0, w_rgb=w)
+            y, u, v = colorsysx.rgb_to_yuv(r0, g0, b0, weights_rgb=w)
             assert 0 <= y <= 1
-            r1, g1, b1 = colorsysx.yuv_to_rgb(y, u, v, w_rgb=w)
+            r1, g1, b1 = colorsysx.yuv_to_rgb(y, u, v, weights_rgb=w)
             assert 0 <= r1 <= 1
             assert 0 <= g1 <= 1
             assert 0 <= b1 <= 1
             assert abs(r1 - r0) <= EPSILON * 2  # doubled, due to clamping
             assert abs(g1 - g0) <= EPSILON * 2
             assert abs(b1 - b0) <= EPSILON * 2
```

### Comparing `colorsysx-1.0a1/tox.ini` & `colorsysx-1.1a1/tox.ini`

 * *Files identical despite different names*

### Comparing `colorsysx-1.0a1/PKG-INFO` & `colorsysx-1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 1.0a1
+Version: 1.1a1
 Summary: Extra, human-relevant, colour spaces derived from RGB.
 Author-email: Andrew Chadwick <a.t.chadwick@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
```

