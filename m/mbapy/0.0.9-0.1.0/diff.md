# Comparing `tmp/mbapy-0.0.9.tar.gz` & `tmp/mbapy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.0.9.tar", last modified: Mon Mar 20 16:40:50 2023, max compression
+gzip compressed data, was "mbapy-0.1.0.tar", last modified: Mon May 22 09:51:42 2023, max compression
```

## Comparing `mbapy-0.0.9.tar` & `mbapy-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 16:40:50.874974 mbapy-0.0.9/
--rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     2177 2023-03-20 16:40:50.874974 mbapy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2023-03-20 15:11:19.000000 mbapy-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 16:40:50.810969 mbapy-0.0.9/mbapy/
--rw-rw-rw-   0        0        0      363 2023-03-20 16:40:02.000000 mbapy-0.0.9/mbapy/__init__.py
--rw-rw-rw-   0        0        0      356 2023-03-20 16:39:34.000000 mbapy-0.0.9/mbapy/__version__.py
--rw-rw-rw-   0        0        0     2572 2023-03-20 16:36:28.000000 mbapy-0.0.9/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2023-03-20 16:40:50.866971 mbapy-0.0.9/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      181 2023-03-20 16:11:34.000000 mbapy-0.0.9/mbapy/dl_torch/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-03-20 16:35:29.000000 mbapy-0.0.9/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.0.9/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0     8732 2023-03-20 16:35:37.000000 mbapy-0.0.9/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0     1622 2023-03-20 16:35:29.000000 mbapy-0.0.9/mbapy/file.py
--rw-rw-rw-   0        0        0    11581 2023-03-20 15:04:49.000000 mbapy-0.0.9/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2023-03-20 16:40:50.874974 mbapy-0.0.9/mbapy/stats/
--rw-rw-rw-   0        0        0      331 2022-12-09 11:25:53.000000 mbapy-0.0.9/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.0.9/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     8827 2023-03-20 16:03:33.000000 mbapy-0.0.9/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2023-03-20 16:40:50.850968 mbapy-0.0.9/mbapy.egg-info/
--rw-rw-rw-   0        0        0     2177 2023-03-20 16:40:50.000000 mbapy-0.0.9/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-03-20 16:40:50.000000 mbapy-0.0.9/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 16:40:50.000000 mbapy-0.0.9/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      351 2023-03-20 16:40:50.000000 mbapy-0.0.9/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-03-20 16:40:50.000000 mbapy-0.0.9/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-20 16:40:50.882973 mbapy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2541 2023-03-20 16:37:52.000000 mbapy-0.0.9/setup.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1064 2023-05-20 15:53:20.000000 mbapy-0.1.0/LICENSE
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-22 09:51:42.624638 mbapy-0.1.0/PKG-INFO
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     5435 2023-05-22 08:19:05.000000 mbapy-0.1.0/README.md
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      559 2023-05-22 09:16:36.000000 mbapy-0.1.0/mbapy/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      387 2023-05-22 08:19:53.000000 mbapy-0.1.0/mbapy/__version__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3867 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/base.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/dl_torch/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      349 2023-05-22 09:18:31.000000 mbapy-0.1.0/mbapy/dl_torch/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    21852 2023-05-22 09:19:55.000000 mbapy-0.1.0/mbapy/dl_torch/bb.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4916 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/data.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     1015 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/hyper_search.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     4018 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/loss.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    12806 2023-05-22 09:17:48.000000 mbapy-0.1.0/mbapy/dl_torch/m.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/dl_torch/paper/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       17 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/dl_torch/paper/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2873 2023-05-22 08:47:43.000000 mbapy-0.1.0/mbapy/dl_torch/paper/bb.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9067 2023-05-22 09:48:08.000000 mbapy-0.1.0/mbapy/dl_torch/utils.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2306 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/file.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    14344 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/plot.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy/stats/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      512 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/__init__.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     3514 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/df.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)    18970 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/geography.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      727 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/stats/reg.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     9184 2023-05-22 07:21:40.000000 mbapy-0.1.0/mbapy/stats/test.py
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     8696 2023-05-20 15:53:20.000000 mbapy-0.1.0/mbapy/web.py
+drwxrwxr-x   0 bhm-bob   (1000) bhm-bob   (1000)        0 2023-05-22 09:51:42.624638 mbapy-0.1.0/mbapy.egg-info/
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     6186 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/PKG-INFO
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      599 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)        1 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)      379 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/requires.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       54 2023-05-22 09:51:42.000000 mbapy-0.1.0/mbapy.egg-info/top_level.txt
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)       38 2023-05-22 09:51:42.624638 mbapy-0.1.0/setup.cfg
+-rw-rw-r--   0 bhm-bob   (1000) bhm-bob   (1000)     2551 2023-05-22 08:22:08.000000 mbapy-0.1.0/setup.py
```

### Comparing `mbapy-0.0.9/LICENSE` & `mbapy-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 BHM-Bob
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 BHM-Bob
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `mbapy-0.0.9/mbapy/dl_torch/loss.py` & `mbapy-0.1.0/mbapy/dl_torch/loss.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-'''
-Author: BHM-Bob 2262029386@qq.com
-Date: 2023-03-21 00:13:11
-LastEditors: BHM-Bob
-LastEditTime: 2023-03-21 00:13:54
-Description: 
-'''
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class AsymmetricLossOptimized(nn.Module):
-    ''' https://github.com/Alibaba-MIIL/ASL/blob/main/src/loss_functions/losses.py \n
-    Notice - optimized version, minimizes memory allocation and gpu uploading,
-    favors inplace operations'''
-
-    def __init__(self, gamma_neg=4, gamma_pos=1, clip=0.05, eps=1e-8, disable_torch_grad_focal_loss=False):
-        super(AsymmetricLossOptimized, self).__init__()
-        self.gamma_neg = gamma_neg
-        self.gamma_pos = gamma_pos
-        self.clip = clip
-        self.disable_torch_grad_focal_loss = disable_torch_grad_focal_loss
-        self.eps = eps
-        # prevent memory allocation and gpu uploading every iteration, and encourages inplace operations
-        self.targets = self.anti_targets = self.xs_pos = self.xs_neg = self.asymmetric_w = self.loss = None
-    def forward(self, x: torch.Tensor, y: torch.Tensor):
-        """"
-        x: input logits
-        y: targets (multi-label binarized vector)
-        """
-        self.targets = y
-        self.anti_targets = 1 - y
-        # Calculating Probabilities
-        self.xs_pos = torch.sigmoid(x-0.5)
-        self.xs_neg = 1.0 - self.xs_pos
-        # Asymmetric Clipping
-        if self.clip is not None and self.clip > 0:
-            self.xs_neg.add_(self.clip).clamp_(max=1)
-        # Basic CE calculation
-        self.loss = self.targets * torch.log(self.xs_pos.clamp(min=self.eps))
-        self.loss.add_(self.anti_targets * torch.log(self.xs_neg.clamp(min=self.eps)))
-        # Asymmetric Focusing
-        if self.gamma_neg > 0 or self.gamma_pos > 0:
-            if self.disable_torch_grad_focal_loss:
-                torch.set_grad_enabled(False)
-            self.xs_pos = self.xs_pos * self.targets
-            self.xs_neg = self.xs_neg * self.anti_targets
-            self.asymmetric_w = torch.pow(1 - self.xs_pos - self.xs_neg,
-                                          self.gamma_pos * self.targets + self.gamma_neg * self.anti_targets)
-            if self.disable_torch_grad_focal_loss:
-                torch.set_grad_enabled(True)
-            self.loss *= self.asymmetric_w
-        # TODO : or mean ???
-        return -self.loss.sum()
-    
-class ASLSingleLabel(nn.Module):
-    '''
-    https://github.com/Alibaba-MIIL/ASL/blob/main/src/loss_functions/losses.py \n
-    This loss is intended for single-label classification problems
-    '''
-    def __init__(self, gamma_pos=0, gamma_neg=4, eps: float = 0.1, reduction='mean'):
-        super(ASLSingleLabel, self).__init__()
-
-        self.eps = eps
-        self.logsoftmax = nn.LogSoftmax(dim=-1)
-        self.targets_classes = []
-        self.gamma_pos = gamma_pos
-        self.gamma_neg = gamma_neg
-        self.reduction = reduction
-    def forward(self, inputs, target):
-        '''
-        "input" dimensions: - (batch_size,number_classes)
-        "target" dimensions: - (batch_size)
-        '''
-        num_classes = inputs.size()[-1]
-        log_preds = self.logsoftmax(inputs)
-        self.targets_classes = torch.zeros_like(inputs).scatter_(1, target.long().unsqueeze(1), 1)
-        # ASL weights
-        targets = self.targets_classes
-        anti_targets = 1 - targets
-        xs_pos = torch.exp(log_preds)
-        xs_neg = 1 - xs_pos
-        xs_pos = xs_pos * targets
-        xs_neg = xs_neg * anti_targets
-        asymmetric_w = torch.pow(1 - xs_pos - xs_neg,
-                                 self.gamma_pos * targets + self.gamma_neg * anti_targets)
-        log_preds = log_preds * asymmetric_w
-        if self.eps > 0:  # label smoothing
-            self.targets_classes = self.targets_classes.mul(1 - self.eps).add(self.eps / num_classes)
-        # loss calculation
-        loss = - self.targets_classes.mul(log_preds)
-        loss = loss.sum(dim=-1)
-        if self.reduction == 'mean':
-            loss = loss.mean()
+'''
+Author: BHM-Bob 2262029386@qq.com
+Date: 2023-03-21 00:13:11
+LastEditors: BHM-Bob
+LastEditTime: 2023-03-21 00:13:54
+Description: 
+'''
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class AsymmetricLossOptimized(nn.Module):
+    ''' https://github.com/Alibaba-MIIL/ASL/blob/main/src/loss_functions/losses.py \n
+    Notice - optimized version, minimizes memory allocation and gpu uploading,
+    favors inplace operations'''
+
+    def __init__(self, gamma_neg=4, gamma_pos=1, clip=0.05, eps=1e-8, disable_torch_grad_focal_loss=False):
+        super(AsymmetricLossOptimized, self).__init__()
+        self.gamma_neg = gamma_neg
+        self.gamma_pos = gamma_pos
+        self.clip = clip
+        self.disable_torch_grad_focal_loss = disable_torch_grad_focal_loss
+        self.eps = eps
+        # prevent memory allocation and gpu uploading every iteration, and encourages inplace operations
+        self.targets = self.anti_targets = self.xs_pos = self.xs_neg = self.asymmetric_w = self.loss = None
+    def forward(self, x: torch.Tensor, y: torch.Tensor):
+        """"
+        x: input logits
+        y: targets (multi-label binarized vector)
+        """
+        self.targets = y
+        self.anti_targets = 1 - y
+        # Calculating Probabilities
+        self.xs_pos = torch.sigmoid(x-0.5)
+        self.xs_neg = 1.0 - self.xs_pos
+        # Asymmetric Clipping
+        if self.clip is not None and self.clip > 0:
+            self.xs_neg.add_(self.clip).clamp_(max=1)
+        # Basic CE calculation
+        self.loss = self.targets * torch.log(self.xs_pos.clamp(min=self.eps))
+        self.loss.add_(self.anti_targets * torch.log(self.xs_neg.clamp(min=self.eps)))
+        # Asymmetric Focusing
+        if self.gamma_neg > 0 or self.gamma_pos > 0:
+            if self.disable_torch_grad_focal_loss:
+                torch.set_grad_enabled(False)
+            self.xs_pos = self.xs_pos * self.targets
+            self.xs_neg = self.xs_neg * self.anti_targets
+            self.asymmetric_w = torch.pow(1 - self.xs_pos - self.xs_neg,
+                                          self.gamma_pos * self.targets + self.gamma_neg * self.anti_targets)
+            if self.disable_torch_grad_focal_loss:
+                torch.set_grad_enabled(True)
+            self.loss *= self.asymmetric_w
+        # TODO : or mean ???
+        return -self.loss.sum()
+    
+class ASLSingleLabel(nn.Module):
+    '''
+    https://github.com/Alibaba-MIIL/ASL/blob/main/src/loss_functions/losses.py \n
+    This loss is intended for single-label classification problems
+    '''
+    def __init__(self, gamma_pos=0, gamma_neg=4, eps: float = 0.1, reduction='mean'):
+        super(ASLSingleLabel, self).__init__()
+
+        self.eps = eps
+        self.logsoftmax = nn.LogSoftmax(dim=-1)
+        self.targets_classes = []
+        self.gamma_pos = gamma_pos
+        self.gamma_neg = gamma_neg
+        self.reduction = reduction
+    def forward(self, inputs, target):
+        '''
+        "input" dimensions: - (batch_size,number_classes)
+        "target" dimensions: - (batch_size)
+        '''
+        num_classes = inputs.size()[-1]
+        log_preds = self.logsoftmax(inputs)
+        self.targets_classes = torch.zeros_like(inputs).scatter_(1, target.long().unsqueeze(1), 1)
+        # ASL weights
+        targets = self.targets_classes
+        anti_targets = 1 - targets
+        xs_pos = torch.exp(log_preds)
+        xs_neg = 1 - xs_pos
+        xs_pos = xs_pos * targets
+        xs_neg = xs_neg * anti_targets
+        asymmetric_w = torch.pow(1 - xs_pos - xs_neg,
+                                 self.gamma_pos * targets + self.gamma_neg * anti_targets)
+        log_preds = log_preds * asymmetric_w
+        if self.eps > 0:  # label smoothing
+            self.targets_classes = self.targets_classes.mul(1 - self.eps).add(self.eps / num_classes)
+        # loss calculation
+        loss = - self.targets_classes.mul(log_preds)
+        loss = loss.sum(dim=-1)
+        if self.reduction == 'mean':
+            loss = loss.mean()
         return
```

### Comparing `mbapy-0.0.9/mbapy/dl_torch/utils.py` & `mbapy-0.1.0/mbapy/dl_torch/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,256 +1,271 @@
-import atexit
-import glob
-import os
-import time
-from queue import Queue
-
-import math
-import torch
-import torch.nn as nn
-
-import mbapy.dl_torch
-import mbapy.base as base
-from mbapy.file import save_json, read_json
-
-
-if mbapy.dl_torch.Params['USE_VIZDOM']:
-    import visdom
-    viz = visdom.Visdom()
-    vizRecord = []
-
-class Mprint:
-    """logging tools"""
-    def __init__(self, path="mp.txt", mode="lazy", cleanFirst=True):
-        self.path = path
-        self.mode = mode
-        self.topString = " "
-        self.string = ""
-
-        if cleanFirst:
-            with open(path, "w") as f:
-                f.write("Mprint : cleanFirst\n")
-
-    def mprint(self, *args):
-        string = '[{''} - {''}] '.format(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), self.topString)
-        for item in args:
-            if type(item) != "":
-                item = str(item)
-            string += item + " "
-
-        print(string)
-
-        if self.mode != "lazy":
-            with open(self.path, "a+") as f:
-                f.write(string + "\n")
-        else:
-            self.string += string + "\n"
-
-    def logOnly(self, *args):
-        string = '[{''} - {''}] '.format(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), self.topString)
-        for item in args:
-            if type(item) != "":
-                item = str(item)
-            string += item + " "
-
-        if self.mode != "lazy":
-            with open(self.path, "a+") as f:
-                f.write(string + "\n")
-        else:
-            self.string += string + "\n"
-
-    def exit(self):
-        with open(self.path, "a+") as f:
-            f.write(self.string)
-            
-class GlobalSettings(base.MyArgs):
-    def __init__(self, mp:Mprint, modelRoot:str):
-        self.read = {}# for data reading
-        self.model = {
-            'model':None,
-            'arch':None,
-            'lr' : 0.01,
-            'in_shape' : [64, 128, 128, 3],
-            'out_dim' : [64, 128], 
-        }
-        self.input = {
-            'load_db_ratio' : 1,
-            'batch_size' : 64,
-            'single_shape':[128, 128, 3]
-        }
-        # default var
-        self.epochs = 1500
-        self.print_freq = 40
-        self.test_freq = 5
-        self.momentum = 0.9
-        self.weight_decay = 1e-4        
-        self.seed = 777
-        self.start_epoch = 0
-        self.moco_m = 0.999
-        self.moco_k = 3200
-        self.byolq_k = 3200
-        self.moco_t = 0.07
-        self.cos = True        
-        # fixed var
-        self.paths = {}
-        self.data = ''
-        self.modelRoot = modelRoot
-        self.resumePathList = glob.glob(os.path.join(modelRoot,'*.tar'))
-        self.resume = self.resumePathList[0] if len(self.resumePathList) > 0 else 'None'
-        # other
-        self.mp = mp#Mp
-    def toDict(self, printOut = False, mp = None):
-        dic = {}
-        for attr in vars(self):
-            dic[attr] = getattr(self,attr)
-        if printOut and mp is not None:
-            [ mp.mprint(attr,' : ',dic[attr]) for attr in dic.keys()]
-        elif printOut:
-            [ print(attr,' : ',dic[attr]) for attr in dic.keys()]
-        return dic
-
-def init_model_parameter(model):
-    # model initilization
-    for m in model.modules():
-        if isinstance(m, nn.Conv2d) or isinstance(m, nn.Conv1d):
-            nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='leaky_relu')
-        elif isinstance(m, nn.BatchNorm2d) or isinstance(m, nn.BatchNorm1d):
-            nn.init.constant_(m.weight, 1)
-            nn.init.constant_(m.bias, 0)
-    return model
-
-def adjust_learning_rate(optimizer, now_epoch, args):
-    """Decay the learning rate based on schedule
-    args"""
-    lr = args.lr
-    if args.cos:  # cosine lr schedule
-        lr *= 0.5 * (1. + math.cos(math.pi * now_epoch / args.epochs))
-    else:  # stepwise lr schedule
-        for milestone in args.schedule:
-            lr *= 0.1 if now_epoch >= milestone else 1.
-    for param_group in optimizer.param_groups:
-        param_group['lr'] = lr
-
-def format_secs(sumSecs):
-    sumHs = int(sumSecs//3600)
-    sumMs = int((sumSecs-sumHs*3600)//60)
-    sumSs = int(sumSecs-sumHs*3600-sumMs*60)
-    return sumHs, sumMs, sumSs
-
-class AverageMeter(object):
-    """from FAIR or MAIR 's MoCo
-    Computes and stores the average and current value"""
-
-    def __init__(self, name, fmt=":f"):
-        self.name = name
-        self.fmt = fmt
-        self.reset()
-
-    def reset(self):
-        self.val = 0
-        self.avg = 0.0
-        self.sum = 0
-        self.count = 0
-
-    def update(self, val, n=1):
-        self.val = val
-        self.sum += val * n
-        self.count += n
-        self.avg = self.sum / self.count
-
-    def __str__(self):
-        fmtstr = "{name} {val" + self.fmt + "} ({avg" + self.fmt + "})"
-        return fmtstr.format(**self.__dict__)
-    
-class ProgressMeter(object):
-    """from FAIR or MAIR 's MoCo"""
-    def __init__(self, num_batches, meters, prefix="", mp = None):
-        self.batch_fmtstr = self._get_batch_fmtstr(num_batches)
-        self.meters = meters
-        self.prefix = prefix
-        self.mp = mp
-
-    def display(self, batch):
-        entries = [self.prefix + self.batch_fmtstr.format(batch)]
-        entries += [str(meter) for meter in self.meters]
-        if self.mp is None:
-            print("\t".join(entries))
-        else:
-            self.mp.mprint("\t".join(entries))
-
-    def _get_batch_fmtstr(self, num_batches):
-        num_digits = len(str(num_batches // 1))
-        fmt = "{:" + str(num_digits) + "d}"
-        return "[" + fmt + "/" + fmt.format(num_batches) + "]"
-    
-class TimeLast(object):
-    def __init__(self):
-        self.lastTime = time.time()
-
-    def update(self, leftTasks):
-        usedTime = time.time() - self.lastTime
-        self.lastTime = time.time()
-        sumLastTime = leftTasks * usedTime
-        return sumLastTime            
-            
-def save_checkpoint(epoch, args:GlobalSettings, model, optimizer, loss, other:dict, tailName:str):
-    state = {
-        "epoch": epoch + 1,
-        "arch": args.arch,
-        "state_dict": model.state_dict(),
-        "optimizer": optimizer.state_dict(),
-        "loss": loss,
-        "args":args.toDict(),
-    }
-    filename = os.path.join(args.modelRoot,
-                            f"checkpoint_{tailName:s}_{time.asctime(time.localtime()).replace(':', '-'):s}.pth.tar")
-    torch.save(state.update(other), filename)
-
-def resume(args, model, optimizer, other:dict = {}):
-    if args.resume and os.path.isfile(args.resume):
-        args.mp.mprint("=> loading checkpoint '{}'".format(args.resume))
-        if args.gpu is None:
-            checkpoint = torch.load(args.resume)
-        else:
-            # Map model to be loaded to specified single gpu.
-            # loc = "cuda:{}".format(args.gpu)
-            checkpoint = torch.load(args.resume)  # , map_location=loc)
-        args.start_epoch = checkpoint["epoch"]
-        model.load_state_dict(checkpoint["state_dict"])
-        optimizer.load_state_dict(checkpoint["optimizer"])
-        old_losses = checkpoint["loss"]
-        args.mp.mprint(
-            "=> loaded checkpoint '{}' (epoch {})".format(
-                args.resume, checkpoint["epoch"]
-            )
-        )
-        if other:
-            other.update()
-            for key in other.keys():
-                if key in checkpoint:
-                    other[key] = checkpoint[key]
-        return model, optimizer, old_losses
-    else:
-        args.mp.mprint("=> no checkpoint found at '{}'".format(args.resume))
-        args.mp.logOnly(str(model))
-        return model, optimizer, 0
-    
-if mbapy.dl_torch.Params['USE_VIZDOM']:
-    def VizLine(Y:float, X:float, win:str, title:str = 'N', name:str = 'N',
-                update:str = 'append', opts:dict = {}):
-        global vizRecord
-        if opts:
-            viz.line(Y = [Y],X = [X],
-                    win=win, update=update,opts =  opts)
-            vizRecord.append([Y, X, win, opts['title'], name, update, opts])
-        else:
-            viz.line(Y = [Y],X = [X],name = name,
-                    win=win, update=update,opts =  dict(title = title))
-            opts = {'title' : title}
-            vizRecord.append([Y, X, win, title, name, update, opts])
-        pass
-
-    def re_viz_from_json_record(path):
-        if os.path.isfile(path):
-            for log in read_json(path):
-                viz.line(Y = [log[0]], X = [log[1]], win = log[2], name = log[4],
+import atexit
+import glob
+import os
+import time
+from queue import Queue
+
+import math
+import numpy as np
+import torch
+import torch.nn as nn
+
+from ..base import MyArgs
+from ..file import save_json, read_json
+
+_Params = {
+    'USE_VIZDOM':False,
+}
+
+if _Params['USE_VIZDOM']:
+    import visdom
+    viz = visdom.Visdom()
+    vizRecord = []
+
+class Mprint:
+    """logging tools"""
+    def __init__(self, path="log.txt", mode="lazy", cleanFirst=True):
+        self.path = path
+        self.mode = mode
+        self.topString = " "
+        self.string = ""
+
+        if cleanFirst:
+            with open(path, "w") as f:
+                f.write("Mprint : cleanFirst\n")
+
+    def mprint(self, *args):
+        string = '[{''} - {''}] '.format(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), self.topString)
+        for item in args:
+            if type(item) != "":
+                item = str(item)
+            string += item + " "
+
+        print(string)
+
+        if self.mode != "lazy":
+            with open(self.path, "a+") as f:
+                f.write(string + "\n")
+        else:
+            self.string += string + "\n"
+
+    def logOnly(self, *args):
+        string = '[{''} - {''}] '.format(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), self.topString)
+        for item in args:
+            if type(item) != "":
+                item = str(item)
+            string += item + " "
+
+        if self.mode != "lazy":
+            with open(self.path, "a+") as f:
+                f.write(string + "\n")
+        else:
+            self.string += string + "\n"
+
+    def exit(self):
+        with open(self.path, "a+") as f:
+            f.write(self.string)
+            
+    def __str__(self):
+        return f'path={self.path:s}, mode={self.mode:s}, topString={self.topString:s}'
+            
+class GlobalSettings(MyArgs):
+    def __init__(self, mp:Mprint, model_root:str):
+        # data loading
+        self.read = {}# for data reading
+        self.batch_size =  64
+        self.load_shape = [3, 128, 128]
+        # model
+        self.model = None
+        self.arch = None
+        self.lr =  0.01
+        self.in_shape =  [64, 3, 128, 128]
+        self.out_shape =  [64, 128]
+        self.load_db_ratio =  1
+        # default var
+        self.epochs = 1500
+        self.print_freq = 40
+        self.test_freq = 5
+        self.momentum = 0.9
+        self.weight_decay = 1e-4        
+        self.seed = 777
+        self.start_epoch = 0
+        self.moco_m = 0.999
+        self.moco_k = 3200
+        self.byolq_k = 3200
+        self.moco_t = 0.07
+        self.cos = True        
+        # fixed var
+        self.paths = {}
+        self.data = ''
+        self.model_root = model_root
+        self.resume_paths = glob.glob(os.path.join(self.model_root,'*.tar'))
+        self.resume = self.resume_paths[0] if len(self.resume_paths) > 0 else 'None'
+        # other
+        self.mp = mp#Mp        
+        if self.seed is not None:
+            import random
+            import torch.backends.cudnn as cudnn
+            random.seed(self.seed)
+            torch.manual_seed(self.seed)
+            cudnn.deterministic = True
+    def toDict(self, printOut = False, mp = None):
+        dic = {}
+        for attr in vars(self):
+            dic[attr] = getattr(self,attr)
+        if printOut and mp is not None:
+            [ mp.mprint(attr,' : ',dic[attr]) for attr in dic.keys()]
+        elif printOut:
+            [ print(attr,' : ',dic[attr]) for attr in dic.keys()]
+        return dic
+    def set_resume(self):
+        self.resume_paths = glob.glob(os.path.join(self.model_root,'*.tar'))
+        self.resume = self.resume_paths[0] if len(self.resume_paths) > 0 else 'None'
+
+def init_model_parameter(model):
+    # model initilization
+    for m in model.modules():
+        if isinstance(m, nn.Conv2d) or isinstance(m, nn.Conv1d):
+            nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='leaky_relu')
+        elif isinstance(m, nn.BatchNorm2d) or isinstance(m, nn.BatchNorm1d):
+            nn.init.constant_(m.weight, 1)
+            nn.init.constant_(m.bias, 0)
+    return model
+
+def adjust_learning_rate(optimizer, now_epoch, args):
+    """Decay the learning rate based on schedule
+    args"""
+    lr = args.lr
+    if args.cos:  # cosine lr schedule
+        lr *= 0.5 * (1. + math.cos(math.pi * now_epoch / args.epochs))
+    else:  # stepwise lr schedule
+        for milestone in args.schedule:
+            lr *= 0.1 if now_epoch >= milestone else 1.
+    for param_group in optimizer.param_groups:
+        param_group['lr'] = lr
+
+def format_secs(sumSecs):
+    sumHs = int(sumSecs//3600)
+    sumMs = int((sumSecs-sumHs*3600)//60)
+    sumSs = int(sumSecs-sumHs*3600-sumMs*60)
+    return sumHs, sumMs, sumSs
+
+class AverageMeter(object):
+    """
+    Computes and stores the average and current value
+    from FAIR or MAIR 's MoCo
+    """
+    def __init__(self, name, fmt=":f"):
+        self.name = name
+        self.fmt = fmt
+        self.reset()
+
+    def reset(self):
+        self.val = 0
+        self.avg = 0.0
+        self.sum = 0
+        self.count = 0
+
+    def update(self, val, n=1):
+        self.val = val
+        self.sum += val * n
+        self.count += n
+        self.avg = self.sum / self.count
+
+    def __str__(self):
+        fmtstr = "{name} {val" + self.fmt + "} ({avg" + self.fmt + "})"
+        return fmtstr.format(**self.__dict__)
+    
+class ProgressMeter(object):
+    """from FAIR or MAIR 's MoCo"""
+    def __init__(self, num_batches, meters, prefix="", mp = None):
+        self.batch_fmtstr = self._get_batch_fmtstr(num_batches)
+        self.meters = meters
+        self.prefix = prefix
+        self.mp = mp
+
+    def display(self, batch):
+        entries = [self.prefix + self.batch_fmtstr.format(batch)]
+        entries += [str(meter) for meter in self.meters]
+        if self.mp is None:
+            print("\t".join(entries))
+        else:
+            self.mp.mprint("\t".join(entries))
+
+    def _get_batch_fmtstr(self, num_batches):
+        num_digits = len(str(num_batches // 1))
+        fmt = "{:" + str(num_digits) + "d}"
+        return "[" + fmt + "/" + fmt.format(num_batches) + "]"
+    
+class TimeLast(object):
+    def __init__(self):
+        self.last_time = time.time()
+
+    def update(self, left_tasks:int, just_done_tasks:int = 1):
+        used_time = time.time() - self.last_time
+        self.last_time = time.time()
+        sum_last_time = left_tasks * used_time / just_done_tasks
+        return sum_last_time            
+            
+def save_checkpoint(epoch, args:GlobalSettings, model, optimizer, loss, other:dict, tailName:str):
+    state = {
+        "epoch": epoch + 1,
+        "arch": args.arch,
+        "state_dict": model.state_dict(),
+        "optimizer": optimizer.state_dict(),
+        "loss": loss,
+        "args":args.toDict(),
+    }
+    state.update(other)
+    filename = os.path.join(args.model_oot,
+                            f"checkpoint_{tailName:s}_{time.asctime(time.localtime()).replace(':', '-'):s}.pth.tar")
+    torch.save(state, filename)
+
+def resume(args, model, optimizer, other:dict = {}):
+    if args.resume and os.path.isfile(args.resume):
+        args.mp.mprint("=> loading checkpoint '{}'".format(args.resume))
+        if args.gpu is None:
+            checkpoint = torch.load(args.resume)
+        else:
+            # Map model to be loaded to specified single gpu.
+            # loc = "cuda:{}".format(args.gpu)
+            checkpoint = torch.load(args.resume)  # , map_location=loc)
+        args.start_epoch = checkpoint["epoch"]
+        model.load_state_dict(checkpoint["state_dict"])
+        optimizer.load_state_dict(checkpoint["optimizer"])
+        old_losses = checkpoint["loss"]
+        args.mp.mprint(
+            "=> loaded checkpoint '{}' (epoch {})".format(
+                args.resume, checkpoint["epoch"]
+            )
+        )
+        if other:
+            other.update()
+            for key in other.keys():
+                if key in checkpoint:
+                    other[key] = checkpoint[key]
+        return model, optimizer, old_losses
+    else:
+        args.mp.mprint("=> no checkpoint found at '{}'".format(args.resume))
+        args.mp.logOnly(str(model))
+        return model, optimizer, 0
+    
+if _Params['USE_VIZDOM']:
+    def VizLine(Y:float, X:float, win:str, title:str = 'N', name:str = 'N',
+                update:str = 'append', opts:dict = {}):
+        global vizRecord
+        if opts:
+            viz.line(Y = [Y],X = [X],
+                    win=win, update=update,opts =  opts)
+            vizRecord.append([Y, X, win, opts['title'], name, update, opts])
+        else:
+            viz.line(Y = [Y],X = [X],name = name,
+                    win=win, update=update,opts =  dict(title = title))
+            opts = {'title' : title}
+            vizRecord.append([Y, X, win, title, name, update, opts])
+        pass
+
+    def re_viz_from_json_record(path):
+        if os.path.isfile(path):
+            for log in read_json(path):
+                viz.line(Y = [log[0]], X = [log[1]], win = log[2], name = log[4],
                         update = log[5],opts =  log[6])
```

### Comparing `mbapy-0.0.9/mbapy/file.py` & `mbapy-0.1.0/mbapy/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,63 @@
-'''
-Author: BHM-Bob 2262029386@qq.com
-Date: 2022-11-01 19:09:54
-LastEditors: BHM-Bob
-LastEditTime: 2023-03-21 00:35:24
-Description: 
-'''
-import chardet
-import json
-import os
-
-import pandas as pd
-
-
-def detect_byte_coding(bits:bytes):
-    adchar = chardet.detect(bits[:(1000 if len(bits) > 1000 else len(bits))])['encoding']
-    if adchar == 'gbk' or adchar == 'GBK' or adchar == 'GB2312':
-        true_text = bits.decode('GB2312', "ignore")
-    else:
-        true_text = bits.decode('utf-8', "ignore")
-    return true_text
-
-def save_json(path:str, obj, encoding:str = 'utf-8', forceUpdate = True):
-    if forceUpdate or not os.path.isfile(path):
-        json_str = json.dumps(obj, indent=1)
-        with open(path, 'w' ,encoding=encoding, errors='ignore') as json_file:
-            json_file.write(json_str)
-def read_json(path:str, encoding:str = 'utf-8', invalidPathReturn = None):
-    if os.path.isfile(path):
-        with open(path, 'r' ,encoding=encoding, errors='ignore') as json_file:
-            json_str = json_file.read()
-        return json.loads(json_str)
-    return invalidPathReturn
-def save_excel(path:str, obj:list[list[str]], columns:list[str], encoding:str = 'utf-8', forceUpdate = True):
-    if forceUpdate or not os.path.isfile(path):
-        df = pd.DataFrame(obj, columns=columns)
-        df.to_excel(path, encoding = encoding)
-def read_excel(path:str, ignoreHead:bool = True,
-                  ignoreFirstCol:bool = True, invalidPathReturn = None):
-    if os.path.isfile(path):
-        df = pd.read_excel(path, )
-        return df
-    return invalidPathReturn
+'''
+Author: BHM-Bob 2262029386@qq.com
+Date: 2022-11-01 19:09:54
+LastEditors: BHM-Bob
+LastEditTime: 2023-04-27 13:01:20
+Description: 
+'''
+import chardet
+import json
+import os
+
+import pandas as pd
+
+
+def detect_byte_coding(bits:bytes):
+    adchar = chardet.detect(bits[:(1000 if len(bits) > 1000 else len(bits))])['encoding']
+    if adchar == 'gbk' or adchar == 'GBK' or adchar == 'GB2312':
+        true_text = bits.decode('GB2312', "ignore")
+    else:
+        true_text = bits.decode('utf-8', "ignore")
+    return true_text
+
+def save_json(path:str, obj, encoding:str = 'utf-8', forceUpdate = True):
+    if forceUpdate or not os.path.isfile(path):
+        json_str = json.dumps(obj, indent=1)
+        with open(path, 'w' ,encoding=encoding, errors='ignore') as json_file:
+            json_file.write(json_str)
+def read_json(path:str, encoding:str = 'utf-8', invalidPathReturn = None):
+    if os.path.isfile(path):
+        with open(path, 'r' ,encoding=encoding, errors='ignore') as json_file:
+            json_str = json_file.read()
+        return json.loads(json_str)
+    return invalidPathReturn
+
+def save_excel(path:str, obj:list[list[str]], columns:list[str], encoding:str = 'utf-8', forceUpdate = True):
+    if forceUpdate or not os.path.isfile(path):
+        df = pd.DataFrame(obj, columns=columns)
+        df.to_excel(path, encoding = encoding)
+def read_excel(path:str, ignoreHead:bool = True,
+                  ignoreFirstCol:bool = True, invalidPathReturn = None):
+    if os.path.isfile(path):
+        df = pd.read_excel(path, )
+        return df
+    return invalidPathReturn
+
+def write_sheets(path:str, sheets:dict[str, pd.DataFrame]):
+    with pd.ExcelWriter(path) as f:
+        for sheet in sheets:
+            sheets[sheet].to_excel(path, sheet_name=sheet)    
+
+def update_excel(path:str, sheets:dict[str, pd.DataFrame] = None):
+    if os.path.isfile(path):
+        dfs = pd.read_excel(path, sheet_name=None)
+        if sheets is None:
+            return dfs
+        else:
+            for sheet in sheets:
+                if isinstance(sheets[sheet], pd.DataFrame):
+                    dfs[sheet] = sheets[sheet]
+            write_sheets(path, dfs)
+    elif sheets is not None:
+        print(f'path is not a file : {path:s}, writing sheets to the file of path')
+        write_sheets(path, sheets)
```

### Comparing `mbapy-0.0.9/mbapy/plot.py` & `mbapy-0.1.0/mbapy/plot.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,247 +1,319 @@
-import itertools
-import sys
-from functools import wraps
-
-import matplotlib.patches as patches
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
-import numpy as np
-import pandas as pd
-import seaborn as sns
-from mpl_toolkits import axisartist
-from mpl_toolkits.axes_grid1 import host_subplot
-
-from mbapy.base import get_wanted_args
-
-# plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文
-plt.rcParams["font.family"] = 'Times New Roman'
-plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
-
-# TODO : not use itertools.product
-def pro_bar_data(factors:list[str], tags:list[str], df:pd.DataFrame):
-    """
-    cacu mean and SE for each combinations of facotors\n
-    data should be like this:\n
-    | factor1 | factor2 | y1 | y2 |...\n
-    |  f1_1   |   f2_1  |2.1 |-2  |...\n
-    after process\n
-    | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
-    |  f1_1   |   f2_1  |2.1       |   -2      |   32           |...\n
-    """
-    if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]
-    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-    ndf = [factors.copy()]
-    for tag in tags:
-        ndf[0] += [tag, tag+'_SE', tag+'_N']
-    for factorCombi in itertools.product(*factor_contents):
-        factorMask = np.array(df[factors[0]] == factorCombi[0])
-        for i in range(1, len(factors)):
-            factorMask &= np.array(df[factors[i]] == factorCombi[i])
-        if(factorMask.sum() > 0):
-            line = []
-            for idx, tag in enumerate(tags):
-                values = np.array(df.loc[factorMask, [tag]])
-                line.append(values.mean())
-                line.append(values.std(ddof = 1)/np.sqrt(values.shape[0]))
-                line.append(values.shape[0])
-            ndf.append(list(factorCombi) + line)
-    return pd.DataFrame(ndf[1:], columns=ndf[0])
-
-def pro_bar_data_R(factors:list[str], tags:list[str], df:pd.DataFrame, suffixs:list[str], **kwargs):
-    """
-    wrapper\n
-    @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
-    def plot_func(values, **kwargs):
-        return produced vars in list format whose length equal to len(suffix)
-    """
-    def ret_wrapper(core_func):
-        def core_wrapper(**kwargs):
-            nonlocal tags
-            if len(tags) == 0:
-                tags = list(df.columns)[len(factors):]
-            factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-            ndf = [factors.copy()]
-            for tag in tags:
-                for suffix in suffixs:
-                    ndf[0] += [tag+suffix]
-            for factorCombi in itertools.product(*factor_contents):
-                factorMask = np.array(df[factors[0]] == factorCombi[0])
-                for i in range(1, len(factors)):
-                    factorMask &= np.array(df[factors[i]] == factorCombi[i])
-                if(factorMask.sum() > 0):
-                    line = []
-                    for idx, tag in enumerate(tags):
-                        values = np.array(df.loc[factorMask, [tag]])
-                        ret_line = core_func(values)
-                        assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
-                        line += ret_line
-                    ndf.append(list(factorCombi) + line)
-            return pd.DataFrame(ndf[1:], columns=ndf[0])
-        return core_wrapper
-    return ret_wrapper
-
-def get_df_data(factors:dict[str, list[str]], tags:list[str], df:pd.DataFrame,
-                include_factors:bool = True):
-    #sub_df = ndf.loc[(ndf['size'] == size1) & (ndf['light'] == light1), ['c', 'w', 'SE']]
-    #sub_df = get_df_data([{'size':[size1], 'light':[light1]}, ['c', 'w', 'SE'])
-    def update_mask(mask, other:np.ndarray, method:str = '&'):
-        return other if mask is None else (mask&other if method == '&' else mask|other)
-    if include_factors:
-        tags = list(factors.keys()) + tags
-    mask = None
-    for factor_name in factors:
-        sub_mask = None
-        for sub_factor in factors[factor_name]:
-            sub_mask = update_mask(sub_mask, np.array(df[factor_name] == sub_factor), '|')
-        mask = update_mask(mask, sub_mask, '&')
-    return df.loc[mask, tags]
-
-def sort_df_factors(factors:list[str], tags:list[str], df:pd.DataFrame):
-    """UnTested
-    sort each combinations of facotors\n
-    data should be like this:\n
-    | factor1 | factor2 | y1 | y2 |...\n
-    |  f1_1   |   f2_1  |2.1 |-2  |...\n
-    |  f1_1   |   f2_2  |2.1 |-2  |...\n
-    ...\n
-    after sort if given facotors=['factor2', 'factor1']\n
-    | factor2 | factor1 | y1 | y2 |...\n
-    |  f2_1   |   f1_1  |2.1 |-2  |...\n
-    |  f2_1   |   f1_2  |2.1 |-2  |...\n
-    ...\n
-    """
-    if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]
-    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-    ndf = [factors.copy()]
-    ndf[0] += tags
-    for factorCombi in itertools.product(*factor_contents):
-        factorMask = df[factors[0]] == factorCombi[0]
-        for i in range(1, len(factors)):
-            factorMask &= df[factors[i]] == factorCombi[i]
-        ndf.append(list(factorCombi) + np.array(df.loc[factorMask, tags].values))
-    return pd.DataFrame(ndf[1:], columns=ndf[0])
-
-class AxisLable():
-    def __init__(self, name:str, hold_space:int = 1) -> None:
-        self.name = name
-        self.hold_space = hold_space
-    def add_space(self, space:int = 1):
-        self.hold_space += space
-
-def pro_hue_pos(factors:list[str], df:pd.DataFrame, width:float, bar_space:float):
-    xlabels, fc_old, pos = [ [] for _ in range(len(factors))], '', []
-    for f_i, f in enumerate(factors):
-        for fc_i, fc in enumerate(df[f]):
-            if fc != fc_old:
-                xlabels[f_i].append(AxisLable(fc))
-                fc_old = fc
-            else:
-                xlabels[f_i][-1].add_space()
-    xlabels.append([AxisLable(factors[-1], df.shape[0])])#master level has an extra total axis as x_title
-    for axis_idx in range(len(xlabels)):
-        pos.append([])
-        if axis_idx == 0:
-            st_pos = bar_space
-            for h_fc_idx in range(len(xlabels[axis_idx+1])):
-                sum_this_hue_bar = xlabels[axis_idx+1][h_fc_idx].hold_space
-                pos[axis_idx] += [st_pos+width*(i+0.5) for i in range(sum_this_hue_bar)]
-                st_pos += (sum_this_hue_bar*width+bar_space)
-        else:
-            st_pos = 0
-            for fc_idx in range(len(xlabels[axis_idx])):
-                this_hue_per = xlabels[axis_idx][fc_idx].hold_space / df.shape[0]
-                pos[axis_idx].append(st_pos+this_hue_per/2)
-                st_pos += this_hue_per
-    return xlabels, pos
-
-def plot_bar(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
-    """
-    stack bar plot with hue style\n
-    factors:[low_lever_factor, medium_lever_factor, ...] or just one
-    tags:[stack_low_y, stack_medium_y, ...] or just one
-    df:df from pro_bar_data or sort_df_factors
-        kwargs:
-    width = 0.4
-    bar_space = 0.2
-    xrotations = [0]*len(factors)
-    colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-    offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]
-    """
-    ax1 = host_subplot(111, axes_class=axisartist.Axes)
-    
-    if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]    
-    args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
-                            'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
-                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]},
-                            kwargs, locals())
-    args.xrotations.append(0)    
-    xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
-    bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
-    
-    for yIdx, yName in enumerate(tags):
-        ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=yName,
-                edgecolor='white', color=args.colors[yIdx])
-        bottom += df[yName]
-    ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
-    ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
-    plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
-    
-    axs = []
-    for idx, sub_pos in enumerate(pos[1:]):
-        axs.append(ax1.twiny())
-        axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
-        new_axisline = axs[-1].get_grid_helper().new_fixed_axis
-        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
-        plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1])
-        axs[-1].axis["top"].major_ticks.set_ticksize(0)
-        # TODO : do not work
-        axs[-1].axis["right"].major_ticks.set_ticksize(0)
-    
-    return np.array(pos[0]), ax1
-
-def plot_positional_hue(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
-    """
-    wrapper\n
-    support args: width, bar_space, xrotations, colors, offset, bottom\n
-    xlabels is in margs
-    @plot_positional_hue(['solution', 'type'], ['root', 'leaf'], ndf)\n
-    def plot_func(ax, x, y, label, label_idx, margs, **kwargs):
-        do something
-    """
-    def ret_wrapper(core_plot_func):
-        def core_wrapper(**kwargs):
-            ax1 = host_subplot(111, axes_class=axisartist.Axes)
-            nonlocal tags
-            if len(tags) == 0:
-                tags = list(df.columns)[len(factors):]    
-            margs = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
-                                    'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
-                                    'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]},
-                                   kwargs)
-            margs.xrotations.append(0)
-            xlabels, pos = pro_hue_pos(factors, df, margs.width, margs.bar_space)
-            margs.add_arg('xlabels', xlabels)
-            margs.add_arg('bottom', np.zeros(len(pos[0])), False)
-            if 'bottom' in kwargs:
-                del kwargs['bottom']
-            for yIdx, yName in enumerate(tags):
-                core_plot_func(ax1, pos[0], df[yName], yName, yIdx, margs, **kwargs)
-            ax1.set_xlim(0, pos[0][-1]+margs.bar_space+margs.width/2)
-            ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
-            plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=margs.xrotations[0])            
-            axs = []
-            for idx, sub_pos in enumerate(pos[1:]):
-                axs.append(ax1.twiny())
-                axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
-                new_axisline = axs[-1].get_grid_helper().new_fixed_axis
-                axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -margs.offset[idx]))
-                plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=margs.xrotations[idx+1])
-                axs[-1].axis["top"].major_ticks.set_ticksize(0)
-                # TODO : do not work
-                axs[-1].axis["right"].major_ticks.set_ticksize(0)            
-            return np.array(pos[0]), ax1
-        return core_wrapper
-    return ret_wrapper
+import itertools
+import sys
+from functools import wraps
+from typing import Union
+
+import matplotlib.patches as patches
+import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+import seaborn as sns
+from mpl_toolkits import axisartist
+from mpl_toolkits.axes_grid1 import host_subplot
+
+from mbapy.base import get_wanted_args
+
+# plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文
+plt.rcParams["font.family"] = 'Times New Roman'
+plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
+colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
+
+def rgb2hex(r, g, b):
+  return '#'+('{:02X}' * 3).format(r, g, b)
+def hex2rgb(hex:str):
+  return [int(hex[i:i+2], 16) for i in (1, 3, 5)]
+def rgbs2hexs(rgbs:list[tuple[float]]):
+    return list(map(lambda x : rgb2hex(*[int(x[i]*255) for i in range(3)]),
+                    rgbs))
+    
+def get_palette(n:int = 10, mode:Union[None, str] = None) -> list[str]:
+    """get a seq of hex colors    
+    Parameters
+    ----------
+    n: how many colors required
+    mode: kind of colors
+        - hls : [default] sns.color_palette('hls', n)
+        - green : sum 5 grenns
+        - pair : plt.get_cmap('tab20')
+        - None : plt.get_cmap('Set1') for n<=9 or plt.get_cmap('Set3') for n<= 12
+    """
+    assert n >= 1
+    if mode == 'hls':
+        return rgbs2hexs(sns.color_palette('hls', n))
+    if n <= 5 and mode == 'green':
+        return ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
+    elif n <= 9:
+        return rgbs2hexs(plt.get_cmap('Set1').colors)
+    elif n <= 12:
+        return rgbs2hexs(plt.get_cmap('Set3').colors)
+    elif n <= 20 and mode == 'pair':
+        return rgbs2hexs(plt.get_cmap('tab20').colors)
+    
+# TODO : not use itertools.product
+def pro_bar_data(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+    """
+    cacu mean and SE for each combinations of facotors\n
+    data should be like this:\n
+    | factor1 | factor2 | y1 | y2 |...\n
+    |  f1_1   |   f2_1  |2.1 |-2  |...\n
+    after process\n
+    | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
+    |  f1_1   |   f2_1  |2.1       |   -2      |   32           |...\n
+    kwargs:
+        min_sample_N:int : min N threshold(>=)
+    """
+    # kwargs
+    min_sample_N = 1 if 'min_sample_N' not in kwargs else kwargs['min_sample_N']
+    assert min_sample_N > 0, 'min_sample_N <= 0'
+    # pro
+    if len(tags) == 0:
+        tags = list(df.columns)[len(factors):]
+    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
+    ndf = [factors.copy()]
+    for tag in tags:
+        ndf[0] += [tag, tag+'_SE', tag+'_N']
+    for factorCombi in itertools.product(*factor_contents):
+        factorMask = np.array(df[factors[0]] == factorCombi[0])
+        for i in range(1, len(factors)):
+            factorMask &= np.array(df[factors[i]] == factorCombi[i])
+        if factorMask.sum() >= min_sample_N:
+            line = []
+            for idx, tag in enumerate(tags):
+                values = np.array(df.loc[factorMask, [tag]])
+                line.append(values.mean())
+                if values.shape[0] > 1:
+                    line.append(values.std(ddof = 1)/np.sqrt(values.shape[0]))
+                else:
+                    line.append(np.NaN)
+                line.append(values.shape[0])
+            ndf.append(list(factorCombi) + line)
+    return pd.DataFrame(ndf[1:], columns=ndf[0])
+
+def pro_bar_data_R(factors:list[str], tags:list[str], df:pd.DataFrame, suffixs:list[str], **kwargs):
+    """
+    wrapper\n
+    @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
+    def plot_func(values, **kwargs):
+        return produced vars in list format whose length equal to len(suffix)
+    """
+    def ret_wrapper(core_func):
+        def core_wrapper(**kwargs):
+            nonlocal tags
+            if len(tags) == 0:
+                tags = list(df.columns)[len(factors):]
+            factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
+            ndf = [factors.copy()]
+            for tag in tags:
+                for suffix in suffixs:
+                    ndf[0] += [tag+suffix]
+            for factorCombi in itertools.product(*factor_contents):
+                factorMask = np.array(df[factors[0]] == factorCombi[0])
+                for i in range(1, len(factors)):
+                    factorMask &= np.array(df[factors[i]] == factorCombi[i])
+                if(factorMask.sum() > 0):
+                    line = []
+                    for idx, tag in enumerate(tags):
+                        values = np.array(df.loc[factorMask, [tag]])
+                        ret_line = core_func(values)
+                        assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
+                        line += ret_line
+                    ndf.append(list(factorCombi) + line)
+            return pd.DataFrame(ndf[1:], columns=ndf[0])
+        return core_wrapper
+    return ret_wrapper
+
+def get_df_data(factors:dict[str, list[str]], tags:list[str], df:pd.DataFrame,
+                include_factors:bool = True):
+    #sub_df = ndf.loc[(ndf['size'] == size1) & (ndf['light'] == light1), ['c', 'w', 'SE']]
+    #sub_df = get_df_data([{'size':[size1], 'light':[light1]}, ['c', 'w', 'SE'])
+    def update_mask(mask, other:np.ndarray, method:str = '&'):
+        return other if mask is None else (mask&other if method == '&' else mask|other)
+    if len(tags) == 0:
+        tags = list(set(df.columns.to_list())-set(factors.keys()))
+    if include_factors:
+        tags = list(factors.keys()) + tags
+    mask = None
+    for factor_name in factors:
+        sub_mask = None
+        if len(factors[factor_name]) == 0:
+            # factors[factor_name] asigned with [], get all sub factors
+            factors[factor_name] = df[factor_name].unique().tolist()
+        for sub_factor in factors[factor_name]:
+            sub_mask = update_mask(sub_mask, np.array(df[factor_name] == sub_factor), '|')
+        mask = update_mask(mask, sub_mask, '&')
+    return df.loc[mask, tags]
+
+def sort_df_factors(factors:list[str], tags:list[str], df:pd.DataFrame):
+    """UnTested
+    sort each combinations of facotors\n
+    data should be like this:\n
+    | factor1 | factor2 | y1 | y2 |...\n
+    |  f1_1   |   f2_1  |2.1 |-2  |...\n
+    |  f1_1   |   f2_2  |2.1 |-2  |...\n
+    ...\n
+    after sort if given facotors=['factor2', 'factor1']\n
+    | factor2 | factor1 | y1 | y2 |...\n
+    |  f2_1   |   f1_1  |2.1 |-2  |...\n
+    |  f2_1   |   f1_2  |2.1 |-2  |...\n
+    ...\n
+    """
+    if len(tags) == 0:
+        tags = list(df.columns)[len(factors):]
+    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
+    ndf = [factors.copy()]
+    ndf[0] += tags
+    for factorCombi in itertools.product(*factor_contents):
+        factorMask = df[factors[0]] == factorCombi[0]
+        for i in range(1, len(factors)):
+            factorMask &= df[factors[i]] == factorCombi[i]
+        ndf.append(list(factorCombi) + np.array(df.loc[factorMask, tags].values))
+    return pd.DataFrame(ndf[1:], columns=ndf[0])
+
+class AxisLable():
+    def __init__(self, name:str, hold_space:int = 1) -> None:
+        self.name = name
+        self.hold_space = hold_space
+    def add_space(self, space:int = 1):
+        self.hold_space += space
+
+def pro_hue_pos(factors:list[str], df:pd.DataFrame, width:float, bar_space:float):
+    xlabels, fc_old, pos = [ [] for _ in range(len(factors))], '', []
+    for f_i, f in enumerate(factors):
+        for fc_i, fc in enumerate(df[f]):
+            if fc != fc_old:
+                xlabels[f_i].append(AxisLable(fc))
+                fc_old = fc
+            else:
+                xlabels[f_i][-1].add_space()
+    xlabels.append([AxisLable(factors[-1], df.shape[0])])#master level has an extra total axis as x_title
+    for axis_idx in range(len(xlabels)):
+        pos.append([])
+        if axis_idx == 0:
+            st_pos = bar_space
+            for h_fc_idx in range(len(xlabels[axis_idx+1])):
+                sum_this_hue_bar = xlabels[axis_idx+1][h_fc_idx].hold_space
+                pos[axis_idx] += [st_pos+width*(i+0.5) for i in range(sum_this_hue_bar)]
+                st_pos += (sum_this_hue_bar*width+bar_space)
+        else:
+            st_pos = 0
+            for fc_idx in range(len(xlabels[axis_idx])):
+                this_hue_per = xlabels[axis_idx][fc_idx].hold_space / df.shape[0]
+                pos[axis_idx].append(st_pos+this_hue_per/2)
+                st_pos += this_hue_per
+    return xlabels, pos
+
+def plot_bar(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+    """
+    stack bar plot with hue style\n
+    factors:[low_lever_factor, medium_lever_factor, ...] or just one
+    tags:[stack_low_y, stack_medium_y, ...] or just one
+    df:df from pro_bar_data or sort_df_factors
+        kwargs:
+    width = 0.4
+    bar_space = 0.2
+    xrotations = [0]*len(factors)
+    colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
+    offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]
+    """
+    ax1 = host_subplot(111, axes_class=axisartist.Axes)
+    
+    if len(tags) == 0:
+        tags = list(df.columns)[len(factors):]    
+    args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
+                            'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
+                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]},
+                            kwargs, locals())
+    args.xrotations.append(0)    
+    xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
+    bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
+    
+    for yIdx, yName in enumerate(tags):
+        ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=yName,
+                edgecolor='white', color=args.colors[yIdx])
+        bottom += df[yName]
+    ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
+    ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
+    plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
+    
+    axs = []
+    for idx, sub_pos in enumerate(pos[1:]):
+        axs.append(ax1.twiny())
+        axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
+        new_axisline = axs[-1].get_grid_helper().new_fixed_axis
+        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
+        plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1])
+        axs[-1].axis["top"].major_ticks.set_ticksize(0)
+        # TODO : do not work
+        axs[-1].axis["right"].major_ticks.set_ticksize(0)
+    
+    return np.array(pos[0]), ax1
+
+def plot_positional_hue(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
+    """
+    wrapper\n
+    support args: width, bar_space, xrotations, colors, offset, bottom\n
+    xlabels is in margs
+    @plot_positional_hue(['solution', 'type'], ['root', 'leaf'], ndf)\n
+    def plot_func(ax, x, y, label, label_idx, margs, **kwargs):
+        do something
+    """
+    def ret_wrapper(core_plot_func):
+        def core_wrapper(**kwargs):
+            ax1 = host_subplot(111, axes_class=axisartist.Axes)
+            nonlocal tags
+            if len(tags) == 0:
+                tags = list(df.columns)[len(factors):]    
+            margs = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
+                                    'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
+                                    'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]},
+                                   kwargs)
+            margs.xrotations.append(0)
+            xlabels, pos = pro_hue_pos(factors, df, margs.width, margs.bar_space)
+            margs.add_arg('xlabels', xlabels)
+            margs.add_arg('bottom', np.zeros(len(pos[0])), False)
+            if 'bottom' in kwargs:
+                del kwargs['bottom']
+            for yIdx, yName in enumerate(tags):
+                core_plot_func(ax1, pos[0], df[yName], yName, yIdx, margs, **kwargs)
+            ax1.set_xlim(0, pos[0][-1]+margs.bar_space+margs.width/2)
+            ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
+            plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=margs.xrotations[0])            
+            axs = []
+            for idx, sub_pos in enumerate(pos[1:]):
+                axs.append(ax1.twiny())
+                axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
+                new_axisline = axs[-1].get_grid_helper().new_fixed_axis
+                axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -margs.offset[idx]))
+                plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=margs.xrotations[idx+1])
+                axs[-1].axis["top"].major_ticks.set_ticksize(0)
+                # TODO : do not work
+                axs[-1].axis["right"].major_ticks.set_ticksize(0)            
+            return np.array(pos[0]), ax1
+        return core_wrapper
+    return ret_wrapper
+
+def qqplot(tags:list[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
+    axs = []
+    fig = plt.figure(figsize = (12, 6))
+    for fig_idx in range(1, ncols*nrows+1):
+        axs.append(fig.add_subplot(nrows, ncols, fig_idx))
+        if 'xlim' in kwargs:
+            axs[-1].set_xlim(kwargs['xlim'])
+        if 'ylim' in kwargs:
+            axs[-1].set_ylim(kwargs['ylim'])            
+        sm.qqplot(np.array(df[tags[fig_idx-1]]), fit=True, line="45", ax=axs[-1])
+        axs[-1].set_title(tags[fig_idx-1]+' - QQPlot', fontdict={'fontsize':15})
+        if 'title' in kwargs:
+            axs[-1].set_ylim(kwargs['title'][fig_idx-1])
+        if 'tick_size' in kwargs:
+            axs[-1].tick_params(labelsize = kwargs['tick_size'])
+        if 'label_size' in kwargs:
+            axs[-1].set_xlabel('Theoretical Quantiles', fontsize = kwargs['label_size'])
+            axs[-1].set_ylabel('Sample Quantiles', fontsize = kwargs['label_size'])
+            
+def save_show(path:str, dpi = 300, bbox_inches = 'tight'):
+    plt.tight_layout()
+    plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
+    plt.show()
```

### Comparing `mbapy-0.0.9/mbapy/stats/geography.py` & `mbapy-0.1.0/mbapy/stats/geography.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-#from https://www.php1.cn/detail/Python_BanZhongG_7c9b41d0.html
-
-provinces = {
-  '吉林省': [125.326800, 43.896160], '黑龙江省': [126.662850, 45.742080],
-  '辽宁省': [123.429250, 41.835710], '内蒙古自治区': [111.765220, 40.817330],
-  '新疆维吾尔自治区': [87.627100, 43.793430], '青海省': [101.780110, 36.620870],
-  '北京市': [116.407170, 39.904690], '天津市': [117.199370, 39.085100],
-  '上海市': [121.473700, 31.230370], '重庆市': [106.550730, 29.564710],
-  '河北省': [114.469790, 38.035990], '河南省': [113.753220, 34.765710],
-  '陕西省': [108.954240, 34.264860], '江苏省': [118.762950, 32.060710],
-  '山东省': [117.020760, 36.668260], '山西省': [112.562720, 37.873430],
-  '甘肃省': [103.826340, 36.059420], '宁夏回族自治区': [106.258670, 38.471170],
-  '四川省': [104.075720, 30.650890], '西藏自治区': [91.117480, 29.647250],
-  '安徽省': [117.285650, 31.861570], '浙江省': [120.153600, 30.265550],
-  '湖北省': [114.342340, 30.545390], '湖南省': [112.983400, 28.112660],
-  '福建省': [119.296590, 26.099820], '江西省': [115.910040, 28.674170],
-  '贵州省': [106.707220, 26.598200], '云南省': [102.709730, 25.045300],
-  '广东省': [113.266270, 23.131710], '广西壮族自治区': [108.327540, 22.815210],
-  '香港': [114.165460, 22.275340], '澳门': [113.549130, 22.198750],
-  '海南省': [110.348630, 20.019970], '台湾省': [121.520076, 25.030724],
-}
-
-city = [
-["北京市","",116.407170,39.904690],
-["天津市","",117.199370,39.085100],
-["上海市","",121.473700,31.230370],
-["重庆市","",106.550730,29.564710],
-["香港","",114.165460,22.275340],
-["澳门","",113.549130,22.198750],
-["河北省","石家庄市",114.514300,38.042760],
-["河北省","唐山市",118.180580,39.630480],
-["河北省","秦皇岛市",119.599640,39.935450],
-["河北省","邯郸市",114.539180,36.625560],
-["河北省","邢台市",114.504430,37.070550],
-["河北省","保定市",115.464590,38.873960],
-["河北省","张家口市",114.887550,40.824440],
-["河北省","承德市",117.963400,40.951500],
-["河北省","沧州市",116.838690,38.304410],
-["河北省","廊坊市",116.683760,39.537750],
-["河北省","衡水市",115.670540,37.738860],
-["河南省","郑州市",113.624930,34.747250],
-["河南省","开封市",114.307310,34.797260],
-["河南省","洛阳市",112.453610,34.618120],
-["河南省","平顶山市",113.192410,33.766090],
-["河南省","安阳市",114.393100,36.097710],
-["河南省","鹤壁市",114.297450,35.747000],
-["河南省","新乡市",113.926750,35.303230],
-["河南省","焦作市",113.242010,35.215630],
-["河南省","濮阳市",115.029320,35.761890],
-["河南省","许昌市",113.852330,34.035700],
-["河南省","漯河市",114.016810,33.581490],
-["河南省","三门峡市",111.200300,34.772610],
-["河南省","南阳市",112.528510,32.990730],
-["河南省","商丘市",115.656350,34.414270],
-["河南省","信阳市",114.092790,32.147140],
-["河南省","周口市",114.696950,33.625830],
-["河南省","驻马店市",114.022990,33.011420],
-["山东省","济南市",117.120090,36.651840],
-["山东省","青岛市",120.382990,36.066230],
-["山东省","淄博市",118.054800,36.813100],
-["山东省","枣庄市",117.321960,34.810710],
-["山东省","东营市",118.674660,37.433650],
-["山东省","烟台市",121.448010,37.463530],
-["山东省","潍坊市",119.161760,36.706860],
-["山东省","济宁市",116.587240,35.414590],
-["山东省","泰安市",117.088400,36.199940],
-["山东省","威海市",122.121710,37.513480],
-["山东省","日照市",119.527190,35.416460],
-["山东省","莱芜市",117.676670,36.213590],
-["山东省","临沂市",118.356460,35.104650],
-["山东省","德州市",116.359270,37.435500],
-["山东省","聊城市",115.985490,36.457020],
-["山东省","滨州市",117.972790,37.382110],
-["山东省","菏泽市",115.481150,35.233630],
-["山西省","太原市",112.556252,37.876876],
-["山西省","大同市",113.304424,40.081863],
-["山西省","阳泉市",113.580470,37.856680],
-["山西省","长治市",113.116490,36.195810],
-["山西省","晋城市",112.851130,35.490390],
-["山西省","朔州市",112.439374,39.357422],
-["山西省","晋中市",112.752780,37.687020],
-["山西省","运城市",111.006990,35.026280],
-["山西省","忻州市",112.734180,38.416700],
-["山西省","临汾市",111.519620,36.088220],
-["山西省","吕梁市",111.141650,37.519340],
-["辽宁省","沈阳市",123.463100,41.677180],
-["辽宁省","大连市",121.614760,38.913690],
-["辽宁省","鞍山市",122.994600,41.107770],
-["辽宁省","抚顺市",123.957220,41.879710],
-["辽宁省","本溪市",123.766860,41.294130],
-["辽宁省","丹东市",124.356010,39.999800],
-["辽宁省","锦州市",121.127030,41.095150],
-["辽宁省","营口市",122.234900,40.666830],
-["辽宁省","阜新市",121.670110,42.021660],
-["辽宁省","辽阳市",123.237360,41.268090],
-["辽宁省","盘锦市",122.070780,41.119960],
-["辽宁省","铁岭市",123.842410,42.286200],
-["辽宁省","朝阳市",120.450800,41.573470],
-["辽宁省","葫芦岛市",120.836990,40.711000],
-["吉林省","长春市",125.323570,43.816020],
-["吉林省","吉林市",126.549440,43.837840],
-["吉林省","四平市",124.350360,43.166460],
-["吉林省","辽源市",125.143680,42.888050],
-["吉林省","通化市",125.939900,41.728290],
-["吉林省","白山市",126.424430,41.940800],
-["吉林省","松原市",124.825150,45.141100],
-["吉林省","白城市",122.838710,45.619600],
-["吉林省","延边朝鲜族自治州",129.509100,42.891190],
-["黑龙江省","哈尔滨市",126.535800,45.802160],
-["黑龙江省","齐齐哈尔市",123.917960,47.354310],
-["黑龙江省","鸡西市",130.969540,45.295240],
-["黑龙江省","鹤岗市",130.297850,47.349890],
-["黑龙江省","双鸭山市",131.159100,46.646580],
-["黑龙江省","大庆市",125.110961,46.595319],
-["黑龙江省","伊春市",128.840490,47.727520],
-["黑龙江省","佳木斯市",130.318820,46.799770],
-["黑龙江省","七台河市",131.003060,45.770650],
-["黑龙江省","牡丹江市",129.632440,44.552690],
-["黑龙江省","黑河市",127.528520,50.245230],
-["黑龙江省","绥化市",126.969320,46.652460],
-["黑龙江省","大兴安岭地区",124.592160,51.923980],
-["江苏省","南京市",118.796470,32.058380],
-["江苏省","无锡市",120.312370,31.490990],
-["江苏省","徐州市",117.285770,34.204400],
-["江苏省","常州市",119.973650,31.810720],
-["江苏省","苏州市",120.583190,31.298340],
-["江苏省","南通市",120.893710,31.979580],
-["江苏省","连云港市",119.222950,34.596690],
-["江苏省","淮安市",119.015950,33.610160],
-["江苏省","盐城市",120.161640,33.349510],
-["江苏省","扬州市",119.412690,32.393580],
-["江苏省","镇江市",119.425000,32.189590],
-["江苏省","泰州市",119.925540,32.455460],
-["江苏省","宿迁市",118.275490,33.961930],
-["浙江省","杭州市",120.155150,30.274150],
-["浙江省","宁波市",121.550270,29.873860],
-["浙江省","温州市",120.699390,27.994920],
-["浙江省","嘉兴市",120.755500,30.745010],
-["浙江省","湖州市",120.088050,30.893050],
-["浙江省","绍兴市",120.580200,30.030330],
-["浙江省","金华市",119.647590,29.078120],
-["浙江省","衢州市",118.874190,28.935920],
-["浙江省","舟山市",122.207780,29.985390],
-["浙江省","台州市",121.420560,28.656110],
-["浙江省","丽水市",119.922930,28.467200],
-["安徽省","合肥市",117.229010,31.820570],
-["安徽省","芜湖市",118.433130,31.352460],
-["安徽省","蚌埠市",117.389320,32.915480],
-["安徽省","淮南市",116.999800,32.625490],
-["安徽省","马鞍山市",118.506110,31.670670],
-["安徽省","淮北市",116.798340,33.954790],
-["安徽省","铜陵市",117.812320,30.944860],
-["安徽省","安庆市",117.063540,30.542940],
-["安徽省","黄山市",118.338660,29.715170],
-["安徽省","滁州市",118.316830,32.301810],
-["安徽省","阜阳市",115.814950,32.889630],
-["安徽省","宿州市",116.963910,33.646140],
-["安徽省","六安市",116.523240,31.734880],
-["安徽省","亳州市",115.779310,33.844610],
-["安徽省","池州市",117.491420,30.664690],
-["安徽省","宣城市",118.758660,30.940780],
-["福建省","福州市",119.296470,26.074210],
-["福建省","厦门市",118.089480,24.479510],
-["福建省","莆田市",119.007710,25.454000],
-["福建省","三明市",117.639220,26.263850],
-["福建省","泉州市",118.675870,24.873890],
-["福建省","漳州市",117.647250,24.513470],
-["福建省","南平市",118.120430,27.331750],
-["福建省","龙岩市",117.017220,25.075040],
-["福建省","宁德市",119.548190,26.665710],
-["江西省","南昌市",115.857940,28.682020],
-["江西省","景德镇市",117.178390,29.268690],
-["江西省","萍乡市",113.854270,27.622890],
-["江西省","九江市",116.001460,29.705480],
-["江西省","新余市",114.917130,27.817760],
-["江西省","鹰潭市",117.069190,28.260190],
-["江西省","赣州市",114.934760,25.831090],
-["江西省","吉安市",114.993760,27.113820],
-["江西省","宜春市",114.416120,27.814430],
-["江西省","抚州市",116.358090,27.947810],
-["江西省","上饶市",117.943570,28.454630],
-["湖北省","武汉市",114.305250,30.592760],
-["湖北省","黄石市",115.038900,30.199530],
-["湖北省","十堰市",110.798010,32.629180],
-["湖北省","宜昌市",111.286420,30.691860],
-["湖北省","襄阳市",112.122550,32.009000],
-["湖北省","鄂州市",114.894950,30.390850],
-["湖北省","荆门市",112.199450,31.035460],
-["湖北省","孝感市",113.916450,30.924830],
-["湖北省","荆州市",112.240690,30.334790],
-["湖北省","黄冈市",114.872380,30.453470],
-["湖北省","咸宁市",114.322450,29.841260],
-["湖北省","随州市",113.382620,31.690130],
-["湖北省","恩施土家族苗族自治州",109.488170,30.272170],
-["湖南省","长沙市",112.938860,28.227780],
-["湖南省","株洲市",113.133960,27.827670],
-["湖南省","湘潭市",112.944110,27.829750],
-["湖南省","衡阳市",112.571950,26.893240],
-["湖南省","邵阳市",111.467700,27.238900],
-["湖南省","岳阳市",113.129190,29.357280],
-["湖南省","常德市",111.698540,29.031580],
-["湖南省","张家界市",110.478390,29.116670],
-["湖南省","益阳市",112.355160,28.553910],
-["湖南省","郴州市",113.014850,25.770630],
-["湖南省","永州市",111.612250,26.420340],
-["湖南省","怀化市",110.001600,27.569740],
-["湖南省","娄底市",111.994580,27.697280],
-["湖南省","湘西土家族苗族自治州",109.738930,28.311730],
-["广东省","广州市",113.264360,23.129080],
-["广东省","韶关市",113.597230,24.810390],
-["广东省","深圳市",114.059560,22.542860],
-["广东省","珠海市",113.576680,22.270730],
-["广东省","汕头市",116.682210,23.353500],
-["广东省","佛山市",113.121920,23.021850],
-["广东省","江门市",113.081610,22.578650],
-["广东省","湛江市",110.358940,21.271340],
-["广东省","茂名市",110.925230,21.663290],
-["广东省","肇庆市",112.465280,23.046900],
-["广东省","惠州市",114.416790,23.110750],
-["广东省","梅州市",116.122640,24.288440],
-["广东省","汕尾市",115.375140,22.785660],
-["广东省","河源市",114.700650,23.743650],
-["广东省","阳江市",111.982560,21.858290],
-["广东省","清远市",113.056150,23.682010],
-["广东省","东莞市",113.751790,23.020670],
-["广东省","中山市",113.392600,22.515950],
-["广东省","潮州市",116.622960,23.656700],
-["广东省","揭阳市",116.372710,23.549720],
-["广东省","云浮市",112.044530,22.915250],
-["海南省","海口市",110.199890,20.044220],
-["海南省","三亚市",109.512090,18.252480],
-["海南省","三沙市",112.333560,16.832720],
-["海南省","儋州市",109.580690,19.520930],
-["四川省","成都市",104.064760,30.570200],
-["四川省","自贡市",104.778440,29.339200],
-["四川省","攀枝花市",101.718720,26.582280],
-["四川省","泸州市",105.442570,28.871700],
-["四川省","德阳市",104.397900,31.126790],
-["四川省","绵阳市",104.679600,31.467510],
-["四川省","广元市",105.843570,32.435490],
-["四川省","遂宁市",105.592730,30.532860],
-["四川省","内江市",105.058440,29.580150],
-["四川省","乐山市",103.765390,29.552210],
-["四川省","南充市",106.110730,30.837310],
-["四川省","眉山市",103.848510,30.075630],
-["四川省","宜宾市",104.641700,28.751300],
-["四川省","广安市",106.633220,30.455960],
-["四川省","达州市",107.467910,31.208640],
-["四川省","雅安市",103.042400,30.010530],
-["四川省","巴中市",106.747330,31.867150],
-["四川省","资阳市",104.627980,30.128590],
-["四川省","阿坝藏族羌族自治州",102.224770,31.899400],
-["四川省","甘孜藏族自治州",101.962540,30.049320],
-["四川省","凉山彝族自治州",102.267460,27.881640],
-["贵州省","贵阳市",106.630240,26.647020],
-["贵州省","六盘水市",104.830230,26.593360],
-["贵州省","遵义市",106.927230,27.725450],
-["贵州省","安顺市",105.946200,26.253670],
-["贵州省","毕节市",105.305040,27.298470],
-["贵州省","铜仁市",109.180990,27.690660],
-["贵州省","黔西南布依族苗族自治州",104.904370,25.089880],
-["贵州省","黔东南苗族侗族自治州",107.984160,26.583640],
-["贵州省","黔南布依族苗族自治州",107.522260,26.254270],
-["云南省","昆明市",102.833220,24.879660],
-["云南省","曲靖市",103.796250,25.490020],
-["云南省","玉溪市",102.547140,24.351800],
-["云南省","保山市",99.161810,25.112050],
-["云南省","昭通市",103.716800,27.338170],
-["云南省","丽江市",100.227100,26.856480],
-["云南省","普洱市",100.966240,22.825210],
-["云南省","临沧市",100.088840,23.884260],
-["云南省","楚雄彝族自治州",101.527670,25.044950],
-["云南省","红河哈尼族彝族自治州",103.375600,23.364220],
-["云南省","文山壮族苗族自治州",104.215040,23.398490],
-["云南省","西双版纳傣族自治州",100.797390,22.007490],
-["云南省","大理白族自治州",100.267640,25.606480],
-["云南省","德宏傣族景颇族自治州",98.584860,24.432320],
-["云南省","怒江傈僳族自治州",98.856700,25.817630],
-["云南省","迪庆藏族自治州",99.703050,27.819080],
-["陕西省","西安市",108.939840,34.341270],
-["陕西省","铜川市",108.945150,34.896730],
-["陕西省","宝鸡市",107.237320,34.361940],
-["陕西省","咸阳市",108.709290,34.329320],
-["陕西省","渭南市",109.510150,34.499970],
-["陕西省","延安市",109.489780,36.585290],
-["陕西省","汉中市",107.023770,33.067610],
-["陕西省","榆林市",109.734580,38.285200],
-["陕西省","安康市",109.029320,32.684860],
-["陕西省","商洛市",109.940410,33.870360],
-["甘肃省","兰州市",103.834170,36.061380],
-["甘肃省","嘉峪关市",98.290110,39.772010],
-["甘肃省","金昌市",102.187590,38.520060],
-["甘肃省","白银市",104.137730,36.544700],
-["甘肃省","天水市",105.724860,34.580850],
-["甘肃省","武威市",102.637970,37.928200],
-["甘肃省","张掖市",100.449810,38.925920],
-["甘肃省","平凉市",106.665300,35.543030],
-["甘肃省","酒泉市",98.493940,39.732550],
-["甘肃省","庆阳市",107.642920,35.709780],
-["甘肃省","定西市",104.625240,35.581130],
-["甘肃省","陇南市",104.921660,33.401000],
-["甘肃省","临夏回族自治州",103.210910,35.601220],
-["甘肃省","甘南藏族自治州",102.911020,34.983270],
-["青海省","西宁市",101.777820,36.617290],
-["青海省","海东市",102.401730,36.482090],
-["青海省","海北藏族自治州",100.900960,36.954540],
-["青海省","黄南藏族自治州",102.015070,35.519910],
-["青海省","海南藏族自治州",100.620370,36.286630],
-["青海省","果洛藏族自治州",100.244750,34.471410],
-["青海省","玉树藏族自治州",97.006500,33.005280],
-["青海省","海西蒙古族藏族自治州",97.371220,37.377100],
-["广西壮族自治区","南宁市",108.366900,22.816730],
-["广西壮族自治区","柳州市",109.415520,24.325430],
-["广西壮族自治区","桂林市",110.290020,25.273610],
-["广西壮族自治区","梧州市",111.279170,23.476910],
-["广西壮族自治区","北海市",109.120080,21.481120],
-["广西壮族自治区","防城港市",108.354720,21.687130],
-["广西壮族自治区","钦州市",108.654310,21.979700],
-["广西壮族自治区","贵港市",109.597640,23.113060],
-["广西壮族自治区","玉林市",110.180980,22.654510],
-["广西壮族自治区","百色市",106.618380,23.902160],
-["广西壮族自治区","贺州市",111.566550,24.403460],
-["广西壮族自治区","河池市",108.085400,24.692910],
-["广西壮族自治区","来宾市",109.222380,23.752100],
-["广西壮族自治区","崇左市",107.364850,22.378950],
-["内蒙古自治区","呼和浩特市",111.751990,40.841490],
-["内蒙古自治区","包头市",109.840210,40.657810],
-["内蒙古自治区","乌海市",106.795460,39.653840],
-["内蒙古自治区","赤峰市",118.888940,42.258600],
-["内蒙古自治区","通辽市",122.244690,43.652470],
-["内蒙古自治区","鄂尔多斯市",109.780870,39.608450],
-["内蒙古自治区","呼伦贝尔市",119.765840,49.211630],
-["内蒙古自治区","巴彦淖尔市",107.387730,40.743170],
-["内蒙古自治区","乌兰察布市",113.133760,40.993910],
-["内蒙古自治区","兴安盟",122.038180,46.082080],
-["内蒙古自治区","锡林郭勒盟",116.047750,43.933200],
-["内蒙古自治区","阿拉善盟",105.728980,38.851530],
-["宁夏回族自治区","银川市",106.232480,38.486440],
-["宁夏回族自治区","石嘴山市",106.384180,38.984100],
-["宁夏回族自治区","吴忠市",106.198790,37.997550],
-["宁夏回族自治区","固原市",106.242590,36.015800],
-["宁夏回族自治区","中卫市",105.196760,37.500260],
-["西藏自治区","拉萨市",91.114500,29.644150],
-["西藏自治区","日喀则市",88.881160,29.267050],
-["西藏自治区","昌都市",97.172250,31.140730],
-["西藏自治区","林芝市",94.361550,29.648950],
-["西藏自治区","山南市",91.773130,29.237050],
-["西藏自治区","那曲市",92.051360,31.476140],
-["西藏自治区","阿里地区",81.145400,30.400510],
-["新疆维吾尔自治区","乌鲁木齐市",87.616880,43.826630],
-["新疆维吾尔自治区","克拉玛依市",84.889270,45.579990],
-["新疆维吾尔自治区","吐鲁番市",89.189540,42.951300],
-["新疆维吾尔自治区","哈密市",93.515380,42.818550],
-["新疆维吾尔自治区","昌吉回族自治州",87.308220,44.011170],
-["新疆维吾尔自治区","博尔塔拉蒙古自治州",82.066650,44.905970],
-["新疆维吾尔自治区","巴音郭楞蒙古自治州",86.145170,41.764040],
-["新疆维吾尔自治区","阿克苏地区",80.260080,41.168420],
-["新疆维吾尔自治区","克孜勒苏柯尔克孜自治州",76.166610,39.715300],
-["新疆维吾尔自治区","喀什地区",75.989760,39.470420],
-["新疆维吾尔自治区","和田地区",79.922470,37.114310],
-["新疆维吾尔自治区","伊犁哈萨克自治州",81.324160,43.916890],
-["新疆维吾尔自治区","塔城地区",82.980460,46.745320],
-["新疆维吾尔自治区","阿勒泰地区",88.140230,47.845640],
+#from https://www.php1.cn/detail/Python_BanZhongG_7c9b41d0.html
+
+provinces = {
+  '吉林省': [125.326800, 43.896160], '黑龙江省': [126.662850, 45.742080],
+  '辽宁省': [123.429250, 41.835710], '内蒙古自治区': [111.765220, 40.817330],
+  '新疆维吾尔自治区': [87.627100, 43.793430], '青海省': [101.780110, 36.620870],
+  '北京市': [116.407170, 39.904690], '天津市': [117.199370, 39.085100],
+  '上海市': [121.473700, 31.230370], '重庆市': [106.550730, 29.564710],
+  '河北省': [114.469790, 38.035990], '河南省': [113.753220, 34.765710],
+  '陕西省': [108.954240, 34.264860], '江苏省': [118.762950, 32.060710],
+  '山东省': [117.020760, 36.668260], '山西省': [112.562720, 37.873430],
+  '甘肃省': [103.826340, 36.059420], '宁夏回族自治区': [106.258670, 38.471170],
+  '四川省': [104.075720, 30.650890], '西藏自治区': [91.117480, 29.647250],
+  '安徽省': [117.285650, 31.861570], '浙江省': [120.153600, 30.265550],
+  '湖北省': [114.342340, 30.545390], '湖南省': [112.983400, 28.112660],
+  '福建省': [119.296590, 26.099820], '江西省': [115.910040, 28.674170],
+  '贵州省': [106.707220, 26.598200], '云南省': [102.709730, 25.045300],
+  '广东省': [113.266270, 23.131710], '广西壮族自治区': [108.327540, 22.815210],
+  '香港': [114.165460, 22.275340], '澳门': [113.549130, 22.198750],
+  '海南省': [110.348630, 20.019970], '台湾省': [121.520076, 25.030724],
+}
+
+city = [
+["北京市","",116.407170,39.904690],
+["天津市","",117.199370,39.085100],
+["上海市","",121.473700,31.230370],
+["重庆市","",106.550730,29.564710],
+["香港","",114.165460,22.275340],
+["澳门","",113.549130,22.198750],
+["河北省","石家庄市",114.514300,38.042760],
+["河北省","唐山市",118.180580,39.630480],
+["河北省","秦皇岛市",119.599640,39.935450],
+["河北省","邯郸市",114.539180,36.625560],
+["河北省","邢台市",114.504430,37.070550],
+["河北省","保定市",115.464590,38.873960],
+["河北省","张家口市",114.887550,40.824440],
+["河北省","承德市",117.963400,40.951500],
+["河北省","沧州市",116.838690,38.304410],
+["河北省","廊坊市",116.683760,39.537750],
+["河北省","衡水市",115.670540,37.738860],
+["河南省","郑州市",113.624930,34.747250],
+["河南省","开封市",114.307310,34.797260],
+["河南省","洛阳市",112.453610,34.618120],
+["河南省","平顶山市",113.192410,33.766090],
+["河南省","安阳市",114.393100,36.097710],
+["河南省","鹤壁市",114.297450,35.747000],
+["河南省","新乡市",113.926750,35.303230],
+["河南省","焦作市",113.242010,35.215630],
+["河南省","濮阳市",115.029320,35.761890],
+["河南省","许昌市",113.852330,34.035700],
+["河南省","漯河市",114.016810,33.581490],
+["河南省","三门峡市",111.200300,34.772610],
+["河南省","南阳市",112.528510,32.990730],
+["河南省","商丘市",115.656350,34.414270],
+["河南省","信阳市",114.092790,32.147140],
+["河南省","周口市",114.696950,33.625830],
+["河南省","驻马店市",114.022990,33.011420],
+["山东省","济南市",117.120090,36.651840],
+["山东省","青岛市",120.382990,36.066230],
+["山东省","淄博市",118.054800,36.813100],
+["山东省","枣庄市",117.321960,34.810710],
+["山东省","东营市",118.674660,37.433650],
+["山东省","烟台市",121.448010,37.463530],
+["山东省","潍坊市",119.161760,36.706860],
+["山东省","济宁市",116.587240,35.414590],
+["山东省","泰安市",117.088400,36.199940],
+["山东省","威海市",122.121710,37.513480],
+["山东省","日照市",119.527190,35.416460],
+["山东省","莱芜市",117.676670,36.213590],
+["山东省","临沂市",118.356460,35.104650],
+["山东省","德州市",116.359270,37.435500],
+["山东省","聊城市",115.985490,36.457020],
+["山东省","滨州市",117.972790,37.382110],
+["山东省","菏泽市",115.481150,35.233630],
+["山西省","太原市",112.556252,37.876876],
+["山西省","大同市",113.304424,40.081863],
+["山西省","阳泉市",113.580470,37.856680],
+["山西省","长治市",113.116490,36.195810],
+["山西省","晋城市",112.851130,35.490390],
+["山西省","朔州市",112.439374,39.357422],
+["山西省","晋中市",112.752780,37.687020],
+["山西省","运城市",111.006990,35.026280],
+["山西省","忻州市",112.734180,38.416700],
+["山西省","临汾市",111.519620,36.088220],
+["山西省","吕梁市",111.141650,37.519340],
+["辽宁省","沈阳市",123.463100,41.677180],
+["辽宁省","大连市",121.614760,38.913690],
+["辽宁省","鞍山市",122.994600,41.107770],
+["辽宁省","抚顺市",123.957220,41.879710],
+["辽宁省","本溪市",123.766860,41.294130],
+["辽宁省","丹东市",124.356010,39.999800],
+["辽宁省","锦州市",121.127030,41.095150],
+["辽宁省","营口市",122.234900,40.666830],
+["辽宁省","阜新市",121.670110,42.021660],
+["辽宁省","辽阳市",123.237360,41.268090],
+["辽宁省","盘锦市",122.070780,41.119960],
+["辽宁省","铁岭市",123.842410,42.286200],
+["辽宁省","朝阳市",120.450800,41.573470],
+["辽宁省","葫芦岛市",120.836990,40.711000],
+["吉林省","长春市",125.323570,43.816020],
+["吉林省","吉林市",126.549440,43.837840],
+["吉林省","四平市",124.350360,43.166460],
+["吉林省","辽源市",125.143680,42.888050],
+["吉林省","通化市",125.939900,41.728290],
+["吉林省","白山市",126.424430,41.940800],
+["吉林省","松原市",124.825150,45.141100],
+["吉林省","白城市",122.838710,45.619600],
+["吉林省","延边朝鲜族自治州",129.509100,42.891190],
+["黑龙江省","哈尔滨市",126.535800,45.802160],
+["黑龙江省","齐齐哈尔市",123.917960,47.354310],
+["黑龙江省","鸡西市",130.969540,45.295240],
+["黑龙江省","鹤岗市",130.297850,47.349890],
+["黑龙江省","双鸭山市",131.159100,46.646580],
+["黑龙江省","大庆市",125.110961,46.595319],
+["黑龙江省","伊春市",128.840490,47.727520],
+["黑龙江省","佳木斯市",130.318820,46.799770],
+["黑龙江省","七台河市",131.003060,45.770650],
+["黑龙江省","牡丹江市",129.632440,44.552690],
+["黑龙江省","黑河市",127.528520,50.245230],
+["黑龙江省","绥化市",126.969320,46.652460],
+["黑龙江省","大兴安岭地区",124.592160,51.923980],
+["江苏省","南京市",118.796470,32.058380],
+["江苏省","无锡市",120.312370,31.490990],
+["江苏省","徐州市",117.285770,34.204400],
+["江苏省","常州市",119.973650,31.810720],
+["江苏省","苏州市",120.583190,31.298340],
+["江苏省","南通市",120.893710,31.979580],
+["江苏省","连云港市",119.222950,34.596690],
+["江苏省","淮安市",119.015950,33.610160],
+["江苏省","盐城市",120.161640,33.349510],
+["江苏省","扬州市",119.412690,32.393580],
+["江苏省","镇江市",119.425000,32.189590],
+["江苏省","泰州市",119.925540,32.455460],
+["江苏省","宿迁市",118.275490,33.961930],
+["浙江省","杭州市",120.155150,30.274150],
+["浙江省","宁波市",121.550270,29.873860],
+["浙江省","温州市",120.699390,27.994920],
+["浙江省","嘉兴市",120.755500,30.745010],
+["浙江省","湖州市",120.088050,30.893050],
+["浙江省","绍兴市",120.580200,30.030330],
+["浙江省","金华市",119.647590,29.078120],
+["浙江省","衢州市",118.874190,28.935920],
+["浙江省","舟山市",122.207780,29.985390],
+["浙江省","台州市",121.420560,28.656110],
+["浙江省","丽水市",119.922930,28.467200],
+["安徽省","合肥市",117.229010,31.820570],
+["安徽省","芜湖市",118.433130,31.352460],
+["安徽省","蚌埠市",117.389320,32.915480],
+["安徽省","淮南市",116.999800,32.625490],
+["安徽省","马鞍山市",118.506110,31.670670],
+["安徽省","淮北市",116.798340,33.954790],
+["安徽省","铜陵市",117.812320,30.944860],
+["安徽省","安庆市",117.063540,30.542940],
+["安徽省","黄山市",118.338660,29.715170],
+["安徽省","滁州市",118.316830,32.301810],
+["安徽省","阜阳市",115.814950,32.889630],
+["安徽省","宿州市",116.963910,33.646140],
+["安徽省","六安市",116.523240,31.734880],
+["安徽省","亳州市",115.779310,33.844610],
+["安徽省","池州市",117.491420,30.664690],
+["安徽省","宣城市",118.758660,30.940780],
+["福建省","福州市",119.296470,26.074210],
+["福建省","厦门市",118.089480,24.479510],
+["福建省","莆田市",119.007710,25.454000],
+["福建省","三明市",117.639220,26.263850],
+["福建省","泉州市",118.675870,24.873890],
+["福建省","漳州市",117.647250,24.513470],
+["福建省","南平市",118.120430,27.331750],
+["福建省","龙岩市",117.017220,25.075040],
+["福建省","宁德市",119.548190,26.665710],
+["江西省","南昌市",115.857940,28.682020],
+["江西省","景德镇市",117.178390,29.268690],
+["江西省","萍乡市",113.854270,27.622890],
+["江西省","九江市",116.001460,29.705480],
+["江西省","新余市",114.917130,27.817760],
+["江西省","鹰潭市",117.069190,28.260190],
+["江西省","赣州市",114.934760,25.831090],
+["江西省","吉安市",114.993760,27.113820],
+["江西省","宜春市",114.416120,27.814430],
+["江西省","抚州市",116.358090,27.947810],
+["江西省","上饶市",117.943570,28.454630],
+["湖北省","武汉市",114.305250,30.592760],
+["湖北省","黄石市",115.038900,30.199530],
+["湖北省","十堰市",110.798010,32.629180],
+["湖北省","宜昌市",111.286420,30.691860],
+["湖北省","襄阳市",112.122550,32.009000],
+["湖北省","鄂州市",114.894950,30.390850],
+["湖北省","荆门市",112.199450,31.035460],
+["湖北省","孝感市",113.916450,30.924830],
+["湖北省","荆州市",112.240690,30.334790],
+["湖北省","黄冈市",114.872380,30.453470],
+["湖北省","咸宁市",114.322450,29.841260],
+["湖北省","随州市",113.382620,31.690130],
+["湖北省","恩施土家族苗族自治州",109.488170,30.272170],
+["湖南省","长沙市",112.938860,28.227780],
+["湖南省","株洲市",113.133960,27.827670],
+["湖南省","湘潭市",112.944110,27.829750],
+["湖南省","衡阳市",112.571950,26.893240],
+["湖南省","邵阳市",111.467700,27.238900],
+["湖南省","岳阳市",113.129190,29.357280],
+["湖南省","常德市",111.698540,29.031580],
+["湖南省","张家界市",110.478390,29.116670],
+["湖南省","益阳市",112.355160,28.553910],
+["湖南省","郴州市",113.014850,25.770630],
+["湖南省","永州市",111.612250,26.420340],
+["湖南省","怀化市",110.001600,27.569740],
+["湖南省","娄底市",111.994580,27.697280],
+["湖南省","湘西土家族苗族自治州",109.738930,28.311730],
+["广东省","广州市",113.264360,23.129080],
+["广东省","韶关市",113.597230,24.810390],
+["广东省","深圳市",114.059560,22.542860],
+["广东省","珠海市",113.576680,22.270730],
+["广东省","汕头市",116.682210,23.353500],
+["广东省","佛山市",113.121920,23.021850],
+["广东省","江门市",113.081610,22.578650],
+["广东省","湛江市",110.358940,21.271340],
+["广东省","茂名市",110.925230,21.663290],
+["广东省","肇庆市",112.465280,23.046900],
+["广东省","惠州市",114.416790,23.110750],
+["广东省","梅州市",116.122640,24.288440],
+["广东省","汕尾市",115.375140,22.785660],
+["广东省","河源市",114.700650,23.743650],
+["广东省","阳江市",111.982560,21.858290],
+["广东省","清远市",113.056150,23.682010],
+["广东省","东莞市",113.751790,23.020670],
+["广东省","中山市",113.392600,22.515950],
+["广东省","潮州市",116.622960,23.656700],
+["广东省","揭阳市",116.372710,23.549720],
+["广东省","云浮市",112.044530,22.915250],
+["海南省","海口市",110.199890,20.044220],
+["海南省","三亚市",109.512090,18.252480],
+["海南省","三沙市",112.333560,16.832720],
+["海南省","儋州市",109.580690,19.520930],
+["四川省","成都市",104.064760,30.570200],
+["四川省","自贡市",104.778440,29.339200],
+["四川省","攀枝花市",101.718720,26.582280],
+["四川省","泸州市",105.442570,28.871700],
+["四川省","德阳市",104.397900,31.126790],
+["四川省","绵阳市",104.679600,31.467510],
+["四川省","广元市",105.843570,32.435490],
+["四川省","遂宁市",105.592730,30.532860],
+["四川省","内江市",105.058440,29.580150],
+["四川省","乐山市",103.765390,29.552210],
+["四川省","南充市",106.110730,30.837310],
+["四川省","眉山市",103.848510,30.075630],
+["四川省","宜宾市",104.641700,28.751300],
+["四川省","广安市",106.633220,30.455960],
+["四川省","达州市",107.467910,31.208640],
+["四川省","雅安市",103.042400,30.010530],
+["四川省","巴中市",106.747330,31.867150],
+["四川省","资阳市",104.627980,30.128590],
+["四川省","阿坝藏族羌族自治州",102.224770,31.899400],
+["四川省","甘孜藏族自治州",101.962540,30.049320],
+["四川省","凉山彝族自治州",102.267460,27.881640],
+["贵州省","贵阳市",106.630240,26.647020],
+["贵州省","六盘水市",104.830230,26.593360],
+["贵州省","遵义市",106.927230,27.725450],
+["贵州省","安顺市",105.946200,26.253670],
+["贵州省","毕节市",105.305040,27.298470],
+["贵州省","铜仁市",109.180990,27.690660],
+["贵州省","黔西南布依族苗族自治州",104.904370,25.089880],
+["贵州省","黔东南苗族侗族自治州",107.984160,26.583640],
+["贵州省","黔南布依族苗族自治州",107.522260,26.254270],
+["云南省","昆明市",102.833220,24.879660],
+["云南省","曲靖市",103.796250,25.490020],
+["云南省","玉溪市",102.547140,24.351800],
+["云南省","保山市",99.161810,25.112050],
+["云南省","昭通市",103.716800,27.338170],
+["云南省","丽江市",100.227100,26.856480],
+["云南省","普洱市",100.966240,22.825210],
+["云南省","临沧市",100.088840,23.884260],
+["云南省","楚雄彝族自治州",101.527670,25.044950],
+["云南省","红河哈尼族彝族自治州",103.375600,23.364220],
+["云南省","文山壮族苗族自治州",104.215040,23.398490],
+["云南省","西双版纳傣族自治州",100.797390,22.007490],
+["云南省","大理白族自治州",100.267640,25.606480],
+["云南省","德宏傣族景颇族自治州",98.584860,24.432320],
+["云南省","怒江傈僳族自治州",98.856700,25.817630],
+["云南省","迪庆藏族自治州",99.703050,27.819080],
+["陕西省","西安市",108.939840,34.341270],
+["陕西省","铜川市",108.945150,34.896730],
+["陕西省","宝鸡市",107.237320,34.361940],
+["陕西省","咸阳市",108.709290,34.329320],
+["陕西省","渭南市",109.510150,34.499970],
+["陕西省","延安市",109.489780,36.585290],
+["陕西省","汉中市",107.023770,33.067610],
+["陕西省","榆林市",109.734580,38.285200],
+["陕西省","安康市",109.029320,32.684860],
+["陕西省","商洛市",109.940410,33.870360],
+["甘肃省","兰州市",103.834170,36.061380],
+["甘肃省","嘉峪关市",98.290110,39.772010],
+["甘肃省","金昌市",102.187590,38.520060],
+["甘肃省","白银市",104.137730,36.544700],
+["甘肃省","天水市",105.724860,34.580850],
+["甘肃省","武威市",102.637970,37.928200],
+["甘肃省","张掖市",100.449810,38.925920],
+["甘肃省","平凉市",106.665300,35.543030],
+["甘肃省","酒泉市",98.493940,39.732550],
+["甘肃省","庆阳市",107.642920,35.709780],
+["甘肃省","定西市",104.625240,35.581130],
+["甘肃省","陇南市",104.921660,33.401000],
+["甘肃省","临夏回族自治州",103.210910,35.601220],
+["甘肃省","甘南藏族自治州",102.911020,34.983270],
+["青海省","西宁市",101.777820,36.617290],
+["青海省","海东市",102.401730,36.482090],
+["青海省","海北藏族自治州",100.900960,36.954540],
+["青海省","黄南藏族自治州",102.015070,35.519910],
+["青海省","海南藏族自治州",100.620370,36.286630],
+["青海省","果洛藏族自治州",100.244750,34.471410],
+["青海省","玉树藏族自治州",97.006500,33.005280],
+["青海省","海西蒙古族藏族自治州",97.371220,37.377100],
+["广西壮族自治区","南宁市",108.366900,22.816730],
+["广西壮族自治区","柳州市",109.415520,24.325430],
+["广西壮族自治区","桂林市",110.290020,25.273610],
+["广西壮族自治区","梧州市",111.279170,23.476910],
+["广西壮族自治区","北海市",109.120080,21.481120],
+["广西壮族自治区","防城港市",108.354720,21.687130],
+["广西壮族自治区","钦州市",108.654310,21.979700],
+["广西壮族自治区","贵港市",109.597640,23.113060],
+["广西壮族自治区","玉林市",110.180980,22.654510],
+["广西壮族自治区","百色市",106.618380,23.902160],
+["广西壮族自治区","贺州市",111.566550,24.403460],
+["广西壮族自治区","河池市",108.085400,24.692910],
+["广西壮族自治区","来宾市",109.222380,23.752100],
+["广西壮族自治区","崇左市",107.364850,22.378950],
+["内蒙古自治区","呼和浩特市",111.751990,40.841490],
+["内蒙古自治区","包头市",109.840210,40.657810],
+["内蒙古自治区","乌海市",106.795460,39.653840],
+["内蒙古自治区","赤峰市",118.888940,42.258600],
+["内蒙古自治区","通辽市",122.244690,43.652470],
+["内蒙古自治区","鄂尔多斯市",109.780870,39.608450],
+["内蒙古自治区","呼伦贝尔市",119.765840,49.211630],
+["内蒙古自治区","巴彦淖尔市",107.387730,40.743170],
+["内蒙古自治区","乌兰察布市",113.133760,40.993910],
+["内蒙古自治区","兴安盟",122.038180,46.082080],
+["内蒙古自治区","锡林郭勒盟",116.047750,43.933200],
+["内蒙古自治区","阿拉善盟",105.728980,38.851530],
+["宁夏回族自治区","银川市",106.232480,38.486440],
+["宁夏回族自治区","石嘴山市",106.384180,38.984100],
+["宁夏回族自治区","吴忠市",106.198790,37.997550],
+["宁夏回族自治区","固原市",106.242590,36.015800],
+["宁夏回族自治区","中卫市",105.196760,37.500260],
+["西藏自治区","拉萨市",91.114500,29.644150],
+["西藏自治区","日喀则市",88.881160,29.267050],
+["西藏自治区","昌都市",97.172250,31.140730],
+["西藏自治区","林芝市",94.361550,29.648950],
+["西藏自治区","山南市",91.773130,29.237050],
+["西藏自治区","那曲市",92.051360,31.476140],
+["西藏自治区","阿里地区",81.145400,30.400510],
+["新疆维吾尔自治区","乌鲁木齐市",87.616880,43.826630],
+["新疆维吾尔自治区","克拉玛依市",84.889270,45.579990],
+["新疆维吾尔自治区","吐鲁番市",89.189540,42.951300],
+["新疆维吾尔自治区","哈密市",93.515380,42.818550],
+["新疆维吾尔自治区","昌吉回族自治州",87.308220,44.011170],
+["新疆维吾尔自治区","博尔塔拉蒙古自治州",82.066650,44.905970],
+["新疆维吾尔自治区","巴音郭楞蒙古自治州",86.145170,41.764040],
+["新疆维吾尔自治区","阿克苏地区",80.260080,41.168420],
+["新疆维吾尔自治区","克孜勒苏柯尔克孜自治州",76.166610,39.715300],
+["新疆维吾尔自治区","喀什地区",75.989760,39.470420],
+["新疆维吾尔自治区","和田地区",79.922470,37.114310],
+["新疆维吾尔自治区","伊犁哈萨克自治州",81.324160,43.916890],
+["新疆维吾尔自治区","塔城地区",82.980460,46.745320],
+["新疆维吾尔自治区","阿勒泰地区",88.140230,47.845640],
 ]
```

### Comparing `mbapy-0.0.9/mbapy.egg-info/SOURCES.txt` & `mbapy-0.1.0/mbapy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 mbapy/web.py
 mbapy.egg-info/PKG-INFO
 mbapy.egg-info/SOURCES.txt
 mbapy.egg-info/dependency_links.txt
 mbapy.egg-info/requires.txt
 mbapy.egg-info/top_level.txt
 mbapy/dl_torch/__init__.py
+mbapy/dl_torch/bb.py
 mbapy/dl_torch/data.py
+mbapy/dl_torch/hyper_search.py
 mbapy/dl_torch/loss.py
+mbapy/dl_torch/m.py
 mbapy/dl_torch/utils.py
+mbapy/dl_torch/paper/__init__.py
+mbapy/dl_torch/paper/bb.py
 mbapy/stats/__init__.py
+mbapy/stats/df.py
 mbapy/stats/geography.py
-mbapy/dl_torch/__init__.py
-mbapy/dl_torch/data.py
-mbapy/dl_torch/loss.py
-mbapy/dl_torch/utils.py
-mbapy/stats/__init__.py
-mbapy/stats/geography.py
+mbapy/stats/reg.py
+mbapy/stats/test.py
```

### Comparing `mbapy-0.0.9/setup.py` & `mbapy-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,99 @@
-'''
-Author: BHM-Bob 2262029386@qq.com
-Date: 2022-11-01 18:30:01
-LastEditors: BHM-Bob
-LastEditTime: 2023-03-21 00:37:37
-Description: 
-'''
-"""
-something is from https://github.com/pypa/sampleproject
-thanks to https://zetcode.com/python/package/
-"""
-
-"""A setuptools based setup module.
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
-import pathlib
-
-# Always prefer setuptools over distutils
-from setuptools import find_packages, setup
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-requires = [
-    "beautifulsoup4>=4.10.1",
-    "bokeh>=2.3.3",
-    "chardet>=5.0.0",
-    "cn2an>=0.5.17",
-    "holoviews>=1.13.1",
-    "imageio>=2.20.2",
-    "jieba>=0.42.1",
-    "Markdown>=3.4.1",
-    "matplotlib>=3.5.3",
-    "multiprocess>=0.70.13",
-    # "numpy>=1.22.1",
-    "pandas>=1.4.3",
-    "pathtools>=0.1.2",
-    "pdfkit>=1.0.0",
-    "Pillow>=9.2.0",
-    "plotly>=5.10.0",
-    "requests>=2.25.1",
-    "scikit-learn>=1.1.2",
-    "scipy>=1.5.1",
-    "seaborn>=0.11.2",
-    "selenium>=4.2.0",
-    "urllib3>=1.22.12",
-    "openpyxl",
-]
-
-setup(
-    name = "mbapy",
-    version = "0.0.9",
-
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Science/Research",
-        "Topic :: Utilities",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        # "Programming Language :: Python :: 3.11",# wait to numpy
-        # "Programming Language :: Python :: 3 :: Only",
-    ],
-        
-    keywords = ["mbapy", "Utilities", "plot"],
-    description = "MyBA in Python",
-    long_description = long_description,
-    long_description_content_type='text/markdown',
-    python_requires=">=3.7, <3.11",
-    license = "MIT Licence",
-
-    url = "https://github.com/BHM-Bob/BA_PY",
-    author = "BHM-Bob G",
-    author_email = "bhmfly@foxmail.com",
-    
-    # packages=["mbapy"],
-    packages=["mbapy", "mbapy/stats", "mbapy/dl_torch"],
-    
-    include_package_data = True,
-    platforms = "any",
-    
-    install_requires=requires,
-)
-
-# python setup.py sdist
-# twine upload dist/mbapy-0.0.8.tar.gz
+'''
+Author: BHM-Bob 2262029386@qq.com
+Date: 2022-11-01 18:30:01
+LastEditors: BHM-Bob 2262029386@qq.com
+LastEditTime: 2023-05-22 16:21:54
+Description: 
+'''
+"""
+something is from https://github.com/pypa/sampleproject
+thanks to https://zetcode.com/python/package/
+"""
+
+"""A setuptools based setup module.
+See:
+https://packaging.python.org/guides/distributing-packages-using-setuptools/
+https://github.com/pypa/sampleproject
+"""
+
+import pathlib
+
+# Always prefer setuptools over distutils
+from setuptools import find_packages, setup
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+requires = [
+    "beautifulsoup4>=4.10.1",
+    "bokeh>=2.3.3",
+    "chardet>=5.0.0",
+    "cn2an>=0.5.17",
+    "holoviews>=1.13.1",
+    "imageio>=2.20.2",
+    "jieba>=0.42.1",
+    "Markdown>=3.4.1",
+    "matplotlib>=3.5.3",
+    "multiprocess>=0.70.13",
+    # "numpy>=1.22.1",
+    "pandas>=1.4.3",
+    "pathtools>=0.1.2",
+    "pdfkit>=1.0.0",
+    "Pillow>=9.2.0",
+    "plotly>=5.10.0",
+    "requests>=2.25.1",
+    "scikit-learn>=1.1.2",
+    "scipy>=1.5.1",
+    "seaborn>=0.11.2",
+    "selenium>=4.2.0",
+    "urllib3>=1.22.12",
+    "openpyxl",
+    "statsmodels",
+    "scikit_posthocs",
+]
+
+setup(
+    name = "mbapy",
+    version = "0.1.0",
+
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Science/Research",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        # "Programming Language :: Python :: 3.11",# wait to numpy
+        # "Programming Language :: Python :: 3 :: Only",
+    ],
+        
+    keywords = ["mbapy", "Utilities", "plot"],
+    description = "MyBA in Python",
+    long_description = long_description,
+    long_description_content_type='text/markdown',
+    python_requires=">=3.7, <3.11",
+    license = "MIT Licence",
+
+    url = "https://github.com/BHM-Bob/BA_PY",
+    author = "BHM-Bob G",
+    author_email = "bhmfly@foxmail.com",
+    
+    # packages=["mbapy"],
+    packages=["mbapy", "mbapy/stats", "mbapy/dl_torch", "mbapy/dl_torch/paper"],
+    
+    include_package_data = True,
+    platforms = "any",
+    
+    install_requires=requires,
+)
+
+# pip install .
+
+
+# python setup.py sdist
+# twine upload dist/mbapy-0.0.15.tar.gz
```

