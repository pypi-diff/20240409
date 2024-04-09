# Comparing `tmp/kuflow_temporal_activity_kuflow-1.4.0.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-1.4.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-1.5.0.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-1.4.0.tar` & `kuflow_temporal_activity_kuflow-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      878 2024-03-15 12:57:18.583490 kuflow_temporal_activity_kuflow-1.4.0/README.md
--rw-r--r--   0        0        0        6 2024-03-15 12:57:18.583490 kuflow_temporal_activity_kuflow-1.4.0/VERSION
--rw-r--r--   0        0        0     1325 2024-03-15 12:57:18.583490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     8652 2024-03-15 12:57:18.583490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/_validation.py
--rw-r--r--   0        0        0     4932 2024-03-15 12:57:18.583490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0    15540 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/kuflow_activities.py
--rw-r--r--   0        0        0     3661 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0     2036 2024-03-15 12:58:02.332013 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22581 2024-03-15 12:58:02.336013 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0    22070 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     1463 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__init__.py
--rw-r--r--   0        0        0      499 2024-03-15 12:58:02.384014 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10493 2024-03-15 12:58:02.384014 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    13245 2024-03-15 12:58:02.392014 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    14343 2024-03-15 12:58:02.392014 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
--rw-r--r--   0        0        0    11189 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
--rw-r--r--   0        0        0    14055 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
--rw-r--r--   0        0        0    15409 2024-03-15 12:57:18.587490 kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
--rw-r--r--   0        0        0      939 2024-03-15 12:58:24.452276 kuflow_temporal_activity_kuflow-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.4.0/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/README.md
+-rw-r--r--   0        0        0        6 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/VERSION
+-rw-r--r--   0        0        0     1325 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     9152 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/_validation.py
+-rw-r--r--   0        0        0     4932 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0    16373 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/kuflow_activities.py
+-rw-r--r--   0        0        0     3803 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0     2133 2024-04-09 11:50:16.973127 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    23527 2024-04-09 11:50:16.973127 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0    23017 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     1463 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-09 11:50:17.025128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10493 2024-04-09 11:50:17.025128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13245 2024-04-09 11:50:17.029128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14343 2024-04-09 11:50:17.029128 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    11189 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
+-rw-r--r--   0        0        0    14055 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
+-rw-r--r--   0        0        0    15409 2024-04-09 11:44:28.833042 kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
+-rw-r--r--   0        0        0      939 2024-04-09 11:50:39.177383 kuflow_temporal_activity_kuflow-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.0/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-1.5.0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/README.md` & `kuflow_temporal_activity_kuflow-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 
 from .kuflow_activities import KuFlowActivities
 
 
 KUFLOW_ENGINE_SIGNAL_COMPLETED_TASK = "KuFlow_Engine_Signal_Completed_Task"
 
 __all__ = ["KuFlowActivities", "KUFLOW_ENGINE_SIGNAL_COMPLETED_TASK"]
-__version__ = "1.4.0"
+__version__ = "1.5.0"
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/_validation.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,30 @@
         raise ApplicationError(
             "'element_definition_code' is required",
             type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
             non_retryable=True,
         )
 
 
+def validate_save_process_entity_request(
+    request: models_temporal.SaveProcessEntityDataRequest,
+) -> None:
+    if not request.process_id:
+        raise ApplicationError(
+            "'process_id' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
+        )
+
+    if not request.data:
+        raise ApplicationError(
+            "'data' is required",
+            type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE,
+            non_retryable=True,
+        )
+
+
 def validate_delete_process_element_request(
     request: models_temporal.DeleteProcessElementRequest,
 ) -> None:
     if not request.process_id:
         raise ApplicationError(
             "'process_id' is required", type=KuFlowFailureType.ACTIVITIES_VALIDATION_FAILURE, non_retryable=True
         )
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/kuflow_activities.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/kuflow_activities.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,32 @@
             )
             process = self._kuflow_client.process.actions_process_save_element(id=request.process_id, command=command)
 
             return models_temporal.SaveProcessElementResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
+    @activity.defn(name="KuFlow_Engine_saveProcessEntityData")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
+    async def save_process_entity_data(
+        self,
+        request: models_temporal.SaveProcessEntityDataRequest,
+    ) -> models_temporal.SaveProcessEntityDataResponse:
+        try:
+            validation.validate_save_process_entity_request(request)
+
+            command = models.ProcessSaveEntityDataCommand(data=request.data)
+            process = self._kuflow_client.process.actions_process_save_entity_data(
+                id=request.process_id, command=command
+            )
+
+            return models_temporal.SaveProcessEntityDataResponse(process=process)
+        except Exception as err:
+            raise exceptions.create_application_error(err) from err
+
     @activity.defn(name="KuFlow_Engine_deleteProcessElement")
     @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def delete_process_element(
         self,
         request: models_temporal.DeleteProcessElementRequest,
     ) -> models_temporal.DeleteProcessElementResponse:
         try:
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     RetrieveTaskResponse,
     RetrieveTenantUserRequest,
     RetrieveTenantUserResponse,
     RobotWorkflowRequest,
     RobotWorkflowResponse,
     SaveProcessElementRequest,
     SaveProcessElementResponse,
+    SaveProcessEntityDataRequest,
+    SaveProcessEntityDataResponse,
     SaveTaskElementRequest,
     SaveTaskElementResponse,
     SaveTaskJsonFormsValueDataRequest,
     SaveTaskJsonFormsValueDataResponse,
     UserActionWorkflowRequest,
     UserActionWorkflowResponse,
     WorkflowRequest,
@@ -87,28 +89,30 @@
     "DeleteTaskElementResponse",
     "DeleteTaskElementValueDocumentRequest",
     "DeleteTaskElementValueDocumentResponse",
     "FindProcessesRequest",
     "FindProcessesResponse",
     "FindTaskRequest",
     "FindTaskResponse",
-    "RetrieveTenantUserRequest",
-    "RetrieveTenantUserResponse",
     "RetrievePrincipalRequest",
     "RetrievePrincipalResponse",
     "RetrieveProcessRequest",
     "RetrieveProcessResponse",
     "RetrieveTaskRequest",
     "RetrieveTaskResponse",
+    "RetrieveTenantUserRequest",
+    "RetrieveTenantUserResponse",
     "RobotWorkflowRequest",
     "RobotWorkflowResponse",
     "SaveProcessElementRequest",
     "SaveProcessElementResponse",
-    "SaveTaskJsonFormsValueDataRequest",
-    "SaveTaskJsonFormsValueDataResponse",
+    "SaveProcessEntityDataRequest",
+    "SaveProcessEntityDataResponse",
     "SaveTaskElementRequest",
     "SaveTaskElementResponse",
+    "SaveTaskJsonFormsValueDataRequest",
+    "SaveTaskJsonFormsValueDataResponse",
     "UserActionWorkflowRequest",
     "UserActionWorkflowResponse",
     "WorkflowRequest",
     "WorkflowResponse",
 ]
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 15 12:57:18 2024 UTC, .py size: 3661 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,134 @@
-00000000: 550d 0d0a 0000 0000 ae45 f465 4d0e 0000  U........E.eM...
+00000000: 550d 0d0a 0000 0000 1c2a 1566 db0e 0000  U........*.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 002a 0000 0040 0000 0073 0c01 0000 6400  .*...@...s....d.
+00000020: 002c 0000 0040 0000 0073 1801 0000 6400  .,...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
 00000080: 6d14 5a14 6d15 5a15 6d16 5a16 6d17 5a17  m.Z.m.Z.m.Z.m.Z.
 00000090: 6d18 5a18 6d19 5a19 6d1a 5a1a 6d1b 5a1b  m.Z.m.Z.m.Z.m.Z.
 000000a0: 6d1c 5a1c 6d1d 5a1d 6d1e 5a1e 6d1f 5a1f  m.Z.m.Z.m.Z.m.Z.
 000000b0: 6d20 5a20 6d21 5a21 6d22 5a22 6d23 5a23  m Z m!Z!m"Z"m#Z#
 000000c0: 6d24 5a24 6d25 5a25 6d26 5a26 6d27 5a27  m$Z$m%Z%m&Z&m'Z'
-000000d0: 6d28 5a28 6d29 5a29 6d2a 5a2a 0100 6402  m(Z(m)Z)m*Z*..d.
-000000e0: 6403 6404 6405 6406 6407 6408 6409 640a  d.d.d.d.d.d.d.d.
-000000f0: 640b 640c 640d 640e 640f 6410 6411 6412  d.d.d.d.d.d.d.d.
-00000100: 6413 6414 6415 6416 6417 6418 6419 641a  d.d.d.d.d.d.d.d.
-00000110: 641b 641c 641d 641e 641f 6420 6421 6422  d.d.d.d.d.d d!d"
-00000120: 6423 6424 6425 6426 6427 6428 6429 642a  d#d$d%d&d'd(d)d*
-00000130: 642b 672a 5a2b 642c 5300 292d e901 0000  d+g*Z+d,S.)-....
-00000140: 0029 2ada 1441 7070 656e 6454 6173 6b4c  .)*..AppendTaskL
-00000150: 6f67 5265 7175 6573 74da 1541 7070 656e  ogRequest..Appen
-00000160: 6454 6173 6b4c 6f67 5265 7370 6f6e 7365  dTaskLogResponse
-00000170: da11 4173 7369 676e 5461 736b 5265 7175  ..AssignTaskRequ
-00000180: 6573 74da 1241 7373 6967 6e54 6173 6b52  est..AssignTaskR
-00000190: 6573 706f 6e73 65da 1d43 6861 6e67 6550  esponse..ChangeP
-000001a0: 726f 6365 7373 496e 6974 6961 746f 7252  rocessInitiatorR
-000001b0: 6571 7565 7374 da1e 4368 616e 6765 5072  equest..ChangePr
-000001c0: 6f63 6573 7349 6e69 7469 6174 6f72 5265  ocessInitiatorRe
-000001d0: 7370 6f6e 7365 da10 436c 6169 6d54 6173  sponse..ClaimTas
-000001e0: 6b52 6571 7565 7374 da11 436c 6169 6d54  kRequest..ClaimT
-000001f0: 6173 6b52 6573 706f 6e73 65da 1343 6f6d  askResponse..Com
-00000200: 706c 6574 6554 6173 6b52 6571 7565 7374  pleteTaskRequest
-00000210: da14 436f 6d70 6c65 7465 5461 736b 5265  ..CompleteTaskRe
-00000220: 7370 6f6e 7365 da11 4372 6561 7465 5461  sponse..CreateTa
-00000230: 736b 5265 7175 6573 74da 1243 7265 6174  skRequest..Creat
-00000240: 6554 6173 6b52 6573 706f 6e73 65da 1b44  eTaskResponse..D
-00000250: 656c 6574 6550 726f 6365 7373 456c 656d  eleteProcessElem
-00000260: 656e 7452 6571 7565 7374 da1c 4465 6c65  entRequest..Dele
-00000270: 7465 5072 6f63 6573 7345 6c65 6d65 6e74  teProcessElement
-00000280: 5265 7370 6f6e 7365 da18 4465 6c65 7465  Response..Delete
-00000290: 5461 736b 456c 656d 656e 7452 6571 7565  TaskElementReque
-000002a0: 7374 da19 4465 6c65 7465 5461 736b 456c  st..DeleteTaskEl
-000002b0: 656d 656e 7452 6573 706f 6e73 65da 2544  ementResponse.%D
-000002c0: 656c 6574 6554 6173 6b45 6c65 6d65 6e74  eleteTaskElement
-000002d0: 5661 6c75 6544 6f63 756d 656e 7452 6571  ValueDocumentReq
-000002e0: 7565 7374 da26 4465 6c65 7465 5461 736b  uest.&DeleteTask
-000002f0: 456c 656d 656e 7456 616c 7565 446f 6375  ElementValueDocu
-00000300: 6d65 6e74 5265 7370 6f6e 7365 da14 4669  mentResponse..Fi
-00000310: 6e64 5072 6f63 6573 7365 7352 6571 7565  ndProcessesReque
-00000320: 7374 da15 4669 6e64 5072 6f63 6573 7365  st..FindProcesse
-00000330: 7352 6573 706f 6e73 65da 0f46 696e 6454  sResponse..FindT
-00000340: 6173 6b52 6571 7565 7374 da10 4669 6e64  askRequest..Find
-00000350: 5461 736b 5265 7370 6f6e 7365 da18 5265  TaskResponse..Re
-00000360: 7472 6965 7665 5072 696e 6369 7061 6c52  trievePrincipalR
-00000370: 6571 7565 7374 da19 5265 7472 6965 7665  equest..Retrieve
-00000380: 5072 696e 6369 7061 6c52 6573 706f 6e73  PrincipalRespons
-00000390: 65da 1652 6574 7269 6576 6550 726f 6365  e..RetrieveProce
-000003a0: 7373 5265 7175 6573 74da 1752 6574 7269  ssRequest..Retri
-000003b0: 6576 6550 726f 6365 7373 5265 7370 6f6e  eveProcessRespon
-000003c0: 7365 da13 5265 7472 6965 7665 5461 736b  se..RetrieveTask
-000003d0: 5265 7175 6573 74da 1452 6574 7269 6576  Request..Retriev
-000003e0: 6554 6173 6b52 6573 706f 6e73 65da 1952  eTaskResponse..R
-000003f0: 6574 7269 6576 6554 656e 616e 7455 7365  etrieveTenantUse
-00000400: 7252 6571 7565 7374 da1a 5265 7472 6965  rRequest..Retrie
-00000410: 7665 5465 6e61 6e74 5573 6572 5265 7370  veTenantUserResp
-00000420: 6f6e 7365 da14 526f 626f 7457 6f72 6b66  onse..RobotWorkf
-00000430: 6c6f 7752 6571 7565 7374 da15 526f 626f  lowRequest..Robo
-00000440: 7457 6f72 6b66 6c6f 7752 6573 706f 6e73  tWorkflowRespons
-00000450: 65da 1953 6176 6550 726f 6365 7373 456c  e..SaveProcessEl
-00000460: 656d 656e 7452 6571 7565 7374 da1a 5361  ementRequest..Sa
-00000470: 7665 5072 6f63 6573 7345 6c65 6d65 6e74  veProcessElement
-00000480: 5265 7370 6f6e 7365 da16 5361 7665 5461  Response..SaveTa
-00000490: 736b 456c 656d 656e 7452 6571 7565 7374  skElementRequest
-000004a0: da17 5361 7665 5461 736b 456c 656d 656e  ..SaveTaskElemen
-000004b0: 7452 6573 706f 6e73 65da 2153 6176 6554  tResponse.!SaveT
-000004c0: 6173 6b4a 736f 6e46 6f72 6d73 5661 6c75  askJsonFormsValu
-000004d0: 6544 6174 6152 6571 7565 7374 da22 5361  eDataRequest."Sa
-000004e0: 7665 5461 736b 4a73 6f6e 466f 726d 7356  veTaskJsonFormsV
-000004f0: 616c 7565 4461 7461 5265 7370 6f6e 7365  alueDataResponse
-00000500: da19 5573 6572 4163 7469 6f6e 576f 726b  ..UserActionWork
-00000510: 666c 6f77 5265 7175 6573 74da 1a55 7365  flowRequest..Use
-00000520: 7241 6374 696f 6e57 6f72 6b66 6c6f 7752  rActionWorkflowR
-00000530: 6573 706f 6e73 65da 0f57 6f72 6b66 6c6f  esponse..Workflo
-00000540: 7752 6571 7565 7374 da10 576f 726b 666c  wRequest..Workfl
-00000550: 6f77 5265 7370 6f6e 7365 7202 0000 0072  owResponser....r
-00000560: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
-00000570: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00000580: 0000 720a 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00000590: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000005a0: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-000005b0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-000005c0: 0000 0072 1700 0000 721e 0000 0072 1f00  ...r....r....r..
-000005d0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000005e0: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-000005f0: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00000600: 2300 0000 7226 0000 0072 2700 0000 7224  #...r&...r'...r$
-00000610: 0000 0072 2500 0000 7228 0000 0072 2900  ...r%...r(...r).
-00000620: 0000 722a 0000 0072 2b00 0000 4e29 2cda  ..r*...r+...N),.
-00000630: 075f 6d6f 6465 6c73 7202 0000 0072 0300  ._modelsr....r..
-00000640: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00000650: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000660: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000670: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000680: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000690: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-000006a0: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-000006b0: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-000006c0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
-000006d0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
-000006e0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
-000006f0: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
-00000700: 722a 0000 0072 2b00 0000 da07 5f5f 616c  r*...r+.....__al
-00000710: 6c5f 5fa9 0072 2e00 0000 722e 0000 00fa  l__..r....r.....
-00000720: 6a2f 776f 726b 2f6b 7566 6c6f 772d 7364  j/work/kuflow-sd
-00000730: 6b2d 7079 7468 6f6e 2f6b 7566 6c6f 772d  k-python/kuflow-
-00000740: 7465 6d70 6f72 616c 2d61 6374 6976 6974  temporal-activit
-00000750: 792d 6b75 666c 6f77 2f6b 7566 6c6f 775f  y-kuflow/kuflow_
-00000760: 7465 6d70 6f72 616c 5f61 6374 6976 6974  temporal_activit
-00000770: 795f 6b75 666c 6f77 2f6d 6f64 656c 732f  y_kuflow/models/
-00000780: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
-00000790: 6475 6c65 3e19 0000 0073 5600 0000 b02f  dule>....sV..../
-000007a0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000007b0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000007c0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000007d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000007e0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-000007f0: 0201 02d6                                ....
+000000d0: 6d28 5a28 6d29 5a29 6d2a 5a2a 6d2b 5a2b  m(Z(m)Z)m*Z*m+Z+
+000000e0: 6d2c 5a2c 0100 6402 6403 6404 6405 6406  m,Z,..d.d.d.d.d.
+000000f0: 6407 6408 6409 640a 640b 640c 640d 640e  d.d.d.d.d.d.d.d.
+00000100: 640f 6410 6411 6412 6413 6414 6415 6416  d.d.d.d.d.d.d.d.
+00000110: 6417 6418 6419 641a 641b 641c 641d 641e  d.d.d.d.d.d.d.d.
+00000120: 641f 6420 6421 6422 6423 6424 6425 6426  d.d d!d"d#d$d%d&
+00000130: 6427 6428 6429 642a 642b 642c 642d 672c  d'd(d)d*d+d,d-g,
+00000140: 5a2d 642e 5300 292f e901 0000 0029 2cda  Z-d.S.)/.....),.
+00000150: 1441 7070 656e 6454 6173 6b4c 6f67 5265  .AppendTaskLogRe
+00000160: 7175 6573 74da 1541 7070 656e 6454 6173  quest..AppendTas
+00000170: 6b4c 6f67 5265 7370 6f6e 7365 da11 4173  kLogResponse..As
+00000180: 7369 676e 5461 736b 5265 7175 6573 74da  signTaskRequest.
+00000190: 1241 7373 6967 6e54 6173 6b52 6573 706f  .AssignTaskRespo
+000001a0: 6e73 65da 1d43 6861 6e67 6550 726f 6365  nse..ChangeProce
+000001b0: 7373 496e 6974 6961 746f 7252 6571 7565  ssInitiatorReque
+000001c0: 7374 da1e 4368 616e 6765 5072 6f63 6573  st..ChangeProces
+000001d0: 7349 6e69 7469 6174 6f72 5265 7370 6f6e  sInitiatorRespon
+000001e0: 7365 da10 436c 6169 6d54 6173 6b52 6571  se..ClaimTaskReq
+000001f0: 7565 7374 da11 436c 6169 6d54 6173 6b52  uest..ClaimTaskR
+00000200: 6573 706f 6e73 65da 1343 6f6d 706c 6574  esponse..Complet
+00000210: 6554 6173 6b52 6571 7565 7374 da14 436f  eTaskRequest..Co
+00000220: 6d70 6c65 7465 5461 736b 5265 7370 6f6e  mpleteTaskRespon
+00000230: 7365 da11 4372 6561 7465 5461 736b 5265  se..CreateTaskRe
+00000240: 7175 6573 74da 1243 7265 6174 6554 6173  quest..CreateTas
+00000250: 6b52 6573 706f 6e73 65da 1b44 656c 6574  kResponse..Delet
+00000260: 6550 726f 6365 7373 456c 656d 656e 7452  eProcessElementR
+00000270: 6571 7565 7374 da1c 4465 6c65 7465 5072  equest..DeletePr
+00000280: 6f63 6573 7345 6c65 6d65 6e74 5265 7370  ocessElementResp
+00000290: 6f6e 7365 da18 4465 6c65 7465 5461 736b  onse..DeleteTask
+000002a0: 456c 656d 656e 7452 6571 7565 7374 da19  ElementRequest..
+000002b0: 4465 6c65 7465 5461 736b 456c 656d 656e  DeleteTaskElemen
+000002c0: 7452 6573 706f 6e73 65da 2544 656c 6574  tResponse.%Delet
+000002d0: 6554 6173 6b45 6c65 6d65 6e74 5661 6c75  eTaskElementValu
+000002e0: 6544 6f63 756d 656e 7452 6571 7565 7374  eDocumentRequest
+000002f0: da26 4465 6c65 7465 5461 736b 456c 656d  .&DeleteTaskElem
+00000300: 656e 7456 616c 7565 446f 6375 6d65 6e74  entValueDocument
+00000310: 5265 7370 6f6e 7365 da14 4669 6e64 5072  Response..FindPr
+00000320: 6f63 6573 7365 7352 6571 7565 7374 da15  ocessesRequest..
+00000330: 4669 6e64 5072 6f63 6573 7365 7352 6573  FindProcessesRes
+00000340: 706f 6e73 65da 0f46 696e 6454 6173 6b52  ponse..FindTaskR
+00000350: 6571 7565 7374 da10 4669 6e64 5461 736b  equest..FindTask
+00000360: 5265 7370 6f6e 7365 da18 5265 7472 6965  Response..Retrie
+00000370: 7665 5072 696e 6369 7061 6c52 6571 7565  vePrincipalReque
+00000380: 7374 da19 5265 7472 6965 7665 5072 696e  st..RetrievePrin
+00000390: 6369 7061 6c52 6573 706f 6e73 65da 1652  cipalResponse..R
+000003a0: 6574 7269 6576 6550 726f 6365 7373 5265  etrieveProcessRe
+000003b0: 7175 6573 74da 1752 6574 7269 6576 6550  quest..RetrieveP
+000003c0: 726f 6365 7373 5265 7370 6f6e 7365 da13  rocessResponse..
+000003d0: 5265 7472 6965 7665 5461 736b 5265 7175  RetrieveTaskRequ
+000003e0: 6573 74da 1452 6574 7269 6576 6554 6173  est..RetrieveTas
+000003f0: 6b52 6573 706f 6e73 65da 1952 6574 7269  kResponse..Retri
+00000400: 6576 6554 656e 616e 7455 7365 7252 6571  eveTenantUserReq
+00000410: 7565 7374 da1a 5265 7472 6965 7665 5465  uest..RetrieveTe
+00000420: 6e61 6e74 5573 6572 5265 7370 6f6e 7365  nantUserResponse
+00000430: da14 526f 626f 7457 6f72 6b66 6c6f 7752  ..RobotWorkflowR
+00000440: 6571 7565 7374 da15 526f 626f 7457 6f72  equest..RobotWor
+00000450: 6b66 6c6f 7752 6573 706f 6e73 65da 1953  kflowResponse..S
+00000460: 6176 6550 726f 6365 7373 456c 656d 656e  aveProcessElemen
+00000470: 7452 6571 7565 7374 da1a 5361 7665 5072  tRequest..SavePr
+00000480: 6f63 6573 7345 6c65 6d65 6e74 5265 7370  ocessElementResp
+00000490: 6f6e 7365 da1c 5361 7665 5072 6f63 6573  onse..SaveProces
+000004a0: 7345 6e74 6974 7944 6174 6152 6571 7565  sEntityDataReque
+000004b0: 7374 da1d 5361 7665 5072 6f63 6573 7345  st..SaveProcessE
+000004c0: 6e74 6974 7944 6174 6152 6573 706f 6e73  ntityDataRespons
+000004d0: 65da 1653 6176 6554 6173 6b45 6c65 6d65  e..SaveTaskEleme
+000004e0: 6e74 5265 7175 6573 74da 1753 6176 6554  ntRequest..SaveT
+000004f0: 6173 6b45 6c65 6d65 6e74 5265 7370 6f6e  askElementRespon
+00000500: 7365 da21 5361 7665 5461 736b 4a73 6f6e  se.!SaveTaskJson
+00000510: 466f 726d 7356 616c 7565 4461 7461 5265  FormsValueDataRe
+00000520: 7175 6573 74da 2253 6176 6554 6173 6b4a  quest."SaveTaskJ
+00000530: 736f 6e46 6f72 6d73 5661 6c75 6544 6174  sonFormsValueDat
+00000540: 6152 6573 706f 6e73 65da 1955 7365 7241  aResponse..UserA
+00000550: 6374 696f 6e57 6f72 6b66 6c6f 7752 6571  ctionWorkflowReq
+00000560: 7565 7374 da1a 5573 6572 4163 7469 6f6e  uest..UserAction
+00000570: 576f 726b 666c 6f77 5265 7370 6f6e 7365  WorkflowResponse
+00000580: da0f 576f 726b 666c 6f77 5265 7175 6573  ..WorkflowReques
+00000590: 74da 1057 6f72 6b66 6c6f 7752 6573 706f  t..WorkflowRespo
+000005a0: 6e73 6572 0200 0000 7203 0000 0072 0400  nser....r....r..
+000005b0: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
+000005c0: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+000005d0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000005e0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+000005f0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00000600: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000610: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000620: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000630: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+00000640: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
+00000650: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00000660: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00000670: 722b 0000 0072 2c00 0000 722d 0000 004e  r+...r,...r-...N
+00000680: 292e da07 5f6d 6f64 656c 7372 0200 0000  )..._modelsr....
+00000690: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+000006a0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+000006b0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+000006c0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+000006d0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+000006e0: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+000006f0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00000700: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000710: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000720: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000730: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+00000740: 2600 0000 7227 0000 0072 2800 0000 7229  &...r'...r(...r)
+00000750: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
+00000760: 0000 722d 0000 00da 075f 5f61 6c6c 5f5f  ..r-.....__all__
+00000770: a900 7230 0000 0072 3000 0000 fa6a 2f77  ..r0...r0....j/w
+00000780: 6f72 6b2f 6b75 666c 6f77 2d73 646b 2d70  ork/kuflow-sdk-p
+00000790: 7974 686f 6e2f 6b75 666c 6f77 2d74 656d  ython/kuflow-tem
+000007a0: 706f 7261 6c2d 6163 7469 7669 7479 2d6b  poral-activity-k
+000007b0: 7566 6c6f 772f 6b75 666c 6f77 5f74 656d  uflow/kuflow_tem
+000007c0: 706f 7261 6c5f 6163 7469 7669 7479 5f6b  poral_activity_k
+000007d0: 7566 6c6f 772f 6d6f 6465 6c73 2f5f 5f69  uflow/models/__i
+000007e0: 6e69 745f 5f2e 7079 da08 3c6d 6f64 756c  nit__.py..<modul
+000007f0: 653e 1900 0000 735a 0000 00b8 3102 0102  e>....sZ....1...
+00000800: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000810: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000820: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000830: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000840: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000850: 0102 0102 d4                             .....
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 15 12:57:18 2024 UTC, .py size: 22070 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 550d 0d0a 0000 0000 ae45 f465 3656 0000  U........E.e6V..
+00000000: 550d 0d0a 0000 0000 1c2a 1566 e959 0000  U........*.f.Y..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 2803 0000 6400  .....@...s(...d.
+00000020: 0004 0000 0040 0000 0073 4c03 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c08 6d09 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6509 6a0a 8303 5a0b  d.d...d.e.j...Z.
 00000070: 4700 6406 6407 8400 6407 6509 6a0a 8303  G.d.d...d.e.j...
 00000080: 5a0c 4700 6408 6409 8400 6409 6509 6a0a  Z.G.d.d...d.e.j.
 00000090: 8303 5a0d 4700 640a 640b 8400 640b 6509  ..Z.G.d.d...d.e.
@@ -47,1366 +47,1425 @@
 000002e0: 6a0a 8303 5a2e 4700 644c 644d 8400 644d  j...Z.G.dLdM..dM
 000002f0: 6509 6a0a 8303 5a2f 4700 644e 644f 8400  e.j...Z/G.dNdO..
 00000300: 644f 6509 6a0a 8303 5a30 4700 6450 6451  dOe.j...Z0G.dPdQ
 00000310: 8400 6451 6509 6a0a 8303 5a31 4700 6452  ..dQe.j...Z1G.dR
 00000320: 6453 8400 6453 6509 6a0a 8303 5a32 4700  dS..dSe.j...Z2G.
 00000330: 6454 6455 8400 6455 6509 6a0a 8303 5a33  dTdU..dUe.j...Z3
 00000340: 4700 6456 6457 8400 6457 6509 6a0a 8303  G.dVdW..dWe.j...
-00000350: 5a34 6458 5300 2959 e900 0000 0029 04da  Z4dXS.)Y.....)..
-00000360: 0341 6e79 da04 4469 6374 da04 4c69 7374  .Any..Dict..List
-00000370: da08 4f70 7469 6f6e 616c 2901 da06 6d6f  ..Optional)...mo
-00000380: 6465 6c73 2901 da0e 5f73 6572 6961 6c69  dels)..._seriali
-00000390: 7a61 7469 6f6e 6300 0000 0000 0000 0000  zationc.........
-000003a0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-000003b0: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
-000003c0: 6403 6404 9c02 6901 5a03 6504 6505 6405  d.d...i.Z.e.e.d.
-000003d0: 6406 9c03 8700 6601 6407 6408 840c 5a06  d.....f.d.d...Z.
-000003e0: 8700 0400 5a07 5300 2909 da0f 576f 726b  ....Z.S.)...Work
-000003f0: 666c 6f77 5265 7175 6573 74da 0a70 726f  flowRequest..pro
-00000400: 6365 7373 5f69 64da 0970 726f 6365 7373  cess_id..process
-00000410: 4964 da03 7374 72a9 02da 036b 6579 da04  Id..str....key..
-00000420: 7479 7065 4ea9 0372 0900 0000 da06 6b77  typeN..r......kw
-00000430: 6172 6773 da06 7265 7475 726e 6302 0000  args..returnc...
-00000440: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00000450: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
-00000460: 6600 7c02 8e01 0100 7c01 7c00 5f02 6401  f.|.....|.|._.d.
-00000470: 5300 a902 7a5f 0a20 2020 2020 2020 2050  S...z_.        P
-00000480: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-00000490: 2020 2020 2020 2070 726f 6365 7373 5f69         process_i
-000004a0: 643a 2049 6465 6e74 6966 6965 7220 6f66  d: Identifier of
-000004b0: 2074 6865 2072 656c 6174 6564 2063 7265   the related cre
-000004c0: 6174 6564 2070 726f 6365 7373 0a20 2020  ated process.   
-000004d0: 2020 2020 204e a903 da05 7375 7065 72da       N....super.
-000004e0: 085f 5f69 6e69 745f 5f72 0900 0000 a903  .__init__r......
-000004f0: da04 7365 6c66 7209 0000 0072 1000 0000  ..selfr....r....
-00000500: a901 da09 5f5f 636c 6173 735f 5fa9 00fa  ....__class__...
-00000510: 692f 776f 726b 2f6b 7566 6c6f 772d 7364  i/work/kuflow-sd
-00000520: 6b2d 7079 7468 6f6e 2f6b 7566 6c6f 772d  k-python/kuflow-
-00000530: 7465 6d70 6f72 616c 2d61 6374 6976 6974  temporal-activit
-00000540: 792d 6b75 666c 6f77 2f6b 7566 6c6f 775f  y-kuflow/kuflow_
-00000550: 7465 6d70 6f72 616c 5f61 6374 6976 6974  temporal_activit
-00000560: 795f 6b75 666c 6f77 2f6d 6f64 656c 732f  y_kuflow/models/
-00000570: 5f6d 6f64 656c 732e 7079 7215 0000 0029  _models.pyr....)
-00000580: 0000 0073 0400 0000 0005 0e01 7a18 576f  ...s........z.Wo
-00000590: 726b 666c 6f77 5265 7175 6573 742e 5f5f  rkflowRequest.__
-000005a0: 696e 6974 5f5f a908 da08 5f5f 6e61 6d65  init__....__name
-000005b0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000005c0: 5f5f 7175 616c 6e61 6d65 5f5f da0e 5f61  __qualname__.._a
-000005d0: 7474 7269 6275 7465 5f6d 6170 720b 0000  ttribute_mapr...
-000005e0: 0072 0200 0000 7215 0000 00da 0d5f 5f63  .r....r......__c
-000005f0: 6c61 7373 6365 6c6c 5f5f 721a 0000 0072  lasscell__r....r
-00000600: 1a00 0000 7218 0000 0072 1b00 0000 7208  ....r....r....r.
-00000610: 0000 0024 0000 0073 0800 0000 0802 0200  ...$...s........
-00000620: 08ff 0404 7208 0000 0063 0000 0000 0000  ....r....c......
-00000630: 0000 0000 0000 0000 0000 0500 0000 0000  ................
-00000640: 0000 733a 0000 0065 005a 0164 005a 0264  ..s:...e.Z.d.Z.d
-00000650: 0164 0164 0264 039c 0269 015a 0364 0865  .d.d.d...i.Z.d.e
-00000660: 0465 0519 0065 0664 0464 059c 0387 0066  .e...e.d.d.....f
-00000670: 0164 0664 0784 0d5a 0787 0004 005a 0853  .d.d...Z.....Z.S
-00000680: 0029 09da 1057 6f72 6b66 6c6f 7752 6573  .)...WorkflowRes
-00000690: 706f 6e73 65da 076d 6573 7361 6765 720b  ponse..messager.
-000006a0: 0000 0072 0c00 0000 4ea9 0372 2300 0000  ...r....N..r#...
-000006b0: 7210 0000 0072 1100 0000 6302 0000 0000  r....r....c.....
-000006c0: 0000 0000 0000 0003 0000 0003 0000 000b  ................
-000006d0: 0000 0073 1800 0000 7400 8300 6a01 6600  ...s....t...j.f.
-000006e0: 7c02 8e01 0100 7c01 7c00 5f02 6401 5300  |.....|.|._.d.S.
-000006f0: a902 7a43 0a20 2020 2020 2020 2050 6172  ..zC.        Par
-00000700: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00000710: 2020 2020 206d 6573 7361 6765 3a20 5265       message: Re
-00000720: 7370 6f6e 7365 206d 6573 7361 6765 0a20  sponse message. 
-00000730: 2020 2020 2020 204e a903 7214 0000 0072         N..r....r
-00000740: 1500 0000 7223 0000 00a9 0372 1700 0000  ....r#.....r....
-00000750: 7223 0000 0072 1000 0000 7218 0000 0072  r#...r....r....r
-00000760: 1a00 0000 721b 0000 0072 1500 0000 3700  ....r....r....7.
-00000770: 0000 7304 0000 0000 050e 017a 1957 6f72  ..s........z.Wor
-00000780: 6b66 6c6f 7752 6573 706f 6e73 652e 5f5f  kflowResponse.__
-00000790: 696e 6974 5f5f 2901 4ea9 0972 1d00 0000  init__).N..r....
-000007a0: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-000007b0: 0500 0000 720b 0000 0072 0200 0000 7215  ....r....r....r.
-000007c0: 0000 0072 2100 0000 721a 0000 0072 1a00  ...r!...r....r..
-000007d0: 0000 7218 0000 0072 1b00 0000 7222 0000  ..r....r....r"..
-000007e0: 0032 0000 0073 0800 0000 0802 0200 08ff  .2...s..........
-000007f0: 0404 7222 0000 0063 0000 0000 0000 0000  ..r"...c........
-00000800: 0000 0000 0000 0000 0700 0000 0000 0000  ................
-00000810: 7352 0000 0065 005a 0164 005a 0264 0164  sR...e.Z.d.Z.d.d
-00000820: 0264 039c 0264 0464 0264 039c 0264 0564  .d...d.d.d...d.d
-00000830: 0264 039c 0264 0664 0264 039c 0264 079c  .d...d.d.d...d..
-00000840: 045a 0365 0465 0465 0465 0465 0564 0864  .Z.e.e.e.e.e.d.d
-00000850: 099c 0687 0066 0164 0a64 0b84 0c5a 0687  .....f.d.d...Z..
-00000860: 0004 005a 0753 0029 0cda 1955 7365 7241  ...Z.S.)...UserA
-00000870: 6374 696f 6e57 6f72 6b66 6c6f 7752 6571  ctionWorkflowReq
-00000880: 7565 7374 720a 0000 0072 0b00 0000 720c  uestr....r....r.
-00000890: 0000 005a 1875 7365 7241 6374 696f 6e44  ...Z.userActionD
-000008a0: 6566 696e 6974 696f 6e43 6f64 655a 0c75  efinitionCodeZ.u
-000008b0: 7365 7241 6374 696f 6e49 645a 1472 6571  serActionIdZ.req
-000008c0: 7565 7374 6f72 5072 696e 6369 7061 6c49  uestorPrincipalI
-000008d0: 6429 0472 0900 0000 da1b 7573 6572 5f61  d).r......user_a
-000008e0: 6374 696f 6e5f 6465 6669 6e69 7469 6f6e  ction_definition
-000008f0: 5f63 6f64 65da 0e75 7365 725f 6163 7469  _code..user_acti
-00000900: 6f6e 5f69 64da 1672 6571 7565 7374 6f72  on_id..requestor
-00000910: 5f70 7269 6e63 6970 616c 5f69 644e 2906  _principal_idN).
-00000920: 7209 0000 0072 2a00 0000 722b 0000 0072  r....r*...r+...r
-00000930: 2c00 0000 7210 0000 0072 1100 0000 6305  ,...r....r....c.
-00000940: 0000 0000 0000 0000 0000 0006 0000 0003  ................
-00000950: 0000 000b 0000 0073 2a00 0000 7400 8300  .......s*...t...
-00000960: 6a01 6600 7c05 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-00000970: 7c02 7c00 5f03 7c03 7c00 5f04 7c04 7c00  |.|._.|.|._.|.|.
-00000980: 5f05 6401 5300 2902 613a 0100 000a 2020  _.d.S.).a:....  
-00000990: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000009a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000009b0: 6f63 6573 735f 6964 3a20 4964 656e 7469  ocess_id: Identi
-000009c0: 6669 6572 206f 6620 7468 6520 7265 6c61  fier of the rela
-000009d0: 7465 6420 7072 6f63 6573 730a 2020 2020  ted process.    
-000009e0: 2020 2020 2020 2020 7573 6572 5f61 6374          user_act
-000009f0: 696f 6e5f 6465 6669 6e69 7469 6f6e 5f63  ion_definition_c
-00000a00: 6f64 653a 2043 6f64 6520 6f66 2074 6865  ode: Code of the
-00000a10: 2075 7365 7220 6163 7469 6f6e 2064 6566   user action def
-00000a20: 696e 6974 696f 6e0a 2020 2020 2020 2020  inition.        
-00000a30: 2020 2020 7573 6572 5f61 6374 696f 6e5f      user_action_
-00000a40: 6964 3a20 4964 656e 7469 6669 6572 206f  id: Identifier o
-00000a50: 6620 7468 6520 7573 6572 2061 6374 696f  f the user actio
-00000a60: 6e0a 2020 2020 2020 2020 2020 2020 7265  n.            re
-00000a70: 7175 6573 746f 725f 7072 696e 6369 7061  questor_principa
-00000a80: 6c5f 6964 3a20 4964 656e 7469 6669 6572  l_id: Identifier
-00000a90: 206f 6620 7468 6520 7072 696e 6369 7061   of the principa
-00000aa0: 6c20 7468 6174 2072 6571 7565 7374 2074  l that request t
-00000ab0: 6865 2075 7365 7220 6163 7469 6f6e 0a20  he user action. 
-00000ac0: 2020 2020 2020 204e 2906 7214 0000 0072         N).r....r
-00000ad0: 1500 0000 7209 0000 0072 2a00 0000 722b  ....r....r*...r+
-00000ae0: 0000 0072 2c00 0000 2906 7217 0000 0072  ...r,...).r....r
-00000af0: 0900 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
-00000b00: 0000 0072 1000 0000 7218 0000 0072 1a00  ...r....r....r..
-00000b10: 0000 721b 0000 0072 1500 0000 4800 0000  ..r....r....H...
-00000b20: 730a 0000 0000 0f0e 0106 0106 0106 017a  s..............z
-00000b30: 2255 7365 7241 6374 696f 6e57 6f72 6b66  "UserActionWorkf
-00000b40: 6c6f 7752 6571 7565 7374 2e5f 5f69 6e69  lowRequest.__ini
-00000b50: 745f 5f72 1c00 0000 721a 0000 0072 1a00  t__r....r....r..
-00000b60: 0000 7218 0000 0072 1b00 0000 7229 0000  ..r....r....r)..
-00000b70: 0040 0000 0073 1800 0000 0802 0801 0801  .@...s..........
-00000b80: 0801 08fc 0609 0201 0201 0201 0201 0201  ................
-00000b90: 02f9 7229 0000 0063 0000 0000 0000 0000  ..r)...c........
-00000ba0: 0000 0000 0000 0000 0500 0000 0000 0000  ................
-00000bb0: 733a 0000 0065 005a 0164 005a 0264 0164  s:...e.Z.d.Z.d.d
-00000bc0: 0164 0264 039c 0269 015a 0364 0865 0465  .d.d...i.Z.d.e.e
-00000bd0: 0519 0065 0664 0464 059c 0387 0066 0164  ...e.d.d.....f.d
-00000be0: 0664 0784 0d5a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
-00000bf0: 09da 1a55 7365 7241 6374 696f 6e57 6f72  ...UserActionWor
-00000c00: 6b66 6c6f 7752 6573 706f 6e73 6572 2300  kflowResponser#.
-00000c10: 0000 720b 0000 0072 0c00 0000 4e72 2400  ..r....r....Nr$.
-00000c20: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000c30: 0000 0003 0000 000b 0000 0073 1800 0000  ...........s....
-00000c40: 7400 8300 6a01 6600 7c02 8e01 0100 7c01  t...j.f.|.....|.
-00000c50: 7c00 5f02 6401 5300 2902 7a4f 0a20 2020  |._.d.S.).zO.   
-00000c60: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-00000c70: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00000c80: 7361 6765 3a20 5573 6572 2061 6374 696f  sage: User actio
-00000c90: 6e20 6d65 7373 6167 6520 7265 7370 6f6e  n message respon
-00000ca0: 7365 0a20 2020 2020 2020 204e 7226 0000  se.        Nr&..
-00000cb0: 0072 2700 0000 7218 0000 0072 1a00 0000  .r'...r....r....
-00000cc0: 721b 0000 0072 1500 0000 6300 0000 7304  r....r....c...s.
-00000cd0: 0000 0000 050e 017a 2355 7365 7241 6374  .......z#UserAct
-00000ce0: 696f 6e57 6f72 6b66 6c6f 7752 6573 706f  ionWorkflowRespo
-00000cf0: 6e73 652e 5f5f 696e 6974 5f5f 2901 4e72  nse.__init__).Nr
-00000d00: 2800 0000 721a 0000 0072 1a00 0000 7218  (...r....r....r.
-00000d10: 0000 0072 1b00 0000 722d 0000 005e 0000  ...r....r-...^..
-00000d20: 0073 0800 0000 0802 0200 08ff 0404 722d  .s............r-
-00000d30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000d40: 0000 0000 0500 0000 0000 0000 733e 0000  ............s>..
-00000d50: 0065 005a 0164 005a 0264 0164 0264 039c  .e.Z.d.Z.d.d.d..
-00000d60: 0264 0464 0264 039c 0264 059c 025a 0365  .d.d.d...d...Z.e
-00000d70: 0465 0465 0564 0664 079c 0487 0066 0164  .e.e.d.d.....f.d
-00000d80: 0864 0984 0c5a 0687 0004 005a 0753 0029  .d...Z.....Z.S.)
-00000d90: 0ada 1452 6f62 6f74 576f 726b 666c 6f77  ...RobotWorkflow
-00000da0: 5265 7175 6573 7472 0a00 0000 720b 0000  Requestr....r...
-00000db0: 0072 0c00 0000 da06 7461 736b 4964 2902  .r......taskId).
-00000dc0: 7209 0000 00da 0774 6173 6b5f 6964 4e29  r......task_idN)
-00000dd0: 0472 0900 0000 7230 0000 0072 1000 0000  .r....r0...r....
-00000de0: 7211 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000df0: 0000 0400 0000 0300 0000 0b00 0000 731e  ..............s.
-00000e00: 0000 0074 0083 006a 0166 007c 038e 0101  ...t...j.f.|....
-00000e10: 007c 017c 005f 027c 027c 005f 0364 0153  .|.|._.|.|._.d.S
-00000e20: 0072 1200 0000 2904 7214 0000 0072 1500  .r....).r....r..
-00000e30: 0000 7209 0000 0072 3000 0000 2904 7217  ..r....r0...).r.
-00000e40: 0000 0072 0900 0000 7230 0000 0072 1000  ...r....r0...r..
-00000e50: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000e60: 0072 1500 0000 7200 0000 7306 0000 0000  .r....r...s.....
-00000e70: 050e 0106 017a 1d52 6f62 6f74 576f 726b  .....z.RobotWork
-00000e80: 666c 6f77 5265 7175 6573 742e 5f5f 696e  flowRequest.__in
-00000e90: 6974 5f5f 721c 0000 0072 1a00 0000 721a  it__r....r....r.
-00000ea0: 0000 0072 1800 0000 721b 0000 0072 2e00  ...r....r....r..
-00000eb0: 0000 6c00 0000 7308 0000 0008 0208 0108  ..l...s.........
-00000ec0: fe06 0572 2e00 0000 6300 0000 0000 0000  ...r....c.......
-00000ed0: 0000 0000 0000 0000 0005 0000 0000 0000  ................
-00000ee0: 0073 3a00 0000 6500 5a01 6400 5a02 6401  .s:...e.Z.d.Z.d.
-00000ef0: 6401 6402 6403 9c02 6901 5a03 6408 6504  d.d.d...i.Z.d.e.
-00000f00: 6505 1900 6506 6404 6405 9c03 8700 6601  e...e.d.d.....f.
-00000f10: 6406 6407 840d 5a07 8700 0400 5a08 5300  d.d...Z.....Z.S.
-00000f20: 2909 da15 526f 626f 7457 6f72 6b66 6c6f  )...RobotWorkflo
-00000f30: 7752 6573 706f 6e73 6572 2300 0000 720b  wResponser#...r.
-00000f40: 0000 0072 0c00 0000 4e72 2400 0000 6302  ...r....Nr$...c.
-00000f50: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00000f60: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
-00000f70: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-00000f80: 6401 5300 7225 0000 0072 2600 0000 7227  d.S.r%...r&...r'
-00000f90: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
-00000fa0: 0000 7215 0000 0081 0000 0073 0400 0000  ..r........s....
-00000fb0: 0005 0e01 7a1e 526f 626f 7457 6f72 6b66  ....z.RobotWorkf
-00000fc0: 6c6f 7752 6573 706f 6e73 652e 5f5f 696e  lowResponse.__in
-00000fd0: 6974 5f5f 2901 4e72 2800 0000 721a 0000  it__).Nr(...r...
-00000fe0: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
-00000ff0: 7231 0000 007c 0000 0073 0800 0000 0802  r1...|...s......
-00001000: 0200 08ff 0404 7231 0000 0063 0000 0000  ......r1...c....
-00001010: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00001020: 0000 0000 7334 0000 0065 005a 0164 005a  ....s4...e.Z.d.Z
-00001030: 0264 0164 0264 0364 049c 0269 015a 0365  .d.d.d.d...i.Z.e
-00001040: 0465 0564 0564 069c 0387 0066 0164 0764  .e.d.d.....f.d.d
-00001050: 0884 0c5a 0687 0004 005a 0753 0029 09da  ...Z.....Z.S.)..
-00001060: 1852 6574 7269 6576 6550 7269 6e63 6970  .RetrievePrincip
-00001070: 616c 5265 7175 6573 74da 0c70 7269 6e63  alRequest..princ
-00001080: 6970 616c 5f69 64da 0b70 7269 6e63 6970  ipal_id..princip
-00001090: 616c 4964 720b 0000 0072 0c00 0000 4e29  alIdr....r....N)
-000010a0: 0372 3300 0000 7210 0000 0072 1100 0000  .r3...r....r....
-000010b0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000010c0: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
-000010d0: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
-000010e0: 5f02 6401 5300 2902 7a5d 0a20 2020 2020  _.d.S.).z].     
-000010f0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-00001100: 2020 2020 2020 2020 2020 2070 7269 6e63             princ
-00001110: 6970 616c 5f69 643a 2049 6465 6e74 6966  ipal_id: Identif
-00001120: 6965 7220 6f66 2074 6865 2072 6571 7565  ier of the reque
-00001130: 7374 6564 2070 7269 6e63 6970 616c 0a20  sted principal. 
-00001140: 2020 2020 2020 204e 2903 7214 0000 0072         N).r....r
-00001150: 1500 0000 7233 0000 0029 0372 1700 0000  ....r3...).r....
-00001160: 7233 0000 0072 1000 0000 7218 0000 0072  r3...r....r....r
-00001170: 1a00 0000 721b 0000 0072 1500 0000 9400  ....r....r......
-00001180: 0000 7304 0000 0000 050e 017a 2152 6574  ..s........z!Ret
-00001190: 7269 6576 6550 7269 6e63 6970 616c 5265  rievePrincipalRe
-000011a0: 7175 6573 742e 5f5f 696e 6974 5f5f 721c  quest.__init__r.
-000011b0: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
-000011c0: 0000 721b 0000 0072 3200 0000 8f00 0000  ..r....r2.......
-000011d0: 7308 0000 0008 0202 0008 ff04 0472 3200  s............r2.
-000011e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000011f0: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
-00001200: 6500 5a01 6400 5a02 6401 6401 6402 6403  e.Z.d.Z.d.d.d.d.
-00001210: 9c02 6901 5a03 6504 6a05 6506 6404 6405  ..i.Z.e.j.e.d.d.
-00001220: 9c03 8700 6601 6406 6407 840c 5a07 8700  ....f.d.d...Z...
-00001230: 0400 5a08 5300 2908 da19 5265 7472 6965  ..Z.S.)...Retrie
-00001240: 7665 5072 696e 6369 7061 6c52 6573 706f  vePrincipalRespo
-00001250: 6e73 65da 0970 7269 6e63 6970 616c da09  nse..principal..
-00001260: 5072 696e 6369 7061 6c72 0c00 0000 4e29  Principalr....N)
-00001270: 0372 3600 0000 7210 0000 0072 1100 0000  .r6...r....r....
-00001280: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00001290: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
-000012a0: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
-000012b0: 5f02 6401 5300 2902 7a4d 0a20 2020 2020  _.d.S.).zM.     
-000012c0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-000012d0: 2020 2020 2020 2020 2020 2070 7269 6e63             princ
-000012e0: 6970 616c 3a20 5072 696e 6369 7061 6c20  ipal: Principal 
-000012f0: 6461 7461 2072 6571 7565 7374 6564 0a20  data requested. 
-00001300: 2020 2020 2020 204e 2903 7214 0000 0072         N).r....r
-00001310: 1500 0000 7236 0000 0029 0372 1700 0000  ....r6...).r....
-00001320: 7236 0000 0072 1000 0000 7218 0000 0072  r6...r....r....r
-00001330: 1a00 0000 721b 0000 0072 1500 0000 a200  ....r....r......
-00001340: 0000 7304 0000 0000 050e 017a 2252 6574  ..s........z"Ret
-00001350: 7269 6576 6550 7269 6e63 6970 616c 5265  rievePrincipalRe
-00001360: 7370 6f6e 7365 2e5f 5f69 6e69 745f 5f29  sponse.__init__)
-00001370: 0972 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001380: 7220 0000 00da 0b6d 6f64 656c 735f 7265  r .....models_re
-00001390: 7374 7237 0000 0072 0200 0000 7215 0000  str7...r....r...
-000013a0: 0072 2100 0000 721a 0000 0072 1a00 0000  .r!...r....r....
-000013b0: 7218 0000 0072 1b00 0000 7235 0000 009d  r....r....r5....
-000013c0: 0000 0073 0800 0000 0802 0200 08ff 0404  ...s............
-000013d0: 7235 0000 0063 0000 0000 0000 0000 0000  r5...c..........
-000013e0: 0000 0000 0000 0400 0000 0000 0000 7334  ..............s4
-000013f0: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00001400: 0364 049c 0269 015a 0365 0465 0564 0564  .d...i.Z.e.e.d.d
-00001410: 069c 0387 0066 0164 0764 0884 0c5a 0687  .....f.d.d...Z..
-00001420: 0004 005a 0753 0029 09da 1952 6574 7269  ...Z.S.)...Retri
-00001430: 6576 6554 656e 616e 7455 7365 7252 6571  eveTenantUserReq
-00001440: 7565 7374 da0e 7465 6e61 6e74 5f75 7365  uest..tenant_use
-00001450: 725f 6964 5a0c 7465 6e61 6e74 5573 6572  r_idZ.tenantUser
-00001460: 4964 720b 0000 0072 0c00 0000 4e29 0372  Idr....r....N).r
-00001470: 3a00 0000 7210 0000 0072 1100 0000 6302  :...r....r....c.
-00001480: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-00001490: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
-000014a0: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-000014b0: 6401 5300 2902 7a61 0a20 2020 2020 2020  d.S.).za.       
-000014c0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-000014d0: 2020 2020 2020 2020 2074 656e 616e 745f           tenant_
-000014e0: 7573 6572 5f69 643a 2049 6465 6e74 6966  user_id: Identif
-000014f0: 6965 7220 6f66 2074 6865 2072 6571 7565  ier of the reque
-00001500: 7374 6564 2074 656e 616e 7420 7573 6572  sted tenant user
-00001510: 0a20 2020 2020 2020 204e 2903 7214 0000  .        N).r...
-00001520: 0072 1500 0000 723a 0000 0029 0372 1700  .r....r:...).r..
-00001530: 0000 723a 0000 0072 1000 0000 7218 0000  ..r:...r....r...
-00001540: 0072 1a00 0000 721b 0000 0072 1500 0000  .r....r....r....
-00001550: b000 0000 7304 0000 0000 050e 017a 2252  ....s........z"R
-00001560: 6574 7269 6576 6554 656e 616e 7455 7365  etrieveTenantUse
-00001570: 7252 6571 7565 7374 2e5f 5f69 6e69 745f  rRequest.__init_
-00001580: 5f72 1c00 0000 721a 0000 0072 1a00 0000  _r....r....r....
-00001590: 7218 0000 0072 1b00 0000 7239 0000 00ab  r....r....r9....
-000015a0: 0000 0073 0800 0000 0802 0200 08ff 0404  ...s............
-000015b0: 7239 0000 0063 0000 0000 0000 0000 0000  r9...c..........
-000015c0: 0000 0000 0000 0400 0000 0000 0000 7336  ..............s6
-000015d0: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-000015e0: 0364 049c 0269 015a 0365 046a 0565 0664  .d...i.Z.e.j.e.d
-000015f0: 0564 069c 0387 0066 0164 0764 0884 0c5a  .d.....f.d.d...Z
-00001600: 0787 0004 005a 0853 0029 09da 1a52 6574  .....Z.S.)...Ret
-00001610: 7269 6576 6554 656e 616e 7455 7365 7252  rieveTenantUserR
-00001620: 6573 706f 6e73 65da 0b74 656e 616e 745f  esponse..tenant_
-00001630: 7573 6572 5a0a 7465 6e61 6e74 5573 6572  userZ.tenantUser
-00001640: 7237 0000 0072 0c00 0000 4e29 0372 3c00  r7...r....N).r<.
-00001650: 0000 7210 0000 0072 1100 0000 6302 0000  ..r....r....c...
-00001660: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-00001670: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
-00001680: 6600 7c02 8e01 0100 7c01 7c00 5f02 6401  f.|.....|.|._.d.
-00001690: 5300 2902 7a51 0a20 2020 2020 2020 2050  S.).zQ.        P
-000016a0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-000016b0: 2020 2020 2020 2074 656e 616e 745f 7573         tenant_us
-000016c0: 6572 3a20 7465 6e61 6e74 5f75 7365 7220  er: tenant_user 
-000016d0: 6461 7461 2072 6571 7565 7374 6564 0a20  data requested. 
-000016e0: 2020 2020 2020 204e 2903 7214 0000 0072         N).r....r
-000016f0: 1500 0000 723c 0000 0029 0372 1700 0000  ....r<...).r....
-00001700: 723c 0000 0072 1000 0000 7218 0000 0072  r<...r....r....r
-00001710: 1a00 0000 721b 0000 0072 1500 0000 be00  ....r....r......
-00001720: 0000 7304 0000 0000 050e 017a 2352 6574  ..s........z#Ret
-00001730: 7269 6576 6554 656e 616e 7455 7365 7252  rieveTenantUserR
-00001740: 6573 706f 6e73 652e 5f5f 696e 6974 5f5f  esponse.__init__
-00001750: 2909 721d 0000 0072 1e00 0000 721f 0000  ).r....r....r...
-00001760: 0072 2000 0000 7238 0000 00da 0a54 656e  .r ...r8.....Ten
-00001770: 616e 7455 7365 7272 0200 0000 7215 0000  antUserr....r...
-00001780: 0072 2100 0000 721a 0000 0072 1a00 0000  .r!...r....r....
-00001790: 7218 0000 0072 1b00 0000 723b 0000 00b9  r....r....r;....
-000017a0: 0000 0073 0800 0000 0802 0200 08ff 0404  ...s............
-000017b0: 723b 0000 0063 0000 0000 0000 0000 0000  r;...c..........
-000017c0: 0000 0000 0000 0700 0000 0000 0000 735a  ..............sZ
-000017d0: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-000017e0: 039c 0264 0464 0264 039c 0264 0564 0664  ...d.d.d...d.d.d
-000017f0: 039c 0264 079c 035a 0364 0c65 0465 0519  ...d...Z.d.e.e..
-00001800: 0065 0465 0519 0065 0465 0665 0719 0019  .e.e...e.e.e....
-00001810: 0065 0864 0864 099c 0587 0066 0164 0a64  .e.d.d.....f.d.d
-00001820: 0b84 0d5a 0987 0004 005a 0a53 0029 0dda  ...Z.....Z.S.)..
-00001830: 1446 696e 6450 726f 6365 7373 6573 5265  .FindProcessesRe
-00001840: 7175 6573 74da 0470 6167 65da 0369 6e74  quest..page..int
-00001850: 720c 0000 00da 0473 697a 65da 0573 6f72  r......size..sor
-00001860: 7473 fa05 5b73 7472 5d29 0372 3f00 0000  ts..[str]).r?...
-00001870: 7241 0000 0072 4200 0000 4e29 0572 3f00  rA...rB...N).r?.
-00001880: 0000 7241 0000 0072 4200 0000 7210 0000  ..rA...rB...r...
-00001890: 0072 1100 0000 6304 0000 0000 0000 0000  .r....c.........
-000018a0: 0000 0005 0000 0003 0000 000b 0000 0073  ...............s
-000018b0: 2400 0000 7400 8300 6a01 6600 7c04 8e01  $...t...j.f.|...
-000018c0: 0100 7c01 7c00 5f02 7c02 7c00 5f03 7c03  ..|.|._.|.|._.|.
-000018d0: 7c00 5f04 6401 5300 2902 7abe 0a20 2020  |._.d.S.).z..   
-000018e0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-000018f0: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
-00001900: 653a 2050 6167 6520 7265 7175 6573 7465  e: Page requeste
-00001910: 642c 2030 2d69 6e64 6578 0a20 2020 2020  d, 0-index.     
-00001920: 2020 2020 2020 2073 697a 653a 2050 6167         size: Pag
-00001930: 6520 7369 7a65 0a20 2020 2020 2020 2020  e size.         
-00001940: 2020 2073 6f72 7473 3a20 536f 7274 696e     sorts: Sortin
-00001950: 6720 6372 6974 6572 6961 2069 6e20 7468  g criteria in th
-00001960: 6520 666f 726d 6174 3a20 7072 6f70 6572  e format: proper
-00001970: 7479 7b2c 6173 637c 6465 7363 7d2e 2045  ty{,asc|desc}. E
-00001980: 7861 6d70 6c65 3a20 6e61 6d65 2c64 6573  xample: name,des
-00001990: 630a 2020 2020 2020 2020 4e29 0572 1400  c.        N).r..
-000019a0: 0000 7215 0000 0072 3f00 0000 7241 0000  ..r....r?...rA..
-000019b0: 0072 4200 0000 2905 7217 0000 0072 3f00  .rB...).r....r?.
-000019c0: 0000 7241 0000 0072 4200 0000 7210 0000  ..rA...rB...r...
-000019d0: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000019e0: 7215 0000 00ce 0000 0073 0800 0000 0009  r........s......
-000019f0: 0e01 0601 0601 7a1d 4669 6e64 5072 6f63  ......z.FindProc
-00001a00: 6573 7365 7352 6571 7565 7374 2e5f 5f69  essesRequest.__i
-00001a10: 6e69 745f 5f29 034e 4e4e 290b 721d 0000  nit__).NNN).r...
-00001a20: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001a30: 7205 0000 0072 4000 0000 7204 0000 0072  r....r@...r....r
-00001a40: 0b00 0000 7202 0000 0072 1500 0000 7221  ....r....r....r!
-00001a50: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
-00001a60: 0000 721b 0000 0072 3e00 0000 c700 0000  ..r....r>.......
-00001a70: 731c 0000 0008 0208 0108 0108 fd06 0700  s...............
-00001a80: 0000 0000 ff02 0106 0006 000a 0002 0102  ................
-00001a90: fe72 3e00 0000 6300 0000 0000 0000 0000  .r>...c.........
-00001aa0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-00001ab0: 3600 0000 6500 5a01 6400 5a02 6401 6401  6...e.Z.d.Z.d.d.
-00001ac0: 6402 6403 9c02 6901 5a03 6504 6a05 6506  d.d...i.Z.e.j.e.
-00001ad0: 6404 6405 9c03 8700 6601 6406 6407 840c  d.d.....f.d.d...
-00001ae0: 5a07 8700 0400 5a08 5300 2908 da15 4669  Z.....Z.S.)...Fi
-00001af0: 6e64 5072 6f63 6573 7365 7352 6573 706f  ndProcessesRespo
-00001b00: 6e73 65da 0970 726f 6365 7373 6573 da0b  nse..processes..
-00001b10: 5072 6f63 6573 7350 6167 6572 0c00 0000  ProcessPager....
-00001b20: 4e29 0372 4500 0000 7210 0000 0072 1100  N).rE...r....r..
-00001b30: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00001b40: 0000 0003 0000 000b 0000 0073 1800 0000  ...........s....
-00001b50: 7400 8300 6a01 6600 7c02 8e01 0100 7c01  t...j.f.|.....|.
-00001b60: 7c00 5f02 6401 5300 2902 7a62 0a20 2020  |._.d.S.).zb.   
-00001b70: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
-00001b80: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00001b90: 6365 7373 6573 3a20 5072 6f63 6573 7320  cesses: Process 
-00001ba0: 7061 6765 2074 6861 7420 6d61 7468 2074  page that math t
-00001bb0: 6865 2072 6571 7565 7374 6564 2063 7269  he requested cri
-00001bc0: 7465 7269 610a 2020 2020 2020 2020 4e29  teria.        N)
-00001bd0: 0372 1400 0000 7215 0000 0072 4500 0000  .r....r....rE...
-00001be0: 2903 7217 0000 0072 4500 0000 7210 0000  ).r....rE...r...
-00001bf0: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001c00: 7215 0000 00e2 0000 0073 0400 0000 0005  r........s......
-00001c10: 0e01 7a1e 4669 6e64 5072 6f63 6573 7365  ..z.FindProcesse
-00001c20: 7352 6573 706f 6e73 652e 5f5f 696e 6974  sResponse.__init
-00001c30: 5f5f 2909 721d 0000 0072 1e00 0000 721f  __).r....r....r.
-00001c40: 0000 0072 2000 0000 7238 0000 0072 4600  ...r ...r8...rF.
-00001c50: 0000 7202 0000 0072 1500 0000 7221 0000  ..r....r....r!..
-00001c60: 0072 1a00 0000 721a 0000 0072 1800 0000  .r....r....r....
-00001c70: 721b 0000 0072 4400 0000 dd00 0000 7308  r....rD.......s.
-00001c80: 0000 0008 0202 0008 ff04 0472 4400 0000  ...........rD...
-00001c90: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001ca0: 0004 0000 0000 0000 0073 3400 0000 6500  .........s4...e.
-00001cb0: 5a01 6400 5a02 6401 6402 6403 6404 9c02  Z.d.Z.d.d.d.d...
-00001cc0: 6901 5a03 6504 6505 6405 6406 9c03 8700  i.Z.e.e.d.d.....
-00001cd0: 6601 6407 6408 840c 5a06 8700 0400 5a07  f.d.d...Z.....Z.
-00001ce0: 5300 2909 da16 5265 7472 6965 7665 5072  S.)...RetrievePr
-00001cf0: 6f63 6573 7352 6571 7565 7374 7209 0000  ocessRequestr...
-00001d00: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00001d10: 4e72 0f00 0000 6302 0000 0000 0000 0000  Nr....c.........
-00001d20: 0000 0003 0000 0003 0000 000b 0000 0073  ...............s
-00001d30: 1800 0000 7400 8300 6a01 6600 7c02 8e01  ....t...j.f.|...
-00001d40: 0100 7c01 7c00 5f02 6401 5300 2902 7a54  ..|.|._.d.S.).zT
-00001d50: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00001d60: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00001d70: 2070 726f 6365 7373 5f69 643a 2050 726f   process_id: Pro
-00001d80: 6365 7373 2049 6465 6e74 6966 6965 7220  cess Identifier 
-00001d90: 746f 2072 6574 7269 6576 650a 2020 2020  to retrieve.    
-00001da0: 2020 2020 4e72 1300 0000 7216 0000 0072      Nr....r....r
-00001db0: 1800 0000 721a 0000 0072 1b00 0000 7215  ....r....r....r.
-00001dc0: 0000 00f0 0000 0073 0400 0000 0005 0e01  .......s........
-00001dd0: 7a1f 5265 7472 6965 7665 5072 6f63 6573  z.RetrieveProces
-00001de0: 7352 6571 7565 7374 2e5f 5f69 6e69 745f  sRequest.__init_
-00001df0: 5f72 1c00 0000 721a 0000 0072 1a00 0000  _r....r....r....
-00001e00: 7218 0000 0072 1b00 0000 7247 0000 00eb  r....r....rG....
-00001e10: 0000 0073 0800 0000 0802 0200 08ff 0404  ...s............
-00001e20: 7247 0000 0063 0000 0000 0000 0000 0000  rG...c..........
-00001e30: 0000 0000 0000 0400 0000 0000 0000 7336  ..............s6
-00001e40: 0000 0065 005a 0164 005a 0264 0164 0164  ...e.Z.d.Z.d.d.d
-00001e50: 0264 039c 0269 015a 0365 046a 0565 0664  .d...i.Z.e.j.e.d
-00001e60: 0464 059c 0387 0066 0164 0664 0784 0c5a  .d.....f.d.d...Z
-00001e70: 0787 0004 005a 0853 0029 08da 1752 6574  .....Z.S.)...Ret
-00001e80: 7269 6576 6550 726f 6365 7373 5265 7370  rieveProcessResp
-00001e90: 6f6e 7365 da07 7072 6f63 6573 73da 0750  onse..process..P
-00001ea0: 726f 6365 7373 720c 0000 004e a903 7249  rocessr....N..rI
-00001eb0: 0000 0072 1000 0000 7211 0000 0063 0200  ...r....r....c..
-00001ec0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00001ed0: 0000 0b00 0000 7318 0000 0074 0083 006a  ......s....t...j
-00001ee0: 0166 007c 028e 0101 007c 017c 005f 0264  .f.|.....|.|._.d
-00001ef0: 0153 0029 027a 490a 2020 2020 2020 2020  .S.).zI.        
-00001f00: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-00001f10: 2020 2020 2020 2020 7072 6f63 6573 733a          process:
-00001f20: 2052 6571 7565 7374 6564 2070 726f 6365   Requested proce
-00001f30: 7373 2064 6174 610a 2020 2020 2020 2020  ss data.        
-00001f40: 4ea9 0372 1400 0000 7215 0000 0072 4900  N..r....r....rI.
-00001f50: 0000 a903 7217 0000 0072 4900 0000 7210  ....r....rI...r.
-00001f60: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
-00001f70: 0000 7215 0000 00fe 0000 0073 0400 0000  ..r........s....
-00001f80: 0005 0e01 7a20 5265 7472 6965 7665 5072  ....z RetrievePr
-00001f90: 6f63 6573 7352 6573 706f 6e73 652e 5f5f  ocessResponse.__
-00001fa0: 696e 6974 5f5f a909 721d 0000 0072 1e00  init__..r....r..
-00001fb0: 0000 721f 0000 0072 2000 0000 7238 0000  ..r....r ...r8..
-00001fc0: 0072 4a00 0000 7202 0000 0072 1500 0000  .rJ...r....r....
-00001fd0: 7221 0000 0072 1a00 0000 721a 0000 0072  r!...r....r....r
-00001fe0: 1800 0000 721b 0000 0072 4800 0000 f900  ....r....rH.....
-00001ff0: 0000 7308 0000 0008 0202 0008 ff04 0472  ..s............r
-00002000: 4800 0000 6300 0000 0000 0000 0000 0000  H...c...........
-00002010: 0000 0000 0007 0000 0000 0000 0073 5400  .............sT.
-00002020: 0000 6500 5a01 6400 5a02 6401 6402 6403  ..e.Z.d.Z.d.d.d.
-00002030: 9c02 6404 6402 6403 9c02 6405 6406 6403  ..d.d.d...d.d.d.
-00002040: 9c02 6407 9c03 5a03 640c 6504 6504 6505  ..d...Z.d.e.e.e.
-00002050: 6506 6507 6a08 1900 1900 6509 6408 6409  e.e.j.....e.d.d.
-00002060: 9c05 8700 6601 640a 640b 840d 5a0a 8700  ....f.d.d...Z...
-00002070: 0400 5a0b 5300 290d da19 5361 7665 5072  ..Z.S.)...SavePr
-00002080: 6f63 6573 7345 6c65 6d65 6e74 5265 7175  ocessElementRequ
-00002090: 6573 7472 0a00 0000 720b 0000 0072 0c00  estr....r....r..
-000020a0: 0000 da15 656c 656d 656e 7444 6566 696e  ....elementDefin
-000020b0: 6974 696f 6e43 6f64 65da 0d65 6c65 6d65  itionCode..eleme
-000020c0: 6e74 5661 6c75 6573 7a15 5b50 726f 6365  ntValuesz.[Proce
-000020d0: 7373 456c 656d 656e 7456 616c 7565 5d29  ssElementValue])
-000020e0: 0372 0900 0000 da17 656c 656d 656e 745f  .r......element_
-000020f0: 6465 6669 6e69 7469 6f6e 5f63 6f64 65da  definition_code.
-00002100: 0e65 6c65 6d65 6e74 5f76 616c 7565 734e  .element_valuesN
-00002110: 2905 7209 0000 0072 5200 0000 7253 0000  ).r....rR...rS..
-00002120: 0072 1000 0000 7211 0000 0063 0400 0000  .r....r....c....
-00002130: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00002140: 0b00 0000 7328 0000 0074 0083 006a 0166  ....s(...t...j.f
-00002150: 007c 048e 0101 007c 017c 005f 027c 027c  .|.....|.|._.|.|
-00002160: 005f 037c 0370 2067 007c 005f 0464 0153  ._.|.p g.|._.d.S
-00002170: 0029 027a ba0a 2020 2020 2020 2020 5061  .).z..        Pa
-00002180: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00002190: 2020 2020 2020 7072 6f63 6573 735f 6964        process_id
-000021a0: 3a20 5072 6f63 6573 7320 6964 656e 7469  : Process identi
-000021b0: 6669 6572 2074 6f20 7570 6461 7465 0a20  fier to update. 
-000021c0: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
-000021d0: 6e74 5f64 6566 696e 6974 696f 6e5f 636f  nt_definition_co
-000021e0: 6465 3a20 456c 656d 656e 7420 6465 6669  de: Element defi
-000021f0: 6e69 7469 6f6e 2063 6f64 650a 2020 2020  nition code.    
-00002200: 2020 2020 2020 2020 656c 656d 656e 745f          element_
-00002210: 7661 6c75 6573 3a20 456c 656d 656e 7420  values: Element 
-00002220: 7661 6c75 6573 0a20 2020 2020 2020 204e  values.        N
-00002230: 2905 7214 0000 0072 1500 0000 7209 0000  ).r....r....r...
-00002240: 0072 5200 0000 7253 0000 0029 0572 1700  .rR...rS...).r..
-00002250: 0000 7209 0000 0072 5200 0000 7253 0000  ..r....rR...rS..
-00002260: 0072 1000 0000 7218 0000 0072 1a00 0000  .r....r....r....
-00002270: 721b 0000 0072 1500 0000 0e01 0000 7308  r....r........s.
-00002280: 0000 0000 0d0e 0106 0106 017a 2253 6176  ...........z"Sav
-00002290: 6550 726f 6365 7373 456c 656d 656e 7452  eProcessElementR
-000022a0: 6571 7565 7374 2e5f 5f69 6e69 745f 5f29  equest.__init__)
-000022b0: 014e 290c 721d 0000 0072 1e00 0000 721f  .N).r....r....r.
-000022c0: 0000 0072 2000 0000 720b 0000 0072 0500  ...r ...r....r..
-000022d0: 0000 7204 0000 0072 3800 0000 da13 5072  ..r....r8.....Pr
-000022e0: 6f63 6573 7345 6c65 6d65 6e74 5661 6c75  ocessElementValu
-000022f0: 6572 0200 0000 7215 0000 0072 2100 0000  er....r....r!...
-00002300: 721a 0000 0072 1a00 0000 7218 0000 0072  r....r....r....r
-00002310: 1b00 0000 724f 0000 0007 0100 0073 1800  ....rO.......s..
-00002320: 0000 0802 0801 0801 08fd 060a 00fc 0202  ................
-00002330: 0201 0201 0c01 0201 02fa 724f 0000 0063  ..........rO...c
-00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002350: 0400 0000 0000 0000 7336 0000 0065 005a  ........s6...e.Z
-00002360: 0164 005a 0264 0164 0164 0264 039c 0269  .d.Z.d.d.d.d...i
-00002370: 015a 0365 046a 0565 0664 0464 059c 0387  .Z.e.j.e.d.d....
-00002380: 0066 0164 0664 0784 0c5a 0787 0004 005a  .f.d.d...Z.....Z
-00002390: 0853 0029 08da 1a53 6176 6550 726f 6365  .S.)...SaveProce
-000023a0: 7373 456c 656d 656e 7452 6573 706f 6e73  ssElementRespons
-000023b0: 6572 4900 0000 724a 0000 0072 0c00 0000  erI...rJ...r....
-000023c0: 4e72 4b00 0000 6302 0000 0000 0000 0000  NrK...c.........
-000023d0: 0000 0003 0000 0003 0000 000b 0000 0073  ...............s
-000023e0: 1800 0000 7400 8300 6a01 6600 7c02 8e01  ....t...j.f.|...
-000023f0: 0100 7c01 7c00 5f02 6401 5300 a902 7a42  ..|.|._.d.S...zB
-00002400: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00002410: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00002420: 2070 726f 6365 7373 3a20 5072 6f63 6573   process: Proces
-00002430: 7320 7570 6461 7465 640a 2020 2020 2020  s updated.      
-00002440: 2020 4e72 4c00 0000 724d 0000 0072 1800    NrL...rM...r..
-00002450: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
-00002460: 0026 0100 0073 0400 0000 0005 0e01 7a23  .&...s........z#
-00002470: 5361 7665 5072 6f63 6573 7345 6c65 6d65  SaveProcessEleme
-00002480: 6e74 5265 7370 6f6e 7365 2e5f 5f69 6e69  ntResponse.__ini
-00002490: 745f 5f72 4e00 0000 721a 0000 0072 1a00  t__rN...r....r..
-000024a0: 0000 7218 0000 0072 1b00 0000 7255 0000  ..r....r....rU..
-000024b0: 0021 0100 0073 0800 0000 0802 0200 08ff  .!...s..........
-000024c0: 0404 7255 0000 0063 0000 0000 0000 0000  ..rU...c........
-000024d0: 0000 0000 0000 0000 0500 0000 0000 0000  ................
-000024e0: 733e 0000 0065 005a 0164 005a 0264 0164  s>...e.Z.d.Z.d.d
-000024f0: 0264 039c 0264 0464 0264 039c 0264 059c  .d...d.d.d...d..
-00002500: 025a 0365 0465 0465 0564 0664 079c 0487  .Z.e.e.e.d.d....
-00002510: 0066 0164 0864 0984 0c5a 0687 0004 005a  .f.d.d...Z.....Z
-00002520: 0753 0029 0ada 1b44 656c 6574 6550 726f  .S.)...DeletePro
-00002530: 6365 7373 456c 656d 656e 7452 6571 7565  cessElementReque
-00002540: 7374 720a 0000 0072 0b00 0000 720c 0000  str....r....r...
-00002550: 0072 5000 0000 2902 7209 0000 0072 5200  .rP...).r....rR.
-00002560: 0000 4e29 0472 0900 0000 7252 0000 0072  ..N).r....rR...r
-00002570: 1000 0000 7211 0000 0063 0300 0000 0000  ....r....c......
-00002580: 0000 0000 0000 0400 0000 0300 0000 0b00  ................
-00002590: 0000 731e 0000 0074 0083 006a 0166 007c  ..s....t...j.f.|
-000025a0: 038e 0101 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
-000025b0: 0364 0153 0029 027a 880a 2020 2020 2020  .d.S.).z..      
-000025c0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
-000025d0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
-000025e0: 735f 6964 3a20 5072 6f63 6573 7320 7265  s_id: Process re
-000025f0: 6c61 7465 640a 2020 2020 2020 2020 2020  lated.          
-00002600: 2020 656c 656d 656e 745f 6465 6669 6e69    element_defini
-00002610: 7469 6f6e 5f63 6f64 653a 2043 6f64 6520  tion_code: Code 
-00002620: 6f66 2074 6865 2065 6c65 6d65 6e74 2074  of the element t
-00002630: 6f20 6465 6c65 7465 0a20 2020 2020 2020  o delete.       
-00002640: 204e 2904 7214 0000 0072 1500 0000 7209   N).r....r....r.
-00002650: 0000 0072 5200 0000 2904 7217 0000 0072  ...rR...).r....r
-00002660: 0900 0000 7252 0000 0072 1000 0000 7218  ....rR...r....r.
-00002670: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
-00002680: 0000 3501 0000 7306 0000 0000 060e 0106  ..5...s.........
-00002690: 017a 2444 656c 6574 6550 726f 6365 7373  .z$DeleteProcess
-000026a0: 456c 656d 656e 7452 6571 7565 7374 2e5f  ElementRequest._
-000026b0: 5f69 6e69 745f 5f72 1c00 0000 721a 0000  _init__r....r...
-000026c0: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
-000026d0: 7257 0000 002f 0100 0073 0800 0000 0802  rW.../...s......
-000026e0: 0801 08fe 0605 7257 0000 0063 0000 0000  ......rW...c....
-000026f0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00002700: 0000 0000 7336 0000 0065 005a 0164 005a  ....s6...e.Z.d.Z
-00002710: 0264 0164 0164 0264 039c 0269 015a 0365  .d.d.d.d...i.Z.e
-00002720: 046a 0565 0664 0464 059c 0387 0066 0164  .j.e.d.d.....f.d
-00002730: 0664 0784 0c5a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
-00002740: 08da 1c44 656c 6574 6550 726f 6365 7373  ...DeleteProcess
-00002750: 456c 656d 656e 7452 6573 706f 6e73 6572  ElementResponser
-00002760: 4900 0000 724a 0000 0072 0c00 0000 4e72  I...rJ...r....Nr
-00002770: 4b00 0000 6302 0000 0000 0000 0000 0000  K...c...........
-00002780: 0003 0000 0003 0000 000b 0000 0073 1800  .............s..
-00002790: 0000 7400 8300 6a01 6600 7c02 8e01 0100  ..t...j.f.|.....
-000027a0: 7c01 7c00 5f02 6401 5300 7256 0000 0072  |.|._.d.S.rV...r
-000027b0: 4c00 0000 724d 0000 0072 1800 0000 721a  L...rM...r....r.
-000027c0: 0000 0072 1b00 0000 7215 0000 0045 0100  ...r....r....E..
-000027d0: 0073 0400 0000 0005 0e01 7a25 4465 6c65  .s........z%Dele
-000027e0: 7465 5072 6f63 6573 7345 6c65 6d65 6e74  teProcessElement
-000027f0: 5265 7370 6f6e 7365 2e5f 5f69 6e69 745f  Response.__init_
-00002800: 5f72 4e00 0000 721a 0000 0072 1a00 0000  _rN...r....r....
-00002810: 7218 0000 0072 1b00 0000 7258 0000 0040  r....r....rX...@
-00002820: 0100 0073 0800 0000 0802 0200 08ff 0404  ...s............
-00002830: 7258 0000 0063 0000 0000 0000 0000 0000  rX...c..........
-00002840: 0000 0000 0000 0700 0000 0000 0000 7352  ..............sR
-00002850: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00002860: 039c 0264 0464 0264 039c 0264 0564 0264  ...d.d.d...d.d.d
-00002870: 039c 0264 069c 035a 0364 0b65 0465 0565  ...d...Z.d.e.e.e
-00002880: 0419 0065 0565 0419 0065 0664 0764 089c  ...e.e...e.d.d..
-00002890: 0587 0066 0164 0964 0a84 0d5a 0787 0004  ...f.d.d...Z....
-000028a0: 005a 0853 0029 0cda 1d43 6861 6e67 6550  .Z.S.)...ChangeP
-000028b0: 726f 6365 7373 496e 6974 6961 746f 7252  rocessInitiatorR
-000028c0: 6571 7565 7374 720a 0000 0072 0b00 0000  equestr....r....
-000028d0: 720c 0000 00da 0565 6d61 696c 7234 0000  r......emailr4..
-000028e0: 0029 0372 0900 0000 725a 0000 0072 3300  .).r....rZ...r3.
-000028f0: 0000 4e29 0572 0900 0000 725a 0000 0072  ..N).r....rZ...r
-00002900: 3300 0000 7210 0000 0072 1100 0000 6304  3...r....r....c.
-00002910: 0000 0000 0000 0000 0000 0005 0000 0003  ................
-00002920: 0000 000b 0000 0073 2400 0000 7400 8300  .......s$...t...
-00002930: 6a01 6600 7c04 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-00002940: 7c02 7c00 5f03 7c03 7c00 5f04 6401 5300  |.|._.|.|._.d.S.
-00002950: 2902 617b 0100 000a 2020 2020 2020 2020  ).a{....        
-00002960: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-00002970: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
-00002980: 6964 3a20 5072 6f63 6573 7320 6964 656e  id: Process iden
-00002990: 7469 6669 6572 2074 6f20 7768 6963 6820  tifier to which 
-000029a0: 7761 6e74 2074 6f20 6368 616e 6765 2074  want to change t
-000029b0: 6865 2069 6e69 7469 6174 6f72 0a20 2020  he initiator.   
-000029c0: 2020 2020 2020 2020 2065 6d61 696c 3a20           email: 
-000029d0: 5573 6572 2065 6d61 696c 2074 6861 7420  User email that 
-000029e0: 7761 6e74 2074 6f20 7573 6520 746f 2061  want to use to a
-000029f0: 7373 6967 6e20 7468 6520 7072 6f63 6573  ssign the proces
-00002a00: 732e 2041 7474 7269 6275 7465 203a 656d  s. Attribute :em
-00002a10: 6169 6c20 6f72 203a 7072 696e 6369 7061  ail or :principa
-00002a20: 6c5f 6964 206d 7573 7420 6265 2073 6574  l_id must be set
-00002a30: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00002a40: 696e 6369 7061 6c5f 6964 3a20 5072 696e  incipal_id: Prin
-00002a50: 6369 7061 6c20 6964 2074 6861 7420 7761  cipal id that wa
-00002a60: 6e74 2074 6f20 7573 6520 746f 2061 7373  nt to use to ass
-00002a70: 6967 6e20 7468 6520 7072 6f63 6573 732e  ign the process.
-00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a90: 2020 2020 2020 2020 2020 2041 7474 7269             Attri
-00002aa0: 6275 7465 203a 656d 6169 6c20 6f72 203a  bute :email or :
-00002ab0: 7072 696e 6369 7061 6c5f 6964 206d 7573  principal_id mus
-00002ac0: 7420 6265 2073 6574 2e0a 2020 2020 2020  t be set..      
-00002ad0: 2020 4e29 0572 1400 0000 7215 0000 0072    N).r....r....r
-00002ae0: 0900 0000 725a 0000 0072 3300 0000 2905  ....rZ...r3...).
-00002af0: 7217 0000 0072 0900 0000 725a 0000 0072  r....r....rZ...r
-00002b00: 3300 0000 7210 0000 0072 1800 0000 721a  3...r....r....r.
-00002b10: 0000 0072 1b00 0000 7215 0000 0055 0100  ...r....r....U..
-00002b20: 0073 0800 0000 000a 0e01 0601 0601 7a26  .s............z&
-00002b30: 4368 616e 6765 5072 6f63 6573 7349 6e69  ChangeProcessIni
-00002b40: 7469 6174 6f72 5265 7175 6573 742e 5f5f  tiatorRequest.__
-00002b50: 696e 6974 5f5f 2902 4e4e a909 721d 0000  init__).NN..r...
-00002b60: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00002b70: 720b 0000 0072 0500 0000 7202 0000 0072  r....r....r....r
-00002b80: 1500 0000 7221 0000 0072 1a00 0000 721a  ....r!...r....r.
-00002b90: 0000 0072 1800 0000 721b 0000 0072 5900  ...r....r....rY.
-00002ba0: 0000 4e01 0000 731a 0000 0008 0208 0108  ..N...s.........
-00002bb0: 0108 fd06 0700 0000 ff02 0102 0006 0006  ................
-00002bc0: 0002 0102 fe72 5900 0000 6300 0000 0000  .....rY...c.....
-00002bd0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-00002be0: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
-00002bf0: 6401 6401 6402 6403 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
-00002c00: 6a05 6506 6404 6405 9c03 8700 6601 6406  j.e.d.d.....f.d.
-00002c10: 6407 840c 5a07 8700 0400 5a08 5300 2908  d...Z.....Z.S.).
-00002c20: da1e 4368 616e 6765 5072 6f63 6573 7349  ..ChangeProcessI
-00002c30: 6e69 7469 6174 6f72 5265 7370 6f6e 7365  nitiatorResponse
-00002c40: 7249 0000 0072 4a00 0000 720c 0000 004e  rI...rJ...r....N
-00002c50: 724b 0000 0063 0200 0000 0000 0000 0000  rK...c..........
-00002c60: 0000 0300 0000 0300 0000 0b00 0000 7318  ..............s.
-00002c70: 0000 0074 0083 006a 0166 007c 028e 0101  ...t...j.f.|....
-00002c80: 007c 017c 005f 0264 0153 0072 5600 0000  .|.|._.d.S.rV...
-00002c90: 724c 0000 0072 4d00 0000 7218 0000 0072  rL...rM...r....r
-00002ca0: 1a00 0000 721b 0000 0072 1500 0000 6a01  ....r....r....j.
-00002cb0: 0000 7304 0000 0000 050e 017a 2743 6861  ..s........z'Cha
-00002cc0: 6e67 6550 726f 6365 7373 496e 6974 6961  ngeProcessInitia
-00002cd0: 746f 7252 6573 706f 6e73 652e 5f5f 696e  torResponse.__in
-00002ce0: 6974 5f5f 724e 0000 0072 1a00 0000 721a  it__rN...r....r.
-00002cf0: 0000 0072 1800 0000 721b 0000 0072 5c00  ...r....r....r\.
-00002d00: 0000 6501 0000 7308 0000 0008 0202 0008  ..e...s.........
-00002d10: ff04 0472 5c00 0000 6300 0000 0000 0000  ...r\...c.......
-00002d20: 0000 0000 0000 0000 000a 0000 0000 0000  ................
-00002d30: 0073 9200 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00002d40: 6402 6403 9c02 6404 6402 6403 9c02 6405  d.d...d.d.d...d.
-00002d50: 6406 6403 9c02 6407 6406 6403 9c02 6408  d.d...d.d.d...d.
-00002d60: 6409 6403 9c02 640a 6406 6403 9c02 640b  d.d...d.d.d...d.
-00002d70: 9c06 5a03 6410 6504 6505 1900 6504 6505  ..Z.d.e.e...e.e.
-00002d80: 1900 6504 6506 6507 1900 1900 6504 6506  ..e.e.e.....e.e.
-00002d90: 6507 1900 1900 6504 6506 6508 6a09 1900  e.....e.e.e.j...
-00002da0: 1900 6504 6506 6507 1900 1900 650a 640c  ..e.e.e.....e.d.
-00002db0: 640d 9c08 8700 6601 640e 640f 840d 5a0b  d.....f.d.d...Z.
-00002dc0: 8700 0400 5a0c 5300 2911 da0f 4669 6e64  ....Z.S.)...Find
-00002dd0: 5461 736b 5265 7175 6573 7472 3f00 0000  TaskRequestr?...
-00002de0: 7240 0000 0072 0c00 0000 7241 0000 0072  r@...r....rA...r
-00002df0: 4200 0000 7243 0000 005a 0a70 726f 6365  B...rC...Z.proce
-00002e00: 7373 4964 73da 0673 7461 7465 737a 0b5b  ssIds..statesz.[
-00002e10: 5461 736b 5374 6174 655d 5a13 7461 736b  TaskState]Z.task
-00002e20: 4465 6669 6e69 7469 6f6e 436f 6465 7329  DefinitionCodes)
-00002e30: 0672 3f00 0000 7241 0000 0072 4200 0000  .r?...rA...rB...
-00002e40: da0b 7072 6f63 6573 735f 6964 7372 5e00  ..process_idsr^.
-00002e50: 0000 da15 7461 736b 5f64 6566 696e 6974  ....task_definit
-00002e60: 696f 6e5f 636f 6465 734e 2908 723f 0000  ion_codesN).r?..
-00002e70: 0072 4100 0000 7242 0000 0072 5f00 0000  .rA...rB...r_...
-00002e80: 725e 0000 0072 6000 0000 7210 0000 0072  r^...r`...r....r
-00002e90: 1100 0000 6307 0000 0000 0000 0000 0000  ....c...........
-00002ea0: 0008 0000 0003 0000 000b 0000 0073 3600  .............s6.
-00002eb0: 0000 7400 8300 6a01 6600 7c07 8e01 0100  ..t...j.f.|.....
-00002ec0: 7c01 7c00 5f02 7c02 7c00 5f03 7c03 7c00  |.|._.|.|._.|.|.
-00002ed0: 5f04 7c04 7c00 5f05 7c05 7c00 5f06 7c06  _.|.|._.|.|._.|.
-00002ee0: 7c00 5f07 6401 5300 2902 617b 0100 000a  |._.d.S.).a{....
-00002ef0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00002f00: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00002f10: 7061 6765 3a20 5061 6765 2072 6571 7565  page: Page reque
-00002f20: 7374 6564 2c20 302d 696e 6465 780a 2020  sted, 0-index.  
-00002f30: 2020 2020 2020 2020 2020 7369 7a65 3a20            size: 
-00002f40: 5061 6765 2073 697a 650a 2020 2020 2020  Page size.      
-00002f50: 2020 2020 2020 736f 7274 733a 2053 6f72        sorts: Sor
-00002f60: 7469 6e67 2063 7269 7465 7269 6120 696e  ting criteria in
-00002f70: 2074 6865 2066 6f72 6d61 743a 2070 726f   the format: pro
-00002f80: 7065 7274 797b 2c61 7363 7c64 6573 637d  perty{,asc|desc}
-00002f90: 2e20 4578 616d 706c 653a 206e 616d 652c  . Example: name,
-00002fa0: 6465 7363 0a20 2020 2020 2020 2020 2020  desc.           
-00002fb0: 2070 726f 6365 7373 5f69 6473 3a20 4669   process_ids: Fi
-00002fc0: 6c74 6572 2074 6173 6b73 2062 7920 7468  lter tasks by th
-00002fd0: 6520 7072 6f63 6573 7320 6964 656e 7469  e process identi
-00002fe0: 6669 6572 730a 2020 2020 2020 2020 2020  fiers.          
-00002ff0: 2020 7374 6174 6573 3a20 4669 6c74 6572    states: Filter
-00003000: 2074 6173 6b73 2062 7920 7468 6520 7374   tasks by the st
-00003010: 6174 6573 0a20 2020 2020 2020 2020 2020  ates.           
-00003020: 2074 6173 6b5f 6465 6669 6e69 7469 6f6e   task_definition
-00003030: 5f63 6f64 6573 3a20 4669 6c74 6572 2074  _codes: Filter t
-00003040: 6173 6b73 2062 7920 7468 6520 7461 736b  asks by the task
-00003050: 5f64 6566 696e 6974 696f 6e5f 636f 6465  _definition_code
-00003060: 730a 2020 2020 2020 2020 4e29 0872 1400  s.        N).r..
-00003070: 0000 7215 0000 0072 3f00 0000 7241 0000  ..r....r?...rA..
-00003080: 0072 4200 0000 725f 0000 0072 5e00 0000  .rB...r_...r^...
-00003090: 7260 0000 0029 0872 1700 0000 723f 0000  r`...).r....r?..
-000030a0: 0072 4100 0000 7242 0000 0072 5f00 0000  .rA...rB...r_...
-000030b0: 725e 0000 0072 6000 0000 7210 0000 0072  r^...r`...r....r
-000030c0: 1800 0000 721a 0000 0072 1b00 0000 7215  ....r....r....r.
-000030d0: 0000 007d 0100 0073 0e00 0000 0013 0e01  ...}...s........
-000030e0: 0601 0601 0601 0601 0601 7a18 4669 6e64  ..........z.Find
-000030f0: 5461 736b 5265 7175 6573 742e 5f5f 696e  TaskRequest.__in
-00003100: 6974 5f5f 2906 4e4e 4e4e 4e4e 290d 721d  it__).NNNNNN).r.
-00003110: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
-00003120: 0000 7205 0000 0072 4000 0000 7204 0000  ..r....r@...r...
-00003130: 0072 0b00 0000 7238 0000 00da 0954 6173  .r....r8.....Tas
-00003140: 6b53 7461 7465 7202 0000 0072 1500 0000  kStater....r....
-00003150: 7221 0000 0072 1a00 0000 721a 0000 0072  r!...r....r....r
-00003160: 1800 0000 721b 0000 0072 5d00 0000 7301  ....r....r]...s.
-00003170: 0000 732e 0000 0008 0208 0108 0108 0108  ..s.............
-00003180: 0108 0108 fa06 0b00 0100 0100 0100 0100  ................
-00003190: 0100 f902 0206 0106 010a 010a 010c 010a  ................
-000031a0: 0102 0102 f772 5d00 0000 6300 0000 0000  .....r]...c.....
-000031b0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
-000031c0: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
-000031d0: 6401 6401 6402 6403 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
-000031e0: 6a05 6506 6404 6405 9c03 8700 6601 6406  j.e.d.d.....f.d.
-000031f0: 6407 840c 5a07 8700 0400 5a08 5300 2908  d...Z.....Z.S.).
-00003200: da10 4669 6e64 5461 736b 5265 7370 6f6e  ..FindTaskRespon
-00003210: 7365 da05 7461 736b 73da 0854 6173 6b50  se..tasks..TaskP
-00003220: 6167 6572 0c00 0000 4e29 0372 6300 0000  ager....N).rc...
-00003230: 7210 0000 0072 1100 0000 6302 0000 0000  r....r....c.....
-00003240: 0000 0000 0000 0003 0000 0003 0000 000b  ................
-00003250: 0000 0073 1800 0000 7400 8300 6a01 6600  ...s....t...j.f.
-00003260: 7c02 8e01 0100 7c01 7c00 5f02 6401 5300  |.....|.|._.d.S.
-00003270: 2902 7a5b 0a20 2020 2020 2020 2050 6172  ).z[.        Par
-00003280: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00003290: 2020 2020 2074 6173 6b73 3a20 5461 736b       tasks: Task
-000032a0: 2070 6167 6520 7468 6174 206d 6174 6820   page that math 
-000032b0: 7468 6520 7265 7175 6573 7465 6420 6372  the requested cr
-000032c0: 6974 6572 6961 0a20 2020 2020 2020 204e  iteria.        N
-000032d0: 2903 7214 0000 0072 1500 0000 7263 0000  ).r....r....rc..
-000032e0: 0029 0372 1700 0000 7263 0000 0072 1000  .).r....rc...r..
-000032f0: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00003300: 0072 1500 0000 9e01 0000 7304 0000 0000  .r........s.....
-00003310: 050e 017a 1946 696e 6454 6173 6b52 6573  ...z.FindTaskRes
-00003320: 706f 6e73 652e 5f5f 696e 6974 5f5f 2909  ponse.__init__).
-00003330: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00003340: 2000 0000 7238 0000 0072 6400 0000 7202   ...r8...rd...r.
-00003350: 0000 0072 1500 0000 7221 0000 0072 1a00  ...r....r!...r..
-00003360: 0000 721a 0000 0072 1800 0000 721b 0000  ..r....r....r...
-00003370: 0072 6200 0000 9901 0000 7308 0000 0008  .rb.......s.....
-00003380: 0202 0008 ff04 0472 6200 0000 6300 0000  .......rb...c...
-00003390: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-000033a0: 0000 0000 0073 3400 0000 6500 5a01 6400  .....s4...e.Z.d.
-000033b0: 5a02 6401 6402 6403 6404 9c02 6901 5a03  Z.d.d.d.d...i.Z.
-000033c0: 6504 6505 6405 6406 9c03 8700 6601 6407  e.e.d.d.....f.d.
-000033d0: 6408 840c 5a06 8700 0400 5a07 5300 2909  d...Z.....Z.S.).
-000033e0: da13 5265 7472 6965 7665 5461 736b 5265  ..RetrieveTaskRe
-000033f0: 7175 6573 7472 3000 0000 722f 0000 0072  questr0...r/...r
-00003400: 0b00 0000 720c 0000 004e a903 7230 0000  ....r....N..r0..
-00003410: 0072 1000 0000 7211 0000 0063 0200 0000  .r....r....c....
-00003420: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00003430: 0b00 0000 7318 0000 0074 0083 006a 0166  ....s....t...j.f
-00003440: 007c 028e 0101 007c 017c 005f 0264 0153  .|.....|.|._.d.S
-00003450: 0029 027a 4e0a 2020 2020 2020 2020 5061  .).zN.        Pa
-00003460: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00003470: 2020 2020 2020 7461 736b 5f69 643a 2054        task_id: T
-00003480: 6173 6b20 6964 656e 7469 6669 6572 2074  ask identifier t
-00003490: 6f20 7265 7472 6965 7665 0a20 2020 2020  o retrieve.     
-000034a0: 2020 204e a903 7214 0000 0072 1500 0000     N..r....r....
-000034b0: 7230 0000 00a9 0372 1700 0000 7230 0000  r0.....r....r0..
-000034c0: 0072 1000 0000 7218 0000 0072 1a00 0000  .r....r....r....
-000034d0: 721b 0000 0072 1500 0000 ac01 0000 7304  r....r........s.
-000034e0: 0000 0000 050e 017a 1c52 6574 7269 6576  .......z.Retriev
-000034f0: 6554 6173 6b52 6571 7565 7374 2e5f 5f69  eTaskRequest.__i
-00003500: 6e69 745f 5f72 1c00 0000 721a 0000 0072  nit__r....r....r
-00003510: 1a00 0000 7218 0000 0072 1b00 0000 7265  ....r....r....re
-00003520: 0000 00a7 0100 0073 0800 0000 0802 0200  .......s........
-00003530: 08ff 0404 7265 0000 0063 0000 0000 0000  ....re...c......
-00003540: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00003550: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
-00003560: 0164 0164 0264 039c 0269 015a 0365 046a  .d.d.d...i.Z.e.j
-00003570: 0565 0664 0464 059c 0387 0066 0164 0664  .e.d.d.....f.d.d
-00003580: 0784 0c5a 0787 0004 005a 0853 0029 08da  ...Z.....Z.S.)..
-00003590: 1452 6574 7269 6576 6554 6173 6b52 6573  .RetrieveTaskRes
-000035a0: 706f 6e73 65da 0474 6173 6bda 0454 6173  ponse..task..Tas
-000035b0: 6b72 0c00 0000 4ea9 0372 6a00 0000 7210  kr....N..rj...r.
-000035c0: 0000 0072 1100 0000 6302 0000 0000 0000  ...r....c.......
-000035d0: 0000 0000 0003 0000 0003 0000 000b 0000  ................
-000035e0: 0073 1800 0000 7400 8300 6a01 6600 7c02  .s....t...j.f.|.
-000035f0: 8e01 0100 7c01 7c00 5f02 6401 5300 2902  ....|.|._.d.S.).
-00003600: 7a39 0a20 2020 2020 2020 2050 6172 616d  z9.        Param
-00003610: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
-00003620: 2020 2074 6173 6b3a 2054 6173 6b20 6461     task: Task da
-00003630: 7461 0a20 2020 2020 2020 204e a903 7214  ta.        N..r.
-00003640: 0000 0072 1500 0000 726a 0000 00a9 0372  ...r....rj.....r
-00003650: 1700 0000 726a 0000 0072 1000 0000 7218  ....rj...r....r.
-00003660: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
-00003670: 0000 ba01 0000 7304 0000 0000 050e 017a  ......s........z
-00003680: 1d52 6574 7269 6576 6554 6173 6b52 6573  .RetrieveTaskRes
-00003690: 706f 6e73 652e 5f5f 696e 6974 5f5f a909  ponse.__init__..
-000036a0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000036b0: 2000 0000 7238 0000 0072 6b00 0000 7202   ...r8...rk...r.
-000036c0: 0000 0072 1500 0000 7221 0000 0072 1a00  ...r....r!...r..
-000036d0: 0000 721a 0000 0072 1800 0000 721b 0000  ..r....r....r...
-000036e0: 0072 6900 0000 b501 0000 7308 0000 0008  .ri.......s.....
-000036f0: 0202 0008 ff04 0472 6900 0000 6300 0000  .......ri...c...
-00003700: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00003710: 0000 0000 0073 3600 0000 6500 5a01 6400  .....s6...e.Z.d.
-00003720: 5a02 6401 6401 6402 6403 9c02 6901 5a03  Z.d.d.d.d...i.Z.
-00003730: 6504 6a05 6506 6404 6405 9c03 8700 6601  e.j.e.d.d.....f.
-00003740: 6406 6407 840c 5a07 8700 0400 5a08 5300  d.d...Z.....Z.S.
-00003750: 2908 da11 4372 6561 7465 5461 736b 5265  )...CreateTaskRe
-00003760: 7175 6573 7472 6a00 0000 726b 0000 0072  questrj...rk...r
-00003770: 0c00 0000 4e72 6c00 0000 6302 0000 0000  ....Nrl...c.....
-00003780: 0000 0000 0000 0003 0000 0003 0000 000b  ................
-00003790: 0000 0073 1800 0000 7400 8300 6a01 6600  ...s....t...j.f.
-000037a0: 7c02 8e01 0100 7c01 7c00 5f02 6401 5300  |.....|.|._.d.S.
-000037b0: 2902 7a3e 0a20 2020 2020 2020 2050 6172  ).z>.        Par
-000037c0: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-000037d0: 2020 2020 2074 6173 6b3a 2054 6173 6b20       task: Task 
-000037e0: 746f 2063 7265 6174 650a 2020 2020 2020  to create.      
-000037f0: 2020 4e72 6d00 0000 726e 0000 0072 1800    Nrm...rn...r..
-00003800: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
-00003810: 00c8 0100 0073 0400 0000 0005 0e01 7a1a  .....s........z.
-00003820: 4372 6561 7465 5461 736b 5265 7175 6573  CreateTaskReques
-00003830: 742e 5f5f 696e 6974 5f5f 726f 0000 0072  t.__init__ro...r
-00003840: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
-00003850: 0000 0072 7000 0000 c301 0000 7308 0000  ...rp.......s...
-00003860: 0008 0202 0008 ff04 0472 7000 0000 6300  .........rp...c.
-00003870: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00003880: 0000 0000 0000 0073 3600 0000 6500 5a01  .......s6...e.Z.
-00003890: 6400 5a02 6401 6401 6402 6403 9c02 6901  d.Z.d.d.d.d...i.
-000038a0: 5a03 6504 6a05 6506 6404 6405 9c03 8700  Z.e.j.e.d.d.....
-000038b0: 6601 6406 6407 840c 5a07 8700 0400 5a08  f.d.d...Z.....Z.
-000038c0: 5300 2908 da12 4372 6561 7465 5461 736b  S.)...CreateTask
-000038d0: 5265 7370 6f6e 7365 726a 0000 0072 6b00  Responserj...rk.
-000038e0: 0000 720c 0000 004e 726c 0000 0063 0200  ..r....Nrl...c..
-000038f0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00003900: 0000 0b00 0000 7318 0000 0074 0083 006a  ......s....t...j
-00003910: 0166 007c 028e 0101 007c 017c 005f 0264  .f.|.....|.|._.d
-00003920: 0153 0029 027a 3c0a 2020 2020 2020 2020  .S.).z<.        
-00003930: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-00003940: 2020 2020 2020 2020 7461 736b 3a20 5461          task: Ta
-00003950: 736b 2063 7265 6174 6564 0a20 2020 2020  sk created.     
-00003960: 2020 204e 726d 0000 0072 6e00 0000 7218     Nrm...rn...r.
-00003970: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
-00003980: 0000 d601 0000 7304 0000 0000 050e 017a  ......s........z
-00003990: 1b43 7265 6174 6554 6173 6b52 6573 706f  .CreateTaskRespo
-000039a0: 6e73 652e 5f5f 696e 6974 5f5f 726f 0000  nse.__init__ro..
-000039b0: 0072 1a00 0000 721a 0000 0072 1800 0000  .r....r....r....
-000039c0: 721b 0000 0072 7100 0000 d101 0000 7308  r....rq.......s.
-000039d0: 0000 0008 0202 0008 ff04 0472 7100 0000  ...........rq...
-000039e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000039f0: 0004 0000 0000 0000 0073 3400 0000 6500  .........s4...e.
-00003a00: 5a01 6400 5a02 6401 6402 6403 6404 9c02  Z.d.Z.d.d.d.d...
-00003a10: 6901 5a03 6504 6505 6405 6406 9c03 8700  i.Z.e.e.d.d.....
-00003a20: 6601 6407 6408 840c 5a06 8700 0400 5a07  f.d.d...Z.....Z.
-00003a30: 5300 2909 da13 436f 6d70 6c65 7465 5461  S.)...CompleteTa
-00003a40: 736b 5265 7175 6573 7472 3000 0000 722f  skRequestr0...r/
-00003a50: 0000 0072 0b00 0000 720c 0000 004e 7266  ...r....r....Nrf
-00003a60: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00003a70: 0300 0000 0300 0000 0b00 0000 7318 0000  ............s...
-00003a80: 0074 0083 006a 0166 007c 028e 0101 007c  .t...j.f.|.....|
-00003a90: 017c 005f 0264 0153 0029 027a 570a 2020  .|._.d.S.).zW.  
-00003aa0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00003ab0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00003ac0: 736b 5f69 643a 2054 6173 6b20 6964 656e  sk_id: Task iden
-00003ad0: 7469 6669 6572 2074 6f20 6d61 726b 2061  tifier to mark a
-00003ae0: 7320 636f 6d70 6c65 7465 640a 2020 2020  s completed.    
-00003af0: 2020 2020 4e72 6700 0000 7268 0000 0072      Nrg...rh...r
-00003b00: 1800 0000 721a 0000 0072 1b00 0000 7215  ....r....r....r.
-00003b10: 0000 00e4 0100 0073 0400 0000 0005 0e01  .......s........
-00003b20: 7a1c 436f 6d70 6c65 7465 5461 736b 5265  z.CompleteTaskRe
-00003b30: 7175 6573 742e 5f5f 696e 6974 5f5f 721c  quest.__init__r.
-00003b40: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
-00003b50: 0000 721b 0000 0072 7200 0000 df01 0000  ..r....rr.......
-00003b60: 7308 0000 0008 0202 0008 ff04 0472 7200  s............rr.
-00003b70: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00003b80: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
-00003b90: 6500 5a01 6400 5a02 6401 6401 6402 6403  e.Z.d.Z.d.d.d.d.
-00003ba0: 9c02 6901 5a03 6504 6a05 6506 6404 6405  ..i.Z.e.j.e.d.d.
-00003bb0: 9c03 8700 6601 6406 6407 840c 5a07 8700  ....f.d.d...Z...
-00003bc0: 0400 5a08 5300 2908 da14 436f 6d70 6c65  ..Z.S.)...Comple
-00003bd0: 7465 5461 736b 5265 7370 6f6e 7365 726a  teTaskResponserj
-00003be0: 0000 0072 6b00 0000 720c 0000 004e 726c  ...rk...r....Nrl
-00003bf0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00003c00: 0300 0000 0300 0000 0b00 0000 7318 0000  ............s...
-00003c10: 0074 0083 006a 0166 007c 028e 0101 007c  .t...j.f.|.....|
-00003c20: 017c 005f 0264 0153 00a9 027a 3c0a 2020  .|._.d.S...z<.  
-00003c30: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00003c40: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00003c50: 736b 3a20 5461 736b 2075 7064 6174 6564  sk: Task updated
-00003c60: 0a20 2020 2020 2020 204e 726d 0000 0072  .        Nrm...r
-00003c70: 6e00 0000 7218 0000 0072 1a00 0000 721b  n...r....r....r.
-00003c80: 0000 0072 1500 0000 f201 0000 7304 0000  ...r........s...
-00003c90: 0000 050e 017a 1d43 6f6d 706c 6574 6554  .....z.CompleteT
-00003ca0: 6173 6b52 6573 706f 6e73 652e 5f5f 696e  askResponse.__in
-00003cb0: 6974 5f5f 726f 0000 0072 1a00 0000 721a  it__ro...r....r.
-00003cc0: 0000 0072 1800 0000 721b 0000 0072 7300  ...r....r....rs.
-00003cd0: 0000 ed01 0000 7308 0000 0008 0202 0008  ......s.........
-00003ce0: ff04 0472 7300 0000 6300 0000 0000 0000  ...rs...c.......
-00003cf0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-00003d00: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
-00003d10: 6402 6403 6404 9c02 6901 5a03 6504 6505  d.d.d...i.Z.e.e.
-00003d20: 6405 6406 9c03 8700 6601 6407 6408 840c  d.d.....f.d.d...
-00003d30: 5a06 8700 0400 5a07 5300 2909 da10 436c  Z.....Z.S.)...Cl
-00003d40: 6169 6d54 6173 6b52 6571 7565 7374 7230  aimTaskRequestr0
-00003d50: 0000 0072 2f00 0000 720b 0000 0072 0c00  ...r/...r....r..
-00003d60: 0000 4e72 6600 0000 6302 0000 0000 0000  ..Nrf...c.......
-00003d70: 0000 0000 0003 0000 0003 0000 000b 0000  ................
-00003d80: 0073 1800 0000 7400 8300 6a01 6600 7c02  .s....t...j.f.|.
-00003d90: 8e01 0100 7c01 7c00 5f02 6401 5300 2902  ....|.|._.d.S.).
-00003da0: 7a5c 0a20 2020 2020 2020 2050 6172 616d  z\.        Param
-00003db0: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
-00003dc0: 2020 2074 6173 6b5f 6964 3a20 5461 736b     task_id: Task
-00003dd0: 2069 6465 6e74 6966 6965 7220 746f 2063   identifier to c
-00003de0: 6c61 696d 2062 7920 7468 6520 7265 7175  laim by the requ
-00003df0: 6573 746f 720a 2020 2020 2020 2020 4e72  estor.        Nr
-00003e00: 6700 0000 7268 0000 0072 1800 0000 721a  g...rh...r....r.
-00003e10: 0000 0072 1b00 0000 7215 0000 0000 0200  ...r....r.......
-00003e20: 0073 0400 0000 0005 0e01 7a19 436c 6169  .s........z.Clai
-00003e30: 6d54 6173 6b52 6571 7565 7374 2e5f 5f69  mTaskRequest.__i
-00003e40: 6e69 745f 5f72 1c00 0000 721a 0000 0072  nit__r....r....r
-00003e50: 1a00 0000 7218 0000 0072 1b00 0000 7275  ....r....r....ru
-00003e60: 0000 00fb 0100 0073 0800 0000 0802 0200  .......s........
-00003e70: 08ff 0404 7275 0000 0063 0000 0000 0000  ....ru...c......
-00003e80: 0000 0000 0000 0000 0000 0400 0000 0000  ................
-00003e90: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
-00003ea0: 0164 0164 0264 039c 0269 015a 0365 046a  .d.d.d...i.Z.e.j
-00003eb0: 0565 0664 0464 059c 0387 0066 0164 0664  .e.d.d.....f.d.d
-00003ec0: 0784 0c5a 0787 0004 005a 0853 0029 08da  ...Z.....Z.S.)..
-00003ed0: 1143 6c61 696d 5461 736b 5265 7370 6f6e  .ClaimTaskRespon
-00003ee0: 7365 726a 0000 0072 6b00 0000 720c 0000  serj...rk...r...
-00003ef0: 004e 726c 0000 0063 0200 0000 0000 0000  .Nrl...c........
-00003f00: 0000 0000 0300 0000 0300 0000 0b00 0000  ................
-00003f10: 7318 0000 0074 0083 006a 0166 007c 028e  s....t...j.f.|..
-00003f20: 0101 007c 017c 005f 0264 0153 0029 027a  ...|.|._.d.S.).z
-00003f30: 3c0a 2020 2020 2020 2020 5061 7261 6d65  <.        Parame
-00003f40: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-00003f50: 2020 7461 736b 3a20 5461 736b 2063 6c61    task: Task cla
-00003f60: 696d 6564 0a20 2020 2020 2020 204e 726d  imed.        Nrm
-00003f70: 0000 0072 6e00 0000 7218 0000 0072 1a00  ...rn...r....r..
-00003f80: 0000 721b 0000 0072 1500 0000 0e02 0000  ..r....r........
-00003f90: 7304 0000 0000 050e 017a 1a43 6c61 696d  s........z.Claim
-00003fa0: 5461 736b 5265 7370 6f6e 7365 2e5f 5f69  TaskResponse.__i
-00003fb0: 6e69 745f 5f72 6f00 0000 721a 0000 0072  nit__ro...r....r
-00003fc0: 1a00 0000 7218 0000 0072 1b00 0000 7276  ....r....r....rv
-00003fd0: 0000 0009 0200 0073 0800 0000 0802 0200  .......s........
-00003fe0: 08ff 0404 7276 0000 0063 0000 0000 0000  ....rv...c......
-00003ff0: 0000 0000 0000 0000 0000 0700 0000 0000  ................
-00004000: 0000 7352 0000 0065 005a 0164 005a 0264  ..sR...e.Z.d.Z.d
-00004010: 0164 0264 039c 0264 0464 0264 039c 0264  .d.d...d.d.d...d
-00004020: 0564 0264 039c 0264 069c 035a 0364 0b65  .d.d...d...Z.d.e
-00004030: 0465 0565 0419 0065 0565 0419 0065 0664  .e.e...e.e...e.d
-00004040: 0764 089c 0587 0066 0164 0964 0a84 0d5a  .d.....f.d.d...Z
-00004050: 0787 0004 005a 0853 0029 0cda 1141 7373  .....Z.S.)...Ass
-00004060: 6967 6e54 6173 6b52 6571 7565 7374 722f  ignTaskRequestr/
-00004070: 0000 0072 0b00 0000 720c 0000 0072 5a00  ...r....r....rZ.
-00004080: 0000 7234 0000 0029 0372 3000 0000 725a  ..r4...).r0...rZ
-00004090: 0000 0072 3300 0000 4e29 0572 3000 0000  ...r3...N).r0...
-000040a0: 725a 0000 0072 3300 0000 7210 0000 0072  rZ...r3...r....r
-000040b0: 1100 0000 6304 0000 0000 0000 0000 0000  ....c...........
-000040c0: 0005 0000 0003 0000 000b 0000 0073 2400  .............s$.
-000040d0: 0000 7400 8300 6a01 6600 7c04 8e01 0100  ..t...j.f.|.....
-000040e0: 7c01 7c00 5f02 7c02 7c00 5f03 7c03 7c00  |.|._.|.|._.|.|.
-000040f0: 5f04 6401 5300 2902 6150 0100 000a 2020  _.d.S.).aP....  
-00004100: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00004110: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
-00004120: 736b 5f69 643a 2054 6173 6b20 746f 2061  sk_id: Task to a
-00004130: 7373 6967 6e20 746f 2074 6865 2065 6d61  ssign to the ema
-00004140: 696c 206f 7220 7072 696e 6369 7061 6c5f  il or principal_
-00004150: 6964 2073 656c 6563 7465 640a 2020 2020  id selected.    
-00004160: 2020 2020 2020 2020 656d 6169 6c3a 2055          email: U
-00004170: 7365 7220 656d 6169 6c20 7468 6174 2077  ser email that w
-00004180: 616e 7420 746f 2075 7365 2074 6f20 6173  ant to use to as
-00004190: 7369 676e 2074 6865 2074 6173 6b2e 2041  sign the task. A
-000041a0: 7474 7269 6275 7465 203a 656d 6169 6c20  ttribute :email 
-000041b0: 6f72 2070 7269 6e63 6970 616c 5f69 6420  or principal_id 
-000041c0: 6d75 7374 2062 6520 7365 740a 2020 2020  must be set.    
-000041d0: 2020 2020 2020 2020 7072 696e 6369 7061          principa
-000041e0: 6c5f 6964 3a20 5072 696e 6369 7061 6c20  l_id: Principal 
-000041f0: 6964 2074 6861 7420 7761 6e74 2074 6f20  id that want to 
-00004200: 7573 6520 746f 2061 7373 6967 6e20 7468  use to assign th
-00004210: 6520 7461 736b 2e20 4174 7472 6962 7574  e task. Attribut
-00004220: 6520 5f65 6d61 696c 206f 7220 7072 696e  e _email or prin
-00004230: 6369 7061 6c5f 6964 206d 7573 7420 6265  cipal_id must be
-00004240: 2073 6574 0a20 2020 2020 2020 204e 2905   set.        N).
-00004250: 7214 0000 0072 1500 0000 7230 0000 0072  r....r....r0...r
-00004260: 5a00 0000 7233 0000 0029 0572 1700 0000  Z...r3...).r....
-00004270: 7230 0000 0072 5a00 0000 7233 0000 0072  r0...rZ...r3...r
-00004280: 1000 0000 7218 0000 0072 1a00 0000 721b  ....r....r....r.
-00004290: 0000 0072 1500 0000 1e02 0000 7308 0000  ...r........s...
-000042a0: 0000 090e 0106 0106 017a 1a41 7373 6967  .........z.Assig
-000042b0: 6e54 6173 6b52 6571 7565 7374 2e5f 5f69  nTaskRequest.__i
-000042c0: 6e69 745f 5f29 024e 4e72 5b00 0000 721a  nit__).NNr[...r.
-000042d0: 0000 0072 1a00 0000 7218 0000 0072 1b00  ...r....r....r..
-000042e0: 0000 7277 0000 0017 0200 0073 1a00 0000  ..rw.......s....
-000042f0: 0802 0801 0801 08fd 0607 0000 00ff 0201  ................
-00004300: 0200 0600 0600 0201 02fe 7277 0000 0063  ..........rw...c
-00004310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004320: 0400 0000 0000 0000 7336 0000 0065 005a  ........s6...e.Z
-00004330: 0164 005a 0264 0164 0164 0264 039c 0269  .d.Z.d.d.d.d...i
-00004340: 015a 0365 046a 0565 0664 0464 059c 0387  .Z.e.j.e.d.d....
-00004350: 0066 0164 0664 0784 0c5a 0787 0004 005a  .f.d.d...Z.....Z
-00004360: 0853 0029 08da 1241 7373 6967 6e54 6173  .S.)...AssignTas
-00004370: 6b52 6573 706f 6e73 6572 6a00 0000 726b  kResponserj...rk
-00004380: 0000 0072 0c00 0000 4e72 6c00 0000 6302  ...r....Nrl...c.
-00004390: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-000043a0: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
-000043b0: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-000043c0: 6401 5300 7274 0000 0072 6d00 0000 726e  d.S.rt...rm...rn
-000043d0: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
-000043e0: 0000 7215 0000 0032 0200 0073 0400 0000  ..r....2...s....
-000043f0: 0005 0e01 7a1b 4173 7369 676e 5461 736b  ....z.AssignTask
-00004400: 5265 7370 6f6e 7365 2e5f 5f69 6e69 745f  Response.__init_
-00004410: 5f72 6f00 0000 721a 0000 0072 1a00 0000  _ro...r....r....
-00004420: 7218 0000 0072 1b00 0000 7278 0000 002d  r....r....rx...-
-00004430: 0200 0073 0800 0000 0802 0200 08ff 0404  ...s............
-00004440: 7278 0000 0063 0000 0000 0000 0000 0000  rx...c..........
-00004450: 0000 0000 0000 0700 0000 0000 0000 7354  ..............sT
-00004460: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00004470: 039c 0264 0464 0264 039c 0264 0564 0664  ...d.d.d...d.d.d
-00004480: 039c 0264 079c 035a 0364 0c65 0465 0465  ...d...Z.d.e.e.e
-00004490: 0565 0665 076a 0819 0019 0065 0964 0864  .e.e.j.....e.d.d
-000044a0: 099c 0587 0066 0164 0a64 0b84 0d5a 0a87  .....f.d.d...Z..
-000044b0: 0004 005a 0b53 0029 0dda 1653 6176 6554  ...Z.S.)...SaveT
-000044c0: 6173 6b45 6c65 6d65 6e74 5265 7175 6573  askElementReques
-000044d0: 7472 2f00 0000 720b 0000 0072 0c00 0000  tr/...r....r....
-000044e0: 7250 0000 0072 5100 0000 7a12 5b54 6173  rP...rQ...z.[Tas
-000044f0: 6b45 6c65 6d65 6e74 5661 6c75 655d 2903  kElementValue]).
-00004500: 7230 0000 0072 5200 0000 7253 0000 004e  r0...rR...rS...N
-00004510: 2905 7230 0000 0072 5200 0000 7253 0000  ).r0...rR...rS..
-00004520: 0072 1000 0000 7211 0000 0063 0400 0000  .r....r....c....
-00004530: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00004540: 0b00 0000 7328 0000 0074 0083 006a 0166  ....s(...t...j.f
-00004550: 007c 048e 0101 007c 017c 005f 027c 027c  .|.....|.|._.|.|
-00004560: 005f 037c 0370 2067 007c 005f 0464 0153  ._.|.p g.|._.d.S
-00004570: 0029 027a a90a 2020 2020 2020 2020 5061  .).z..        Pa
-00004580: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00004590: 2020 2020 2020 7461 736b 5f69 643a 2054        task_id: T
-000045a0: 6173 6b20 746f 2075 7064 6174 650a 2020  ask to update.  
-000045b0: 2020 2020 2020 2020 2020 656c 656d 656e            elemen
-000045c0: 745f 6465 6669 6e69 7469 6f6e 5f63 6f64  t_definition_cod
-000045d0: 653a 2045 6c65 6d65 6e74 2064 6566 696e  e: Element defin
-000045e0: 6974 696f 6e20 636f 6465 0a20 2020 2020  ition code.     
-000045f0: 2020 2020 2020 2065 6c65 6d65 6e74 5f76         element_v
-00004600: 616c 7565 733a 2045 6c65 6d65 6e74 2076  alues: Element v
-00004610: 616c 7565 730a 2020 2020 2020 2020 4e29  alues.        N)
-00004620: 0572 1400 0000 7215 0000 0072 3000 0000  .r....r....r0...
-00004630: 7252 0000 0072 5300 0000 2905 7217 0000  rR...rS...).r...
-00004640: 0072 3000 0000 7252 0000 0072 5300 0000  .r0...rR...rS...
-00004650: 7210 0000 0072 1800 0000 721a 0000 0072  r....r....r....r
-00004660: 1b00 0000 7215 0000 0042 0200 0073 0800  ....r....B...s..
-00004670: 0000 000d 0e01 0601 0601 7a1f 5361 7665  ..........z.Save
-00004680: 5461 736b 456c 656d 656e 7452 6571 7565  TaskElementReque
-00004690: 7374 2e5f 5f69 6e69 745f 5f29 014e 290c  st.__init__).N).
-000046a0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000046b0: 2000 0000 720b 0000 0072 0500 0000 7204   ...r....r....r.
-000046c0: 0000 0072 3800 0000 da10 5461 736b 456c  ...r8.....TaskEl
-000046d0: 656d 656e 7456 616c 7565 7202 0000 0072  ementValuer....r
-000046e0: 1500 0000 7221 0000 0072 1a00 0000 721a  ....r!...r....r.
-000046f0: 0000 0072 1800 0000 721b 0000 0072 7900  ...r....r....ry.
-00004700: 0000 3b02 0000 7318 0000 0008 0208 0108  ..;...s.........
-00004710: 0108 fd06 0a00 fc02 0202 0102 010c 0102  ................
-00004720: 0102 fa72 7900 0000 6300 0000 0000 0000  ...ry...c.......
-00004730: 0000 0000 0000 0000 0004 0000 0000 0000  ................
-00004740: 0073 3600 0000 6500 5a01 6400 5a02 6401  .s6...e.Z.d.Z.d.
-00004750: 6401 6402 6403 9c02 6901 5a03 6504 6a05  d.d.d...i.Z.e.j.
-00004760: 6506 6404 6405 9c03 8700 6601 6406 6407  e.d.d.....f.d.d.
-00004770: 840c 5a07 8700 0400 5a08 5300 2908 da17  ..Z.....Z.S.)...
-00004780: 5361 7665 5461 736b 456c 656d 656e 7452  SaveTaskElementR
-00004790: 6573 706f 6e73 6572 6a00 0000 726b 0000  esponserj...rk..
-000047a0: 0072 0c00 0000 4e72 6c00 0000 6302 0000  .r....Nrl...c...
-000047b0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000047c0: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
-000047d0: 6600 7c02 8e01 0100 7c01 7c00 5f02 6401  f.|.....|.|._.d.
-000047e0: 5300 7274 0000 0072 6d00 0000 726e 0000  S.rt...rm...rn..
-000047f0: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00004800: 7215 0000 005a 0200 0073 0400 0000 0005  r....Z...s......
-00004810: 0e01 7a20 5361 7665 5461 736b 456c 656d  ..z SaveTaskElem
-00004820: 656e 7452 6573 706f 6e73 652e 5f5f 696e  entResponse.__in
-00004830: 6974 5f5f 726f 0000 0072 1a00 0000 721a  it__ro...r....r.
-00004840: 0000 0072 1800 0000 721b 0000 0072 7b00  ...r....r....r{.
-00004850: 0000 5502 0000 7308 0000 0008 0202 0008  ..U...s.........
-00004860: ff04 0472 7b00 0000 6300 0000 0000 0000  ...r{...c.......
-00004870: 0000 0000 0000 0000 0005 0000 0000 0000  ................
-00004880: 0073 3e00 0000 6500 5a01 6400 5a02 6401  .s>...e.Z.d.Z.d.
-00004890: 6402 6403 9c02 6404 6402 6403 9c02 6405  d.d...d.d.d...d.
-000048a0: 9c02 5a03 6504 6504 6505 6406 6407 9c04  ..Z.e.e.e.d.d...
-000048b0: 8700 6601 6408 6409 840c 5a06 8700 0400  ..f.d.d...Z.....
-000048c0: 5a07 5300 290a da18 4465 6c65 7465 5461  Z.S.)...DeleteTa
-000048d0: 736b 456c 656d 656e 7452 6571 7565 7374  skElementRequest
-000048e0: 722f 0000 0072 0b00 0000 720c 0000 0072  r/...r....r....r
-000048f0: 5000 0000 2902 7230 0000 0072 5200 0000  P...).r0...rR...
-00004900: 4e29 0472 3000 0000 7252 0000 0072 1000  N).r0...rR...r..
-00004910: 0000 7211 0000 0063 0300 0000 0000 0000  ..r....c........
-00004920: 0000 0000 0400 0000 0300 0000 0b00 0000  ................
-00004930: 731e 0000 0074 0083 006a 0166 007c 038e  s....t...j.f.|..
-00004940: 0101 007c 017c 005f 027c 027c 005f 0364  ...|.|._.|.|._.d
-00004950: 0153 0029 027a 930a 2020 2020 2020 2020  .S.).z..        
-00004960: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-00004970: 2020 2020 2020 2020 7461 736b 5f69 643a          task_id:
-00004980: 2054 6173 6b20 746f 2075 7064 6174 650a   Task to update.
-00004990: 2020 2020 2020 2020 2020 2020 656c 656d              elem
-000049a0: 656e 745f 6465 6669 6e69 7469 6f6e 5f63  ent_definition_c
-000049b0: 6f64 653a 2045 6c65 6d65 6e74 2064 6566  ode: Element def
-000049c0: 696e 6974 696f 6e20 636f 6465 2074 6f20  inition code to 
-000049d0: 6465 6c65 7465 2061 6c6c 2076 616c 7565  delete all value
-000049e0: 730a 2020 2020 2020 2020 4e29 0472 1400  s.        N).r..
-000049f0: 0000 7215 0000 0072 3000 0000 7252 0000  ..r....r0...rR..
-00004a00: 0029 0472 1700 0000 7230 0000 0072 5200  .).r....r0...rR.
-00004a10: 0000 7210 0000 0072 1800 0000 721a 0000  ..r....r....r...
-00004a20: 0072 1b00 0000 7215 0000 0069 0200 0073  .r....r....i...s
-00004a30: 0600 0000 0006 0e01 0601 7a21 4465 6c65  ..........z!Dele
-00004a40: 7465 5461 736b 456c 656d 656e 7452 6571  teTaskElementReq
-00004a50: 7565 7374 2e5f 5f69 6e69 745f 5f72 1c00  uest.__init__r..
-00004a60: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
-00004a70: 0072 1b00 0000 727c 0000 0063 0200 0073  .r....r|...c...s
-00004a80: 0800 0000 0802 0801 08fe 0605 727c 0000  ............r|..
-00004a90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00004aa0: 0000 0400 0000 0000 0000 7336 0000 0065  ..........s6...e
-00004ab0: 005a 0164 005a 0264 0164 0164 0264 039c  .Z.d.Z.d.d.d.d..
-00004ac0: 0269 015a 0365 046a 0565 0664 0464 059c  .i.Z.e.j.e.d.d..
-00004ad0: 0387 0066 0164 0664 0784 0c5a 0787 0004  ...f.d.d...Z....
-00004ae0: 005a 0853 0029 08da 1944 656c 6574 6554  .Z.S.)...DeleteT
-00004af0: 6173 6b45 6c65 6d65 6e74 5265 7370 6f6e  askElementRespon
-00004b00: 7365 726a 0000 0072 6b00 0000 720c 0000  serj...rk...r...
-00004b10: 004e 726c 0000 0063 0200 0000 0000 0000  .Nrl...c........
-00004b20: 0000 0000 0300 0000 0300 0000 0b00 0000  ................
-00004b30: 7318 0000 0074 0083 006a 0166 007c 028e  s....t...j.f.|..
-00004b40: 0101 007c 017c 005f 0264 0153 0072 7400  ...|.|._.d.S.rt.
-00004b50: 0000 726d 0000 0072 6e00 0000 7218 0000  ..rm...rn...r...
-00004b60: 0072 1a00 0000 721b 0000 0072 1500 0000  .r....r....r....
-00004b70: 7902 0000 7304 0000 0000 050e 017a 2244  y...s........z"D
-00004b80: 656c 6574 6554 6173 6b45 6c65 6d65 6e74  eleteTaskElement
-00004b90: 5265 7370 6f6e 7365 2e5f 5f69 6e69 745f  Response.__init_
-00004ba0: 5f72 6f00 0000 721a 0000 0072 1a00 0000  _ro...r....r....
-00004bb0: 7218 0000 0072 1b00 0000 727d 0000 0074  r....r....r}...t
-00004bc0: 0200 0073 0800 0000 0802 0200 08ff 0404  ...s............
-00004bd0: 727d 0000 0063 0000 0000 0000 0000 0000  r}...c..........
-00004be0: 0000 0000 0000 0500 0000 0000 0000 733e  ..............s>
-00004bf0: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00004c00: 039c 0264 0464 0264 039c 0264 059c 025a  ...d.d.d...d...Z
-00004c10: 0365 0465 0465 0564 0664 079c 0487 0066  .e.e.e.d.d.....f
-00004c20: 0164 0864 0984 0c5a 0687 0004 005a 0753  .d.d...Z.....Z.S
-00004c30: 0029 0ada 2544 656c 6574 6554 6173 6b45  .)..%DeleteTaskE
-00004c40: 6c65 6d65 6e74 5661 6c75 6544 6f63 756d  lementValueDocum
-00004c50: 656e 7452 6571 7565 7374 722f 0000 0072  entRequestr/...r
-00004c60: 0b00 0000 720c 0000 00da 0a64 6f63 756d  ....r......docum
-00004c70: 656e 7449 6429 0272 3000 0000 da0b 646f  entId).r0.....do
-00004c80: 6375 6d65 6e74 5f69 644e 2904 7230 0000  cument_idN).r0..
-00004c90: 0072 8000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00004ca0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00004cb0: 0003 0000 000b 0000 0073 1e00 0000 7400  .........s....t.
-00004cc0: 8300 6a01 6600 7c03 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
-00004cd0: 5f02 7c02 7c00 5f03 6401 5300 2902 7a78  _.|.|._.d.S.).zx
-00004ce0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00004cf0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
-00004d00: 2074 6173 6b5f 6964 3a20 5461 736b 2074   task_id: Task t
-00004d10: 6f20 7570 6461 7465 0a20 2020 2020 2020  o update.       
-00004d20: 2020 2020 2064 6f63 756d 656e 745f 6964       document_id
-00004d30: 3a20 446f 6375 6d65 6e74 2069 6420 746f  : Document id to
-00004d40: 2064 656c 6574 6520 7570 6461 7465 640a   delete updated.
-00004d50: 2020 2020 2020 2020 4e29 0472 1400 0000          N).r....
-00004d60: 7215 0000 0072 3000 0000 7280 0000 0029  r....r0...r....)
-00004d70: 0472 1700 0000 7230 0000 0072 8000 0000  .r....r0...r....
-00004d80: 7210 0000 0072 1800 0000 721a 0000 0072  r....r....r....r
-00004d90: 1b00 0000 7215 0000 0088 0200 0073 0600  ....r........s..
-00004da0: 0000 0006 0e01 0601 7a2e 4465 6c65 7465  ........z.Delete
-00004db0: 5461 736b 456c 656d 656e 7456 616c 7565  TaskElementValue
-00004dc0: 446f 6375 6d65 6e74 5265 7175 6573 742e  DocumentRequest.
-00004dd0: 5f5f 696e 6974 5f5f 721c 0000 0072 1a00  __init__r....r..
-00004de0: 0000 721a 0000 0072 1800 0000 721b 0000  ..r....r....r...
-00004df0: 0072 7e00 0000 8202 0000 7308 0000 0008  .r~.......s.....
-00004e00: 0208 0108 fe06 0572 7e00 0000 6300 0000  .......r~...c...
-00004e10: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00004e20: 0000 0000 0073 3600 0000 6500 5a01 6400  .....s6...e.Z.d.
-00004e30: 5a02 6401 6401 6402 6403 9c02 6901 5a03  Z.d.d.d.d...i.Z.
-00004e40: 6504 6a05 6506 6404 6405 9c03 8700 6601  e.j.e.d.d.....f.
-00004e50: 6406 6407 840c 5a07 8700 0400 5a08 5300  d.d...Z.....Z.S.
-00004e60: 2908 da26 4465 6c65 7465 5461 736b 456c  )..&DeleteTaskEl
-00004e70: 656d 656e 7456 616c 7565 446f 6375 6d65  ementValueDocume
-00004e80: 6e74 5265 7370 6f6e 7365 726a 0000 0072  ntResponserj...r
-00004e90: 6b00 0000 720c 0000 004e 726c 0000 0063  k...r....Nrl...c
-00004ea0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00004eb0: 0300 0000 0b00 0000 7318 0000 0074 0083  ........s....t..
-00004ec0: 006a 0166 007c 028e 0101 007c 017c 005f  .j.f.|.....|.|._
-00004ed0: 0264 0153 0072 7400 0000 726d 0000 0072  .d.S.rt...rm...r
-00004ee0: 6e00 0000 7218 0000 0072 1a00 0000 721b  n...r....r....r.
-00004ef0: 0000 0072 1500 0000 9802 0000 7304 0000  ...r........s...
-00004f00: 0000 050e 017a 2f44 656c 6574 6554 6173  .....z/DeleteTas
-00004f10: 6b45 6c65 6d65 6e74 5661 6c75 6544 6f63  kElementValueDoc
-00004f20: 756d 656e 7452 6573 706f 6e73 652e 5f5f  umentResponse.__
-00004f30: 696e 6974 5f5f 726f 0000 0072 1a00 0000  init__ro...r....
-00004f40: 721a 0000 0072 1800 0000 721b 0000 0072  r....r....r....r
-00004f50: 8100 0000 9302 0000 7308 0000 0008 0202  ........s.......
-00004f60: 0008 ff04 0472 8100 0000 6300 0000 0000  .....r....c.....
-00004f70: 0000 0000 0000 0000 0000 0006 0000 0000  ................
-00004f80: 0000 0073 4c00 0000 6500 5a01 6400 5a02  ...sL...e.Z.d.Z.
-00004f90: 6401 6402 6403 9c02 6404 6405 6403 9c02  d.d.d...d.d.d...
-00004fa0: 6406 9c02 5a03 640b 6504 6505 6506 6504  d...Z.d.e.e.e.e.
-00004fb0: 6507 6602 1900 1900 6507 6407 6408 9c04  e.f.....e.d.d...
-00004fc0: 8700 6601 6409 640a 840d 5a08 8700 0400  ..f.d.d...Z.....
-00004fd0: 5a09 5300 290c da21 5361 7665 5461 736b  Z.S.)..!SaveTask
-00004fe0: 4a73 6f6e 466f 726d 7356 616c 7565 4461  JsonFormsValueDa
-00004ff0: 7461 5265 7175 6573 7472 2f00 0000 720b  taRequestr/...r.
-00005000: 0000 0072 0c00 0000 da04 6461 7461 7a08  ...r......dataz.
-00005010: 7b6f 626a 6563 747d 2902 7230 0000 0072  {object}).r0...r
-00005020: 8300 0000 4e29 0472 3000 0000 7283 0000  ....N).r0...r...
-00005030: 0072 1000 0000 7211 0000 0063 0300 0000  .r....r....c....
-00005040: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00005050: 0b00 0000 7322 0000 0074 0083 006a 0166  ....s"...t...j.f
-00005060: 007c 038e 0101 007c 017c 005f 027c 0270  .|.....|.|._.|.p
-00005070: 1a69 007c 005f 0364 0153 0029 027a 650a  .i.|._.d.S.).ze.
-00005080: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00005090: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-000050a0: 7461 736b 5f69 643a 2054 6173 6b20 746f  task_id: Task to
-000050b0: 2075 7064 6174 650a 2020 2020 2020 2020   update.        
-000050c0: 2020 2020 6461 7461 3a20 6a73 6f6e 2064      data: json d
-000050d0: 6174 6120 746f 2073 6176 650a 2020 2020  ata to save.    
-000050e0: 2020 2020 4e29 0472 1400 0000 7215 0000      N).r....r...
-000050f0: 0072 3000 0000 7283 0000 0029 0472 1700  .r0...r....).r..
-00005100: 0000 7230 0000 0072 8300 0000 7210 0000  ..r0...r....r...
-00005110: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00005120: 7215 0000 00a7 0200 0073 0600 0000 0006  r........s......
-00005130: 0e01 0601 7a2a 5361 7665 5461 736b 4a73  ....z*SaveTaskJs
-00005140: 6f6e 466f 726d 7356 616c 7565 4461 7461  onFormsValueData
-00005150: 5265 7175 6573 742e 5f5f 696e 6974 5f5f  Request.__init__
-00005160: 2901 4e29 0a72 1d00 0000 721e 0000 0072  ).N).r....r....r
-00005170: 1f00 0000 7220 0000 0072 0b00 0000 7205  ....r ...r....r.
-00005180: 0000 0072 0300 0000 7202 0000 0072 1500  ...r....r....r..
-00005190: 0000 7221 0000 0072 1a00 0000 721a 0000  ..r!...r....r...
-000051a0: 0072 1800 0000 721b 0000 0072 8200 0000  .r....r....r....
-000051b0: a102 0000 7308 0000 0008 0208 0108 fe06  ....s...........
-000051c0: 0572 8200 0000 6300 0000 0000 0000 0000  .r....c.........
-000051d0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-000051e0: 3600 0000 6500 5a01 6400 5a02 6401 6401  6...e.Z.d.Z.d.d.
-000051f0: 6402 6403 9c02 6901 5a03 6504 6a05 6506  d.d...i.Z.e.j.e.
-00005200: 6404 6405 9c03 8700 6601 6406 6407 840c  d.d.....f.d.d...
-00005210: 5a07 8700 0400 5a08 5300 2908 da22 5361  Z.....Z.S.).."Sa
-00005220: 7665 5461 736b 4a73 6f6e 466f 726d 7356  veTaskJsonFormsV
-00005230: 616c 7565 4461 7461 5265 7370 6f6e 7365  alueDataResponse
-00005240: 726a 0000 0072 6b00 0000 720c 0000 004e  rj...rk...r....N
-00005250: 726c 0000 0063 0200 0000 0000 0000 0000  rl...c..........
-00005260: 0000 0300 0000 0300 0000 0b00 0000 7318  ..............s.
-00005270: 0000 0074 0083 006a 0166 007c 028e 0101  ...t...j.f.|....
-00005280: 007c 017c 005f 0264 0153 0072 7400 0000  .|.|._.d.S.rt...
-00005290: 726d 0000 0072 6e00 0000 7218 0000 0072  rm...rn...r....r
-000052a0: 1a00 0000 721b 0000 0072 1500 0000 b702  ....r....r......
-000052b0: 0000 7304 0000 0000 050e 017a 2b53 6176  ..s........z+Sav
-000052c0: 6554 6173 6b4a 736f 6e46 6f72 6d73 5661  eTaskJsonFormsVa
-000052d0: 6c75 6544 6174 6152 6573 706f 6e73 652e  lueDataResponse.
-000052e0: 5f5f 696e 6974 5f5f 726f 0000 0072 1a00  __init__ro...r..
-000052f0: 0000 721a 0000 0072 1800 0000 721b 0000  ..r....r....r...
-00005300: 0072 8400 0000 b202 0000 7308 0000 0008  .r........s.....
-00005310: 0202 0008 ff04 0472 8400 0000 6300 0000  .......r....c...
-00005320: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00005330: 0000 0000 0073 4000 0000 6500 5a01 6400  .....s@...e.Z.d.
-00005340: 5a02 6401 6402 6403 9c02 6404 6405 6403  Z.d.d.d...d.d.d.
-00005350: 9c02 6406 9c02 5a03 6504 6505 6a06 6507  ..d...Z.e.e.j.e.
-00005360: 6407 6408 9c04 8700 6601 6409 640a 840c  d.d.....f.d.d...
-00005370: 5a08 8700 0400 5a09 5300 290b da14 4170  Z.....Z.S.)...Ap
-00005380: 7065 6e64 5461 736b 4c6f 6752 6571 7565  pendTaskLogReque
-00005390: 7374 722f 0000 0072 0b00 0000 720c 0000  str/...r....r...
-000053a0: 00da 036c 6f67 da03 4c6f 6729 0272 3000  ...log..Log).r0.
-000053b0: 0000 7286 0000 004e 2904 7230 0000 0072  ..r....N).r0...r
-000053c0: 8600 0000 7210 0000 0072 1100 0000 6303  ....r....r....c.
-000053d0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-000053e0: 0000 000b 0000 0073 1e00 0000 7400 8300  .......s....t...
-000053f0: 6a01 6600 7c03 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
-00005400: 7c02 7c00 5f03 6401 5300 2902 7a6e 0a20  |.|._.d.S.).zn. 
-00005410: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00005420: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00005430: 6173 6b5f 6964 3a20 5461 736b 2074 6f20  ask_id: Task to 
-00005440: 7570 6461 7465 0a20 2020 2020 2020 2020  update.         
-00005450: 2020 206c 6f67 3a20 4c6f 6720 6461 7461     log: Log data
-00005460: 2074 6f20 6164 6420 746f 2074 6865 2074   to add to the t
-00005470: 6173 6b0a 2020 2020 2020 2020 4e29 0472  ask.        N).r
-00005480: 1400 0000 7215 0000 0072 3000 0000 7286  ....r....r0...r.
-00005490: 0000 0029 0472 1700 0000 7230 0000 0072  ...).r....r0...r
-000054a0: 8600 0000 7210 0000 0072 1800 0000 721a  ....r....r....r.
-000054b0: 0000 0072 1b00 0000 7215 0000 00c6 0200  ...r....r.......
-000054c0: 0073 0600 0000 0006 0e01 0601 7a1d 4170  .s..........z.Ap
-000054d0: 7065 6e64 5461 736b 4c6f 6752 6571 7565  pendTaskLogReque
-000054e0: 7374 2e5f 5f69 6e69 745f 5f29 0a72 1d00  st.__init__).r..
-000054f0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00005500: 0072 0b00 0000 7238 0000 0072 8700 0000  .r....r8...r....
-00005510: 7202 0000 0072 1500 0000 7221 0000 0072  r....r....r!...r
-00005520: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
-00005530: 0000 0072 8500 0000 c002 0000 7308 0000  ...r........s...
-00005540: 0008 0208 0108 fe06 0572 8500 0000 6300  .........r....c.
-00005550: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00005560: 0000 0000 0000 0073 3600 0000 6500 5a01  .......s6...e.Z.
-00005570: 6400 5a02 6401 6401 6402 6403 9c02 6901  d.Z.d.d.d.d...i.
-00005580: 5a03 6504 6a05 6506 6404 6405 9c03 8700  Z.e.j.e.d.d.....
-00005590: 6601 6406 6407 840c 5a07 8700 0400 5a08  f.d.d...Z.....Z.
-000055a0: 5300 2908 da15 4170 7065 6e64 5461 736b  S.)...AppendTask
-000055b0: 4c6f 6752 6573 706f 6e73 6572 6a00 0000  LogResponserj...
-000055c0: 726b 0000 0072 0c00 0000 4e72 6c00 0000  rk...r....Nrl...
-000055d0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000055e0: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
-000055f0: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
-00005600: 5f02 6401 5300 7274 0000 0072 6d00 0000  _.d.S.rt...rm...
-00005610: 726e 0000 0072 1800 0000 721a 0000 0072  rn...r....r....r
-00005620: 1b00 0000 7215 0000 00d6 0200 0073 0400  ....r........s..
-00005630: 0000 0005 0e01 7a1e 4170 7065 6e64 5461  ......z.AppendTa
-00005640: 736b 4c6f 6752 6573 706f 6e73 652e 5f5f  skLogResponse.__
-00005650: 696e 6974 5f5f 726f 0000 0072 1a00 0000  init__ro...r....
-00005660: 721a 0000 0072 1800 0000 721b 0000 0072  r....r....r....r
-00005670: 8800 0000 d102 0000 7308 0000 0008 0202  ........s.......
-00005680: 0008 ff04 0472 8800 0000 4e29 35da 0674  .....r....N)5..t
-00005690: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-000056a0: 0400 0000 7205 0000 00da 0b6b 7566 6c6f  ....r......kuflo
-000056b0: 775f 7265 7374 7206 0000 0072 3800 0000  w_restr....r8...
-000056c0: 5a16 6b75 666c 6f77 5f72 6573 742e 5f67  Z.kuflow_rest._g
-000056d0: 656e 6572 6174 6564 7207 0000 00da 054d  eneratedr......M
-000056e0: 6f64 656c 7208 0000 0072 2200 0000 7229  odelr....r"...r)
-000056f0: 0000 0072 2d00 0000 722e 0000 0072 3100  ...r-...r....r1.
-00005700: 0000 7232 0000 0072 3500 0000 7239 0000  ..r2...r5...r9..
-00005710: 0072 3b00 0000 723e 0000 0072 4400 0000  .r;...r>...rD...
-00005720: 7247 0000 0072 4800 0000 724f 0000 0072  rG...rH...rO...r
-00005730: 5500 0000 7257 0000 0072 5800 0000 7259  U...rW...rX...rY
-00005740: 0000 0072 5c00 0000 725d 0000 0072 6200  ...r\...r]...rb.
-00005750: 0000 7265 0000 0072 6900 0000 7270 0000  ..re...ri...rp..
-00005760: 0072 7100 0000 7272 0000 0072 7300 0000  .rq...rr...rs...
-00005770: 7275 0000 0072 7600 0000 7277 0000 0072  ru...rv...rw...r
-00005780: 7800 0000 7279 0000 0072 7b00 0000 727c  x...ry...r{...r|
-00005790: 0000 0072 7d00 0000 727e 0000 0072 8100  ...r}...r~...r..
-000057a0: 0000 7282 0000 0072 8400 0000 7285 0000  ..r....r....r...
-000057b0: 0072 8800 0000 721a 0000 0072 1a00 0000  .r....r....r....
-000057c0: 721a 0000 0072 1b00 0000 da08 3c6d 6f64  r....r......<mod
-000057d0: 756c 653e 1900 0000 7358 0000 0018 020c  ule>....sX......
-000057e0: 010c 0812 0e12 0e12 1e12 0e12 1012 1312  ................
-000057f0: 0e12 0e12 0e12 0e12 1612 0e12 0e12 0e12  ................
-00005800: 1a12 0e12 1112 0e12 1712 0e12 2612 0e12  ............&...
-00005810: 0e12 0e12 0e12 0e12 0e12 0e12 0e12 0e12  ................
-00005820: 1612 0e12 1a12 0e12 1112 0e12 1112 0e12  ................
-00005830: 1112 0e12 11                             .....
+00000350: 5a34 4700 6458 6459 8400 6459 6509 6a0a  Z4G.dXdY..dYe.j.
+00000360: 8303 5a35 4700 645a 645b 8400 645b 6509  ..Z5G.dZd[..d[e.
+00000370: 6a0a 8303 5a36 645c 5300 295d e900 0000  j...Z6d\S.)]....
+00000380: 0029 04da 0341 6e79 da04 4469 6374 da04  .)...Any..Dict..
+00000390: 4c69 7374 da08 4f70 7469 6f6e 616c 2901  List..Optional).
+000003a0: da06 6d6f 6465 6c73 2901 da0e 5f73 6572  ..models)..._ser
+000003b0: 6961 6c69 7a61 7469 6f6e 6300 0000 0000  ializationc.....
+000003c0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+000003d0: 0000 0073 3400 0000 6500 5a01 6400 5a02  ...s4...e.Z.d.Z.
+000003e0: 6401 6402 6403 6404 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
+000003f0: 6505 6405 6406 9c03 8700 6601 6407 6408  e.d.d.....f.d.d.
+00000400: 840c 5a06 8700 0400 5a07 5300 2909 da0f  ..Z.....Z.S.)...
+00000410: 576f 726b 666c 6f77 5265 7175 6573 74da  WorkflowRequest.
+00000420: 0a70 726f 6365 7373 5f69 64da 0970 726f  .process_id..pro
+00000430: 6365 7373 4964 da03 7374 72a9 02da 036b  cessId..str....k
+00000440: 6579 da04 7479 7065 4ea9 0372 0900 0000  ey..typeN..r....
+00000450: da06 6b77 6172 6773 da06 7265 7475 726e  ..kwargs..return
+00000460: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000470: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
+00000480: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+00000490: 5f02 6401 5300 a902 7a5f 0a20 2020 2020  _.d.S...z_.     
+000004a0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+000004b0: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+000004c0: 7373 5f69 643a 2049 6465 6e74 6966 6965  ss_id: Identifie
+000004d0: 7220 6f66 2074 6865 2072 656c 6174 6564  r of the related
+000004e0: 2063 7265 6174 6564 2070 726f 6365 7373   created process
+000004f0: 0a20 2020 2020 2020 204e a903 da05 7375  .        N....su
+00000500: 7065 72da 085f 5f69 6e69 745f 5f72 0900  per..__init__r..
+00000510: 0000 a903 da04 7365 6c66 7209 0000 0072  ......selfr....r
+00000520: 1000 0000 a901 da09 5f5f 636c 6173 735f  ........__class_
+00000530: 5fa9 00fa 692f 776f 726b 2f6b 7566 6c6f  _...i/work/kuflo
+00000540: 772d 7364 6b2d 7079 7468 6f6e 2f6b 7566  w-sdk-python/kuf
+00000550: 6c6f 772d 7465 6d70 6f72 616c 2d61 6374  low-temporal-act
+00000560: 6976 6974 792d 6b75 666c 6f77 2f6b 7566  ivity-kuflow/kuf
+00000570: 6c6f 775f 7465 6d70 6f72 616c 5f61 6374  low_temporal_act
+00000580: 6976 6974 795f 6b75 666c 6f77 2f6d 6f64  ivity_kuflow/mod
+00000590: 656c 732f 5f6d 6f64 656c 732e 7079 7215  els/_models.pyr.
+000005a0: 0000 0029 0000 0073 0400 0000 0005 0e01  ...)...s........
+000005b0: 7a18 576f 726b 666c 6f77 5265 7175 6573  z.WorkflowReques
+000005c0: 742e 5f5f 696e 6974 5f5f a908 da08 5f5f  t.__init__....__
+000005d0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000005e0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000005f0: da0e 5f61 7474 7269 6275 7465 5f6d 6170  .._attribute_map
+00000600: 720b 0000 0072 0200 0000 7215 0000 00da  r....r....r.....
+00000610: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 721a  .__classcell__r.
+00000620: 0000 0072 1a00 0000 7218 0000 0072 1b00  ...r....r....r..
+00000630: 0000 7208 0000 0024 0000 0073 0800 0000  ..r....$...s....
+00000640: 0802 0200 08ff 0404 7208 0000 0063 0000  ........r....c..
+00000650: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00000660: 0000 0000 0000 733a 0000 0065 005a 0164  ......s:...e.Z.d
+00000670: 005a 0264 0164 0164 0264 039c 0269 015a  .Z.d.d.d.d...i.Z
+00000680: 0364 0865 0465 0519 0065 0664 0464 059c  .d.e.e...e.d.d..
+00000690: 0387 0066 0164 0664 0784 0d5a 0787 0004  ...f.d.d...Z....
+000006a0: 005a 0853 0029 09da 1057 6f72 6b66 6c6f  .Z.S.)...Workflo
+000006b0: 7752 6573 706f 6e73 65da 076d 6573 7361  wResponse..messa
+000006c0: 6765 720b 0000 0072 0c00 0000 4ea9 0372  ger....r....N..r
+000006d0: 2300 0000 7210 0000 0072 1100 0000 6302  #...r....r....c.
+000006e0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000006f0: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
+00000700: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
+00000710: 6401 5300 a902 7a43 0a20 2020 2020 2020  d.S...zC.       
+00000720: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+00000730: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00000740: 3a20 5265 7370 6f6e 7365 206d 6573 7361  : Response messa
+00000750: 6765 0a20 2020 2020 2020 204e a903 7214  ge.        N..r.
+00000760: 0000 0072 1500 0000 7223 0000 00a9 0372  ...r....r#.....r
+00000770: 1700 0000 7223 0000 0072 1000 0000 7218  ....r#...r....r.
+00000780: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00000790: 0000 3700 0000 7304 0000 0000 050e 017a  ..7...s........z
+000007a0: 1957 6f72 6b66 6c6f 7752 6573 706f 6e73  .WorkflowRespons
+000007b0: 652e 5f5f 696e 6974 5f5f 2901 4ea9 0972  e.__init__).N..r
+000007c0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+000007d0: 0000 0072 0500 0000 720b 0000 0072 0200  ...r....r....r..
+000007e0: 0000 7215 0000 0072 2100 0000 721a 0000  ..r....r!...r...
+000007f0: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
+00000800: 7222 0000 0032 0000 0073 0800 0000 0802  r"...2...s......
+00000810: 0200 08ff 0404 7222 0000 0063 0000 0000  ......r"...c....
+00000820: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+00000830: 0000 0000 7352 0000 0065 005a 0164 005a  ....sR...e.Z.d.Z
+00000840: 0264 0164 0264 039c 0264 0464 0264 039c  .d.d.d...d.d.d..
+00000850: 0264 0564 0264 039c 0264 0664 0264 039c  .d.d.d...d.d.d..
+00000860: 0264 079c 045a 0365 0465 0465 0465 0465  .d...Z.e.e.e.e.e
+00000870: 0564 0864 099c 0687 0066 0164 0a64 0b84  .d.d.....f.d.d..
+00000880: 0c5a 0687 0004 005a 0753 0029 0cda 1955  .Z.....Z.S.)...U
+00000890: 7365 7241 6374 696f 6e57 6f72 6b66 6c6f  serActionWorkflo
+000008a0: 7752 6571 7565 7374 720a 0000 0072 0b00  wRequestr....r..
+000008b0: 0000 720c 0000 005a 1875 7365 7241 6374  ..r....Z.userAct
+000008c0: 696f 6e44 6566 696e 6974 696f 6e43 6f64  ionDefinitionCod
+000008d0: 655a 0c75 7365 7241 6374 696f 6e49 645a  eZ.userActionIdZ
+000008e0: 1472 6571 7565 7374 6f72 5072 696e 6369  .requestorPrinci
+000008f0: 7061 6c49 6429 0472 0900 0000 da1b 7573  palId).r......us
+00000900: 6572 5f61 6374 696f 6e5f 6465 6669 6e69  er_action_defini
+00000910: 7469 6f6e 5f63 6f64 65da 0e75 7365 725f  tion_code..user_
+00000920: 6163 7469 6f6e 5f69 64da 1672 6571 7565  action_id..reque
+00000930: 7374 6f72 5f70 7269 6e63 6970 616c 5f69  stor_principal_i
+00000940: 644e 2906 7209 0000 0072 2a00 0000 722b  dN).r....r*...r+
+00000950: 0000 0072 2c00 0000 7210 0000 0072 1100  ...r,...r....r..
+00000960: 0000 6305 0000 0000 0000 0000 0000 0006  ..c.............
+00000970: 0000 0003 0000 000b 0000 0073 2a00 0000  ...........s*...
+00000980: 7400 8300 6a01 6600 7c05 8e01 0100 7c01  t...j.f.|.....|.
+00000990: 7c00 5f02 7c02 7c00 5f03 7c03 7c00 5f04  |._.|.|._.|.|._.
+000009a0: 7c04 7c00 5f05 6401 5300 2902 613a 0100  |.|._.d.S.).a:..
+000009b0: 000a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+000009c0: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+000009d0: 2020 7072 6f63 6573 735f 6964 3a20 4964    process_id: Id
+000009e0: 656e 7469 6669 6572 206f 6620 7468 6520  entifier of the 
+000009f0: 7265 6c61 7465 6420 7072 6f63 6573 730a  related process.
+00000a00: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00000a10: 5f61 6374 696f 6e5f 6465 6669 6e69 7469  _action_definiti
+00000a20: 6f6e 5f63 6f64 653a 2043 6f64 6520 6f66  on_code: Code of
+00000a30: 2074 6865 2075 7365 7220 6163 7469 6f6e   the user action
+00000a40: 2064 6566 696e 6974 696f 6e0a 2020 2020   definition.    
+00000a50: 2020 2020 2020 2020 7573 6572 5f61 6374          user_act
+00000a60: 696f 6e5f 6964 3a20 4964 656e 7469 6669  ion_id: Identifi
+00000a70: 6572 206f 6620 7468 6520 7573 6572 2061  er of the user a
+00000a80: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000a90: 2020 7265 7175 6573 746f 725f 7072 696e    requestor_prin
+00000aa0: 6369 7061 6c5f 6964 3a20 4964 656e 7469  cipal_id: Identi
+00000ab0: 6669 6572 206f 6620 7468 6520 7072 696e  fier of the prin
+00000ac0: 6369 7061 6c20 7468 6174 2072 6571 7565  cipal that reque
+00000ad0: 7374 2074 6865 2075 7365 7220 6163 7469  st the user acti
+00000ae0: 6f6e 0a20 2020 2020 2020 204e 2906 7214  on.        N).r.
+00000af0: 0000 0072 1500 0000 7209 0000 0072 2a00  ...r....r....r*.
+00000b00: 0000 722b 0000 0072 2c00 0000 2906 7217  ..r+...r,...).r.
+00000b10: 0000 0072 0900 0000 722a 0000 0072 2b00  ...r....r*...r+.
+00000b20: 0000 722c 0000 0072 1000 0000 7218 0000  ..r,...r....r...
+00000b30: 0072 1a00 0000 721b 0000 0072 1500 0000  .r....r....r....
+00000b40: 4800 0000 730a 0000 0000 0f0e 0106 0106  H...s...........
+00000b50: 0106 017a 2255 7365 7241 6374 696f 6e57  ...z"UserActionW
+00000b60: 6f72 6b66 6c6f 7752 6571 7565 7374 2e5f  orkflowRequest._
+00000b70: 5f69 6e69 745f 5f72 1c00 0000 721a 0000  _init__r....r...
+00000b80: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
+00000b90: 7229 0000 0040 0000 0073 1800 0000 0802  r)...@...s......
+00000ba0: 0801 0801 0801 08fc 0609 0201 0201 0201  ................
+00000bb0: 0201 0201 02f9 7229 0000 0063 0000 0000  ......r)...c....
+00000bc0: 0000 0000 0000 0000 0000 0000 0500 0000  ................
+00000bd0: 0000 0000 733a 0000 0065 005a 0164 005a  ....s:...e.Z.d.Z
+00000be0: 0264 0164 0164 0264 039c 0269 015a 0364  .d.d.d.d...i.Z.d
+00000bf0: 0865 0465 0519 0065 0664 0464 059c 0387  .e.e...e.d.d....
+00000c00: 0066 0164 0664 0784 0d5a 0787 0004 005a  .f.d.d...Z.....Z
+00000c10: 0853 0029 09da 1a55 7365 7241 6374 696f  .S.)...UserActio
+00000c20: 6e57 6f72 6b66 6c6f 7752 6573 706f 6e73  nWorkflowRespons
+00000c30: 6572 2300 0000 720b 0000 0072 0c00 0000  er#...r....r....
+00000c40: 4e72 2400 0000 6302 0000 0000 0000 0000  Nr$...c.........
+00000c50: 0000 0003 0000 0003 0000 000b 0000 0073  ...............s
+00000c60: 1800 0000 7400 8300 6a01 6600 7c02 8e01  ....t...j.f.|...
+00000c70: 0100 7c01 7c00 5f02 6401 5300 2902 7a4f  ..|.|._.d.S.).zO
+00000c80: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000c90: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00000ca0: 206d 6573 7361 6765 3a20 5573 6572 2061   message: User a
+00000cb0: 6374 696f 6e20 6d65 7373 6167 6520 7265  ction message re
+00000cc0: 7370 6f6e 7365 0a20 2020 2020 2020 204e  sponse.        N
+00000cd0: 7226 0000 0072 2700 0000 7218 0000 0072  r&...r'...r....r
+00000ce0: 1a00 0000 721b 0000 0072 1500 0000 6300  ....r....r....c.
+00000cf0: 0000 7304 0000 0000 050e 017a 2355 7365  ..s........z#Use
+00000d00: 7241 6374 696f 6e57 6f72 6b66 6c6f 7752  rActionWorkflowR
+00000d10: 6573 706f 6e73 652e 5f5f 696e 6974 5f5f  esponse.__init__
+00000d20: 2901 4e72 2800 0000 721a 0000 0072 1a00  ).Nr(...r....r..
+00000d30: 0000 7218 0000 0072 1b00 0000 722d 0000  ..r....r....r-..
+00000d40: 005e 0000 0073 0800 0000 0802 0200 08ff  .^...s..........
+00000d50: 0404 722d 0000 0063 0000 0000 0000 0000  ..r-...c........
+00000d60: 0000 0000 0000 0000 0500 0000 0000 0000  ................
+00000d70: 733e 0000 0065 005a 0164 005a 0264 0164  s>...e.Z.d.Z.d.d
+00000d80: 0264 039c 0264 0464 0264 039c 0264 059c  .d...d.d.d...d..
+00000d90: 025a 0365 0465 0465 0564 0664 079c 0487  .Z.e.e.e.d.d....
+00000da0: 0066 0164 0864 0984 0c5a 0687 0004 005a  .f.d.d...Z.....Z
+00000db0: 0753 0029 0ada 1452 6f62 6f74 576f 726b  .S.)...RobotWork
+00000dc0: 666c 6f77 5265 7175 6573 7472 0a00 0000  flowRequestr....
+00000dd0: 720b 0000 0072 0c00 0000 da06 7461 736b  r....r......task
+00000de0: 4964 2902 7209 0000 00da 0774 6173 6b5f  Id).r......task_
+00000df0: 6964 4e29 0472 0900 0000 7230 0000 0072  idN).r....r0...r
+00000e00: 1000 0000 7211 0000 0063 0300 0000 0000  ....r....c......
+00000e10: 0000 0000 0000 0400 0000 0300 0000 0b00  ................
+00000e20: 0000 731e 0000 0074 0083 006a 0166 007c  ..s....t...j.f.|
+00000e30: 038e 0101 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
+00000e40: 0364 0153 0072 1200 0000 2904 7214 0000  .d.S.r....).r...
+00000e50: 0072 1500 0000 7209 0000 0072 3000 0000  .r....r....r0...
+00000e60: 2904 7217 0000 0072 0900 0000 7230 0000  ).r....r....r0..
+00000e70: 0072 1000 0000 7218 0000 0072 1a00 0000  .r....r....r....
+00000e80: 721b 0000 0072 1500 0000 7200 0000 7306  r....r....r...s.
+00000e90: 0000 0000 050e 0106 017a 1d52 6f62 6f74  .........z.Robot
+00000ea0: 576f 726b 666c 6f77 5265 7175 6573 742e  WorkflowRequest.
+00000eb0: 5f5f 696e 6974 5f5f 721c 0000 0072 1a00  __init__r....r..
+00000ec0: 0000 721a 0000 0072 1800 0000 721b 0000  ..r....r....r...
+00000ed0: 0072 2e00 0000 6c00 0000 7308 0000 0008  .r....l...s.....
+00000ee0: 0208 0108 fe06 0572 2e00 0000 6300 0000  .......r....c...
+00000ef0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
+00000f00: 0000 0000 0073 3a00 0000 6500 5a01 6400  .....s:...e.Z.d.
+00000f10: 5a02 6401 6401 6402 6403 9c02 6901 5a03  Z.d.d.d.d...i.Z.
+00000f20: 6408 6504 6505 1900 6506 6404 6405 9c03  d.e.e...e.d.d...
+00000f30: 8700 6601 6406 6407 840d 5a07 8700 0400  ..f.d.d...Z.....
+00000f40: 5a08 5300 2909 da15 526f 626f 7457 6f72  Z.S.)...RobotWor
+00000f50: 6b66 6c6f 7752 6573 706f 6e73 6572 2300  kflowResponser#.
+00000f60: 0000 720b 0000 0072 0c00 0000 4e72 2400  ..r....r....Nr$.
+00000f70: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00000f80: 0000 0003 0000 000b 0000 0073 1800 0000  ...........s....
+00000f90: 7400 8300 6a01 6600 7c02 8e01 0100 7c01  t...j.f.|.....|.
+00000fa0: 7c00 5f02 6401 5300 7225 0000 0072 2600  |._.d.S.r%...r&.
+00000fb0: 0000 7227 0000 0072 1800 0000 721a 0000  ..r'...r....r...
+00000fc0: 0072 1b00 0000 7215 0000 0081 0000 0073  .r....r........s
+00000fd0: 0400 0000 0005 0e01 7a1e 526f 626f 7457  ........z.RobotW
+00000fe0: 6f72 6b66 6c6f 7752 6573 706f 6e73 652e  orkflowResponse.
+00000ff0: 5f5f 696e 6974 5f5f 2901 4e72 2800 0000  __init__).Nr(...
+00001000: 721a 0000 0072 1a00 0000 7218 0000 0072  r....r....r....r
+00001010: 1b00 0000 7231 0000 007c 0000 0073 0800  ....r1...|...s..
+00001020: 0000 0802 0200 08ff 0404 7231 0000 0063  ..........r1...c
+00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001040: 0400 0000 0000 0000 7334 0000 0065 005a  ........s4...e.Z
+00001050: 0164 005a 0264 0164 0264 0364 049c 0269  .d.Z.d.d.d.d...i
+00001060: 015a 0365 0465 0564 0564 069c 0387 0066  .Z.e.e.d.d.....f
+00001070: 0164 0764 0884 0c5a 0687 0004 005a 0753  .d.d...Z.....Z.S
+00001080: 0029 09da 1852 6574 7269 6576 6550 7269  .)...RetrievePri
+00001090: 6e63 6970 616c 5265 7175 6573 74da 0c70  ncipalRequest..p
+000010a0: 7269 6e63 6970 616c 5f69 64da 0b70 7269  rincipal_id..pri
+000010b0: 6e63 6970 616c 4964 720b 0000 0072 0c00  ncipalIdr....r..
+000010c0: 0000 4e29 0372 3300 0000 7210 0000 0072  ..N).r3...r....r
+000010d0: 1100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000010e0: 0003 0000 0003 0000 000b 0000 0073 1800  .............s..
+000010f0: 0000 7400 8300 6a01 6600 7c02 8e01 0100  ..t...j.f.|.....
+00001100: 7c01 7c00 5f02 6401 5300 2902 7a5d 0a20  |.|._.d.S.).z]. 
+00001110: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00001120: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00001130: 7269 6e63 6970 616c 5f69 643a 2049 6465  rincipal_id: Ide
+00001140: 6e74 6966 6965 7220 6f66 2074 6865 2072  ntifier of the r
+00001150: 6571 7565 7374 6564 2070 7269 6e63 6970  equested princip
+00001160: 616c 0a20 2020 2020 2020 204e 2903 7214  al.        N).r.
+00001170: 0000 0072 1500 0000 7233 0000 0029 0372  ...r....r3...).r
+00001180: 1700 0000 7233 0000 0072 1000 0000 7218  ....r3...r....r.
+00001190: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+000011a0: 0000 9400 0000 7304 0000 0000 050e 017a  ......s........z
+000011b0: 2152 6574 7269 6576 6550 7269 6e63 6970  !RetrievePrincip
+000011c0: 616c 5265 7175 6573 742e 5f5f 696e 6974  alRequest.__init
+000011d0: 5f5f 721c 0000 0072 1a00 0000 721a 0000  __r....r....r...
+000011e0: 0072 1800 0000 721b 0000 0072 3200 0000  .r....r....r2...
+000011f0: 8f00 0000 7308 0000 0008 0202 0008 ff04  ....s...........
+00001200: 0472 3200 0000 6300 0000 0000 0000 0000  .r2...c.........
+00001210: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+00001220: 3600 0000 6500 5a01 6400 5a02 6401 6401  6...e.Z.d.Z.d.d.
+00001230: 6402 6403 9c02 6901 5a03 6504 6a05 6506  d.d...i.Z.e.j.e.
+00001240: 6404 6405 9c03 8700 6601 6406 6407 840c  d.d.....f.d.d...
+00001250: 5a07 8700 0400 5a08 5300 2908 da19 5265  Z.....Z.S.)...Re
+00001260: 7472 6965 7665 5072 696e 6369 7061 6c52  trievePrincipalR
+00001270: 6573 706f 6e73 65da 0970 7269 6e63 6970  esponse..princip
+00001280: 616c da09 5072 696e 6369 7061 6c72 0c00  al..Principalr..
+00001290: 0000 4e29 0372 3600 0000 7210 0000 0072  ..N).r6...r....r
+000012a0: 1100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000012b0: 0003 0000 0003 0000 000b 0000 0073 1800  .............s..
+000012c0: 0000 7400 8300 6a01 6600 7c02 8e01 0100  ..t...j.f.|.....
+000012d0: 7c01 7c00 5f02 6401 5300 2902 7a4d 0a20  |.|._.d.S.).zM. 
+000012e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000012f0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+00001300: 7269 6e63 6970 616c 3a20 5072 696e 6369  rincipal: Princi
+00001310: 7061 6c20 6461 7461 2072 6571 7565 7374  pal data request
+00001320: 6564 0a20 2020 2020 2020 204e 2903 7214  ed.        N).r.
+00001330: 0000 0072 1500 0000 7236 0000 0029 0372  ...r....r6...).r
+00001340: 1700 0000 7236 0000 0072 1000 0000 7218  ....r6...r....r.
+00001350: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00001360: 0000 a200 0000 7304 0000 0000 050e 017a  ......s........z
+00001370: 2252 6574 7269 6576 6550 7269 6e63 6970  "RetrievePrincip
+00001380: 616c 5265 7370 6f6e 7365 2e5f 5f69 6e69  alResponse.__ini
+00001390: 745f 5f29 0972 1d00 0000 721e 0000 0072  t__).r....r....r
+000013a0: 1f00 0000 7220 0000 00da 0b6d 6f64 656c  ....r .....model
+000013b0: 735f 7265 7374 7237 0000 0072 0200 0000  s_restr7...r....
+000013c0: 7215 0000 0072 2100 0000 721a 0000 0072  r....r!...r....r
+000013d0: 1a00 0000 7218 0000 0072 1b00 0000 7235  ....r....r....r5
+000013e0: 0000 009d 0000 0073 0800 0000 0802 0200  .......s........
+000013f0: 08ff 0404 7235 0000 0063 0000 0000 0000  ....r5...c......
+00001400: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00001410: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
+00001420: 0164 0264 0364 049c 0269 015a 0365 0465  .d.d.d...i.Z.e.e
+00001430: 0564 0564 069c 0387 0066 0164 0764 0884  .d.d.....f.d.d..
+00001440: 0c5a 0687 0004 005a 0753 0029 09da 1952  .Z.....Z.S.)...R
+00001450: 6574 7269 6576 6554 656e 616e 7455 7365  etrieveTenantUse
+00001460: 7252 6571 7565 7374 da0e 7465 6e61 6e74  rRequest..tenant
+00001470: 5f75 7365 725f 6964 5a0c 7465 6e61 6e74  _user_idZ.tenant
+00001480: 5573 6572 4964 720b 0000 0072 0c00 0000  UserIdr....r....
+00001490: 4e29 0372 3a00 0000 7210 0000 0072 1100  N).r:...r....r..
+000014a0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+000014b0: 0000 0003 0000 000b 0000 0073 1800 0000  ...........s....
+000014c0: 7400 8300 6a01 6600 7c02 8e01 0100 7c01  t...j.f.|.....|.
+000014d0: 7c00 5f02 6401 5300 2902 7a61 0a20 2020  |._.d.S.).za.   
+000014e0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+000014f0: 0a20 2020 2020 2020 2020 2020 2074 656e  .            ten
+00001500: 616e 745f 7573 6572 5f69 643a 2049 6465  ant_user_id: Ide
+00001510: 6e74 6966 6965 7220 6f66 2074 6865 2072  ntifier of the r
+00001520: 6571 7565 7374 6564 2074 656e 616e 7420  equested tenant 
+00001530: 7573 6572 0a20 2020 2020 2020 204e 2903  user.        N).
+00001540: 7214 0000 0072 1500 0000 723a 0000 0029  r....r....r:...)
+00001550: 0372 1700 0000 723a 0000 0072 1000 0000  .r....r:...r....
+00001560: 7218 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00001570: 1500 0000 b000 0000 7304 0000 0000 050e  ........s.......
+00001580: 017a 2252 6574 7269 6576 6554 656e 616e  .z"RetrieveTenan
+00001590: 7455 7365 7252 6571 7565 7374 2e5f 5f69  tUserRequest.__i
+000015a0: 6e69 745f 5f72 1c00 0000 721a 0000 0072  nit__r....r....r
+000015b0: 1a00 0000 7218 0000 0072 1b00 0000 7239  ....r....r....r9
+000015c0: 0000 00ab 0000 0073 0800 0000 0802 0200  .......s........
+000015d0: 08ff 0404 7239 0000 0063 0000 0000 0000  ....r9...c......
+000015e0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+000015f0: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
+00001600: 0164 0264 0364 049c 0269 015a 0365 046a  .d.d.d...i.Z.e.j
+00001610: 0565 0664 0564 069c 0387 0066 0164 0764  .e.d.d.....f.d.d
+00001620: 0884 0c5a 0787 0004 005a 0853 0029 09da  ...Z.....Z.S.)..
+00001630: 1a52 6574 7269 6576 6554 656e 616e 7455  .RetrieveTenantU
+00001640: 7365 7252 6573 706f 6e73 65da 0b74 656e  serResponse..ten
+00001650: 616e 745f 7573 6572 5a0a 7465 6e61 6e74  ant_userZ.tenant
+00001660: 5573 6572 7237 0000 0072 0c00 0000 4e29  Userr7...r....N)
+00001670: 0372 3c00 0000 7210 0000 0072 1100 0000  .r<...r....r....
+00001680: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00001690: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
+000016a0: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+000016b0: 5f02 6401 5300 2902 7a51 0a20 2020 2020  _.d.S.).zQ.     
+000016c0: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+000016d0: 2020 2020 2020 2020 2020 2074 656e 616e             tenan
+000016e0: 745f 7573 6572 3a20 7465 6e61 6e74 5f75  t_user: tenant_u
+000016f0: 7365 7220 6461 7461 2072 6571 7565 7374  ser data request
+00001700: 6564 0a20 2020 2020 2020 204e 2903 7214  ed.        N).r.
+00001710: 0000 0072 1500 0000 723c 0000 0029 0372  ...r....r<...).r
+00001720: 1700 0000 723c 0000 0072 1000 0000 7218  ....r<...r....r.
+00001730: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00001740: 0000 be00 0000 7304 0000 0000 050e 017a  ......s........z
+00001750: 2352 6574 7269 6576 6554 656e 616e 7455  #RetrieveTenantU
+00001760: 7365 7252 6573 706f 6e73 652e 5f5f 696e  serResponse.__in
+00001770: 6974 5f5f 2909 721d 0000 0072 1e00 0000  it__).r....r....
+00001780: 721f 0000 0072 2000 0000 7238 0000 00da  r....r ...r8....
+00001790: 0a54 656e 616e 7455 7365 7272 0200 0000  .TenantUserr....
+000017a0: 7215 0000 0072 2100 0000 721a 0000 0072  r....r!...r....r
+000017b0: 1a00 0000 7218 0000 0072 1b00 0000 723b  ....r....r....r;
+000017c0: 0000 00b9 0000 0073 0800 0000 0802 0200  .......s........
+000017d0: 08ff 0404 723b 0000 0063 0000 0000 0000  ....r;...c......
+000017e0: 0000 0000 0000 0000 0000 0700 0000 0000  ................
+000017f0: 0000 735a 0000 0065 005a 0164 005a 0264  ..sZ...e.Z.d.Z.d
+00001800: 0164 0264 039c 0264 0464 0264 039c 0264  .d.d...d.d.d...d
+00001810: 0564 0664 039c 0264 079c 035a 0364 0c65  .d.d...d...Z.d.e
+00001820: 0465 0519 0065 0465 0519 0065 0465 0665  .e...e.e...e.e.e
+00001830: 0719 0019 0065 0864 0864 099c 0587 0066  .....e.d.d.....f
+00001840: 0164 0a64 0b84 0d5a 0987 0004 005a 0a53  .d.d...Z.....Z.S
+00001850: 0029 0dda 1446 696e 6450 726f 6365 7373  .)...FindProcess
+00001860: 6573 5265 7175 6573 74da 0470 6167 65da  esRequest..page.
+00001870: 0369 6e74 720c 0000 00da 0473 697a 65da  .intr......size.
+00001880: 0573 6f72 7473 fa05 5b73 7472 5d29 0372  .sorts..[str]).r
+00001890: 3f00 0000 7241 0000 0072 4200 0000 4e29  ?...rA...rB...N)
+000018a0: 0572 3f00 0000 7241 0000 0072 4200 0000  .r?...rA...rB...
+000018b0: 7210 0000 0072 1100 0000 6304 0000 0000  r....r....c.....
+000018c0: 0000 0000 0000 0005 0000 0003 0000 000b  ................
+000018d0: 0000 0073 2400 0000 7400 8300 6a01 6600  ...s$...t...j.f.
+000018e0: 7c04 8e01 0100 7c01 7c00 5f02 7c02 7c00  |.....|.|._.|.|.
+000018f0: 5f03 7c03 7c00 5f04 6401 5300 2902 7abe  _.|.|._.d.S.).z.
+00001900: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00001910: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00001920: 2070 6167 653a 2050 6167 6520 7265 7175   page: Page requ
+00001930: 6573 7465 642c 2030 2d69 6e64 6578 0a20  ested, 0-index. 
+00001940: 2020 2020 2020 2020 2020 2073 697a 653a             size:
+00001950: 2050 6167 6520 7369 7a65 0a20 2020 2020   Page size.     
+00001960: 2020 2020 2020 2073 6f72 7473 3a20 536f         sorts: So
+00001970: 7274 696e 6720 6372 6974 6572 6961 2069  rting criteria i
+00001980: 6e20 7468 6520 666f 726d 6174 3a20 7072  n the format: pr
+00001990: 6f70 6572 7479 7b2c 6173 637c 6465 7363  operty{,asc|desc
+000019a0: 7d2e 2045 7861 6d70 6c65 3a20 6e61 6d65  }. Example: name
+000019b0: 2c64 6573 630a 2020 2020 2020 2020 4e29  ,desc.        N)
+000019c0: 0572 1400 0000 7215 0000 0072 3f00 0000  .r....r....r?...
+000019d0: 7241 0000 0072 4200 0000 2905 7217 0000  rA...rB...).r...
+000019e0: 0072 3f00 0000 7241 0000 0072 4200 0000  .r?...rA...rB...
+000019f0: 7210 0000 0072 1800 0000 721a 0000 0072  r....r....r....r
+00001a00: 1b00 0000 7215 0000 00ce 0000 0073 0800  ....r........s..
+00001a10: 0000 0009 0e01 0601 0601 7a1d 4669 6e64  ..........z.Find
+00001a20: 5072 6f63 6573 7365 7352 6571 7565 7374  ProcessesRequest
+00001a30: 2e5f 5f69 6e69 745f 5f29 034e 4e4e 290b  .__init__).NNN).
+00001a40: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00001a50: 2000 0000 7205 0000 0072 4000 0000 7204   ...r....r@...r.
+00001a60: 0000 0072 0b00 0000 7202 0000 0072 1500  ...r....r....r..
+00001a70: 0000 7221 0000 0072 1a00 0000 721a 0000  ..r!...r....r...
+00001a80: 0072 1800 0000 721b 0000 0072 3e00 0000  .r....r....r>...
+00001a90: c700 0000 731c 0000 0008 0208 0108 0108  ....s...........
+00001aa0: fd06 0700 0000 0000 ff02 0106 0006 000a  ................
+00001ab0: 0002 0102 fe72 3e00 0000 6300 0000 0000  .....r>...c.....
+00001ac0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00001ad0: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
+00001ae0: 6401 6401 6402 6403 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
+00001af0: 6a05 6506 6404 6405 9c03 8700 6601 6406  j.e.d.d.....f.d.
+00001b00: 6407 840c 5a07 8700 0400 5a08 5300 2908  d...Z.....Z.S.).
+00001b10: da15 4669 6e64 5072 6f63 6573 7365 7352  ..FindProcessesR
+00001b20: 6573 706f 6e73 65da 0970 726f 6365 7373  esponse..process
+00001b30: 6573 da0b 5072 6f63 6573 7350 6167 6572  es..ProcessPager
+00001b40: 0c00 0000 4e29 0372 4500 0000 7210 0000  ....N).rE...r...
+00001b50: 0072 1100 0000 6302 0000 0000 0000 0000  .r....c.........
+00001b60: 0000 0003 0000 0003 0000 000b 0000 0073  ...............s
+00001b70: 1800 0000 7400 8300 6a01 6600 7c02 8e01  ....t...j.f.|...
+00001b80: 0100 7c01 7c00 5f02 6401 5300 2902 7a62  ..|.|._.d.S.).zb
+00001b90: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00001ba0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00001bb0: 2070 726f 6365 7373 6573 3a20 5072 6f63   processes: Proc
+00001bc0: 6573 7320 7061 6765 2074 6861 7420 6d61  ess page that ma
+00001bd0: 7468 2074 6865 2072 6571 7565 7374 6564  th the requested
+00001be0: 2063 7269 7465 7269 610a 2020 2020 2020   criteria.      
+00001bf0: 2020 4e29 0372 1400 0000 7215 0000 0072    N).r....r....r
+00001c00: 4500 0000 2903 7217 0000 0072 4500 0000  E...).r....rE...
+00001c10: 7210 0000 0072 1800 0000 721a 0000 0072  r....r....r....r
+00001c20: 1b00 0000 7215 0000 00e2 0000 0073 0400  ....r........s..
+00001c30: 0000 0005 0e01 7a1e 4669 6e64 5072 6f63  ......z.FindProc
+00001c40: 6573 7365 7352 6573 706f 6e73 652e 5f5f  essesResponse.__
+00001c50: 696e 6974 5f5f 2909 721d 0000 0072 1e00  init__).r....r..
+00001c60: 0000 721f 0000 0072 2000 0000 7238 0000  ..r....r ...r8..
+00001c70: 0072 4600 0000 7202 0000 0072 1500 0000  .rF...r....r....
+00001c80: 7221 0000 0072 1a00 0000 721a 0000 0072  r!...r....r....r
+00001c90: 1800 0000 721b 0000 0072 4400 0000 dd00  ....r....rD.....
+00001ca0: 0000 7308 0000 0008 0202 0008 ff04 0472  ..s............r
+00001cb0: 4400 0000 6300 0000 0000 0000 0000 0000  D...c...........
+00001cc0: 0000 0000 0004 0000 0000 0000 0073 3400  .............s4.
+00001cd0: 0000 6500 5a01 6400 5a02 6401 6402 6403  ..e.Z.d.Z.d.d.d.
+00001ce0: 6404 9c02 6901 5a03 6504 6505 6405 6406  d...i.Z.e.e.d.d.
+00001cf0: 9c03 8700 6601 6407 6408 840c 5a06 8700  ....f.d.d...Z...
+00001d00: 0400 5a07 5300 2909 da16 5265 7472 6965  ..Z.S.)...Retrie
+00001d10: 7665 5072 6f63 6573 7352 6571 7565 7374  veProcessRequest
+00001d20: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00001d30: 0c00 0000 4e72 0f00 0000 6302 0000 0000  ....Nr....c.....
+00001d40: 0000 0000 0000 0003 0000 0003 0000 000b  ................
+00001d50: 0000 0073 1800 0000 7400 8300 6a01 6600  ...s....t...j.f.
+00001d60: 7c02 8e01 0100 7c01 7c00 5f02 6401 5300  |.....|.|._.d.S.
+00001d70: 2902 7a54 0a20 2020 2020 2020 2050 6172  ).zT.        Par
+00001d80: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+00001d90: 2020 2020 2070 726f 6365 7373 5f69 643a       process_id:
+00001da0: 2050 726f 6365 7373 2049 6465 6e74 6966   Process Identif
+00001db0: 6965 7220 746f 2072 6574 7269 6576 650a  ier to retrieve.
+00001dc0: 2020 2020 2020 2020 4e72 1300 0000 7216          Nr....r.
+00001dd0: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
+00001de0: 0000 7215 0000 00f0 0000 0073 0400 0000  ..r........s....
+00001df0: 0005 0e01 7a1f 5265 7472 6965 7665 5072  ....z.RetrievePr
+00001e00: 6f63 6573 7352 6571 7565 7374 2e5f 5f69  ocessRequest.__i
+00001e10: 6e69 745f 5f72 1c00 0000 721a 0000 0072  nit__r....r....r
+00001e20: 1a00 0000 7218 0000 0072 1b00 0000 7247  ....r....r....rG
+00001e30: 0000 00eb 0000 0073 0800 0000 0802 0200  .......s........
+00001e40: 08ff 0404 7247 0000 0063 0000 0000 0000  ....rG...c......
+00001e50: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00001e60: 0000 7336 0000 0065 005a 0164 005a 0264  ..s6...e.Z.d.Z.d
+00001e70: 0164 0164 0264 039c 0269 015a 0365 046a  .d.d.d...i.Z.e.j
+00001e80: 0565 0664 0464 059c 0387 0066 0164 0664  .e.d.d.....f.d.d
+00001e90: 0784 0c5a 0787 0004 005a 0853 0029 08da  ...Z.....Z.S.)..
+00001ea0: 1752 6574 7269 6576 6550 726f 6365 7373  .RetrieveProcess
+00001eb0: 5265 7370 6f6e 7365 da07 7072 6f63 6573  Response..proces
+00001ec0: 73da 0750 726f 6365 7373 720c 0000 004e  s..Processr....N
+00001ed0: a903 7249 0000 0072 1000 0000 7211 0000  ..rI...r....r...
+00001ee0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00001ef0: 0000 0300 0000 0b00 0000 7318 0000 0074  ..........s....t
+00001f00: 0083 006a 0166 007c 028e 0101 007c 017c  ...j.f.|.....|.|
+00001f10: 005f 0264 0153 0029 027a 490a 2020 2020  ._.d.S.).zI.    
+00001f20: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+00001f30: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+00001f40: 6573 733a 2052 6571 7565 7374 6564 2070  ess: Requested p
+00001f50: 726f 6365 7373 2064 6174 610a 2020 2020  rocess data.    
+00001f60: 2020 2020 4ea9 0372 1400 0000 7215 0000      N..r....r...
+00001f70: 0072 4900 0000 a903 7217 0000 0072 4900  .rI.....r....rI.
+00001f80: 0000 7210 0000 0072 1800 0000 721a 0000  ..r....r....r...
+00001f90: 0072 1b00 0000 7215 0000 00fe 0000 0073  .r....r........s
+00001fa0: 0400 0000 0005 0e01 7a20 5265 7472 6965  ........z Retrie
+00001fb0: 7665 5072 6f63 6573 7352 6573 706f 6e73  veProcessRespons
+00001fc0: 652e 5f5f 696e 6974 5f5f a909 721d 0000  e.__init__..r...
+00001fd0: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00001fe0: 7238 0000 0072 4a00 0000 7202 0000 0072  r8...rJ...r....r
+00001ff0: 1500 0000 7221 0000 0072 1a00 0000 721a  ....r!...r....r.
+00002000: 0000 0072 1800 0000 721b 0000 0072 4800  ...r....r....rH.
+00002010: 0000 f900 0000 7308 0000 0008 0202 0008  ......s.........
+00002020: ff04 0472 4800 0000 6300 0000 0000 0000  ...rH...c.......
+00002030: 0000 0000 0000 0000 0007 0000 0000 0000  ................
+00002040: 0073 5400 0000 6500 5a01 6400 5a02 6401  .sT...e.Z.d.Z.d.
+00002050: 6402 6403 9c02 6404 6402 6403 9c02 6405  d.d...d.d.d...d.
+00002060: 6406 6403 9c02 6407 9c03 5a03 640c 6504  d.d...d...Z.d.e.
+00002070: 6504 6505 6506 6507 6a08 1900 1900 6509  e.e.e.e.j.....e.
+00002080: 6408 6409 9c05 8700 6601 640a 640b 840d  d.d.....f.d.d...
+00002090: 5a0a 8700 0400 5a0b 5300 290d da19 5361  Z.....Z.S.)...Sa
+000020a0: 7665 5072 6f63 6573 7345 6c65 6d65 6e74  veProcessElement
+000020b0: 5265 7175 6573 7472 0a00 0000 720b 0000  Requestr....r...
+000020c0: 0072 0c00 0000 da15 656c 656d 656e 7444  .r......elementD
+000020d0: 6566 696e 6974 696f 6e43 6f64 65da 0d65  efinitionCode..e
+000020e0: 6c65 6d65 6e74 5661 6c75 6573 7a15 5b50  lementValuesz.[P
+000020f0: 726f 6365 7373 456c 656d 656e 7456 616c  rocessElementVal
+00002100: 7565 5d29 0372 0900 0000 da17 656c 656d  ue]).r......elem
+00002110: 656e 745f 6465 6669 6e69 7469 6f6e 5f63  ent_definition_c
+00002120: 6f64 65da 0e65 6c65 6d65 6e74 5f76 616c  ode..element_val
+00002130: 7565 734e 2905 7209 0000 0072 5200 0000  uesN).r....rR...
+00002140: 7253 0000 0072 1000 0000 7211 0000 0063  rS...r....r....c
+00002150: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00002160: 0300 0000 0b00 0000 7328 0000 0074 0083  ........s(...t..
+00002170: 006a 0166 007c 048e 0101 007c 017c 005f  .j.f.|.....|.|._
+00002180: 027c 027c 005f 037c 0370 2067 007c 005f  .|.|._.|.p g.|._
+00002190: 0464 0153 0029 027a ba0a 2020 2020 2020  .d.S.).z..      
+000021a0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+000021b0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+000021c0: 735f 6964 3a20 5072 6f63 6573 7320 6964  s_id: Process id
+000021d0: 656e 7469 6669 6572 2074 6f20 7570 6461  entifier to upda
+000021e0: 7465 0a20 2020 2020 2020 2020 2020 2065  te.            e
+000021f0: 6c65 6d65 6e74 5f64 6566 696e 6974 696f  lement_definitio
+00002200: 6e5f 636f 6465 3a20 456c 656d 656e 7420  n_code: Element 
+00002210: 6465 6669 6e69 7469 6f6e 2063 6f64 650a  definition code.
+00002220: 2020 2020 2020 2020 2020 2020 656c 656d              elem
+00002230: 656e 745f 7661 6c75 6573 3a20 456c 656d  ent_values: Elem
+00002240: 656e 7420 7661 6c75 6573 0a20 2020 2020  ent values.     
+00002250: 2020 204e 2905 7214 0000 0072 1500 0000     N).r....r....
+00002260: 7209 0000 0072 5200 0000 7253 0000 0029  r....rR...rS...)
+00002270: 0572 1700 0000 7209 0000 0072 5200 0000  .r....r....rR...
+00002280: 7253 0000 0072 1000 0000 7218 0000 0072  rS...r....r....r
+00002290: 1a00 0000 721b 0000 0072 1500 0000 0e01  ....r....r......
+000022a0: 0000 7308 0000 0000 0d0e 0106 0106 017a  ..s............z
+000022b0: 2253 6176 6550 726f 6365 7373 456c 656d  "SaveProcessElem
+000022c0: 656e 7452 6571 7565 7374 2e5f 5f69 6e69  entRequest.__ini
+000022d0: 745f 5f29 014e 290c 721d 0000 0072 1e00  t__).N).r....r..
+000022e0: 0000 721f 0000 0072 2000 0000 720b 0000  ..r....r ...r...
+000022f0: 0072 0500 0000 7204 0000 0072 3800 0000  .r....r....r8...
+00002300: da13 5072 6f63 6573 7345 6c65 6d65 6e74  ..ProcessElement
+00002310: 5661 6c75 6572 0200 0000 7215 0000 0072  Valuer....r....r
+00002320: 2100 0000 721a 0000 0072 1a00 0000 7218  !...r....r....r.
+00002330: 0000 0072 1b00 0000 724f 0000 0007 0100  ...r....rO......
+00002340: 0073 1800 0000 0802 0801 0801 08fd 060a  .s..............
+00002350: 00fc 0202 0201 0201 0c01 0201 02fa 724f  ..............rO
+00002360: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002370: 0000 0000 0400 0000 0000 0000 7336 0000  ............s6..
+00002380: 0065 005a 0164 005a 0264 0164 0164 0264  .e.Z.d.Z.d.d.d.d
+00002390: 039c 0269 015a 0365 046a 0565 0664 0464  ...i.Z.e.j.e.d.d
+000023a0: 059c 0387 0066 0164 0664 0784 0c5a 0787  .....f.d.d...Z..
+000023b0: 0004 005a 0853 0029 08da 1a53 6176 6550  ...Z.S.)...SaveP
+000023c0: 726f 6365 7373 456c 656d 656e 7452 6573  rocessElementRes
+000023d0: 706f 6e73 6572 4900 0000 724a 0000 0072  ponserI...rJ...r
+000023e0: 0c00 0000 4e72 4b00 0000 6302 0000 0000  ....NrK...c.....
+000023f0: 0000 0000 0000 0003 0000 0003 0000 000b  ................
+00002400: 0000 0073 1800 0000 7400 8300 6a01 6600  ...s....t...j.f.
+00002410: 7c02 8e01 0100 7c01 7c00 5f02 6401 5300  |.....|.|._.d.S.
+00002420: a902 7a42 0a20 2020 2020 2020 2050 6172  ..zB.        Par
+00002430: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+00002440: 2020 2020 2070 726f 6365 7373 3a20 5072       process: Pr
+00002450: 6f63 6573 7320 7570 6461 7465 640a 2020  ocess updated.  
+00002460: 2020 2020 2020 4e72 4c00 0000 724d 0000        NrL...rM..
+00002470: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00002480: 7215 0000 0026 0100 0073 0400 0000 0005  r....&...s......
+00002490: 0e01 7a23 5361 7665 5072 6f63 6573 7345  ..z#SaveProcessE
+000024a0: 6c65 6d65 6e74 5265 7370 6f6e 7365 2e5f  lementResponse._
+000024b0: 5f69 6e69 745f 5f72 4e00 0000 721a 0000  _init__rN...r...
+000024c0: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
+000024d0: 7255 0000 0021 0100 0073 0800 0000 0802  rU...!...s......
+000024e0: 0200 08ff 0404 7255 0000 0063 0000 0000  ......rU...c....
+000024f0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00002500: 0000 0000 734c 0000 0065 005a 0164 005a  ....sL...e.Z.d.Z
+00002510: 0264 0164 0264 039c 0264 0464 0564 039c  .d.d.d...d.d.d..
+00002520: 0264 069c 025a 0364 0b65 0465 0565 0665  .d...Z.d.e.e.e.e
+00002530: 0465 0766 0219 0019 0065 0764 0764 089c  .e.f.....e.d.d..
+00002540: 0487 0066 0164 0964 0a84 0d5a 0887 0004  ...f.d.d...Z....
+00002550: 005a 0953 0029 0cda 1c53 6176 6550 726f  .Z.S.)...SavePro
+00002560: 6365 7373 456e 7469 7479 4461 7461 5265  cessEntityDataRe
+00002570: 7175 6573 7472 0a00 0000 720b 0000 0072  questr....r....r
+00002580: 0c00 0000 da04 6461 7461 fa08 7b6f 626a  ......data..{obj
+00002590: 6563 747d 2902 7209 0000 0072 5800 0000  ect}).r....rX...
+000025a0: 4e29 0472 0900 0000 7258 0000 0072 1000  N).r....rX...r..
+000025b0: 0000 7211 0000 0063 0300 0000 0000 0000  ..r....c........
+000025c0: 0000 0000 0400 0000 0300 0000 0b00 0000  ................
+000025d0: 7322 0000 0074 0083 006a 0166 007c 038e  s"...t...j.f.|..
+000025e0: 0101 007c 017c 005f 027c 0270 1a69 007c  ...|.|._.|.p.i.|
+000025f0: 005f 0364 0153 0029 027a 700a 2020 2020  ._.d.S.).zp.    
+00002600: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+00002610: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
+00002620: 6573 735f 6964 3a20 5072 6f63 6573 7320  ess_id: Process 
+00002630: 6964 656e 7469 6669 6572 2074 6f20 7570  identifier to up
+00002640: 6461 7465 0a20 2020 2020 2020 2020 2020  date.           
+00002650: 2064 6174 613a 2044 6174 6120 7661 6c75   data: Data valu
+00002660: 6573 0a20 2020 2020 2020 204e 2904 7214  es.        N).r.
+00002670: 0000 0072 1500 0000 7209 0000 0072 5800  ...r....r....rX.
+00002680: 0000 2904 7217 0000 0072 0900 0000 7258  ..).r....r....rX
+00002690: 0000 0072 1000 0000 7218 0000 0072 1a00  ...r....r....r..
+000026a0: 0000 721b 0000 0072 1500 0000 3501 0000  ..r....r....5...
+000026b0: 7306 0000 0000 0b0e 0106 017a 2553 6176  s..........z%Sav
+000026c0: 6550 726f 6365 7373 456e 7469 7479 4461  eProcessEntityDa
+000026d0: 7461 5265 7175 6573 742e 5f5f 696e 6974  taRequest.__init
+000026e0: 5f5f 2901 4ea9 0a72 1d00 0000 721e 0000  __).N..r....r...
+000026f0: 0072 1f00 0000 7220 0000 0072 0b00 0000  .r....r ...r....
+00002700: 7205 0000 0072 0300 0000 7202 0000 0072  r....r....r....r
+00002710: 1500 0000 7221 0000 0072 1a00 0000 721a  ....r!...r....r.
+00002720: 0000 0072 1800 0000 721b 0000 0072 5700  ...r....r....rW.
+00002730: 0000 2f01 0000 7314 0000 0008 0208 0108  ../...s.........
+00002740: fe06 0800 fd02 0202 010e 0102 0102 fb72  ...............r
+00002750: 5700 0000 6300 0000 0000 0000 0000 0000  W...c...........
+00002760: 0000 0000 0004 0000 0000 0000 0073 3600  .............s6.
+00002770: 0000 6500 5a01 6400 5a02 6401 6401 6402  ..e.Z.d.Z.d.d.d.
+00002780: 6403 9c02 6901 5a03 6504 6a05 6506 6404  d...i.Z.e.j.e.d.
+00002790: 6405 9c03 8700 6601 6406 6407 840c 5a07  d.....f.d.d...Z.
+000027a0: 8700 0400 5a08 5300 2908 da1d 5361 7665  ....Z.S.)...Save
+000027b0: 5072 6f63 6573 7345 6e74 6974 7944 6174  ProcessEntityDat
+000027c0: 6152 6573 706f 6e73 6572 4900 0000 724a  aResponserI...rJ
+000027d0: 0000 0072 0c00 0000 4e72 4b00 0000 6302  ...r....NrK...c.
+000027e0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000027f0: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
+00002800: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
+00002810: 6401 5300 7256 0000 0072 4c00 0000 724d  d.S.rV...rL...rM
+00002820: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
+00002830: 0000 7215 0000 004a 0100 0073 0400 0000  ..r....J...s....
+00002840: 0005 0e01 7a26 5361 7665 5072 6f63 6573  ....z&SaveProces
+00002850: 7345 6e74 6974 7944 6174 6152 6573 706f  sEntityDataRespo
+00002860: 6e73 652e 5f5f 696e 6974 5f5f 724e 0000  nse.__init__rN..
+00002870: 0072 1a00 0000 721a 0000 0072 1800 0000  .r....r....r....
+00002880: 721b 0000 0072 5b00 0000 4501 0000 7308  r....r[...E...s.
+00002890: 0000 0008 0202 0008 ff04 0472 5b00 0000  ...........r[...
+000028a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000028b0: 0005 0000 0000 0000 0073 3e00 0000 6500  .........s>...e.
+000028c0: 5a01 6400 5a02 6401 6402 6403 9c02 6404  Z.d.Z.d.d.d...d.
+000028d0: 6402 6403 9c02 6405 9c02 5a03 6504 6504  d.d...d...Z.e.e.
+000028e0: 6505 6406 6407 9c04 8700 6601 6408 6409  e.d.d.....f.d.d.
+000028f0: 840c 5a06 8700 0400 5a07 5300 290a da1b  ..Z.....Z.S.)...
+00002900: 4465 6c65 7465 5072 6f63 6573 7345 6c65  DeleteProcessEle
+00002910: 6d65 6e74 5265 7175 6573 7472 0a00 0000  mentRequestr....
+00002920: 720b 0000 0072 0c00 0000 7250 0000 0029  r....r....rP...)
+00002930: 0272 0900 0000 7252 0000 004e 2904 7209  .r....rR...N).r.
+00002940: 0000 0072 5200 0000 7210 0000 0072 1100  ...rR...r....r..
+00002950: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
+00002960: 0000 0003 0000 000b 0000 0073 1e00 0000  ...........s....
+00002970: 7400 8300 6a01 6600 7c03 8e01 0100 7c01  t...j.f.|.....|.
+00002980: 7c00 5f02 7c02 7c00 5f03 6401 5300 2902  |._.|.|._.d.S.).
+00002990: 7a88 0a20 2020 2020 2020 2050 6172 616d  z..        Param
+000029a0: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+000029b0: 2020 2070 726f 6365 7373 5f69 643a 2050     process_id: P
+000029c0: 726f 6365 7373 2072 656c 6174 6564 0a20  rocess related. 
+000029d0: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
+000029e0: 6e74 5f64 6566 696e 6974 696f 6e5f 636f  nt_definition_co
+000029f0: 6465 3a20 436f 6465 206f 6620 7468 6520  de: Code of the 
+00002a00: 656c 656d 656e 7420 746f 2064 656c 6574  element to delet
+00002a10: 650a 2020 2020 2020 2020 4e29 0472 1400  e.        N).r..
+00002a20: 0000 7215 0000 0072 0900 0000 7252 0000  ..r....r....rR..
+00002a30: 0029 0472 1700 0000 7209 0000 0072 5200  .).r....r....rR.
+00002a40: 0000 7210 0000 0072 1800 0000 721a 0000  ..r....r....r...
+00002a50: 0072 1b00 0000 7215 0000 0059 0100 0073  .r....r....Y...s
+00002a60: 0600 0000 0006 0e01 0601 7a24 4465 6c65  ..........z$Dele
+00002a70: 7465 5072 6f63 6573 7345 6c65 6d65 6e74  teProcessElement
+00002a80: 5265 7175 6573 742e 5f5f 696e 6974 5f5f  Request.__init__
+00002a90: 721c 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00002aa0: 1800 0000 721b 0000 0072 5c00 0000 5301  ....r....r\...S.
+00002ab0: 0000 7308 0000 0008 0208 0108 fe06 0572  ..s............r
+00002ac0: 5c00 0000 6300 0000 0000 0000 0000 0000  \...c...........
+00002ad0: 0000 0000 0004 0000 0000 0000 0073 3600  .............s6.
+00002ae0: 0000 6500 5a01 6400 5a02 6401 6401 6402  ..e.Z.d.Z.d.d.d.
+00002af0: 6403 9c02 6901 5a03 6504 6a05 6506 6404  d...i.Z.e.j.e.d.
+00002b00: 6405 9c03 8700 6601 6406 6407 840c 5a07  d.....f.d.d...Z.
+00002b10: 8700 0400 5a08 5300 2908 da1c 4465 6c65  ....Z.S.)...Dele
+00002b20: 7465 5072 6f63 6573 7345 6c65 6d65 6e74  teProcessElement
+00002b30: 5265 7370 6f6e 7365 7249 0000 0072 4a00  ResponserI...rJ.
+00002b40: 0000 720c 0000 004e 724b 0000 0063 0200  ..r....NrK...c..
+00002b50: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00002b60: 0000 0b00 0000 7318 0000 0074 0083 006a  ......s....t...j
+00002b70: 0166 007c 028e 0101 007c 017c 005f 0264  .f.|.....|.|._.d
+00002b80: 0153 0072 5600 0000 724c 0000 0072 4d00  .S.rV...rL...rM.
+00002b90: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00002ba0: 0072 1500 0000 6901 0000 7304 0000 0000  .r....i...s.....
+00002bb0: 050e 017a 2544 656c 6574 6550 726f 6365  ...z%DeleteProce
+00002bc0: 7373 456c 656d 656e 7452 6573 706f 6e73  ssElementRespons
+00002bd0: 652e 5f5f 696e 6974 5f5f 724e 0000 0072  e.__init__rN...r
+00002be0: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
+00002bf0: 0000 0072 5d00 0000 6401 0000 7308 0000  ...r]...d...s...
+00002c00: 0008 0202 0008 ff04 0472 5d00 0000 6300  .........r]...c.
+00002c10: 0000 0000 0000 0000 0000 0000 0000 0007  ................
+00002c20: 0000 0000 0000 0073 5200 0000 6500 5a01  .......sR...e.Z.
+00002c30: 6400 5a02 6401 6402 6403 9c02 6404 6402  d.Z.d.d.d...d.d.
+00002c40: 6403 9c02 6405 6402 6403 9c02 6406 9c03  d...d.d.d...d...
+00002c50: 5a03 640b 6504 6505 6504 1900 6505 6504  Z.d.e.e.e...e.e.
+00002c60: 1900 6506 6407 6408 9c05 8700 6601 6409  ..e.d.d.....f.d.
+00002c70: 640a 840d 5a07 8700 0400 5a08 5300 290c  d...Z.....Z.S.).
+00002c80: da1d 4368 616e 6765 5072 6f63 6573 7349  ..ChangeProcessI
+00002c90: 6e69 7469 6174 6f72 5265 7175 6573 7472  nitiatorRequestr
+00002ca0: 0a00 0000 720b 0000 0072 0c00 0000 da05  ....r....r......
+00002cb0: 656d 6169 6c72 3400 0000 2903 7209 0000  emailr4...).r...
+00002cc0: 0072 5f00 0000 7233 0000 004e 2905 7209  .r_...r3...N).r.
+00002cd0: 0000 0072 5f00 0000 7233 0000 0072 1000  ...r_...r3...r..
+00002ce0: 0000 7211 0000 0063 0400 0000 0000 0000  ..r....c........
+00002cf0: 0000 0000 0500 0000 0300 0000 0b00 0000  ................
+00002d00: 7324 0000 0074 0083 006a 0166 007c 048e  s$...t...j.f.|..
+00002d10: 0101 007c 017c 005f 027c 027c 005f 037c  ...|.|._.|.|._.|
+00002d20: 037c 005f 0464 0153 0029 0261 7b01 0000  .|._.d.S.).a{...
+00002d30: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00002d40: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00002d50: 2070 726f 6365 7373 5f69 643a 2050 726f   process_id: Pro
+00002d60: 6365 7373 2069 6465 6e74 6966 6965 7220  cess identifier 
+00002d70: 746f 2077 6869 6368 2077 616e 7420 746f  to which want to
+00002d80: 2063 6861 6e67 6520 7468 6520 696e 6974   change the init
+00002d90: 6961 746f 720a 2020 2020 2020 2020 2020  iator.          
+00002da0: 2020 656d 6169 6c3a 2055 7365 7220 656d    email: User em
+00002db0: 6169 6c20 7468 6174 2077 616e 7420 746f  ail that want to
+00002dc0: 2075 7365 2074 6f20 6173 7369 676e 2074   use to assign t
+00002dd0: 6865 2070 726f 6365 7373 2e20 4174 7472  he process. Attr
+00002de0: 6962 7574 6520 3a65 6d61 696c 206f 7220  ibute :email or 
+00002df0: 3a70 7269 6e63 6970 616c 5f69 6420 6d75  :principal_id mu
+00002e00: 7374 2062 6520 7365 742e 0a20 2020 2020  st be set..     
+00002e10: 2020 2020 2020 2070 7269 6e63 6970 616c         principal
+00002e20: 5f69 643a 2050 7269 6e63 6970 616c 2069  _id: Principal i
+00002e30: 6420 7468 6174 2077 616e 7420 746f 2075  d that want to u
+00002e40: 7365 2074 6f20 6173 7369 676e 2074 6865  se to assign the
+00002e50: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
+00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e70: 2020 2020 4174 7472 6962 7574 6520 3a65      Attribute :e
+00002e80: 6d61 696c 206f 7220 3a70 7269 6e63 6970  mail or :princip
+00002e90: 616c 5f69 6420 6d75 7374 2062 6520 7365  al_id must be se
+00002ea0: 742e 0a20 2020 2020 2020 204e 2905 7214  t..        N).r.
+00002eb0: 0000 0072 1500 0000 7209 0000 0072 5f00  ...r....r....r_.
+00002ec0: 0000 7233 0000 0029 0572 1700 0000 7209  ..r3...).r....r.
+00002ed0: 0000 0072 5f00 0000 7233 0000 0072 1000  ...r_...r3...r..
+00002ee0: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00002ef0: 0072 1500 0000 7901 0000 7308 0000 0000  .r....y...s.....
+00002f00: 0a0e 0106 0106 017a 2643 6861 6e67 6550  .......z&ChangeP
+00002f10: 726f 6365 7373 496e 6974 6961 746f 7252  rocessInitiatorR
+00002f20: 6571 7565 7374 2e5f 5f69 6e69 745f 5f29  equest.__init__)
+00002f30: 024e 4ea9 0972 1d00 0000 721e 0000 0072  .NN..r....r....r
+00002f40: 1f00 0000 7220 0000 0072 0b00 0000 7205  ....r ...r....r.
+00002f50: 0000 0072 0200 0000 7215 0000 0072 2100  ...r....r....r!.
+00002f60: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
+00002f70: 0072 1b00 0000 725e 0000 0072 0100 0073  .r....r^...r...s
+00002f80: 1a00 0000 0802 0801 0801 08fd 0607 0000  ................
+00002f90: 00ff 0201 0200 0600 0600 0201 02fe 725e  ..............r^
+00002fa0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002fb0: 0000 0000 0400 0000 0000 0000 7336 0000  ............s6..
+00002fc0: 0065 005a 0164 005a 0264 0164 0164 0264  .e.Z.d.Z.d.d.d.d
+00002fd0: 039c 0269 015a 0365 046a 0565 0664 0464  ...i.Z.e.j.e.d.d
+00002fe0: 059c 0387 0066 0164 0664 0784 0c5a 0787  .....f.d.d...Z..
+00002ff0: 0004 005a 0853 0029 08da 1e43 6861 6e67  ...Z.S.)...Chang
+00003000: 6550 726f 6365 7373 496e 6974 6961 746f  eProcessInitiato
+00003010: 7252 6573 706f 6e73 6572 4900 0000 724a  rResponserI...rJ
+00003020: 0000 0072 0c00 0000 4e72 4b00 0000 6302  ...r....NrK...c.
+00003030: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00003040: 0000 000b 0000 0073 1800 0000 7400 8300  .......s....t...
+00003050: 6a01 6600 7c02 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
+00003060: 6401 5300 7256 0000 0072 4c00 0000 724d  d.S.rV...rL...rM
+00003070: 0000 0072 1800 0000 721a 0000 0072 1b00  ...r....r....r..
+00003080: 0000 7215 0000 008e 0100 0073 0400 0000  ..r........s....
+00003090: 0005 0e01 7a27 4368 616e 6765 5072 6f63  ....z'ChangeProc
+000030a0: 6573 7349 6e69 7469 6174 6f72 5265 7370  essInitiatorResp
+000030b0: 6f6e 7365 2e5f 5f69 6e69 745f 5f72 4e00  onse.__init__rN.
+000030c0: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
+000030d0: 0072 1b00 0000 7261 0000 0089 0100 0073  .r....ra.......s
+000030e0: 0800 0000 0802 0200 08ff 0404 7261 0000  ............ra..
+000030f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003100: 0000 0a00 0000 0000 0000 7392 0000 0065  ..........s....e
+00003110: 005a 0164 005a 0264 0164 0264 039c 0264  .Z.d.Z.d.d.d...d
+00003120: 0464 0264 039c 0264 0564 0664 039c 0264  .d.d...d.d.d...d
+00003130: 0764 0664 039c 0264 0864 0964 039c 0264  .d.d...d.d.d...d
+00003140: 0a64 0664 039c 0264 0b9c 065a 0364 1065  .d.d...d...Z.d.e
+00003150: 0465 0519 0065 0465 0519 0065 0465 0665  .e...e.e...e.e.e
+00003160: 0719 0019 0065 0465 0665 0719 0019 0065  .....e.e.e.....e
+00003170: 0465 0665 086a 0919 0019 0065 0465 0665  .e.e.j.....e.e.e
+00003180: 0719 0019 0065 0a64 0c64 0d9c 0887 0066  .....e.d.d.....f
+00003190: 0164 0e64 0f84 0d5a 0b87 0004 005a 0c53  .d.d...Z.....Z.S
+000031a0: 0029 11da 0f46 696e 6454 6173 6b52 6571  .)...FindTaskReq
+000031b0: 7565 7374 723f 0000 0072 4000 0000 720c  uestr?...r@...r.
+000031c0: 0000 0072 4100 0000 7242 0000 0072 4300  ...rA...rB...rC.
+000031d0: 0000 5a0a 7072 6f63 6573 7349 6473 da06  ..Z.processIds..
+000031e0: 7374 6174 6573 7a0b 5b54 6173 6b53 7461  statesz.[TaskSta
+000031f0: 7465 5d5a 1374 6173 6b44 6566 696e 6974  te]Z.taskDefinit
+00003200: 696f 6e43 6f64 6573 2906 723f 0000 0072  ionCodes).r?...r
+00003210: 4100 0000 7242 0000 00da 0b70 726f 6365  A...rB.....proce
+00003220: 7373 5f69 6473 7263 0000 00da 1574 6173  ss_idsrc.....tas
+00003230: 6b5f 6465 6669 6e69 7469 6f6e 5f63 6f64  k_definition_cod
+00003240: 6573 4e29 0872 3f00 0000 7241 0000 0072  esN).r?...rA...r
+00003250: 4200 0000 7264 0000 0072 6300 0000 7265  B...rd...rc...re
+00003260: 0000 0072 1000 0000 7211 0000 0063 0700  ...r....r....c..
+00003270: 0000 0000 0000 0000 0000 0800 0000 0300  ................
+00003280: 0000 0b00 0000 7336 0000 0074 0083 006a  ......s6...t...j
+00003290: 0166 007c 078e 0101 007c 017c 005f 027c  .f.|.....|.|._.|
+000032a0: 027c 005f 037c 037c 005f 047c 047c 005f  .|._.|.|._.|.|._
+000032b0: 057c 057c 005f 067c 067c 005f 0764 0153  .|.|._.|.|._.d.S
+000032c0: 0029 0261 7b01 0000 0a20 2020 2020 2020  .).a{....       
+000032d0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+000032e0: 2020 2020 2020 2020 2070 6167 653a 2050           page: P
+000032f0: 6167 6520 7265 7175 6573 7465 642c 2030  age requested, 0
+00003300: 2d69 6e64 6578 0a20 2020 2020 2020 2020  -index.         
+00003310: 2020 2073 697a 653a 2050 6167 6520 7369     size: Page si
+00003320: 7a65 0a20 2020 2020 2020 2020 2020 2073  ze.            s
+00003330: 6f72 7473 3a20 536f 7274 696e 6720 6372  orts: Sorting cr
+00003340: 6974 6572 6961 2069 6e20 7468 6520 666f  iteria in the fo
+00003350: 726d 6174 3a20 7072 6f70 6572 7479 7b2c  rmat: property{,
+00003360: 6173 637c 6465 7363 7d2e 2045 7861 6d70  asc|desc}. Examp
+00003370: 6c65 3a20 6e61 6d65 2c64 6573 630a 2020  le: name,desc.  
+00003380: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+00003390: 735f 6964 733a 2046 696c 7465 7220 7461  s_ids: Filter ta
+000033a0: 736b 7320 6279 2074 6865 2070 726f 6365  sks by the proce
+000033b0: 7373 2069 6465 6e74 6966 6965 7273 0a20  ss identifiers. 
+000033c0: 2020 2020 2020 2020 2020 2073 7461 7465             state
+000033d0: 733a 2046 696c 7465 7220 7461 736b 7320  s: Filter tasks 
+000033e0: 6279 2074 6865 2073 7461 7465 730a 2020  by the states.  
+000033f0: 2020 2020 2020 2020 2020 7461 736b 5f64            task_d
+00003400: 6566 696e 6974 696f 6e5f 636f 6465 733a  efinition_codes:
+00003410: 2046 696c 7465 7220 7461 736b 7320 6279   Filter tasks by
+00003420: 2074 6865 2074 6173 6b5f 6465 6669 6e69   the task_defini
+00003430: 7469 6f6e 5f63 6f64 6573 0a20 2020 2020  tion_codes.     
+00003440: 2020 204e 2908 7214 0000 0072 1500 0000     N).r....r....
+00003450: 723f 0000 0072 4100 0000 7242 0000 0072  r?...rA...rB...r
+00003460: 6400 0000 7263 0000 0072 6500 0000 2908  d...rc...re...).
+00003470: 7217 0000 0072 3f00 0000 7241 0000 0072  r....r?...rA...r
+00003480: 4200 0000 7264 0000 0072 6300 0000 7265  B...rd...rc...re
+00003490: 0000 0072 1000 0000 7218 0000 0072 1a00  ...r....r....r..
+000034a0: 0000 721b 0000 0072 1500 0000 a101 0000  ..r....r........
+000034b0: 730e 0000 0000 130e 0106 0106 0106 0106  s...............
+000034c0: 0106 017a 1846 696e 6454 6173 6b52 6571  ...z.FindTaskReq
+000034d0: 7565 7374 2e5f 5f69 6e69 745f 5f29 064e  uest.__init__).N
+000034e0: 4e4e 4e4e 4e29 0d72 1d00 0000 721e 0000  NNNNN).r....r...
+000034f0: 0072 1f00 0000 7220 0000 0072 0500 0000  .r....r ...r....
+00003500: 7240 0000 0072 0400 0000 720b 0000 0072  r@...r....r....r
+00003510: 3800 0000 da09 5461 736b 5374 6174 6572  8.....TaskStater
+00003520: 0200 0000 7215 0000 0072 2100 0000 721a  ....r....r!...r.
+00003530: 0000 0072 1a00 0000 7218 0000 0072 1b00  ...r....r....r..
+00003540: 0000 7262 0000 0097 0100 0073 2e00 0000  ..rb.......s....
+00003550: 0802 0801 0801 0801 0801 0801 08fa 060b  ................
+00003560: 0001 0001 0001 0001 0001 00f9 0202 0601  ................
+00003570: 0601 0a01 0a01 0c01 0a01 0201 02f7 7262  ..............rb
+00003580: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003590: 0000 0000 0400 0000 0000 0000 7336 0000  ............s6..
+000035a0: 0065 005a 0164 005a 0264 0164 0164 0264  .e.Z.d.Z.d.d.d.d
+000035b0: 039c 0269 015a 0365 046a 0565 0664 0464  ...i.Z.e.j.e.d.d
+000035c0: 059c 0387 0066 0164 0664 0784 0c5a 0787  .....f.d.d...Z..
+000035d0: 0004 005a 0853 0029 08da 1046 696e 6454  ...Z.S.)...FindT
+000035e0: 6173 6b52 6573 706f 6e73 65da 0574 6173  askResponse..tas
+000035f0: 6b73 da08 5461 736b 5061 6765 720c 0000  ks..TaskPager...
+00003600: 004e 2903 7268 0000 0072 1000 0000 7211  .N).rh...r....r.
+00003610: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003620: 0300 0000 0300 0000 0b00 0000 7318 0000  ............s...
+00003630: 0074 0083 006a 0166 007c 028e 0101 007c  .t...j.f.|.....|
+00003640: 017c 005f 0264 0153 0029 027a 5b0a 2020  .|._.d.S.).z[.  
+00003650: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00003660: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+00003670: 736b 733a 2054 6173 6b20 7061 6765 2074  sks: Task page t
+00003680: 6861 7420 6d61 7468 2074 6865 2072 6571  hat math the req
+00003690: 7565 7374 6564 2063 7269 7465 7269 610a  uested criteria.
+000036a0: 2020 2020 2020 2020 4e29 0372 1400 0000          N).r....
+000036b0: 7215 0000 0072 6800 0000 2903 7217 0000  r....rh...).r...
+000036c0: 0072 6800 0000 7210 0000 0072 1800 0000  .rh...r....r....
+000036d0: 721a 0000 0072 1b00 0000 7215 0000 00c2  r....r....r.....
+000036e0: 0100 0073 0400 0000 0005 0e01 7a19 4669  ...s........z.Fi
+000036f0: 6e64 5461 736b 5265 7370 6f6e 7365 2e5f  ndTaskResponse._
+00003700: 5f69 6e69 745f 5f29 0972 1d00 0000 721e  _init__).r....r.
+00003710: 0000 0072 1f00 0000 7220 0000 0072 3800  ...r....r ...r8.
+00003720: 0000 7269 0000 0072 0200 0000 7215 0000  ..ri...r....r...
+00003730: 0072 2100 0000 721a 0000 0072 1a00 0000  .r!...r....r....
+00003740: 7218 0000 0072 1b00 0000 7267 0000 00bd  r....r....rg....
+00003750: 0100 0073 0800 0000 0802 0200 08ff 0404  ...s............
+00003760: 7267 0000 0063 0000 0000 0000 0000 0000  rg...c..........
+00003770: 0000 0000 0000 0400 0000 0000 0000 7334  ..............s4
+00003780: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
+00003790: 0364 049c 0269 015a 0365 0465 0564 0564  .d...i.Z.e.e.d.d
+000037a0: 069c 0387 0066 0164 0764 0884 0c5a 0687  .....f.d.d...Z..
+000037b0: 0004 005a 0753 0029 09da 1352 6574 7269  ...Z.S.)...Retri
+000037c0: 6576 6554 6173 6b52 6571 7565 7374 7230  eveTaskRequestr0
+000037d0: 0000 0072 2f00 0000 720b 0000 0072 0c00  ...r/...r....r..
+000037e0: 0000 4ea9 0372 3000 0000 7210 0000 0072  ..N..r0...r....r
+000037f0: 1100 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00003800: 0003 0000 0003 0000 000b 0000 0073 1800  .............s..
+00003810: 0000 7400 8300 6a01 6600 7c02 8e01 0100  ..t...j.f.|.....
+00003820: 7c01 7c00 5f02 6401 5300 2902 7a4e 0a20  |.|._.d.S.).zN. 
+00003830: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00003840: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00003850: 6173 6b5f 6964 3a20 5461 736b 2069 6465  ask_id: Task ide
+00003860: 6e74 6966 6965 7220 746f 2072 6574 7269  ntifier to retri
+00003870: 6576 650a 2020 2020 2020 2020 4ea9 0372  eve.        N..r
+00003880: 1400 0000 7215 0000 0072 3000 0000 a903  ....r....r0.....
+00003890: 7217 0000 0072 3000 0000 7210 0000 0072  r....r0...r....r
+000038a0: 1800 0000 721a 0000 0072 1b00 0000 7215  ....r....r....r.
+000038b0: 0000 00d0 0100 0073 0400 0000 0005 0e01  .......s........
+000038c0: 7a1c 5265 7472 6965 7665 5461 736b 5265  z.RetrieveTaskRe
+000038d0: 7175 6573 742e 5f5f 696e 6974 5f5f 721c  quest.__init__r.
+000038e0: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
+000038f0: 0000 721b 0000 0072 6a00 0000 cb01 0000  ..r....rj.......
+00003900: 7308 0000 0008 0202 0008 ff04 0472 6a00  s............rj.
+00003910: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00003920: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
+00003930: 6500 5a01 6400 5a02 6401 6401 6402 6403  e.Z.d.Z.d.d.d.d.
+00003940: 9c02 6901 5a03 6504 6a05 6506 6404 6405  ..i.Z.e.j.e.d.d.
+00003950: 9c03 8700 6601 6406 6407 840c 5a07 8700  ....f.d.d...Z...
+00003960: 0400 5a08 5300 2908 da14 5265 7472 6965  ..Z.S.)...Retrie
+00003970: 7665 5461 736b 5265 7370 6f6e 7365 da04  veTaskResponse..
+00003980: 7461 736b da04 5461 736b 720c 0000 004e  task..Taskr....N
+00003990: a903 726f 0000 0072 1000 0000 7211 0000  ..ro...r....r...
+000039a0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+000039b0: 0000 0300 0000 0b00 0000 7318 0000 0074  ..........s....t
+000039c0: 0083 006a 0166 007c 028e 0101 007c 017c  ...j.f.|.....|.|
+000039d0: 005f 0264 0153 0029 027a 390a 2020 2020  ._.d.S.).z9.    
+000039e0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+000039f0: 2020 2020 2020 2020 2020 2020 7461 736b              task
+00003a00: 3a20 5461 736b 2064 6174 610a 2020 2020  : Task data.    
+00003a10: 2020 2020 4ea9 0372 1400 0000 7215 0000      N..r....r...
+00003a20: 0072 6f00 0000 a903 7217 0000 0072 6f00  .ro.....r....ro.
+00003a30: 0000 7210 0000 0072 1800 0000 721a 0000  ..r....r....r...
+00003a40: 0072 1b00 0000 7215 0000 00de 0100 0073  .r....r........s
+00003a50: 0400 0000 0005 0e01 7a1d 5265 7472 6965  ........z.Retrie
+00003a60: 7665 5461 736b 5265 7370 6f6e 7365 2e5f  veTaskResponse._
+00003a70: 5f69 6e69 745f 5fa9 0972 1d00 0000 721e  _init__..r....r.
+00003a80: 0000 0072 1f00 0000 7220 0000 0072 3800  ...r....r ...r8.
+00003a90: 0000 7270 0000 0072 0200 0000 7215 0000  ..rp...r....r...
+00003aa0: 0072 2100 0000 721a 0000 0072 1a00 0000  .r!...r....r....
+00003ab0: 7218 0000 0072 1b00 0000 726e 0000 00d9  r....r....rn....
+00003ac0: 0100 0073 0800 0000 0802 0200 08ff 0404  ...s............
+00003ad0: 726e 0000 0063 0000 0000 0000 0000 0000  rn...c..........
+00003ae0: 0000 0000 0000 0400 0000 0000 0000 7336  ..............s6
+00003af0: 0000 0065 005a 0164 005a 0264 0164 0164  ...e.Z.d.Z.d.d.d
+00003b00: 0264 039c 0269 015a 0365 046a 0565 0664  .d...i.Z.e.j.e.d
+00003b10: 0464 059c 0387 0066 0164 0664 0784 0c5a  .d.....f.d.d...Z
+00003b20: 0787 0004 005a 0853 0029 08da 1143 7265  .....Z.S.)...Cre
+00003b30: 6174 6554 6173 6b52 6571 7565 7374 726f  ateTaskRequestro
+00003b40: 0000 0072 7000 0000 720c 0000 004e 7271  ...rp...r....Nrq
+00003b50: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003b60: 0300 0000 0300 0000 0b00 0000 7318 0000  ............s...
+00003b70: 0074 0083 006a 0166 007c 028e 0101 007c  .t...j.f.|.....|
+00003b80: 017c 005f 0264 0153 0029 027a 3e0a 2020  .|._.d.S.).z>.  
+00003b90: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00003ba0: 3a0a 2020 2020 2020 2020 2020 2020 7461  :.            ta
+00003bb0: 736b 3a20 5461 736b 2074 6f20 6372 6561  sk: Task to crea
+00003bc0: 7465 0a20 2020 2020 2020 204e 7272 0000  te.        Nrr..
+00003bd0: 0072 7300 0000 7218 0000 0072 1a00 0000  .rs...r....r....
+00003be0: 721b 0000 0072 1500 0000 ec01 0000 7304  r....r........s.
+00003bf0: 0000 0000 050e 017a 1a43 7265 6174 6554  .......z.CreateT
+00003c00: 6173 6b52 6571 7565 7374 2e5f 5f69 6e69  askRequest.__ini
+00003c10: 745f 5f72 7400 0000 721a 0000 0072 1a00  t__rt...r....r..
+00003c20: 0000 7218 0000 0072 1b00 0000 7275 0000  ..r....r....ru..
+00003c30: 00e7 0100 0073 0800 0000 0802 0200 08ff  .....s..........
+00003c40: 0404 7275 0000 0063 0000 0000 0000 0000  ..ru...c........
+00003c50: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00003c60: 7336 0000 0065 005a 0164 005a 0264 0164  s6...e.Z.d.Z.d.d
+00003c70: 0164 0264 039c 0269 015a 0365 046a 0565  .d.d...i.Z.e.j.e
+00003c80: 0664 0464 059c 0387 0066 0164 0664 0784  .d.d.....f.d.d..
+00003c90: 0c5a 0787 0004 005a 0853 0029 08da 1243  .Z.....Z.S.)...C
+00003ca0: 7265 6174 6554 6173 6b52 6573 706f 6e73  reateTaskRespons
+00003cb0: 6572 6f00 0000 7270 0000 0072 0c00 0000  ero...rp...r....
+00003cc0: 4e72 7100 0000 6302 0000 0000 0000 0000  Nrq...c.........
+00003cd0: 0000 0003 0000 0003 0000 000b 0000 0073  ...............s
+00003ce0: 1800 0000 7400 8300 6a01 6600 7c02 8e01  ....t...j.f.|...
+00003cf0: 0100 7c01 7c00 5f02 6401 5300 2902 7a3c  ..|.|._.d.S.).z<
+00003d00: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00003d10: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00003d20: 2074 6173 6b3a 2054 6173 6b20 6372 6561   task: Task crea
+00003d30: 7465 640a 2020 2020 2020 2020 4e72 7200  ted.        Nrr.
+00003d40: 0000 7273 0000 0072 1800 0000 721a 0000  ..rs...r....r...
+00003d50: 0072 1b00 0000 7215 0000 00fa 0100 0073  .r....r........s
+00003d60: 0400 0000 0005 0e01 7a1b 4372 6561 7465  ........z.Create
+00003d70: 5461 736b 5265 7370 6f6e 7365 2e5f 5f69  TaskResponse.__i
+00003d80: 6e69 745f 5f72 7400 0000 721a 0000 0072  nit__rt...r....r
+00003d90: 1a00 0000 7218 0000 0072 1b00 0000 7276  ....r....r....rv
+00003da0: 0000 00f5 0100 0073 0800 0000 0802 0200  .......s........
+00003db0: 08ff 0404 7276 0000 0063 0000 0000 0000  ....rv...c......
+00003dc0: 0000 0000 0000 0000 0000 0400 0000 0000  ................
+00003dd0: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
+00003de0: 0164 0264 0364 049c 0269 015a 0365 0465  .d.d.d...i.Z.e.e
+00003df0: 0564 0564 069c 0387 0066 0164 0764 0884  .d.d.....f.d.d..
+00003e00: 0c5a 0687 0004 005a 0753 0029 09da 1343  .Z.....Z.S.)...C
+00003e10: 6f6d 706c 6574 6554 6173 6b52 6571 7565  ompleteTaskReque
+00003e20: 7374 7230 0000 0072 2f00 0000 720b 0000  str0...r/...r...
+00003e30: 0072 0c00 0000 4e72 6b00 0000 6302 0000  .r....Nrk...c...
+00003e40: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00003e50: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
+00003e60: 6600 7c02 8e01 0100 7c01 7c00 5f02 6401  f.|.....|.|._.d.
+00003e70: 5300 2902 7a57 0a20 2020 2020 2020 2050  S.).zW.        P
+00003e80: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+00003e90: 2020 2020 2020 2074 6173 6b5f 6964 3a20         task_id: 
+00003ea0: 5461 736b 2069 6465 6e74 6966 6965 7220  Task identifier 
+00003eb0: 746f 206d 6172 6b20 6173 2063 6f6d 706c  to mark as compl
+00003ec0: 6574 6564 0a20 2020 2020 2020 204e 726c  eted.        Nrl
+00003ed0: 0000 0072 6d00 0000 7218 0000 0072 1a00  ...rm...r....r..
+00003ee0: 0000 721b 0000 0072 1500 0000 0802 0000  ..r....r........
+00003ef0: 7304 0000 0000 050e 017a 1c43 6f6d 706c  s........z.Compl
+00003f00: 6574 6554 6173 6b52 6571 7565 7374 2e5f  eteTaskRequest._
+00003f10: 5f69 6e69 745f 5f72 1c00 0000 721a 0000  _init__r....r...
+00003f20: 0072 1a00 0000 7218 0000 0072 1b00 0000  .r....r....r....
+00003f30: 7277 0000 0003 0200 0073 0800 0000 0802  rw.......s......
+00003f40: 0200 08ff 0404 7277 0000 0063 0000 0000  ......rw...c....
+00003f50: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00003f60: 0000 0000 7336 0000 0065 005a 0164 005a  ....s6...e.Z.d.Z
+00003f70: 0264 0164 0164 0264 039c 0269 015a 0365  .d.d.d.d...i.Z.e
+00003f80: 046a 0565 0664 0464 059c 0387 0066 0164  .j.e.d.d.....f.d
+00003f90: 0664 0784 0c5a 0787 0004 005a 0853 0029  .d...Z.....Z.S.)
+00003fa0: 08da 1443 6f6d 706c 6574 6554 6173 6b52  ...CompleteTaskR
+00003fb0: 6573 706f 6e73 6572 6f00 0000 7270 0000  esponsero...rp..
+00003fc0: 0072 0c00 0000 4e72 7100 0000 6302 0000  .r....Nrq...c...
+00003fd0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+00003fe0: 000b 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
+00003ff0: 6600 7c02 8e01 0100 7c01 7c00 5f02 6401  f.|.....|.|._.d.
+00004000: 5300 a902 7a3c 0a20 2020 2020 2020 2050  S...z<.        P
+00004010: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+00004020: 2020 2020 2020 2074 6173 6b3a 2054 6173         task: Tas
+00004030: 6b20 7570 6461 7465 640a 2020 2020 2020  k updated.      
+00004040: 2020 4e72 7200 0000 7273 0000 0072 1800    Nrr...rs...r..
+00004050: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
+00004060: 0016 0200 0073 0400 0000 0005 0e01 7a1d  .....s........z.
+00004070: 436f 6d70 6c65 7465 5461 736b 5265 7370  CompleteTaskResp
+00004080: 6f6e 7365 2e5f 5f69 6e69 745f 5f72 7400  onse.__init__rt.
+00004090: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
+000040a0: 0072 1b00 0000 7278 0000 0011 0200 0073  .r....rx.......s
+000040b0: 0800 0000 0802 0200 08ff 0404 7278 0000  ............rx..
+000040c0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000040d0: 0000 0400 0000 0000 0000 7334 0000 0065  ..........s4...e
+000040e0: 005a 0164 005a 0264 0164 0264 0364 049c  .Z.d.Z.d.d.d.d..
+000040f0: 0269 015a 0365 0465 0564 0564 069c 0387  .i.Z.e.e.d.d....
+00004100: 0066 0164 0764 0884 0c5a 0687 0004 005a  .f.d.d...Z.....Z
+00004110: 0753 0029 09da 1043 6c61 696d 5461 736b  .S.)...ClaimTask
+00004120: 5265 7175 6573 7472 3000 0000 722f 0000  Requestr0...r/..
+00004130: 0072 0b00 0000 720c 0000 004e 726b 0000  .r....r....Nrk..
+00004140: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+00004150: 0000 0300 0000 0b00 0000 7318 0000 0074  ..........s....t
+00004160: 0083 006a 0166 007c 028e 0101 007c 017c  ...j.f.|.....|.|
+00004170: 005f 0264 0153 0029 027a 5c0a 2020 2020  ._.d.S.).z\.    
+00004180: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+00004190: 2020 2020 2020 2020 2020 2020 7461 736b              task
+000041a0: 5f69 643a 2054 6173 6b20 6964 656e 7469  _id: Task identi
+000041b0: 6669 6572 2074 6f20 636c 6169 6d20 6279  fier to claim by
+000041c0: 2074 6865 2072 6571 7565 7374 6f72 0a20   the requestor. 
+000041d0: 2020 2020 2020 204e 726c 0000 0072 6d00         Nrl...rm.
+000041e0: 0000 7218 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+000041f0: 0072 1500 0000 2402 0000 7304 0000 0000  .r....$...s.....
+00004200: 050e 017a 1943 6c61 696d 5461 736b 5265  ...z.ClaimTaskRe
+00004210: 7175 6573 742e 5f5f 696e 6974 5f5f 721c  quest.__init__r.
+00004220: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
+00004230: 0000 721b 0000 0072 7a00 0000 1f02 0000  ..r....rz.......
+00004240: 7308 0000 0008 0202 0008 ff04 0472 7a00  s............rz.
+00004250: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00004260: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
+00004270: 6500 5a01 6400 5a02 6401 6401 6402 6403  e.Z.d.Z.d.d.d.d.
+00004280: 9c02 6901 5a03 6504 6a05 6506 6404 6405  ..i.Z.e.j.e.d.d.
+00004290: 9c03 8700 6601 6406 6407 840c 5a07 8700  ....f.d.d...Z...
+000042a0: 0400 5a08 5300 2908 da11 436c 6169 6d54  ..Z.S.)...ClaimT
+000042b0: 6173 6b52 6573 706f 6e73 6572 6f00 0000  askResponsero...
+000042c0: 7270 0000 0072 0c00 0000 4e72 7100 0000  rp...r....Nrq...
+000042d0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000042e0: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
+000042f0: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+00004300: 5f02 6401 5300 2902 7a3c 0a20 2020 2020  _.d.S.).z<.     
+00004310: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+00004320: 2020 2020 2020 2020 2020 2074 6173 6b3a             task:
+00004330: 2054 6173 6b20 636c 6169 6d65 640a 2020   Task claimed.  
+00004340: 2020 2020 2020 4e72 7200 0000 7273 0000        Nrr...rs..
+00004350: 0072 1800 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00004360: 7215 0000 0032 0200 0073 0400 0000 0005  r....2...s......
+00004370: 0e01 7a1a 436c 6169 6d54 6173 6b52 6573  ..z.ClaimTaskRes
+00004380: 706f 6e73 652e 5f5f 696e 6974 5f5f 7274  ponse.__init__rt
+00004390: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
+000043a0: 0000 721b 0000 0072 7b00 0000 2d02 0000  ..r....r{...-...
+000043b0: 7308 0000 0008 0202 0008 ff04 0472 7b00  s............r{.
+000043c0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000043d0: 0000 0007 0000 0000 0000 0073 5200 0000  ...........sR...
+000043e0: 6500 5a01 6400 5a02 6401 6402 6403 9c02  e.Z.d.Z.d.d.d...
+000043f0: 6404 6402 6403 9c02 6405 6402 6403 9c02  d.d.d...d.d.d...
+00004400: 6406 9c03 5a03 640b 6504 6505 6504 1900  d...Z.d.e.e.e...
+00004410: 6505 6504 1900 6506 6407 6408 9c05 8700  e.e...e.d.d.....
+00004420: 6601 6409 640a 840d 5a07 8700 0400 5a08  f.d.d...Z.....Z.
+00004430: 5300 290c da11 4173 7369 676e 5461 736b  S.)...AssignTask
+00004440: 5265 7175 6573 7472 2f00 0000 720b 0000  Requestr/...r...
+00004450: 0072 0c00 0000 725f 0000 0072 3400 0000  .r....r_...r4...
+00004460: 2903 7230 0000 0072 5f00 0000 7233 0000  ).r0...r_...r3..
+00004470: 004e 2905 7230 0000 0072 5f00 0000 7233  .N).r0...r_...r3
+00004480: 0000 0072 1000 0000 7211 0000 0063 0400  ...r....r....c..
+00004490: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+000044a0: 0000 0b00 0000 7324 0000 0074 0083 006a  ......s$...t...j
+000044b0: 0166 007c 048e 0101 007c 017c 005f 027c  .f.|.....|.|._.|
+000044c0: 027c 005f 037c 037c 005f 0464 0153 0029  .|._.|.|._.d.S.)
+000044d0: 0261 5001 0000 0a20 2020 2020 2020 2050  .aP....        P
+000044e0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+000044f0: 2020 2020 2020 2074 6173 6b5f 6964 3a20         task_id: 
+00004500: 5461 736b 2074 6f20 6173 7369 676e 2074  Task to assign t
+00004510: 6f20 7468 6520 656d 6169 6c20 6f72 2070  o the email or p
+00004520: 7269 6e63 6970 616c 5f69 6420 7365 6c65  rincipal_id sele
+00004530: 6374 6564 0a20 2020 2020 2020 2020 2020  cted.           
+00004540: 2065 6d61 696c 3a20 5573 6572 2065 6d61   email: User ema
+00004550: 696c 2074 6861 7420 7761 6e74 2074 6f20  il that want to 
+00004560: 7573 6520 746f 2061 7373 6967 6e20 7468  use to assign th
+00004570: 6520 7461 736b 2e20 4174 7472 6962 7574  e task. Attribut
+00004580: 6520 3a65 6d61 696c 206f 7220 7072 696e  e :email or prin
+00004590: 6369 7061 6c5f 6964 206d 7573 7420 6265  cipal_id must be
+000045a0: 2073 6574 0a20 2020 2020 2020 2020 2020   set.           
+000045b0: 2070 7269 6e63 6970 616c 5f69 643a 2050   principal_id: P
+000045c0: 7269 6e63 6970 616c 2069 6420 7468 6174  rincipal id that
+000045d0: 2077 616e 7420 746f 2075 7365 2074 6f20   want to use to 
+000045e0: 6173 7369 676e 2074 6865 2074 6173 6b2e  assign the task.
+000045f0: 2041 7474 7269 6275 7465 205f 656d 6169   Attribute _emai
+00004600: 6c20 6f72 2070 7269 6e63 6970 616c 5f69  l or principal_i
+00004610: 6420 6d75 7374 2062 6520 7365 740a 2020  d must be set.  
+00004620: 2020 2020 2020 4e29 0572 1400 0000 7215        N).r....r.
+00004630: 0000 0072 3000 0000 725f 0000 0072 3300  ...r0...r_...r3.
+00004640: 0000 2905 7217 0000 0072 3000 0000 725f  ..).r....r0...r_
+00004650: 0000 0072 3300 0000 7210 0000 0072 1800  ...r3...r....r..
+00004660: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
+00004670: 0042 0200 0073 0800 0000 0009 0e01 0601  .B...s..........
+00004680: 0601 7a1a 4173 7369 676e 5461 736b 5265  ..z.AssignTaskRe
+00004690: 7175 6573 742e 5f5f 696e 6974 5f5f 2902  quest.__init__).
+000046a0: 4e4e 7260 0000 0072 1a00 0000 721a 0000  NNr`...r....r...
+000046b0: 0072 1800 0000 721b 0000 0072 7c00 0000  .r....r....r|...
+000046c0: 3b02 0000 731a 0000 0008 0208 0108 0108  ;...s...........
+000046d0: fd06 0700 0000 ff02 0102 0006 0006 0002  ................
+000046e0: 0102 fe72 7c00 0000 6300 0000 0000 0000  ...r|...c.......
+000046f0: 0000 0000 0000 0000 0004 0000 0000 0000  ................
+00004700: 0073 3600 0000 6500 5a01 6400 5a02 6401  .s6...e.Z.d.Z.d.
+00004710: 6401 6402 6403 9c02 6901 5a03 6504 6a05  d.d.d...i.Z.e.j.
+00004720: 6506 6404 6405 9c03 8700 6601 6406 6407  e.d.d.....f.d.d.
+00004730: 840c 5a07 8700 0400 5a08 5300 2908 da12  ..Z.....Z.S.)...
+00004740: 4173 7369 676e 5461 736b 5265 7370 6f6e  AssignTaskRespon
+00004750: 7365 726f 0000 0072 7000 0000 720c 0000  sero...rp...r...
+00004760: 004e 7271 0000 0063 0200 0000 0000 0000  .Nrq...c........
+00004770: 0000 0000 0300 0000 0300 0000 0b00 0000  ................
+00004780: 7318 0000 0074 0083 006a 0166 007c 028e  s....t...j.f.|..
+00004790: 0101 007c 017c 005f 0264 0153 0072 7900  ...|.|._.d.S.ry.
+000047a0: 0000 7272 0000 0072 7300 0000 7218 0000  ..rr...rs...r...
+000047b0: 0072 1a00 0000 721b 0000 0072 1500 0000  .r....r....r....
+000047c0: 5602 0000 7304 0000 0000 050e 017a 1b41  V...s........z.A
+000047d0: 7373 6967 6e54 6173 6b52 6573 706f 6e73  ssignTaskRespons
+000047e0: 652e 5f5f 696e 6974 5f5f 7274 0000 0072  e.__init__rt...r
+000047f0: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
+00004800: 0000 0072 7d00 0000 5102 0000 7308 0000  ...r}...Q...s...
+00004810: 0008 0202 0008 ff04 0472 7d00 0000 6300  .........r}...c.
+00004820: 0000 0000 0000 0000 0000 0000 0000 0007  ................
+00004830: 0000 0000 0000 0073 5400 0000 6500 5a01  .......sT...e.Z.
+00004840: 6400 5a02 6401 6402 6403 9c02 6404 6402  d.Z.d.d.d...d.d.
+00004850: 6403 9c02 6405 6406 6403 9c02 6407 9c03  d...d.d.d...d...
+00004860: 5a03 640c 6504 6504 6505 6506 6507 6a08  Z.d.e.e.e.e.e.j.
+00004870: 1900 1900 6509 6408 6409 9c05 8700 6601  ....e.d.d.....f.
+00004880: 640a 640b 840d 5a0a 8700 0400 5a0b 5300  d.d...Z.....Z.S.
+00004890: 290d da16 5361 7665 5461 736b 456c 656d  )...SaveTaskElem
+000048a0: 656e 7452 6571 7565 7374 722f 0000 0072  entRequestr/...r
+000048b0: 0b00 0000 720c 0000 0072 5000 0000 7251  ....r....rP...rQ
+000048c0: 0000 007a 125b 5461 736b 456c 656d 656e  ...z.[TaskElemen
+000048d0: 7456 616c 7565 5d29 0372 3000 0000 7252  tValue]).r0...rR
+000048e0: 0000 0072 5300 0000 4e29 0572 3000 0000  ...rS...N).r0...
+000048f0: 7252 0000 0072 5300 0000 7210 0000 0072  rR...rS...r....r
+00004900: 1100 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00004910: 0005 0000 0003 0000 000b 0000 0073 2800  .............s(.
+00004920: 0000 7400 8300 6a01 6600 7c04 8e01 0100  ..t...j.f.|.....
+00004930: 7c01 7c00 5f02 7c02 7c00 5f03 7c03 7020  |.|._.|.|._.|.p 
+00004940: 6700 7c00 5f04 6401 5300 2902 7aa9 0a20  g.|._.d.S.).z.. 
+00004950: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00004960: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00004970: 6173 6b5f 6964 3a20 5461 736b 2074 6f20  ask_id: Task to 
+00004980: 7570 6461 7465 0a20 2020 2020 2020 2020  update.         
+00004990: 2020 2065 6c65 6d65 6e74 5f64 6566 696e     element_defin
+000049a0: 6974 696f 6e5f 636f 6465 3a20 456c 656d  ition_code: Elem
+000049b0: 656e 7420 6465 6669 6e69 7469 6f6e 2063  ent definition c
+000049c0: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+000049d0: 656c 656d 656e 745f 7661 6c75 6573 3a20  element_values: 
+000049e0: 456c 656d 656e 7420 7661 6c75 6573 0a20  Element values. 
+000049f0: 2020 2020 2020 204e 2905 7214 0000 0072         N).r....r
+00004a00: 1500 0000 7230 0000 0072 5200 0000 7253  ....r0...rR...rS
+00004a10: 0000 0029 0572 1700 0000 7230 0000 0072  ...).r....r0...r
+00004a20: 5200 0000 7253 0000 0072 1000 0000 7218  R...rS...r....r.
+00004a30: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00004a40: 0000 6602 0000 7308 0000 0000 0d0e 0106  ..f...s.........
+00004a50: 0106 017a 1f53 6176 6554 6173 6b45 6c65  ...z.SaveTaskEle
+00004a60: 6d65 6e74 5265 7175 6573 742e 5f5f 696e  mentRequest.__in
+00004a70: 6974 5f5f 2901 4e29 0c72 1d00 0000 721e  it__).N).r....r.
+00004a80: 0000 0072 1f00 0000 7220 0000 0072 0b00  ...r....r ...r..
+00004a90: 0000 7205 0000 0072 0400 0000 7238 0000  ..r....r....r8..
+00004aa0: 00da 1054 6173 6b45 6c65 6d65 6e74 5661  ...TaskElementVa
+00004ab0: 6c75 6572 0200 0000 7215 0000 0072 2100  luer....r....r!.
+00004ac0: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
+00004ad0: 0072 1b00 0000 727e 0000 005f 0200 0073  .r....r~..._...s
+00004ae0: 1800 0000 0802 0801 0801 08fd 060a 00fc  ................
+00004af0: 0202 0201 0201 0c01 0201 02fa 727e 0000  ............r~..
+00004b00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004b10: 0000 0400 0000 0000 0000 7336 0000 0065  ..........s6...e
+00004b20: 005a 0164 005a 0264 0164 0164 0264 039c  .Z.d.Z.d.d.d.d..
+00004b30: 0269 015a 0365 046a 0565 0664 0464 059c  .i.Z.e.j.e.d.d..
+00004b40: 0387 0066 0164 0664 0784 0c5a 0787 0004  ...f.d.d...Z....
+00004b50: 005a 0853 0029 08da 1753 6176 6554 6173  .Z.S.)...SaveTas
+00004b60: 6b45 6c65 6d65 6e74 5265 7370 6f6e 7365  kElementResponse
+00004b70: 726f 0000 0072 7000 0000 720c 0000 004e  ro...rp...r....N
+00004b80: 7271 0000 0063 0200 0000 0000 0000 0000  rq...c..........
+00004b90: 0000 0300 0000 0300 0000 0b00 0000 7318  ..............s.
+00004ba0: 0000 0074 0083 006a 0166 007c 028e 0101  ...t...j.f.|....
+00004bb0: 007c 017c 005f 0264 0153 0072 7900 0000  .|.|._.d.S.ry...
+00004bc0: 7272 0000 0072 7300 0000 7218 0000 0072  rr...rs...r....r
+00004bd0: 1a00 0000 721b 0000 0072 1500 0000 7e02  ....r....r....~.
+00004be0: 0000 7304 0000 0000 050e 017a 2053 6176  ..s........z Sav
+00004bf0: 6554 6173 6b45 6c65 6d65 6e74 5265 7370  eTaskElementResp
+00004c00: 6f6e 7365 2e5f 5f69 6e69 745f 5f72 7400  onse.__init__rt.
+00004c10: 0000 721a 0000 0072 1a00 0000 7218 0000  ..r....r....r...
+00004c20: 0072 1b00 0000 7280 0000 0079 0200 0073  .r....r....y...s
+00004c30: 0800 0000 0802 0200 08ff 0404 7280 0000  ............r...
+00004c40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004c50: 0000 0500 0000 0000 0000 733e 0000 0065  ..........s>...e
+00004c60: 005a 0164 005a 0264 0164 0264 039c 0264  .Z.d.Z.d.d.d...d
+00004c70: 0464 0264 039c 0264 059c 025a 0365 0465  .d.d...d...Z.e.e
+00004c80: 0465 0564 0664 079c 0487 0066 0164 0864  .e.d.d.....f.d.d
+00004c90: 0984 0c5a 0687 0004 005a 0753 0029 0ada  ...Z.....Z.S.)..
+00004ca0: 1844 656c 6574 6554 6173 6b45 6c65 6d65  .DeleteTaskEleme
+00004cb0: 6e74 5265 7175 6573 7472 2f00 0000 720b  ntRequestr/...r.
+00004cc0: 0000 0072 0c00 0000 7250 0000 0029 0272  ...r....rP...).r
+00004cd0: 3000 0000 7252 0000 004e 2904 7230 0000  0...rR...N).r0..
+00004ce0: 0072 5200 0000 7210 0000 0072 1100 0000  .rR...r....r....
+00004cf0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00004d00: 0003 0000 000b 0000 0073 1e00 0000 7400  .........s....t.
+00004d10: 8300 6a01 6600 7c03 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+00004d20: 5f02 7c02 7c00 5f03 6401 5300 2902 7a93  _.|.|._.d.S.).z.
+00004d30: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00004d40: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+00004d50: 2074 6173 6b5f 6964 3a20 5461 736b 2074   task_id: Task t
+00004d60: 6f20 7570 6461 7465 0a20 2020 2020 2020  o update.       
+00004d70: 2020 2020 2065 6c65 6d65 6e74 5f64 6566       element_def
+00004d80: 696e 6974 696f 6e5f 636f 6465 3a20 456c  inition_code: El
+00004d90: 656d 656e 7420 6465 6669 6e69 7469 6f6e  ement definition
+00004da0: 2063 6f64 6520 746f 2064 656c 6574 6520   code to delete 
+00004db0: 616c 6c20 7661 6c75 6573 0a20 2020 2020  all values.     
+00004dc0: 2020 204e 2904 7214 0000 0072 1500 0000     N).r....r....
+00004dd0: 7230 0000 0072 5200 0000 2904 7217 0000  r0...rR...).r...
+00004de0: 0072 3000 0000 7252 0000 0072 1000 0000  .r0...rR...r....
+00004df0: 7218 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00004e00: 1500 0000 8d02 0000 7306 0000 0000 060e  ........s.......
+00004e10: 0106 017a 2144 656c 6574 6554 6173 6b45  ...z!DeleteTaskE
+00004e20: 6c65 6d65 6e74 5265 7175 6573 742e 5f5f  lementRequest.__
+00004e30: 696e 6974 5f5f 721c 0000 0072 1a00 0000  init__r....r....
+00004e40: 721a 0000 0072 1800 0000 721b 0000 0072  r....r....r....r
+00004e50: 8100 0000 8702 0000 7308 0000 0008 0208  ........s.......
+00004e60: 0108 fe06 0572 8100 0000 6300 0000 0000  .....r....c.....
+00004e70: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00004e80: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
+00004e90: 6401 6401 6402 6403 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
+00004ea0: 6a05 6506 6404 6405 9c03 8700 6601 6406  j.e.d.d.....f.d.
+00004eb0: 6407 840c 5a07 8700 0400 5a08 5300 2908  d...Z.....Z.S.).
+00004ec0: da19 4465 6c65 7465 5461 736b 456c 656d  ..DeleteTaskElem
+00004ed0: 656e 7452 6573 706f 6e73 6572 6f00 0000  entResponsero...
+00004ee0: 7270 0000 0072 0c00 0000 4e72 7100 0000  rp...r....Nrq...
+00004ef0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00004f00: 0003 0000 000b 0000 0073 1800 0000 7400  .........s....t.
+00004f10: 8300 6a01 6600 7c02 8e01 0100 7c01 7c00  ..j.f.|.....|.|.
+00004f20: 5f02 6401 5300 7279 0000 0072 7200 0000  _.d.S.ry...rr...
+00004f30: 7273 0000 0072 1800 0000 721a 0000 0072  rs...r....r....r
+00004f40: 1b00 0000 7215 0000 009d 0200 0073 0400  ....r........s..
+00004f50: 0000 0005 0e01 7a22 4465 6c65 7465 5461  ......z"DeleteTa
+00004f60: 736b 456c 656d 656e 7452 6573 706f 6e73  skElementRespons
+00004f70: 652e 5f5f 696e 6974 5f5f 7274 0000 0072  e.__init__rt...r
+00004f80: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
+00004f90: 0000 0072 8200 0000 9802 0000 7308 0000  ...r........s...
+00004fa0: 0008 0202 0008 ff04 0472 8200 0000 6300  .........r....c.
+00004fb0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00004fc0: 0000 0000 0000 0073 3e00 0000 6500 5a01  .......s>...e.Z.
+00004fd0: 6400 5a02 6401 6402 6403 9c02 6404 6402  d.Z.d.d.d...d.d.
+00004fe0: 6403 9c02 6405 9c02 5a03 6504 6504 6505  d...d...Z.e.e.e.
+00004ff0: 6406 6407 9c04 8700 6601 6408 6409 840c  d.d.....f.d.d...
+00005000: 5a06 8700 0400 5a07 5300 290a da25 4465  Z.....Z.S.)..%De
+00005010: 6c65 7465 5461 736b 456c 656d 656e 7456  leteTaskElementV
+00005020: 616c 7565 446f 6375 6d65 6e74 5265 7175  alueDocumentRequ
+00005030: 6573 7472 2f00 0000 720b 0000 0072 0c00  estr/...r....r..
+00005040: 0000 da0a 646f 6375 6d65 6e74 4964 2902  ....documentId).
+00005050: 7230 0000 00da 0b64 6f63 756d 656e 745f  r0.....document_
+00005060: 6964 4e29 0472 3000 0000 7285 0000 0072  idN).r0...r....r
+00005070: 1000 0000 7211 0000 0063 0300 0000 0000  ....r....c......
+00005080: 0000 0000 0000 0400 0000 0300 0000 0b00  ................
+00005090: 0000 731e 0000 0074 0083 006a 0166 007c  ..s....t...j.f.|
+000050a0: 038e 0101 007c 017c 005f 027c 027c 005f  .....|.|._.|.|._
+000050b0: 0364 0153 0029 027a 780a 2020 2020 2020  .d.S.).zx.      
+000050c0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+000050d0: 2020 2020 2020 2020 2020 7461 736b 5f69            task_i
+000050e0: 643a 2054 6173 6b20 746f 2075 7064 6174  d: Task to updat
+000050f0: 650a 2020 2020 2020 2020 2020 2020 646f  e.            do
+00005100: 6375 6d65 6e74 5f69 643a 2044 6f63 756d  cument_id: Docum
+00005110: 656e 7420 6964 2074 6f20 6465 6c65 7465  ent id to delete
+00005120: 2075 7064 6174 6564 0a20 2020 2020 2020   updated.       
+00005130: 204e 2904 7214 0000 0072 1500 0000 7230   N).r....r....r0
+00005140: 0000 0072 8500 0000 2904 7217 0000 0072  ...r....).r....r
+00005150: 3000 0000 7285 0000 0072 1000 0000 7218  0...r....r....r.
+00005160: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00005170: 0000 ac02 0000 7306 0000 0000 060e 0106  ......s.........
+00005180: 017a 2e44 656c 6574 6554 6173 6b45 6c65  .z.DeleteTaskEle
+00005190: 6d65 6e74 5661 6c75 6544 6f63 756d 656e  mentValueDocumen
+000051a0: 7452 6571 7565 7374 2e5f 5f69 6e69 745f  tRequest.__init_
+000051b0: 5f72 1c00 0000 721a 0000 0072 1a00 0000  _r....r....r....
+000051c0: 7218 0000 0072 1b00 0000 7283 0000 00a6  r....r....r.....
+000051d0: 0200 0073 0800 0000 0802 0801 08fe 0605  ...s............
+000051e0: 7283 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000051f0: 0000 0000 0000 0400 0000 0000 0000 7336  ..............s6
+00005200: 0000 0065 005a 0164 005a 0264 0164 0164  ...e.Z.d.Z.d.d.d
+00005210: 0264 039c 0269 015a 0365 046a 0565 0664  .d...i.Z.e.j.e.d
+00005220: 0464 059c 0387 0066 0164 0664 0784 0c5a  .d.....f.d.d...Z
+00005230: 0787 0004 005a 0853 0029 08da 2644 656c  .....Z.S.)..&Del
+00005240: 6574 6554 6173 6b45 6c65 6d65 6e74 5661  eteTaskElementVa
+00005250: 6c75 6544 6f63 756d 656e 7452 6573 706f  lueDocumentRespo
+00005260: 6e73 6572 6f00 0000 7270 0000 0072 0c00  nsero...rp...r..
+00005270: 0000 4e72 7100 0000 6302 0000 0000 0000  ..Nrq...c.......
+00005280: 0000 0000 0003 0000 0003 0000 000b 0000  ................
+00005290: 0073 1800 0000 7400 8300 6a01 6600 7c02  .s....t...j.f.|.
+000052a0: 8e01 0100 7c01 7c00 5f02 6401 5300 7279  ....|.|._.d.S.ry
+000052b0: 0000 0072 7200 0000 7273 0000 0072 1800  ...rr...rs...r..
+000052c0: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
+000052d0: 00bc 0200 0073 0400 0000 0005 0e01 7a2f  .....s........z/
+000052e0: 4465 6c65 7465 5461 736b 456c 656d 656e  DeleteTaskElemen
+000052f0: 7456 616c 7565 446f 6375 6d65 6e74 5265  tValueDocumentRe
+00005300: 7370 6f6e 7365 2e5f 5f69 6e69 745f 5f72  sponse.__init__r
+00005310: 7400 0000 721a 0000 0072 1a00 0000 7218  t...r....r....r.
+00005320: 0000 0072 1b00 0000 7286 0000 00b7 0200  ...r....r.......
+00005330: 0073 0800 0000 0802 0200 08ff 0404 7286  .s............r.
+00005340: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00005350: 0000 0000 0600 0000 0000 0000 734c 0000  ............sL..
+00005360: 0065 005a 0164 005a 0264 0164 0264 039c  .e.Z.d.Z.d.d.d..
+00005370: 0264 0464 0564 039c 0264 069c 025a 0364  .d.d.d...d...Z.d
+00005380: 0b65 0465 0565 0665 0465 0766 0219 0019  .e.e.e.e.e.f....
+00005390: 0065 0764 0764 089c 0487 0066 0164 0964  .e.d.d.....f.d.d
+000053a0: 0a84 0d5a 0887 0004 005a 0953 0029 0cda  ...Z.....Z.S.)..
+000053b0: 2153 6176 6554 6173 6b4a 736f 6e46 6f72  !SaveTaskJsonFor
+000053c0: 6d73 5661 6c75 6544 6174 6152 6571 7565  msValueDataReque
+000053d0: 7374 722f 0000 0072 0b00 0000 720c 0000  str/...r....r...
+000053e0: 0072 5800 0000 7259 0000 0029 0272 3000  .rX...rY...).r0.
+000053f0: 0000 7258 0000 004e 2904 7230 0000 0072  ..rX...N).r0...r
+00005400: 5800 0000 7210 0000 0072 1100 0000 6303  X...r....r....c.
+00005410: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00005420: 0000 000b 0000 0073 2200 0000 7400 8300  .......s"...t...
+00005430: 6a01 6600 7c03 8e01 0100 7c01 7c00 5f02  j.f.|.....|.|._.
+00005440: 7c02 701a 6900 7c00 5f03 6401 5300 2902  |.p.i.|._.d.S.).
+00005450: 7a65 0a20 2020 2020 2020 2050 6172 616d  ze.        Param
+00005460: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+00005470: 2020 2074 6173 6b5f 6964 3a20 5461 736b     task_id: Task
+00005480: 2074 6f20 7570 6461 7465 0a20 2020 2020   to update.     
+00005490: 2020 2020 2020 2064 6174 613a 206a 736f         data: jso
+000054a0: 6e20 6461 7461 2074 6f20 7361 7665 0a20  n data to save. 
+000054b0: 2020 2020 2020 204e 2904 7214 0000 0072         N).r....r
+000054c0: 1500 0000 7230 0000 0072 5800 0000 2904  ....r0...rX...).
+000054d0: 7217 0000 0072 3000 0000 7258 0000 0072  r....r0...rX...r
+000054e0: 1000 0000 7218 0000 0072 1a00 0000 721b  ....r....r....r.
+000054f0: 0000 0072 1500 0000 cb02 0000 7306 0000  ...r........s...
+00005500: 0000 060e 0106 017a 2a53 6176 6554 6173  .......z*SaveTas
+00005510: 6b4a 736f 6e46 6f72 6d73 5661 6c75 6544  kJsonFormsValueD
+00005520: 6174 6152 6571 7565 7374 2e5f 5f69 6e69  ataRequest.__ini
+00005530: 745f 5f29 014e 725a 0000 0072 1a00 0000  t__).NrZ...r....
+00005540: 721a 0000 0072 1800 0000 721b 0000 0072  r....r....r....r
+00005550: 8700 0000 c502 0000 7308 0000 0008 0208  ........s.......
+00005560: 0108 fe06 0572 8700 0000 6300 0000 0000  .....r....c.....
+00005570: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+00005580: 0000 0073 3600 0000 6500 5a01 6400 5a02  ...s6...e.Z.d.Z.
+00005590: 6401 6401 6402 6403 9c02 6901 5a03 6504  d.d.d.d...i.Z.e.
+000055a0: 6a05 6506 6404 6405 9c03 8700 6601 6406  j.e.d.d.....f.d.
+000055b0: 6407 840c 5a07 8700 0400 5a08 5300 2908  d...Z.....Z.S.).
+000055c0: da22 5361 7665 5461 736b 4a73 6f6e 466f  ."SaveTaskJsonFo
+000055d0: 726d 7356 616c 7565 4461 7461 5265 7370  rmsValueDataResp
+000055e0: 6f6e 7365 726f 0000 0072 7000 0000 720c  onsero...rp...r.
+000055f0: 0000 004e 7271 0000 0063 0200 0000 0000  ...Nrq...c......
+00005600: 0000 0000 0000 0300 0000 0300 0000 0b00  ................
+00005610: 0000 7318 0000 0074 0083 006a 0166 007c  ..s....t...j.f.|
+00005620: 028e 0101 007c 017c 005f 0264 0153 0072  .....|.|._.d.S.r
+00005630: 7900 0000 7272 0000 0072 7300 0000 7218  y...rr...rs...r.
+00005640: 0000 0072 1a00 0000 721b 0000 0072 1500  ...r....r....r..
+00005650: 0000 db02 0000 7304 0000 0000 050e 017a  ......s........z
+00005660: 2b53 6176 6554 6173 6b4a 736f 6e46 6f72  +SaveTaskJsonFor
+00005670: 6d73 5661 6c75 6544 6174 6152 6573 706f  msValueDataRespo
+00005680: 6e73 652e 5f5f 696e 6974 5f5f 7274 0000  nse.__init__rt..
+00005690: 0072 1a00 0000 721a 0000 0072 1800 0000  .r....r....r....
+000056a0: 721b 0000 0072 8800 0000 d602 0000 7308  r....r........s.
+000056b0: 0000 0008 0202 0008 ff04 0472 8800 0000  ...........r....
+000056c0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000056d0: 0005 0000 0000 0000 0073 4000 0000 6500  .........s@...e.
+000056e0: 5a01 6400 5a02 6401 6402 6403 9c02 6404  Z.d.Z.d.d.d...d.
+000056f0: 6405 6403 9c02 6406 9c02 5a03 6504 6505  d.d...d...Z.e.e.
+00005700: 6a06 6507 6407 6408 9c04 8700 6601 6409  j.e.d.d.....f.d.
+00005710: 640a 840c 5a08 8700 0400 5a09 5300 290b  d...Z.....Z.S.).
+00005720: da14 4170 7065 6e64 5461 736b 4c6f 6752  ..AppendTaskLogR
+00005730: 6571 7565 7374 722f 0000 0072 0b00 0000  equestr/...r....
+00005740: 720c 0000 00da 036c 6f67 da03 4c6f 6729  r......log..Log)
+00005750: 0272 3000 0000 728a 0000 004e 2904 7230  .r0...r....N).r0
+00005760: 0000 0072 8a00 0000 7210 0000 0072 1100  ...r....r....r..
+00005770: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
+00005780: 0000 0003 0000 000b 0000 0073 1e00 0000  ...........s....
+00005790: 7400 8300 6a01 6600 7c03 8e01 0100 7c01  t...j.f.|.....|.
+000057a0: 7c00 5f02 7c02 7c00 5f03 6401 5300 2902  |._.|.|._.d.S.).
+000057b0: 7a6e 0a20 2020 2020 2020 2050 6172 616d  zn.        Param
+000057c0: 6574 6572 733a 0a20 2020 2020 2020 2020  eters:.         
+000057d0: 2020 2074 6173 6b5f 6964 3a20 5461 736b     task_id: Task
+000057e0: 2074 6f20 7570 6461 7465 0a20 2020 2020   to update.     
+000057f0: 2020 2020 2020 206c 6f67 3a20 4c6f 6720         log: Log 
+00005800: 6461 7461 2074 6f20 6164 6420 746f 2074  data to add to t
+00005810: 6865 2074 6173 6b0a 2020 2020 2020 2020  he task.        
+00005820: 4e29 0472 1400 0000 7215 0000 0072 3000  N).r....r....r0.
+00005830: 0000 728a 0000 0029 0472 1700 0000 7230  ..r....).r....r0
+00005840: 0000 0072 8a00 0000 7210 0000 0072 1800  ...r....r....r..
+00005850: 0000 721a 0000 0072 1b00 0000 7215 0000  ..r....r....r...
+00005860: 00ea 0200 0073 0600 0000 0006 0e01 0601  .....s..........
+00005870: 7a1d 4170 7065 6e64 5461 736b 4c6f 6752  z.AppendTaskLogR
+00005880: 6571 7565 7374 2e5f 5f69 6e69 745f 5f29  equest.__init__)
+00005890: 0a72 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+000058a0: 7220 0000 0072 0b00 0000 7238 0000 0072  r ...r....r8...r
+000058b0: 8b00 0000 7202 0000 0072 1500 0000 7221  ....r....r....r!
+000058c0: 0000 0072 1a00 0000 721a 0000 0072 1800  ...r....r....r..
+000058d0: 0000 721b 0000 0072 8900 0000 e402 0000  ..r....r........
+000058e0: 7308 0000 0008 0208 0108 fe06 0572 8900  s............r..
+000058f0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00005900: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
+00005910: 6500 5a01 6400 5a02 6401 6401 6402 6403  e.Z.d.Z.d.d.d.d.
+00005920: 9c02 6901 5a03 6504 6a05 6506 6404 6405  ..i.Z.e.j.e.d.d.
+00005930: 9c03 8700 6601 6406 6407 840c 5a07 8700  ....f.d.d...Z...
+00005940: 0400 5a08 5300 2908 da15 4170 7065 6e64  ..Z.S.)...Append
+00005950: 5461 736b 4c6f 6752 6573 706f 6e73 6572  TaskLogResponser
+00005960: 6f00 0000 7270 0000 0072 0c00 0000 4e72  o...rp...r....Nr
+00005970: 7100 0000 6302 0000 0000 0000 0000 0000  q...c...........
+00005980: 0003 0000 0003 0000 000b 0000 0073 1800  .............s..
+00005990: 0000 7400 8300 6a01 6600 7c02 8e01 0100  ..t...j.f.|.....
+000059a0: 7c01 7c00 5f02 6401 5300 7279 0000 0072  |.|._.d.S.ry...r
+000059b0: 7200 0000 7273 0000 0072 1800 0000 721a  r...rs...r....r.
+000059c0: 0000 0072 1b00 0000 7215 0000 00fa 0200  ...r....r.......
+000059d0: 0073 0400 0000 0005 0e01 7a1e 4170 7065  .s........z.Appe
+000059e0: 6e64 5461 736b 4c6f 6752 6573 706f 6e73  ndTaskLogRespons
+000059f0: 652e 5f5f 696e 6974 5f5f 7274 0000 0072  e.__init__rt...r
+00005a00: 1a00 0000 721a 0000 0072 1800 0000 721b  ....r....r....r.
+00005a10: 0000 0072 8c00 0000 f502 0000 7308 0000  ...r........s...
+00005a20: 0008 0202 0008 ff04 0472 8c00 0000 4e29  .........r....N)
+00005a30: 37da 0674 7970 696e 6772 0200 0000 7203  7..typingr....r.
+00005a40: 0000 0072 0400 0000 7205 0000 00da 0b6b  ...r....r......k
+00005a50: 7566 6c6f 775f 7265 7374 7206 0000 0072  uflow_restr....r
+00005a60: 3800 0000 5a16 6b75 666c 6f77 5f72 6573  8...Z.kuflow_res
+00005a70: 742e 5f67 656e 6572 6174 6564 7207 0000  t._generatedr...
+00005a80: 00da 054d 6f64 656c 7208 0000 0072 2200  ...Modelr....r".
+00005a90: 0000 7229 0000 0072 2d00 0000 722e 0000  ..r)...r-...r...
+00005aa0: 0072 3100 0000 7232 0000 0072 3500 0000  .r1...r2...r5...
+00005ab0: 7239 0000 0072 3b00 0000 723e 0000 0072  r9...r;...r>...r
+00005ac0: 4400 0000 7247 0000 0072 4800 0000 724f  D...rG...rH...rO
+00005ad0: 0000 0072 5500 0000 7257 0000 0072 5b00  ...rU...rW...r[.
+00005ae0: 0000 725c 0000 0072 5d00 0000 725e 0000  ..r\...r]...r^..
+00005af0: 0072 6100 0000 7262 0000 0072 6700 0000  .ra...rb...rg...
+00005b00: 726a 0000 0072 6e00 0000 7275 0000 0072  rj...rn...ru...r
+00005b10: 7600 0000 7277 0000 0072 7800 0000 727a  v...rw...rx...rz
+00005b20: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
+00005b30: 0000 727e 0000 0072 8000 0000 7281 0000  ..r~...r....r...
+00005b40: 0072 8200 0000 7283 0000 0072 8600 0000  .r....r....r....
+00005b50: 7287 0000 0072 8800 0000 7289 0000 0072  r....r....r....r
+00005b60: 8c00 0000 721a 0000 0072 1a00 0000 721a  ....r....r....r.
+00005b70: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00005b80: 653e 1900 0000 735c 0000 0018 020c 010c  e>....s\........
+00005b90: 0812 0e12 0e12 1e12 0e12 1012 1312 0e12  ................
+00005ba0: 0e12 0e12 0e12 1612 0e12 0e12 0e12 1a12  ................
+00005bb0: 0e12 1612 0e12 1112 0e12 1712 0e12 2612  ..............&.
+00005bc0: 0e12 0e12 0e12 0e12 0e12 0e12 0e12 0e12  ................
+00005bd0: 0e12 1612 0e12 1a12 0e12 1112 0e12 1112  ................
+00005be0: 0e12 1112 0e12 11                        .......
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,50 @@
         Parameters:
             process: Process updated
         """
         super().__init__(**kwargs)
         self.process = process
 
 
+class SaveProcessEntityDataRequest(_serialization.Model):
+    _attribute_map = {
+        "process_id": {"key": "processId", "type": "str"},
+        "data": {"key": "data", "type": "{object}"},
+    }
+
+    def __init__(
+        self,
+        process_id: str,
+        data: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
+    ) -> None:
+        """
+        Parameters:
+            process_id: Process identifier to update
+            data: Data values
+        """
+        super().__init__(**kwargs)
+        self.process_id = process_id
+        self.data = data or {}
+
+
+class SaveProcessEntityDataResponse(_serialization.Model):
+    _attribute_map = {
+        "process": {"key": "process", "type": "Process"},
+    }
+
+    def __init__(self, process: models_rest.Process, **kwargs: Any) -> None:
+        """
+        Parameters:
+            process: Process updated
+        """
+        super().__init__(**kwargs)
+        self.process = process
+
+
 class DeleteProcessElementRequest(_serialization.Model):
     _attribute_map = {
         "process_id": {"key": "processId", "type": "str"},
         "element_definition_code": {"key": "elementDefinitionCode", "type": "str"},
     }
 
     def __init__(self, process_id: str, element_definition_code: str, **kwargs: Any) -> None:
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__init__.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 15 12:57:18 2024 UTC, .py size: 11189 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ae45 f465 b52b 0000  U........E.e.+..
+00000000: 550d 0d0a 0000 0000 1c2a 1566 b52b 0000  U........*.f.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 15 12:57:18 2024 UTC, .py size: 14055 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ae45 f465 e736 0000  U........E.e.6..
+00000000: 550d 0d0a 0000 0000 1c2a 1566 e736 0000  U........*.f.6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 15 12:57:18 2024 UTC, .py size: 15409 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ae45 f465 313c 0000  U........E.e1<..
+00000000: 550d 0d0a 0000 0000 1c2a 1566 313c 0000  U........*.f1<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d00 5a00 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py` & `kuflow_temporal_activity_kuflow-1.5.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/pyproject.toml` & `kuflow_temporal_activity_kuflow-1.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "1.4.0"
+version = "1.5.0"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^1.4.0"
+kuflow-temporal-common = "^1.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ruff = ">=0.1.8,<1.0.0"
 pytest = "^7.3.1"
 pyyaml = "^6.0"
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/setup.py` & `kuflow_temporal_activity_kuflow-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
  'kuflow_temporal_activity_kuflow.models',
  'kuflow_temporal_activity_kuflow.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=1.4.0,<2.0.0']
+['kuflow-temporal-common>=1.5.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-1.4.0/PKG-INFO` & `kuflow_temporal_activity_kuflow-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 1.4.0
+Version: 1.5.0
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
-Requires-Dist: kuflow-temporal-common (>=1.4.0,<2.0.0)
+Requires-Dist: kuflow-temporal-common (>=1.5.0,<2.0.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

