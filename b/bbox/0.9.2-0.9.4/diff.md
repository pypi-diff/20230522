# Comparing `tmp/bbox-0.9.2.tar.gz` & `tmp/bbox-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbox-0.9.2.tar", last modified: Thu Apr  2 03:52:45 2020, max compression
+gzip compressed data, was "bbox-0.9.4.tar", max compression
```

## Comparing `bbox-0.9.2.tar` & `bbox-0.9.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2020-04-02 03:30:44.897222 bbox-0.9.2/LICENSE
--rw-r--r--   0        0        0      408 2020-04-02 03:50:26.258601 bbox-0.9.2/bbox/__init__.py
--rw-r--r--   0        0        0     7046 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/bbox2d.py
--rw-r--r--   0        0        0    10320 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/bbox2d_list.py
--rw-r--r--   0        0        0     9394 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/bbox3d.py
--rw-r--r--   0        0        0      758 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/box_modes.py
--rw-r--r--   0        0        0     4969 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/geometry.py
--rw-r--r--   0        0        0     4870 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/metrics.py
--rw-r--r--   0        0        0     2490 2020-04-02 03:30:44.897222 bbox-0.9.2/bbox/utils.py
--rw-r--r--   0        0        0      526 2020-04-02 03:51:41.466484 bbox-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      649 2020-04-02 03:52:46.010488 bbox-0.9.2/setup.py
--rw-r--r--   0        0        0      529 2020-04-02 03:52:46.011252 bbox-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-07-26 12:07:16.264048 bbox-0.9.4/LICENSE
+-rw-r--r--   0        0        0      399 2023-05-22 15:33:02.082287 bbox-0.9.4/bbox/__init__.py
+-rw-r--r--   0        0        0     7483 2022-07-26 12:07:16.265801 bbox-0.9.4/bbox/bbox2d.py
+-rw-r--r--   0        0        0    10314 2022-07-26 12:07:16.266261 bbox-0.9.4/bbox/bbox2d_list.py
+-rw-r--r--   0        0        0     9388 2022-07-26 12:07:16.266728 bbox-0.9.4/bbox/bbox3d.py
+-rw-r--r--   0        0        0      758 2022-07-26 12:07:16.267198 bbox-0.9.4/bbox/box_modes.py
+-rw-r--r--   0        0        0     5101 2023-05-22 15:30:24.267436 bbox-0.9.4/bbox/geometry.py
+-rw-r--r--   0        0        0     4961 2023-05-22 15:24:14.304875 bbox-0.9.4/bbox/metrics.py
+-rw-r--r--   0        0        0     2519 2023-05-22 15:20:21.884975 bbox-0.9.4/bbox/utils.py
+-rw-r--r--   0        0        0      517 2023-05-22 15:33:23.702937 bbox-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 bbox-0.9.4/PKG-INFO
```

### Comparing `bbox-0.9.2/LICENSE` & `bbox-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbox-0.9.2/bbox/bbox2d.py` & `bbox-0.9.4/bbox/bbox2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         The values are 0 for XYWH format and 1 for XYXY format. See :py:mod:`~bbox.box_modes`.
 
     Raises:
         ValueError: If `x` is not of length 4.
         TypeError: If `x` is not of type {list, tuple, numpy.ndarray, BBox2D}
 
     """
+
     def __init__(self, x, mode=XYWH):
         # Copy constructor makes the constructor idempotent
         if isinstance(x, BBox2D):
             x = x.numpy(mode=mode)
 
         elif isinstance(x, (list, tuple)):
             if len(x) != 4:
@@ -38,30 +39,30 @@
             if x.ndim >= 2:
                 x = x.flatten()
             if x.size != 4:
                 raise ValueError(
                     "Invalid input length. Input should have 4 elements.")
         else:
             raise TypeError(
-                "Expected input to constructor to be a 4 element " \
-                    "list, tuple, numpy ndarray, or BBox2D object.")
+                "Expected input to constructor to be a 4 element "
+                "list, tuple, numpy ndarray, or BBox2D object.")
 
         if mode == XYXY:
             w = x[2] - x[0] + 1
             h = x[3] - x[1] + 1
         elif mode == XYWH:
             w = x[2]
             h = x[3]
         else:
             raise ValueError('argument mode has invalid value')
 
-        self._x1 = np.float(x[0])
-        self._y1 = np.float(x[1])
-        self._w = np.float(w)
-        self._h = np.float(h)
+        self._x1 = float(x[0])
+        self._y1 = float(x[1])
+        self._w = float(w)
+        self._h = float(h)
 
         # (x2, y2) will be used for indexing, hence we need to subtract 1
         self._x2 = self._x1 + self._w - 1
         self._y2 = self._y1 + self._h - 1
 
     def __eq__(self, x):
         if not isinstance(x, BBox2D):
@@ -231,15 +232,15 @@
         """
         Return bounding box as a numpy vector of length 4.
         Format depends on ``mode`` flag (default is XYWH).
 
         Args:
             mode (BoxMode2D): Mode in which to return the box. See :py:mod:`~bbox.box_modes`.
         """
-        return np.asarray(self.tolist(mode=mode), dtype=np.float)
+        return np.asarray(self.tolist(mode=mode), dtype=float)
 
     def __repr__(self):
         return "BBox2D([{x}, {y}, {w}, {h}])".format(x=self.x1, y=self.y1, w=self.w, h=self.h)
 
     def mul(self, s):
         """
         Multiply the box by a scalar. Used for scaling bounding boxes.
@@ -253,7 +254,22 @@
         return BBox2D([self.x1*s, self.y1*s, self.x2*s, self.y2*s], mode=XYXY)
 
     def __mul__(self, s):
         return self.mul(s)
 
     def __rmul__(self, s):
         return self.mul(s)
+
+    def contains(self, point):
+        """
+        Check if `point` is inside the bounding box.
+
+        Args:
+            point (:py:class:`Iterable`): Vector of 2 values (x, y).
+        """
+        try:
+            if len(point) != 2:
+                raise ValueError("Invalid argument point.")
+        except:
+            raise ValueError("Argument is not an iterable.")
+
+        return self.x1 <= point[0] <= self.x2 and self.y1 <= point[1] <= self.y2
```

### Comparing `bbox-0.9.2/bbox/bbox2d_list.py` & `bbox-0.9.4/bbox/bbox2d_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         Append a bounding box to the bounding box list.
 
         Args:
             x: Bounding box to append.
         """
         if isinstance(x, (tuple, list, np.ndarray)):
             try:
-                x = np.asarray(x, dtype=np.float)
+                x = np.asarray(x, dtype=float)
             except (ValueError,):
                 raise ValueError(
                     "Expected list, tuple, or numpy array of ints/floats")
 
             if x.ndim == 1:
                 x = x[np.newaxis, :]
 
@@ -279,15 +279,15 @@
 
         Args:
             x: Bounding box to insert.
             idx (:py:class:`int`): Position where to insert bounding box.
         """
         if isinstance(x, (tuple, list, np.ndarray)):
             try:
-                x = np.asarray(x, dtype=np.float)
+                x = np.asarray(x, dtype=float)
             except (ValueError,):
                 raise ValueError(
                     "Expected list, tuple, or numpy array of ints/floats")
 
             if x.ndim > 1 or x.shape[0] != 4:
                 raise ValueError(
                     "Input should have shape Nx4, got {0}".format(x.shape))
```

### Comparing `bbox-0.9.2/bbox/bbox3d.py` & `bbox-0.9.4/bbox/bbox3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             raise ValueError("Center coordinates should be a vector of size 3")
         self._c = c
 
     def __valid_scalar(self, x):
         if not np.isscalar(x):
             raise ValueError("Value should be a scalar")
         else:  # x is a scalar so we check for numeric type
-            if not isinstance(x, (np.float, np.int)):
+            if not isinstance(x, (float, int)):
                 raise TypeError("Value needs to be either a float or an int")
         return x
 
     @property
     def cx(self):
         """
         :py:class:`float`: X coordinate of center.
```

### Comparing `bbox-0.9.2/bbox/box_modes.py` & `bbox-0.9.4/bbox/box_modes.py`

 * *Files identical despite different names*

### Comparing `bbox-0.9.2/bbox/geometry.py` & `bbox-0.9.4/bbox/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,16 @@
         min2 = min(min2, projection)
         max2 = max(max2, projection)
 
     if max1 >= min2 and max2 >= min1:
         d = min(max2 - min1, max1 - min2)
         # push a bit more than needed so the shapes do not overlap in future
         # tests due to float precision
-        d_over_o_squared = d/np.dot(o, o) + 1e-10
-        pv = d_over_o_squared*o
+        d_over_o_squared = d / np.dot(o, o) + 1e-10
+        pv = d_over_o_squared * o
         return False, pv
     else:
         return True, None
 
 
 def polygon_collision(p1, p2):
     """
@@ -138,40 +138,45 @@
     Area is computed using the Shoelace Algorithm.
 
     Args:
         polygon: 2D array of points.
     """
     x = polygon[:, 0]
     y = polygon[:, 1]
-    area = (np.dot(x, np.roll(y, -1)) -
-            np.dot(np.roll(x, -1), y))
-    return np.abs(area)/2
+    area = (np.dot(x, np.roll(y, -1)) - np.dot(np.roll(x, -1), y))
+    return np.abs(area) / 2
 
 
 def polygon_intersection(poly1, poly2):
     """
     Use the Sutherland-Hodgman algorithm to compute the intersection of 2 convex polygons.
     """
+
     def line_intersection(e1, e2, s, e):
         dc = e1 - e2
         dp = s - e
         n1 = np.cross(e1, e2)
         n2 = np.cross(s, e)
         n3 = 1.0 / (np.cross(dc, dp))
-        return np.array([(n1*dp[0] - n2*dc[0]) * n3, (n1*dp[1] - n2*dc[1]) * n3])
+        return np.array([(n1 * dp[0] - n2 * dc[0]) * n3,
+                         (n1 * dp[1] - n2 * dc[1]) * n3])
 
     def is_inside_edge(p, e1, e2):
         """Return True if e is inside edge (e1, e2)"""
-        return np.cross(e2-e1, p-e1) >= 0
+        return np.cross(e2 - e1, p - e1) >= 0
 
     output_list = poly1
     # e1 and e2 are the edge vertices for each edge in the clipping polygon
     e1 = poly2[-1]
 
     for e2 in poly2:
+        # If there is no point of intersection
+        if len(output_list) == 0:
+            break
+
         input_list = output_list
         output_list = []
         s = input_list[-1]
 
         for e in input_list:
             if is_inside_edge(e, e1, e2):
                 # if s in not inside edge (e1, e2)
```

### Comparing `bbox-0.9.2/bbox/metrics.py` & `bbox-0.9.4/bbox/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Functions for metrics related to 2D and 3D bounding boxes."""
 
-# pylint: disable=invalid-name,missing-docstring,assignment-from-no-return,logging-format-interpolation
+# pylint: disable=invalid-name,missing-docstring,assignment-from-no-return,logging-fstring-interpolation
 
 import logging
 
 import numpy as np
 
-from bbox import BBox2D, BBox2DList, BBox3D
 from bbox.geometry import polygon_area, polygon_collision, polygon_intersection
 
+from .bbox2d import BBox2D
+from .bbox2d_list import BBox2DList
+from .bbox3d import BBox3D
+
 logger = logging.getLogger(__name__)
 
 
 def iou_2d(a: BBox2D, b: BBox2D):
     """
     Compute the Intersection over Union (IoU) of a pair of 2D bounding boxes.
 
@@ -34,30 +37,30 @@
     """
 
     xA = np.maximum(a.x1, b.x1)
     yA = np.maximum(a.y1, b.y1)
     xB = np.minimum(a.x2, b.x2)
     yB = np.minimum(a.y2, b.y2)
 
-    logger.debug("xA={0} yA={1} xB={2} yB={3}".format(xA, yA, xB, yB))
+    logger.debug("xA={xA} yA={yA} xB={xB} yB={yB}")
 
     inter_w = xB - xA + 1
     inter_w = inter_w * (inter_w >= 0)
 
     inter_h = yB - yA + 1
     inter_h = inter_h * (inter_h >= 0)
 
     intersection = inter_w * inter_h
 
-    logger.debug("jaccard_index: intersection={0}".format(intersection))
+    logger.debug(f"jaccard_index: intersection={intersection}")
 
     a_area = a.width * a.height
     b_area = b.width * b.height
 
-    logger.debug("jaccard_index: a_area: {0}, b_area: {1}".format(a_area, b_area))
+    logger.debug(f"jaccard_index: a_area: {a_area}, b_area: {b_area}")
 
     iou = intersection / (a_area + b_area - intersection)
 
     # set nan and +/- inf to 0
     if np.isinf(iou) or np.isnan(iou):
         iou = 0
 
@@ -87,16 +90,16 @@
 
     # We need to add a trailing dimension so that max/min gives us a (N,N) matrix
     xA = np.maximum(a.x1[:, np.newaxis], b.x1[:, np.newaxis].T)
     yA = np.maximum(a.y1[:, np.newaxis], b.y1[:, np.newaxis].T)
     xB = np.minimum(a.x2[:, np.newaxis], b.x2[:, np.newaxis].T)
     yB = np.minimum(a.y2[:, np.newaxis], b.y2[:, np.newaxis].T)
 
-    logger.debug("\nmulti_jaccard_index:\nxA\n{0}\nyA\n{1}\nxB\n{2}\nyB\n{3}".format(
-        xA, yA, xB, yB))
+    logger.debug(
+        "\nmulti_jaccard_index:\nxA\n{xA}\nyA\n{yA}\nxB\n{xB}\nyB\n{yB}")
 
     inter_w = xB - xA + 1
     inter_w[inter_w < 0] = 0
 
     inter_h = yB - yA + 1
     inter_h[inter_h < 0] = 0
 
@@ -104,30 +107,30 @@
     # thus we are aggressive about freeing memory up.
     del xA
     del yA
     del xB
     del yB
 
     intersection = inter_w * inter_h
-    logger.debug(
-        "\nmulti_jaccard_index intersection:\n {0}".format(intersection))
+    logger.debug(f"\nmulti_jaccard_index intersection:\n {intersection}")
 
     a_area = a.width[:, np.newaxis] * a.height[:, np.newaxis]
     b_area = b.width[:, np.newaxis] * b.height[:, np.newaxis]
     logger.debug(
-        "\nmulti_jaccard_index:\n a_area:\n {0} \nb_area:\n {1}".format(a_area, b_area))
+        f"\nmulti_jaccard_index:\n a_area:\n {a_area} \nb_area:\n {b_area}")
 
     iou = intersection / (a_area + b_area.T - intersection)
 
     # set nan and +/- inf to 0
     iou[np.isinf(iou)] = 0
     iou[np.isnan(iou)] = 0
 
     return iou
 
+
 def iou_3d(a: BBox3D, b: BBox3D):
     """
     Compute the Intersection over Union (IoU) of a pair of 3D bounding boxes.
 
     Alias for `jaccard_index_3d`.
     """
     return jaccard_index_3d(a, b)
@@ -148,20 +151,24 @@
         :py:class:`float`: The IoU of the 2 bounding boxes.
     """
     # check if the two boxes don't overlap
     if not polygon_collision(a.p[0:4, 0:2], b.p[0:4, 0:2]):
         return np.round_(0, decimals=5)
 
     intersection_points = polygon_intersection(a.p[0:4, 0:2], b.p[0:4, 0:2])
+    # If intersection_points is empty, means the boxes don't intersect
+    if len(intersection_points) == 0:
+        return 0.0
+
     inter_area = polygon_area(intersection_points)
 
     zmax = np.minimum(a.cz, b.cz)
     zmin = np.maximum(a.cz - a.h, b.cz - b.h)
 
-    inter_vol = inter_area * np.maximum(0, zmax-zmin)
+    inter_vol = inter_area * np.maximum(0, zmax - zmin)
 
     a_vol = a.l * a.w * a.h
     b_vol = b.l * b.w * b.h
 
     union_vol = (a_vol + b_vol - inter_vol)
 
     iou = inter_vol / union_vol
```

### Comparing `bbox-0.9.2/bbox/utils.py` & `bbox-0.9.4/bbox/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,41 +7,43 @@
 - [https://github.com/rbgirshick/py-faster-rcnn/blob/master/lib/nms/py_cpu_nms.py]
 """
 
 # pylint: disable=invalid-name,missing-docstring,assignment-from-no-return,logging-format-interpolation
 
 import numpy as np
 
-from bbox import BBox2DList
 from bbox.box_modes import XYXY
 
+from .bbox2d_list import BBox2DList
+
 
 def nms(bbl, scores, thresh):
     """
     Perform fast non-maximum suppression on a set of bounding boxes \
         given their associated confidences.
 
     Args:
         bbl (:py:class:`BBox2DList`): List of 2D bounding boxes.
         scores (:py:class:`list` or :py:class:`ndarray`): Scores for each bounding box.
 
     Raises:
         ValueError: If arguments are of incorrect type or size.
     """
     if bbl.shape[0] == 0:
-        return np.array([]).astype(np.int)
+        return np.array([]).astype(int)
 
     if not isinstance(scores, (list, np.ndarray)):
         raise ValueError("`scores` should be a list of numpy array")
 
     # convert to numpy array if it is a list
     scores = np.asarray(scores)
 
     if not scores.shape[0] == bbl.shape[0]:
-        raise ValueError("box list and scores should have the same number of elements.")
+        raise ValueError(
+            "box list and scores should have the same number of elements.")
 
     areas = bbl.w * bbl.h
     order = scores.argsort()[::-1]
 
     keep = []
     while order.size > 0:
         i = order[0]
@@ -57,34 +59,34 @@
         inter = w * h
 
         overlap = inter / (areas[i] + areas[order[1:]] - inter)
 
         idx = np.where(overlap <= thresh)[0]
         order = order[idx + 1]
 
-    return np.array(keep).astype(np.int)
+    return np.array(keep).astype(int)
 
 
 def aspect_ratio(bbox, ratios):
     """
     Enumerate box for each aspect ratio.
 
     Args:
         bbox (:py:class:`BBox2D`): 2D bounding box.
         ratios (:py:class:`list`): list of int/float values.
     """
 
     cx, cy = bbox.center()
     w, h = bbox.w, bbox.h
     size = w * h
-    ratios = np.asarray(ratios, dtype=np.float)
+    ratios = np.asarray(ratios, dtype=float)
 
     size_ratios = size / ratios
 
     ws = np.round(np.sqrt(size_ratios))
     hs = np.round(ws * ratios)
 
-    stack = np.vstack((cx - 0.5*(ws-1), cy - 0.5*(hs-1),
-                       cx + 0.5*(ws-1), cy + 0.5*(hs-1)))
+    stack = np.vstack((cx - 0.5 * (ws - 1), cy - 0.5 * (hs - 1),
+                       cx + 0.5 * (ws - 1), cy + 0.5 * (hs - 1)))
 
     boxes = BBox2DList(stack.T, mode=XYXY)
     return boxes
```

### Comparing `bbox-0.9.2/pyproject.toml` & `bbox-0.9.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "bbox"
-version = "0.9.2"
+version = "0.9.4"
 description = "Python library for 2D/3D bounding boxes"
 authors = ["Varun Agrawal <varagrawal@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.18.2"
+python = ">=3.8"
+numpy = "^1.22.0"
 pyquaternion = "^0.9.5"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.4.4"
 pendulum = "^2.1.0"
-codecov = "^2.0.22"
-coverage = "^5.0.4"
+coverage = ">=5.5"
 pytest-cov = "^2.8.1"
-pytest = "^5.4.1"
+pytest = "^6.2.5"
 matplotlib = "^3.2.1"
-pillow = "^7.1.0"
+pillow = "^9.3.0"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

