# Comparing `tmp/ecgai_drawing-0.1.13.tar.gz` & `tmp/ecgai_drawing-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecgai_drawing-0.1.13.tar", max compression
+gzip compressed data, was "ecgai_drawing-0.1.14.tar", max compression
```

## Comparing `ecgai_drawing-0.1.13.tar` & `ecgai_drawing-0.1.14.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0      993 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/pyproject.toml
--rw-r--r--   0        0        0       78 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/__init__.py
--rw-r--r--   0        0        0     5709 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/create_ecg_plot.py
--rw-r--r--   0        0        0      988 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plot_image.py
--rw-r--r--   0        0        0    11995 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plotter.py
--rw-r--r--   0        0        0        0 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/__init__.py
--rw-r--r--   0        0        0      178 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/artifact.py
--rw-r--r--   0        0        0      481 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/color_style.py
--rw-r--r--   0        0        0      563 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/ecg_lead_name.py
--rw-r--r--   0        0        0      676 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/enum_ordered_base.py
--rw-r--r--   0        0        0      105 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/enums/show_grid.py
--rw-r--r--   0        0        0     8622 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/images.py
--rw-r--r--   0        0        0        0 2023-05-06 16:19:51.225548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/__init__.py
--rw-r--r--   0        0        0      812 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_lead.py
--rw-r--r--   0        0        0      647 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_leads.py
--rw-r--r--   0        0        0      851 2023-05-06 16:19:51.229548 ecgai_drawing-0.1.13/src/ecgai_drawing/models/model_base.py
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 ecgai_drawing-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0     1010 2023-05-22 20:24:04.828234 ecgai_drawing-0.1.14/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/__init__.py
+-rw-r--r--   0        0        0     5709 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/create_ecg_plot.py
+-rw-r--r--   0        0        0     5993 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_grid_plotter.py
+-rw-r--r--   0        0        0      988 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plot_image.py
+-rw-r--r--   0        0        0    13186 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plotter.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/artifact.py
+-rw-r--r--   0        0        0      481 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/color_style.py
+-rw-r--r--   0        0        0      563 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/ecg_lead_name.py
+-rw-r--r--   0        0        0      676 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/enum_ordered_base.py
+-rw-r--r--   0        0        0      105 2023-05-22 20:24:04.832234 ecgai_drawing-0.1.14/src/ecgai_drawing/enums/show_grid.py
+-rw-r--r--   0        0        0  1010336 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/bw_six_x_two.png
+-rw-r--r--   0        0        0   862301 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/grid_images/colour_six_x_two.png
+-rw-r--r--   0        0        0    11934 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/images.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_lead.py
+-rw-r--r--   0        0        0      647 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_leads.py
+-rw-r--r--   0        0        0      851 2023-05-22 20:24:04.836234 ecgai_drawing-0.1.14/src/ecgai_drawing/models/model_base.py
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 ecgai_drawing-0.1.14/PKG-INFO
```

### Comparing `ecgai_drawing-0.1.13/pyproject.toml` & `ecgai_drawing-0.1.14/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "ecgai-drawing"
-version = "0.1.13"
+version = "0.1.14"
 description = ""
 authors = ["RobC <rob.clapham@gmail.com>"]
 
 [tool.poetry.dependencies]
 #TODO change poetry version to <4.0, currently required by scipy
 python = "^3.9,<3.12"
 numpy = "^1.23.2"
 aenum = "^3.1.11"
 pydantic = "^1.9.2"
 matplotlib = "^3.5.3"
 scikit-image = "^0.19.3"
 scipy = "^1.9.0"
 opencv-python = "^4.6.0"
+timer = "^0.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pre-commit = "^2.20.0"
 pylint = "^2.14.5"
 coverage = "^6.4.4"
 #tox-poetry-installer = {extras = ["poetry"], version = "^0.8.4"}
```

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/create_ecg_plot.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/create_ecg_plot.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plot_image.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plot_image.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/ecg_plotter.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/ecg_plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import pathlib
 from math import ceil
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.axes import Subplot
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 from matplotlib.figure import Figure
 from matplotlib.ticker import AutoMinorLocator
 from numpy import ndarray
 from pydantic.dataclasses import dataclass
 
+# from definitions import ROOT_DIR
 from ecgai_drawing import images
 from ecgai_drawing.enums.color_style import ColorStyle
+from ecgai_drawing.images import combine_images, load_image
 from ecgai_drawing.models.ecg_leads import Leads
 
 # from skimage.COLOR import rgba2rgb
 
 
 @dataclass
 class EcgPlotter:
@@ -35,15 +38,15 @@
         "V5",
         "V6",
     ]
     lead_order: list = None
     sample_rate: int = 500
     title: str = "ECG 12 lead"
     color_style: ColorStyle = ColorStyle.COLOR
-    line_width: float = 0.5
+    line_width: float = 1.0
     columns: int = 2
     row_height: int = 6
     show_lead_name: bool = True
     show_grid: bool = False
     show_separate_line: bool = True
     adjust_subplots: bool = True
 
@@ -69,21 +72,28 @@
             ndarray:
 
         """
         self.sample_rate = sample_rate
         self.title = title
         self._set_style(color_style, show_grid)
         image = self._create_plot(ecg_leads)
-
         # convert from rgba format to rgb format
         image = images.convert_from_rgba_to_rgb(image=image)
-
         # convert from rgb format to bgr format required by openCv
         image = images.convert_from_rgb_to_bgr(image=image)
 
+        if self.show_grid:
+            # consider using different grid image based on the configuration of the Ecg plot
+            base_image = load_image(image_name="colour_six_x_two.png", image_path=data_directory())
+        else:
+            base_image = np.zeros([768, 2048, 3], dtype=np.uint8)
+            base_image.fill(255)
+            # if self.color_style == ColorStyle.COLOR:
+        image = combine_images(base_image=base_image, top_image=image)
+
         return image
 
     def _draw_plot(self, ecg_leads: Leads):
         leads = self._convert_to_ndarray(ecg_leads=ecg_leads)
 
         if not self.lead_order:
             self.lead_order = list(range(len(leads)))
@@ -102,24 +112,25 @@
         subplot = self._setup_subplot(figure, x_max, x_min, y_max, y_min)
 
         display_factor **= 0.5
 
         color_line, color_major_grid, color_minor_grid = self._set_line_style()
 
         if self.show_grid:
-            self._draw_grid(
-                subplot=subplot,
-                color_major_grid=color_major_grid,
-                color_minor_grid=color_minor_grid,
-                display_factor=display_factor,
-                x_max=x_max,
-                x_min=x_min,
-                y_max=y_max,
-                y_min=y_min,
-            )
+            pass
+            # self._draw_grid(
+            #     subplot=subplot,
+            #     color_major_grid=color_major_grid,
+            #     color_minor_grid=color_minor_grid,
+            #     display_factor=display_factor,
+            #     x_max=x_max,
+            #     x_min=x_min,
+            #     y_max=y_max,
+            #     y_min=y_min,
+            # )
 
         self._draw_plot_leads(
             subplot=subplot,
             color_line=color_line,
             display_factor=display_factor,
             leads=leads,
             length_seconds=length_seconds,
@@ -192,14 +203,15 @@
         subplot.spines["top"].set_visible(False)
         subplot.spines["right"].set_visible(False)
         subplot.spines["bottom"].set_visible(False)
         subplot.spines["left"].set_visible(False)
         return subplot
 
     def _setup_figure(self, display_factor: float, rows: int, length_seconds: float) -> Figure:
+
         figure = plt.figure(
             figsize=(
                 length_seconds * self.columns * display_factor,
                 rows * self.row_height / 5 * display_factor,
             )
         )
         figure.subplots_adjust(
@@ -221,15 +233,15 @@
 
     def _set_line_style(
         self,
     ) -> tuple[tuple[float, float, float], tuple[float, float, float], tuple[float, float, float]]:
         if self.color_style == ColorStyle.COLOR:
             color_major_grid = (1, 0, 0)
             color_minor_grid = (1, 0.7, 0.7)
-            color_line = (0, 0, 0.7)
+            color_line = (0, 0, 0)
         elif self.color_style in [
             ColorStyle.BLACK_AND_WHITE,
             ColorStyle.GREY_SCALE,
             ColorStyle.MASK,
         ]:
             color_major_grid = (0.4, 0.4, 0.4)
             color_minor_grid = (0.75, 0.75, 0.75)
@@ -297,20 +309,33 @@
             which="minor",
             linestyle="-",
             linewidth=0.5 * display_factor,
             color=color_minor_grid,
         )
 
     def _create_plot(self, ecg_leads):
+
         plt.ioff()
+        # plot_start = time.time()
+
         self._draw_plot(ecg_leads=ecg_leads)
+        # plot_finish = time.time()
+        # plot_execution_time = plot_finish - plot_start
+        # print(f"Plotting took {plot_execution_time:.6f} seconds")
         canvas = plt.get_current_fig_manager().canvas
+
         plt.close()
+        # agg=canvas
         agg = canvas.switch_backends(FigureCanvasAgg)
+
+        # draw_start = time.time()
         agg.draw()
+        # draw_finish = time.time()
+        # draw_execution_time = draw_finish - draw_start
+        # print(f"Drawing took {draw_execution_time:.6f} seconds")
         return np.asarray(agg.buffer_rgba())
 
     # @staticmethod
     # def _convert_to_mask(image: ndarray) -> ndarray:
     #     return images.convert_to_mask(image)
 
     def _set_style(self, color_style: ColorStyle, show_grid: bool):
@@ -349,7 +374,13 @@
     #     output_array = np.zeros(shape=[number_of_leads, number_of_signals])
     #     for array_position, lead in enumerate(ecg_leads.leads):
     #         sig = [v.voltage for v in lead.signals]
     #         # g = s.signals
     #         p_lead = np.array(sig)
     #         output_array[array_position] = p_lead
     #     return output_array
+
+
+def data_directory() -> pathlib.Path:
+    file_path = pathlib.Path(pathlib.Path(pathlib.Path(__file__).parent, "grid_images"))
+    print(file_path)
+    return file_path
```

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/enums/ecg_lead_name.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/enums/ecg_lead_name.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/enums/enum_ordered_base.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/enums/enum_ordered_base.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/images.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/images.py`

 * *Files 20% similar despite different names*

```diff
@@ -73,16 +73,101 @@
 
 def convert_from_base64_string(stream: str) -> ndarray:
     jpg_original = base64.b64decode(stream)
     jpg_as_np = np.frombuffer(jpg_original, dtype=np.uint8)
     img = cv2.imdecode(jpg_as_np, flags=1)
     return img
 
-    # image = base64.b64decode(stream)
-    # return convert_from_bytes(image)
+
+#
+# def combine_color_images(base_image: ndarray, top_image: ndarray) -> ndarray:
+#     rows, cols, channels = top_image.shape
+#     roi = base_image[0:rows, 0:cols]
+#
+#     top_image_gray = convert_to_grey_scale(top_image)
+#
+#     ret, mask = cv2.threshold(top_image_gray, 200, 255, cv2.THRESH_BINARY)
+#
+#     mask_inv = cv2.bitwise_not(mask)
+#
+#     img_back = cv2.bitwise_and(roi, roi, mask=mask)
+#
+#     top_image_colour = cv2.bitwise_and(top_image, top_image, mask=mask_inv)
+#     # return top_image_colour
+#     img_out = cv2.add(img_back, top_image_colour)
+#     base_image[0:rows, 0:cols] = img_out
+#     return base_image
+#
+#
+# def combine_grey_scale_images(base_image: ndarray, top_image: ndarray) -> ndarray:
+#     top_rows, top_cols, top_channels = top_image.shape
+#     base_rows, base_cols, base_channels = base_image.shape
+#
+#     start_row = int((base_rows - top_rows) / 2)
+#     start_col = int((base_cols - top_cols) / 2)
+#     white = [255, 255, 255]
+#     top_image_border = cv2.copyMakeBorder(top_image,
+#                                           start_row,
+#                                           start_row,
+#                                           start_col,
+#                                           start_col,
+#                                           cv2.BORDER_CONSTANT,
+#                                           value=white)
+#     border_rows, border_cols, border_channels = top_image_border.shape
+#
+#     roi = base_image[0:base_rows, 0:base_cols]
+#
+#     top_image_gray = convert_to_grey_scale(top_image_border)
+#     base_image_gray = convert_to_grey_scale(base_image)
+#     ret, mask = cv2.threshold(top_image_gray, 200, 255, cv2.THRESH_BINARY)
+#
+#     mask_inv = cv2.bitwise_not(mask)
+#
+#     img_back = cv2.bitwise_and(roi, roi, mask=mask)
+#
+#     top_image_colour = cv2.bitwise_and(top_image_border, top_image_border, mask=mask_inv)
+#     # return top_image_colour
+#     # top_image_out = convert_to_grey_scale(top_image_colour)
+#     img_out = cv2.add(img_back, top_image_colour)
+#     base_image[0:border_rows, 0:border_cols] = img_out
+#     return base_image
+
+
+def combine_images(base_image: ndarray, top_image: ndarray) -> ndarray:
+    top_rows, top_cols, top_channels = top_image.shape
+    base_rows, base_cols, base_channels = base_image.shape
+
+    start_row = int((base_rows - top_rows) / 2)
+    start_col = int((base_cols - top_cols) / 2)
+
+    if start_row < 0 or start_col < 0:
+        raise ValueError("Top image is too big for base image")
+
+    white = [255, 255, 255]
+    top_image_border = cv2.copyMakeBorder(
+        top_image, start_row, start_row, start_col, start_col, cv2.BORDER_CONSTANT, value=white
+    )
+    border_rows, border_cols, border_channels = top_image_border.shape
+
+    roi = base_image[0:base_rows, 0:base_cols]
+
+    top_image_gray = convert_to_grey_scale(top_image_border)
+    # base_image_gray = convert_to_grey_scale(base_image)
+    ret, mask = cv2.threshold(top_image_gray, 200, 255, cv2.THRESH_BINARY)
+
+    mask_inv = cv2.bitwise_not(mask)
+
+    img_back = cv2.bitwise_and(roi, roi, mask=mask)
+
+    top_image_colour = cv2.bitwise_and(top_image_border, top_image_border, mask=mask_inv)
+    # return top_image_colour
+    # top_image_out = convert_to_grey_scale(top_image_colour)
+    img_out = cv2.add(img_back, top_image_colour)
+    base_image[0:border_rows, 0:border_cols] = img_out
+    return base_image
 
 
 # def create_binary_image(COLOR_WITHOUT_GRID_NAME: str, image_path: str) -> ndarray:
 #     image = load_image(COLOR_WITHOUT_GRID_NAME=COLOR_WITHOUT_GRID_NAME, image_path=image_path, as_gray=True)
 #     thresh = threshold_isodata(image)
 #     return image > thresh
```

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_lead.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_lead.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/models/ecg_leads.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/models/ecg_leads.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/src/ecgai_drawing/models/model_base.py` & `ecgai_drawing-0.1.14/src/ecgai_drawing/models/model_base.py`

 * *Files identical despite different names*

### Comparing `ecgai_drawing-0.1.13/PKG-INFO` & `ecgai_drawing-0.1.14/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecgai-drawing
-Version: 0.1.13
+Version: 0.1.14
 Summary: 
 Author: RobC
 Author-email: rob.clapham@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,7 +12,8 @@
 Requires-Dist: aenum (>=3.1.11,<4.0.0)
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.6.0,<5.0.0)
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Requires-Dist: timer (>=0.2.2,<0.3.0)
```

