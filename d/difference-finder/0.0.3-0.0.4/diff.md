# Comparing `tmp/difference_finder-0.0.3.tar.gz` & `tmp/difference_finder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "difference_finder-0.0.3.tar", last modified: Sun May 21 11:11:36 2023, max compression
+gzip compressed data, was "difference_finder-0.0.4.tar", last modified: Mon May 22 12:56:48 2023, max compression
```

## Comparing `difference_finder-0.0.3.tar` & `difference_finder-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-21 11:11:36.321010 difference_finder-0.0.3/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4373 2023-05-21 11:11:36.321010 difference_finder-0.0.3/PKG-INFO
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     3936 2023-05-21 07:37:57.000000 difference_finder-0.0.3/README.md
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-21 11:11:36.321010 difference_finder-0.0.3/difference_finder/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       21 2023-05-21 11:04:50.000000 difference_finder-0.0.3/difference_finder/__init__.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1723 2023-05-20 12:40:53.000000 difference_finder-0.0.3/difference_finder/data.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4729 2023-05-21 07:33:36.000000 difference_finder-0.0.3/difference_finder/finder.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      441 2023-05-21 07:30:55.000000 difference_finder-0.0.3/difference_finder/logger.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1514 2023-05-20 13:29:54.000000 difference_finder-0.0.3/difference_finder/metrics.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1834 2023-05-20 13:05:45.000000 difference_finder-0.0.3/difference_finder/processor.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1516 2023-05-20 11:07:27.000000 difference_finder-0.0.3/difference_finder/strategy.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2964 2023-05-20 12:42:22.000000 difference_finder-0.0.3/difference_finder/utils.py
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-21 11:11:36.321010 difference_finder-0.0.3/difference_finder.egg-info/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4373 2023-05-21 11:11:36.000000 difference_finder-0.0.3/difference_finder.egg-info/PKG-INFO
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      411 2023-05-21 11:11:36.000000 difference_finder-0.0.3/difference_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        1 2023-05-21 11:11:36.000000 difference_finder-0.0.3/difference_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       18 2023-05-21 11:11:36.000000 difference_finder-0.0.3/difference_finder.egg-info/top_level.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       38 2023-05-21 11:11:36.321010 difference_finder-0.0.3/setup.cfg
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      649 2023-05-21 11:04:41.000000 difference_finder-0.0.3/setup.py
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-22 12:56:48.706994 difference_finder-0.0.4/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4373 2023-05-22 12:56:48.706994 difference_finder-0.0.4/PKG-INFO
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     3936 2023-05-21 07:37:57.000000 difference_finder-0.0.4/README.md
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-22 12:56:48.706994 difference_finder-0.0.4/difference_finder/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       21 2023-05-22 12:49:39.000000 difference_finder-0.0.4/difference_finder/__init__.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1723 2023-05-20 12:40:53.000000 difference_finder-0.0.4/difference_finder/data.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     5336 2023-05-22 12:47:16.000000 difference_finder-0.0.4/difference_finder/finder.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      441 2023-05-21 07:30:55.000000 difference_finder-0.0.4/difference_finder/logger.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1514 2023-05-20 13:29:54.000000 difference_finder-0.0.4/difference_finder/metrics.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1834 2023-05-20 13:05:45.000000 difference_finder-0.0.4/difference_finder/processor.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1816 2023-05-22 12:25:10.000000 difference_finder-0.0.4/difference_finder/strategy.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2964 2023-05-20 12:42:22.000000 difference_finder-0.0.4/difference_finder/utils.py
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-22 12:56:48.706994 difference_finder-0.0.4/difference_finder.egg-info/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4373 2023-05-22 12:56:48.000000 difference_finder-0.0.4/difference_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      451 2023-05-22 12:56:48.000000 difference_finder-0.0.4/difference_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        1 2023-05-22 12:56:48.000000 difference_finder-0.0.4/difference_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       57 2023-05-22 12:56:48.000000 difference_finder-0.0.4/difference_finder.egg-info/requires.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       18 2023-05-22 12:56:48.000000 difference_finder-0.0.4/difference_finder.egg-info/top_level.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       38 2023-05-22 12:56:48.706994 difference_finder-0.0.4/setup.cfg
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      813 2023-05-22 12:55:23.000000 difference_finder-0.0.4/setup.py
```

### Comparing `difference_finder-0.0.3/PKG-INFO` & `difference_finder-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difference_finder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find difference between two images using pytorch.
 Home-page: https://github.com/jeongsol-kim/difference_finder
 Author: Jeongsol Kim
 Author-email: wjdthf3927@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `difference_finder-0.0.3/README.md` & `difference_finder-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.3/difference_finder/data.py` & `difference_finder-0.0.4/difference_finder/data.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.3/difference_finder/finder.py` & `difference_finder-0.0.4/difference_finder/finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 
 class Finder(object):
     def __init__(self,
                  pre_processor: Optional[object]='identity',
                  post_processor: Optional[object]='identity',
                  strategy: Optional[str]='gradient',
                  metric: Optional[str]='mse',
+                 device: Optional[str]='cpu',
                  verbose: Optional[bool]=False,
                  ):
         self.pre_processor = get_preprocessor(name=pre_processor)
         self.post_processor = get_postprocessor(name=post_processor)
         self.strategy = get_strategy(name=strategy)
         self.metric = get_metric(name=metric)
+        self.device = device
         
         self.logger = Logger().initLogger()
         if not verbose:
             self.logger.setLevel('CRITICAL')
 
     def _shape_check(self, img: torch.Tensor):
         # ndim == 2 -> (HW)
@@ -55,59 +57,71 @@
             if d1 > d3 and d2 > d3:
                 self.logger.info('Given dimension NxHxWxC, convert to NxCxHxW.')
                 img = img.permute(0, 3, 1, 2)
         else:
             raise NotImplementedError(f'Unexpected input shape - {img.ndim}D')
         return img
         
-    def run_on_image(self, img1: torch.Tensor, img2: torch.Tensor):
-        img1 = self.pre_processor(self._shape_check(img1))
-        img2 = self.pre_processor(self._shape_check(img2))
-        _map = self.strategy(img1, img2, metric_fn=self.metric)
+    def run_on_image(self, img1: torch.Tensor, img2: torch.Tensor, return_metric: Optional[bool]=False):
+        img1 = self.pre_processor(self._shape_check(img1)).to(self.device)
+        img2 = self.pre_processor(self._shape_check(img2)).to(self.device)
+        _map, _metric = self.strategy(img1, img2, metric_fn=self.metric, return_metric=return_metric)
         output = self.post_processor(_map)
 
         # output as numpy
         # remove batch dimension and reduce mean.
         # shared for every post_process, so excluded.
         output = to_np(output)[0].mean(axis=-1)
+
+        if return_metric:
+            return (output, _metric)
         return output
     
-    def run_on_directory(self, img1: Path, img2: Path):
+    def run_on_directory(self, img1: Path, img2: Path, return_metric: Optional[bool]=False):
         files1 = get_image_files(img1)
         self.logger.info(f'Images detected from the first directory: {len(files1)}')
         files2 = get_image_files(img2)
         self.logger.info(f'Images detected from the second directory: {len(files2)}')
         loader = get_loader(files1=files1,
                             files2=files2,
                             transform=ToTensor(),
                             num_workers=0
                             )
         outputs = []
+        metrics = []
         for i, (first_img, second_img) in enumerate(loader):
             self.logger.info(f'Run on {i+1}th image.')
-            output = self.run_on_image(first_img, second_img)
-            outputs.append(output)
+            output = self.run_on_image(first_img, second_img, return_metric)
+            if return_metric:
+                outputs.append(output[0])
+                metrics.append(output[1])
+            else:
+                outputs.append(output)
+        
+        if return_metric:
+            return (outputs, metrics)
         return outputs
     
     def run(self,
             img1: Union[Path, torch.Tensor],
-            img2: Union[Path, torch.Tensor]):
+            img2: Union[Path, torch.Tensor],
+            return_metric: Optional[bool]=False):
 
         if isinstance(img1, Path) and isinstance(img2, Path):
             if img1.is_dir() and img2.is_dir():
                 self.logger.info(f'Get two image directories.')
-                output = self.run_on_directory(img1, img2)
+                output = self.run_on_directory(img1, img2, return_metric)
             else:
                 self.logger.info(f'Get two image paths.')
                 loader = get_loader(files1=[img1],
                                     files2=[img2],
                                     transform=ToTensor(),
                                     num_workers=0)
                 first_img, second_img = next(iter(loader))
-                output = self.run_on_image(first_img, second_img)
+                output = self.run_on_image(first_img, second_img, return_metric)
         else:
             self.logger.info(f'Get two image tensors.')
             output = self.run_on_image(img1, img2)
         return output
 
     def save_fn(self):
         pass
```

### Comparing `difference_finder-0.0.3/difference_finder/metrics.py` & `difference_finder-0.0.4/difference_finder/metrics.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.3/difference_finder/processor.py` & `difference_finder-0.0.4/difference_finder/processor.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.3/difference_finder/utils.py` & `difference_finder-0.0.4/difference_finder/utils.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.3/difference_finder.egg-info/PKG-INFO` & `difference_finder-0.0.4/difference_finder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difference-finder
-Version: 0.0.3
+Version: 0.0.4
 Summary: Find difference between two images using pytorch.
 Home-page: https://github.com/jeongsol-kim/difference_finder
 Author: Jeongsol Kim
 Author-email: wjdthf3927@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `difference_finder-0.0.3/setup.py` & `difference_finder-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import setuptools
 
 setuptools.setup(
     name="difference_finder",
-    version="0.0.3",
+    version="0.0.4",
     license='MIT',
     author="Jeongsol Kim",
     author_email="wjdthf3927@gmail.com",
     description="Find difference between two images using pytorch.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/jeongsol-kim/difference_finder",
     packages=setuptools.find_packages(),
+    install_requires=[
+        'numpy',
+        'Pillow',
+        'rich',
+        'torch',
+        'torchvision',
+        'lpips',
+        'pytorch-msssim',
+    ],
     classifiers=[
         # 패키지에 대한 태그
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
 )
```

