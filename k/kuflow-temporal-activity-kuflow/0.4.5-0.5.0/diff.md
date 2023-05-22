# Comparing `tmp/kuflow_temporal_activity_kuflow-0.4.5.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-0.4.5.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-0.5.0.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-0.4.5.tar` & `kuflow_temporal_activity_kuflow-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      878 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/README.md
--rw-r--r--   0        0        0        6 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/VERSION
--rw-r--r--   0        0        0     1320 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     2696 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0      849 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
--rw-r--r--   0        0        0    11009 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
--rw-r--r--   0        0        0     3391 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0    13208 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     7215 2023-05-15 11:39:40.707021 kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/validation.py
--rw-r--r--   0        0        0      838 2023-05-15 11:41:11.594938 kuflow_temporal_activity_kuflow-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.5/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/README.md
+-rw-r--r--   0        0        0        6 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/VERSION
+-rw-r--r--   0        0        0     1320 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     3817 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0     1970 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
+-rw-r--r--   0        0        0    12934 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
+-rw-r--r--   0        0        0     3553 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0    22166 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     8623 2023-05-22 09:05:44.091853 kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/validation.py
+-rw-r--r--   0        0        0     1037 2023-05-22 09:07:38.734449 kuflow_temporal_activity_kuflow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.5.0/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.5.0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/README.md` & `kuflow_temporal_activity_kuflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .kuflow_async_activities import KuFlowAsyncActivities
 from .kuflow_sync_activities import KuFlowSyncActivities
 
 __all__ = ["KuFlowAsyncActivities", "KuFlowSyncActivities"]
-__version__ = "0.4.5"
+__version__ = "0.5.0"
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py` & `kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,38 @@
+# coding=utf-8
+#
+# MIT License
+#
+# Copyright (c) 2022 KuFlow
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+
 from temporalio import activity
 
 from kuflow_rest import KuFlowRestClient, models
-from kuflow_temporal_activity_kuflow import validation
 from kuflow_temporal_common import exceptions
 
-from . import models as models_temporal
+from . import models as models_temporal, validation
 
 
 class KuFlowSyncActivities:
     def __init__(self, kuflow_client: KuFlowRestClient) -> None:
         self._kuflow_client = kuflow_client
         self.activities = [
             self.retrieve_principal,
@@ -34,252 +58,267 @@
     async def retrieve_principal(
         self,
         request: models_temporal.RetrievePrincipalRequest,
     ) -> models_temporal.RetrievePrincipalResponse:
         try:
             validation.validate_retrieve_principal_request(request)
 
-            principal = self._kuflow_client.principal.retrieve_principal(id=request.principalId)
+            principal = self._kuflow_client.principal.retrieve_principal(id=request.principal_id)
 
             return models_temporal.RetrievePrincipalResponse(principal=principal)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def find_processes(
         self,
         request: models_temporal.FindProcessesRequest,
     ) -> models_temporal.FindProcessesResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
-            procesPage = self._kuflow_client.process.find_processes(**non_none_props)
+            proces_page = self._kuflow_client.process.find_processes(**non_none_props)
 
-            return models_temporal.FindProcessesResponse(processes=procesPage)
+            return models_temporal.FindProcessesResponse(processes=proces_page)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def retrieve_process(
         self,
         request: models_temporal.RetrieveProcessRequest,
     ) -> models_temporal.RetrieveProcessResponse:
         try:
             validation.validate_retrieve_process_request(request)
 
-            process = self._kuflow_client.process.retrieve_process(id=request.processId)
+            process = self._kuflow_client.process.retrieve_process(id=request.process_id)
 
             return models_temporal.RetrieveProcessResponse(process=process)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def save_process_element(
         self,
         request: models_temporal.SaveProcessElementRequest,
     ) -> models_temporal.SaveProcessElementResponse:
         try:
             validation.validate_save_process_element_request(request)
 
             command = models.ProcessSaveElementCommand(
-                element_definition_code=request.elementDefinitionCode, element_values=request.elementValues
+                element_definition_code=request.element_definition_code, element_values=request.element_values
             )
-            process = self._kuflow_client.process.actions_process_save_element(id=request.processId, command=command)
+            process = self._kuflow_client.process.actions_process_save_element(id=request.process_id, command=command)
 
             return models_temporal.SaveProcessElementResponse(process=process)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def delete_process_element(
         self,
         request: models_temporal.DeleteProcessElementRequest,
     ) -> models_temporal.DeleteProcessElementResponse:
         try:
             validation.validate_delete_process_element_request(request)
 
-            command = models.ProcessDeleteElementCommand(element_definition_code=request.elementDefinitionCode)
+            command = models.ProcessDeleteElementCommand(element_definition_code=request.element_definition_code)
 
-            process = self._kuflow_client.process.actions_process_delete_element(id=request.processId, command=command)
+            process = self._kuflow_client.process.actions_process_delete_element(id=request.process_id, command=command)
 
             return models_temporal.DeleteProcessElementResponse(process=process)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def complete_process(
         self,
         request: models_temporal.CompleteProcessRequest,
     ) -> models_temporal.CompleteProcessResponse:
         try:
             validation.validate_complete_process_request(request)
 
-            process = self._kuflow_client.process.actions_process_complete(request.processId)
+            process = self._kuflow_client.process.actions_process_complete(request.process_id)
 
             return models_temporal.CompleteProcessResponse(process=process)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def change_process_initiator(
         self,
         request: models_temporal.ChangeProcessInitiatorRequest,
     ) -> models_temporal.ChangeProcessInitiatorResponse:
         try:
             validation.validate_change_process_initiator_request(request)
 
-            command = models.ProcessChangeInitiatorCommand(email=request.email, principal_id=request.principalId)
+            command = models.ProcessChangeInitiatorCommand(email=request.email, principal_id=request.principal_id)
             process = self._kuflow_client.process.actions_process_change_initiator(
-                id=request.processId, command=command
+                id=request.process_id, command=command
             )
 
             return models_temporal.ChangeProcessInitiatorResponse(process=process)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def find_tasks(
         self,
         request: models_temporal.FindTaskRequest,
     ) -> models_temporal.FindTaskResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
-            taskPage = self._kuflow_client.task.find_tasks(**non_none_props)
+            task_page = self._kuflow_client.task.find_tasks(**non_none_props)
 
-            return models_temporal.FindTaskResponse(tasks=taskPage)
+            return models_temporal.FindTaskResponse(tasks=task_page)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def retrieve_task(
         self,
         request: models_temporal.RetrieveTaskRequest,
     ) -> models_temporal.RetrieveTaskResponse:
         try:
             validation.validate_retrieve_task_request(request)
 
-            task = self._kuflow_client.task.retrieve_task(id=request.taskId)
+            task = self._kuflow_client.task.retrieve_task(id=request.task_id)
 
             return models_temporal.RetrieveTaskResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def create_task(
         self,
         request: models_temporal.CreateTaskRequest,
     ) -> models_temporal.CreateTaskResponse:
         try:
             validation.validate_create_task_request(request)
 
             task = self._kuflow_client.task.create_task(task=request.task)
 
             return models_temporal.CreateTaskResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def complete_task(
         self,
         request: models_temporal.CompleteTaskRequest,
     ) -> models_temporal.CompleteTaskResponse:
         try:
             validation.validate_complete_task_request(request)
 
-            task = self._kuflow_client.task.actions_task_complete(id=request.taskId)
+            task = self._kuflow_client.task.actions_task_complete(id=request.task_id)
 
             return models_temporal.CompleteTaskResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def claim_task(
         self,
         request: models_temporal.ClaimTaskRequest,
-    ) -> models_temporal.CompleteTaskResponse:
+    ) -> models_temporal.ClaimTaskResponse:
         try:
             validation.validate_claim_task_request(request)
 
-            task = self._kuflow_client.task.actions_task_claim(id=request.taskId)
+            task = self._kuflow_client.task.actions_task_claim(id=request.task_id)
 
             return models_temporal.ClaimTaskResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def assign_task(
         self,
         request: models_temporal.AssignTaskRequest,
     ) -> models_temporal.AssignTaskResponse:
         try:
             validation.validate_assign_task_request(request)
 
-            command = models.TaskAssignCommand(email=request.email, principal_id=request.principalId)
-            task = self._kuflow_client.task.actions_task_assign(id=request.taskId, command=command)
+            command = models.TaskAssignCommand(email=request.email, principal_id=request.principal_id)
+            task = self._kuflow_client.task.actions_task_assign(id=request.task_id, command=command)
 
             return models_temporal.AssignTaskResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def save_task_element(
         self,
         request: models_temporal.SaveTaskElementRequest,
     ) -> models_temporal.SaveTaskElementResponse:
         try:
             validation.validate_save_task_element_request(request)
 
             command = models.TaskSaveElementCommand(
-                element_definition_code=request.elementDefinitionCode, element_values=request.elementValues
+                element_definition_code=request.element_definition_code, element_values=request.element_values
             )
-            task = self._kuflow_client.task.actions_task_save_element(id=request.taskId, command=command)
+            task = self._kuflow_client.task.actions_task_save_element(id=request.task_id, command=command)
 
             return models_temporal.SaveTaskElementResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def delete_task_element(
         self,
         request: models_temporal.DeleteTaskElementRequest,
     ) -> models_temporal.DeleteTaskElementResponse:
         try:
             validation.validate_delete_task_element_request(request)
 
-            command = models.TaskDeleteElementCommand(element_definition_code=request.elementDefinitionCode)
-            task = self._kuflow_client.task.actions_task_delete_element(id=request.taskId, command=command)
+            command = models.TaskDeleteElementCommand(element_definition_code=request.element_definition_code)
+            task = self._kuflow_client.task.actions_task_delete_element(id=request.task_id, command=command)
 
             return models_temporal.DeleteTaskElementResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def delete_task_element_value_document(
         self,
         request: models_temporal.DeleteTaskElementValueDocumentRequest,
     ) -> models_temporal.DeleteTaskElementValueDocumentResponse:
         try:
             validation.validate_delete_task_element_value_document_request(request)
 
-            command = models.TaskDeleteElementValueDocumentCommand(document_id=request.documentId)
+            command = models.TaskDeleteElementValueDocumentCommand(document_id=request.document_id)
             task = self._kuflow_client.task.actions_task_delete_element_value_document(
-                id=request.taskId, command=command
+                id=request.task_id, command=command
             )
 
             return models_temporal.DeleteTaskElementValueDocumentResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
+
+    @activity.defn
+    async def save_task_json_forms_value_data(
+        self,
+        request: models_temporal.SaveTaskJsonFormsValueDataRequest,
+    ) -> models_temporal.SaveTaskJsonFormsValueDataResponse:
+        try:
+            validation.validate_save_task_json_forms_value_data(request)
+
+            command = models.TaskSaveJsonFormsValueDataCommand(data=request.data)
+            task = self._kuflow_client.task.actions_task_save_json_forms_value_data(id=request.task_id, command=command)
+
+            return models_temporal.SaveTaskJsonFormsValueDataResponse(task=task)
+        except Exception as err:
+            raise exceptions.create_application_error(err) from err
 
     @activity.defn
     async def append_task_log(
         self,
         request: models_temporal.AppendTaskLogRequest,
     ) -> models_temporal.AppendTaskLogResponse:
         try:
             validation.validate_append_task_log_request(request)
 
-            task = self._kuflow_client.task.actions_task_append_log(id=request.taskId, log=request.log)
+            task = self._kuflow_client.task.actions_task_append_log(id=request.task_id, log=request.log)
 
             return models_temporal.AppendTaskLogResponse(task=task)
         except Exception as err:
-            return exceptions.create_application_error(err)
+            raise exceptions.create_application_error(err) from err
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     RetrievePrincipalResponse,
     RetrieveProcessRequest,
     RetrieveProcessResponse,
     RetrieveTaskRequest,
     RetrieveTaskResponse,
     SaveProcessElementRequest,
     SaveProcessElementResponse,
+    SaveTaskJsonFormsValueDataRequest,
+    SaveTaskJsonFormsValueDataResponse,
     SaveTaskElementRequest,
     SaveTaskElementResponse,
     UserActionWorkflowRequest,
     UserActionWorkflowResponse,
     WorkflowRequest,
     WorkflowResponse,
 )
@@ -93,14 +95,16 @@
     "RetrievePrincipalResponse",
     "RetrieveProcessRequest",
     "RetrieveProcessResponse",
     "RetrieveTaskRequest",
     "RetrieveTaskResponse",
     "SaveProcessElementRequest",
     "SaveProcessElementResponse",
+    "SaveTaskJsonFormsValueDataRequest",
+    "SaveTaskJsonFormsValueDataResponse",
     "SaveTaskElementRequest",
     "SaveTaskElementResponse",
     "UserActionWorkflowRequest",
     "UserActionWorkflowResponse",
     "WorkflowRequest",
     "WorkflowResponse",
 ]
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/kuflow_temporal_activity_kuflow/validation.py` & `kuflow_temporal_activity_kuflow-0.5.0/kuflow_temporal_activity_kuflow/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,217 +1,256 @@
+# coding=utf-8
+#
+# MIT License
+#
+# Copyright (c) 2022 KuFlow
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+#
+
 from temporalio.exceptions import ApplicationError
 
 from kuflow_temporal_common.exceptions import KuFlowFailureType
 
-from .models import _models as models_temporal
+from . import models as models_temporal
 
 
 def validate_retrieve_principal_request(
     request: models_temporal.RetrievePrincipalRequest,
 ) -> None:
-    if not request.principalId:
+    if not request.principal_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_retrieve_process_request(
     request: models_temporal.RetrieveProcessRequest,
 ) -> None:
-    if not request.processId:
+    if not request.process_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_save_process_element_request(
     request: models_temporal.SaveProcessElementRequest,
 ) -> None:
-    if not request.processId:
+    if not request.process_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.elementDefinitionCode:
+    if not request.element_definition_code:
         raise ApplicationError(
-            message="'elementDefinitionCode' is required",
-            non_retryable=True,
+            "'elementDefinitionCode' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_delete_process_element_request(
     request: models_temporal.DeleteProcessElementRequest,
 ) -> None:
-    if not request.processId:
+    if not request.process_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.elementDefinitionCode:
+    if not request.element_definition_code:
         raise ApplicationError(
-            message="'elementDefinitionCode' is required",
-            non_retryable=True,
+            "'elementDefinitionCode' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_complete_process_request(
     request: models_temporal.CompleteProcessRequest,
 ) -> None:
-    if not request.processId:
+    if not request.process_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_change_process_initiator_request(
     request: models_temporal.ChangeProcessInitiatorRequest,
 ) -> None:
-    if not request.processId:
+    if not request.process_id:
         raise ApplicationError(
-            message="'processId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'processId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.email and not request.principalId:
+    if not request.email and not request.principal_id:
         raise ApplicationError(
-            message="'email' or 'principalId' is required",
-            non_retryable=True,
+            "'email' or 'principalId' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_retrieve_task_request(
     request: models_temporal.RetrieveTaskRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_create_task_request(
     request: models_temporal.CreateTaskRequest,
 ) -> None:
     if not request.task.id:
         raise ApplicationError(
-            message="'task.id' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'task.id' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
     if not request.task.process_id:
         raise ApplicationError(
-            message="'task.process_id' is required",
-            non_retryable=True,
-            type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            "'task.process_id' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
     if not request.task.task_definition.code:
         raise ApplicationError(
-            message="'task.taskDefinition.code' is required",
-            non_retryable=True,
+            "'task.taskDefinition.code' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_complete_task_request(
     request: models_temporal.CompleteTaskRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_claim_task_request(
     request: models_temporal.ClaimTaskRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
 
 def validate_assign_task_request(
     request: models_temporal.AssignTaskRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.email and not request.principalId:
+    if not request.email and not request.principal_id:
         raise ApplicationError(
-            message="'email' or 'principalId' is required",
-            non_retryable=True,
+            "'email' or 'principalId' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_save_task_element_request(
     request: models_temporal.SaveTaskElementRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.elementDefinitionCode:
+    if not request.element_definition_code:
         raise ApplicationError(
-            message="'elementDefinitionCode' is required",
-            non_retryable=True,
+            "'elementDefinitionCode' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_delete_task_element_request(
     request: models_temporal.DeleteTaskElementRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.elementDefinitionCode:
+    if not request.element_definition_code:
         raise ApplicationError(
-            message="'elementDefinitionCode' is required",
-            non_retryable=True,
+            "'elementDefinitionCode' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_delete_task_element_value_document_request(
     request: models_temporal.DeleteTaskElementValueDocumentRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
-    if not request.documentId:
+    if not request.document_id:
         raise ApplicationError(
-            message="'documentId' is required",
+            "'documentId' is required",
+            type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
             non_retryable=True,
+        )
+
+
+def validate_save_task_json_forms_value_data(
+    request: models_temporal.SaveTaskJsonFormsValueDataRequest,
+) -> None:
+    if not request.task_id:
+        raise ApplicationError(
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
+        )
+
+    if not request.data:
+        raise ApplicationError(
+            "'data' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
 
 def validate_append_task_log_request(
     request: models_temporal.AppendTaskLogRequest,
 ) -> None:
-    if not request.taskId:
+    if not request.task_id:
         raise ApplicationError(
-            message="'taskId' is required", non_retryable=True, type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE
+            "'taskId' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
 
     if not request.log.level:
         raise ApplicationError(
-            message="'log.level' is required",
-            non_retryable=True,
+            "'log.level' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
 
     if not request.log.message:
         raise ApplicationError(
-            message="'log.message' is required",
-            non_retryable=True,
+            "'log.message' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
         )
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/setup.py` & `kuflow_temporal_activity_kuflow-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kuflow_temporal_activity_kuflow', 'kuflow_temporal_activity_kuflow.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.4.5,<0.5.0']
+['kuflow-temporal-common>=0.5.0,<0.6.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-0.4.5/PKG-INFO` & `kuflow_temporal_activity_kuflow-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 0.4.5
+Version: 0.5.0
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.4.5,<0.5.0)
+Requires-Dist: kuflow-temporal-common (>=0.5.0,<0.6.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

