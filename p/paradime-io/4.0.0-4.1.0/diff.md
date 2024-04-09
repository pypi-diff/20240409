# Comparing `tmp/paradime_io-4.0.0.tar.gz` & `tmp/paradime_io-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradime_io-4.0.0.tar", max compression
+gzip compressed data, was "paradime_io-4.1.0.tar", max compression
```

## Comparing `paradime_io-4.0.0.tar` & `paradime_io-4.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1074 2024-03-21 14:29:53.412536 paradime_io-4.0.0/LICENSE
--rw-r--r--   0        0        0     1060 2024-03-21 14:29:53.412536 paradime_io-4.0.0/README.md
--rw-r--r--   0        0        0       84 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/audit_log/__init__.py
--rw-r--r--   0        0        0     1901 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/audit_log/client.py
--rw-r--r--   0        0        0      423 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/audit_log/types.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/bolt/__init__.py
--rw-r--r--   0        0        0    11566 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/bolt/client.py
--rw-r--r--   0        0        0     1609 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/bolt/types.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/custom_integration/__init__.py
--rw-r--r--   0        0        0    12369 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/custom_integration/client.py
--rw-r--r--   0        0        0    17115 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/custom_integration/types.py
--rw-r--r--   0        0        0      321 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/custom_integration/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/users/__init__.py
--rw-r--r--   0        0        0     4052 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/users/client.py
--rw-r--r--   0        0        0      656 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/users/types.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/workspaces/__init__.py
--rw-r--r--   0        0        0      823 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/workspaces/client.py
--rw-r--r--   0        0        0       88 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/apis/workspaces/types.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/cli/__init__.py
--rw-r--r--   0        0        0     3138 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/cli/bolt.py
--rw-r--r--   0        0        0      538 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/cli/cli.py
--rw-r--r--   0        0        0      963 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/cli/login.py
--rw-r--r--   0        0        0      192 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/cli/version.py
--rw-r--r--   0        0        0     3437 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/client/api_client.py
--rw-r--r--   0        0        0      231 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/client/api_exception.py
--rw-r--r--   0        0        0      974 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/client/paradime_cli_client.py
--rw-r--r--   0        0        0     1692 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/client/paradime_client.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/core/bolt/__init__.py
--rw-r--r--   0        0        0     5615 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/core/bolt/schedule.py
--rw-r--r--   0        0        0      376 2024-03-21 14:29:53.416536 paradime_io-4.0.0/paradime/version.py
--rw-r--r--   0        0        0     1122 2024-03-21 14:29:53.416536 paradime_io-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 paradime_io-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-09 12:10:15.356576 paradime_io-4.1.0/LICENSE
+-rw-r--r--   0        0        0     1060 2024-04-09 12:10:15.356576 paradime_io-4.1.0/README.md
+-rw-r--r--   0        0        0       84 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/audit_log/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/audit_log/client.py
+-rw-r--r--   0        0        0      423 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/audit_log/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/bolt/__init__.py
+-rw-r--r--   0        0        0    14252 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/bolt/client.py
+-rw-r--r--   0        0        0      387 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/bolt/exception.py
+-rw-r--r--   0        0        0     1609 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/bolt/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.356576 paradime_io-4.1.0/paradime/apis/custom_integration/__init__.py
+-rw-r--r--   0        0        0    12369 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/custom_integration/client.py
+-rw-r--r--   0        0        0    17115 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/custom_integration/types.py
+-rw-r--r--   0        0        0      321 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/custom_integration/utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/users/__init__.py
+-rw-r--r--   0        0        0     4052 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/users/client.py
+-rw-r--r--   0        0        0      656 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/users/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/workspaces/__init__.py
+-rw-r--r--   0        0        0      823 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/workspaces/client.py
+-rw-r--r--   0        0        0       88 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/apis/workspaces/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/cli/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/cli/bolt.py
+-rw-r--r--   0        0        0      538 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/cli/cli.py
+-rw-r--r--   0        0        0      963 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/cli/login.py
+-rw-r--r--   0        0        0      192 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/cli/version.py
+-rw-r--r--   0        0        0     3437 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/client/api_client.py
+-rw-r--r--   0        0        0      231 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/client/api_exception.py
+-rw-r--r--   0        0        0      974 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/client/paradime_cli_client.py
+-rw-r--r--   0        0        0     1692 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/client/paradime_client.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/core/bolt/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/core/bolt/schedule.py
+-rw-r--r--   0        0        0      376 2024-04-09 12:10:15.360576 paradime_io-4.1.0/paradime/version.py
+-rw-r--r--   0        0        0     1138 2024-04-09 12:10:15.360576 paradime_io-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 paradime_io-4.1.0/PKG-INFO
```

### Comparing `paradime_io-4.0.0/LICENSE` & `paradime_io-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/README.md` & `paradime_io-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/audit_log/client.py` & `paradime_io-4.1.0/paradime/apis/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/bolt/client.py` & `paradime_io-4.1.0/paradime/apis/bolt/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from typing import List, Optional
 
+import requests
+
+from paradime.apis.bolt.exception import (
+    BoltScheduleArtifactNotFoundException,
+    BoltScheduleLatestRunNotFoundException,
+)
 from paradime.apis.bolt.types import (
     BoltCommand,
     BoltCommandArtifact,
     BoltDeferredSchedule,
     BoltRunState,
     BoltSchedule,
     BoltScheduleInfo,
@@ -343,7 +349,76 @@
                 cancelBoltRun(scheduleRunId: $runId) {
                     ok
                 }
             }
         """
 
         self.client._call_gql(query=query, variables={"runId": int(run_id)})
+
+    def get_latest_artifact_url(
+        self, *, schedule_name: str, artifact_path: str, command_index: Optional[int] = None
+    ) -> str:
+        """
+        Retrieves the URL of the latest artifact for a given schedule.
+
+        Args:
+            schedule_name (str): The name of the schedule.
+            artifact_path (str): The path of the artifact.
+            command_index (Optional[int]): The index of the command in the schedule. Defaults to searching through all commands from the last command to the first.
+
+        Returns:
+            str: The URL of the latest artifact.
+        """
+
+        # Get the latest run ID for the schedule
+        schedule = self.get_schedule(schedule_name)
+        latest_run_id = schedule.latest_run_id
+        if not latest_run_id:
+            raise BoltScheduleLatestRunNotFoundException(
+                f"No latest run ID found for schedule {schedule_name!r}."
+            )
+
+        # Get all the commands for the schedule
+        all_commands = self.list_run_commands(latest_run_id)
+        commands_to_look = all_commands[::-1]
+        if command_index is not None:
+            commands_to_look = [all_commands[command_index]]
+
+        # Find the artifact
+        artifact_id = None
+        for command in commands_to_look:
+            artifacts = self.list_command_artifacts(command.id)
+            for artifact in artifacts:
+                if artifact.path == artifact_path:
+                    artifact_id = artifact.id
+                    break
+        if artifact_id is None:
+            raise BoltScheduleArtifactNotFoundException(
+                f"No artifact found for schedule {schedule_name!r} and run id {latest_run_id}."
+            )
+
+        # Get the URL of the artifact
+        artifact_url = self.get_artifact_url(artifact_id)
+
+        return artifact_url
+
+    def get_latest_manifest_json(
+        self, schedule_name: str, command_index: Optional[int] = None
+    ) -> dict:
+        """
+        Retrieves the latest manifest JSON for a given schedule.
+
+        Args:
+            schedule_name (str): The name of the schedule.
+            command_index (Optional[int]): The index of the command in the schedule. Defaults to None.
+
+        Returns:
+            dict: The content of the latest manifest JSON.
+        """
+
+        manifest_url = self.get_latest_artifact_url(
+            schedule_name=schedule_name,
+            artifact_path="target/manifest.json",
+            command_index=command_index,
+        )
+
+        return requests.get(manifest_url).json()
```

### Comparing `paradime_io-4.0.0/paradime/apis/bolt/types.py` & `paradime_io-4.1.0/paradime/apis/bolt/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/custom_integration/client.py` & `paradime_io-4.1.0/paradime/apis/custom_integration/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/custom_integration/types.py` & `paradime_io-4.1.0/paradime/apis/custom_integration/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/users/client.py` & `paradime_io-4.1.0/paradime/apis/users/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/users/types.py` & `paradime_io-4.1.0/paradime/apis/users/types.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/apis/workspaces/client.py` & `paradime_io-4.1.0/paradime/apis/workspaces/client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/cli/bolt.py` & `paradime_io-4.1.0/paradime/cli/bolt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Final, List
 
 import click
 
 from paradime.apis.bolt.types import BoltRunState
 from paradime.client.api_exception import ParadimeAPIException
-from paradime.client.paradime_cli_client import get_cli_client, get_cli_client_or_exit
+from paradime.client.paradime_cli_client import get_cli_client_or_exit
 from paradime.core.bolt.schedule import (
     SCHEDULE_FILE_NAME,
     is_allowed_command,
     is_valid_schedule_at_path,
     parse_command,
 )
```

### Comparing `paradime_io-4.0.0/paradime/cli/cli.py` & `paradime_io-4.1.0/paradime/cli/cli.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/cli/login.py` & `paradime_io-4.1.0/paradime/cli/login.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/client/api_client.py` & `paradime_io-4.1.0/paradime/client/api_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/client/paradime_cli_client.py` & `paradime_io-4.1.0/paradime/client/paradime_cli_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/client/paradime_client.py` & `paradime_io-4.1.0/paradime/client/paradime_client.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/paradime/core/bolt/schedule.py` & `paradime_io-4.1.0/paradime/core/bolt/schedule.py`

 * *Files identical despite different names*

### Comparing `paradime_io-4.0.0/pyproject.toml` & `paradime_io-4.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paradime-io"
-version = "4.0.0"
+version = "4.1.0"
 description = "Paradime - Python SDK"
 authors = ["Bhuvan Singla <bhuvan@paradime.io>", "Maximilian Mitchell <max@paradime.io>"]
 readme = "README.md"
 packages = [
 	{ include = "paradime", from = "." },
 ]
 
@@ -22,14 +22,15 @@
 
 
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.20240125"
 mypy = "^1.8.0"
 black = "^24.2.0"
 isort = "^5.13.2"
+ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.mypy]
```

### Comparing `paradime_io-4.0.0/PKG-INFO` & `paradime_io-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradime-io
-Version: 4.0.0
+Version: 4.1.0
 Summary: Paradime - Python SDK
 Author: Bhuvan Singla
 Author-email: bhuvan@paradime.io
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paradime-io Version: 4.0.0 Summary: Paradime -
+Metadata-Version: 2.1 Name: paradime-io Version: 4.1.0 Summary: Paradime -
 Python SDK Author: Bhuvan Singla Author-email: bhuvan@paradime.io Requires-
 Python: >=3.8 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: croniter
 (>=2.0.2,<3.0.0) Requires-Dist: pydantic (==1.10.14) Requires-Dist: python-
```

