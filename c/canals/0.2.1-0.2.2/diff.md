# Comparing `tmp/canals-0.2.1.tar.gz` & `tmp/canals-0.2.2.tar.gz`

## Comparing `canals-0.2.1.tar` & `canals-0.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.1/canals/__about__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.1/canals/__init__.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.1/canals/errors.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/__init__.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/component.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/decorators.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.1/canals/component/input_output.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/__init__.py
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/draw.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.1/canals/draw/mermaid.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/_utils.py
--rw-r--r--   0        0        0    28710 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.1/canals/pipeline/save_load.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.1/canals/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.2.1/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.1/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.1/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/components.md
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.1/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.1/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.1/images/canals-logo-light.png
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/__init__.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.1/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.1/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/__init__.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_accumulate.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_add_value.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_double.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_greet.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_merge_loop.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_parity.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_remainder.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_repeat.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_subtract.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_sum.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 canals-0.2.1/test/sample_components/test_threshold.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.1/LICENSE
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 canals-0.2.1/README.md
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 canals-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.2.2/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 canals-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.2.2/canals/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.2.2/canals/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 canals-0.2.2/canals/errors.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/__init__.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/component.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/decorators.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 canals-0.2.2/canals/component/input_output.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/draw.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 canals-0.2.2/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 canals-0.2.2/canals/pipeline/sockets.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.2.2/canals/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.2.2/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.2.2/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.2.2/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/components.md
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 canals-0.2.2/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.2.2/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.2.2/images/canals-logo-light.png
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/__init__.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 canals-0.2.2/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.2.2/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/__init__.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_accumulate.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_add_value.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_double.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_greet.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_parity.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_remainder.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_repeat.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_subtract.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_sum.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 canals-0.2.2/test/sample_components/test_threshold.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 canals-0.2.2/README.md
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 canals-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 canals-0.2.2/PKG-INFO
```

### Comparing `canals-0.2.1/.pre-commit-config.yaml` & `canals-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/mkdocs.yml` & `canals-0.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/.github/workflows/tests.yml` & `canals-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/component/component.py` & `canals-0.2.2/canals/component/component.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/component/decorators.py` & `canals-0.2.2/canals/component/decorators.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/component/input_output.py` & `canals-0.2.2/canals/component/input_output.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/draw/draw.py` & `canals-0.2.2/canals/draw/draw.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Literal, Optional, Dict, get_args, Any
 
 import logging
 from pathlib import Path
 
 import networkx
 
-from canals.pipeline._utils import find_pipeline_inputs, find_pipeline_outputs
+from canals.pipeline.sockets import find_pipeline_inputs, find_pipeline_outputs
 from canals.draw.graphviz import to_agraph
 from canals.draw.mermaid import to_mermaid_image, to_mermaid_text
 
 
 logger = logging.getLogger(__name__)
 RenderingEngines = Literal["graphviz", "mermaid-img", "mermaid-text"]
 
@@ -41,14 +41,24 @@
 
     else:
         raise ValueError(f"Unknown rendering engine '{engine}'. Choose one from: {get_args(RenderingEngines)}.")
 
     logger.debug("Pipeline diagram saved at %s", path)
 
 
+def convert_for_debug(
+    graph: networkx.MultiDiGraph,
+) -> Any:
+    """
+    Renders the pipeline graph with additional debug information into a text file that Mermaid can later render.
+    """
+    graph = _prepare_for_drawing(graph=graph, style_map={})
+    return to_mermaid_text(graph=graph)
+
+
 def convert(
     graph: networkx.MultiDiGraph,
     engine: RenderingEngines = "mermaid-img",
     style_map: Optional[Dict[str, str]] = None,
 ) -> Any:
     """
     Renders the pipeline graph with the correct render and returns it.
```

### Comparing `canals-0.2.1/canals/draw/graphviz.py` & `canals-0.2.2/canals/draw/graphviz.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/draw/mermaid.py` & `canals-0.2.2/canals/draw/mermaid.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/pipeline/_utils.py` & `canals-0.2.2/canals/pipeline/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai> SPDX-License-Identifier: Apache-2.0
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 from typing import Tuple, Optional, List, Iterable, Dict, Any, get_args
 
 import logging
 import inspect
 import itertools
 from dataclasses import dataclass
```

### Comparing `canals-0.2.1/canals/pipeline/pipeline.py` & `canals-0.2.2/canals/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
-from typing import Optional, Any, Dict, List, Tuple, Literal
+from typing import Optional, Any, Dict, List, Tuple, Literal, Union
 
+import os
+import json
 import datetime
 import logging
 from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
 
 import networkx
 
 from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
 from canals.component.input_output import ComponentInput
-from canals.draw import draw, RenderingEngines
-from canals.pipeline._utils import (
+from canals.draw import draw, convert_for_debug, RenderingEngines
+from canals.pipeline.sockets import (
     InputSocket,
     OutputSocket,
     find_input_sockets,
     find_output_sockets,
     find_unambiguous_connection,
     parse_connection_name,
     validate_pipeline_input,
@@ -35,28 +37,31 @@
     Builds a graph of components and orchestrates their execution according to the execution graph.
     """
 
     def __init__(
         self,
         metadata: Optional[Dict[str, Any]] = None,
         max_loops_allowed: int = 100,
+        debug_path: Union[Path, str] = Path(".canals_debug/"),
     ):
         """
         Creates the Pipeline.
 
         Args:
             metadata: arbitrary dictionary to store metadata about this pipeline. Make sure all the values contained in
                 this dictionary can be serialized and deserialized if you wish to save this pipeline to file with
                 `save_pipelines()/load_pipelines()`.
             max_loops_allowed: how many times the pipeline can run the same node before throwing an exception.
+            debug_path: when debug is enabled in `run()`, where to save the debug data.
         """
         self.metadata = metadata or {}
         self.max_loops_allowed = max_loops_allowed
         self.graph = networkx.MultiDiGraph()
         self.debug: Dict[int, Dict[str, Any]] = {}
+        self.debug_path = Path(debug_path)
 
     def __eq__(self, other) -> bool:
         """
         Equal pipelines share every metadata, node and edge, but they're not required to use
         the same node instances: this allows pipeline saved and then loaded back to be equal to themselves.
         """
         if (
@@ -333,27 +338,23 @@
                 for node, input_data in data.items()
             }
         )
         pipeline_output: Dict[str, Dict[str, Any]] = {}
 
         if debug:
             logger.info("Debug mode ON.")
-            self.debug = {}
+        self.debug = {}
 
         # *** PIPELINE EXECUTION LOOP ***
         # We select the nodes to run by popping them in FIFO order from the inputs buffer.
         step = 0
         while inputs_buffer:
             step += 1
             if debug:
-                self.debug[step] = {
-                    "time": datetime.datetime.now(),
-                    "inputs_buffer": list(inputs_buffer.items()),
-                    "pipeline_output": pipeline_output,
-                }
+                self._record_pipeline_step(step, inputs_buffer, pipeline_output)
             logger.debug("> Queue at step %s: %s", step, {k: list(v.keys()) for k, v in inputs_buffer.items()})
 
             component, inputs = inputs_buffer.popitem(last=False)  # FIFO
 
             # if debug:
             #     draw(deepcopy(self.graph), engine="graphviz", path=f"debug/step_{current_step}.jpg", running=component, queued=inputs_buffer.keys())
 
@@ -383,24 +384,39 @@
                 pipeline_output[component] = output
             else:
                 inputs_buffer = self._route_output(
                     node_results=output, node_name=component, inputs_buffer=inputs_buffer
                 )
 
         if debug:
-            self.debug[step + 1] = {
-                "time": datetime.datetime.now(),
-                "inputs_buffer": list(inputs_buffer.items()),
-                "pipeline_output": pipeline_output,
-            }
+            self._record_pipeline_step(step + 1, inputs_buffer, pipeline_output)
+
+            # Save to json
+            os.makedirs(self.debug_path, exist_ok=True)
+            with open(self.debug_path / "data.json", "w", encoding="utf-8") as datafile:
+                json.dump(self.debug, datafile, indent=4, default=str)
+
+            # Store in the output
             pipeline_output["_debug"] = self.debug  # type: ignore
 
         logger.info("Pipeline executed successfully.")
         return pipeline_output
 
+    def _record_pipeline_step(self, step, inputs_buffer, pipeline_output):
+        """
+        Stores a snapshot of this step into the self.debug dictionary of the pipeline.
+        """
+        mermaid_graph = convert_for_debug(deepcopy(self.graph))
+        self.debug[step] = {
+            "time": datetime.datetime.now(),
+            "inputs_buffer": list(inputs_buffer.items()),
+            "pipeline_output": pipeline_output,
+            "diagram": mermaid_graph,
+        }
+
     def _clear_visits_count(self):
         """
         Make sure all nodes's visits count is zero.
         """
         for node in self.graph.nodes:
             self.graph.nodes[node]["visits"] = 0
```

### Comparing `canals-0.2.1/canals/pipeline/save_load.py` & `canals-0.2.2/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/canals/testing/test_component.py` & `canals-0.2.2/canals/testing/test_component.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/docs/index.md` & `canals-0.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/docs/concepts/components.md` & `canals-0.2.2/docs/concepts/components.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/docs/concepts/concepts.md` & `canals-0.2.2/docs/concepts/concepts.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/docs/concepts/pipelines.md` & `canals-0.2.2/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/images/canals-logo-dark.png` & `canals-0.2.2/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/images/canals-logo-light.png` & `canals-0.2.2/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/test_save_load.py` & `canals-0.2.2/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/pipelines/integration/test_variable_merging_pipeline.py` & `canals-0.2.2/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/__init__.py` & `canals-0.2.2/test/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_accumulate.py` & `canals-0.2.2/test/sample_components/test_accumulate.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_add_value.py` & `canals-0.2.2/test/sample_components/test_add_value.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_double.py` & `canals-0.2.2/test/sample_components/test_double.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_greet.py` & `canals-0.2.2/test/sample_components/test_greet.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_merge_loop.py` & `canals-0.2.2/test/sample_components/test_merge_loop.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_parity.py` & `canals-0.2.2/test/sample_components/test_parity.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_remainder.py` & `canals-0.2.2/test/sample_components/test_remainder.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_repeat.py` & `canals-0.2.2/test/sample_components/test_repeat.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_subtract.py` & `canals-0.2.2/test/sample_components/test_subtract.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_sum.py` & `canals-0.2.2/test/sample_components/test_sum.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/test/sample_components/test_threshold.py` & `canals-0.2.2/test/sample_components/test_threshold.py`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/.gitignore` & `canals-0.2.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -125,7 +125,11 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Canals
+drafts/
+.canals_debug/
```

### Comparing `canals-0.2.1/LICENSE` & `canals-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/README.md` & `canals-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/pyproject.toml` & `canals-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.2.1/PKG-INFO` & `canals-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.2.1
+Version: 0.2.2
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canals Version: 0.2.1 Summary: A component
+Metadata-Version: 2.1 Name: canals Version: 0.2.2 Summary: A component
 orchestration engine for Haystack Project-URL: Documentation, https://
 github.com/deepset-ai/canals#readme Project-URL: Issues, https://github.com/
 deepset-ai/canals/issues Project-URL: Source, https://github.com/deepset-ai/
 canals Author-email: ZanSara
 zanzottera@deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: License :: Freely
 Distributable Classifier: License :: OSI Approved :: Apache Software License
```

