# Comparing `tmp/onnx2kerastl-0.0.93.tar.gz` & `tmp/onnx2kerastl-0.0.94.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.93.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.94.dev1.tar", max compression
```

## Comparing `onnx2kerastl-0.0.93.tar` & `onnx2kerastl-0.0.94.dev1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.93/LICENSE
--rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.93/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.93/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.93/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.93/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.93/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.93/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      697 2023-05-16 16:00:58.651041 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0     4950 2023-05-17 13:31:53.385365 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxgridsampler.py
--rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.93/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.93/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.93/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.93/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.93/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.93/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.93/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.93/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.93/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.93/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.93/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     4965 2023-05-16 15:44:21.797652 onnx2kerastl-0.0.93/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.93/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.93/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-17 13:32:39.118919 onnx2kerastl-0.0.93/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.94.dev1/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.94.dev1/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.94.dev1/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.94.dev1/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.94.dev1/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.94.dev1/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.94.dev1/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-21 12:41:16.202993 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.94.dev1/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.94.dev1/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.94.dev1/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.94.dev1/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.94.dev1/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.94.dev1/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.94.dev1/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.94.dev1/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.94.dev1/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.94.dev1/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.94.dev1/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5011 2023-05-22 12:41:21.229261 onnx2kerastl-0.0.94.dev1/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.94.dev1/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.94.dev1/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1035 2023-05-22 13:22:13.621961 onnx2kerastl-0.0.94.dev1/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.94.dev1/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.93/LICENSE` & `onnx2kerastl-0.0.94.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from onnx2kerastl.customonnxlayer.onnxhardsigmoid import OnnxHardSigmoid
 from onnx2kerastl.customonnxlayer.onnxsqrt import OnnxSqrt
 from onnx2kerastl.customonnxlayer.onnxreducemean import OnnxReduceMean
 from onnx2kerastl.customonnxlayer.onnxerf import OnnxErf
 from onnx2kerastl.customonnxlayer.onnxabs import OnnxAbs
 from onnx2kerastl.customonnxlayer.onnxlstm import OnnxLSTM
-from onnx2kerastl.customonnxlayer.onnxgridsampler import OnnxGridSampler
 
 onnx_custom_objects_map = {
     "OnnxHardSigmoid": OnnxHardSigmoid,
     "OnnxSqrt": OnnxSqrt,
     "OnnxReduceMean": OnnxReduceMean,
     "OnnxAbs": OnnxAbs,
     "OnnxErf": OnnxErf,
-    "OnnxGridSampler": OnnxGridSampler,
     "OnnxLSTM": OnnxLSTM
 }
```

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxgridsampler.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/sampling_layers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,115 @@
-from typing import List
-
-from keras.layers import Layer
+import keras
 import tensorflow as tf
 
 
-class OnnxGridSampler(Layer):
+def convert_range(node, params, layers, lambda_func, node_name, keras_name):
+    start_range = layers[node.input[0]]
+    limit_range = layers[node.input[1]]
+    delta_range = layers[node.input[2]]
+    layers[node_name] = tf.range(start_range, limit_range, delta_range)
+
+
+def convert_gridsample(node, params, layers, lambda_func, node_name, keras_name):
     """
-Args:
-    sample_grid: tuple
-    **kwargs:
-"""
-    def __init__(self, sample_grid: List[int], **kwargs):
-        super().__init__(**kwargs)
-        self.sample_grid = sample_grid
-
-    def get_config(self):
-        config = super().get_config()
-        config.update({
-            "sample_grid": self.sample_grid
-        })
-        return config
-
-    def call(self, inputs, **kwargs):
-        torch_shape = tf.shape(inputs)
-        max_xy = tf.expand_dims(
-            tf.expand_dims(tf.expand_dims(tf.convert_to_tensor([torch_shape[3] - 1, torch_shape[2] - 1]), 0), 0), 0)
-        max_xy = tf.cast(max_xy, tf.float32)
-        grid_index_coords = 0.5 * (self.sample_grid + 1.) * max_xy  # transform from [-1,1] to [0,H-1]/[0,W-1]
-        result = self.interpolate_wrapper(inputs, grid_index_coords, torch_shape)
-        return result
-
-    @staticmethod
-    def interpolate_wrapper(torch_img, grid_index_coords, torch_shape) -> tf.Tensor:
-        """tf.function implementation of interpolate_bilinear."""
-        grid_index_coords = grid_index_coords + 1  # fix locs considering we add padding
-        orig_query_shape = tf.shape(grid_index_coords)
-        query_points = tf.reshape(grid_index_coords, [orig_query_shape[0], -1, 2])
-        padded_img = tf.keras.layers.ZeroPadding2D(padding=(1, 1), data_format="channels_first")(torch_img)
-        grid = tf.keras.layers.Permute((2, 3, 1))(padded_img)
-        indexing = 'ji'
-        grid_shape = tf.shape(grid)
-        query_shape = tf.shape(query_points)
-        batch_size, height, width, channels = (
-            grid_shape[0],
-            grid_shape[1],
-            grid_shape[2],
-            grid_shape[3],
+    Convert gridsample.
+    :param node: current operation node
+    :param params: operation attributes
+    :param layers: available keras layers
+    :param lambda_func: function for keras Lambda layer
+    :param node_name: internal converter name
+    :param keras_name: resulting layer name
+    :return: None
+    """
+    assert params['mode'].decode('ascii') == 'bilinear'
+    assert params['padding_mode'].decode('ascii') == 'zeros'
+    assert params['align_corners'] == 1
+    params['mode'] = params['mode'].decode('ascii')
+    params['padding_mode'] = params['padding_mode'].decode('ascii')
+    img = layers[node.input[0]]
+    sample_grid = layers[node.input[1]]
+    torch_shape = tf.shape(img)
+    max_xy = tf.expand_dims(
+        tf.expand_dims(tf.expand_dims(tf.convert_to_tensor([torch_shape[3] - 1, torch_shape[2] - 1]), 0), 0), 0)
+    max_xy = tf.cast(max_xy, tf.float32)
+    grid_index_coords = 0.5 * (sample_grid + 1.) * max_xy  # transform from [-1,1] to [0,H-1]/[0,W-1]
+    grid_index_coords = grid_index_coords + 1  # fix locs considering we add padding
+    orig_query_shape = tf.shape(grid_index_coords)
+    query_points = tf.reshape(grid_index_coords, [orig_query_shape[0], -1, 2])
+    padded_img = tf.keras.layers.ZeroPadding2D(padding=(1, 1), data_format="channels_first")(img)
+    grid = tf.keras.layers.Permute((2, 3, 1))(padded_img)
+    indexing = 'ji'
+    grid_shape = tf.shape(grid)
+    query_shape = tf.shape(query_points)
+    batch_size, height, width, channels = (
+        grid_shape[0],
+        grid_shape[1],
+        grid_shape[2],
+        grid_shape[3],
+    )
+    num_queries = query_shape[1]
+
+    query_type = query_points.dtype
+    grid_type = grid.dtype
+
+    alphas = []
+    floors = []
+    ceils = []
+    index_order = [0, 1] if indexing == "ij" else [1, 0]
+    # unstacked_query_points = tf.unstack(query_points, axis=2, num=2)
+
+    for i, dim in enumerate(index_order):
+        queries = query_points[:, :, dim, ...]
+        # queries = unstacked_query_points[dim]
+
+        size_in_indexing_dimension = grid_shape[i + 1]
+
+        # max_floor is size_in_indexing_dimension - 2 so that max_floor + 1
+        # is still a valid index into the grid.
+        max_floor = tf.cast(size_in_indexing_dimension - 2, query_type)
+        min_floor = tf.constant(0.0, dtype=query_type)
+        floor = tf.math.minimum(
+            tf.math.maximum(min_floor, tf.math.floor(queries)), max_floor
+        )
+        int_floor = tf.cast(floor, tf.dtypes.int32)
+        floors.append(int_floor)
+        ceil = int_floor + 1
+        ceils.append(ceil)
+
+        # alpha has the same type as the grid, as we will directly use alpha
+        # when taking linear combinations of pixel values from the image.
+        alpha = tf.cast(queries - floor, grid_type)
+        min_alpha = tf.constant(0.0, dtype=grid_type)
+        max_alpha = tf.constant(1.0, dtype=grid_type)
+        alpha = tf.math.minimum(tf.math.maximum(min_alpha, alpha), max_alpha)
+
+        # Expand alpha to [b, n, 1] so we can use broadcasting
+        # (since the alpha values don't depend on the channel).
+        alpha = tf.expand_dims(alpha, 2)
+        alphas.append(alpha)
+
+        flattened_grid = tf.reshape(grid, [batch_size * height * width, channels])
+        batch_offsets = tf.reshape(
+            tf.range(batch_size) * height * width, [batch_size, 1]
         )
-        num_queries = query_shape[1]
-
-        query_type = query_points.dtype
-        grid_type = grid.dtype
 
-        alphas = []
-        floors = []
-        ceils = []
-        index_order = [0, 1] if indexing == "ij" else [1, 0]
-        unstacked_query_points = tf.unstack(query_points, axis=2, num=2)
-
-        for i, dim in enumerate(index_order):
-            queries = unstacked_query_points[dim]
-
-            size_in_indexing_dimension = grid_shape[i + 1]
-
-            # max_floor is size_in_indexing_dimension - 2 so that max_floor + 1
-            # is still a valid index into the grid.
-            max_floor = tf.cast(size_in_indexing_dimension - 2, query_type)
-            min_floor = tf.constant(0.0, dtype=query_type)
-            floor = tf.math.minimum(
-                tf.math.maximum(min_floor, tf.math.floor(queries)), max_floor
-            )
-            int_floor = tf.cast(floor, tf.dtypes.int32)
-            floors.append(int_floor)
-            ceil = int_floor + 1
-            ceils.append(ceil)
-
-            # alpha has the same type as the grid, as we will directly use alpha
-            # when taking linear combinations of pixel values from the image.
-            alpha = tf.cast(queries - floor, grid_type)
-            min_alpha = tf.constant(0.0, dtype=grid_type)
-            max_alpha = tf.constant(1.0, dtype=grid_type)
-            alpha = tf.math.minimum(tf.math.maximum(min_alpha, alpha), max_alpha)
-
-            # Expand alpha to [b, n, 1] so we can use broadcasting
-            # (since the alpha values don't depend on the channel).
-            alpha = tf.expand_dims(alpha, 2)
-            alphas.append(alpha)
-
-            flattened_grid = tf.reshape(grid, [batch_size * height * width, channels])
-            batch_offsets = tf.reshape(
-                tf.range(batch_size) * height * width, [batch_size, 1]
-            )
-
-        # This wraps tf.gather. We reshape the image data such that the
-        # batch, y, and x coordinates are pulled into the first dimension.
-        # Then we gather. Finally, we reshape the output back. It's possible this
-        # code would be made simpler by using tf.gather_nd.
-        def gather(y_coords, x_coords, name=None):
-            linear_coordinates = batch_offsets + y_coords * width + x_coords
-            gathered_values = tf.gather(flattened_grid, linear_coordinates)
-            return tf.reshape(gathered_values, [batch_size, num_queries, channels])
-
-        # grab the pixel values in the 4 corners around each query point
-        top_left = gather(floors[0], floors[1], "top_left")
-        top_right = gather(floors[0], ceils[1], "top_right")
-        bottom_left = gather(ceils[0], floors[1], "bottom_left")
-        bottom_right = gather(ceils[0], ceils[1], "bottom_right")
-
-        interp_top = alphas[1] * (top_right - top_left) + top_left
-        interp_bottom = alphas[1] * (bottom_right - bottom_left) + bottom_left
-        interp = alphas[0] * (interp_bottom - interp_top) + interp_top
-        tf_reshaped_results = tf.reshape(interp, tf.concat([orig_query_shape[:-1], torch_shape[1:2]], axis=0))
-        return tf.keras.layers.Permute((3, 1, 2))(tf_reshaped_results)
+    # This wraps tf.gather. We reshape the image data such that the
+    # batch, y, and x coordinates are pulled into the first dimension.
+    # Then we gather. Finally, we reshape the output back. It's possible this
+    # code would be made simpler by using tf.gather_nd.
+    def gather(y_coords, x_coords, name=None):
+        linear_coordinates = batch_offsets + y_coords * width + x_coords
+        gathered_values = tf.gather(flattened_grid, linear_coordinates)
+        return tf.reshape(gathered_values, [batch_size, num_queries, channels])
+
+    # grab the pixel values in the 4 corners around each query point
+    top_left = gather(floors[0], floors[1], "top_left")
+    top_right = gather(floors[0], ceils[1], "top_right")
+    bottom_left = gather(ceils[0], floors[1], "bottom_left")
+    bottom_right = gather(ceils[0], ceils[1], "bottom_right")
+
+    interp_top = alphas[1] * (top_right - top_left) + top_left
+    interp_bottom = alphas[1] * (bottom_right - bottom_left) + bottom_left
+    interp = alphas[0] * (interp_bottom - interp_top) + interp_top
+    tf_reshaped_results = tf.reshape(interp, tf.concat([orig_query_shape[:-1], torch_shape[1:2]], axis=0))
+    ret = tf.keras.layers.Permute((3, 1, 2))(tf_reshaped_results)
+    layers[node_name] = ret
```

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.94.dev1/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.93/pyproject.toml` & `onnx2kerastl-0.0.94.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.93"
+version = "0.0.94.dev1"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.93/PKG-INFO` & `onnx2kerastl-0.0.94.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.93
+Version: 0.0.94.dev1
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

