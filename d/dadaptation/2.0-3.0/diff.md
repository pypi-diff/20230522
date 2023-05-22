# Comparing `tmp/dadaptation-2.0.tar.gz` & `tmp/dadaptation-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/private/home/adefazio/dadaptation/dist/.tmp-ylrxb0c3/dadaptation-2.0.tar", last modified: Thu Apr 20 15:42:27 2023, max compression
+gzip compressed data, was "dist/dadaptation-3.0.tar", last modified: Mon May 22 15:06:30 2023, max compression
```

## Comparing `dadaptation-2.0.tar` & `dadaptation-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-2.0/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2747 2023-04-20 15:42:27.000000 dadaptation-2.0/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2286 2023-04-20 15:38:30.000000 dadaptation-2.0/README.md
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      148 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9168 2023-02-09 18:31:57.000000 dadaptation-2.0/dadaptation/dadapt_adagrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9012 2023-04-18 15:13:04.000000 dadaptation-2.0/dadaptation/dadapt_adam.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9593 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/dadapt_adan.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7131 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/dadapt_sgd.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation/experimental/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      121 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8230 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_adam_ip.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9737 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_adan_ip.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7213 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_sgd_ip.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2747 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      480 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-2.0/pyproject.toml
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-04-20 15:42:27.000000 dadaptation-2.0/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-04-20 15:33:41.000000 dadaptation-2.0/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-3.0/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3327 2023-05-22 15:06:30.000000 dadaptation-3.0/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2829 2023-05-22 15:04:09.000000 dadaptation-3.0/README.md
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      184 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9568 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adagrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8764 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adam.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9511 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_adan.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5309 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_lion.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6974 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/dadapt_sgd.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation/experimental/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       94 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/experimental/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9113 2023-05-22 15:03:35.000000 dadaptation-3.0/dadaptation/experimental/dadapt_adam_preprint.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9737 2023-04-17 18:47:49.000000 dadaptation-3.0/dadaptation/experimental/dadapt_adan_ip.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-05-22 15:06:30.000000 dadaptation-3.0/dadaptation.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     3327 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      471 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-05-22 15:06:29.000000 dadaptation-3.0/dadaptation.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-3.0/pyproject.toml
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-05-22 15:06:30.000000 dadaptation-3.0/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-05-22 15:03:35.000000 dadaptation-3.0/setup.py
```

### Comparing `dadaptation-2.0/LICENSE` & `dadaptation-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dadaptation-2.0/PKG-INFO` & `dadaptation-3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 2.0
+Version: 3.0
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,31 +18,37 @@
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
+**NEW V3.0 release uses an improved algorithm that may give different results from past versions. The old version is still availiable under experimental/d_adapt_adam_preprint.**
+
 ## Details
 
 The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
- - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
+ - **Set the LR parameter to 1.0**. This parameter is not ignored. Setting it larger to smaller will directly scale up or down the D-Adapted learning rate estimate.
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
- - Only the AdaGrad version supports sparse gradients.
- - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
+ - Only the AdaGrad version supports sparse gradients. It does not adapt as efficiently as the other variants and should be considered experimental.
  - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
 ## Change Log
 
+### Version 3.0
+ - Major improvements to DAdaptAdam, improving the performance particularly on Transformer models. This variant may behave differently in practice. The old version is availiable under experimental/d_adapt_adam_preprint if you wish to continue to use it.
+ - The IP variant is now the main variant of the method.
+ - Added Lion. This is highly experimental. Feedback on it's performance is welcome.
+
 ### Version 2.0
- - Added DAdaptAdan - should still be considered experimental.
+ - Added Adan - should still be considered experimental.
  - Added support for PyTorch's Fully Sharded Data Parallel. 
  - Improved support of edge cases such as learning rate zero.
  - Improved logging - uses Python logging rather than print statements
 
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
@@ -52,7 +60,9 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
+
+
```

### Comparing `dadaptation-2.0/README.md` & `dadaptation-3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
+**NEW V3.0 release uses an improved algorithm that may give different results from past versions. The old version is still availiable under experimental/d_adapt_adam_preprint.**
+
 ## Details
 
 The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
- - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
+ - **Set the LR parameter to 1.0**. This parameter is not ignored. Setting it larger to smaller will directly scale up or down the D-Adapted learning rate estimate.
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
- - Only the AdaGrad version supports sparse gradients.
- - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
+ - Only the AdaGrad version supports sparse gradients. It does not adapt as efficiently as the other variants and should be considered experimental.
  - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
 ## Change Log
 
+### Version 3.0
+ - Major improvements to DAdaptAdam, improving the performance particularly on Transformer models. This variant may behave differently in practice. The old version is availiable under experimental/d_adapt_adam_preprint if you wish to continue to use it.
+ - The IP variant is now the main variant of the method.
+ - Added Lion. This is highly experimental. Feedback on it's performance is welcome.
+
 ### Version 2.0
- - Added DAdaptAdan - should still be considered experimental.
+ - Added Adan - should still be considered experimental.
  - Added support for PyTorch's Fully Sharded Data Parallel. 
  - Improved support of edge cases such as learning rate zero.
  - Improved logging - uses Python logging rather than print statements
 
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
```

### Comparing `dadaptation-2.0/dadaptation/dadapt_adagrad.py` & `dadaptation-3.0/dadaptation/dadapt_adagrad.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,30 @@
 
 import math
 from typing import TYPE_CHECKING, Any, Callable, Optional
 
 import torch
 import torch.optim
 import pdb
+import logging
 
 if TYPE_CHECKING:
     from torch.optim.optimizer import _params_t
 else:
     _params_t = Any
 
 
 class DAdaptAdaGrad(torch.optim.Optimizer):
     """
-    Adagrad with D-Adaptation. Leave LR set to 1 unless you encounter instability.
+    Adagrad with D-Adaptation. We recommend Adam or SGD be used instead in most situations, 
+    as D-Adaptation on top of AdaGrad does not adapt the learning rate as quickly in 
+    practice as the other variants.
+
+    Leave LR set to 1 unless you encounter instability.
+
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
@@ -105,14 +111,16 @@
             k = group['k']
             decay = group['weight_decay']
 
             ######
             for p in group['params']:
                 if p.grad is None:
                     continue
+                if hasattr(p, "_fsdp_flattened"):
+                    raise RuntimeError("D-Adapt AdaGrad doesn't currently support fully-sharded data parallel. Use D-Adapt Adam instead")
                 grad = p.grad.data
 
                 state = self.state[p]
                 
                 if "alphak" not in state:
                     state["alphak"] = torch.full_like(p.data, fill_value=1e-6).detach()
                     state['sk'] = torch.zeros_like(p.data).detach()
@@ -201,15 +209,15 @@
         d_hat = d
         
         if lr > 0.0:
             d_hat = (sksq_weighted - gsq_weighted)/skl1
             d = group['d'] = max(d, min(d_hat, d*growth_rate))
 
         if log_every > 0 and k % log_every == 0:
-            print(f"d_hat: {d_hat}, d: {d}. sksq_weighted={sksq_weighted:1.1e} skl1={skl1:1.1e} gsq_weighted={gsq_weighted:1.1e} lr={lr}")
+            logging.info(f"d_hat: {d_hat}, d: {d}. sksq_weighted={sksq_weighted:1.1e} skl1={skl1:1.1e} gsq_weighted={gsq_weighted:1.1e} lr={lr}")
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
             group['skl1'] = skl1
             group['sksq_weighted'] = sksq_weighted
 
             group['d'] = d
```

### Comparing `dadaptation-2.0/dadaptation/dadapt_adam.py` & `dadaptation-3.0/dadaptation/experimental/dadapt_adam_preprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,20 @@
 
 def to_real(x):
     if torch.is_complex(x):
         return x.real
     else:
         return x
 
-class DAdaptAdam(torch.optim.Optimizer):
+class DAdaptAdamPreprint(torch.optim.Optimizer):
     r"""
-    Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    
+    This is an earlier variant of D-Adapt Adam used in early preprints of the paper, and source
+    code releases V1 and V2. Use this if you encounter performance regressions after the latest update.
+
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
@@ -241,8 +244,8 @@
 
 
                 ### Take step
                 p.data.addcdiv_(exp_avg, denom, value=-1)
 
             group['k'] = k + 1
 
-        return loss
+        return loss
```

### Comparing `dadaptation-2.0/dadaptation/dadapt_adan.py` & `dadaptation-3.0/dadaptation/dadapt_adan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 # 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-import math
-from typing import TYPE_CHECKING, Any, Callable, Optional
+from typing import TYPE_CHECKING, Any
 
 import torch
 import torch.optim
-import pdb
-import logging
-import os
 
 if TYPE_CHECKING:
     from torch.optim.optimizer import _params_t
 else:
     _params_t = Any
 
+
 def to_real(x):
     if torch.is_complex(x):
         return x.real
     else:
         return x
 
+
 class DAdaptAdan(torch.optim.Optimizer):
     r"""
     Implements Adan with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
     Adan was proposed in
     Adan: Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models[J]. arXiv preprint arXiv:2208.06677, 2022.
     https://arxiv.org/abs/2208.06677
     Arguments:
@@ -161,15 +159,15 @@
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(to_real(p.data), memory_format=torch.preserve_format).detach()
                     
                 if state['step'] == 0:
                     # Previous gradient values
                     state['pre_grad'] = grad.clone()
 
-                exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_diff'], state['exp_avg_sq']
+                exp_avg, exp_avg_diff, exp_avg_sq = state['exp_avg'], state['exp_avg_diff'], state['exp_avg_sq']
                 grad_diff = grad - state['pre_grad']
                 
                 grad_grad = to_real(grad * grad.conj())
                 update = grad + beta2 * grad_diff
                 update_update = to_real(update * update.conj())
                 
                 exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1. - beta1))
@@ -213,16 +211,16 @@
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
 
                 state = self.state[p]
 
-                exp_avg, exp_avg_sq, exp_avg_diff = state['exp_avg'], state['exp_avg_diff'], state['exp_avg_sq']
-                
+                exp_avg, exp_avg_diff, exp_avg_sq = state['exp_avg'], state['exp_avg_diff'], state['exp_avg_sq']
+
                 state['step'] += 1
                 
                 denom = exp_avg_sq.sqrt().add_(eps)
                 denom = denom.type(p.type())
                 
                 update = (exp_avg + beta2 * exp_avg_diff).div_(denom)
```

### Comparing `dadaptation-2.0/dadaptation/dadapt_sgd.py` & `dadaptation-3.0/dadaptation/dadapt_sgd.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 import pdb
 import math
 import logging
 import torch.distributed as dist
 
 class DAdaptSGD(torch.optim.Optimizer):
     r"""
-    Implements SGD with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
-        betas (Tuple[float, float], optional): coefficients used for computing
-            running averages of gradient and its square (default: (0.9, 0.999))
         momentum (float): 
-            Momentum value in  the range [0,1) (default: 0.9).
+            Momentum value in  the range [0,1) (default: 0).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
@@ -36,156 +35,155 @@
         fsdp_in_use (bool):
             If you're using sharded parameters, this should be set to True. The optimizer
             will attempt to auto-detect this, but if you're using an implementation other
             than PyTorch's builtin version, the auto-detection won't work.
     """
     def __init__(self, params, 
         lr=1.0, 
-        momentum=0, 
+        momentum=0.0, 
         weight_decay=0, 
         log_every=0,
         d0=1e-6, growth_rate=float('inf'),
         fsdp_in_use=False):
 
-        if d0 <= 0:
+        if not 0.0 < d0:
             raise ValueError("Invalid d0 value: {}".format(d0))
-        if lr <= 0:
+        if not 0.0 < lr:
             raise ValueError("Invalid learning rate: {}".format(lr))
 
         defaults = dict(lr=lr,
             momentum=momentum, 
-            weight_decay=weight_decay, 
-            k=0,
+            weight_decay=weight_decay, k=0,
             log_every=log_every,
-            gsq_weighted=0.0, 
-            g0_norm=0.0,
+            numerator_weighted=0.0, 
             d=d0, 
             growth_rate=growth_rate,
             fsdp_in_use=fsdp_in_use)
         self.loggables = {}
 
         try:
             self.rank = torch.distributed.get_rank()
         except:
             self.rank = 0
 
-        #self.group = dist.new_group(range(dist.get_world_size()))
-
         super().__init__(params, defaults)
 
     def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
 
+        group = self.param_groups[0]
         lr = max(group['lr'] for group in self.param_groups)
 
-        # Stored at the group level to ensure resuming from checkpoints works
-        group = self.param_groups[0]
         decay = group['weight_decay']
         momentum = group['momentum']
         log_every = group['log_every']
         ck = 1 - momentum
         k = group['k']
 
-        gsq_weighted = group['gsq_weighted']
-        g0_norm = group['g0_norm']
+        numerator_weighted = group['numerator_weighted']
         growth_rate = group['growth_rate']
-        fsdp_in_use = group['fsdp_in_use']
         d = group['d']
-
-        g_sq = 0.0
+        fsdp_in_use = group['fsdp_in_use']
+        
+        group = self.param_groups[0]
+        
         sk_sq = 0.0
 
-        for group in self.param_groups:
-            group_lr = group['lr']
-            if group_lr not in [lr, 0.0]:
-                raise RuntimeError(f"Setting different lr values in different parameter groups is only supported for values of 0")
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-                if hasattr(p, "_fsdp_flattened"):
-                    fsdp_in_use = True
-                grad = p.grad.data
-                
-                # Apply weight decay
-                if decay != 0:
-                    if grad.is_sparse:
-                        raise RuntimeError("weight_decay option is not compatible with sparse gradients")
-
-                    grad.add_(p.data, alpha=decay)
-
-                state = self.state[p]
+        if k == 0: 
+            g_sq = 0.0
+            for group in self.param_groups:
+                group_lr = group['lr']
+                for p in group['params']:
+                    if p.grad is None:
+                        continue
+                    if hasattr(p, "_fsdp_flattened"):
+                        fsdp_in_use = True
+                    grad = p.grad.data
+                    
+                    # Apply weight decay
+                    if decay != 0:
+                        grad.add(p.data, alpha=decay)
 
-                if group_lr > 0.0:
-                    g_sq += (grad * grad).sum().item()
+                    state = self.state[p]
 
-        # if we have any gradients available, will have g_sq > 0 (unless \|g\|=0)
-        if g_sq == 0:
-            return loss
+                    if group_lr > 0.0:
+                        g_sq += (grad * grad).sum().item()
 
-        if k == 0: 
             if fsdp_in_use:
                 dist_tensor = torch.zeros(1).cuda()
                 dist_tensor[0] = g_sq
                 dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
                 global_gsq = dist_tensor[0]
             else:
                 global_gsq = g_sq
-            g0_norm = math.sqrt(global_gsq)
+            group['g0_norm'] = g0_norm = math.sqrt(global_gsq)
+
+        g0_norm = group['g0_norm']
 
         dlr = d*lr/g0_norm
 
         for group in self.param_groups:
             group_lr = group['lr']
+            if group_lr not in [lr, 0.0]:
+                raise RuntimeError(f"Setting different lr values in different parameter groups is only supported for values of 0")
+            
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
                 state = self.state[p]
 
                 if 'z' not in state:
                     z = state['z'] = torch.clone(p.data).detach()
                     s = state['s'] = torch.zeros_like(p.data).detach()
                     x0 = state['x0'] = torch.clone(p.data).detach()
 
+                # Apply weight decay
+                if decay != 0:
+                    grad.add_(p.data, alpha=decay)
+
                 s = state['s']
 
                 if group_lr > 0.0:
+                    numerator_weighted += dlr * torch.dot(grad.flatten(), s.flatten()).item()
+                    
                     s.data.add_(grad, alpha=dlr)
-                
-                sk_sq += (s * s).sum().item()
+                    sk_sq += (s * s).sum().item()
             ######
 
-        gsq_weighted = gsq_weighted + dlr*dlr*g_sq
         d_hat = d
 
         if lr > 0.0:
             if fsdp_in_use:
                 dist_tensor = torch.zeros(2).cuda()
                 dist_tensor[0] = sk_sq
-                dist_tensor[1] = gsq_weighted
+                dist_tensor[1] = numerator_weighted
                 dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
                 global_sk_sq = dist_tensor[0]
-                global_gsq_weighted = dist_tensor[1]
+                global_numerator_weighted = dist_tensor[1]
             else:
                 global_sk_sq = sk_sq
-                global_gsq_weighted = gsq_weighted
+                global_numerator_weighted = numerator_weighted
 
-            d_hat = (global_sk_sq - global_gsq_weighted)/(math.sqrt(global_sk_sq))
-            d = group['d'] = max(d, min(d_hat, d*growth_rate))
+            d_hat = 2*global_numerator_weighted/math.sqrt(global_sk_sq)
+            d = max(d, min(d_hat, d*growth_rate))
+
+
+        # if we have not done any updates
+        # if we have any gradients available, will have sk_sq > 0 (unless \|g\|=0)
+        if global_sk_sq == 0:
+            return loss
 
         if log_every > 0 and k % log_every == 0:
-            logging.info(
-                f"(k={k}) dlr: {dlr:1.1e} d_hat: {d_hat:1.1e}, d: {d:1.8}. "
-                f"sk_sq={global_sk_sq:1.1e} gsq_weighted={global_gsq_weighted:1.1e} "
-                f"g0_norm={g0_norm:1.1e}{' (FSDP)' if fsdp_in_use else ''}")
+            logging.info(f"(r={self.rank},k={k}) dlr: {dlr} d_hat: {d_hat}, d: {d}. sk_norm={math.sqrt(global_sk_sq)} numerator_weighted={global_numerator_weighted} g0_norm={g0_norm}")
 
         for group in self.param_groups:
-            group['gsq_weighted'] = gsq_weighted
+            group['numerator_weighted'] = numerator_weighted
             group['d'] = d
             group['g0_norm'] = g0_norm
             ######################################
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
@@ -199,9 +197,8 @@
                 z.data.copy_(x0 - s)
 
                 # x step
                 p.data.mul_(1-ck).add_(z, alpha=ck)
 
             group['k'] = k + 1
 
-        return loss
-
+        return loss
```

### Comparing `dadaptation-2.0/dadaptation/experimental/dadapt_adam_ip.py` & `dadaptation-3.0/dadaptation/dadapt_adam.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,40 +15,36 @@
 import torch.distributed as dist
 
 if TYPE_CHECKING:
     from torch.optim.optimizer import _params_t
 else:
     _params_t = Any
 
-class DAdaptAdamIP(torch.optim.Optimizer):
+class DAdaptAdam(torch.optim.Optimizer):
     r"""
     Implements Adam with D-Adaptation automatic step-sizes. 
     Leave LR set to 1 unless you encounter instability.
-
-    This IP variant uses a tighter bound than the non-IP version,
-    and so will typically choose larger step sizes. It has not 
-    been as extensively tested.
     
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
-        momentum (float): 
-            Momentum value in  the range [0,1) (default: 0.9).
         eps (float): 
             Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
         decouple (boolean): 
             Use AdamW style decoupled weight decay
+        use_bias_correction (boolean):
+            Turn on Adam's bias correction. Off by default.
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
             prevent the D estimate from growing faster than this multiplicative rate. 
             Default is inf, for unrestricted. Values like 1.02 give a kind of learning
             rate warmup effect.
         fsdp_in_use (bool):
@@ -56,14 +52,15 @@
             will attempt to auto-detect this, but if you're using an implementation other
             than PyTorch's builtin version, the auto-detection won't work.
     """
     def __init__(self, params, lr=1.0, 
                  betas=(0.9, 0.999), eps=1e-8,
                  weight_decay=0, log_every=0,
                  decouple=False,
+                 use_bias_correction=False,
                  d0=1e-6, growth_rate=float('inf'),
                  fsdp_in_use=False):
         if not 0.0 < d0:
             raise ValueError("Invalid d0 value: {}".format(d0))
         if not 0.0 < lr:
             raise ValueError("Invalid learning rate: {}".format(lr))
         if not 0.0 < eps:
@@ -80,14 +77,15 @@
         defaults = dict(lr=lr, betas=betas, eps=eps,
                         weight_decay=weight_decay,
                         d = d0, 
                         k=0, 
                         numerator_weighted=0.0,
                         log_every=log_every,
                         growth_rate=growth_rate,
+                        use_bias_correction=use_bias_correction,
                         decouple=decouple,
                         fsdp_in_use=fsdp_in_use)
         self.d0 = d0
         super().__init__(params, defaults)
 
     @property
     def supports_memory_efficient_fp16(self):
@@ -107,33 +105,47 @@
         loss = None
         if closure is not None:
             loss = closure()
 
         sk_l1 = 0.0
 
         group = self.param_groups[0]
+        use_bias_correction = group['use_bias_correction']
         numerator_weighted = group['numerator_weighted']
+        beta1, beta2 = group['betas']
+        k = group['k']
+
         d = group['d']
         lr = max(group['lr'] for group in self.param_groups)
 
-        dlr = d*lr
+        if use_bias_correction:
+            bias_correction = ((1-beta2**(k+1))**0.5)/(1-beta1**(k+1))
+        else:
+            bias_correction = 1
+
+        dlr = d*lr*bias_correction
         
         growth_rate = group['growth_rate']
         decouple = group['decouple']
         log_every = group['log_every']
         fsdp_in_use = group['fsdp_in_use']
 
-        beta1, beta2 = group['betas']
+        
+        sqrt_beta2 = beta2**(0.5)
 
         numerator_acum = 0.0
 
         for group in self.param_groups:
             decay = group['weight_decay']
             k = group['k']
             eps = group['eps']
+            group_lr = group['lr']
+
+            if group_lr not in [lr, 0.0]:
+                raise RuntimeError(f"Setting different lr values in different parameter groups is only supported for values of 0")
 
             for p in group['params']:
                 if p.grad is None:
                     continue
                 if hasattr(p, "_fsdp_flattened"):
                     fsdp_in_use = True
                 
@@ -154,48 +166,49 @@
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p.data).detach()
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 
                 s = state['s']
 
-                denom = exp_avg_sq.sqrt().add_(eps)
-                numerator_acum += dlr * torch.dot(grad.flatten(), s.div(denom).flatten()).item()
-
-                # Adam EMA updates
-                exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1-beta1))
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1-beta2)
+                if group_lr > 0.0:
+                    denom = exp_avg_sq.sqrt().add_(eps)
+                    numerator_acum += dlr * torch.dot(grad.flatten(), s.div(denom).flatten()).item()
+
+                    # Adam EMA updates
+                    exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1-beta1))
+                    exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1-beta2)
 
-                s.mul_(beta2).add_(grad, alpha=dlr*(1-beta2))
-                sk_l1 += s.abs().sum().item()
+                    s.mul_(sqrt_beta2).add_(grad, alpha=dlr*(1-sqrt_beta2))
+                    sk_l1 += s.abs().sum().item()
 
             ######
 
-        numerator_weighted = beta2*numerator_weighted + (1-beta2)*numerator_acum
+        numerator_weighted = sqrt_beta2*numerator_weighted + (1-sqrt_beta2)*numerator_acum
         d_hat = d
 
         # if we have not done any progres, return
         # if we have any gradients available, will have sk_l1 > 0 (unless \|g\|=0)
         if sk_l1 == 0:
             return loss
         
         if lr > 0.0:
             if fsdp_in_use:
-                dist_tensor = torch.zeros(3).cuda()
+                dist_tensor = torch.zeros(2).cuda()
                 dist_tensor[0] = numerator_weighted
                 dist_tensor[1] = sk_l1
                 dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
                 global_numerator_weighted = dist_tensor[0]
                 global_sk_l1 = dist_tensor[1]
             else:
                 global_numerator_weighted = numerator_weighted
                 global_sk_l1 = sk_l1
 
 
-            d_hat = 2*(beta2/(1-beta2))*global_numerator_weighted/global_sk_l1
+            d_hat = global_numerator_weighted/((1-sqrt_beta2)*global_sk_l1)
             d = max(d, min(d_hat, d*growth_rate))
 
         if log_every > 0 and k % log_every == 0:
             logging.info(f"lr: {lr} dlr: {dlr} d_hat: {d_hat}, d: {d}. sk_l1={global_sk_l1:1.1e} numerator_weighted={global_numerator_weighted:1.1e}")
 
         for group in self.param_groups:
             group['numerator_weighted'] = numerator_weighted
```

### Comparing `dadaptation-2.0/dadaptation/experimental/dadapt_adan_ip.py` & `dadaptation-3.0/dadaptation/experimental/dadapt_adan_ip.py`

 * *Files identical despite different names*

### Comparing `dadaptation-2.0/dadaptation.egg-info/PKG-INFO` & `dadaptation-3.0/dadaptation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 2.0
+Version: 3.0
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,31 +18,37 @@
 
 Learning rate free learning for SGD, AdaGrad and Adam! 
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
+**NEW V3.0 release uses an improved algorithm that may give different results from past versions. The old version is still availiable under experimental/d_adapt_adam_preprint.**
+
 ## Details
 
 The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
- - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
+ - **Set the LR parameter to 1.0**. This parameter is not ignored. Setting it larger to smaller will directly scale up or down the D-Adapted learning rate estimate.
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
- - Only the AdaGrad version supports sparse gradients.
- - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
+ - Only the AdaGrad version supports sparse gradients. It does not adapt as efficiently as the other variants and should be considered experimental.
  - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
 ## Change Log
 
+### Version 3.0
+ - Major improvements to DAdaptAdam, improving the performance particularly on Transformer models. This variant may behave differently in practice. The old version is availiable under experimental/d_adapt_adam_preprint if you wish to continue to use it.
+ - The IP variant is now the main variant of the method.
+ - Added Lion. This is highly experimental. Feedback on it's performance is welcome.
+
 ### Version 2.0
- - Added DAdaptAdan - should still be considered experimental.
+ - Added Adan - should still be considered experimental.
  - Added support for PyTorch's Fully Sharded Data Parallel. 
  - Improved support of edge cases such as learning rate zero.
  - Improved logging - uses Python logging rather than print statements
 
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
@@ -52,7 +60,9 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
+
+
```

### Comparing `dadaptation-2.0/setup.py` & `dadaptation-3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dadaptation",
-    version="2.0",
+    version="3.0",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Learning Rate Free Learning for Adam, SGD and AdaGrad",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/dadaptation",
     packages=setuptools.find_packages(),
```

