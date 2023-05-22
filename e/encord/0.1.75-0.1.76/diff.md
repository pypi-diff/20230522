# Comparing `tmp/encord-0.1.75.tar.gz` & `tmp/encord-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.75.tar", max compression
+gzip compressed data, was "encord-0.1.76.tar", max compression
```

## Comparing `encord-0.1.75.tar` & `encord-0.1.76.tar`

### file list

```diff
@@ -1,73 +1,75 @@
--rw-r--r--   0        0        0    11330 2023-05-09 09:11:04.774966 encord-0.1.75/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-09 09:11:04.774966 encord-0.1.75/README.md
--rw-r--r--   0        0        0       84 2023-05-09 09:11:04.774966 encord-0.1.75/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-05-09 09:11:04.794966 encord-0.1.75/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-05-09 09:11:04.794966 encord-0.1.75/encord/_version.py
--rw-r--r--   0        0        0    47909 2023-05-09 09:11:04.794966 encord-0.1.75/encord/client.py
--rw-r--r--   0        0        0    10825 2023-05-09 09:11:04.794966 encord-0.1.75/encord/configs.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-05-09 09:11:04.794966 encord-0.1.75/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-05-09 09:11:04.794966 encord-0.1.75/encord/dataset.py
--rw-r--r--   0        0        0     5823 2023-05-09 09:11:04.794966 encord-0.1.75/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/__init__.py
--rw-r--r--   0        0        0      535 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/constants.py
--rw-r--r--   0        0        0     6607 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/error_utils.py
--rw-r--r--   0        0        0     5999 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/query_methods.py
--rw-r--r--   0        0        0     1691 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/request.py
--rw-r--r--   0        0        0     5880 2023-05-09 09:11:04.794966 encord-0.1.75/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/classification.py
--rw-r--r--   0        0        0    29709 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   135230 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-05-09 09:11:04.794966 encord-0.1.75/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-05-09 09:11:04.794966 encord-0.1.75/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32206 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      201 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/formatter.py
--rw-r--r--   0        0        0     1155 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-05-09 09:11:04.794966 encord-0.1.75/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    38903 2023-05-09 09:11:04.794966 encord-0.1.75/encord/project.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9526 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-05-09 09:11:04.798966 encord-0.1.75/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27801 2023-05-09 09:11:04.798966 encord-0.1.75/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4231 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-05-09 09:11:04.798966 encord-0.1.75/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1659 2023-05-09 09:11:04.798966 encord-0.1.75/pyproject.toml
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.75/setup.py
--rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.75/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-05-22 16:10:18.357820 encord-0.1.76/LICENSE
+-rw-r--r--   0        0        0     2595 2023-05-22 16:10:18.357820 encord-0.1.76/README.md
+-rw-r--r--   0        0        0       84 2023-05-22 16:10:18.357820 encord-0.1.76/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-22 16:10:18.377820 encord-0.1.76/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-22 16:10:18.377820 encord-0.1.76/encord/_version.py
+-rw-r--r--   0        0        0    49178 2023-05-22 16:10:18.377820 encord-0.1.76/encord/client.py
+-rw-r--r--   0        0        0    10825 2023-05-22 16:10:18.377820 encord-0.1.76/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/enums.py
+-rw-r--r--   0        0        0     3211 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-22 16:10:18.377820 encord-0.1.76/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-05-22 16:10:18.377820 encord-0.1.76/encord/dataset.py
+-rw-r--r--   0        0        0     6302 2023-05-22 16:10:18.377820 encord-0.1.76/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/__init__.py
+-rw-r--r--   0        0        0     5329 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/limits.py
+-rw-r--r--   0        0        0     7875 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-05-22 16:10:18.377820 encord-0.1.76/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/classification.py
+-rw-r--r--   0        0        0    29709 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/common.py
+-rw-r--r--   0        0        0      172 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   139903 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      137 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      148 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-05-22 16:10:18.377820 encord-0.1.76/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-05-22 16:10:18.377820 encord-0.1.76/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5377 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-05-22 16:10:18.377820 encord-0.1.76/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32206 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      188 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/model.py
+-rw-r--r--   0        0        0      745 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8844 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-22 16:10:18.381820 encord-0.1.76/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    39203 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-05-22 16:10:18.381820 encord-0.1.76/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27840 2023-05-22 16:10:18.381820 encord-0.1.76/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-05-22 16:10:18.381820 encord-0.1.76/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1685 2023-05-22 16:10:18.381820 encord-0.1.76/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 encord-0.1.76/setup.py
+-rw-r--r--   0        0        0     3774 1970-01-01 00:00:00.000000 encord-0.1.76/PKG-INFO
```

### Comparing `encord-0.1.75/LICENSE` & `encord-0.1.76/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/README.md` & `encord-0.1.76/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/client.py` & `encord-0.1.76/encord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
             else:
                 raise encord.exceptions.EncordException(message="An error has occurred during video upload.")
         else:
             raise encord.exceptions.EncordException(message="{} does not point to a file.".format(file_path))
 
     def create_image_group(
         self,
-        file_paths: List[str],
+        file_paths: Iterable[str],
         max_workers: Optional[int] = None,
         cloud_upload_settings: CloudUploadSettings = CloudUploadSettings(),
         title: Optional[str] = None,
         *,
         create_video: bool = True,
     ):
         """
@@ -731,23 +731,25 @@
         data_title_like: Optional[str] = None,
         workflow_graph_node_title_eq: Optional[str] = None,
         workflow_graph_node_title_like: Optional[str] = None,
     ) -> List[LabelRowMetadata]:
         """
         This function is documented in :meth:`encord.project.Project.list_label_rows`.
         """
-        if label_statuses:
-            label_statuses = [label_status.value for label_status in label_statuses]
+
+        label_statuses_values = (
+            [label_status.value for label_status in label_statuses] if label_statuses is not None else None
+        )
         edited_before = parse_datetime("edited_before", edited_before)
         edited_after = parse_datetime("edited_after", edited_after)
 
         payload = {
             "edited_before": edited_before,
             "edited_after": edited_after,
-            "label_statuses": label_statuses,
+            "label_statuses": label_statuses_values,
             "shadow_data_state": shadow_data_state.value if shadow_data_state else None,
             "include_uninitialised_labels": include_uninitialised_labels,
             "data_hashes": data_hashes,
             "label_hashes": label_hashes,
             "data_title_eq": data_title_eq,
             "data_title_like": data_title_like,
             "workflow_graph_node_title_eq": workflow_graph_node_title_eq,
@@ -864,20 +866,53 @@
     def save_label_row(self, uid, label):
         """
         This function is documented in :meth:`encord.project.Project.save_label_row`.
         """
         label = LabelRow(label)
         return self._querier.basic_setter(LabelRow, uid, payload=label)
 
+    def save_label_rows(self, uids: List[str], payload=List[LabelRow]):
+        """
+        This function is meant for internal use, please consider using :class:`encord.objects.LabelRowV2` class instead
+
+        Saves multiple label rows. See :meth:`.save_label_row`
+
+        Args:
+            uids: list of label hashes
+            payload: list of LabelRow objects
+
+        Returns:
+            None
+        """
+        payload = {
+            "multi_request": True,
+            "labels": payload,
+        }
+        return self._querier.basic_setter(LabelRow, uid=uids, payload=payload)
+
     def create_label_row(self, uid):
         """
         This function is documented in :meth:`encord.project.Project.create_label_row`.
         """
         return self._querier.basic_put(LabelRow, uid=uid, payload=None)
 
+    def create_label_rows(self, uids: List[str]) -> List[LabelRow]:
+        """
+        This function is meant for internal use, please consider using :class:`encord.objects.LabelRowV2` class instead
+
+        Create multiple label rows. See :meth:`.create_label_row`
+
+        Args:
+            uids: list of data uids where label_status is NOT_LABELLED.
+
+        Returns:
+            List[LabelRow]: A list of created label rows
+        """
+        return self._querier.put_multiple(LabelRow, uid=uids, payload={"multi_request": True})
+
     def submit_label_row_for_review(self, uid):
         """
         This function is documented in :meth:`encord.project.Project.submit_label_row_for_review`.
         """
         return self._querier.basic_put(Review, uid=uid, payload=None)
 
     def add_datasets(self, dataset_hashes: List[str]) -> bool:
@@ -982,22 +1017,22 @@
                 "title": title,
                 "description": description,
                 "features": features,
                 "model": model,
             }
         )
 
-        model = Model(
+        model_payload = Model(
             {
                 "model_operation": ModelOperations.CREATE.value,
                 "model_parameters": model_row,
             }
         )
 
-        return self._querier.basic_put(Model, None, payload=model)
+        return self._querier.basic_put(Model, None, payload=model_payload)
 
     def model_delete(self, uid: str) -> bool:
         """
         This function is documented in :meth:`encord.project.Project.model_delete`.
         """
 
         return self._querier.basic_delete(Model, uid=uid)
@@ -1218,15 +1253,19 @@
 
         return video, images
 
     def get_websocket_url(self) -> str:
         return self._config.get_websocket_url()
 
     def get_label_logs(
-        self, user_hash: str = None, data_hash: str = None, from_unix_seconds: int = None, to_unix_seconds: int = None
+        self,
+        user_hash: Optional[str] = None,
+        data_hash: Optional[str] = None,
+        from_unix_seconds: Optional[int] = None,
+        to_unix_seconds: Optional[int] = None,
     ) -> List[LabelLog]:
         """
         This function is documented in :meth:`encord.project.Project.get_label_logs`.
         """
 
         # Flag for backwards compatibility
         include_user_email_and_interface_key = True
```

### Comparing `encord-0.1.75/encord/configs.py` & `encord-0.1.76/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/constants/enums.py` & `encord-0.1.76/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/constants/model.py` & `encord-0.1.76/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/constants/model_weights.py` & `encord-0.1.76/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/constants/string_constants.py` & `encord-0.1.76/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/constants/test/test_enums.py` & `encord-0.1.76/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/dataset.py` & `encord-0.1.76/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/exceptions.py` & `encord-0.1.76/encord/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,27 +10,40 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 import time
 from datetime import datetime, timezone
+from dataclasses import dataclass, field, fields
+from typing import Optional
+
+
+@dataclass
+class ExceptionContext:
+    timestamp: datetime = field(default_factory=lambda: datetime.now(tz=timezone.utc).isoformat())
+
+    def __str__(self):
+        return " ".join(
+            f"{object_field.name}={getattr(self, object_field.name)!r}"
+            for object_field in fields(self)
+            if getattr(self, object_field.name) is not None
+        )
 
 
 class EncordException(Exception):
     """Base class for all exceptions."""
 
-    def __init__(self, message):
+    def __init__(self, message: str, context: Optional[ExceptionContext] = None):
         super().__init__(message)
         self.message = message
+        self.context = context if context is not None else ExceptionContext()
 
     def __str__(self):
-        datetime_postfix = f"Error timestamp: {datetime.now(tz=timezone.utc).isoformat()}."
-
-        return f"{self.message} {datetime_postfix}"
+        return f"{self.message} {self.context}"
 
 
 CordException = EncordException
 
 
 class InitialisationError(EncordException):
     """Exception thrown when API key fails to initialise."""
```

### Comparing `encord-0.1.75/encord/http/constants.py` & `encord-0.1.76/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/http/error_utils.py` & `encord-0.1.76/encord/http/error_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,113 +37,131 @@
 DUPLICATE_SSH_KEY_ERROR = ["DUPLICATE_SSH_KEY_ERROR"]
 SSH_KEY_NOT_FOUND_ERROR = ["SSH_KEY_NOT_FOUND_ERROR"]
 INVALID_ARGUMENTS_ERROR = ["INVALID_ARGUMENTS_ERROR"]
 MULTI_LABEL_LIMIT_ERROR = ["MULTI_LABEL_LIMIT_ERROR"]
 WRONG_PROJECT_TYPE_ERROR = ["WRONG_PROJECT_TYPE_ERROR"]
 
 
-def check_error_response(response, payload=None):
+def check_error_response(response, context=None, payload=None):
     """
     Checks server response.
     Called if HTTP response status code is an error response.
     """
     if response == AUTHENTICATION_ERROR:
-        raise AuthenticationError("You are not authenticated to access the Encord platform.")
+        raise AuthenticationError("You are not authenticated to access the Encord platform.", context=context)
 
     if response == AUTHORISATION_ERROR:
-        raise AuthorisationError("You are not authorised to access this asset.")
+        raise AuthorisationError("You are not authorised to access this asset.", context=context)
 
     if response == RESOURCE_NOT_FOUND_ERROR:
         if payload:
-            raise ResourceNotFoundError(payload)
-        raise ResourceNotFoundError("The requested resource was not found in the database.")
+            raise ResourceNotFoundError(payload, context=context)
+        raise ResourceNotFoundError("The requested resource was not found in the database.", context=context)
 
     if response == METHOD_NOT_ALLOWED_ERROR:
-        raise MethodNotAllowedError("HTTP method is not allowed.")
+        raise MethodNotAllowedError("HTTP method is not allowed.", context=context)
 
     if response == UNKNOWN_ERROR:
-        raise UnknownException("An unknown error occurred.")
+        raise UnknownException("An unknown error occurred.", context=context)
 
     if response == OPERATION_NOT_ALLOWED_ERROR:
-        raise OperationNotAllowed("The read/write operation is not allowed by the API key.")
+        raise OperationNotAllowed("The read/write operation is not allowed by the API key.", context=context)
 
     if response == ANSWER_DICTIONARY_ERROR:
-        raise AnswerDictionaryError("An object or classification is missing in the answer dictionaries.")
+        raise AnswerDictionaryError(
+            "An object or classification is missing in the answer dictionaries.", context=context
+        )
 
     if response == CORRUPTED_LABEL_ERROR:
         raise CorruptedLabelError(
             "The label blurb is corrupted. This could be due to the number of "
-            "frame labels exceeding the number of frames in the labelled video."
+            "frame labels exceeding the number of frames in the labelled video.",
+            context=context,
         )
 
     if response == FILE_TYPE_NOT_SUPPORTED_ERROR:
-        raise FileTypeNotSupportedError("Supported file types are: image/jpeg, image/png, video/webm, video/mp4.")
+        raise FileTypeNotSupportedError(
+            "Supported file types are: image/jpeg, image/png, video/webm, video/mp4.", context=context
+        )
 
     if response == FILE_SIZE_NOT_SUPPORTED_ERROR:
-        raise FileSizeNotSupportedError("The combined size of the input files is larger than the supported limit")
+        raise FileSizeNotSupportedError(
+            "The combined size of the input files is larger than the supported limit", context=context
+        )
 
     if response == FEATURE_DOES_NOT_EXIST_ERROR:
-        raise FeatureDoesNotExistError("The passed feature does not exist in the project ontology.")
+        raise FeatureDoesNotExistError("The passed feature does not exist in the project ontology.", context=context)
 
     if response == MODEL_WEIGHTS_INCONSISTENT_ERROR:
-        raise ModelWeightsInconsistentError("The passed model weights are incompatible with the selected model.")
+        raise ModelWeightsInconsistentError(
+            "The passed model weights are incompatible with the selected model.", context=context
+        )
 
     if response == MODEL_FEATURES_INCONSISTENT_ERROR:
-        raise ModelFeaturesInconsistentError("The passed features are incompatible with the selected model.")
+        raise ModelFeaturesInconsistentError(
+            "The passed features are incompatible with the selected model.", context=context
+        )
 
     if response == UPLOAD_OPERATION_NOT_SUPPORTED_ERROR:
         raise UploadOperationNotSupportedError(
-            "Uploading a file to an external (e.g. S3/GCP/Azure) dataset is not " "permitted."
+            "Uploading a file to an external (e.g. S3/GCP/Azure) dataset is not " "permitted.", context=context
         )
 
     if response == DETECTION_RANGE_INVALID_ERROR:
         raise DetectionRangeInvalidError(
-            "The detection range is invalid (e.g. less than 0, or" " higher than num frames in the video)"
+            "The detection range is invalid (e.g. less than 0, or" " higher than num frames in the video)",
+            context=context,
         )
 
     if response == INVALID_DATE_FORMAT_ERROR:
-        raise InvalidDateFormatError("Invalid date format supplied as input")
+        raise InvalidDateFormatError("Invalid date format supplied as input", context=context)
 
     if response == RESOURCE_EXISTS_ERROR:
         raise ResourceExistsError(
-            "Trying to create a resource that already exists. " "Payload for this failure is: " + str(payload)
+            "Trying to create a resource that already exists. " "Payload for this failure is: " + str(payload),
+            context=context,
         )
 
     if response == DUPLICATE_SSH_KEY_ERROR:
-        raise DuplicateSshKeyError("The used SSH key exists more than once. Please create a unique user SSH key.")
+        raise DuplicateSshKeyError(
+            "The used SSH key exists more than once. Please create a unique user SSH key.", context=context
+        )
 
     if response == SSH_KEY_NOT_FOUND_ERROR:
         raise SshKeyNotFound(
-            "The used SSH key does not exist on the Encord platform. Please add this SSH key to your user profile."
+            "The used SSH key does not exist on the Encord platform. Please add this SSH key to your user profile.",
+            context=context,
         )
 
     if response == INVALID_ARGUMENTS_ERROR:
         default_message = "Some of the arguments to the SDK function were invalid."
         if payload is None:
             message = default_message
         else:
             message = payload
-        raise InvalidArgumentsError(message)
+        raise InvalidArgumentsError(message, context=context)
 
     if response == MULTI_LABEL_LIMIT_ERROR:
         maximum_labels_allowed = payload["maximum_labels_allowed"]
         raise MultiLabelLimitError(
             f"Too many labels were requested. The limit is {maximum_labels_allowed}. Please reduce the amount "
             "of requested labels to stay under the reported limit.",
             maximum_labels_allowed=maximum_labels_allowed,
+            context=context,
         )
 
     if response == WRONG_PROJECT_TYPE_ERROR:
         default_message = "Operation is not supported by the project type"
         if payload is None:
             message = default_message
         else:
             message = payload
-        raise WrongProjectTypeError(message)
+        raise WrongProjectTypeError(message, context=context)
 
     payload_string = ""
     if payload:
         payload_string = f" with the following payload `{payload}`"
     raise GenericServerError(
         f"The Encord server has reported an error of type `{response}`{payload_string}. Please do not parse this error "
-        "programmatically, instead please upgrade the SDK to the latest version to get the exact error."
+        "programmatically, instead please upgrade the SDK to the latest version to get the exact error.",
+        context=context,
     )
```

### Comparing `encord-0.1.75/encord/http/querier.py` & `encord-0.1.76/encord/http/querier.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,127 +11,168 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 import dataclasses
 import logging
 import platform
+import uuid
+import random
 from contextlib import contextmanager
-from typing import Any, List, Optional, Type, TypeVar
+from typing import Any, List, Tuple, Optional, Type, TypeVar, Generator
 
 import requests
 import requests.exceptions
-from requests import Session
+from requests import Session, Response
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from encord.configs import BaseConfig
 from encord.exceptions import *
 from encord.http.error_utils import check_error_response
 from encord.http.query_methods import QueryMethods
 from encord.http.request import Request
 from encord.orm.formatter import Formatter
 from encord._version import __version__ as encord_version
 
 logger = logging.getLogger(__name__)
 
+HEADER_USER_AGENT = "User-Agent"
+HEADER_CLOUD_TRACE_CONTEXT = "X-Cloud-Trace-Context"
+
+
+@dataclass
+class RequestContext(ExceptionContext):
+    trace_id: Optional[str] = None
+    span_id: Optional[str] = None
+
 
 class Querier:
     """Querier for DB get/post requests."""
 
     T = TypeVar("T")
 
     def __init__(self, config: BaseConfig):
         self._config = config
 
     def basic_getter(self, db_object_type: Type[T], uid=None, payload=None) -> T:
         """Single DB object getter."""
-        request = self.request(QueryMethods.GET, db_object_type, uid, self._config.read_timeout, payload=payload)
-        res = self.execute(request)
+        request = self._request(QueryMethods.GET, db_object_type, uid, self._config.read_timeout, payload=payload)
+        res, context = self._execute(request)
         if res:
             return self._parse_response(db_object_type, res)
         else:
-            raise ResourceNotFoundError("Resource not found.")
+            raise ResourceNotFoundError("Resource not found.", context=context)
 
     def get_multiple(self, object_type: Type[T], uid=None, payload=None) -> List[T]:
-        request = self.request(QueryMethods.GET, object_type, uid, self._config.read_timeout, payload=payload)
-        result = self.execute(request)
+        return self._request_multiple(QueryMethods.GET, object_type, uid, payload)
+
+    def post_multiple(self, object_type: Type[T], uid=None, payload=None) -> List[T]:
+        return self._request_multiple(QueryMethods.POST, object_type, uid, payload)
+
+    def put_multiple(self, object_type: Type[T], uid=None, payload=None) -> List[T]:
+        return self._request_multiple(QueryMethods.PUT, object_type, uid, payload)
+
+    def _request_multiple(self, method: QueryMethods, object_type: Type[T], uid: List[str], payload=None) -> List[T]:
+        request = self._request(method, object_type, uid, self._config.read_timeout, payload=payload)
+        result, context = self._execute(request)
 
         if result is not None:
             return [self._parse_response(object_type, item) for item in result]
         else:
-            raise ResourceNotFoundError(f"[{object_type}] not found for query with uid=[{uid}] and payload=[{payload}]")
+            raise ResourceNotFoundError(
+                f"[{object_type}] not found for query with uid=[{uid}] and payload=[{payload}]", context=context
+            )
 
     @staticmethod
     def _parse_response(object_type: Type[T], item: dict) -> T:
         if issubclass(object_type, Formatter):
             return object_type.from_dict(item)
         elif dataclasses.is_dataclass(object_type):
             return object_type(**item)
         else:
             return object_type(item)
 
     def basic_delete(self, db_object_type: Type[T], uid=None):
         """Single DB object getter."""
-        request = self.request(
+        request = self._request(
             QueryMethods.DELETE,
             db_object_type,
             uid,
             self._config.read_timeout,
         )
 
-        return self.execute(request)
+        res, _ = self._execute(request)
+        return res
 
     def basic_setter(self, db_object_type: Type[T], uid, payload):
         """Single DB object setter."""
-        request = self.request(
+        request = self._request(
             QueryMethods.POST,
             db_object_type,
             uid,
             self._config.write_timeout,
             payload=payload,
         )
 
-        res = self.execute(request)
+        res, context = self._execute(request)
 
         if res:
             return res
         else:
-            raise RequestException("Setting %s with uid %s failed." % (db_object_type, uid))
+            raise RequestException(f"Setting {db_object_type} with uid {uid} failed.", context=context)
 
     def basic_put(self, db_object_type, uid, payload, enable_logging=True):
         """Single DB object put request."""
-        request = self.request(
+        request = self._request(
             QueryMethods.PUT,
             db_object_type,
             uid,
             self._config.write_timeout,
             payload=payload,
         )
 
-        res = self.execute(request, enable_logging)
+        res, context = self._execute(request, enable_logging)
 
         if res:
             return res
         else:
-            raise RequestException("Setting %s with uid %s failed." % (db_object_type, uid))
+            raise RequestException(f"Setting {db_object_type} with uid {uid} failed.", context=context)
 
     @staticmethod
     def _user_agent():
-        return f"Encord Python SDK {encord_version}; Python {platform.python_version()}"
+        return f"encord-sdk-python/{encord_version} python/{platform.python_version()}"
+
+    @staticmethod
+    def _tracing_id() -> str:
+        return f"{uuid.uuid4().hex}/{random.randint(1, 2**63 - 1)};o=1"
+
+    @staticmethod
+    def _exception_context_from_response(response: Response) -> RequestContext:
+        try:
+            x_cloud_trace_context = response.headers.get(HEADER_CLOUD_TRACE_CONTEXT)
+            if x_cloud_trace_context is None:
+                return RequestContext()
+
+            x_cloud_trace_context = x_cloud_trace_context.split(";")[0]
+            trace_id, span_id = (x_cloud_trace_context.split("/") + [None, None])[:2]
+            return RequestContext(trace_id=trace_id, span_id=span_id)
+        except Exception:
+            return RequestContext()
 
-    def request(self, method, db_object_type: Type[T], uid, timeout, payload=None):
+    def _request(self, method, db_object_type: Type[T], uid, timeout, payload=None):
         request = Request(method, db_object_type, uid, timeout, self._config.connect_timeout, payload)
 
         request.headers = self._config.define_headers(request.data)
-        request.headers["User-Agent"] = self._user_agent()
+        request.headers[HEADER_USER_AGENT] = self._user_agent()
+        request.headers[HEADER_CLOUD_TRACE_CONTEXT] = self._tracing_id()
 
         return request
 
-    def execute(self, request, enable_logging=True) -> Any:
+    def _execute(self, request: Request, enable_logging=True) -> Tuple[Any, RequestContext]:
         """Execute a request."""
         if enable_logging:
             logger.info("Request: %s", (request.data[:100] + "..") if len(request.data) > 100 else request.data)
 
         req = requests.Request(
             method=request.http_method,
             url=self._config.endpoint,
@@ -142,30 +183,31 @@
         timeouts = (request.connect_timeout, request.timeout)
 
         req_settings = self._config.requests_settings
         with create_new_session(
             max_retries=req_settings.max_retries, backoff_factor=req_settings.backoff_factor
         ) as session:
             res = session.send(req, timeout=timeouts)
+            context = self._exception_context_from_response(res)
 
             try:
                 res_json = res.json()
             except Exception as e:
-                raise EncordException("Error parsing JSON response: %s" % res.text) from e
+                raise RequestException(f"Error parsing JSON response: {res.text}", context=context) from e
 
         if res_json.get("status") != requests.codes.ok:
             response = res_json.get("response")
             extra_payload = res_json.get("payload")
-            check_error_response(response, extra_payload)
+            check_error_response(response, context, extra_payload)
 
-        return res_json.get("response")
+        return res_json.get("response"), context
 
 
 @contextmanager
-def create_new_session(max_retries: Optional[int] = None, backoff_factor: float = 0) -> Session:
+def create_new_session(max_retries: Optional[int] = None, backoff_factor: float = 0) -> Generator[Session, None, None]:
     retry_policy = Retry(total=max_retries, connect=max_retries, read=max_retries, backoff_factor=backoff_factor)
 
     with Session() as session:
         session.mount("http://", HTTPAdapter(max_retries=retry_policy))
         session.mount("https://", HTTPAdapter(max_retries=retry_policy))
 
         yield session
```

### Comparing `encord-0.1.75/encord/http/query_methods.py` & `encord-0.1.76/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/http/request.py` & `encord-0.1.76/encord/http/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import json
-from typing import Dict
+from typing import Dict, Optional
 
 from encord.http.query_methods import QueryMethods
 
 
 class Request(object):
     """
     Request object. Takes query parameters and prepares them for execution.
@@ -28,30 +28,30 @@
         self,
         query_method,
         db_object_type,
         uid,
         timeout,
         connect_timeout,
         payload,
-    ):
+    ) -> None:
         self.http_method = QueryMethods.POST
         self.data: str = json.dumps(
             {
                 "query_type": db_object_type.__name__.lower(),
                 "query_method": query_method,
                 "values": {
                     "uid": uid,
                     "payload": payload,
                 },
             }
         )
         self.timeout = timeout
         self.connect_timeout = connect_timeout
 
-        self.headers: Dict = None
+        self.headers: Optional[Dict] = None
 
     def __str__(self):
         return f"Request({self.http_method}, {self.data}, {self.headers}, {self.timeout}, {self.connect_timeout})"
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `encord-0.1.75/encord/http/utils.py` & `encord-0.1.76/encord/http/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import mimetypes
 import os.path
 from dataclasses import dataclass
-from typing import List, Optional, Type, TypeVar, Union
+from typing import List, Optional, Type, TypeVar, Union, Iterable
 
 from tqdm import tqdm
 
 from encord.configs import BaseConfig
 from encord.exceptions import CloudUploadError
 from encord.http.querier import Querier, create_new_session
 from encord.orm.dataset import (
@@ -45,34 +45,37 @@
     even if a few images were not successfully uploaded. The unsuccessfully uploaded images will then be logged.
     """
 
 
 OrmT = TypeVar("OrmT")
 
 
+def _get_content_type(orm_class: Union[Type[Images], Type[Video], Type[DicomSeries]], file_path: str) -> Optional[str]:
+    if orm_class == Images:
+        return mimetypes.guess_type(file_path)[0]
+    elif orm_class == Video:
+        return "application/octet-stream"
+    elif orm_class == DicomSeries:
+        return "application/dicom"
+    else:
+        raise ValueError(f"Unsupported type `{orm_class}`")
+
+
 def upload_to_signed_url_list(
-    file_paths: List[str],
+    file_paths: Iterable[str],
     config: BaseConfig,
     querier: Querier,
     orm_class: Union[Type[Images], Type[Video], Type[DicomSeries]],
     cloud_upload_settings: CloudUploadSettings,
 ) -> List[Union[SignedVideoURL, SignedImageURL, SignedDicomURL]]:
     """Upload files and return the upload returns in the same order as the file paths supplied."""
     failed_uploads = []
     successful_uploads = []
     for file_path in tqdm(file_paths):
-        if orm_class == Images:
-            content_type = mimetypes.guess_type(file_path)[0]
-        elif orm_class == Video:
-            content_type = "application/octet-stream"
-        elif orm_class == DicomSeries:
-            content_type = "application/dicom"
-        else:
-            raise RuntimeError(f"Unsupported type `{orm_class}`")
-
+        content_type = _get_content_type(orm_class, file_path)
         file_name = os.path.basename(file_path)
         signed_url = _get_signed_url(file_name, orm_class, querier)
         assert signed_url.get("title", "") == file_name, "Ordering issue"
 
         try:
             if cloud_upload_settings.max_retries is not None:
                 max_retries = cloud_upload_settings.max_retries
@@ -96,15 +99,17 @@
 
     if failed_uploads:
         logger.warning("The upload was incomplete for the following items: %s", failed_uploads)
 
     return successful_uploads
 
 
-def upload_video_to_encord(signed_url: SignedVideoURL, video_title: Optional[str], querier: Querier) -> Video:
+def upload_video_to_encord(
+    signed_url: Union[SignedVideoURL, SignedImageURL, SignedDicomURL], video_title: Optional[str], querier: Querier
+) -> Video:
     payload = {
         "signed_url": signed_url["signed_url"],
         "data_hash": signed_url["data_hash"],
         "title": signed_url["title"],
         "file_link": signed_url["file_link"],
         "video_title": video_title,
     }
@@ -112,40 +117,43 @@
         Video,
         uid=signed_url.get("data_hash"),
         payload=payload,
         enable_logging=False,
     )
 
 
-def upload_images_to_encord(signed_urls: List[dict], querier: Querier) -> Images:
+def upload_images_to_encord(
+    signed_urls: List[Union[SignedVideoURL, SignedImageURL, SignedDicomURL]], querier: Querier
+) -> Images:
     return querier.basic_put(Images, uid=None, payload=signed_urls, enable_logging=False)
 
 
 def _get_signed_url(
     file_name: str, orm_class: Union[Type[Images], Type[Video], Type[DicomSeries]], querier: Querier
 ) -> Union[SignedVideoURL, SignedImageURL, SignedDicomURL]:
     if orm_class == Video:
         return querier.basic_getter(SignedVideoURL, uid=file_name)
     elif orm_class == Images:
         return querier.basic_getter(SignedImagesURL, uid=[file_name])[0]
     elif orm_class == DicomSeries:
         return querier.basic_getter(SignedDicomsURL, uid=[file_name])[0]
+    raise ValueError(f"Unsupported type `{orm_class}`")
 
 
 def _upload_single_file(
     file_path: str,
     signed_url: dict,
-    content_type: str,
+    content_type: Optional[str],
     *,
     max_retries: int,
     backoff_factor: float,
     cache_max_age: int = CACHE_DURATION_IN_SECONDS,
 ) -> None:
     with create_new_session(max_retries=max_retries, backoff_factor=backoff_factor) as session:
-        url = signed_url.get("signed_url")
+        url = signed_url["signed_url"]
 
         with open(file_path, "rb") as f:
             res_upload = session.put(
                 url, data=f, headers={"Content-Type": content_type, "Cache-Control": f"max-age={cache_max_age}"}
             )
 
             if res_upload.status_code != 200:
```

### Comparing `encord-0.1.75/encord/objects/common.py` & `encord-0.1.76/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/objects/coordinates.py` & `encord-0.1.76/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/objects/frames.py` & `encord-0.1.76/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/objects/internal_helpers.py` & `encord-0.1.76/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/objects/ontology_labels_impl.py` & `encord-0.1.76/encord/objects/ontology_labels_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Union,
     overload,
 )
 from uuid import uuid4
 
 from dateutil.parser import parse
 
-from encord.client import EncordClientProject
+from encord.client import EncordClientProject, LabelRow as OrmLabelRow
 from encord.constants.enums import DataType
 from encord.exceptions import LabelRowError, OntologyError
 from encord.objects.common import (
     Attribute,
     AttributeClasses,
     AttributeTypes,
     ChecklistAttribute,
@@ -87,15 +87,16 @@
     does_type_match,
     filter_by_type,
     short_uuid_str,
 )
 from encord.orm.formatter import Formatter
 from encord.orm.label_row import AnnotationTaskStatus, LabelRowMetadata, LabelStatus, WorkflowGraphNode
 from encord.exceptions import WrongProjectTypeError
-
+from encord.http.bundle import Bundle, BundleResultHandler, BundleResultMapper
+from encord.http.limits import LABEL_ROW_BUNDLE_GET_LIMIT, LABEL_ROW_BUNDLE_CREATE_LIMIT, LABEL_ROW_BUNDLE_SAVE_LIMIT
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Object:
     """
@@ -853,14 +854,34 @@
             f"object_feature_hash={self._ontology_classification.feature_node_hash})"
         )
 
     def __lt__(self, other) -> bool:
         return self.classification_hash < other.classification_hash
 
 
+@dataclass
+class BundledGetRowsPayload:
+    uids: List[str]
+    get_signed_url: bool
+    include_object_feature_hashes: Optional[Set[str]]
+    include_classification_feature_hashes: Optional[Set[str]]
+    include_reviews: bool
+
+
+@dataclass
+class BundledCreateRowsPayload:
+    uids: List[str]
+
+
+@dataclass
+class BundledSaveRowsPayload:
+    uids: List[str]
+    payload: List[Dict]
+
+
 class LabelRowV2:
     """
     This class represents a single label row. It is corresponding to exactly one data row within a project. It holds all
     the labels for that data row.
 
     You can access a many metadata fields with this class directly. If you want to read or write labels you will need to
     call :meth:`.initialise_labels()` first. To upload your added labels call :meth:`.save()`.
@@ -1023,14 +1044,15 @@
 
     def initialise_labels(
         self,
         include_object_feature_hashes: Optional[Set[str]] = None,
         include_classification_feature_hashes: Optional[Set[str]] = None,
         include_reviews: bool = False,
         overwrite: bool = False,
+        bundle: Optional[Bundle] = None,
     ) -> None:
         """
         Call this function to start reading or writing labels. This will fetch the labels that are currently stored
         in the Encord server. If you only want to inspect a subset of labels, you can filter them. Please note that if
         you filter the labels, and upload them later, you will effectively delete all the labels that had been filtered
         previously.
 
@@ -1052,34 +1074,107 @@
                 subset of classifications and later, save the label, you will effectively delete all the
                 classification instances that are stored in the Encord platform, which were not included in this
                 filtered subset.
             include_reviews: Whether to request read only information about the reviews of the label row.
             overwrite: If the label row was already initialised, you need to set this flag to `True` to overwrite the
                 current labels with the labels stored in the Encord server. If this is `False` and the label row was
                 already initialised, this function will throw an error.
+            bundle: If not passed, initialisation is performed independently. If passed, it will be delayed and
+                initialised along with other objects in the same bundle.
         """
         if self.is_labelling_initialised and not overwrite:
             raise LabelRowError(
                 "You are trying to re-initialise a label row that has already been initialised. This would overwrite "
                 "current labels. If this is your intend, set the `overwrite` flag to `True`."
             )
 
-        get_signed_url = False
-        if self.label_hash is None:
-            label_row_dict = self._project_client.create_label_row(self.data_hash)
-        else:
-            label_row_dict = self._project_client.get_label_row(
+        if bundle is not None:
+            self.__batched_initialise(
+                bundle,
                 uid=self.label_hash,
-                get_signed_url=get_signed_url,
+                get_signed_url=False,
                 include_object_feature_hashes=include_object_feature_hashes,
                 include_classification_feature_hashes=include_classification_feature_hashes,
                 include_reviews=include_reviews,
             )
+        else:
+            if self.label_hash is None:
+                label_row_dict = self._project_client.create_label_row(self.data_hash)
+            else:
+                label_row_dict = self._project_client.get_label_row(
+                    uid=self.label_hash,
+                    get_signed_url=False,
+                    include_object_feature_hashes=include_object_feature_hashes,
+                    include_classification_feature_hashes=include_classification_feature_hashes,
+                    include_reviews=include_reviews,
+                )
 
-        self.from_labels_dict(label_row_dict)
+            self.from_labels_dict(label_row_dict)
+
+    def __batched_initialise(
+        self,
+        bundle: Bundle,
+        uid,
+        get_signed_url,
+        include_object_feature_hashes,
+        include_classification_feature_hashes,
+        include_reviews,
+    ):
+        if self.label_hash is None:
+            bundle.add(
+                operation=self._project_client.create_label_rows,
+                request_reducer=self._bundle_create_rows_reducer,
+                result_mapper=BundleResultMapper(
+                    result_mapping_predicate=self._bundle_create_rows_mapping_predicate,
+                    result_handler=BundleResultHandler(predicate=self.data_hash, handler=self.from_labels_dict),
+                ),
+                payload=BundledCreateRowsPayload(
+                    uids=[self.data_hash],
+                ),
+                limit=LABEL_ROW_BUNDLE_CREATE_LIMIT,
+            )
+        else:
+            bundle.add(
+                operation=self._project_client.get_label_rows,
+                request_reducer=self._bundle_get_rows_reducer,
+                result_mapper=BundleResultMapper(
+                    result_mapping_predicate=self._bundle_get_rows_mapping_predicate,
+                    result_handler=BundleResultHandler(predicate=self.label_hash, handler=self.from_labels_dict),
+                ),
+                payload=BundledGetRowsPayload(
+                    uids=[uid],
+                    get_signed_url=get_signed_url,
+                    include_object_feature_hashes=include_object_feature_hashes,
+                    include_classification_feature_hashes=include_classification_feature_hashes,
+                    include_reviews=include_reviews,
+                ),
+                limit=LABEL_ROW_BUNDLE_GET_LIMIT,
+            )
+
+    @staticmethod
+    def _bundle_create_rows_reducer(
+        bundle_payload: BundledCreateRowsPayload, payload: BundledCreateRowsPayload
+    ) -> BundledCreateRowsPayload:
+        bundle_payload.uids += payload.uids
+        return bundle_payload
+
+    @staticmethod
+    def _bundle_get_rows_reducer(
+        bundle_payload: BundledGetRowsPayload, payload: BundledGetRowsPayload
+    ) -> BundledGetRowsPayload:
+        bundle_payload.uids += payload.uids
+        return bundle_payload
+
+    @staticmethod
+    def _bundle_get_rows_mapping_predicate(entry: OrmLabelRow) -> str:
+        return entry["label_hash"]
+
+    @staticmethod
+    def _bundle_create_rows_mapping_predicate(entry: OrmLabelRow) -> str:
+        return entry["data_hash"]
 
     def from_labels_dict(self, label_row_dict: dict) -> None:
         """
         If you have a label row dictionary in the same format that the Encord servers produce, you can initialise the
         LabelRow from that directly. In most cases you should prefer using the `initialise_labels` method.
 
         This function also initialises the label row.
@@ -1119,23 +1214,44 @@
         """
         self._check_labelling_is_initalised()
 
         if self.data_type not in (DataType.IMAGE, DataType.IMG_GROUP):
             raise LabelRowError("This function is only supported for label rows of image or image group data types.")
         return self._label_row_read_only_data.image_hash_to_frame[image_hash]
 
-    def save(self):
+    def save(self, bundle: Bundle = None) -> None:
         """
         Upload the created labels with the Encord server. This will overwrite any labels that someone has created
         in the platform in the meantime.
+
+        Args:
+            bundle: if not passed, save is executed immediately. If passed, it is executed as a part of the bundle
         """
         self._check_labelling_is_initalised()
 
         dict_labels = self.to_encord_dict()
-        self._project_client.save_label_row(uid=self.label_hash, label=dict_labels)
+
+        if bundle is None:
+            self._project_client.save_label_row(uid=self.label_hash, label=dict_labels)
+        else:
+            bundle.add(
+                operation=self._project_client.save_label_rows,
+                request_reducer=self._batch_save_rows_reducer,
+                result_mapper=None,
+                payload=BundledSaveRowsPayload(uids=[self.label_hash], payload=[dict_labels]),
+                limit=LABEL_ROW_BUNDLE_SAVE_LIMIT,
+            )
+
+    @staticmethod
+    def _batch_save_rows_reducer(
+        bundle_payload: BundledSaveRowsPayload, payload: BundledSaveRowsPayload
+    ) -> BundledSaveRowsPayload:
+        bundle_payload.uids += payload.uids
+        bundle_payload.payload += payload.payload
+        return bundle_payload
 
     def get_frame_view(self, frame: Union[int, str] = 0) -> FrameView:
         """
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
                 Defaults to the first frame.
         """
@@ -2157,15 +2273,15 @@
             If the attribute is static, then the answer value is returned, assuming an answer value has already been
             set. If the attribute is dynamic, the AnswersForFrames object is returned.
         """
         if attribute is None:
             attribute = self._ontology_object.attributes[0]
         elif not self._is_attribute_valid_child_of_object_instance(attribute):
             raise LabelRowError("The attribute is not a valid child of the classification.")
-        elif not self._is_selectable_child_attribute(attribute):
+        elif not attribute.dynamic and not self._is_selectable_child_attribute(attribute):
             return None
 
         if is_dynamic is not None and is_dynamic is not attribute.dynamic:
             raise LabelRowError(
                 f"The attribute is {'dynamic' if attribute.dynamic else 'static'}, but is_dynamic is set to "
                 f"{is_dynamic}."
             )
@@ -2206,15 +2322,15 @@
             overwrite: If `True`, the answer will be overwritten if it already exists. If `False`, this will throw
                 a LabelRowError if the answer already exists. This argument is ignored for dynamic attributes.
         """
         if attribute is None:
             attribute = _infer_attribute_from_answer(self._ontology_object.attributes, answer)
         if not self._is_attribute_valid_child_of_object_instance(attribute):
             raise LabelRowError("The attribute is not a valid child of the object.")
-        elif not self._is_selectable_child_attribute(attribute):
+        elif not attribute.dynamic and not self._is_selectable_child_attribute(attribute):
             raise LabelRowError(
                 "Setting a nested attribute is only possible if all parent attributes have been selected."
             )
         elif frames is not None and attribute.dynamic is False:
             raise LabelRowError("Setting frames is only possible for dynamic attributes.")
 
         if attribute.dynamic:
@@ -2539,15 +2655,15 @@
 
         def _get_object_frame_instance_data(self) -> ObjectInstance.FrameData:
             return self._object_instance._frames_to_instance_data[self._frame]
 
         def _check_if_frame_view_is_valid(self) -> None:
             if self._frame not in self._object_instance._frames_to_instance_data:
                 raise LabelRowError(
-                    "Tryinannotation to use an ObjectInstance.Annotation for an ObjectInstance that is not on the frameAnnotation"
+                    "Trying to use an ObjectInstance.Annotation for an ObjectInstance that is not on the frame"
                 )
 
     @dataclass
     class FrameInfo:
         created_at: datetime = field(default_factory=datetime.now)
         created_by: Optional[str] = None
         """None defaults to the user of the SDK once uploaded to the server."""
@@ -2649,14 +2765,17 @@
         is_dynamic_child = self._dynamic_answer_manager.is_valid_dynamic_attribute(attribute)
         return is_dynamic_child or is_static_child
 
     def _is_selectable_child_attribute(self, attribute: Attribute) -> bool:
         # I have the ontology classification, so I can build the tree from that. Basically do a DFS.
         ontology_object = self._ontology_object
         for search_attribute in ontology_object.attributes:
+            if search_attribute.dynamic:
+                continue
+
             if _search_child_attributes(attribute, search_attribute, self._static_answer_map):
                 return True
         return False
 
     def _get_all_static_answers(self) -> List[Answer]:
         return list(self._static_answer_map.values())
```

### Comparing `encord-0.1.75/encord/objects/project.py` & `encord-0.1.76/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/objects/utils.py` & `encord-0.1.76/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/ontology.py` & `encord-0.1.76/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/api_key.py` & `encord-0.1.76/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/base_orm.py` & `encord-0.1.76/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/dataset.py` & `encord-0.1.76/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/dataset_with_user_role.py` & `encord-0.1.76/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/label_log.py` & `encord-0.1.76/encord/orm/label_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     annotation_hash: str  # Legacy value. Replaced by identifier.
     identifier: str
     data_hash: str
     feature_hash: str
     action: Action
     label_name: str
     time_taken: int
-    created_at: datetime.datetime
+    created_at: datetime
     frame: int
 
 
 class Action(IntEnum):
     ADD = 0
     EDIT = 1
     DELETE = 2
```

### Comparing `encord-0.1.75/encord/orm/label_row.py` & `encord-0.1.76/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/labeling_algorithm.py` & `encord-0.1.76/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/model.py` & `encord-0.1.76/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/ontology.py` & `encord-0.1.76/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/project.py` & `encord-0.1.76/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/project_api_key.py` & `encord-0.1.76/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/project_with_user_role.py` & `encord-0.1.76/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/orm/test/test_dataset.py` & `encord-0.1.76/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/project.py` & `encord-0.1.76/encord/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from encord.orm.project import CopyDatasetOptions, CopyLabelsOptions
 from encord.orm.project import Project as OrmProject
 from encord.project_ontology.classification_type import ClassificationType
 from encord.project_ontology.object_type import ObjectShape
 from encord.project_ontology.ontology import Ontology as LegacyOntology
 from encord.utilities.project_user import ProjectUser, ProjectUserRole
 from encord.ontology import Ontology
+from encord.http.bundle import Bundle
 
 
 class Project:
     """
     Access project related data and manipulate the project.
     """
 
@@ -938,7 +939,15 @@
     def _get_project_instance(self):
         if self._project_instance is None:
             self._project_instance = self.get_project()
         return self._project_instance
 
     def _invalidate_project_instance(self):
         self._project_instance = None
+
+    def create_bundle(self) -> Bundle:
+        """
+        Initialises a bundle to reduce amount of network calls performed by the Encord SDK
+
+        See the :class:`encord.http.bundle.Bundle` documentation for more details
+        """
+        return Bundle()
```

### Comparing `encord-0.1.75/encord/project_ontology/classification_attribute.py` & `encord-0.1.76/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/project_ontology/classification_option.py` & `encord-0.1.76/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/project_ontology/ontology.py` & `encord-0.1.76/encord/project_ontology/ontology.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         "#194D33",
         "#0C797D",
         "#0062B1",
         "#653294",
         "#AB149E",
     )
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.ontology_objects: List[OntologyObject] = []
         self.ontology_classifications: List[OntologyClassification] = []
         self.color_index = 0
 
     def __str__(self):
         return str(self.to_dict())
 
@@ -214,39 +214,46 @@
             "id": ontology_object.id,
             "color": ontology_object.color,
             "name": ontology_object.name,
             "shape": ontology_object.shape.value,
             "featureNodeHash": ontology_object.feature_node_hash,
         }
 
+    def __ontology_classification_options_to_dict(
+        self, options: Optional[Iterable[ClassificationOption]]
+    ) -> Optional[List[Dict]]:
+        if options is None:
+            return None
+
+        option_dicts = []
+        for classification_option in options:
+            option = {
+                "id": classification_option.id,
+                "label": classification_option.label,
+                "value": classification_option.value,
+                "featureNodeHash": classification_option.feature_node_hash,
+            }
+            option_dicts.append(option)
+        return option_dicts
+
     def ontology_classification_to_dict(self, ontology_classification: OntologyClassification) -> Dict:
-        classification = {
-            "id": ontology_classification.id,
-            "featureNodeHash": ontology_classification.feature_node_hash,
-        }
         attributes = []
         for classification_attribute in ontology_classification.attributes:
             attribute = {
                 "id": classification_attribute.id,
                 "name": classification_attribute.name,
                 "type": classification_attribute.classification_type.value,
                 "required": classification_attribute.required,
                 "featureNodeHash": classification_attribute.feature_node_hash,
+                "options": self.__ontology_classification_options_to_dict(classification_attribute.options),
             }
-            if classification_attribute.options:
-                options = []
-                for classification_option in classification_attribute.options:
-                    option = {
-                        "id": classification_option.id,
-                        "label": classification_option.label,
-                        "value": classification_option.value,
-                        "featureNodeHash": classification_option.feature_node_hash,
-                    }
-                    options.append(option)
-                attribute["options"] = options
             attributes.append(attribute)
 
-        classification["attributes"] = attributes
+        classification = {
+            "id": ontology_classification.id,
+            "featureNodeHash": ontology_classification.feature_node_hash,
+            "attributes": attributes,
+        }
         return classification
 
     def __format_option_value(self, label: str):
         return label.replace(" ", "_")
```

### Comparing `encord-0.1.75/encord/project_ontology/ontology_classification.py` & `encord-0.1.76/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/project_ontology/ontology_object.py` & `encord-0.1.76/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/user_client.py` & `encord-0.1.76/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import base64
-import datetime
+from datetime import datetime
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import dateutil
 
@@ -234,15 +234,15 @@
             {"dataset": DatasetInfo(**convert_dates(d.dataset)), "user_role": DatasetUserRole(d.user_role)}
             for d in data
         ]
 
     @staticmethod
     def create_with_ssh_private_key(
         ssh_private_key: Optional[str] = None,
-        password: str = None,
+        password: Optional[str] = None,
         requests_settings: RequestsSettings = DEFAULT_REQUESTS_SETTINGS,
         **kwargs,
     ) -> EncordUserClient:
         if not ssh_private_key:
             ssh_private_key = get_env_ssh_key()
 
         user_config = UserConfig.from_ssh_private_key(
@@ -561,15 +561,17 @@
                 {
                     "ontology": Ontology(querier, config, ontology),
                     "user_role": OntologyUserRole(row.user_role),
                 }
             )
         return retval
 
-    def create_ontology(self, title: str, description: str = "", structure: OntologyStructure = None) -> Ontology:
+    def create_ontology(
+        self, title: str, description: str = "", structure: Optional[OntologyStructure] = None
+    ) -> Ontology:
         structure_dict = structure.to_dict() if structure else dict()
         ontology = {
             "title": title,
             "description": description,
             "editor": structure_dict,
         }
 
@@ -600,15 +602,15 @@
                     continue
             elif not isinstance(clause, ListingFilter):
                 continue
 
             if clause.value.endswith("before") or clause.value.endswith("after"):
                 if isinstance(val, str):
                     val = dateutil.parser.isoparse(val)
-                if isinstance(val, datetime.datetime):
+                if isinstance(val, datetime):
                     val = val.isoformat()
                 else:
                     raise ValueError(f"Value for {clause.name} filter should be a datetime")
 
             ret[clause.value] = val
 
         return ret
```

### Comparing `encord-0.1.75/encord/utilities/client_utilities.py` & `encord-0.1.76/encord/utilities/client_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from datetime import datetime
 import pprint
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, Optional, Set, TypeVar, Union
 
-import dateutil
+from dateutil import parser as datetime_parser
 
 
 def pretty_print(data):
     return pprint.pformat(data, indent=4, width=10)
 
 
 class APIKeyScopes(Enum):
@@ -116,19 +116,19 @@
 
 @dataclass
 class CvatImporterError:
     dataset_hash: str
     issues: Issues
 
 
-def parse_datetime(key: str, val: Union[str, datetime]) -> str:
+def parse_datetime(key: str, val: Optional[Union[str, datetime]]) -> Optional[str]:
     if not val:
         return None
     if isinstance(val, str):
-        return dateutil.parser.isoparse(val).isoformat()
+        return datetime_parser.isoparse(val).isoformat()
     if isinstance(val, datetime):
         return val.isoformat()
     else:
         raise ValueError(f"Value for {key} should be a datetime")
 
 
 T = TypeVar("T")
```

### Comparing `encord-0.1.75/encord/utilities/label_utilities.py` & `encord-0.1.76/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/encord/utilities/project_user.py` & `encord-0.1.76/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.75/pyproject.toml` & `encord-0.1.76/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.75"
+version = "0.1.76"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -37,15 +37,15 @@
 sphinx-toolbox = "^3.4.0"
 prettyprinter = "0.18.0"
 isort = "^5.10.1"
 pydata-sphinx-theme = "^0.8.1"
 Pillow = "^9.1.0"
 sphinx-gallery = "^0.10.1"
 deepdiff = "^6.2.1"
-
+types-requests = "^2.25.0"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `encord-0.1.75/setup.py` & `encord-0.1.76/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'tqdm>=4.32.1,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'encord',
-    'version': '0.1.75',
+    'version': '0.1.76',
     'description': 'Encord Python SDK Client',
     'long_description': '<h1 align="center">\n  <p align="center">Encord Python API Client</p>\n  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>\n</h1>\n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer vision***\n\n## 💻 Features\n\n- Minimal low-level Python client that allows you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`\n\n## ✨ Relevant Links\n* [Encord website](https://encord.com)\n* [Encord web app](https://app.encord.com)\n* [Encord documentation](https://docs.encord.com)\n\n## 💡 Getting Started\n\nFor full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).\n\nFirst, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:\n\n```bash\npip install encord\n```\n\nThen, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.\n\n```bash\nexport ENCORD_PROJECT_ID="<project_id>"\nexport ENCORD_API_KEY="<project_api_key>"\n```\n\nPassing the resource ID and API key as environment variables, you can initialise the Encord client directly.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\n```\n\nIf you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.\n\n```python\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise("<resource_id>", "<resource_api_key>")\n```\n\nIf you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.\n\n```py\nfrom encord.client import EncordClient\nfrom encord.client import EncordConfig\n\nconfig = EncordConfig("<resource_id>", "<resource_api_key>")\nclient = EncordClient.initialise_with_config(config)\n```\n\nOnce you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.\n\n```py\nfrom encord.client import EncordClient\n\nclient = EncordClient.initialise()\nproject = client.get_project()\n```\n\n## 🐛 Troubleshooting\n\nPlease report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.\n',
     'author': 'Cord Technologies Limited',
     'author_email': 'hello@encord.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/encord-team/encord-client-python',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['cord',
 'encord', 'encord.constants', 'encord.constants.test', 'encord.http',
 'encord.objects', 'encord.orm', 'encord.orm.test', 'encord.project_ontology',
 'encord.utilities'] package_data = \ {'': ['*']} install_requires = \
 ['cryptography>=3.4.8,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0',
 'requests>=2.25.0,<3.0.0', 'tqdm>=4.32.1,<5.0.0'] extras_require = \ {':
 python_version < "3.8"': ['importlib_metadata>=6.1.0,<7.0.0']} setup_kwargs =
-{ 'name': 'encord', 'version': '0.1.75', 'description': 'Encord Python SDK
+{ 'name': 'encord', 'version': '0.1.76', 'description': 'Encord Python SDK
 Client', 'long_description': '
            ****** \nEncord Python API Client\n [Cord_logo]\n ******
 \n\n[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]
 (https://opensource.org/licenses/Apache-2.0)\n\n***The data engine for computer
 vision***\n\n## ð» Features\n\n- Minimal low-level Python client that allows
 you to interact with Encord\'s API\n- Supports Python: `3.7`, `3.8`, `3.9`, and
 `3.10`\n\n## â¨ Relevant Links\n* [Encord website](https://encord.com)\n*
```

### Comparing `encord-0.1.75/PKG-INFO` & `encord-0.1.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.75
+Version: 0.1.76
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.75 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.76 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

