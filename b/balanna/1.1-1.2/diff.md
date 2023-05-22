# Comparing `tmp/balanna-1.1.tar.gz` & `tmp/balanna-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balanna-1.1.tar", last modified: Mon May  8 08:49:05 2023, max compression
+gzip compressed data, was "balanna-1.2.tar", last modified: Mon May 22 11:06:40 2023, max compression
```

## Comparing `balanna-1.1.tar` & `balanna-1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.015508 balanna-1.1/
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-08 07:14:59.000000 balanna-1.1/LICENSE
--rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-08 08:49:05.015508 balanna-1.1/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-08 07:14:59.000000 balanna-1.1/README.md
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:04.999507 balanna-1.1/balanna/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-08 08:42:52.000000 balanna-1.1/balanna/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-08 07:14:59.000000 balanna-1.1/balanna/__main__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-08 07:14:59.000000 balanna-1.1/balanna/camera_trajectories.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     2013 2023-05-08 08:42:52.000000 balanna-1.1/balanna/rendering_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-08 07:14:59.000000 balanna-1.1/balanna/trimesh.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.011508 balanna-1.1/balanna/utils/
--rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-08 07:14:59.000000 balanna-1.1/balanna/utils/__init__.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-08 07:14:59.000000 balanna-1.1/balanna/utils/geometry.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-08 08:42:52.000000 balanna-1.1/balanna/utils/vedo_utils.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)    10610 2023-05-08 08:42:52.000000 balanna-1.1/balanna/window_base.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4645 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_dataset.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     4593 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_generator.py
--rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-08 07:14:59.000000 balanna-1.1/balanna/window_real_time.py
-drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-08 08:49:05.007508 balanna-1.1/balanna.egg-info/
--rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/PKG-INFO
--rw-r--r--   0 sas      (23222) tumuser  (20909)      494 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/SOURCES.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/dependency_links.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/requires.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-08 08:49:04.000000 balanna-1.1/balanna.egg-info/top_level.txt
--rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-08 08:49:05.015508 balanna-1.1/setup.cfg
--rw-r--r--   0 sas      (23222) tumuser  (20909)      493 2023-05-08 08:43:23.000000 balanna-1.1/setup.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.295783 balanna-1.2/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1070 2023-05-22 07:50:24.000000 balanna-1.2/LICENSE
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-22 11:06:40.295783 balanna-1.2/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-22 07:50:24.000000 balanna-1.2/README.md
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.279783 balanna-1.2/balanna/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      613 2023-05-22 07:50:24.000000 balanna-1.2/balanna/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1095 2023-05-22 07:50:24.000000 balanna-1.2/balanna/__main__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     1581 2023-05-22 07:50:24.000000 balanna-1.2/balanna/camera_trajectories.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     2023 2023-05-22 07:54:36.000000 balanna-1.2/balanna/rendering_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    10078 2023-05-22 07:50:24.000000 balanna-1.2/balanna/trimesh.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.291783 balanna-1.2/balanna/utils/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       30 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/__init__.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      559 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/geometry.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      122 2023-05-22 09:14:27.000000 balanna-1.2/balanna/utils/types.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4463 2023-05-22 07:50:24.000000 balanna-1.2/balanna/utils/vedo_utils.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)    11208 2023-05-22 09:13:19.000000 balanna-1.2/balanna/window_base.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4618 2023-05-22 08:19:05.000000 balanna-1.2/balanna/window_dataset.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     4566 2023-05-22 08:19:32.000000 balanna-1.2/balanna/window_generator.py
+-rw-r--r--   0 sas      (23222) tumuser  (20909)     7265 2023-05-22 07:50:24.000000 balanna-1.2/balanna/window_real_time.py
+drwxr-xr-x   0 sas      (23222) tumuser  (20909)        0 2023-05-22 11:06:40.287783 balanna-1.2/balanna.egg-info/
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      245 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/PKG-INFO
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      517 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/SOURCES.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        1 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/dependency_links.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)       56 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/requires.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)        8 2023-05-22 11:06:40.000000 balanna-1.2/balanna.egg-info/top_level.txt
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      103 2023-05-22 11:06:40.295783 balanna-1.2/setup.cfg
+-rw-r--r--   0 sas      (23222) tumuser  (20909)      493 2023-05-22 11:06:34.000000 balanna-1.2/setup.py
```

### Comparing `balanna-1.1/LICENSE` & `balanna-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `balanna-1.1/README.md` & `balanna-1.2/README.md`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/__init__.py` & `balanna-1.2/balanna/__init__.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/__main__.py` & `balanna-1.2/balanna/__main__.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/camera_trajectories.py` & `balanna-1.2/balanna/camera_trajectories.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/rendering_dataset.py` & `balanna-1.2/balanna/rendering_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     show_labels: bool = False,
     use_scene_cam: bool = False,
     debug: bool = False
 ):
     """Render scenes stored in scene iterator to a numpy array (num_frames, H, W, 3).
 
     The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
-    Currently, only trimesh scenes are supported.
+    See SceneDictType for currently supported object types.
 
     Args:
         scenes: sorted list of scene dictionaries.
         show_labels: display the scene dict keys.
         use_scene_cam: use camera transform from trimesh scenes.
         debug: printing debug information.
     """
```

### Comparing `balanna-1.1/balanna/trimesh.py` & `balanna-1.2/balanna/trimesh.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/utils/geometry.py` & `balanna-1.2/balanna/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/utils/vedo_utils.py` & `balanna-1.2/balanna/utils/vedo_utils.py`

 * *Files identical despite different names*

### Comparing `balanna-1.1/balanna/window_base.py` & `balanna-1.2/balanna/window_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from PIL import Image
 from PyQt5 import Qt
 from typing import Any, Dict, List, Optional, Union
 from vtk.qt.QVTKRenderWindowInteractor import QVTKRenderWindowInteractor
 
 from balanna.utils.vedo_utils import trimesh_scene_2_vedo
 
-SceneDictType = Dict[str, Any]
+SceneDictType = Dict[str, Union[trimesh.Scene, Axes, str, np.ndarray, vedo.Volume]]
 
 
 class MainWindow(Qt.QMainWindow):
 
     def __init__(
         self,
         image_keys: List[str],
@@ -119,23 +119,21 @@
                 print("\033[93m" + "Video directory already exists, overwriting it ..." + "\033[0m")
             self.video_directory.mkdir(exist_ok=True, parents=True)
 
     def render_(self, scene_dict: SceneDictType, resetcam: bool = False):
         start_time = time.perf_counter()
 
         for key, element in scene_dict.items():
-            if isinstance(element, trimesh.Scene) and key in self.scene_key_dict:
-                at = self.scene_key_dict[key]
+            if isinstance(element, trimesh.Scene):
                 meshes_vedo, camera_dict = trimesh_scene_2_vedo(
                     scene=element,
                     label=key if self.show_labels else None,
                     use_scene_cam=self.use_scene_cam
                 )
-                self.vps[at].clear()
-                self.vps[at].show(meshes_vedo, bg="white", resetcam=resetcam, camera=camera_dict)
+                self.render_scene_at_key_(key, meshes_vedo, resetcam=resetcam, camera_dict=camera_dict)
 
             elif isinstance(element, np.ndarray) and key in self.image_widge_dict:
                 if len(element.shape) == 3:
                     if element.shape[0] == 3:
                         element = np.transpose(element, (1, 2, 0))  # (C, H, W) -> (H, W, C)
                 else:
                     element = np.stack([element] * 3, axis=-1)
@@ -154,26 +152,44 @@
                 self.figureCanvas[at].figure.clf()
                 # set new references of axes element
                 element.figure = self.figureCanvas[at].figure
                 self.figureCanvas[at].figure.add_axes(element)
                 # draw figure to update!
                 self.figureCanvas[at].draw()
 
+            elif isinstance(element, vedo.Volume):
+                self.render_scene_at_key_(key, [element], resetcam=resetcam)
+
             else:
                 print("\033[93m" + f"Invalid element in scene dict of type {type(element)}, skipping ..." + "\033[0m")
                 continue
 
         if self.debug:
             dt = int((time.perf_counter() - start_time) * 1000)  # secs -> milliseconds
             print("\033[36m" + f"Rendering time: {dt} ms" + "\033[0m")
 
         if self.video_directory is not None:
             self.screenshot(self.video_directory, prefix=f"{self.__video_index:05d}")
             self.__video_index += 1
 
+    def render_scene_at_key_(
+        self,
+        key: str,
+        meshes: List[Union[vedo.Mesh, vedo.Volume]],
+        resetcam: bool = False,
+        camera_dict: Optional[Dict[str, np.ndarray]] = None
+    ):
+        if key not in self.scene_key_dict:
+            print("\033[93m" + f"Key {key} not in scene key dicts, skipping ..." + "\033[0m")
+            return
+
+        at = self.scene_key_dict[key]
+        self.vps[at].clear()
+        self.vps[at].show(meshes, bg="white", resetcam=resetcam, camera=camera_dict)
+
     def __align_event(self, event=None, align_id: int = None):  # noqa
         if self.num_scenes < 2:
             return
         if align_id is None:
             align_id = self._current_align_id
 
         camera = self.vps[align_id].camera
```

### Comparing `balanna-1.1/balanna/window_dataset.py` & `balanna-1.2/balanna/window_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import pathlib
-import trimesh
 
 from matplotlib.axes import Axes
 from PyQt5 import Qt
 from typing import List, Optional, Union
 
 from .window_base import MainWindow, SceneDictType
+from .utils.types import contains_scene
 
 
 __all__ = ['display_dataset']
 
 
 class MainWindowDataset(MainWindow):
 
@@ -30,15 +30,15 @@
         self.fps = fps
         if len(scenes) == 0:
             return
         self.__frame_idx = 0
         scene_dict = self.scenes[0]
 
         image_keys = [key for key, value in scene_dict.items() if isinstance(value, np.ndarray)]
-        scene_keys = [key for key, value in scene_dict.items() if isinstance(value, trimesh.Scene)]
+        scene_keys = [key for key, value in scene_dict.items() if contains_scene(value)]
         figure_keys = [key for key, value in scene_dict.items() if isinstance(value, Axes)]
         super(MainWindowDataset, self).__init__(
             image_keys=image_keys,
             scene_keys=scene_keys,
             figure_keys=figure_keys,
             video_directory=video_directory,
             horizontal=horizontal,
@@ -106,15 +106,15 @@
     show_labels: bool = False,
     use_scene_cam: bool = False,
     debug: bool = False
 ):
     """Display scenes stored in scene iterator as PyQt app.
 
     The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
-    Currently, images (np.array), 3D scenes (trimesh.Scene) and strings (for prinout) are supported.
+    See SceneDictType for currently supported object types.
 
     Args:
         scenes: sorted list of scene dictionaries.
         horizontal: window orientation, horizontal or vertical stacking.
         loop: start looping from beginning.
         fps: frames (i.e. scenes) per second for looping.
         video_directory: directory for storing screenshots.
```

### Comparing `balanna-1.1/balanna/window_generator.py` & `balanna-1.2/balanna/window_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import pathlib
-import trimesh
 
 from matplotlib.axes import Axes
 from PyQt5 import Qt
 from typing import Iterable, Optional, Union
 
 from .window_base import MainWindow, SceneDictType
+from .utils.types import contains_scene
 
 
 __all__ = ['display_scenes', 'display_generated']
 
 
 class MainWindowGenerator(MainWindow):
 
@@ -29,15 +29,15 @@
         self.scene_iterator = scene_iterator
         self.fps = fps
         scene_dict = self.get_next_scene_dict()
         if scene_dict is None:
             return
 
         image_keys = [key for key, value in scene_dict.items() if isinstance(value, np.ndarray)]
-        scene_keys = [key for key, value in scene_dict.items() if isinstance(value, trimesh.Scene)]
+        scene_keys = [key for key, value in scene_dict.items() if contains_scene(value)]
         figure_keys = [key for key, value in scene_dict.items() if isinstance(value, Axes)]
         super(MainWindowGenerator, self).__init__(
             image_keys=image_keys,
             scene_keys=scene_keys,
             figure_keys=figure_keys,
             video_directory=video_directory,
             horizontal=horizontal,
@@ -99,15 +99,15 @@
     show_labels: bool = False,
     use_scene_cam: bool = False,
     debug: bool = False
 ):
     """Display scenes stored in scene iterator as PyQt app.
 
     The scene iterator yields a dictionary that describes the elements of the scene, one dictionary per frame.
-    Currently, images (np.array), 3D scenes (trimesh.Scene) and strings (for prinout) are supported.
+    See SceneDictType for currently supported object types.
 
     Args:
         scene_iterator: iterator function to get the scene dictionaries.
         horizontal: window orientation, horizontal or vertical stacking.
         loop: start looping from beginning.
         fps: frames (i.e. scenes) per second for looping.
         video_directory: directory for storing screenshots.
```

### Comparing `balanna-1.1/balanna/window_real_time.py` & `balanna-1.2/balanna/window_real_time.py`

 * *Files identical despite different names*

