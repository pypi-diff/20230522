# Comparing `tmp/lognflow-0.7.0.tar.gz` & `tmp/lognflow-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.0.tar", last modified: Mon May 15 01:23:53 2023, max compression
+gzip compressed data, was "lognflow-0.7.1.tar", last modified: Mon May 22 04:55:54 2023, max compression
```

## Comparing `lognflow-0.7.0.tar` & `lognflow-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.990351 lognflow-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 01:23:31.000000 lognflow-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 01:23:31.000000 lognflow-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-15 01:23:31.000000 lognflow-0.7.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 01:23:31.000000 lognflow-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 01:23:31.000000 lognflow-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-15 01:23:53.990351 lognflow-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-15 01:23:31.000000 lognflow-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 01:23:31.000000 lognflow-0.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70856 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-15 01:23:31.000000 lognflow-0.7.0/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 01:23:53.000000 lognflow-0.7.0/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-15 01:23:53.990351 lognflow-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-15 01:23:31.000000 lognflow-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:23:53.986351 lognflow-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-15 01:23:31.000000 lognflow-0.7.0/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 04:55:41.000000 lognflow-0.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-22 04:55:41.000000 lognflow-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 04:55:41.000000 lognflow-0.7.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-22 04:55:41.000000 lognflow-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 04:55:41.000000 lognflow-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-22 04:55:54.878346 lognflow-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-22 04:55:41.000000 lognflow-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.874346 lognflow-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.874346 lognflow-0.7.1/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65386 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 04:55:54.878346 lognflow-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-22 04:55:41.000000 lognflow-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 04:55:41.000000 lognflow-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.0/CONTRIBUTING.rst` & `lognflow-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/HISTORY.rst` & `lognflow-0.7.1/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -79,7 +79,13 @@
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
 
 0.7.0 (2023-05-15)
 ------------------
 * logviewer returns data by log_sigle if the full name is mentioned.
+
+0.7.1 (2023-05-22)
+------------------
+* printprogress supports lognflow.
+* bugs fixed in lognflow.
+* For now I guess lognflow and logviewer could be separate.
```

### Comparing `lognflow-0.7.0/LICENSE` & `lognflow-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/PKG-INFO` & `lognflow-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.0
+Version: 0.7.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -171,7 +171,13 @@
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
 
 0.7.0 (2023-05-15)
 ------------------
 * logviewer returns data by log_sigle if the full name is mentioned.
+
+0.7.1 (2023-05-22)
+------------------
+* printprogress supports lognflow.
+* bugs fixed in lognflow.
+* For now I guess lognflow and logviewer could be separate.
```

### Comparing `lognflow-0.7.0/README.rst` & `lognflow-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/docs/Makefile` & `lognflow-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/docs/conf.py` & `lognflow-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/docs/installation.rst` & `lognflow-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/docs/make.bat` & `lognflow-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/lognflow/lognflow.py` & `lognflow-0.7.1/lognflow/lognflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         log_name = self.log_name if (log_name is None) else log_name
 
         if((print_text is None) | (print_text is True)):
             print_text = self._print_text
         if(print_text):
             if(log_time_stamp):
                 print(f'T:{self.time_stamp:>6.6f}| ', end='')
-            print(to_be_logged)
+            print(to_be_logged, end = end)
                 
         if ( (not (log_name in self._loggers_dict)) or new_file):
             self._log_text_handler(log_name, 
                                    log_size_limit = log_size_limit,
                                    time_tag = time_tag)
 
         curr_textinlog = self._loggers_dict[log_name]
@@ -408,15 +408,18 @@
         if(isinstance(to_be_logged, list)):
             for _ in to_be_logged:
                 _tolog = str(_)
                 _logger.append(_tolog)
         else:
             _tolog = str(to_be_logged)
             _logger.append(_tolog)
-        if(_logger[-1][-1] != end):
+        if(len(_logger[-1]) > 0):
+            if(_logger[-1][-1] != end):
+                _logger.append(end)
+        else:
             _logger.append(end)
         log_size = 0
         for _logger_el in _logger:
             curr_textinlog.to_be_logged.append(_logger_el)
             log_size += len(_logger_el)
         curr_textinlog.log_size += log_size
         
@@ -665,14 +668,15 @@
         cax = divider.append_axes("right", size="5%", pad=0.05)
         cbar = fig.colorbar(mappable, cax=cax)
         # cbar.ax.tick_params(size=0.01)
 
     def log_multichannel_by_subplots(self, 
         parameter_name: str, 
         parameter_value: np.ndarray,
+        frame_shape = None,
         image_format='jpeg', 
         dpi=1200, 
         time_tag: bool = None,
         add_colorbar = False,
         remove_axis_ticks = True,
         **kwargs):
         """log multiple images as a tiled square
@@ -689,21 +693,26 @@
                     Wheather if the time stamp is in the file name or not.
                     
         """
         
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
         n_r, n_c, n_ch = parameter_value.shape
-        n_ch_sq = int(np.ceil(n_ch ** 0.5))
-        _, ax = plt.subplots(n_ch_sq,n_ch_sq)
+        
+        if(frame_shape is None):
+            n_ch_sq = int(np.ceil(n_ch ** 0.5))
+            n_ch_r, n_ch_c = (n_ch_sq, n_ch_sq)
+        else:
+            n_ch_r, n_ch_c = frame_shape
+        _, ax = plt.subplots(n_ch_r,n_ch_c)
         if(remove_axis_ticks):
             plt.setp(ax, xticks=[], yticks=[])
-        for rcnt in range(n_ch_sq):
-            for ccnt in range(n_ch_sq):
-                im = parameter_value[:,:, ccnt + rcnt * n_ch_sq]
+        for rcnt in range(n_ch_r):
+            for ccnt in range(n_ch_c):
+                im = parameter_value[:,:, ccnt + rcnt * n_ch_c]
                 im_ch = ax[rcnt, ccnt].imshow(im, **kwargs)
                 if(add_colorbar):
                     self.add_colorbar(im_ch)
         return self.log_plt(parameter_name = parameter_name,
                      image_format=image_format, dpi=dpi,
                      time_tag = time_tag)
             
@@ -876,15 +885,16 @@
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
         try:
             # from mpl_toolkits.mplot3d import Axes3D
             n_r, n_c = parameter_value.shape
             fig = plt.figure()
             ax = fig.add_subplot(111, projection='3d')
-            X, Y = np.meshgrid(np.arange(n_r), np.arange(n_c))
+            X, Y = np.meshgrid(np.arange(n_r, dtype='int'), 
+                               np.arange(n_c, dtype='int'))
             ax.plot_surface(X, Y, parameter_value, **kwargs)
             fpath = self.log_plt(
                 parameter_name = parameter_name, 
                 image_format=image_format, dpi=dpi,
                 time_tag = time_tag)
             return fpath
         except:
@@ -1039,43 +1049,120 @@
             if(len(stack.shape) == 4):
                 canv = np.zeros((n_imgs, new_n_R, new_n_C), 
                                 dtype = stack.dtype)
             if(len(stack.shape) == 5):
                 canv = np.zeros((n_imgs, new_n_R, new_n_C, 3),
                                  dtype = stack.dtype)
             used_ch_cnt = 0
-
-            stack[:,   :1      ] = borders
-            stack[:,   : ,   :1] = borders
-            stack[:, -1:       ] = borders
-            stack[:,   : , -1: ] = borders
+            if(borders is not None):
+                stack[:,   :1      ] = borders
+                stack[:,   : ,   :1] = borders
+                stack[:, -1:       ] = borders
+                stack[:,   : , -1: ] = borders
             
             for rcnt in range(square_side):
                 for ccnt in range(square_side):
                     ch_cnt = rcnt + square_side*ccnt
                     if (ch_cnt<n_ch):
                         canv[:, rcnt*n_R: (rcnt + 1)*n_R,
                                 ccnt*n_C: (ccnt + 1)*n_C] = \
                             stack[..., used_ch_cnt]
                         used_ch_cnt += 1
         else:
             return None
         return canv
 
+    def multichannel_to_frame(self, stack, 
+                              frame_shape : tuple = None, borders = 0):
+        """ turn a stack of multi-channel images into a frame of images
+            This is very useful when lots of images need to be tiled
+            against each other.
+        
+            :param stack: np.ndarray
+                    It must have the shape of either
+                    n_r x n_c x n_ch
+                    n_r x n_c x  3  x n_ch
+                    n_f x n_r x n_c x n_ch
+                    n_f x n_r x n_c x  3  x n_ch
+                    
+                In both cases n_ch will be turned into a square tile
+                Remember if you have N images to put into a square, the input
+                shape should be 1 x n_r x n_c x N
+            :param frame_shape: tuple
+                The shape of the frame to put n_rows and n_colmnss of images
+                close to each other to form a rectangle of image.
+            :param borders: literal or np.inf or np.nan
+                When plotting images with matplotlib.pyplot.imshow, there
+                needs to be a border between them. This is the value for the 
+                border elements.
+                
+            output
+            ---------
+                Since we have N channels to be laid into a square, the side
+                length woul be ceil(N**0.5)
+                it produces an np.array of shape n_f x n_r * S x n_c * S or
+                n_f x n_r * S x n_c * S x 3 in case of RGB input.
+        """
+        if(len(stack.shape) == 4):
+            if(stack.shape[3] == 3):
+                stack = np.array([stack])
+        if(len(stack.shape) == 3):
+            stack = np.array([stack])
+        
+        if((len(stack.shape) == 4) | (len(stack.shape) == 5)):
+            if(len(stack.shape) == 4):
+                n_imgs, n_R, n_C, n_ch = stack.shape
+            if(len(stack.shape) == 5):
+                n_imgs, n_R, n_C, is_rgb, n_ch = stack.shape
+                if(is_rgb != 3):
+                    return None
+            if(frame_shape is None):
+                square_side = int(np.ceil(np.sqrt(n_ch)))
+                frame_n_r, frame_n_c = (square_side, square_side)
+            else:
+                frame_n_r, frame_n_c = frame_shape
+            
+            new_n_R = n_R * frame_n_r
+            new_n_C = n_C * frame_n_c
+            if(len(stack.shape) == 4):
+                canv = np.zeros((n_imgs, new_n_R, new_n_C), 
+                                dtype = stack.dtype)
+            if(len(stack.shape) == 5):
+                canv = np.zeros((n_imgs, new_n_R, new_n_C, 3),
+                                 dtype = stack.dtype)
+            used_ch_cnt = 0
+            if(borders is not None):
+                stack[:,   :1      ] = borders
+                stack[:,   : ,   :1] = borders
+                stack[:, -1:       ] = borders
+                stack[:,   : , -1: ] = borders
+            
+            for rcnt in range(frame_n_r):
+                for ccnt in range(frame_n_c):
+                    ch_cnt = rcnt + frame_n_c*ccnt
+                    if (ch_cnt<n_ch):
+                        canv[:, rcnt*n_R: (rcnt + 1)*n_R,
+                                ccnt*n_C: (ccnt + 1)*n_C] = \
+                            stack[..., used_ch_cnt]
+                        used_ch_cnt += 1
+        else:
+            return None
+        return canv
+
     def _handle_images_stack(self, stack, borders = 0):
         canv = None
         if(len(stack.shape) == 2):
             canv = np.expand_dims(stack, axis=0)
         if(len(stack.shape) == 3):
             if(stack.shape[2] == 3):
                 canv = np.expand_dims(stack, axis=0)
             else:
                 canv = stack
         if((len(stack.shape) == 4) | (len(stack.shape) == 5)):
-            canv = self.multichannel_to_square(stack, borders = borders)
+            canv = self.multichannel_to_frame(stack, borders = borders)
         return canv
     
     def prepare_stack_of_images(self, 
                                 list_of_stacks, 
                                 borders = 0):
         """Prepare the stack of images
             If you wish to use the log_canvas, chances are you have a list
@@ -1357,247 +1444,14 @@
         ani = animation.ArtistAnimation(\
             fig, ims, interval = interval, blit = blit,
             repeat_delay = repeat_delay)    
         ani.save(fpath, dpi = dpi, 
                  writer = animation.PillowWriter(fps=int(1000/interval)))
         return fpath
 
-    def get_text(self, log_name='main_log'):
-        """ get text log files
-            Given the log_name, this function returns the text therein.
-
-            Parameters
-            ----------
-            :param log_name:
-                the log name. If not given then it is the main log.
-        """
-        flist = list(self.log_dir.glob(f'{log_name}*.txt'))
-        flist.sort()
-        n_files = len(flist)
-        if (n_files>0):
-            txt = []
-            for fcnt in range(n_files):
-                with open(flist[fcnt]) as f_txt:
-                    txt.append(f_txt.readlines())
-            if(n_files == 1):
-                txt = txt[0]
-            return txt
-
-    def get_single(self, var_name, single_shot_index = -1, 
-                     suffix = '.np*'):
-        """ get a single variable
-            return the value of a saved variable.
-
-            :param var_name:
-                variable name
-            :param single_shot_index:
-                If there are many snapshots of a variable, this input can
-                limit the returned to a set of indices.
-            :param suffix:
-                If there are different suffixes availble for a variable
-                this input needs to be set. npy, npz, mat, and torch are
-                supported.
-                
-            .. note::
-                when reading a MATLAB file, the output is a dictionary.
-        """
-        var_name = var_name.replace('\t', '\\t').replace('\n', '\\n')\
-            .replace('\r', '\\r').replace('\b', '\\b')
-        
-        suffix = suffix.strip('.')
-        assert single_shot_index == int(single_shot_index), \
-                    f'single_shot_index {single_shot_index} must be an integer'
-        flist = []            
-        if((self.log_dir / var_name).is_file()):
-            flist = [self.log_dir / var_name]
-        elif((self.log_dir / f'{var_name}.{suffix}').is_file()):
-            flist = [self.log_dir / f'{var_name}.{suffix}']
-        else:
-            _var_name = (self.log_dir / var_name).name
-            _var_dir = (self.log_dir / var_name).parent
-            flist = list(_var_dir.glob(f'{_var_name}*.{suffix}'))
-            if(len(flist) == 0):
-                flist = list(_var_dir.glob(f'{_var_name}*.*'))
-                if(len(flist) > 0):
-                    # self.log_text(None, 
-                    #     'Can not find the file with the given suffix, '\
-                    #     +'but found some with a different suffix, '\
-                    #     +f'one file is: {flist[single_shot_index]}')
-                    pass
-                    
-        if(len(flist) > 0):
-            flist.sort()
-        else:
-            var_dir = self.log_dir / var_name
-            if(var_dir.is_dir()):
-                flist = list(var_dir.glob('*.*'))
-            if(len(flist) > 0):
-                flist.sort()
-            else:
-                # self.log_text(None, 'No such variable')
-                return
-        var_path = flist[single_shot_index]
-                
-        if(var_path.is_file()):
-            # self.log_text(None, f'Loading {var_path}')
-            if(var_path.suffix == '.npz'):
-                buf = np.load(var_path)
-                try:
-                    time_array = buf['time_array']
-                    n_logs = (time_array > 0).sum()
-                    time_array = time_array[:n_logs]
-                    data_array = buf['data_array']
-                    data_array = data_array[:n_logs]
-                    return((time_array, data_array))
-                except:
-                    return buf
-            if(var_path.suffix == '.npy'):
-                return(np.load(var_path))
-            if(var_path.suffix == '.mat'):
-                return(loadmat(var_path))
-            if(var_path.suffix == '.txt'):
-                with open(var_path) as f_txt:
-                    return(f_txt.read())
-            if((var_path.suffix == '.tif') | (var_path.suffix == '.tiff')):
-                from tifffile import imread
-                return(imread(var_path))                
-            if(var_path.suffix == '.torch'):      
-                from torch import load as torch_load 
-                return(torch_load(var_path))
-            try:
-                img = imread(var_path)
-                return(img)
-            except:
-                pass
-    
-    def get_stack_of_files(self, 
-        var_name = None, flist = [], suffix = '*',
-        return_data = False, return_flist = True) -> tuple:
-        
-        """ Get list or data of all files in a directory
-        
-            This function gives the list of paths of all files in a directory
-            for a single variable. 
-
-            :param var_name:
-                The directory or variable name to look for the files
-            :type var_name: str
-            
-            :param flist:
-                list of Paths, if data is returned, this flist input can limit 
-                the data requested to this list.
-            :type flist: list
-            
-            :param suffix:
-                the suffix of files to look for, e.g. 'txt'
-            :type siffix: str
-            
-            :param return_data: 
-                    with flist you can limit the data that is returned.
-                    Otherwise the data for all files in the directory will be
-                    returned
-            :param return_flist
-                    Maybe you are only intrested in the flist.
-                    
-            :return:
-                It returns a tuple, (dataset, flist),
-                dataset will be a numpy array in case all files produce same
-                shape numpy arrays.
-                flist is type pathlib.Path
-            :rtype: tuple
-            
-            
-        """
-        suffix = suffix.strip('.')
-        if not flist:
-            assert var_name is not None, \
-                ' The file list is empty. Please provide the ' \
-                + 'variable name or a non-empty file list.'
-            var_dir = self.log_dir / var_name
-            if(var_dir.is_dir()):
-                var_fname = None
-                flist = list(var_dir.glob(f'*.{suffix}'))
-            else:
-                var_fname = var_dir.name
-                var_dir = var_dir.parent
-                patt = f'{var_fname}*.{suffix}'
-                patt = patt.replace('**', '*')
-                flist = list(var_dir.glob(patt))
-        if flist:
-            flist.sort()
-            n_files = len(flist)
-            if((not return_data) & return_flist):
-                return(flist)
-            data_type = None
-            if(data_type is None):
-                try:
-                    fdata = np.load(flist[0])
-                    data_type = 'numpy'
-                except:
-                    pass
-            if(data_type is None):
-                try:
-                    fdata = imread(flist[0])
-                    data_type = 'image'
-                except:
-                    pass
-            if(data_type is not None):
-                dataset = np.zeros((n_files, ) + fdata.shape, 
-                                   dtype=fdata.dtype)
-                for fcnt, fpath in enumerate(flist):
-                    if(data_type == 'numpy'):
-                        dataset[fcnt] = np.load(fpath)
-                    elif(data_type == 'image'):
-                        dataset[fcnt] = imread(fpath)
-                # self.log_text(None, f'shape is: {dataset.shape}')
-                if(return_flist):
-                    return(dataset, flist)
-                else:
-                    return(dataset)
-            else:
-                # self.log_text(None, f'File {flist[0].name} cannot be opened'\
-                #           + r' by np.load() or plt.imread()')
-                pass
-            
-    def get_common_files(self, var_name_A, var_name_B):
-        """ get common files in two directories
-        
-            It happens often in ML that there are two directories, A and B,
-            and we are interested to get the flist in both that is common 
-            between them. returns a tuple of two lists of files.
-            
-            :param var_name_A:
-                directory A name
-            :param var_name_B:
-                directory B name
-        """
-        flist_A = self.get_stack_of_files(
-            var_name_A, return_data = False, return_flist = True)
-        flist_B = self.get_stack_of_files(
-            var_name_B, return_data = False, return_flist = True)
-        
-        suffix_A = flist_A[0].suffix
-        suffix_B = flist_B[0].suffix 
-        parent_A = flist_A[0].parent
-        parent_B = flist_B[0].parent
-        
-        fstems_A = [_fst.stem for _fst in flist_A]
-        fstems_B = [_fst.stem for _fst in flist_B]
-        
-        fstems_A_set = set(fstems_A)
-        fstems_B_set = set(fstems_B)
-        common_stems = list(fstems_A_set.intersection(fstems_B_set))
-
-        flist_A_new = [parent_A / (common_stem + suffix_A) \
-                          for common_stem in common_stems]
-        flist_B_new = [parent_B / (common_stem + suffix_B) \
-                          for common_stem in common_stems]
-
-        return(flist_A_new, flist_B_new)
-    
     def replace_time_with_index(self, var_name):
         """ index in file names
             lognflow uses time stamps to make new log files for a variable.
             That is done by putting time stamp after the name of the variable.
             This function changes all of the time stamps, sorted ascendingly,
             by indices.
             
@@ -1629,22 +1483,18 @@
         for log_name in list(self._loggers_dict):
             self.log_text_flush(log_name, flush = True)
         for parameter_name in list(self._vars_dict):
             self.log_var_flush(parameter_name)
 
     def __call__(self, *args, **kwargs):
         """calling the object
-        
             In the case of the following code::
-            
                 logger = lognflow()
                 logger('Hello lognflow')
-            
             The text (str(...)) will be passed to the main log text file.
-        
         """
         self.log_text(None, *args, **kwargs)
 
     def __del__(self):
         try:
             self.flush_all()
         except:
```

### Comparing `lognflow-0.7.0/lognflow/logviewer.py` & `lognflow-0.7.1/lognflow/logviewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,20 +115,23 @@
                 return
         var_path = flist[single_shot_index]
                 
         if(var_path.is_file()):
             self.logger(f'Loading {var_path}')
             if(var_path.suffix == '.npz'):
                 buf = np.load(var_path)
-                time_array = buf['time_array']
-                n_logs = (time_array > 0).sum()
-                time_array = time_array[:n_logs]
-                data_array = buf['data_array']
-                data_array = data_array[:n_logs]
-                return((time_array, data_array))
+                try:
+                    time_array = buf['time_array']
+                    n_logs = (time_array > 0).sum()
+                    time_array = time_array[:n_logs]
+                    data_array = buf['data_array']
+                    data_array = data_array[:n_logs]
+                    return((time_array, data_array))
+                except:
+                    return(buf)
             if(var_path.suffix == '.npy'):
                 return(np.load(var_path))
             if(var_path.suffix == '.mat'):
                 from scipy.io import loadmat
                 return(loadmat(var_path))
             if(var_path.suffix == '.txt'):
                 with open(var_path) as f_txt:
@@ -236,14 +239,16 @@
                 try:
                     from matplotlib.pyplot import imread
                     fdata = imread(flist[0])
                     read_func = plt.imread
                 except:
                     pass
             if(read_func is not None):
+                assert callable(read_func), \
+                    f'given read_func: {read_func} is not callable.'
                 fdata = read_func(flist[0])
                 dataset = np.zeros((n_files, ) + fdata.shape, 
                                    dtype=fdata.dtype)
                 for fcnt, fpath in enumerate(flist):
                     dataset[fcnt] = read_func(fpath)
                 if(verbose):
                     self.logger(f'logviewer: Reading dataset from {var_dir}'
@@ -291,45 +296,12 @@
         flist_A_new = [parent_A / (common_stem + suffix_A) \
                           for common_stem in common_stems]
         flist_B_new = [parent_B / (common_stem + suffix_B) \
                           for common_stem in common_stems]
 
         return(flist_A_new, flist_B_new)
     
-    def replace_time_with_index(self, var_name):
-        """ index in file names
-            lognflow uses time stamps to make new log files for a variable.
-            That is done by putting _time_stamp after the name of the variable.
-            This function changes all of the time stamps, sorted ascendingly,
-            by indices.
-            
-            Parameters
-            ----------
-            :param var_name:
-                variable name
-        """
-        var_dir = self.log_dir / var_name
-        if(var_dir.is_dir()):
-            var_fname = None
-            flist = list(var_dir.glob(f'*.*'))
-        else:
-            var_fname = var_dir.name
-            var_dir = var_dir.parent
-            flist = list(var_dir.glob(f'{var_fname}_*.*'))
-        if flist:
-            flist.sort()
-            fcnt_width = len(str(len(flist)))
-            for fcnt, fpath in enumerate(flist):
-                self.logger(f'Changing {flist[fcnt].name}')
-                fname_new = ''
-                if(var_fname is not None):
-                    fname_new = var_fname + '_'
-                fname_new += f'{fcnt:0{fcnt_width}d}' + flist[fcnt].suffix
-                fpath_new = flist[fcnt].parent / fname_new
-                self.logger(f'To {fpath_new.name}')
-                flist[fcnt].rename(fpath_new)
-                
     def __repr__(self):
-        return f'<logviewer(log_dir = {self.log_dir})>'
+        return f'{self.log_dir}'
 
     def __bool__(self):
         return self.log_dir.is_dir()
```

### Comparing `lognflow-0.7.0/lognflow/printprogress.py` & `lognflow-0.7.1/lognflow/printprogress.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     and then call it in every iteration of the loop. If you'd like it
     to go faster, call it with give number of steps that have passed.
     """
     def __init__(self, 
                  n_steps, 
                  numTicks = 80,
                  title = None,
+                 method = 'linear',
                  print_function = print,
-                 method = 'linear'):
+                 **print_function_kwargs):
         """
             n_steps: int
                 Number of iterations in the for loop
             numTicks: int
                 The number of charachters in a row of the screen - 2
                 default: 78 for old screens that have 80 coloumns
             title : str 
@@ -38,14 +39,15 @@
                        p                   x      
                 |-----------|--------------------------|
                            ck                       n_steps
                 As such  x/(n-c) = p/c => x = p(n/c - 1)
                 more options to come
         """
         assert method in ['linear', 'linear_robust']
+        self.print_function_kwargs = print_function_kwargs
         self.method = method
         self.in_print_function = print_function
         if(n_steps != int(n_steps)):
             self._print_func('textProgBar takes integers no less than 2 ')
             n_steps = int(n_steps)
         if(n_steps<2):
             n_steps = 2
@@ -75,15 +77,16 @@
         self._print_func(' ', end = '')
     
     def _print_func(self, text, end='\n'):
         if (self.in_print_function is not None):
             if (self.in_print_function == print):
                 print(text, end = end, flush = True)
             else:
-                self.in_print_function(text)
+                self.in_print_function(text, end = end,
+                                       **self.print_function_kwargs)
         
     def _calc_ETA(self):
         if(self.method == 'linear'):
             passedTime = time() - self.startTime
             remTimeS = passedTime * ( self.n_steps / self.ck - 1)
         
         return remTimeS
```

### Comparing `lognflow-0.7.0/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.1/lognflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.0
+Version: 0.7.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -171,7 +171,13 @@
 * Fixing readme for PyPI.
 * removed marker from log_plot. user marker and linestyle keyword arguments.
 * printprogress returns proper ETA every time if print_function is set to None::
 
 0.7.0 (2023-05-15)
 ------------------
 * logviewer returns data by log_sigle if the full name is mentioned.
+
+0.7.1 (2023-05-22)
+------------------
+* printprogress supports lognflow.
+* bugs fixed in lognflow.
+* For now I guess lognflow and logviewer could be separate.
```

### Comparing `lognflow-0.7.0/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.1/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/setup.py` & `lognflow-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.0/tests/test_lognflow.py` & `lognflow-0.7.1/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.0/tests/test_logviewer.py` & `lognflow-0.7.1/tests/test_logviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         'A/', return_data=False, return_flist=True)
     flist_B = logged.get_stack_of_files(
         'B/', return_data=False, return_flist=True)
     
     logger(flist_A)
     logger(flist_B)
     
-    logged.replace_time_with_index('A/')
-    logged.replace_time_with_index('B/')
+    logger.replace_time_with_index('A/')
+    logger.replace_time_with_index('B/')
     
     stack_A = logged.get_stack_of_files('A/', return_data = True, return_flist = False)
     stack_B = logged.get_stack_of_files('B/', return_data = True, return_flist = False)
 
     logger(stack_A.shape)
     logger(stack_B.shape)
     
@@ -98,15 +98,15 @@
     logged = logviewer(logger.log_dir, logger)
 
     data_in, flist = logged.get_stack_of_files(
         'test_param', return_data=True, return_flist=True)
     
     logger(flist)
 
-    logged.replace_time_with_index('test_param')
+    logger.replace_time_with_index('test_param')
     
     data_out, flist = logged.get_stack_of_files(
         'test_param', return_data=True, return_flist=True)
     
     logger(flist)
     
     logger(data_in)
```

### Comparing `lognflow-0.7.0/tests/test_printprogress.py` & `lognflow-0.7.1/tests/test_printprogress.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 def test_content(response):
     """Sample pytest test function with the pytest fixture as an argument."""
     # from bs4 import BeautifulSoup
     # assert 'GitHub' in BeautifulSoup(response.content).title.string
 
 def test_printprogress():
     N = 15000000
-    pprog = printprogress(N)
+    pprog = printprogress(Ne)
     for _ in range(N):
         pprog()
     # assert input('Did it show you a progress bar? (y for yes)')=='y'
-    
+
+def test_with_logger():
+    logger = lognflow()
+    N = 1500000
+    pprog = printprogress(Ne, print_function = logger, log_time_stamp = False)
+    for _ in range(N):
+        pprog()
+
 if __name__ == '__main__':
-    test_printprogress()
+    test_printprogress()
+    test_with_logger()
+    exit()
```

