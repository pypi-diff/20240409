# Comparing `tmp/camunda_client-0.4.8.tar.gz` & `tmp/camunda_client-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camunda_client-0.4.8.tar", last modified: Wed Feb  7 09:22:30 2024, max compression
+gzip compressed data, was "camunda_client-0.4.9.tar", last modified: Wed Feb 14 06:46:04 2024, max compression
```

## Comparing `camunda_client-0.4.8.tar` & `camunda_client-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11558 2023-12-22 07:42:20.860234 camunda_client-0.4.8/LICENSE
--rw-r--r--   0        0        0     1349 2023-12-15 08:09:13.178810 camunda_client-0.4.8/README.md
--rw-r--r--   0        0        0      672 2024-02-07 09:22:13.666926 camunda_client-0.4.8/camunda_client/__init__.py
--rw-r--r--   0        0        0      264 2024-01-30 10:19:51.819407 camunda_client-0.4.8/camunda_client/clients/__init__.py
--rw-r--r--   0        0        0      160 2023-12-13 15:24:20.689086 camunda_client-0.4.8/camunda_client/clients/dto.py
--rw-r--r--   0        0        0     1997 2024-02-07 06:42:15.519849 camunda_client-0.4.8/camunda_client/clients/endpoints.py
--rw-r--r--   0        0        0       78 2024-01-30 10:22:03.617327 camunda_client-0.4.8/camunda_client/clients/engine/__init__.py
--rw-r--r--   0        0        0     9076 2024-02-07 06:42:15.519849 camunda_client-0.4.8/camunda_client/clients/engine/client.py
--rw-r--r--   0        0        0      666 2024-01-30 10:26:29.635222 camunda_client-0.4.8/camunda_client/clients/engine/schemas/__init__.py
--rw-r--r--   0        0        0      818 2024-01-12 09:59:32.782307 camunda_client-0.4.8/camunda_client/clients/engine/schemas/body.py
--rw-r--r--   0        0        0     1272 2023-12-18 14:13:19.265634 camunda_client-0.4.8/camunda_client/clients/engine/schemas/enums.py
--rw-r--r--   0        0        0     2149 2023-12-19 13:13:57.975227 camunda_client-0.4.8/camunda_client/clients/engine/schemas/query.py
--rw-r--r--   0        0        0     3359 2024-02-07 09:22:03.157633 camunda_client-0.4.8/camunda_client/clients/engine/schemas/response.py
--rw-r--r--   0        0        0      149 2023-12-08 11:58:13.037949 camunda_client-0.4.8/camunda_client/clients/external_task/__init__.py
--rw-r--r--   0        0        0     5849 2023-12-19 13:17:55.622703 camunda_client-0.4.8/camunda_client/clients/external_task/client.py
--rw-r--r--   0        0        0      454 2023-12-12 11:59:14.251852 camunda_client-0.4.8/camunda_client/clients/external_task/dto.py
--rw-r--r--   0        0        0      442 2023-12-19 13:08:35.987494 camunda_client-0.4.8/camunda_client/clients/external_task/schemas/__init__.py
--rw-r--r--   0        0        0     1809 2023-12-19 13:21:43.082009 camunda_client-0.4.8/camunda_client/clients/external_task/schemas/body.py
--rw-r--r--   0        0        0     1015 2024-01-17 05:11:48.547169 camunda_client-0.4.8/camunda_client/clients/external_task/schemas/response.py
--rw-r--r--   0        0        0      266 2024-02-07 06:42:15.519849 camunda_client-0.4.8/camunda_client/clients/schemas.py
--rw-r--r--   0        0        0      361 2023-12-13 15:09:13.016072 camunda_client-0.4.8/camunda_client/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-22 13:28:02.138549 camunda_client-0.4.8/camunda_client/py.typed
--rw-r--r--   0        0        0     1330 2023-12-18 11:58:42.723066 camunda_client-0.4.8/camunda_client/types_.py
--rw-r--r--   0        0        0     2116 2024-02-06 14:30:09.815074 camunda_client-0.4.8/camunda_client/utils.py
--rw-r--r--   0        0        0      283 2024-01-30 10:18:45.043783 camunda_client-0.4.8/camunda_client/worker/__init__.py
--rw-r--r--   0        0        0     2356 2024-01-30 10:26:29.635222 camunda_client-0.4.8/camunda_client/worker/context.py
--rw-r--r--   0        0        0      855 2023-12-18 11:58:49.515348 camunda_client-0.4.8/camunda_client/worker/dto.py
--rw-r--r--   0        0        0     2747 2023-12-15 14:00:19.416929 camunda_client-0.4.8/camunda_client/worker/task_worker.py
--rw-r--r--   0        0        0     1263 2023-12-12 12:05:01.022693 camunda_client-0.4.8/camunda_client/worker/topic_consumer.py
--rw-r--r--   0        0        0     2682 2024-02-07 09:22:30.676910 camunda_client-0.4.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-12 12:46:36.064757 camunda_client-0.4.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 08:09:52.502326 camunda_client-0.4.8/tests/camunda_client/__init__.py
--rw-r--r--   0        0        0     2795 2024-01-11 08:09:52.502326 camunda_client-0.4.8/tests/camunda_client/test_deserialize.py
--rw-r--r--   0        0        0      134 2024-01-11 08:09:52.502326 camunda_client-0.4.8/tests/conftest.py
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 camunda_client-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-12-22 07:42:20.860234 camunda_client-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1349 2023-12-15 08:09:13.178810 camunda_client-0.4.9/README.md
+-rw-r--r--   0        0        0      672 2024-02-14 06:45:24.844281 camunda_client-0.4.9/camunda_client/__init__.py
+-rw-r--r--   0        0        0      264 2024-01-30 10:19:51.819407 camunda_client-0.4.9/camunda_client/clients/__init__.py
+-rw-r--r--   0        0        0      160 2023-12-13 15:24:20.689086 camunda_client-0.4.9/camunda_client/clients/dto.py
+-rw-r--r--   0        0        0     2120 2024-02-14 06:41:34.352237 camunda_client-0.4.9/camunda_client/clients/endpoints.py
+-rw-r--r--   0        0        0       78 2024-01-30 10:22:03.617327 camunda_client-0.4.9/camunda_client/clients/engine/__init__.py
+-rw-r--r--   0        0        0     8711 2024-02-14 06:41:34.352237 camunda_client-0.4.9/camunda_client/clients/engine/client.py
+-rw-r--r--   0        0        0      666 2024-01-30 10:26:29.635222 camunda_client-0.4.9/camunda_client/clients/engine/schemas/__init__.py
+-rw-r--r--   0        0        0      882 2024-02-14 06:41:34.353236 camunda_client-0.4.9/camunda_client/clients/engine/schemas/body.py
+-rw-r--r--   0        0        0     1272 2023-12-18 14:13:19.265634 camunda_client-0.4.9/camunda_client/clients/engine/schemas/enums.py
+-rw-r--r--   0        0        0     2149 2023-12-19 13:13:57.975227 camunda_client-0.4.9/camunda_client/clients/engine/schemas/query.py
+-rw-r--r--   0        0        0     3359 2024-02-07 09:22:03.157633 camunda_client-0.4.9/camunda_client/clients/engine/schemas/response.py
+-rw-r--r--   0        0        0      149 2023-12-08 11:58:13.037949 camunda_client-0.4.9/camunda_client/clients/external_task/__init__.py
+-rw-r--r--   0        0        0     5849 2023-12-19 13:17:55.622703 camunda_client-0.4.9/camunda_client/clients/external_task/client.py
+-rw-r--r--   0        0        0      454 2023-12-12 11:59:14.251852 camunda_client-0.4.9/camunda_client/clients/external_task/dto.py
+-rw-r--r--   0        0        0      442 2023-12-19 13:08:35.987494 camunda_client-0.4.9/camunda_client/clients/external_task/schemas/__init__.py
+-rw-r--r--   0        0        0     1809 2023-12-19 13:21:43.082009 camunda_client-0.4.9/camunda_client/clients/external_task/schemas/body.py
+-rw-r--r--   0        0        0     1015 2024-01-17 05:11:48.547169 camunda_client-0.4.9/camunda_client/clients/external_task/schemas/response.py
+-rw-r--r--   0        0        0      266 2024-02-07 06:42:15.519849 camunda_client-0.4.9/camunda_client/clients/schemas.py
+-rw-r--r--   0        0        0      361 2023-12-13 15:09:13.016072 camunda_client-0.4.9/camunda_client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-12-22 13:28:02.138549 camunda_client-0.4.9/camunda_client/py.typed
+-rw-r--r--   0        0        0     1330 2023-12-18 11:58:42.723066 camunda_client-0.4.9/camunda_client/types_.py
+-rw-r--r--   0        0        0     2116 2024-02-06 14:30:09.815074 camunda_client-0.4.9/camunda_client/utils.py
+-rw-r--r--   0        0        0      283 2024-01-30 10:18:45.043783 camunda_client-0.4.9/camunda_client/worker/__init__.py
+-rw-r--r--   0        0        0     2356 2024-01-30 10:26:29.635222 camunda_client-0.4.9/camunda_client/worker/context.py
+-rw-r--r--   0        0        0      855 2023-12-18 11:58:49.515348 camunda_client-0.4.9/camunda_client/worker/dto.py
+-rw-r--r--   0        0        0     2747 2023-12-15 14:00:19.416929 camunda_client-0.4.9/camunda_client/worker/task_worker.py
+-rw-r--r--   0        0        0     1263 2023-12-12 12:05:01.022693 camunda_client-0.4.9/camunda_client/worker/topic_consumer.py
+-rw-r--r--   0        0        0     2682 2024-02-14 06:46:04.344160 camunda_client-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-12 12:46:36.064757 camunda_client-0.4.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 08:09:52.502326 camunda_client-0.4.9/tests/camunda_client/__init__.py
+-rw-r--r--   0        0        0     2795 2024-01-11 08:09:52.502326 camunda_client-0.4.9/tests/camunda_client/test_deserialize.py
+-rw-r--r--   0        0        0      134 2024-01-11 08:09:52.502326 camunda_client-0.4.9/tests/conftest.py
+-rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 camunda_client-0.4.9/PKG-INFO
```

### Comparing `camunda_client-0.4.8/LICENSE` & `camunda_client-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/README.md` & `camunda_client-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/__init__.py` & `camunda_client-0.4.9/camunda_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     "ExternalTaskDTO",
     "process_variable",
     "VariableValueSchema",
     "Variables",
 ]
 
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
```

### Comparing `camunda_client-0.4.8/camunda_client/clients/endpoints.py` & `camunda_client-0.4.9/camunda_client/clients/endpoints.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,7 +62,11 @@
     @classmethod
     def claim_task(cls, task_id: str) -> str:
         return f"{cls.task}/{task_id}/claim"
 
     @classmethod
     def unclaim_task(cls, task_id: str) -> str:
         return f"{cls.task}/{task_id}/unclaim"
+
+    @classmethod
+    def set_assignee_task(cls, task_id: str) -> str:
+        return f"{cls.task}/{task_id}/assignee"
```

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/client.py` & `camunda_client-0.4.9/camunda_client/clients/engine/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from uuid import UUID
 
 import httpx
 from pydantic.type_adapter import TypeAdapter
 
 from camunda_client.clients.dto import AuthData
 from camunda_client.clients.endpoints import CamundaUrls
-from camunda_client.clients.engine.schemas.body import ClaimTaskSchema
+from camunda_client.clients.engine.schemas.body import (
+    ClaimTaskSchema,
+    SetAssigneeTaskSchema,
+)
 from camunda_client.clients.engine.schemas.response import (
     HistoricTaskInstanceSchema,
     TaskSchema,
     VariableInstanceSchema,
 )
 from camunda_client.clients.schemas import CountSchema, PaginationParams
 from camunda_client.types_ import Variables
@@ -233,35 +236,22 @@
     ) -> None:
         """
         Claims a task for a specific user.
         """
         response = await self._http_client.post(self._urls.unclaim_task(str(task_id)))
         raise_for_status(response)
 
-
-# • эндпоинт старта процесса
-# • эндпоинт получения списка юзер таск
-# эндпоинт получения списка юзер таск через фильтры ?
-# • эндпоинт для получения переменных user_task get_variables
-# • эндпоинт для завершения task
-# • эндпоинт get task history
-# • POST /task/{id}/claim
-# • POST /task/anId/unclaim
-
-
-"""
-
-
-    async def get_user_tasks(self) -> dict[str, Any]:
-        raise NotImplementedError
-
-    async def get_variables(self) -> dict[str, Any]:
-        raise NotImplementedError
-
-    async def get_process_history(self) -> dict[str, Any]:
-        raise NotImplementedError
-
-    async def get_task_count(self, user_id: UUID) -> dict[str, Any]:
-        raise NotImplementedError
-
-
-"""
+    async def set_assignee_task(
+        self,
+        task_id: UUID,
+        user_id: UUID,
+    ) -> None:
+        """
+        Changes the assignee of a task to a specific user..
+        """
+        response = await self._http_client.post(
+            self._urls.set_assignee_task(str(task_id)),
+            content=SetAssigneeTaskSchema(user_id=str(user_id)).model_dump_json(
+                by_alias=True,
+            ),
+        )
+        raise_for_status(response)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/schemas/__init__.py` & `camunda_client-0.4.9/camunda_client/clients/engine/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/schemas/body.py` & `camunda_client-0.4.9/camunda_client/clients/engine/schemas/body.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,7 +26,11 @@
     sorting: SortSchema | None = None
     process_instance_id: UUID | None = None
 
 
 class GetHistoryTasksFilterSchema(BaseSchema):
     process_instance_id: UUID | None = None
     sorting: SortSchema | None = None
+
+
+class SetAssigneeTaskSchema(BaseSchema):
+    user_id: str
```

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/schemas/enums.py` & `camunda_client-0.4.9/camunda_client/clients/engine/schemas/enums.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/schemas/query.py` & `camunda_client-0.4.9/camunda_client/clients/engine/schemas/query.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/engine/schemas/response.py` & `camunda_client-0.4.9/camunda_client/clients/engine/schemas/response.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/external_task/client.py` & `camunda_client-0.4.9/camunda_client/clients/external_task/client.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/external_task/schemas/body.py` & `camunda_client-0.4.9/camunda_client/clients/external_task/schemas/body.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/clients/external_task/schemas/response.py` & `camunda_client-0.4.9/camunda_client/clients/external_task/schemas/response.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/types_.py` & `camunda_client-0.4.9/camunda_client/types_.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/utils.py` & `camunda_client-0.4.9/camunda_client/utils.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/worker/context.py` & `camunda_client-0.4.9/camunda_client/worker/context.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/worker/dto.py` & `camunda_client-0.4.9/camunda_client/worker/dto.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/worker/task_worker.py` & `camunda_client-0.4.9/camunda_client/worker/task_worker.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/camunda_client/worker/topic_consumer.py` & `camunda_client-0.4.9/camunda_client/worker/topic_consumer.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/pyproject.toml` & `camunda_client-0.4.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "camunda-client"
-version = "0.4.8"
+version = "0.4.9"
 description = ""
 authors = [
     { name = "Strana Dev", email = "pypi@stranadev.ru" },
 ]
 dependencies = [
     "pydantic>=2.5.2",
     "httpx>=0.26.0",
@@ -65,15 +65,15 @@
     "camunda_client/clients/*",
     "camunda_client/exceptions.py",
     "camunda_client/types_.py",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.8"
+version = "0.4.9"
 version_files = [
     "camunda_client/__init__.py",
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
 plugins = [
```

### Comparing `camunda_client-0.4.8/tests/camunda_client/test_deserialize.py` & `camunda_client-0.4.9/tests/camunda_client/test_deserialize.py`

 * *Files identical despite different names*

### Comparing `camunda_client-0.4.8/PKG-INFO` & `camunda_client-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camunda-client
-Version: 0.4.8
+Version: 0.4.9
 Author-Email: Strana Dev <pypi@stranadev.ru>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/stranadev/camunda-client
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=2.5.2
 Requires-Dist: httpx>=0.26.0
 Requires-Dist: orjson>=3.9.10
```

