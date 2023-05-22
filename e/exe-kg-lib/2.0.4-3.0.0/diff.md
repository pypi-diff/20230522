# Comparing `tmp/exe_kg_lib-2.0.4.tar.gz` & `tmp/exe_kg_lib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exe_kg_lib-2.0.4.tar", max compression
+gzip compressed data, was "exe_kg_lib-3.0.0.tar", max compression
```

## Comparing `exe_kg_lib-2.0.4.tar` & `exe_kg_lib-3.0.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0    34283 2023-05-08 15:34:05.255395 exe_kg_lib-2.0.4/LICENSE.md
--rw-r--r--   0        0        0    15902 2023-05-08 15:34:05.255395 exe_kg_lib-2.0.4/README.md
--rw-r--r--   0        0        0       27 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/__init__.py
--rw-r--r--   0        0        0      102 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/__init__.py
--rw-r--r--   0        0        0     1253 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/data_entity.py
--rw-r--r--   0        0        0      788 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/entity.py
--rw-r--r--   0        0        0    31697 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/exe_kg.py
--rw-r--r--   0        0        0      773 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/kg_schema.py
--rw-r--r--   0        0        0     3528 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/task.py
--rw-r--r--   0        0        0     1914 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/__init__.py
--rw-r--r--   0        0        0     5619 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/ml_tasks.py
--rw-r--r--   0        0        0     1967 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/statistic_tasks.py
--rw-r--r--   0        0        0     3108 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/visual_tasks.py
--rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/cli/__init__.py
--rw-r--r--   0        0        0      938 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/cli/main.py
--rw-r--r--   0        0        0      108 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/__init__.py
--rw-r--r--   0        0        0     3130 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/cli_utils.py
--rw-r--r--   0        0        0     7290 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/kg_creation_utils.py
--rw-r--r--   0        0        0     6250 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/query_utils.py
--rw-r--r--   0        0        0      679 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/string_utils.py
--rw-r--r--   0        0        0        0 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/__init__.py
--rw-r--r--   0        0        0     2660 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/ml_utils.py
--rw-r--r--   0        0        0     2606 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/statistic_utils.py
--rw-r--r--   0        0        0     2388 2023-05-08 15:34:05.259395 exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/visual_utils.py
--rw-r--r--   0        0        0     3645 2023-05-08 15:34:28.212725 exe_kg_lib-2.0.4/pyproject.toml
--rw-r--r--   0        0        0    17350 1970-01-01 00:00:00.000000 exe_kg_lib-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34283 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/LICENSE.md
+-rw-r--r--   0        0        0    15902 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/README.md
+-rw-r--r--   0        0        0       27 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/__init__.py
+-rw-r--r--   0        0        0     1253 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/data_entity.py
+-rw-r--r--   0        0        0      788 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/entity.py
+-rw-r--r--   0        0        0    32574 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/exe_kg.py
+-rw-r--r--   0        0        0      773 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/kg_schema.py
+-rw-r--r--   0        0        0     3528 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/task.py
+-rw-r--r--   0        0        0     1914 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/__init__.py
+-rw-r--r--   0        0        0     5619 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/ml_tasks.py
+-rw-r--r--   0        0        0     1967 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/statistic_tasks.py
+-rw-r--r--   0        0        0     3108 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/visual_tasks.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/cli/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/shacl/__init__.py
+-rw-r--r--   0        0        0     1967 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/shacl/base_shape_graph_generator.py
+-rw-r--r--   0        0        0    26612 2023-05-22 08:26:12.898873 exe_kg_lib-3.0.0/exe_kg_lib/shacl/shacl_shape_graph.ttl
+-rw-r--r--   0        0        0      108 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/__init__.py
+-rw-r--r--   0        0        0     3130 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/cli_utils.py
+-rw-r--r--   0        0        0     7290 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/kg_creation_utils.py
+-rw-r--r--   0        0        0      809 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/kg_validation_utils.py
+-rw-r--r--   0        0        0     6378 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/query_utils.py
+-rw-r--r--   0        0        0      679 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/string_utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/__init__.py
+-rw-r--r--   0        0        0     2660 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/ml_utils.py
+-rw-r--r--   0        0        0     2606 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/statistic_utils.py
+-rw-r--r--   0        0        0     2388 2023-05-22 08:26:12.902873 exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/visual_utils.py
+-rw-r--r--   0        0        0     3683 2023-05-22 08:26:33.683014 exe_kg_lib-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    17344 1970-01-01 00:00:00.000000 exe_kg_lib-3.0.0/PKG-INFO
```

### Comparing `exe_kg_lib-2.0.4/LICENSE.md` & `exe_kg_lib-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/README.md` & `exe_kg_lib-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/data_entity.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/data_entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/entity.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/entity.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/exe_kg.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/exe_kg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright (c) 2022 Robert Bosch GmbH
 # SPDX-License-Identifier: AGPL-3.0
 
+import itertools
 import os
 from typing import Dict, Union
 
 import pandas as pd
 from rdflib import Literal
 
+from exe_kg_lib.utils.kg_validation_utils import check_kg_executability
+
 from ..utils.cli_utils import (get_input_for_existing_data_entities,
                                get_input_for_new_data_entities)
 from ..utils.kg_creation_utils import (add_and_attach_data_entity,
                                        add_data_entity_instance,
                                        add_instance_from_parent_with_relation,
                                        add_literal, create_pipeline_task,
                                        name_instance)
@@ -69,14 +72,15 @@
         self.data_semantics = Entity(self.top_level_schema.namespace.DataSemantics)
         self.data_structure = Entity(self.top_level_schema.namespace.DataStructure)
 
         # self.input_kg: KG eventually filled with 3 KG schemas and the input executable KG in case of KG execution
         self.input_kg = Graph(bind_namespaces="rdflib")
         if input_exe_kg_path:  # KG execution mode
             self.input_kg.parse(input_exe_kg_path, format="n3")  # parse input executable KG
+            check_kg_executability(self.input_kg)
             all_ns = [n for n in self.input_kg.namespace_manager.namespaces()]
             bottom_level_schema_info_set = False  # flag indicating that a bottom-level schema was found
             for schema_name, schema_info in KG_SCHEMAS.items():  # search for used bottom-level schema
                 if (
                     schema_name == "Data Science"  # or schema_name == "Visualization"
                 ):  # skip top-level KG schema and Visualization schema that is always used
                     continue
@@ -287,15 +291,15 @@
             filter(lambda pair: pair[1].split("#")[1] == method, results), None
         )  # match given method_type with query result
         if chosen_property_method is None:
             print(f"Property connecting task of type {task} with method of type {method} not found")
             exit(1)
 
         # instantiate method and link it with the task using the appropriate chosen_property_method[0] relation
-        add_instance_from_parent_with_relation(
+        method_entity = add_instance_from_parent_with_relation(
             kg_schema_to_use.namespace,
             self.output_kg,
             method_parent,
             chosen_property_method[0],
             next_task,
             name_instance(self.task_type_dict, self.method_type_dict, method_parent),
         )
@@ -308,15 +312,15 @@
             property_iri = pair[0]
             property_name = property_iri.split("#")[1]
             range_iri = pair[1]
             input_property = Literal(
                 lexical_or_value=properties_dict[property_name],
                 datatype=range_iri,
             )
-            add_literal(self.output_kg, next_task, property_iri, input_property)
+            add_literal(self.output_kg, method_entity, property_iri, input_property)
 
         self.last_created_task = next_task  # store created task
 
         return next_task
 
     def _add_inputs_to_task(
         self,
@@ -328,29 +332,32 @@
         Instantiates and adds given input data entities to the given task of self.output_kg
         if input_data_entity_dict is None, user is asked to specify input data entities
         Args:
             task_entity: the task to add the input to
             input_data_entity_dict: keys -> input entity names corresponding to the given task as defined in the chosen bottom-level KG schema
                                     values -> list of corresponding data entities to be added as input to the task
         """
+
+        use_cli = input_data_entity_dict is None
+
         # fetch compatible inputs from KG schema
         results = list(
             get_input_properties_and_inputs(
                 self.input_kg,
                 self.top_level_schema.namespace_prefix,
                 task_entity.parent_entity.iri,
             )
         )
 
         # task_type_index was incremented when creating the task entity
         # reset the index to match the currently created task's index
         task_type_index = self.task_type_dict[task_entity.type] - 1
-        for _, input_entity_iri in results:
+        for _, input_entity_iri, data_structure_iri in results:
             input_entity_name = input_entity_iri.split("#")[1]
-            if input_data_entity_dict:
+            if not use_cli:
                 input_data_entity_list = input_data_entity_dict[input_entity_name]
             else:
                 # use CLI
                 print(f"Specify input corresponding to {input_entity_name}")
                 input_data_entity_list = get_input_for_existing_data_entities(self.existing_data_entity_list)
                 input_data_entity_list += get_input_for_new_data_entities(
                     self.data_semantics_list,
@@ -372,27 +379,31 @@
                     input_data_entity,
                 )
                 # instantiate and attach data entity with reference to the given data entity
                 data_entity = DataEntity(
                     data_entity_iri,
                     DataEntity(input_entity_iri, self.data_entity),
                     has_reference=input_data_entity.iri,
+                    has_data_structure_iri=data_structure_iri,
                 )
                 add_and_attach_data_entity(
                     self.output_kg,
                     self.data,
                     self.top_level_schema.kg,
                     self.top_level_schema.namespace,
                     data_entity,
                     self.top_level_schema.namespace.hasInput,
                     task_entity,
                 )
                 task_entity.input_dict[input_entity_name] = data_entity
                 same_input_index += 1
 
+                if use_cli:
+                    check_kg_executability(self.output_kg)
+
     def _add_outputs_to_task(self, task_entity: Task) -> None:
         """
         Instantiates and adds output data entities to the given task of self.output_kg, based on the task's definition in the KG schema
         Args:
             task_entity: the task to add the output to
         """
         # fetch compatible outputs from KG schema
@@ -403,29 +414,33 @@
                 task_entity.parent_entity.iri,
             )
         )
 
         # task_type_index was incremented when creating the task entity
         # reset the index to match the currently created task's index
         task_type_index = self.task_type_dict[task_entity.type] - 1
-        for output_property, output_entity_iri in results:
+        for output_property, output_parent_entity_iri, data_structure_iri in results:
             # instantiate and add data entity
-            data_entity_iri = output_entity_iri + str(task_type_index)
-            data_entity = DataEntity(data_entity_iri, self.data_entity)
+            output_data_entity_iri = output_parent_entity_iri + str(task_type_index)
+            output_data_entity = DataEntity(
+                output_data_entity_iri,
+                DataEntity(output_parent_entity_iri, self.data_entity),
+                has_data_structure_iri=data_structure_iri,
+            )
             add_and_attach_data_entity(
                 self.output_kg,
                 self.data,
                 self.top_level_schema.kg,
                 self.top_level_schema.namespace,
-                data_entity,
+                output_data_entity,
                 self.top_level_schema.namespace.hasOutput,
                 task_entity,
             )
-            task_entity.output_dict[output_entity_iri.split("#")[1]] = data_entity
-            self.existing_data_entity_list.append(data_entity)
+            task_entity.output_dict[output_parent_entity_iri.split("#")[1]] = output_data_entity
+            self.existing_data_entity_list.append(output_data_entity)
 
     def _create_next_task_cli(self) -> Union[None, Task]:
         """
         Instantiates and adds task (without method) based on user input to self.output_kg
         Adds task's output data entities to self.existing_data_entity_list
         Returns:
             None: in case user wants to end the pipeline creation
@@ -524,14 +539,16 @@
                 range_iri = pair[1]
                 input_property = Literal(
                     lexical_or_value=input("\t{} in range({}): ".format(pair[0].split("#")[1], range)),
                     datatype=range_iri,
                 )
                 add_literal(self.output_kg, task_to_attach_to, property_instance, input_property)
 
+        check_kg_executability(self.output_kg)
+
     def start_pipeline_creation(self, pipeline_name: str, input_data_path: str) -> None:
         """
         Handles the pipeline creation through CLI
         Args:
             pipeline_name: name for the pipeline
             input_data_path: path for the input data to be used by the pipeline's tasks
         """
@@ -554,14 +571,16 @@
 
     def save_created_kg(self, file_path: str) -> None:
         """
         Saves self.output_kg to a file
         Args:
             file_path: path of the output file
         """
+        check_kg_executability(self.output_kg)
+
         dir_path = os.path.dirname(file_path)
         os.makedirs(dir_path, exist_ok=True)
 
         self.output_kg.serialize(destination=file_path)
         print(f"Executable KG saved in {file_path}")
 
     def _property_value_to_field_value(self, property_value: str) -> Union[str, DataEntity]:
@@ -680,15 +699,18 @@
 
         # create Task sub-class object
         if canvas_method:
             task = Class(task_iri, Task(task_parent_iri), canvas_method)
         else:
             task = Class(task_iri, Task(task_parent_iri))
 
-        for s, p, o in self.input_kg.triples((URIRef(task_iri), None, None)):
+        task_related_triples = self.input_kg.triples((URIRef(task_iri), None, None))
+        method_related_triples = self.input_kg.triples((URIRef(method.iri), None, None))
+
+        for s, p, o in itertools.chain(task_related_triples, method_related_triples):
             # parse property name and value
             field_name = property_name_to_field_name(str(p))
             if not hasattr(task, field_name) or field_name == "type":
                 continue
             field_value = self._property_value_to_field_value(str(o))
 
             # set field value dynamically
```

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/kg_schema.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/kg_schema.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/task.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/task.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/README.md` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/README.md`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/ml_tasks.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/ml_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/statistic_tasks.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/statistic_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/classes/tasks/visual_tasks.py` & `exe_kg_lib-3.0.0/exe_kg_lib/classes/tasks/visual_tasks.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/cli/main.py` & `exe_kg_lib-3.0.0/exe_kg_lib/cli/main.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/cli_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/kg_creation_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/kg_creation_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/query_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/query_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,30 @@
         "?m rdfs:subClassOf " + namespace_prefix + ":AtomicMethod . }",
         initBindings={"entity_iri": URIRef(entity_parent_iri)},
     )
 
 
 def get_input_properties_and_inputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
     return input_kg.query(
-        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
+        "\nSELECT ?p ?m ?s WHERE {?p rdfs:domain ?entity_iri . "
         "?p rdfs:range ?m ."
         "?p rdfs:subPropertyOf " + namespace_prefix + ":hasInput ."
-        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
+        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . "
+        "?m " + namespace_prefix + ":hasDataStructure ?s . }",
         initBindings={"entity_iri": URIRef(entity_parent_iri)},
     )
 
 
 def get_output_properties_and_outputs(input_kg, namespace_prefix, entity_parent_iri: str) -> query.Result:
     return input_kg.query(
-        "\nSELECT ?p ?m WHERE {?p rdfs:domain ?entity_iri . "
+        "\nSELECT ?p ?m ?s WHERE {?p rdfs:domain ?entity_iri . "
         "?p rdfs:range ?m ."
         "?p rdfs:subPropertyOf " + namespace_prefix + ":hasOutput ."
-        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . }",
+        "?m rdfs:subClassOf " + namespace_prefix + ":DataEntity . "
+        "?m " + namespace_prefix + ":hasDataStructure ?s . }",
         initBindings={"entity_iri": URIRef(entity_parent_iri)},
     )
 
 
 def query_pipeline_info(kg, namespace_prefix):
     return kg.query(
         f"\nSELECT ?p ?i ?t WHERE {{?p rdf:type {namespace_prefix}:Pipeline ;"
```

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/string_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/ml_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/ml_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/statistic_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/statistic_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/exe_kg_lib/utils/task_utils/visual_utils.py` & `exe_kg_lib-3.0.0/exe_kg_lib/utils/task_utils/visual_utils.py`

 * *Files identical despite different names*

### Comparing `exe_kg_lib-2.0.4/pyproject.toml` & `exe_kg_lib-3.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exe-kg-lib"
-version = "2.0.4" # not used when bumping version via poe bump-version-tag or cd.yaml
+version = "3.0.0" # not used when bumping version via poe bump-version-tag or cd.yaml
 description = "Library for executable ML pipelines represented by KGs."
 license = "AGPL-3.0"
 authors = ["Antonis Klironomos <antonis.klironomos@de.bosch.com>", "Mohamed Gad-Elrab <mohamed.gad-elrab@de.bosch.com>"]
 
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Developers",
@@ -31,14 +31,15 @@
 pandas = "^1.5.2"
 scikit-learn = "^1.1.3"
 black = {extras = ["d"], version = ">=22.10,<24.0"}
 matplotlib = "^3.6.2"
 rdflib = "^6.2.0"
 mkdocs = "^1.4.2"
 typer-cli = "^0.0.13"
+pyshacl = "^0.21.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=22.10,<24.0"
 genbadge = {extras = ["coverage", "tests"], version = "^1.1.0"}
 isort = {extras = ["colors"], version = "^5.10.1"}
 mkdocs-gen-files = "^0.4.0"
 mkdocs-git-revision-date-localized-plugin = "^1.1.0"
@@ -49,14 +50,15 @@
 poethepoet = ">=0.16.5,<0.19.0"
 pre-commit = ">=2.20,<4.0"
 pytest = ">=7.2.0"
 pytest-cov = "^4.0.0"
 pytest-html = "^3.2.0"
 pytest-xdist = "^3.0.2"
 pyupgrade = "^3.2.3"
+shexer = "^2.1.1"
 
 # Tools config
 [tool.black]
 line-length = 120
 
 [tool.coverage.report]
 fail_under = 60
```

### Comparing `exe_kg_lib-2.0.4/PKG-INFO` & `exe_kg_lib-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exe-kg-lib
-Version: 2.0.4
+Version: 3.0.0
 Summary: Library for executable ML pipelines represented by KGs.
 Home-page: https://boschresearch.github.io/ExeKGLib
 License: AGPL-3.0
 Author: Antonis Klironomos
 Author-email: antonis.klironomos@de.bosch.com
 Maintainer: Antonis Klironomos
 Maintainer-email: antonis.klironomos@de.bosch.com
@@ -15,21 +15,21 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: black[d] (>=22.10,<24.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pyshacl (>=0.21.0,<0.22.0)
 Requires-Dist: rdflib (>=6.2.0,<7.0.0)
 Requires-Dist: scikit-learn (>=1.1.3,<2.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
 Project-URL: Repository, https://github.com/boschresearch/ExeKGLib
 Description-Content-Type: text/markdown
```

