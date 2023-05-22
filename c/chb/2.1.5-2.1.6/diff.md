# Comparing `tmp/chb-2.1.5.tar.gz` & `tmp/chb-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chb-2.1.5.tar", last modified: Thu Apr 20 15:10:23 2023, max compression
+gzip compressed data, was "chb-2.1.6.tar", last modified: Mon May 22 06:30:11 2023, max compression
```

## Comparing `chb-2.1.5.tar` & `chb-2.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.952567 chb-2.1.5/
--rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      637 2023-04-20 15:10:23.952567 chb-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.948342 chb-2.1.5/chb/
--rw-rw-rw-   0        0        0     5471 2023-04-07 05:55:28.000000 chb-2.1.5/chb/__init__.py
--rw-rw-rw-   0        0        0     8851 2023-04-20 15:09:42.000000 chb-2.1.5/chb/_dao.py
--rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_importable.py
--rw-rw-rw-   0        0        0     3977 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_imports.py
--rw-rw-rw-   0        0        0     4644 2023-04-07 05:55:28.000000 chb-2.1.5/chb/_log.py
--rw-rw-rw-   0        0        0    25832 2023-04-20 15:04:31.000000 chb-2.1.5/chb/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:10:23.951569 chb-2.1.5/chb.egg-info/
--rw-rw-rw-   0        0        0      637 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-20 15:10:23.000000 chb-2.1.5/chb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 15:10:23.953564 chb-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-20 15:04:31.000000 chb-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.433036 chb-2.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-07 05:55:28.000000 chb-2.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      637 2023-05-22 06:30:11.433036 chb-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-04-07 05:55:28.000000 chb-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.428049 chb-2.1.6/chb/
+-rw-rw-rw-   0        0        0     5506 2023-05-22 06:29:52.000000 chb-2.1.6/chb/__init__.py
+-rw-rw-rw-   0        0        0     8851 2023-04-20 15:09:42.000000 chb-2.1.6/chb/_dao.py
+-rw-rw-rw-   0        0        0     3424 2023-04-07 05:55:28.000000 chb-2.1.6/chb/_importable.py
+-rw-rw-rw-   0        0        0     4038 2023-05-22 06:17:54.000000 chb-2.1.6/chb/_imports.py
+-rw-rw-rw-   0        0        0     4644 2023-04-07 05:55:28.000000 chb-2.1.6/chb/_log.py
+-rw-rw-rw-   0        0        0    26819 2023-05-22 06:20:18.000000 chb-2.1.6/chb/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:30:11.431041 chb-2.1.6/chb.egg-info/
+-rw-rw-rw-   0        0        0      637 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-22 06:30:11.000000 chb-2.1.6/chb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 06:30:11.433442 chb-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-05-22 06:27:10.000000 chb-2.1.6/setup.py
```

### Comparing `chb-2.1.5/LICENSE.txt` & `chb-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chb-2.1.5/PKG-INFO` & `chb-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.5
+Version: 2.1.6
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.5/chb/__init__.py` & `chb-2.1.6/chb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,7 +145,8 @@
 from chb._utils import bar
 from chb._utils import bar2
 from chb._utils import getsizeof
 from chb._utils import getdeepsizeof
 from chb._utils import Timer
 from chb._utils import GetFirstLetter
 from chb._utils import Cpen
+from chb._utils import show_image
```

### Comparing `chb-2.1.5/chb/_dao.py` & `chb-2.1.6/chb/_dao.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.5/chb/_importable.py` & `chb-2.1.6/chb/_importable.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.5/chb/_imports.py` & `chb-2.1.6/chb/_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 from ._importable import LazyImport, _get_import_statements
 
 ### Data Wrangling
 pd = LazyImport("import pandas as pd")
 np = LazyImport("import numpy as np")
+transforms = LazyImport("from torchvision import transforms")
+
 #
 # ### Data Visualization and Plotting
-# mpl = LazyImport("import matplotlib as mpl")
-# plt = LazyImport("import matplotlib.pyplot as plt")
+mpl = LazyImport("import matplotlib as mpl")
+plt = LazyImport("import matplotlib.pyplot as plt")
 # sns = LazyImport("import seaborn as sns")
 # Image = LazyImport("from PIL import Image")
 #
 #
 # xgb = LazyImport("import xgboost as xgb")
 # lgb = LazyImport("import lightgbm as lgb")
 #
```

### Comparing `chb-2.1.5/chb/_log.py` & `chb-2.1.6/chb/_log.py`

 * *Files identical despite different names*

### Comparing `chb-2.1.5/chb/_utils.py` & `chb-2.1.6/chb/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -652,9 +652,26 @@
         while True:
             lines = self.f.readlines(num_lines)
             if not lines:
                 break
             yield lines
 
 
+def show_image(img_lst, **imshow_kwargs):
+    """
+    pytorch建模过程中，展示图片用。图片可以是Pillow.Image，也可以是torch.Tensor。
+    img_lst: 保存图像和标题的list，形如：[(image1, title1),(image2, title2)]。image可以使Pillow.Image对象，也可以是torch.Tensor。
+    imshow_kwargs: 需要传递给plt.imshow的参数
+    """
+    mpl.rcParams['font.sans-serif'] = ['SimHei']  # 中文字体支持
+    fig, axs =plt.subplots(1,len(img_lst), constrained_layout=True,  figsize=(2*len(img_lst),2), squeeze=False)
+    for i, (img, title) in enumerate(img_lst):
+        if isinstance(img, torch.Tensor):  # 如果是torch.Tensor类型，就必须转换成Pillow.Image类型，才能进行展示
+            img = transforms.ToPILImage()(img)
+        axs[0, i].imshow(np.asarray(img), **imshow_kwargs)
+        # axs[0, i].set(xticklabels=[], yticklabels=[], xticks=[], yticks=[])
+        axs[0, i].set_title(title)
+    plt.show()
+
+
 if __name__=='__main__':
     print(Timer.datebetween('2022-01-01 00:00:00', '2022-01-04 00:00:00'))
```

### Comparing `chb-2.1.5/chb.egg-info/PKG-INFO` & `chb-2.1.6/chb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chb
-Version: 2.1.5
+Version: 2.1.6
 Summary: chb常用代码库
 Home-page: https://github.com/ChenHuabin321/pypi
 Author: chenhuabin
 Author-email: chenhuabin321@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chb-2.1.5/setup.py` & `chb-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chb",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="2.1.5",  # 包版本号，便于维护版本
+    version="2.1.6",  # 包版本号，便于维护版本
     author="chenhuabin",  # 作者，可以写自己的姓名
     author_email="chenhuabin321@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="chb常用代码库",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/ChenHuabin321/pypi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

