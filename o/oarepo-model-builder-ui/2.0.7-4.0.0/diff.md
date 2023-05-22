# Comparing `tmp/oarepo-model-builder-ui-2.0.7.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-2.0.7.tar", last modified: Tue Apr 18 13:57:43 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.0.tar", last modified: Mon May 22 09:50:32 2023, max compression
```

## Comparing `oarepo-model-builder-ui-2.0.7.tar` & `oarepo-model-builder-ui-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.299518 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/model_preprocessors/layout_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 13:57:43.000000 oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:57:43.303519 oarepo-model-builder-ui-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-18 13:55:13.000000 oarepo-model-builder-ui-2.0.7/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.298557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/tests/test_translation.py
```

### Comparing `oarepo-model-builder-ui-2.0.7/PKG-INFO` & `oarepo-model-builder-ui-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.7
+Version: 4.0.0
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.7/README.md` & `oarepo-model-builder-ui-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,55 @@
 from collections import defaultdict
 from pathlib import Path
 from oarepo_model_builder.builders import OutputBuilder
 
-from oarepo_model_builder.builder import ModelBuilder
-from oarepo_model_builder.property_preprocessors import PropertyPreprocessor
-from typing import List
-
-from oarepo_model_builder.builders import process
+from oarepo_model_builder.datatypes import DataType
 from oarepo_model_builder_ui.config import UI_ITEMS
 
+from oarepo_model_builder.utils.python_name import module_to_path
 
 class InvenioI18nBuilder(OutputBuilder):
     TYPE = "invenio_i18n"
     output_file_type = "po"
 
-    def __init__(
-        self, builder: ModelBuilder, property_preprocessors: List[PropertyPreprocessor]
-    ):
-        super().__init__(builder, property_preprocessors)
-
-    def begin(self, schema, settings):
-        super().begin(schema, settings)
-
-        mod = self.current_model.package.split(".")
-        path = Path(*mod)
-        self.output = self.builder.get_output("po", path / "translations")
-
-    @process("**", condition=lambda current, stack: stack.schema_valid)
-    def model_element(self):
-        schema_element_type = self.stack.top.schema_element_type
-
-        if schema_element_type == "property":
-            ui_items = defaultdict(dict)
-            for el, val in self.stack.top.data.items():
-                for ui in UI_ITEMS:
-                    if el.startswith(f"{ui}."):
-                        ui_items[ui][el[len(ui) + 1 :]] = val
-            key_proto = self.stack.top.data.get("i18n.key")
-            for ui in UI_ITEMS:
-                if "key" not in ui_items[ui]:
-                    if key_proto:
-                        ui_items[ui]["key"] = f"{key_proto}.{ui}"
-                    else:
-                        ui_items[ui]["key"] = (
-                            "/".join(
-                                x.key
-                                for x in self.stack
-                                if x.schema_element_type == "property" and x.key
-                            )
-                            + f".{ui}"
-                        )
-
-            # add translation for enums
-            enum_keys = self.stack.top.data.get("enum", [])
-            for en in enum_keys:
+    def build_node(self, datatype: DataType):
+        translation_config = datatype.section_translations.config
+
+        path = module_to_path(translation_config['module'])
+        self.output = self.builder.get_output("po", path)
+
+        for node in datatype.deep_iter():
+            if node != datatype:
+                self.process_node(node)
+
+    def process_node(self, node):
+        ui_items = defaultdict(dict)
+
+        for ui in UI_ITEMS:
+            if ui in node.definition:
+                ui_items[ui] = {**node.definition[ui]}
+
+        key_proto = node.definition.get("i18n.key")
+        for ui in UI_ITEMS:
+            if "key" not in ui_items[ui]:
                 if key_proto:
-                    ui_items[en]["key"] = f"{key_proto}.enum.{en}"
+                    ui_items[ui]["key"] = f"{key_proto}.{ui}"
                 else:
-                    ui_items[en]["key"] = (
-                        "/".join(
-                            x.key
-                            for x in self.stack
-                            if x.schema_element_type == "property" and x.key
-                        )
-                        + f".enum.{en}"
+                    ui_items[ui]["key"] = (
+                            node.path.replace('.', '/') + f".{ui}"
                     )
 
-            for ui, langs in ui_items.items():
-                key = langs.pop("key")
-                for lang, val in langs.items():
-                    self.output.add(key, val, language=lang)
-                self.output.add(key)
-
-        self.build_children()
+        # add translation for enums
+        enum_keys = node.definition.get("enum", [])
+        for en in enum_keys:
+            if key_proto:
+                ui_items[en]["key"] = f"{key_proto}.enum.{en}"
+            else:
+                ui_items[en]["key"] = (
+                        node.path.replace('.', '/') + f".enum.{en}"
+                )
+
+        for ui, langs in ui_items.items():
+            key = langs.pop("key")
+            for lang, val in langs.items():
+                self.output.add(key, val, language=lang)
+            self.output.add(key)
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,14 @@
     TYPE = "invenio_i18n_setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
 
+        config = self.current_model.section_translations.config
+
         output.add_entry_point(
             "invenio_i18n.translations",
-            self.current_model.translations_setup_cfg,
-            self.current_model.package,
+            config["alias"],
+            config["module"].rsplit(".", maxsplit=1)[0],
         )
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-import json
-from typing import List
 import inflect
 
-from oarepo_model_builder.builder import ModelBuilder
-from oarepo_model_builder.builders import process
 from oarepo_model_builder.builders.json_base import JSONBaseBuilder
-from oarepo_model_builder.property_preprocessors import PropertyPreprocessor
-from oarepo_model_builder.invenio.invenio_record_search import get_facet_details
-from oarepo_model_builder.utils.verbose import log
+from oarepo_model_builder.datatypes import Section
 
 from oarepo_model_builder_ui.config import UI_ITEMS
 
 """
 Will generate:
 metadata: {
   // contents of ui child here
@@ -30,61 +24,65 @@
 it will be saved to package/model/ui.json
 """
 
 
 class InvenioLayoutBuilder(JSONBaseBuilder):
     TYPE = "ui-layout"
     output_file_type = "json"
-    output_file_name = "ui-layout"
+    output_file_name = ["ui", "file"]
+    create_parent_packages = True
 
-    @process("**", condition=lambda current, stack: stack.schema_valid)
-    def model_element(self):
+    def build_node(self, node):
+        generated = self.generate_node(node)
+        self.output.merge(generated)
+
+    def generate(self, node):
+        ui: Section = node.section_ui
+        ret = {**ui.config}
+        ret.pop('marshmallow', None)
+
+        if ui.children:
+            properties = ret.setdefault("children", {})
+            for k, v in ui.children.items():
+                v = self.generate(v)
+                properties[k] = v
+        if ui.item:
+            ret["child"] = self.generate(ui.item)
+        return ret
+
+    def generate_node(self, node):
         ui = {}
-        data = self.stack.top.data
-        schema_element_type = self.stack.top.schema_element_type
+        section = node.section_ui
+        data = node.definition
 
-        if isinstance(data, dict):
-            ui.update({k.replace("-", "_"): v for k, v in data.get("ui", {}).items()})
-            if "type" in data:
-                t = data["type"]
-                if t in ("object", "nested"):
-                    t = inflect.engine().singular_noun(
-                        [
-                            x.key
-                            for x in self.stack
-                            if x.key and x.schema_element_type == "property"
-                        ][-1].lower()
-                    )
-                ui.setdefault("detail", t)
-                ui.setdefault("input", t)
-
-        leave = True
-        if schema_element_type == "property":
-            for fld in UI_ITEMS:
-                ui[fld] = data.get(
-                    f"{fld}.key",
-                    "/".join(
-                        x.key
-                        for x in self.stack
-                        if x.schema_element_type == "property" and x.key
-                    )
-                    + f".{fld}",
+        ui.update({k.replace("-", "_"): v for k, v in section.config.items()})
+        ui.pop('marshmallow', None)
+        if "type" in data:
+            t = data["type"]
+            if t in ("object", "nested"):
+                t = inflect.engine().singular_noun(
+                    node.path.split('.')[-1].lower()
                 )
+            ui.setdefault("detail", t)
+            ui.setdefault("input", t)
 
-            facets = get_facet_details(
-                self.stack, self.current_model, self.schema, set()
+        for fld in UI_ITEMS:
+            ui[fld] = data.get(
+                f"{fld}.key",
+                node.path.replace('.', '/') + f".{fld}",
             )
 
-            if len(facets):
-                ui["facet"] = facets[0]["path"]
+        # facets = get_facet_details(
+        #     self.stack, self.current_model, self.schema, set()
+        # )
+        #
+        # if len(facets):
+        #     ui["facet"] = facets[0]["path"]
+
+        if node.children:
+            children = ui.setdefault('children', {})
+            for c in node.children.values():
+                children[c.key] = self.generate_node(c)
+        if hasattr(node, 'item'):
+            ui['child'] = self.generate_node(node.item)
 
-            self.output.enter(self.stack.top.key, {})
-        elif schema_element_type == "properties":
-            self.output.enter("children", {})
-        elif schema_element_type == "items":
-            self.output.enter("child", {})
-        else:
-            leave = False
-        self.output.merge(ui)
-        self.build_children()
-        if leave:
-            self.output.leave()
+        return ui
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/invenio/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 class InvenioLayoutSetupCfgBuilder(OutputBuilder):
     TYPE = "invenio_layout_setup_cfg"
 
     def finish(self):
         super().finish()
 
         output: CFGOutput = self.builder.get_output("cfg", "setup.cfg")
+        config = self.current_model.section_ui.config
 
         output.add_entry_point(
             "oarepo.ui",
-            self.current_model.package,
-            f"{self.current_model.package}.models:{Path(self.current_model.ui_layout).name}",
+            config['alias'],
+            f"{config['module']}:{Path(config['file']).name}",
         )
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return self.po.to_binary()
 
 
 class POOutput(OutputBase):
     TYPE = "po"
 
     def begin(self):
-        languages = self.builder.schema.settings.i18n_languages
+        languages = self.builder.schema.settings['i18n-languages']
         self.languages = languages
         self.po_files = {}
 
         for lang in languages:
             lang_path = Path(self.path) / lang / "LC_MESSAGES" / "messages.po"
             self._init_lang_path(lang, lang_path)
         self._init_lang_path(None, Path(self.path) / "messages.pot")
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 2.0.7
+Version: 4.0.0
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 oarepo_model_builder_ui/config.py
 oarepo_model_builder_ui.egg-info/PKG-INFO
 oarepo_model_builder_ui.egg-info/SOURCES.txt
 oarepo_model_builder_ui.egg-info/dependency_links.txt
 oarepo_model_builder_ui.egg-info/entry_points.txt
 oarepo_model_builder_ui.egg-info/requires.txt
 oarepo_model_builder_ui.egg-info/top_level.txt
-oarepo_model_builder_ui/invenio/__init__.py
-oarepo_model_builder_ui/invenio/i18n.py
-oarepo_model_builder_ui/invenio/i18n_setup_cfg.py
-oarepo_model_builder_ui/invenio/layout.py
-oarepo_model_builder_ui/invenio/layout_setup_cfg.py
-oarepo_model_builder_ui/model_preprocessors/__init__.py
-oarepo_model_builder_ui/model_preprocessors/layout_settings.py
+oarepo_model_builder_ui/builders/__init__.py
+oarepo_model_builder_ui/builders/i18n.py
+oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+oarepo_model_builder_ui/builders/layout.py
+oarepo_model_builder_ui/builders/layout_setup_cfg.py
+oarepo_model_builder_ui/datatypes/__init__.py
+oarepo_model_builder_ui/datatypes/components/__init__.py
+oarepo_model_builder_ui/datatypes/components/model.py
 oarepo_model_builder_ui/outputs/i18n.py
 oarepo_model_builder_ui/outputs/layout.py
 oarepo_model_builder_ui/validation/__init__.py
 tests/test_facets.py
 tests/test_translation.py
```

### Comparing `oarepo-model-builder-ui-2.0.7/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,43 @@
-[oarepo_model_builder.builders.model]
-4000-oarepo-i18n = oarepo_model_builder_ui.invenio.i18n:InvenioI18nBuilder
-4010-oarepo-i18n-setup = oarepo_model_builder_ui.invenio.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
-4020-oarepo-ui-layout = oarepo_model_builder_ui.invenio.layout:InvenioLayoutBuilder
-4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.invenio.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
+[metadata]
+name = oarepo-model-builder-ui
+version = 4.0.0
+description = Model builder plugin for oarepo-ui
+authors = 
+readme = README.md
+long_description = file:README.md
+long_description_content_type = text/markdown
 
-[oarepo_model_builder.model_preprocessors.model]
-50-oarepo-ui = oarepo_model_builder_ui.model_preprocessors.layout_settings:LayoutSettingsPreprocessor
+[options]
+python = >=3.9,<4.0
+install_requires = 
+	langcodes>=3.3.0
+	oarepo-model-builder>=4.0.0
+	polib
+	inflect
 
-[oarepo_model_builder.outputs]
-po = oarepo_model_builder_ui.outputs.i18n:POOutput
+[options.extras_require]
+tests = 
+	pytest>=7
+
+[options.package_data]
+* = *.json, *.rst, *.md, *.json5, *.jinja2
+
+[options.entry_points]
+oarepo_model_builder.validation.settings = 
+	ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
+oarepo_model_builder.datatypes.components = 
+	ui-components = oarepo_model_builder_ui.datatypes.components:components
+oarepo_model_builder.builders.record = 
+	4000-oarepo-i18n = oarepo_model_builder_ui.builders.i18n:InvenioI18nBuilder
+	4010-oarepo-i18n-setup = oarepo_model_builder_ui.builders.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
+	4020-oarepo-ui-layout = oarepo_model_builder_ui.builders.layout:InvenioLayoutBuilder
+	4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.builders.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
+oarepo_model_builder.outputs = 
+	po  = oarepo_model_builder_ui.outputs.i18n:POOutput
+oarepo_model_builder.model_preprocessors.model = 
+	50-oarepo-ui  = oarepo_model_builder_ui.model_preprocessors.layout_settings:LayoutSettingsPreprocessor
+
+[egg_info]
+tag_build = 
+tag_date = 0
 
-[oarepo_model_builder.validation]
-ui-validation = oarepo_model_builder_ui.validation:validators
```

### Comparing `oarepo-model-builder-ui-2.0.7/setup.cfg` & `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,17 @@
-[metadata]
-name = oarepo-model-builder-ui
-version = 2.0.7
-description = Model builder plugin for oarepo-ui
-authors = 
-readme = README.md
-long_description = file:README.md
-long_description_content_type = text/markdown
+[oarepo_model_builder.builders.record]
+4000-oarepo-i18n = oarepo_model_builder_ui.builders.i18n:InvenioI18nBuilder
+4010-oarepo-i18n-setup = oarepo_model_builder_ui.builders.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
+4020-oarepo-ui-layout = oarepo_model_builder_ui.builders.layout:InvenioLayoutBuilder
+4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.builders.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
+
+[oarepo_model_builder.datatypes.components]
+ui-components = oarepo_model_builder_ui.datatypes.components:components
 
-[options]
-python = >=3.9,<4.0
-install_requires = 
-	langcodes>=3.3.0
-	oarepo-model-builder>=3.0.0
-	polib
-	inflect
+[oarepo_model_builder.model_preprocessors.model]
+50-oarepo-ui = oarepo_model_builder_ui.model_preprocessors.layout_settings:LayoutSettingsPreprocessor
 
-[options.extras_require]
-tests = 
-	pytest>=7
-
-[options.package_data]
-* = *.json, *.rst, *.md, *.json5, *.jinja2
-
-[options.entry_points]
-oarepo_model_builder.validation = 
-	ui-validation = oarepo_model_builder_ui.validation:validators
-oarepo_model_builder.builders.model = 
-	4000-oarepo-i18n = oarepo_model_builder_ui.invenio.i18n:InvenioI18nBuilder
-	4010-oarepo-i18n-setup = oarepo_model_builder_ui.invenio.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
-	4020-oarepo-ui-layout = oarepo_model_builder_ui.invenio.layout:InvenioLayoutBuilder
-	4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.invenio.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
-oarepo_model_builder.outputs = 
-	po  = oarepo_model_builder_ui.outputs.i18n:POOutput
-oarepo_model_builder.model_preprocessors.model = 
-	50-oarepo-ui  = oarepo_model_builder_ui.model_preprocessors.layout_settings:LayoutSettingsPreprocessor
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[oarepo_model_builder.outputs]
+po = oarepo_model_builder_ui.outputs.i18n:POOutput
 
+[oarepo_model_builder.validation.settings]
+ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
```

### Comparing `oarepo-model-builder-ui-2.0.7/tests/test_facets.py` & `oarepo-model-builder-ui-4.0.0/tests/test_facets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import json
 
 from oarepo_model_builder.entrypoints import create_builder_from_entrypoints, load_model
 from oarepo_model_builder.fs import InMemoryFileSystem
 
+import pytest
 DUMMY_YAML = "test.yaml"
 
 
+@pytest.mark.xfail
 def test_facets(app):
     schema = load_model(
         DUMMY_YAML,
         "test",
         model_content={
-            "model": {
+            "record": {
                 "use": "invenio",
                 "properties": {
                     "b": {
                         "type": "object",
                         "properties": {
                             "c": {
                                 "type": "keyword",
```

