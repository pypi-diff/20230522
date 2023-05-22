# Comparing `tmp/foxai-0.5.3.tar.gz` & `tmp/foxai-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxai-0.5.3.tar", max compression
+gzip compressed data, was "foxai-0.5.4.tar", max compression
```

## Comparing `foxai-0.5.3.tar` & `foxai-0.5.4.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-02-22 12:38:27.816254 foxai-0.5.3/LICENSE
--rw-r--r--   0        0        0     7575 2023-02-22 12:38:27.816254 foxai-0.5.3/README.md
--rw-r--r--   0        0        0      162 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/__init__.py
--rw-r--r--   0        0        0     3735 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/array_utils.py
--rw-r--r--   0        0        0        0 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/callbacks/__init__.py
--rw-r--r--   0        0        0     8730 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/callbacks/wandb_callback.py
--rw-r--r--   0        0        0        0 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/cli/__init__.py
--rw-r--r--   0        0        0      486 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/cli/config_model.py
--rw-r--r--   0        0        0     7571 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/cli/experiment_update.py
--rw-r--r--   0        0        0     9308 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/context_manager.py
--rw-r--r--   0        0        0     1166 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/__init__.py
--rw-r--r--   0        0        0     1122 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/base_explainer.py
--rw-r--r--   0        0        0     8369 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/conductance.py
--rw-r--r--   0        0        0     4847 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/deconv.py
--rw-r--r--   0        0        0    13193 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/deeplift.py
--rw-r--r--   0        0        0    13361 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/deeplift_shap.py
--rw-r--r--   0        0        0    18593 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/gradcam.py
--rw-r--r--   0        0        0    12402 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/gradient_shap.py
--rw-r--r--   0        0        0     5064 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/guided_backprop.py
--rw-r--r--   0        0        0     8334 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/input_x_gradient.py
--rw-r--r--   0        0        0    14073 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/integrated_gradients.py
--rw-r--r--   0        0        0     7842 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/lrp.py
--rw-r--r--   0        0        0     1253 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/model_utils.py
--rw-r--r--   0        0        0     7576 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/noise_tunnel.py
--rw-r--r--   0        0        0     7994 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/occlusion.py
--rw-r--r--   0        0        0     4139 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/explainer/saliency.py
--rw-r--r--   0        0        0      752 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/logger.py
--rw-r--r--   0        0        0     6278 2023-02-22 12:38:27.824254 foxai-0.5.3/foxai/visualizer.py
--rw-r--r--   0        0        0     1920 2023-02-22 12:38:27.828255 foxai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     9134 1970-01-01 00:00:00.000000 foxai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 11:45:51.749264 foxai-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7626 2023-05-22 11:45:51.749264 foxai-0.5.4/README.md
+-rw-r--r--   0        0        0      162 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/__init__.py
+-rw-r--r--   0        0        0     3735 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/array_utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/callbacks/__init__.py
+-rw-r--r--   0        0        0     8744 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/config_model.py
+-rw-r--r--   0        0        0     7650 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/cli/experiment_update.py
+-rw-r--r--   0        0        0     9778 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/context_manager.py
+-rw-r--r--   0        0        0     1603 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/__init__.py
+-rw-r--r--   0        0        0     1118 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/base_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/__init__.py
+-rw-r--r--   0        0        0     8381 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/conductance.py
+-rw-r--r--   0        0        0     4859 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deconv.py
+-rw-r--r--   0        0        0    13218 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift.py
+-rw-r--r--   0        0        0    13386 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift_shap.py
+-rw-r--r--   0        0        0    24493 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradcam.py
+-rw-r--r--   0        0        0    12414 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradient_shap.py
+-rw-r--r--   0        0        0     5076 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/guided_backprop.py
+-rw-r--r--   0        0        0     8346 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/input_x_gradient.py
+-rw-r--r--   0        0        0    14085 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/integrated_gradients.py
+-rw-r--r--   0        0        0     7867 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/lrp.py
+-rw-r--r--   0        0        0     7588 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/noise_tunnel.py
+-rw-r--r--   0        0        0     7990 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/occlusion.py
+-rw-r--r--   0        0        0     4135 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/algorithm/saliency.py
+-rw-r--r--   0        0        0     1253 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/model_utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/__init__.py
+-rw-r--r--   0        0        0     2639 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/base_object_detector.py
+-rw-r--r--   0        0        0      679 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/types.py
+-rw-r--r--   0        0        0     1745 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/explainer/computer_vision/object_detection/utils.py
+-rw-r--r--   0        0        0      752 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/logger.py
+-rw-r--r--   0        0        0    10221 2023-05-22 11:45:51.753264 foxai-0.5.4/foxai/visualizer.py
+-rw-r--r--   0        0        0     1940 2023-05-22 11:45:51.757264 foxai-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     9185 1970-01-01 00:00:00.000000 foxai-0.5.4/PKG-INFO
```

### Comparing `foxai-0.5.3/LICENSE` & `foxai-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foxai-0.5.3/README.md` & `foxai-0.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     * [Note](#note)
         * [Artifacts directory structure](#artifacts-directory-structure)
         * [Examples](#examples)
 
 # Installation
 
 Installation requirements:
-* `Python` >= 3.7 & < 4.0
+* `Python` >=3.7.2,<3.11
 
 **Important**: For any problems regarding installation we advise to refer first to our [FAQ](FAQ.md).
 
 ## GPU acceleration
 
 To use the torch library with GPU acceleration, you need to install
 a dedicated version of torch with support for the installed version of CUDA
-drivers in the version supported by the library, at the moment `torch==1.12.1`.
+drivers in the version supported by the library, at the moment `torch>=1.12.1,<2.0.0`.
 A list of `torch` wheels with CUDA support can be found at
 [https://download.pytorch.org/whl/torch/](https://download.pytorch.org/whl/torch/).
 
 ## Manual installation
 
 If you would like to install from the source you can build a `wheel` package using `poetry`.
 The assumption is that the `poetry` package is installed. You can find how to install
@@ -68,27 +68,27 @@
 ```python
 import torch
 from pytorch_lightning import Trainer
 from pytorch_lightning.loggers import WandbLogger
 
 import wandb
 from foxai.callbacks.wandb_callback import WandBCallback
-from foxai.context_manager import Explainers, ExplainerWithParams
+from foxai.context_manager import CVClassificationExplainers, ExplainerWithParams
 
     ...
     wandb.login()
     wandb_logger = WandbLogger(project=project_name, log_model="all")
     callback = WandBCallback(
         wandb_logger=wandb_logger,
         explainers=[
             ExplainerWithParams(
-                explainer_name=Explainers.CV_INTEGRATED_GRADIENTS_EXPLAINER
+                explainer_name=CVClassificationExplainers.CV_INTEGRATED_GRADIENTS_EXPLAINER
             ),
             ExplainerWithParams(
-                explainer_name=Explainers.CV_GRADIENT_SHAP_EXPLAINER
+                explainer_name=CVClassificationExplainers.CV_GRADIENT_SHAP_EXPLAINER
             ),
         ],
         idx_to_label={index: index for index in range(0, 10)},
     )
     model = LitMNIST()
     trainer = Trainer(
         accelerator="gpu",
@@ -141,20 +141,20 @@
 ## CUDA
 
 The recommended version of CUDA is `10.2` as it is supported since version
 `1.5.0` of `torch`. You can check the compatibility of your CUDA version
 with the current version of `torch`:
 https://pytorch.org/get-started/previous-versions/.
 
-As our starting Docker image we were using the one provided by Nvidia: ``nvidia/cuda:10.2-devel-ubuntu18.04``. 
+As our starting Docker image we were using the one provided by Nvidia: ``nvidia/cuda:10.2-devel-ubuntu18.04``.
 
-If you wish an easy to use docker image we advise to use our ``Dockerfile``. 
+If you wish an easy to use docker image we advise to use our ``Dockerfile``.
 
 ## pyenv
-Optional step, but probably one of the easiest way to actually get Python version with all the needed aditional tools (e.g. pip). 
+Optional step, but probably one of the easiest way to actually get Python version with all the needed aditional tools (e.g. pip).
 
 `pyenv` is a tool used to manage multiple versions of Python. To install
 this package follow the instructions on the project repository page:
 https://github.com/pyenv/pyenv#installation. After installation You can
 install desired Python version, e.g. `3.8.16`:
 ```bash
 pyenv install 3.8.16
@@ -211,15 +211,15 @@
 Once all the steps have been completed, the environment is ready to go.
 A virtual environment by default will be created with the name `.venv` inside
 the project directory.
 
 ## Pre-commit hooks setup
 
 To improve the development experience, please make sure to install
-our [pre-commit][https://pre-commit.com/] hooks as the very first step after
+our [pre-commit](https://pre-commit.com/) hooks as the very first step after
 cloning the repository:
 
 ```bash
 poetry run pre-commit install
 ```
 
 ## Note
```

### Comparing `foxai-0.5.3/foxai/array_utils.py` & `foxai-0.5.4/foxai/array_utils.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.3/foxai/callbacks/wandb_callback.py` & `foxai-0.5.4/foxai/callbacks/wandb_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from collections import defaultdict
 from typing import Dict, Generator, List, Optional, Tuple, cast
 
 import matplotlib
 import numpy as np
 import pytorch_lightning as pl
 import torch
+import wandb
 from pytorch_lightning.loggers import WandbLogger
 from torch.utils.data import DataLoader
 
-import wandb
 from foxai.array_utils import convert_standardized_float_to_uint8, standardize_array
-from foxai.context_manager import FoXaiExplainer, ExplainerWithParams
+from foxai.context_manager import ExplainerWithParams, FoXaiExplainer
 from foxai.visualizer import mean_channels_visualization
 
 AttributeMapType = Dict[str, List[np.ndarray]]
 CaptionMapType = Dict[str, List[str]]
 FigureMapType = Dict[str, List[matplotlib.pyplot.Figure]]
 
 
@@ -114,15 +114,15 @@
             caption_dict[explainer_name].append(f"label: {target_label}")
             figure = mean_channels_visualization(
                 attributions=explainer_attributes,
                 transformed_img=item,
             )
             figures_dict[explainer_name].append(figure)
             standardized_attr = standardize_array(
-                explainer_attributes.detach().cpu().numpy()
+                explainer_attributes.detach().cpu().numpy().astype(float)
             )
 
             attributes_dict[explainer_name].append(
                 convert_standardized_float_to_uint8(standardized_attr),
             )
 
         return attributes_dict, caption_dict, figures_dict
```

### Comparing `foxai-0.5.3/foxai/cli/experiment_update.py` & `foxai-0.5.4/foxai/cli/experiment_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 import os
 from typing import Any, Dict, List, cast
 
 import hydra
 import pandas as pd
 import pytorch_lightning as pl
 import torch
+import wandb
 from omegaconf import DictConfig
 from torchvision.io import ImageReadMode, read_image
 
-import wandb
 from foxai.cli.config_model import ConfigDataModel, MethodDataModel
-from foxai.context_manager import FoXaiExplainer, Explainers, ExplainerWithParams
+from foxai.context_manager import (
+    CVClassificationExplainers,
+    ExplainerWithParams,
+    FoXaiExplainer,
+)
 
 
 def download_upload_metadata(api_run: wandb.apis.public.Run) -> Dict[str, Any]:
     """Fetch uploaded data samples metadata from logs history.
 
     Args:
         run_api: WandB Api object.
@@ -114,15 +118,17 @@
         ConfigDataModel object.
     """
 
     method_config_list: List[MethodDataModel] = []
     for entry in config["explainers"]:
         explainer_config: Dict[str, Any] = entry["explainer_with_params"]
         explainer: ExplainerWithParams = ExplainerWithParams(
-            explainer_name=Explainers[explainer_config["explainer_name"]],
+            explainer_name=CVClassificationExplainers[
+                explainer_config["explainer_name"]
+            ],
             kwargs=explainer_config.get("kwargs", {}),
         )
         method_config_list.append(
             MethodDataModel(
                 explainer_with_params=explainer,
                 artifact_name=entry.get("artifact_name", None),
             )
```

### Comparing `foxai-0.5.3/foxai/context_manager.py` & `foxai-0.5.4/foxai/context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         target=pred_label_idx,
     ) as xai_model:
         output, xai_explanations = xai_model(img_tensor)
 """
 import logging
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Dict, Generic, List, Optional, Tuple, cast
+from typing import Any, Dict, Generic, List, Optional, Tuple, Union, cast
 
 import torch
 
 from foxai import explainer
 from foxai.explainer import (
     DeconvolutionCVExplainer,
     DeepLIFTCVExplainer,
@@ -32,14 +32,15 @@
     GuidedGradCAMCVExplainer,
     InputXGradientCVExplainer,
     IntegratedGradientsCVExplainer,
     LayerConductanceCVExplainer,
     LayerDeepLIFTCVExplainer,
     LayerDeepLIFTSHAPCVExplainer,
     LayerGradCAMCVExplainer,
+    LayerGradCAMObjectDetectionExplainer,
     LayerGradientSHAPCVExplainer,
     LayerInputXGradientCVExplainer,
     LayerIntegratedGradientsCVExplainer,
     LayerLRPCVExplainer,
     LayerNoiseTunnelCVExplainer,
     LRPCVExplainer,
     NoiseTunnelCVExplainer,
@@ -57,16 +58,16 @@
     # pylint: disable = global-statement
     global _LOGGER
     if _LOGGER is None:
         _LOGGER = create_logger(__name__)
     return _LOGGER
 
 
-class Explainers(Enum):
-    """Enum of supported explainers types."""
+class CVClassificationExplainers(Enum):
+    """Enum of supported computer vision classification explainers types."""
 
     CV_OCCLUSION_EXPLAINER: str = OcclusionCVExplainer.__name__
     CV_INTEGRATED_GRADIENTS_EXPLAINER: str = IntegratedGradientsCVExplainer.__name__
     CV_NOISE_TUNNEL_EXPLAINER: str = NoiseTunnelCVExplainer.__name__
     CV_GRADIENT_SHAP_EXPLAINER: str = GradientSHAPCVExplainer.__name__
     CV_LRP_EXPLAINER: str = LRPCVExplainer.__name__
     CV_GUIDEDGRADCAM_EXPLAINER: str = GuidedGradCAMCVExplainer.__name__
@@ -85,22 +86,34 @@
     CV_LAYER_DEEPLIFT_SHAP_EXPLAINER: str = LayerDeepLIFTSHAPCVExplainer.__name__
     CV_DECONVOLUTION_EXPLAINER: str = DeconvolutionCVExplainer.__name__
     CV_LAYER_CONDUCTANCE_EXPLAINER: str = LayerConductanceCVExplainer.__name__
     CV_SALIENCY_EXPLAINER: str = SaliencyCVExplainer.__name__
     CV_GUIDED_BACKPOPAGATION_EXPLAINER: str = GuidedBackpropCVExplainer.__name__
 
 
+class CVObjectDetectionExplainers(Enum):
+    """Enum of supported computer vision object detection explainers types."""
+
+    CV_LAYER_GRADCAM_OBJECT_DETECTION_EXPLAINER: str = (
+        LayerGradCAMObjectDetectionExplainer.__name__
+    )
+
+
 @dataclass
 class ExplainerWithParams:
     """Holder for explainer name (class name) and it's params"""
 
-    explainer_name: Explainers
+    explainer_name: Union[CVClassificationExplainers, CVObjectDetectionExplainers]
     kwargs: Dict[str, Any] = field(default_factory=dict)
 
-    def __init__(self, explainer_name: Explainers, **kwargs) -> None:
+    def __init__(
+        self,
+        explainer_name: Union[CVClassificationExplainers, CVObjectDetectionExplainers],
+        **kwargs
+    ) -> None:
         self.explainer_name = explainer_name
         if kwargs:
             self.kwargs = kwargs
         else:
             self.kwargs = {}
```

### Comparing `foxai-0.5.3/foxai/explainer/base_explainer.py` & `foxai-0.5.4/foxai/explainer/base_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import ABC, abstractmethod
 from typing import TypeVar
 
 import torch
 from captum._utils.typing import TargetType
 
 
-class CVExplainer(ABC):
+class Explainer(ABC):
     """Abstract explainer class."""
 
     # TODO: add support in explainer for multiple input models
     @abstractmethod
     def calculate_features(
         self,
         model: torch.nn.Module,
@@ -35,9 +35,9 @@
 
         Returns:
             str: Name of algorithm.
         """
         return type(self).__name__
 
 
-CVExplainerT = TypeVar("CVExplainerT", bound=CVExplainer)
+CVExplainerT = TypeVar("CVExplainerT", bound=Explainer)
 """CVExplainer subclass type."""
```

### Comparing `foxai-0.5.3/foxai/explainer/conductance.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/conductance.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from typing import Any, Optional, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import LayerConductance
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import get_last_conv_model_layer
 
 
-class LayerConductanceCVExplainer(CVExplainer):
+class LayerConductanceCVExplainer(Explainer):
     """Layer Conductance algorithm explainer."""
 
     # pylint: disable = unused-argument
     def create_explainer(
         self,
         model: torch.nn.Module,
         layer: torch.nn.Module,
```

### Comparing `foxai-0.5.3/foxai/explainer/deconv.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deconv.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Any
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import Deconvolution
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import modify_modules
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import modify_modules
 
 
-class BaseDeconvolutionCVExplainer(CVExplainer):
+class BaseDeconvolutionCVExplainer(Explainer):
     """Base Deconvolution algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
     ) -> Deconvolution:
```

### Comparing `foxai-0.5.3/foxai/explainer/deeplift.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 from typing import Any, Callable, Optional, Tuple, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import DeepLift, LayerDeepLift
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer, modify_modules
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import (
+    get_last_conv_model_layer,
+    modify_modules,
+)
 
 
-class BaseDeepLIFTCVExplainer(CVExplainer):
+class BaseDeepLIFTCVExplainer(Explainer):
     """Base DeepLIFT algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         multiply_by_inputs: bool = True,
```

### Comparing `foxai-0.5.3/foxai/explainer/deeplift_shap.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/deeplift_shap.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 from typing import Any, Callable, Optional, Tuple, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import DeepLiftShap, LayerDeepLiftShap
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer, modify_modules
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import (
+    get_last_conv_model_layer,
+    modify_modules,
+)
 
 
-class BaseDeepLIFTSHAPCVExplainer(CVExplainer):
+class BaseDeepLIFTSHAPCVExplainer(Explainer):
     """Base DeepLIFT SHAP algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         multiply_by_inputs: bool = True,
```

### Comparing `foxai-0.5.3/foxai/explainer/gradient_shap.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/gradient_shap.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from typing import Any, Optional, Tuple, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import GradientShap, LayerGradientShap
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import get_last_conv_model_layer
 
 
-class BaseGradientSHAPCVExplainer(CVExplainer):
+class BaseGradientSHAPCVExplainer(Explainer):
     """Base Gradient SHAP algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         multiply_by_inputs: bool = True,
```

### Comparing `foxai-0.5.3/foxai/explainer/guided_backprop.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/guided_backprop.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Any
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import GuidedBackprop
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import modify_modules
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import modify_modules
 
 
-class BaseGuidedBackpropCVExplainer(CVExplainer):
+class BaseGuidedBackpropCVExplainer(Explainer):
     """Base Guided Backpropagation algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         **kwargs,
```

### Comparing `foxai-0.5.3/foxai/explainer/input_x_gradient.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/input_x_gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from typing import Any, Optional, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import InputXGradient, LayerGradientXActivation
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import get_last_conv_model_layer
 
 
-class BaseInputXGradientSHAPCVExplainer(CVExplainer):
+class BaseInputXGradientSHAPCVExplainer(Explainer):
     """Base Input X Gradient algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         **kwargs,
```

### Comparing `foxai-0.5.3/foxai/explainer/integrated_gradients.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/integrated_gradients.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from typing import Any, Optional, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import IntegratedGradients, LayerIntegratedGradients
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import get_last_conv_model_layer
 
 
-class BaseIntegratedGradientsCVExplainer(CVExplainer):
+class BaseIntegratedGradientsCVExplainer(Explainer):
     """Base Integrated Gradients algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         multiply_by_inputs: bool = True,
```

### Comparing `foxai-0.5.3/foxai/explainer/lrp.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/lrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import LRP, LayerLRP
 from captum.attr._utils.lrp_rules import EpsilonRule, GammaRule
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer, modify_modules
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import (
+    get_last_conv_model_layer,
+    modify_modules,
+)
 
 
-class BaseLRPCVExplainer(CVExplainer):
+class BaseLRPCVExplainer(Explainer):
     """Base LRP algorithm explainer."""
 
     @abstractmethod
     def create_explainer(
         self,
         model: torch.nn.Module,
         **kwargs,
```

### Comparing `foxai-0.5.3/foxai/explainer/model_utils.py` & `foxai-0.5.4/foxai/explainer/computer_vision/model_utils.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.3/foxai/explainer/noise_tunnel.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/noise_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Optional, Tuple, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import IntegratedGradients, LayerIntegratedGradients, NoiseTunnel
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
-from foxai.explainer.model_utils import get_last_conv_model_layer
+from foxai.explainer.base_explainer import Explainer
+from foxai.explainer.computer_vision.model_utils import get_last_conv_model_layer
 
 
-class BaseNoiseTunnelCVExplainer(CVExplainer):
+class BaseNoiseTunnelCVExplainer(Explainer):
     """Base Noise Tunnel algorithm explainer."""
 
     @abstractmethod
     def create_explainer(self, model: torch.nn.Module, **kwargs) -> NoiseTunnel:
         """Create explainer object.
 
         Args:
```

### Comparing `foxai-0.5.3/foxai/explainer/occlusion.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/occlusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from typing import Any, Tuple, Union
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import Occlusion
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
+from foxai.explainer.base_explainer import Explainer
 
 
-class OcclusionCVExplainer(CVExplainer):
+class OcclusionCVExplainer(Explainer):
     """Occlusion algorithm explainer."""
 
     def calculate_features(
         self,
         model: torch.nn.Module,
         input_data: torch.Tensor,
         pred_label_idx: TargetType = None,
```

### Comparing `foxai-0.5.3/foxai/explainer/saliency.py` & `foxai-0.5.4/foxai/explainer/computer_vision/algorithm/saliency.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from typing import Any
 
 import torch
 from captum._utils.typing import TargetType
 from captum.attr import Saliency
 
 from foxai.array_utils import validate_result
-from foxai.explainer.base_explainer import CVExplainer
+from foxai.explainer.base_explainer import Explainer
 
 
-class SaliencyCVExplainer(CVExplainer):
+class SaliencyCVExplainer(Explainer):
     """Saliency algorithm explainer."""
 
     def calculate_features(
         self,
         model: torch.nn.Module,
         input_data: torch.Tensor,
         pred_label_idx: TargetType = None,
```

### Comparing `foxai-0.5.3/foxai/logger.py` & `foxai-0.5.4/foxai/logger.py`

 * *Files identical despite different names*

### Comparing `foxai-0.5.3/pyproject.toml` & `foxai-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foxai"
-version = "0.5.3"
+version = "0.5.4"
 description = "Model Interpretability for PyTorch."
 authors = ["ReasonField Lab Team"]
 maintainers = [
 	"Adam Jan Kaczmarek <adam.kaczmarek@reasonfieldlab.com>",
 	"Adam Wawrzyński <adam.wawrzynski@reasonfieldlab.com>",
 	"Kamil Rzechowski <kamil.rzechowski@reasonfieldlab.com>",
 	"Rafał Pytel <rafal.pytel@reasonfieldlab.com>"
@@ -25,15 +25,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering",
 ]
 readme = "README.md"
 packages = [{include = "foxai"}]
 license = "Apache-2.0"
-documentation = "https://softwaremill.github.io/foxai/"
+documentation = "https://softwaremill.github.io/FoXAI/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/softwaremill/foxai/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<3.11"
 numpy = ">=1.21.4,<2.0.0"
@@ -50,14 +50,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 pylint = "2.15.4"
 mypy = "0.991"
 pytest = "7.2.0"
 pre-commit = "2.21.0"
 nbstripout = "0.6.1"
+notebook = "^6.5.3"
 
 [tool.poetry.group.example.dependencies]
 torchmetrics = ">=0.11.0,<1.0.0"
 torchvision = ">=0.13.1,<1.0.0"
 
 [tool.poetry.scripts]
 foxai-wandb-updater = "foxai.cli.experiment_update:main"
```

### Comparing `foxai-0.5.3/PKG-INFO` & `foxai-0.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxai
-Version: 0.5.3
+Version: 0.5.4
 Summary: Model Interpretability for PyTorch.
 Home-page: https://github.com/softwaremill/FoXAI
 License: Apache-2.0
 Keywords: Model Interpretability,XAI,explainable AI,Model Understanding,Feature Importance,PyTorch
 Author: ReasonField Lab Team
 Maintainer: Adam Jan Kaczmarek
 Maintainer-email: adam.kaczmarek@reasonfieldlab.com
@@ -26,15 +26,15 @@
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: pytorch-lightning (>=1.5.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: single-source (>=0.3.0,<1.0.0)
 Requires-Dist: torch (>=1.12.1,<2.0.0)
 Requires-Dist: wandb (>=0.13.7,<1.0.0)
 Project-URL: Bug Tracker, https://github.com/softwaremill/foxai/issues
-Project-URL: Documentation, https://softwaremill.github.io/foxai/
+Project-URL: Documentation, https://softwaremill.github.io/FoXAI/
 Project-URL: Repository, https://github.com/softwaremill/FoXAI
 Description-Content-Type: text/markdown
 
 # FoXAI
 
 FoXAI simplifies the application of e**X**plainable **AI** algorithms to explain the
 performance of neural network models during training. The library acts as an
@@ -58,23 +58,23 @@
     * [Note](#note)
         * [Artifacts directory structure](#artifacts-directory-structure)
         * [Examples](#examples)
 
 # Installation
 
 Installation requirements:
-* `Python` >= 3.7 & < 4.0
+* `Python` >=3.7.2,<3.11
 
 **Important**: For any problems regarding installation we advise to refer first to our [FAQ](FAQ.md).
 
 ## GPU acceleration
 
 To use the torch library with GPU acceleration, you need to install
 a dedicated version of torch with support for the installed version of CUDA
-drivers in the version supported by the library, at the moment `torch==1.12.1`.
+drivers in the version supported by the library, at the moment `torch>=1.12.1,<2.0.0`.
 A list of `torch` wheels with CUDA support can be found at
 [https://download.pytorch.org/whl/torch/](https://download.pytorch.org/whl/torch/).
 
 ## Manual installation
 
 If you would like to install from the source you can build a `wheel` package using `poetry`.
 The assumption is that the `poetry` package is installed. You can find how to install
@@ -104,27 +104,27 @@
 ```python
 import torch
 from pytorch_lightning import Trainer
 from pytorch_lightning.loggers import WandbLogger
 
 import wandb
 from foxai.callbacks.wandb_callback import WandBCallback
-from foxai.context_manager import Explainers, ExplainerWithParams
+from foxai.context_manager import CVClassificationExplainers, ExplainerWithParams
 
     ...
     wandb.login()
     wandb_logger = WandbLogger(project=project_name, log_model="all")
     callback = WandBCallback(
         wandb_logger=wandb_logger,
         explainers=[
             ExplainerWithParams(
-                explainer_name=Explainers.CV_INTEGRATED_GRADIENTS_EXPLAINER
+                explainer_name=CVClassificationExplainers.CV_INTEGRATED_GRADIENTS_EXPLAINER
             ),
             ExplainerWithParams(
-                explainer_name=Explainers.CV_GRADIENT_SHAP_EXPLAINER
+                explainer_name=CVClassificationExplainers.CV_GRADIENT_SHAP_EXPLAINER
             ),
         ],
         idx_to_label={index: index for index in range(0, 10)},
     )
     model = LitMNIST()
     trainer = Trainer(
         accelerator="gpu",
@@ -177,20 +177,20 @@
 ## CUDA
 
 The recommended version of CUDA is `10.2` as it is supported since version
 `1.5.0` of `torch`. You can check the compatibility of your CUDA version
 with the current version of `torch`:
 https://pytorch.org/get-started/previous-versions/.
 
-As our starting Docker image we were using the one provided by Nvidia: ``nvidia/cuda:10.2-devel-ubuntu18.04``. 
+As our starting Docker image we were using the one provided by Nvidia: ``nvidia/cuda:10.2-devel-ubuntu18.04``.
 
-If you wish an easy to use docker image we advise to use our ``Dockerfile``. 
+If you wish an easy to use docker image we advise to use our ``Dockerfile``.
 
 ## pyenv
-Optional step, but probably one of the easiest way to actually get Python version with all the needed aditional tools (e.g. pip). 
+Optional step, but probably one of the easiest way to actually get Python version with all the needed aditional tools (e.g. pip).
 
 `pyenv` is a tool used to manage multiple versions of Python. To install
 this package follow the instructions on the project repository page:
 https://github.com/pyenv/pyenv#installation. After installation You can
 install desired Python version, e.g. `3.8.16`:
 ```bash
 pyenv install 3.8.16
@@ -247,15 +247,15 @@
 Once all the steps have been completed, the environment is ready to go.
 A virtual environment by default will be created with the name `.venv` inside
 the project directory.
 
 ## Pre-commit hooks setup
 
 To improve the development experience, please make sure to install
-our [pre-commit][https://pre-commit.com/] hooks as the very first step after
+our [pre-commit](https://pre-commit.com/) hooks as the very first step after
 cloning the repository:
 
 ```bash
 poetry run pre-commit install
 ```
 
 ## Note
```

