# Comparing `tmp/unitrack-4.5.0.tar.gz` & `tmp/unitrack-4.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitrack-4.5.0.tar", last modified: Tue May 16 12:16:08 2023, max compression
+gzip compressed data, was "unitrack-4.6.9.tar", last modified: Mon May 22 19:42:59 2023, max compression
```

## Comparing `unitrack-4.5.0.tar` & `unitrack-4.6.9.tar`

### file list

```diff
@@ -1,46 +1,41 @@
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1068 2023-05-13 07:58:27.000000 unitrack-4.5.0/LICENSE
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      729 2023-05-16 12:16:08.319301 unitrack-4.5.0/PKG-INFO
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)       75 2023-05-13 07:58:27.000000 unitrack-4.5.0/README.md
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     6393 2023-05-16 12:15:34.000000 unitrack-4.5.0/pyproject.toml
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)       38 2023-05-16 12:16:08.319301 unitrack-4.5.0/setup.cfg
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/unitrack/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      855 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/__init__.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/assignment/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      275 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/assignment/__init__.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3512 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/auction.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1470 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/base_assignment.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2357 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/greedy.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2254 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/hungarian.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1349 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/jonker.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      162 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/constants.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1926 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/context.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/costs/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      225 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/costs/__init__.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1125 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/base_cost.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      720 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/category.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3710 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/iou.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2224 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/reduce.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3134 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/wrap.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/fields/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      129 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/fields/__init__.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1274 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/fields/base_field.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      485 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/fields/value.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     4043 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/memory.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/stages/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      128 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/stages/__init__.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1391 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/association.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1068 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/base_stage.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1304 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/lost.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/states/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      127 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/states/__init__.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      992 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/states/base_state.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2177 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/states/value.py
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2774 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/tracker.py
-drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/unitrack.egg-info/
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      729 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/PKG-INFO
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1175 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/SOURCES.txt
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        1 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/dependency_links.txt
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      436 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/requires.txt
--rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        9 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/top_level.txt
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.173502 unitrack-4.6.9/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1068 2023-05-13 07:58:27.000000 unitrack-4.6.9/LICENSE
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     4948 2023-05-22 19:42:59.173502 unitrack-4.6.9/PKG-INFO
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     4294 2023-05-17 06:17:50.000000 unitrack-4.6.9/README.md
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     6393 2023-05-16 12:15:34.000000 unitrack-4.6.9/pyproject.toml
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)       38 2023-05-22 19:42:59.173502 unitrack-4.6.9/setup.cfg
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.163501 unitrack-4.6.9/sources/
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.163501 unitrack-4.6.9/sources/unitrack/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      861 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/__init__.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.173502 unitrack-4.6.9/sources/unitrack/assignment/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      275 2023-05-16 12:15:34.000000 unitrack-4.6.9/sources/unitrack/assignment/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3512 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/assignment/auction.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1470 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/assignment/base_assignment.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2357 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/assignment/greedy.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2254 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/assignment/hungarian.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1349 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/assignment/jonker.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      190 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/constants.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.173502 unitrack-4.6.9/sources/unitrack/costs/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      225 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/costs/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1889 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/costs/base_cost.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      587 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/costs/category.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3176 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/costs/iou.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2224 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/costs/reduce.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3088 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/costs/wrap.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     6227 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/memory.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.173502 unitrack-4.6.9/sources/unitrack/stages/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      128 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/stages/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1966 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/stages/association.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      845 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/stages/base_stage.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1318 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/stages/lost.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.173502 unitrack-4.6.9/sources/unitrack/states/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      127 2023-05-13 07:58:27.000000 unitrack-4.6.9/sources/unitrack/states/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1666 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/states/base_state.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2127 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/states/value.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1870 2023-05-22 19:42:36.000000 unitrack-4.6.9/sources/unitrack/tracker.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-22 19:42:59.163501 unitrack-4.6.9/sources/unitrack.egg-info/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     4948 2023-05-22 19:42:59.000000 unitrack-4.6.9/sources/unitrack.egg-info/PKG-INFO
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1040 2023-05-22 19:42:59.000000 unitrack-4.6.9/sources/unitrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        1 2023-05-22 19:42:59.000000 unitrack-4.6.9/sources/unitrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      436 2023-05-22 19:42:59.000000 unitrack-4.6.9/sources/unitrack.egg-info/requires.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        9 2023-05-22 19:42:59.000000 unitrack-4.6.9/sources/unitrack.egg-info/top_level.txt
```

### Comparing `unitrack-4.5.0/LICENSE` & `unitrack-4.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/pyproject.toml` & `unitrack-4.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/__init__.py` & `unitrack-4.6.9/sources/unitrack/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     Process that assigns each Detection to a Tracklet.
 Lost
     State of a Tracklet that has not been assigned to a detection at the current
     or a previous frame.
 
 """
 
-__version__ = "4.5.0"
+__version__ = "4.6.9"
 
-from . import costs, fields, stages, states  # noqa: F401
-from .context import *  # noqa: F401, F403
+from . import assignment, costs, stages, states  # noqa: F401
+from .constants import *  # noqa: F401, F403
 from .memory import *  # noqa: F401, F403
 from .tracker import *  # noqa: F401, F403
```

### Comparing `unitrack-4.5.0/sources/unitrack/assignment/auction.py` & `unitrack-4.6.9/sources/unitrack/assignment/auction.py`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/assignment/base_assignment.py` & `unitrack-4.6.9/sources/unitrack/assignment/base_assignment.py`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/assignment/greedy.py` & `unitrack-4.6.9/sources/unitrack/assignment/greedy.py`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/assignment/hungarian.py` & `unitrack-4.6.9/sources/unitrack/assignment/hungarian.py`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/assignment/jonker.py` & `unitrack-4.6.9/sources/unitrack/assignment/jonker.py`

 * *Files identical despite different names*

### Comparing `unitrack-4.5.0/sources/unitrack/costs/base_cost.py` & `unitrack-4.6.9/sources/unitrack/costs/base_cost.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import abstractmethod
 from typing import Iterable, Optional, Sequence
 
 import torch
 from tensordict import TensorDictBase
 
-__all__ = ["Cost"]
+__all__ = ["Cost", "FieldCost"]
 
 
 class Cost(torch.nn.Module):
     """
     A cost module computes an assignment cost matrix between detections and
     tracklets.
     """
@@ -16,30 +16,59 @@
     required_fields: torch.jit.Final[list[str]]
 
     def __init__(self, required_fields: Iterable[str]):
         super().__init__()
 
         self.required_fields = list(set(required_fields))
 
+    @abstractmethod
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+        """
+        Computes the assignment costs between previous tracklets and current
+        detections.
+
+        This is an abstract method that should be overwritten.
+
+        Parameters
+        ----------
+        cs
+            Candidate observations (N).
+        ds
+            Detections (M).
+        Returns
+        -------
+            Cost matrix (N x M).
+        """
+        raise NotImplementedError
+
+
+class FieldCost(Cost):
+    field: torch.jit.Final[str]
+
+    def __init__(self, field: str):
+        super().__init__(required_fields=[field])
+
+        self.field = field
+
     def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
-        return self.compute(cs, ds)
+        return self.compute(cs.get(self.field), ds.get(self.field))
 
     @abstractmethod
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+    def compute(self, cs: torch.Tensor, ds: torch.Tensor) -> torch.Tensor:
         """
-        Computes the assignment costs between :class:`.Tracklets` and
-        :class:`.TensorDictBase`.
+        Computes the assignment costs between previous tracklets and current
+        detections.
 
-        This is an abstract method that should be overwritten be subclassses.
+        This is an abstract method that should be overwritten.
 
         Parameters
         ----------
-        ts
-            Tracklets instance.
+        cs
+            Candidate observations (N) values for a single field.
         ds
-            TensorDictBase instance.
+            Detections (M) values for a single field.
 
         Returns
         -------
-            Cost matrix
+            Cost matrix (N x M).
         """
         raise NotImplementedError
```

### Comparing `unitrack-4.5.0/sources/unitrack/costs/iou.py` & `unitrack-4.6.9/sources/unitrack/costs/iou.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,60 +6,43 @@
 version of that package.
 """
 
 
 from typing import Final, Tuple
 
 import torch
-from tensordict import TensorDictBase
 from torch import Tensor
 from torchvision.ops import box_iou
 
-from .base_cost import Cost
+from .base_cost import FieldCost
 
 __all__ = ["MaskIoU", "BoxIoU"]
 
 DEFAULT_EPS: Final = 1e-8
 
 
-class MaskIoU(Cost):
+class MaskIoU(FieldCost):
     """
     Computes IoU cost matrix between two sets of bitmasks.
     """
 
     eps: torch.jit.Final[float]
-    field: torch.jit.Final[str]
 
-    def __init__(self, field: str, eps: float = DEFAULT_EPS):
-        super().__init__(required_fields=(field,))
-
-        self.field: Final = field
+    def __init__(self, eps: float = DEFAULT_EPS, **kwargs):
+        super().__init__(**kwargs)
         self.eps = eps
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> Tensor:
-        return _naive_mask_iou(cs.get(self.field), ds.get(self.field), self.eps)
-
-
-class BoxIoU(Cost):
-    """
-    Computes the generalized IoU cost matrix between two sets of bounding boxes.
-    """
+    def compute(self, cs: Tensor, ds: Tensor) -> Tensor:
+        return _naive_mask_iou(cs, ds, self.eps)
 
-    field: torch.jit.Final[str]
-    eps: torch.jit.Final[float]
-
-    def __init__(self, field: str, eps: float = DEFAULT_EPS):
-        super().__init__(required_fields=(field,))
-
-        self.field = field
-        self.eps = eps
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> Tensor:
-        cs_field = _pad_degenerate_boxes(cs.get(self.field))
-        ds_field = _pad_degenerate_boxes(ds.get(self.field))
+class BoxIoU(MaskIoU):
+    def compute(self, cs: Tensor, ds: Tensor) -> Tensor:
+        cs_field = _pad_degenerate_boxes(cs)
+        ds_field = _pad_degenerate_boxes(ds)
 
         return 1.0 - _complete_box_iou(cs_field, ds_field, self.eps)
 
 
 def _naive_mask_iou(cs: Tensor, ds: Tensor, eps: float) -> Tensor:
     cs_m = cs.reshape(len(cs), -1).int()
     ds_m = ds.reshape(len(ds), -1).int()
```

### Comparing `unitrack-4.5.0/sources/unitrack/costs/reduce.py` & `unitrack-4.6.9/sources/unitrack/costs/reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self, cost: Cost, weight: float):
         super().__init__(required_fields=cost.required_fields)
 
         self.cost = cost
         self.weight = weight
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
         return self.weight * self.cost(cs, ds)
 
 
 class Reduction(Enum):
     """
     Reduction method for :class:`.Reduce` cost module.
     """
@@ -62,15 +62,15 @@
         self.method = method
         self.costs = nn.ModuleList(costs)
         if weights is None:
             weights = [1.0] * len(costs)
 
         self.register_buffer("weights", torch.tensor(weights, dtype=torch.float32).unsqueeze_(-1).unsqueeze_(-1))
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
         costs = torch.stack([cost(cs, ds) for cost in self.costs])
         costs = costs * self.weights
         costs = _reduce_stack(costs, self.method)
 
         return costs
```

### Comparing `unitrack-4.5.0/sources/unitrack/costs/wrap.py` & `unitrack-4.6.9/sources/unitrack/costs/wrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,89 +5,86 @@
 from torch import Tensor
 
 from .base_cost import Cost
 
 __all__ = ["Distance", "Cosine"]
 
 
-DEFAULT_EPS: Final = 1e-8
+DEFAULT_EPS: Final = 1e-7
 
 
 class Distance(Cost):
     """
     Cost function that wraps a distance module.
     """
 
-    select: List[int]
-    p: float
+    select: torch.jit.Final[List[int]]
+    p: torch.jit.Final[float]
+    field: torch.jit.Final[str]
 
     def __init__(
         self,
         field: str,
         select: Optional[List[int]] = None,
         p_norm: float = 2.0,
-        alpha: float = 1.0,
     ):
         """
         Parameters
         ----------
         critereon
             Module that computes distance between two fields
         field_name
             Name if the field to read tensors from that are passed to the
             ``torch.cdist`` function.
         select
             List of indices to select from the field.
         p_norm
             Value of p-norm.
-        alpha
-            Result distance ^ alpha
         """
         super().__init__(required_fields=(field,))
 
         self.field = field
 
         if select is None:
             select = []
 
         self.select = select  # type: ignore
-        self.p_norm = p_norm
-        self.alpha = alpha
+        self.p = p_norm
 
     def get_field(self, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[torch.Tensor, torch.Tensor]:
         ts_field = cs.get(self.field)
         ds_field = ds.get(self.field)
 
         if len(self.select) > 0:
             assert ts_field.shape[1] >= max(self.select)
             assert ds_field.shape[1] >= max(self.select)
 
             ts_field = ts_field[:, self.select]
             ds_field = ds_field[:, self.select]
 
         return ts_field, ds_field
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase):
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
-        return torch.cdist(ts_field, ds_field, self.p_norm) * self.alpha
+        return torch.cdist(ts_field, ds_field, self.p, "donot_use_mm_for_euclid_dist")
 
 
 class Cosine(Distance):
     """
     Computes the distance between two fields based on a similarity measure with
     range $[0,1]$ by computing $1 - S(x,y)$.
     """
 
     def __init__(self, *args, eps: float = DEFAULT_EPS, **kwargs):
         super().__init__(*args, **kwargs)
         self.eps = eps
 
     def compute(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
-        return (1.0 - _cosine_similarity(ts_field, ds_field, eps=self.eps)) ** self.alpha
+        return 1.0 - _cosine_similarity(ts_field, ds_field, eps=self.eps)
 
 
 def _cosine_similarity(a: Tensor, b: Tensor, eps=DEFAULT_EPS) -> Tensor:
     """
     Manual computation of the cosine similarity.
 
     Based on: https://stackoverflow.com/questions/50411191/how-to-compute-the-cosine-similarity-in-pytorch-for-all-rows-in-a-matrix-with-re  # noqa: E501
```

### Comparing `unitrack-4.5.0/sources/unitrack/stages/association.py` & `unitrack-4.6.9/sources/unitrack/stages/association.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Tuple
 
 from tensordict import TensorDictBase
 
 from ..assignment import Assignment
-from ..context import Context
+from ..constants import KEY_FRAME, KEY_ID, KEY_INDEX
 from ..costs import Cost
 from .base_stage import Stage
 
 __all__ = ["Association"]
 
 
 class Association(Stage):
@@ -17,36 +17,58 @@
     """
 
     def __init__(
         self,
         cost: Cost,
         assignment: Assignment,
     ) -> None:
-        super().__init__([], [])
+        super().__init__()
 
         self.cost = cost
         self.assignment = assignment
 
         self._extend_required_fields(self.cost)
 
     def _extend_required_fields(self, *costs: Cost) -> None:
         for cost in costs:
             self.required_fields += cost.required_fields
 
-    def forward(self, ctx: Context, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[TensorDictBase, TensorDictBase]:
+    def forward(
+        self, ctx: TensorDictBase, cs: TensorDictBase, ds: TensorDictBase
+    ) -> Tuple[TensorDictBase, TensorDictBase]:
         if len(cs) == 0 or len(ds) == 0:
             return cs, ds
 
         cost_matrix = self.cost(cs, ds)
 
         matches, cs_fail_idx, ds_fail_idx = self.assignment(cost_matrix)
 
         if len(matches) > 0:
             cs_match = cs.get_sub_tensordict(matches[:, 0])
             ds_match = ds.get_sub_tensordict(matches[:, 1])
 
-            ctx.match(cs_match, ds_match)
+            self.match(cs_match, ds_match)
 
         cs_fail = cs.get_sub_tensordict(cs_fail_idx)
         ds_fail = ds.get_sub_tensordict(ds_fail_idx)
 
         return cs_fail, ds_fail
+
+    def match(self, cs: TensorDictBase, ds: TensorDictBase) -> None:
+        """
+        Match candidates to detections. Propagates data and IDs from detections to candidates.
+
+        Parameters
+        ----------
+        cs
+            Candidates
+        ds
+            Detections
+        """
+        for key, value in ds.items():
+            if key.startswith("_"):
+                continue
+            if key not in cs.keys():
+                continue
+            cs.set_(key, value)
+
+        cs.set_(KEY_INDEX, ds.get(KEY_INDEX))
```

### Comparing `unitrack-4.5.0/sources/unitrack/stages/base_stage.py` & `unitrack-4.6.9/sources/unitrack/stages/base_stage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 from abc import abstractmethod
 from typing import Iterable, List, Tuple
 
 import torch
 from tensordict import TensorDictBase
 
-from ..context import Context
-
 __all__ = ["Stage"]
 
 
 class Stage(torch.nn.Module):
     """
     Base class for stages in a ::class::`..Tracker`.
 
     Inputs to a stage are in the context data, or as fields of the detections.
     """
 
-    required_fields: torch.jit.Final[List[str]]
-    required_data: torch.jit.Final[List[str]]
-
     def __init__(
         self,
-        required_fields: Iterable[str],
-        required_data: Iterable[str],
+        required_fields: Iterable[str] = (),
     ):
         super().__init__()
 
         self.required_fields = list(required_fields)
-        self.required_data = list(required_data)
 
-    @torch.jit.unused
     def __repr__(self) -> str:
         req = ", ".join(self.required_fields)
         return f"{type(self).__name__}(fields=[{req}])"
 
     @abstractmethod
     def forward(
         self,
-        ctx: Context,
+        ctx: TensorDictBase,
         cs: TensorDictBase,
         ds: TensorDictBase,
     ) -> Tuple[TensorDictBase, TensorDictBase]:
         raise NotImplementedError
```

### Comparing `unitrack-4.5.0/sources/unitrack/stages/lost.py` & `unitrack-4.6.9/sources/unitrack/stages/lost.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Tuple
 
 import torch
 from tensordict import TensorDictBase
 
-from ..constants import KEY_FRAME
-from ..context import Context
+from ..constants import KEY_DELTA, KEY_FRAME
 from .base_stage import Stage
 
 __all__ = ["Lost"]
 
 
 class Lost(Stage):
     """
@@ -29,20 +28,22 @@
         """
         Parameters
         ----------
         max_lost
             Maximum amount of time a candidate may remain lost.
         """
 
-        super().__init__([], [])
+        super().__init__()
 
         assert max_lost > 0, max_lost
 
         self.max_lost = max_lost
 
-    def forward(self, ctx: Context, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[TensorDictBase, TensorDictBase]:
+    def forward(
+        self, ctx: TensorDictBase, cs: TensorDictBase, ds: TensorDictBase
+    ) -> Tuple[TensorDictBase, TensorDictBase]:
         if len(cs) == 0:
             return cs, ds
 
-        time_lost = ctx.frame - cs.get(KEY_FRAME) - ctx.delta
+        time_lost = ctx.get(KEY_FRAME) - cs.get(KEY_FRAME) - ctx.get(KEY_DELTA)
 
         return cs.get_sub_tensordict(time_lost > self.max_lost), ds
```

### Comparing `unitrack-4.5.0/sources/unitrack/states/value.py` & `unitrack-4.6.9/sources/unitrack/states/value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,79 @@
+from typing import TypeAlias
+
 import torch
+from torch import Tensor
 
 from .base_state import State
 
+DataType: TypeAlias = torch.dtype | str
+
+
+def _cast_dtype(dtype: DataType) -> torch.dtype:
+    if isinstance(dtype, str):
+        dtype = getattr(torch, dtype)
+    if not isinstance(dtype, torch.dtype):
+        raise ValueError(f"No a valid data type: {dtype}!")
+    return dtype
+
 
 class Value(State):
     """
     A :class:`.State` that holds values as-is without any updating logic
     implemented.
     """
 
-    values: torch.Tensor
+    values: Tensor
 
-    def __init__(self, dtype: torch.dtype | str):
+    def __init__(self, dtype: DataType):
         super().__init__()
-
-        if isinstance(dtype, str):
-            dtype = getattr(torch, dtype)
-        if not isinstance(dtype, torch.dtype):
-            raise ValueError(f"No a valid data type: {dtype}!")
+        dtype = _cast_dtype(dtype)
 
         self.register_buffer("values", torch.empty(0, dtype=dtype), persistent=False)
 
-    @torch.jit.export
-    def update(self, values: torch.Tensor) -> None:
+    def update(self, values: Tensor) -> None:
         self.values = values
 
-    @torch.jit.export
-    def extend(self, values: torch.Tensor) -> None:
+    def extend(self, values: Tensor) -> None:
         values_cat = torch.cat([self.values, values], dim=0)
         self.values = values_cat
 
-    @torch.jit.export
-    def observe(self) -> torch.Tensor:
+    def observe(self) -> Tensor:
         return self.values
 
-    @torch.jit.export
     def reset(self) -> None:
         self.values = self.values[:0]
 
 
 class MeanValues(State):
     """
     A :class:`.State` that computes the mean of its values over a given window
     size.
     """
 
-    values_history: torch.Tensor
+    values_history: Tensor
 
     def __init__(self, window: int, dtype: torch.dtype | str):
         super().__init__()
 
         if isinstance(dtype, str):
             dtype = getattr(torch, dtype)
         if not isinstance(dtype, torch.dtype):
             raise ValueError(f"No a valid data type: {dtype}!")
 
         self.window = window
         self.register_buffer("values_history", torch.zeros((0,), dtype=dtype), persistent=False)
 
-    @torch.jit.export
-    def update(self, values: torch.Tensor) -> None:
+    def forward(self, values: Tensor) -> None:
         raise NotImplementedError
 
-    @torch.jit.export
-    def extend(self, values: torch.Tensor) -> None:
+    def extend(self, values: Tensor) -> None:
         values = values.unsqueeze(0)
         values = values.expand((self.values_history.shape[0], *values.shape))
 
         self.values_history = torch.cat([self.values_history, values], dim=1)
 
-    @torch.jit.export
-    def observe(self) -> torch.Tensor:
+    def observe(self) -> Tensor:
         return torch.mean(self.values_history, dim=0)
 
-    @torch.jit.export
     def reset(self) -> None:
         self.values_history = self.values_history[:0]
```

### Comparing `unitrack-4.5.0/sources/unitrack/tracker.py` & `unitrack-4.6.9/sources/unitrack/tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,62 @@
-from typing import Dict, List, Mapping, Tuple, cast
+from typing import Dict, List, Mapping, Sequence, Tuple, cast
 
 import torch
 import torch.nn as nn
 from tensordict import TensorDict, TensorDictBase
+from tensordict.nn import (
+    TensorDictModule, TensorDictModuleBase, TensorDictSequential,
+)
 
 from .constants import KEY_ACTIVE, KEY_FRAME, KEY_ID, KEY_INDEX, KEY_START
-from .context import Context
-from .fields import Field
 from .stages import Stage
 
 
 class MultiStageTracker(nn.Module):
     """
     Multi-stage tracker that applies a cascade of stages to a set of detections.
     """
 
-    def __init__(self, fields: Mapping[str, Field], stages: List[Stage]):
+    def __init__(self, fields: Sequence[TensorDictModule], stages: Sequence[Stage]):
         super().__init__()
 
         assert len(stages) > 0
 
+        self.fields = TensorDictSequential(*fields)
         self.stages = cast(List[Stage], nn.ModuleList(stages))
-        self.fields = cast(Dict[str, Field], nn.ModuleDict({**fields}))
-
-        self._validate()
-
-    def _validate(self):
-        for i, stage in enumerate(self.stages):
-            for id in stage.required_fields:
-                if id not in self.fields:
-                    raise ValueError(f"Field with ID '{id}' missing for {stage}!")
-
-    def get_required_fields(self) -> List[str]:
-        field_keys: List[str] = []
-        for f in self.fields.values():
-            field_keys += f.required_keys
-        return field_keys
-
-    def get_required_data(self) -> List[str]:
-        data_keys: List[str] = []
-        for f in self.stages:
-            data_keys += f.required_data
-        return data_keys
 
     def forward(
         self,
-        ctx: Context,
+        ctx: TensorDictBase,
         obs: TensorDictBase,
-    ) -> Tuple[TensorDictBase, TensorDictBase]:
+        inp: TensorDictBase,
+    ) -> tuple[TensorDictBase, TensorDictBase]:
         """
         Perform tracking, returns a tuple of updated observations and the field-values of new tracklets.
 
-        Parameters
-        ----------
-        ctx
-            Context object
-        obs
-            Observations
-        det
-            Detections
 
         Returns
         -------
         Tuple[TensorDict, TensorDict]
             Updated observations and field-values of new tracklets.
         """
 
-        new = self._apply_fields(ctx)
-        obs, new = self._apply_stages(ctx, obs, new)
+        # Read the amount of detections
+        num_det = inp.batch_size[0]
 
-        return obs, new
+        # Fields target (newly detected objects)
+        new = TensorDict(
+            {
+                KEY_INDEX: torch.arange(num_det, device=inp.device),
+            },
+            batch_size=[num_det],
+            device=inp.device,
+        )
+        self.fields(inp, tensordict_out=new)
 
-    def _apply_fields(self, ctx: Context) -> TensorDictBase:
-        items = {key: field(ctx) for key, field in self.fields.items()}
-        items[KEY_INDEX] = torch.arange(len(ctx.ids), device=ctx.ids.device)
-        return TensorDict(items, batch_size=ctx.ids.shape, device=ctx.ids.device)  # type: ignore
-
-    def _apply_stages(
-        self, ctx: Context, obs: TensorDictBase, new: TensorDictBase
-    ) -> Tuple[TensorDictBase, TensorDictBase]:
         obs_candidates = obs.get_sub_tensordict(obs.get(KEY_ACTIVE))
         for stage in self.stages:
             obs_candidates, new = stage(ctx, obs_candidates, new)
 
         if len(obs_candidates) > 0 and obs_candidates.batch_size[0] > 0:
             obs_candidates.fill_(KEY_ACTIVE, False)
```

### Comparing `unitrack-4.5.0/sources/unitrack.egg-info/SOURCES.txt` & `unitrack-4.6.9/sources/unitrack.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 sources/unitrack/__init__.py
 sources/unitrack/constants.py
-sources/unitrack/context.py
 sources/unitrack/memory.py
 sources/unitrack/tracker.py
 sources/unitrack.egg-info/PKG-INFO
 sources/unitrack.egg-info/SOURCES.txt
 sources/unitrack.egg-info/dependency_links.txt
 sources/unitrack.egg-info/requires.txt
 sources/unitrack.egg-info/top_level.txt
@@ -19,17 +18,14 @@
 sources/unitrack/assignment/jonker.py
 sources/unitrack/costs/__init__.py
 sources/unitrack/costs/base_cost.py
 sources/unitrack/costs/category.py
 sources/unitrack/costs/iou.py
 sources/unitrack/costs/reduce.py
 sources/unitrack/costs/wrap.py
-sources/unitrack/fields/__init__.py
-sources/unitrack/fields/base_field.py
-sources/unitrack/fields/value.py
 sources/unitrack/stages/__init__.py
 sources/unitrack/stages/association.py
 sources/unitrack/stages/base_stage.py
 sources/unitrack/stages/lost.py
 sources/unitrack/states/__init__.py
 sources/unitrack/states/base_state.py
 sources/unitrack/states/value.py
```

