# Comparing `tmp/ado_wrapper-0.0.4.tar.gz` & `tmp/ado_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.4.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.5.tar", max compression
```

## Comparing `ado_wrapper-0.0.4.tar` & `ado_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.4/LICENSE
--rw-r--r--   0        0        0      516 2024-04-05 11:51:02.152589 ado_wrapper-0.0.4/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.4/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6432 2024-04-06 09:40:50.980917 ado_wrapper-0.0.4/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     1878 2024-04-07 10:54:07.604713 ado_wrapper-0.0.4/ado_wrapper/client.py
--rw-r--r--   0        0        0    17154 2024-04-07 10:01:31.474982 ado_wrapper-0.0.4/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.4/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.4/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     2999 2024-04-05 15:06:59.436804 ado_wrapper-0.0.4/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1173 2024-04-05 15:06:51.254984 ado_wrapper-0.0.4/ado_wrapper/plan_resources/singletons.py
--rw-r--r--   0        0        0      659 2024-04-07 11:10:47.369677 ado_wrapper-0.0.4/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4568 2024-04-07 12:20:36.607817 ado_wrapper-0.0.4/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    13854 2024-04-07 12:25:08.207236 ado_wrapper-0.0.4/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6586 2024-04-07 12:41:44.539525 ado_wrapper-0.0.4/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3622 2024-04-07 10:59:40.805971 ado_wrapper-0.0.4/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2087 2024-04-07 12:49:21.264048 ado_wrapper-0.0.4/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14999 2024-04-07 12:28:52.324575 ado_wrapper-0.0.4/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    13064 2024-04-07 11:01:07.349289 ado_wrapper-0.0.4/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0     9139 2024-04-07 12:30:48.891543 ado_wrapper-0.0.4/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5084 2024-04-07 12:49:15.437789 ado_wrapper-0.0.4/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4762 2024-04-07 12:49:33.320370 ado_wrapper-0.0.4/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8229 2024-04-07 12:50:04.637373 ado_wrapper-0.0.4/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     5117 2024-04-07 12:32:55.829004 ado_wrapper-0.0.4/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     7045 2024-04-07 12:41:33.897870 ado_wrapper-0.0.4/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8104 2024-04-06 09:40:50.988258 ado_wrapper-0.0.4/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4230 2024-04-07 10:39:34.190691 ado_wrapper-0.0.4/ado_wrapper/utils.py
--rw-r--r--   0        0        0     1997 2024-04-06 09:49:20.016252 ado_wrapper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 ado_wrapper-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.5/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.5/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.5/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6446 2024-04-08 17:57:20.745729 ado_wrapper-0.0.5/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2123 2024-04-09 20:35:21.978850 ado_wrapper-0.0.5/ado_wrapper/client.py
+-rw-r--r--   0        0        0    17177 2024-04-08 17:58:36.801350 ado_wrapper-0.0.5/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.5/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.5/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.5/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1805 2024-04-09 15:28:42.531252 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1497 2024-04-09 20:33:02.558531 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.5/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.5/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.5/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.5/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.5/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.5/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.5/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.5/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0     9135 2024-04-09 18:30:44.069270 ado_wrapper-0.0.5/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     6093 2024-04-09 18:53:39.689874 ado_wrapper-0.0.5/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.5/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8370 2024-04-09 18:46:26.714212 ado_wrapper-0.0.5/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.5/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8415 2024-04-09 18:32:40.182058 ado_wrapper-0.0.5/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8347 2024-04-09 20:34:04.740783 ado_wrapper-0.0.5/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.5/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2098 2024-04-09 09:42:33.352412 ado_wrapper-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.5/PKG-INFO
```

### Comparing `ado_wrapper-0.0.4/LICENSE` & `ado_wrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.4/ado_wrapper/__main__.py` & `ado_wrapper-0.0.5/ado_wrapper/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     )
     action_group = parser.add_mutually_exclusive_group()
     action_group.add_argument(
         "--plan", help="Runs a plan for the resources, rather than making them", action="store_true", default=False, dest="plan"
     )
     action_group.add_argument("--apply", help="Applies the plan to the resources", action="store_true", default=False, dest="apply")
     parser.add_argument(
-        "--purge-state", "--wipe-state-", help="Deletes everything in the state file", action="store_true", default=False, dest="purge_state"
+        "--purge-state", "--wipe-state-", help="Deletes everything in the state file", action="store_true", default=False, dest="purge_state"  # fmt: skip
     )
     parser.add_argument("--state-file", help="The name of the state file to use", type=str, default="main.state", dest="state_file")
     args = parser.parse_args()
 
     if args.email is None and args.token is None and args.ado_org is None and args.ado_project is None and args.creds_file is None:
         raise ValueError("You must provide either --email and --token or --creds_file")
 
@@ -99,9 +99,10 @@
                     internal_state["resources"][resource_type][resource_id] = instance.to_json()
         ado_client.state_manager.write_state_file(internal_state)
 
     if args.plan:
         print("[ADO_WRAPPER] Running plan for resources:")
         # Plan for resources
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/client.py` & `ado_wrapper-0.0.5/ado_wrapper/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from typing import Literal
+
 import requests
 from requests.auth import HTTPBasicAuth
 
 from ado_wrapper.state_manager import StateManager
+from ado_wrapper.plan_resources.plan_state_manager import PlanStateManager
 from ado_wrapper.utils import AuthenticationError
 
 
 class AdoClient:
     def __init__(  # pylint: disable=too-many-arguments
         self, ado_email: str, ado_pat: str, ado_org: str, ado_project: str,
-        state_file_name: str | None = "main.state", bypass_initialisation: bool = False # fmt: skip
+        state_file_name: str | None = "main.state", bypass_initialisation: bool = False,
+        action: Literal["plan", "apply"] = "apply"  # fmt: skip
     ) -> None:
         """Takes an email, PAT, org, project, and state file name. The state file name is optional, and if not provided,
         state will not be stored in "main.state" """
         self.ado_email = ado_email
         self.ado_pat = ado_pat
         self.auth = HTTPBasicAuth(ado_email, ado_pat)
         self.ado_org = ado_org
         self.ado_project = ado_project
-        self.plan = False
+        self.plan_mode = action == "plan"
 
         if not bypass_initialisation:
             # Verify Token is working (helps with setup for first time users):
             request = requests.get(f"https://dev.azure.com/{self.ado_org}/_apis/projects?api-version=7.1", auth=self.auth)
             if request.status_code != 200:
                 raise AuthenticationError(f"Failed to authenticate with ADO: {request.text}")
 
             from ado_wrapper.resources.projects import Project  # Stop circular import
-            self.ado_project_id = Project.get_by_name(self, self.ado_project).project_id  # type: ignore[union-attr]
-
             from ado_wrapper.resources.users import AdoUser  # Stop circular import
+
+            self.ado_project_id = Project.get_by_name(self, self.ado_project).project_id  # type: ignore[union-attr]
             try:
                 self.pat_author: AdoUser = AdoUser.get_by_email(self, ado_email)
             except ValueError:
-                print(f"[ADO_WRAPPER] WARNING: User {ado_email} not found in ADO, nothing critical, but stops releases from being made, and plans from being accurate.")
+                print(
+                    f"[ADO_WRAPPER] WARNING: User {ado_email} not found in ADO, nothing critical, but stops releases from being made, and plans from being accurate."
+                )
 
-        self.state_manager: StateManager = StateManager(self, state_file_name)  # Has to be last
+        self.state_manager = StateManager(self, state_file_name) if action == "apply" else PlanStateManager(self)  # Has to be last
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/dumps.py` & `ado_wrapper-0.0.5/ado_wrapper/dumps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,199 @@
 """This file hosts a collection of dumps with the purpose of documenting the responses, all personal information has been removed."""
 
+# fmt: off
+
 ADO_USER_DUMP = {
-    'subjectKind': 'user',
-    'metaType': 'member',
-    'directoryAlias': '<first.last>',
-    'domain': '<32_char_uuid>',
-    'principalName': '<first.last@company.com>',
-    'mailAddress': '<first.last@company.com>',
-    'origin': 'aad',
-    'originId': '<32_char_uuid>',
-    'displayName': '<First> <Last>',
-    '_links': {'self': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>'}, 'memberships': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Memberships/<user_descriptor>'}, 'membershipState': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/MembershipStates/<user_descriptor>'}, 'storageKey': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/StorageKeys/<user_descriptor>'}, 'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}},
-    'url': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>',
-    'descriptor': '<user_descriptor>',
+    "subjectKind": "user",
+    "metaType": "member",
+    "directoryAlias": "<first.last>",
+    "domain": "<32_char_uuid>",
+    "principalName": "<first.last@company.com>",
+    "mailAddress": "<first.last@company.com>",
+    "origin": "aad",
+    "originId": "<32_char_uuid>",
+    "displayName": "<First> <Last>",
+    "_links": {"self": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>"}, "memberships": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Memberships/<user_descriptor>"}, "membershipState": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/MembershipStates/<user_descriptor>"}, "storageKey": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/StorageKeys/<user_descriptor>"}, "avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}},
+    "url": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>",
+    "descriptor": "<user_descriptor>",
 }
 
 BRANCH_DUMP = {
-    'name': 'refs/heads/test-branch',
-    'objectId': '<object_id>',
-    'creator': {'displayName': '<First> <Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}}, 'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_api/_common/identityImage?id=<user_id>', 'descriptor': '<user_descriptor>'},
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs?filter=heads%2Ftest-branch',
+    "name": "refs/heads/test-branch",
+    "objectId": "<object_id>",
+    "creator": {"displayName": "<First> <Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_api/_common/identityImage?id=<user_id>", "descriptor": "<user_descriptor>"},
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs?filter=heads%2Ftest-branch",
 }
 
 BUILD_DUMP = {
-    '_links': {'self': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Builds/93458'}, 'web': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/results?buildId=93458'}, 'sourceVersionDisplayUri': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/{build_id}/sources'}, 'timeline': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/{build_id}/Timeline'}, 'badge': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/status/{build_def_id}'}},
-    'properties': {},
-    'tags': [],
-    'validationResults': [],
-    'plans': [
-        {'planId': '<32_char_id>'}
+    "_links": {"self": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Builds/93458"}, "web": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/results?buildId=93458"}, "sourceVersionDisplayUri": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/{build_id}/sources"}, "timeline": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/{build_id}/Timeline"}, "badge": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/status/{build_def_id}"}},
+    "properties": {},
+    "tags": [],
+    "validationResults": [],
+    "plans": [
+        {"planId": "<32_char_id>"}
     ],
-    'triggerInfo': {},
-    'id': "{build_id}",
-    'buildNumber': '20240101.1',
-    'status': 'notStarted',
-    'queueTime': '2024-03-17T11:03:29.2982876Z',
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Builds/{build_id}',
-    'definition': {'drafts': [], 'id': "{build_def_id}", 'name': 'ado_wrapper-test-build', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/{build_id}?revision=1', 'uri': 'vstfs:///Build/Definition/{build_id}', 'path': '\\', 'type': 'build', 'queueStatus': 'enabled', 'revision': 1, 'project': {'id': '{ado_client.project_id}', 'name': 'Platform', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': "{revision}", 'visibility': 'private', 'lastUpdateTime': '2024-01-01T12:14:30.36Z'}},
-    'buildNumberRevision': 1,
-    'project': {'id': '{ado_client.project_id}', 'name': 'Platform', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': 399, 'visibility': 'private', 'lastUpdateTime': '2024-02-06T14:14:30.36Z'},
-    'uri': 'vstfs:///Build/Build/93458',
-    'sourceBranch': 'refs/heads/my-branch',
-    'sourceVersion': '<commit_id>',
-    'queue': {'id': "{queue_id}", 'name': '<pool_name>', 'pool': {'id': "{pool_id}", 'name': '<pool_name'}},
-    'priority': 'normal',
-    'reason': 'manual',
-    'requestedFor': {'displayName': '<First Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}}, 'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>', 'descriptor': '<user_descriptor>'},
-    'requestedBy': {'displayName': '<First Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}}, 'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>', 'descriptor': '<user_descriptor>'},
-    'lastChangedDate': '2024-03-17T11:03:29.373Z',
-    'lastChangedBy': {'displayName': '<First Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}}, 'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>', 'descriptor': '<user_descriptor>'},
-    'orchestrationPlan': {'planId': '<plan_id>'},
-    'logs': {'id': 0, 'type': 'Container', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/93458/logs'},
-    'repository': {'id': '<repo_id>', 'type': 'TfsGit', 'name': 'ado_wrapper-test-repo-for-create-delete-builds', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds', 'clean': None, 'checkoutSubmodules': False},
-    'retainedByRelease': False,
-    'triggeredByBuild': None,
-    'appendCommitMessageToRunName': True
+    "triggerInfo": {},
+    "id": "{build_id}",
+    "buildNumber": "20240101.1",
+    "status": "notStarted",
+    "queueTime": "2024-03-17T11:03:29.2982876Z",
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Builds/{build_id}",
+    "definition": {"drafts": [], "id": "{build_def_id}", "name": "ado_wrapper-test-build", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/{build_id}?revision=1", "uri": "vstfs:///Build/Definition/{build_id}", "path": "\\", "type": "build", "queueStatus": "enabled", "revision": 1, "project": {"id": "{ado_client.project_id}", "name": "Platform", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": "{revision}", "visibility": "private", "lastUpdateTime": "2024-01-01T12:14:30.36Z"}},
+    "buildNumberRevision": 1,
+    "project": {"id": "{ado_client.project_id}", "name": "Platform", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"},
+    "uri": "vstfs:///Build/Build/93458",
+    "sourceBranch": "refs/heads/my-branch",
+    "sourceVersion": "<commit_id>",
+    "queue": {"id": "{queue_id}", "name": "<pool_name>", "pool": {"id": "{pool_id}", "name": "<pool_name"}},
+    "priority": "normal",
+    "reason": "manual",
+    "requestedFor": {"displayName": "<First Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>", "descriptor": "<user_descriptor>"},
+    "requestedBy": {"displayName": "<First Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>", "descriptor": "<user_descriptor>"},
+    "lastChangedDate": "2024-03-17T11:03:29.373Z",
+    "lastChangedBy": {"displayName": "<First Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>", "descriptor": "<user_descriptor>"},
+    "orchestrationPlan": {"planId": "<plan_id>"},
+    "logs": {"id": 0, "type": "Container", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/builds/93458/logs"},
+    "repository": {"id": "<repo_id>", "type": "TfsGit", "name": "ado_wrapper-test-repo-for-create-delete-builds", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds", "clean": None, "checkoutSubmodules": False},
+    "retainedByRelease": False,
+    "triggeredByBuild": None,
+    "appendCommitMessageToRunName": True
 }
 
 BUILD_DEFINITION_DUMP = {
-    'properties': {},
-    'tags': [],
-    '_links': {'self': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/2601?revision=1'}, 'web': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/definition?definitionId=2601'}, 'editor': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/designer?id=2601&_a=edit-build-definition'}, 'badge': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/status/2601'}},
-    'description': '<description>',
-    'jobAuthorizationScope': 'projectCollection',
-    'process': {'yamlFilename': 'build.yaml', 'type': 2},
-    'repository': {'id': '<repo_id>','type': 'TfsGit', 'name': 'ado_wrapper-test-repo-for-create-delete-builds', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds', 'defaultBranch': 'refs/heads/my-branch', 'clean': None, 'checkoutSubmodules': False},
-    'quality': 'definition',
-    'authoredBy': {'displayName': '<First> <Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}},'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>', 'descriptor': '<user_descriptor>'},
-    'drafts': [],
-    'queue': {'_links': {'self': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/build/Queues/575'}}, 'id': 575, 'name': '<pool_name>', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/build/Queues/575', 'pool': {'id': 195, 'name': '<pool_name>'}},
-    'id': 2601,
-    'name': 'ado_wrapper-test-build',
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/2601?revision=1',
-    'uri': 'vstfs:///Build/Definition/2601',
-    'path': '\\',
-    'type': 'build',
-    'queueStatus': 'enabled',
-    'revision': 1,
-    'createdDate': '2024-03-17T11:03:28.943Z',
-    'project': {'id': '{ado_client.project_id}', 'name': '{ado_client.project}', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': 399, 'visibility': 'private', 'lastUpdateTime': '2024-02-06T14:14:30.36Z'}
+    "properties": {},
+    "tags": [],
+    "_links": {"self": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/2601?revision=1"}, "web": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/definition?definitionId=2601"}, "editor": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_build/designer?id=2601&_a=edit-build-definition"}, "badge": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/status/2601"}},
+    "description": "<description>",
+    "jobAuthorizationScope": "projectCollection",
+    "process": {"yamlFilename": "build.yaml", "type": 2},
+    "repository": {"id": "<repo_id>","type": "TfsGit", "name": "ado_wrapper-test-repo-for-create-delete-builds", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds", "defaultBranch": "refs/heads/my-branch", "clean": None, "checkoutSubmodules": False},
+    "quality": "definition",
+    "authoredBy": {"displayName": "<First> <Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}},"id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>", "descriptor": "<user_descriptor>"},
+    "drafts": [],
+    "queue": {"_links": {"self": {"href": "https://dev.azure.com/{ado_client.org}/_apis/build/Queues/575"}}, "id": 575, "name": "<pool_name>", "url": "https://dev.azure.com/{ado_client.org}/_apis/build/Queues/575", "pool": {"id": 195, "name": "<pool_name>"}},
+    "id": 2601,
+    "name": "ado_wrapper-test-build",
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/build/Definitions/2601?revision=1",
+    "uri": "vstfs:///Build/Definition/2601",
+    "path": "\\",
+    "type": "build",
+    "queueStatus": "enabled",
+    "revision": 1,
+    "createdDate": "2024-03-17T11:03:28.943Z",
+    "project": {"id": "{ado_client.project_id}", "name": "{ado_client.project}", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"}
 }
 
 COMMIT_DUMP = {
-    'commitId': '<commit_id>',
-    'author': {'name': '<First Last>', 'email': '<first.last@company.com>', 'date': '2024-03-17T11:45:19Z'},
-    'committer': {'name': '<First Last>', 'email': '<first.last@company.com>', 'date': '2024-03-17T11:45:19Z'},
-    'comment': 'Add README.md',
-    'changeCounts': {'Add': 1, 'Edit': 0, 'Delete': 0},
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>',
-    'remoteUrl': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds/commit/<other_commit_id>',
+    "commitId": "<commit_id>",
+    "author": {"name": "<First Last>", "email": "<first.last@company.com>", "date": "2024-03-17T11:45:19Z"},
+    "committer": {"name": "<First Last>", "email": "<first.last@company.com>", "date": "2024-03-17T11:45:19Z"},
+    "comment": "Add README.md",
+    "changeCounts": {"Add": 1, "Edit": 0, "Delete": 0},
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>",
+    "remoteUrl": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-create-delete-builds/commit/<other_commit_id>",
 }
 
 GROUP_DUMP = {
-    'subjectKind': 'group',
-    'description': '{description}',
-    'domain': 'vstfs:///Classification/TeamProject/{group_id}',
-    'principalName': 'Our Team Name',
-    'mailAddress': None,
-    'origin': 'vsts',
-    'originId': '{originId}',
-    'displayName': 'Our Team',
-    '_links': {'self': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Groups/{subject_descriptor}'}, 'memberships': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Memberships/{subject_descriptor}'}, 'membershipState': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/MembershipStates/{subject_descriptor}'}, 'storageKey': {'href': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/StorageKeys/{subject_descriptor}'}},
-    'url': 'https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Groups/{subject_descriptor}'}
+    "subjectKind": "group",
+    "description": "{description}",
+    "domain": "vstfs:///Classification/TeamProject/{group_id}",
+    "principalName": "Our Team Name",
+    "mailAddress": None,
+    "origin": "vsts",
+    "originId": "{originId}",
+    "displayName": "Our Team",
+    "_links": {"self": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Groups/{subject_descriptor}"}, "memberships": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Memberships/{subject_descriptor}"}, "membershipState": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/MembershipStates/{subject_descriptor}"}, "storageKey": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/StorageKeys/{subject_descriptor}"}},
+    "url": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Groups/{subject_descriptor}"}
 
 
 PROJECT_DUMP = {
-    'id': '<32_char_uuid>',
-    'name': '<project_name>',
-    'description': '<description>',
-    'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/<project_id>',
-    'state': 'wellFormed',
-    'revision': 194,
-    'visibility': 'private',
-    'lastUpdateTime': '2024-03-18T16:41:05.14Z',
+    "id": "<32_char_uuid>",
+    "name": "<project_name>",
+    "description": "<description>",
+    "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/<project_id>",
+    "state": "wellFormed",
+    "revision": 194,
+    "visibility": "private",
+    "lastUpdateTime": "2024-03-18T16:41:05.14Z",
 }
 
 PULL_REQUEST_DUMP = {
-    'repository ': {'id': '<repo_id>', 'name': 'ado_wrapper-test-repo-for-get-pull-request-by-id', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>', 'project': {'id': '<project_id>', 'name': '<project_name>', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': 399, 'visibility': 'private', 'lastUpdateTime': '2024-02-06T14:14:30.36Z'}, 'size': 980, 'remoteUrl': 'https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id', 'sshUrl': 'git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/ado_wrapper-test-repo-for-get-pull-request-by-id', 'webUrl': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id', 'isDisabled': False, 'isInMaintenance': False},
-    'pullRequestId': "{pull_request_id}",
-    'codeReviewId': "{code_review_id}",
-    'status': 'active',
-    'createdBy': {'displayName': '<First Last>', 'url': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>', '_links': {'avatar': {'href': 'https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>'}}, 'id': '<user_id>', 'uniqueName': '<first.last@company.com>', 'imageUrl': 'https://dev.azure.com/{ado_client.org}/_api/_common/identityImage?id=<user_id>', 'descriptor': '<user_descriptor>'},
-    'creationDate': '2021-03-17T11:18:39.9163346Z',
-    'title': '<title>',
-    'description': '<description>',
-    'sourceRefName': 'refs/heads/test-branch',
-    'targetRefName': 'refs/heads/main',
-    'mergeStatus': 'succeeded',
-    'isDraft': False,
-    'mergeId': '<32_char_uuid>',
-    'lastMergeSourceCommit': {'commitId': '<commit_id>', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>'},
-    'lastMergeTargetCommit': {'commitId': '<commit_id>', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>'},
-    'lastMergeCommit': {'commitId': '<commit_id>', 'author': {'name': '<First Last>', 'email': '<first.last@company.com>', 'date': '2024-03-17T11:18:40Z'}, 'committer': {'name': '<First Last>', 'email': '<first.last@company.com>', 'date': '2024-03-17T11:18:40Z'}, 'comment': '<comment>', 'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>'},
-    'reviewers': [],
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237',
-    '_links': {'self': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237'}, 'repository': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>'}, 'workItems': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/workitems'}, 'sourceBranch': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs/heads/test-branch'}, 'targetBranch': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs/heads/main'}, 'statuses': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/statuses'}, 'sourceCommit': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>'}, 'targetCommit': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>'}, 'createdBy': {'href': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>'}, 'iterations': {'href': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/iterations'}},
-    'supportsIterations': True,
-    'artifactId': 'vstfs:///Git/PullRequestId/<project_id>%2f<repo_id>%2f10237'
+    "repository ": {"id": "<repo_id>", "name": "ado_wrapper-test-repo-for-get-pull-request-by-id", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>", "project": {"id": "<project_id>", "name": "<project_name>", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"}, "size": 980, "remoteUrl": "https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id", "sshUrl": "git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/ado_wrapper-test-repo-for-get-pull-request-by-id", "webUrl": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/ado_wrapper-test-repo-for-get-pull-request-by-id", "isDisabled": False, "isInMaintenance": False},
+    "pullRequestId": "{pull_request_id}",
+    "codeReviewId": "{code_review_id}",
+    "status": "active",
+    "createdBy": {"displayName": "<First Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_api/_common/identityImage?id=<user_id>", "descriptor": "<user_descriptor>"},
+    "creationDate": "2021-03-17T11:18:39.9163346Z",
+    "title": "<title>",
+    "description": "<description>",
+    "sourceRefName": "refs/heads/test-branch",
+    "targetRefName": "refs/heads/main",
+    "mergeStatus": "succeeded",
+    "isDraft": False,
+    "mergeId": "<32_char_uuid>",
+    "lastMergeSourceCommit": {"commitId": "<commit_id>", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>"},
+    "lastMergeTargetCommit": {"commitId": "<commit_id>", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>"},
+    "lastMergeCommit": {"commitId": "<commit_id>", "author": {"name": "<First Last>", "email": "<first.last@company.com>", "date": "2024-03-17T11:18:40Z"}, "committer": {"name": "<First Last>", "email": "<first.last@company.com>", "date": "2024-03-17T11:18:40Z"}, "comment": "<comment>", "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>"},
+    "reviewers": [],
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237",
+    "_links": {"self": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237"}, "repository": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>"}, "workItems": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/workitems"}, "sourceBranch": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs/heads/test-branch"}, "targetBranch": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs/heads/main"}, "statuses": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/statuses"}, "sourceCommit": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>"}, "targetCommit": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/commits/<commit_id>"}, "createdBy": {"href": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>"}, "iterations": {"href": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/pullRequests/10237/iterations"}},
+    "supportsIterations": True,
+    "artifactId": "vstfs:///Git/PullRequestId/<project_id>%2f<repo_id>%2f10237"
 }
 
 REPO_DUMP = {
-    'id': '<repo_id>',
-    'name': '{repo_name}',
-    'url': 'https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/{self.repo_id}',
-    'project': {'id': '{ado_client.project_id}', 'name': '{<project_name>}', 'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}', 'state': 'wellFormed', 'revision': 399, 'visibility': 'private', 'lastUpdateTime': '2024-02-06T14:14:30.36Z'},
-    'size': 0,
-    'remoteUrl': 'https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}',
-    'sshUrl': 'git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/{repo_name}',
-    'webUrl': 'https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}',
-    'isDisabled': False,
-    'isInMaintenance': False,
+    "id": "<repo_id>",
+    "name": "{repo_name}",
+    "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/{self.repo_id}",
+    "project": {"id": "{ado_client.project_id}", "name": "{<project_name>}", "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}", "state": "wellFormed", "revision": 399, "visibility": "private", "lastUpdateTime": "2024-02-06T14:14:30.36Z"},
+    "size": 0,
+    "remoteUrl": "https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}",
+    "sshUrl": "git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/{repo_name}",
+    "webUrl": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}",
+    "isDisabled": False,
+    "isInMaintenance": False,
 }
 
 SERVICE_ENDPOINT_DUMP = {
-    'data': {},
-    'id': '{service_endpoint_id}',
-    'name': '{service_connection_name}',
-    'type': 'github',
-    'url': 'https://github.com',
-    'createdBy': "<Member>",
-    'description': '{description}',
-    'authorization': {'parameters': {'AccessToken': None}, 'scheme': 'Token'},
-    'isShared': False,
-    'isOutdated': False, 'isReady': True,
-    'owner': 'Library',
-    'serviceEndpointProjectReferences': [{'projectReference': {'id': '{project_id}', 'name': '{project_name}'},
-                                          'name': '{service_connection_name}', 'description': '{description}'}]
+    "data": {},
+    "id": "{service_endpoint_id}",
+    "name": "{service_connection_name}",
+    "type": "github",
+    "url": "https://github.com",
+    "createdBy": "<Member>",
+    "description": "{description}",
+    "authorization": {"parameters": {"AccessToken": None}, "scheme": "Token"},
+    "isShared": False,
+    "isOutdated": False, "isReady": True,
+    "owner": "Library",
+    "serviceEndpointProjectReferences": [{"projectReference": {"id": "{project_id}", "name": "{project_name}"},
+                                          "name": "{service_connection_name}", "description": "{description}"}]
 }
 
 TEAM_DUMP = {
-    'id': '<32_char_uuid>',
-    'name': 'Systems Team',
-    'url': 'https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}/teams/<32_char_uuid>',
-    'description': '<description>',
-    'identityUrl': 'https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<32_char_uuid>',
-    'projectName': '<project_name',
-    'projectId': '<32_char_uuid>'
+    "id": "<32_char_uuid>",
+    "name": "Systems Team",
+    "url": "https://dev.azure.com/{ado_client.org}/_apis/projects/{ado_client.project_id}/teams/<32_char_uuid>",
+    "description": "<description>",
+    "identityUrl": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<32_char_uuid>",
+    "projectName": "<project_name",
+    "projectId": "<32_char_uuid>"
 }
 
 VARIABLE_GROUP_DUMP = {
-    'variables': {'a': {'value': 'b', 'isReadOnly': True}},
-    'id': 528,
-    'type': 'Vsts',
-    'name': 'ado_wrapper-test-for-create-delete',
-    'description': 'my_description',
-    'createdBy': {'displayName': None, 'id': '<user_id>'},
-    'createdOn': '2024-03-17T11:04:25.4233333Z',
-    'modifiedBy': {'displayName': None, 'id': '<user_id>'},
-    'modifiedOn': '2024-03-17T11:04:25.4233333Z',
-    'isShared': False,
-    'variableGroupProjectReferences': [
-        {'projectReference': {'id': '{ado_client.project_id}', 'name': '<project_name'}, 'name': '{repo_name}', 'description': '{description}'}
+    "variables": {"a": {"value": "b", "isReadOnly": True}},
+    "id": 528,
+    "type": "Vsts",
+    "name": "ado_wrapper-test-for-create-delete",
+    "description": "my_description",
+    "createdBy": {"displayName": None, "id": "<user_id>"},
+    "createdOn": "2024-03-17T11:04:25.4233333Z",
+    "modifiedBy": {"displayName": None, "id": "<user_id>"},
+    "modifiedOn": "2024-03-17T11:04:25.4233333Z",
+    "isShared": False,
+    "variableGroupProjectReferences": [
+        {"projectReference": {"id": "{ado_client.project_id}", "name": "<project_name"}, "name": "{repo_name}", "description": "{description}"}
     ]
 }
+
+# fmt: on
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ado_wrapper.resources.branches import Branch
 from ado_wrapper.resources.builds import Build, BuildDefinition
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
 from ado_wrapper.resources.repo import Repo, BuildRepository
+from ado_wrapper.resources.service_endpoint import ServiceEndpoint
 from ado_wrapper.resources.teams import Team
 from ado_wrapper.resources.users import AdoUser, TeamMember, Member, Reviewer
 from ado_wrapper.resources.variable_groups import VariableGroup
-from ado_wrapper.resources.service_endpoint import ServiceEndpoint
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/branches.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from __future__ import annotations
+
 from dataclasses import dataclass, field
-from typing import Literal
+from typing import Literal, TYPE_CHECKING
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 BranchEditableAttribute = Literal["name"]
 
+
 @dataclass
 class Branch(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/refs?view=azure-devops-rest-7.1
     This isn't entirely what I wanted, you can't branch without a commit, so I need to add a commit method to this class
     And overall, just use commits if you can.
     """
 
@@ -57,15 +62,15 @@
     def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str) -> list["Branch"]:
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/refs?filter=heads&api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "Branch":
+    def get_by_name(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "Branch | None":
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.name == branch_name:
                 return branch
         raise ValueError(f"Branch {branch_name} not found")
 
     @classmethod
     def get_main_branch(cls, ado_client: AdoClient, repo_id: str) -> "Branch":  # type: ignore[return]  # pylint: disable=inconsistent-return-statements
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/builds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from datetime import datetime
-from typing import Any, Literal
 from dataclasses import dataclass, field
+from typing import Any, Literal, TYPE_CHECKING
 import time
 
 import requests
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 from ado_wrapper.resources.repo import BuildRepository
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 BuildDefinitionEditableAttribute = Literal["name", "description"]
 BuildStatus = Literal["notStarted", "inProgress", "completed", "cancelling", "postponed", "notSet", "none"]
 QueuePriority = Literal["low", "belowNormal", "normal", "aboveNormal", "high"]
 
 # ========================================================================================================
 
 
@@ -61,31 +63,31 @@
     priority: QueuePriority = "normal"
 
     def __str__(self) -> str:
         return f"{self.build_number} ({self.build_id}), {self.status}"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Build":
-        requested_by = Member(data["requestedBy"]["displayName"], data["requestedBy"]["uniqueName"], data["requestedBy"]["id"])
+        requested_by = Member.from_request_payload(data["requestedBy"])
         build_repo = BuildRepository.from_request_payload(data["repository"])
         build_definition = BuildDefinition.from_request_payload(data["definition"]) if "definition" in data else None
         return cls(str(data["id"]), str(data["buildNumber"]), data["status"], requested_by, build_repo, data.get("templateParameters", {}),
                    build_definition, from_ado_date_string(data.get("startTime")), from_ado_date_string(data.get("finishTime")),
                    from_ado_date_string(data.get("queueTime")), data["reason"], data["priority"])  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, build_id: str) -> "Build":
-        return super().get_by_id(
+    def get_by_id(cls, ado_client: "AdoClient", build_id: str) -> "Build":
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
-        cls, ado_client: AdoClient, definition_id: str, source_branch: str = "refs/heads/main", permit_use_of_var_groups: bool = False,  # fmt: skip
+        cls, ado_client: "AdoClient", definition_id: str, source_branch: str = "refs/heads/main", permit_use_of_var_groups: bool = False,  # fmt: skip
     ) -> "Build":
         """`permit_var_groups` defines whether the variable group will be automatically allowed for the build or need manual approval."""
         # if permit_use_of_var_groups:
         #     rint(f"Variable Groups: {BuildDefinition.get_by_id(ado_client, definition_id).variable_groups}")
         #     for var_group_id in BuildDefinition.get_by_id(ado_client, definition_id).variable_groups:
         #         request = requests.patch(f"https://dev.azure.com/{ado_client.ado_org}/{definition_id}/_apis/pipelines/pipelinePermissions/variablegroup/{var_group_id}")  # fmt: skip
         #         rint(request.text, request.status_code)
@@ -93,44 +95,42 @@
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds?definitionId={definition_id}&api-version=7.1",
             {"reason": "An automated build created with the ado_wrapper Python library", "sourceBranch": source_branch},
         )  # type: ignore[return-value]
 
     @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, build_id: str) -> None:  # type: ignore[override]
+    def delete_by_id(cls, ado_client: "AdoClient", build_id: str) -> None:  # type: ignore[override]
         cls.delete_all_leases(ado_client, build_id)
         return super().delete_by_id(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds/{build_id}?api-version=7.1",
             build_id,
         )
 
-    def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: Any) -> None:  # type: ignore[override]
+    def update(self, ado_client: "AdoClient", attribute_name: str, attribute_value: Any) -> None:  # type: ignore[override]
         return super().update(
             ado_client, "patch",
             f"/{ado_client.ado_project}/_apis/build/builds/{self.build_id}?api-version=7.1",
             attribute_name, attribute_value, {attribute_name: attribute_value}  # fmt: skip
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_all_by_definition(cls, ado_client: AdoClient, definition_id: str) -> "list[Build]":
-        return super().get_all(ado_client,
+    def get_all_by_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Build]":
+        return super().get_all(
+            ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds?definitions={definition_id}&api-version=7.1",
         )  # type: ignore[return-value]
 
-    def delete(self, ado_client: AdoClient) -> None:
-        return self.delete_by_id(ado_client, self.build_id)
-
     @classmethod
-    def create_and_wait_until_completion(cls, ado_client: AdoClient, definition_id: str, branch_name: str = "main",
+    def create_and_wait_until_completion(cls, ado_client: "AdoClient", definition_id: str, branch_name: str = "main",
                                          max_timeout_seconds: int = 300) -> "Build":  # fmt: skip
         """Creates a build and waits until it is completed, or raises a TimeoutError if it takes too long.
         WARNING: This is a blocking operation, it will not return until the build is completed or the timeout is reached."""
         build = cls.create(ado_client, definition_id, branch_name, True)
         start_time = datetime.now()
         while True:
             build = Build.get_by_id(ado_client, build.build_id)
@@ -138,15 +138,15 @@
                 break
             if (datetime.now() - start_time).seconds > max_timeout_seconds:
                 raise TimeoutError(f"The build did not complete within {max_timeout_seconds} seconds ({max_timeout_seconds//60} minutes)")
             time.sleep(3)
         return build
 
     @staticmethod
-    def delete_all_leases(ado_client: AdoClient, build_id: str) -> None:
+    def delete_all_leases(ado_client: "AdoClient", build_id: str) -> None:
         leases_request = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}/leases?api-version=7.1",
             auth=ado_client.auth,
         )
         if leases_request.status_code != 200:
             print(f"Could not delete leases, {leases_request.status_code}")
             return
@@ -180,43 +180,40 @@
 
     def __str__(self) -> str:
         return f"{self.name}, {self.build_definition_id}, created by {self.created_by}, created on {self.created_date!s}"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "BuildDefinition":
         """Repo is not always present, Member is sometimes present, sometimes None"""
-        created_by = (
-            Member(data["authoredBy"]["displayName"], data["authoredBy"]["uniqueName"], data["authoredBy"]["id"])
-            if "authoredBy" in data else None
-        )  # fmt: skip
+        created_by = Member.from_request_payload(data["authoredBy"]) if "authoredBy" in data else None  # fmt: skip
         build_repository = BuildRepository.from_request_payload(data["repository"]) if "repository" in data else None
         return cls(str(data["id"]), data["name"], data.get("description", ""), data.get("process", {"yamlFilename": "UNKNOWN"})["yamlFilename"], created_by,
                 from_ado_date_string(data.get("createdDate")), build_repository, str(data["revision"]), data.get("process"), data.get("variables", {}), data.get("variableGroups", []))  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, build_definition_id: str) -> "BuildDefinition":
-        return super().get_by_id(
+    def get_by_id(cls, ado_client: "AdoClient", build_definition_id: str) -> "BuildDefinition":
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions/{build_definition_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
-        cls, ado_client: AdoClient, name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
+        cls, ado_client: "AdoClient", name: str, repo_id: str, repo_name: str, path_to_pipeline: str,
         description: str, agent_pool_id: str, variable_groups: list[str], branch_name: str = "main",  # fmt: skip
     ) -> "BuildDefinition":
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.0",
             payload=get_build_definition(name, repo_id, repo_name, path_to_pipeline, description, ado_client.ado_project,
                                          agent_pool_id, branch_name)  # fmt: skip
         )  # type: ignore[return-value]
         #  | {"variableGroups": [{"id": x for x in variable_groups}]},
 
-    def update(self, ado_client: AdoClient, attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
+    def update(self, ado_client: "AdoClient", attribute_name: BuildDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         if self.build_repo is None or self.process is None:
             raise ValueError("This build definition does not have a (repository or process) in its data, it cannot be updated")
         payload = (
             {"name": self.name, "id": self.build_definition_id, "revision": int(self.revision),
              "repository": {"id": self.build_repo.build_repository_id, "type": self.build_repo.type},
              "process": {"yamlFilename": self.process["yamlFilename"], "type": self.process["type"]}} | # fmt: skip
             {attribute_name: attribute_value}  # fmt: skip
@@ -225,44 +222,39 @@
             ado_client, "put",
             f"/{ado_client.ado_project}/_apis/build/definitions/{self.build_definition_id}?api-version=7.1", #secretsSourceDefinitionRevision={self.revision}&
             attribute_name, attribute_value, payload  # fmt: skip
         )
         self.revision = str(int(self.revision) + 1)
 
     @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, resource_id: str) -> None:  # type: ignore[override]
-        builds = Build.get_all_by_definition(ado_client, resource_id)
-        for build in builds:
-            build.delete(ado_client)
+    def delete_by_id(cls, ado_client: "AdoClient", resource_id: str) -> None:  # type: ignore[override]
+        for build in Build.get_all_by_definition(ado_client, resource_id):
+            build.delete(ado_client)  # Can't remove from state because retention policies etc.
         return super().delete_by_id(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions/{resource_id}?forceDelete=true&api-version=7.1",
             resource_id,
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> "list[BuildDefinition]":  # type: ignore[override]
+    def get_all(cls, ado_client: "AdoClient") -> "list[BuildDefinition]":  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/definitions?api-version=7.1",
         )  # type: ignore[return-value]
 
-    def get_all_builds_by_definition(self, ado_client: AdoClient) -> "list[Build]":
+    def get_all_builds_by_definition(self, ado_client: "AdoClient") -> "list[Build]":
         return Build.get_all_by_definition(ado_client, self.build_definition_id)
 
     @classmethod
-    def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str) -> "list[BuildDefinition]":
-        response = requests.get(
+    def get_all_by_repo_id(cls, ado_client: "AdoClient", repo_id: str) -> "list[BuildDefinition]":
+        return super().get_all(
+            ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/definitions?repositoryId={repo_id}&repositoryType={'TfsGit'}&api-version=7.1",
-            auth=ado_client.auth,
-        ).json()["value"]
-        return [cls.from_request_payload(build) for build in response]
-
-    def delete(self, ado_client: AdoClient) -> None:
-        return self.delete_by_id(ado_client, self.build_definition_id)
+        )  # type: ignore[return-value]
 
 
 # ========================================================================================================
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/commits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Literal, Any
 from datetime import datetime
 from dataclasses import dataclass, field
+from typing import Literal, Any, TYPE_CHECKING
 
 import requests
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.utils import from_ado_date_string, InvalidPermissionsError
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 ChangeType = Literal["edit", "add", "delete"]
 FIRST_COMMIT_ID = "0000000000000000000000000000000000000000"  # I don't know why this works, but it does, please leave it.
 
 
 def get_commit_body_template(old_object_id: str | None, updates: dict[str, str], branch_name: str, change_type: ChangeType, commit_message: str) -> dict[str, str | dict | list]:  # type: ignore[type-arg]
     return {
         "refUpdates": [
@@ -59,23 +61,23 @@
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Commit":
         member = Member(data["author"]["name"], data["author"]["email"], "UNKNOWN")
         return cls(data["commitId"], member, from_ado_date_string(data["author"]["date"]), data["comment"])
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str, commit_id: str) -> "Commit":  # type: ignore[override]
-        return super().get_by_id(
+    def get_by_id(cls, ado_client: "AdoClient", repo_id: str, commit_id: str) -> "Commit":  # type: ignore[override]
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits/{commit_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
-        cls, ado_client: AdoClient, repo_id: str, from_branch_name: str, to_branch_name: str, updates: dict[str, str], change_type: ChangeType, commit_message: str,  # fmt: skip
+        cls, ado_client: "AdoClient", repo_id: str, from_branch_name: str, to_branch_name: str, updates: dict[str, str], change_type: ChangeType, commit_message: str,  # fmt: skip
     ) -> "Commit":
         """Creates a commit in the given repository with the given updates and returns the commit object.
         Takes a branch to get the latest commit from (and to update), and a to_branch to fork to."""
         assert not (
             from_branch_name.startswith("refs/heads/") or to_branch_name.startswith("refs/heads/")
         ), "Branch names should not start with 'refs/heads/'"
         if not updates:
@@ -89,37 +91,37 @@
         if request.status_code == 403:
             raise InvalidPermissionsError("You do not have permission to create a commit in this repo (possibly due to main branch protections)")  # fmt: skip
         if not request.json().get("commits"):
             raise ValueError("The commit was not created successfully.\nError:", request.json())
         return cls.from_request_payload(request.json()["commits"][-1])
 
     @staticmethod
-    def delete_by_id(ado_client: AdoClient, commit_id: str) -> None:  # type: ignore[override]
+    def delete_by_id(ado_client: "AdoClient", commit_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_latest_by_repo(cls, ado_client: AdoClient, repo_id: str, branch_name: str | None = None) -> "Commit":
+    def get_latest_by_repo(cls, ado_client: "AdoClient", repo_id: str, branch_name: str | None = None) -> "Commit":
         return max(cls.get_all_by_repo(ado_client, repo_id, branch_name), key=lambda commit: commit.date)
 
     @classmethod
-    def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str, branch_name: str | None = None) -> "list[Commit]":
+    def get_all_by_repo(cls, ado_client: "AdoClient", repo_id: str, branch_name: str | None = None) -> "list[Commit]":
         """Returns a list of all commits in the given repository."""
         extra_query = (f"searchCriteria.itemVersion.version={branch_name}&searchCriteria.itemVersion.versionType={'branch'}&"
                        if branch_name is not None else "")  # fmt: skip
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits?{extra_query}api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def add_initial_readme(cls, ado_client: AdoClient, repo_id: str) -> "Commit":
+    def add_initial_readme(cls, ado_client: "AdoClient", repo_id: str) -> "Commit":
         default_commit_body = get_commit_body_template(None, {}, "main", "add", "")
         default_commit_body["commits"] = [{
             "comment": "Add README.md",
             "changes": [{
                 "changeType": 1, "item": {"path": "/README.md"},
                 "newContentTemplate": {"name": "README.md", "type": "readme"}
             }],
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "Group":
         return cls(data["url"].split("/_apis/Graph/Groups/", maxsplit=1)[1], data["displayName"], data.get("description", ""),
                    data["domain"].removeprefix("vstfs:///Classification/TeamProject/"), data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, group_descriptor: str) -> "Group":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/groups/{group_descriptor}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, name: str) -> "Group":  # type: ignore[override]
         raise NotImplementedError
@@ -55,29 +55,23 @@
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, group_name: str) -> "Group":
-        for group in cls.get_all(ado_client):
-            if group.name == group_name:
-                return group
-        raise ValueError(f"Group {group_name} not found")
+    def get_by_name(cls, ado_client: AdoClient, group_name: str) -> "Group | None":
+        return cls.get_by_abstract_filter(ado_client, lambda group: group.name == group_name)  # type: ignore[return-value, attr-defined]
 
     # def get_members(self, ado_client: AdoClient) -> list["GroupMember"]:
     #     request = requests.get(
     #         f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/groups/{self.group_id}/members?api-version=7.1-preview.2",
     #         auth=ado_client.auth,
     #     ).json()
     #     rint(request)
     #     # return [GroupMember.from_request_payload(member) for member in request]
 
-    def delete(self, ado_client: AdoClient, group_id: str) -> None:
-        self.delete_by_id(ado_client, group_id)
-
     @classmethod
     def get_all_by_member(cls, ado_client: AdoClient, member_descriptor_id: str) -> list["Group"]:
         raise NotImplementedError
         # Will finish this later
         # return [group for group in cls.get_all(ado_client) if group.group_descriptor == member_descriptor_id]
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from typing import Any
+from __future__ import annotations
+
+from typing import Any, TYPE_CHECKING
 from datetime import datetime
 from dataclasses import dataclass, field
 
-import requests
-
-from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 
 @dataclass
 class Project(StateManagedResource):
     "https://learn.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.1"
     project_id: str = field(metadata={"is_id_field": True})  # None are editable
     name: str
     description: str
@@ -18,15 +20,15 @@
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Project":
         return cls(data["id"], data["name"], data.get("description", ""), data.get("lastUpdateTime"))
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, project_id: str) -> "Project":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,
             f"/_apis/projects/{project_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, project_name: str, project_description: str) -> "Project":  # type: ignore[override]
         raise NotImplementedError
@@ -44,11 +46,8 @@
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, project_name: str) -> "Project | None":
-        for project in cls.get_all(ado_client):
-            if project.name == project_name:
-                return project
-        return None
+        return cls.get_by_abstract_filter(ado_client, lambda project: project.name == project_name)  # type: ignore[return-value, attr-defined]
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/pull_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,24 +41,24 @@
     def __str__(self) -> str:
         return f"PullRequest(id={self.pull_request_id}, title={self.title}, repo_name={self.repo.name}, author={self.author!s}, status={self.merge_status})"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "PullRequest":
         from ado_wrapper.resources.repo import Repo  # Circular import
 
-        author = Member(data["createdBy"]["displayName"], data["createdBy"]["uniqueName"], data["createdBy"]["id"])
+        author = Member.from_request_payload(data["createdBy"])
         reviewers = [Reviewer.from_request_payload(reviewer) for reviewer in data["reviewers"]]
         repository = Repo(data["repository"]["id"], data["repository"]["name"])
         return cls(str(data["pullRequestId"]), data["title"], data.get("description", ""), data["sourceRefName"],
                    data["targetRefName"], author, from_ado_date_string(data["creationDate"]), repository,
                    from_ado_date_string(data.get("closedDate")), data["isDraft"], data.get("mergeStatus", "notSet"), reviewers)  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, pull_request_id: str) -> "PullRequest":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/pullrequests/{pull_request_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, repo_id: str, from_branch_name: str, pull_request_title: str,
@@ -113,29 +113,26 @@
         request = requests.put(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/reviewers/{reviewer_id}?api-version=7.1",
                                 json={"vote": "0", "isRequired": "true"}, auth=ado_client.auth)  # fmt: skip
         assert request.status_code < 300
 
     def close(self, ado_client: AdoClient) -> None:
         self.update(ado_client, "merge_status", "abandoned")
 
-    def delete(self, ado_client: AdoClient) -> None:
-        self.delete_by_id(ado_client, self.pull_request_id)
-
     def mark_as_draft(self, ado_client: AdoClient) -> None:
         return self.update(ado_client, "is_draft", True)
 
     def unmark_as_draft(self, ado_client: AdoClient) -> None:
         return self.update(ado_client, "is_draft", True)
 
     def get_reviewers(self, ado_client: AdoClient) -> list[Member]:
         request = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/reviewers?api-version=7.1",
             auth=ado_client.auth,
         ).json()
-        return [Member(reviewer["displayName"], reviewer["uniqueName"], reviewer["id"]) for reviewer in request["value"]]
+        return [Member.from_request_payload(reviewer) for reviewer in request["value"]]
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list[PullRequest]:
         pull_requests = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?searchCriteria.status={status}&api-version=7.1",
             auth=ado_client.auth,
         ).json()
@@ -176,79 +173,86 @@
         """Gets a list of comments on a pull request, optionally ignoring system messages."""
         return [comment for thread in self.get_comment_threads(ado_client, ignore_system_messages) for comment in thread.comments]
 
     def post_comment(self, ado_client: AdoClient, content: str) -> PullRequestComment:
         payload = {"comments": [{"commentType": 1, "content": content}], "status": "1"}
         request = requests.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/threads?api-version=7.1",
-            json=payload, auth=ado_client.auth,
+            json=payload,
+            auth=ado_client.auth,
         ).json()
         return PullRequestComment.from_request_payload(request["comments"][0])
 
 
 @dataclass
 class PullRequestCommentThread(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-request-thread-comments/list?view=azure-devops-rest-7.1
     Represents a chain of comments on a pull request, with the status e.g. Resolved, Active, etc."""
+
     thread_id: str
     status: str | None
     comments: list["PullRequestComment"]
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "PullRequestCommentThread":
         comments = [PullRequestComment.from_request_payload(comment) for comment in data["comments"]]
         return cls(data["id"], data.get("status"), comments)
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, thread_id: str) -> PullRequestCommentThread:  # type: ignore[override]
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads/{thread_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, content: str) -> StateManagedResource:  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str, content: str) -> "PullRequest":  # type: ignore[override]
         return super().create(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads?api-version=7.1",
             {"comments": [{"commentType": 1, "content": content}]},
-        )
+        )  # type: ignore[return-value]
 
     def update(self, ado_client: AdoClient, attribute_name: PrCommentStatus, attribute_value: Any) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     def delete_by_id(self, ado_client: AdoClient, repo_id: str, pull_request_id: str, thread_id: str) -> None:  # type: ignore[override]
         return super().delete_by_id(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads/{thread_id}?api-version=7.1",
-            thread_id
+            thread_id,
         )
 
     @classmethod
     def get_all(cls, ado_client: AdoClient, repo_id: str, pull_request_id: str) -> list[PullRequestCommentThread]:  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/threads?api-version=7.1",
         )  # type: ignore[return-value]
 
+
 @dataclass
 class PullRequestComment:
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-request-thread-comments/list?view=azure-devops-rest-7.1
     Comments' content will be None if they've been deleted, or if they're system comments."""
+
     comment_id: str
     parent_comment_id: str = field(repr=False)
     content: str | None
     author: Member
     creation_date: datetime = field(repr=False)
     comment_type: CommentType
     is_deleted: bool = field(repr=False)
     liked_users: list[Member] = field(repr=False)
 
     def __str__(self) -> str:
-        return f"PullRequestComment(id={self.comment_id}, author_email=`{self.author.email}`, content=`{self.content}`, creation_date={self.creation_date}, comment_type={self.comment_type}" + (", is_deleted=True" if self.is_deleted else "") + ")"
+        return (
+            f"PullRequestComment(id={self.comment_id}, author_email=`{self.author.email}`, content=`{self.content}`, "
+            f"creation_date={self.creation_date}, comment_type={self.comment_type}{', is_deleted=True' if self.is_deleted else ''})"
+        )
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "PullRequestComment":
-        author = Member(data["author"]["displayName"], data["author"]["uniqueName"], data["author"]["id"])
-        liked_users = [Member(user["displayName"], user["uniqueName"], user["id"]) for user in data.get("usersLiked", [])]
+        author = Member.from_request_payload(data["author"])
+        liked_users = [Member.from_request_payload(user) for user in data.get("usersLiked", [])]
         return cls(str(data["id"]), str(data["parentCommentId"]), data.get("content"), author, from_ado_date_string(data["publishedDate"]),
                    data.get("commentType", "regular"), data.get("isDeleted", False), liked_users)  # fmt: skip
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/releases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from datetime import datetime
-from typing import Any, Literal
 from dataclasses import dataclass, field
+from typing import Any, Literal, TYPE_CHECKING
 
 import requests
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.resources.users import Member
 
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 ReleaseDefinitionEditableAttribute = Literal["name", "description", "release_name_format", "variable_groups"]
 ReleaseStatus = Literal["active", "abandoned", "draft", "undefined"]
 
 # ========================================================================================================
 # WARNING: THIS FILE IS MAINLY UNTESTED, AND MAY NOT WORK AS EXPECTED
 # FEEL FREE TO MAKE A PR TO FIX/IMPROVE THIS FILE
 # ========================================================================================================
 
 
 def get_release_definition(
-    ado_client: AdoClient, name: str, variable_group_ids: list[int], agent_pool_id: str, revision: str = "1", _id: str = ""
+    ado_client: "AdoClient", name: str, variable_group_ids: list[int], agent_pool_id: str, revision: str = "1", _id: str = ""
 ) -> dict[str, Any]:
     return {
         "name": name,
         "id": _id,
         "variableGroups": variable_group_ids,
         "path": "\\",
         "releaseNameFormat": "Release-$(rev: r)",
@@ -99,55 +101,52 @@
     keep_forever: bool = field(default=False, repr=False)
 
     def __str__(self) -> str:
         return f"{self.name} ({self.release_id}), {self.status}"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Release":
-        created_by = Member(data["createdBy"]["displayName"], data["createdBy"]["uniqueName"], data["createdBy"]["id"])
-        return cls(data["id"], data["name"], data["status"], from_ado_date_string(data["createdOn"]), created_by, data["description"],
+        created_by = Member.from_request_payload(data["createdBy"])
+        return cls(str(data["id"]), data["name"], data["status"], from_ado_date_string(data["createdOn"]), created_by, data["description"],
                    data.get("variables", None), data.get("variableGroups", None), data["keepForever"])  # fmt: skip
 
     @classmethod  # TO-DO: Test
-    def get_by_id(cls, ado_client: AdoClient, release_id: str) -> "Release":
-        return super().get_by_id(
+    def get_by_id(cls, ado_client: "AdoClient", release_id: str) -> "Release":
+        return super().get_by_url(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases/{release_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod  # TO-DO: Test
-    def create(cls, ado_client: AdoClient, definition_id: str, description: str = "Made with the ado_wrapper Python library") -> "Release":  # type: ignore[override]
+    def create(cls, ado_client: "AdoClient", definition_id: str, description: str = "Made with the ado_wrapper Python library") -> "Release":  # type: ignore[override]
         return super().create(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases?api-version=7.1",
             {"definitionId": definition_id, "description": description},
         )  # type: ignore[return-value]
 
     @classmethod  # TO-DO: Test
-    def delete_by_id(cls, ado_client: AdoClient, release_id: str) -> None:  # type: ignore[override]
+    def delete_by_id(cls, ado_client: "AdoClient", release_id: str) -> None:  # type: ignore[override]
         return super().delete_by_id(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases/{release_id}?api-version=7.1",
             release_id,
         )
 
-    # ============ End of requirement set by all state managed resources ================== #
-    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-    # =============== Start of additional methods included with class ===================== #
-
-    def delete(self, ado_client: AdoClient) -> None:
-        self.delete_by_id(ado_client, self.release_id)
-
     @classmethod
-    def get_all(cls, ado_client: AdoClient, definition_id: str) -> "list[Release]":  # type: ignore[override]
+    def get_all(cls, ado_client: "AdoClient", definition_id: str) -> "list[Release]":  # type: ignore[override]
         return super().get_all(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases?api-version=7.1&definitionId={definition_id}",
         )  # type: ignore[return-value]
 
+    # ============ End of requirement set by all state managed resources ================== #
+    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
+    # =============== Start of additional methods included with class ===================== #
+
 
 # ========================================================================================================
 
 
 @dataclass
 class ReleaseDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/release/definitions?view=azure-devops-rest-7.1"""
@@ -177,76 +176,72 @@
     def agent_pool_id(self) -> str:
         if self._agent_pool_id == "1":
             raise ValueError("No agent pool id has been found! Cannot do this operation!")
         return self._agent_pool_id
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "ReleaseDefinition":
-        created_by = Member(data["createdBy"]["displayName"], data["createdBy"]["uniqueName"], data["createdBy"]["id"])
+        created_by = Member.from_request_payload(data["createdBy"])
         return cls(str(data["id"]), data["name"], data.get("description") or "", created_by, from_ado_date_string(data["createdOn"]),
                    data["releaseNameFormat"], data["variableGroups"], data.get("isDeleted", False), data.get("variables", None),
                    data.get("environments", []), data.get("environments", [{"deployPhases": [{"deploymentInput": {"queueId": "1"}}]}]
                             )[0]["deployPhases"][0]["deploymentInput"]["queueId"], data.get("revision", "1"), data)  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, release_definition_id: str) -> "ReleaseDefinition":
-        return super().get_by_id(
+    def get_by_id(cls, ado_client: "AdoClient", release_definition_id: str) -> "ReleaseDefinition":
+        return super().get_by_url(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{release_definition_id}?api-version=7.0",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, variable_group_ids: list[int], agent_pool_id: str) -> "ReleaseDefinition":  # type: ignore[override]
+    def create(cls, ado_client: "AdoClient", name: str, variable_group_ids: list[int], agent_pool_id: str) -> "ReleaseDefinition":  # type: ignore[override]
         """Takes a list of variable group ids to include, and an agent_pool_id"""
         return super().create(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.0",
             get_release_definition(ado_client, name, variable_group_ids, agent_pool_id),
         )  # type: ignore[return-value]
 
     @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, release_definition_id: str) -> None:  # type: ignore[override]
+    def delete_by_id(cls, ado_client: "AdoClient", release_definition_id: str) -> None:  # type: ignore[override]
         for release in ReleaseDefinition.get_all_releases_for_definition(ado_client, release_definition_id):
-            release.delete(ado_client)
+            ado_client.state_manager.remove_resource_from_state("Release", release.release_id)
         return super().delete_by_id(
             ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{release_definition_id}?forceDelete=True&api-version=7.1",
             release_definition_id,
         )
 
-    def update(self, ado_client: AdoClient, attribute_name: ReleaseDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
+    def update(self, ado_client: "AdoClient", attribute_name: ReleaseDefinitionEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
         self.revision = str(int(self.revision) + 1)
         return super().update(
             ado_client, "put",
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions/{self.release_definition_id}?api-version=7.1",
             attribute_name, attribute_value, self._raw_data,  # fmt: skip
         )
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
-    def delete(self, ado_client: AdoClient) -> None:
-        return self.delete_by_id(ado_client, self.release_definition_id)
-
     @classmethod
-    def get_all_releases_for_definition(cls, ado_client: AdoClient, definition_id: str) -> "list[Release]":
+    def get_all_releases_for_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Release]":
         response = requests.get(
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases?api-version=7.1&definitionId={definition_id}",
             auth=ado_client.auth,
         ).json()
         return [Release.from_request_payload(release) for release in response["value"]]
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> "list[ReleaseDefinition]":  # type: ignore[override]
-        response = requests.get(
+    def get_all(cls, ado_client: "AdoClient") -> "list[ReleaseDefinition]":  # type: ignore[override]
+        return super().get_all(
+            ado_client,
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/definitions?api-version=7.1",
-            auth=ado_client.auth,
-        ).json()["value"]
-        return [cls.from_request_payload(data) for data in response]
+        )  # type: ignore[return-value]
 
 
 # ========================================================================================================
 
 # @dataclass
 # class ReleaseEnvironment:
 #     """https://learn.microsoft.com/en-us/rest/api/azure/devops/release/definitions/list?view=azure-devops-rest-7.1&tabs=HTTP#releasedefinitionenvironment"""
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import io
 import zipfile
 from dataclasses import dataclass, field
-from typing import Any, Literal
+from typing import Any, Literal, TYPE_CHECKING
 
 import requests
 
-from ado_wrapper.client import AdoClient
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.utils import ResourceNotFound, UnknownError
 
-# from plan_resources.singletons import plannable_resource
+if TYPE_CHECKING:
+    from ado_wrapper.client import AdoClient
+
 RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
 
 # ====================================================================
 
 
 @dataclass
 class Repo(StateManagedResource):
@@ -36,21 +37,20 @@
     def from_request_payload(cls, data: dict[str, str]) -> "Repo":
         return cls(
             data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
         )
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "Repo":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    # @plannable_resource
     def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> "Repo":  # type: ignore[override]
         repo: Repo = super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
             {"name": name},
         )  # type: ignore[assignment]
         if include_readme:
@@ -62,14 +62,15 @@
             ado_client, "patch",
             f"/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}?api-version=7.1",
             attribute_name, attribute_value, {},  # fmt: skip
         )
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, repo_id: str) -> None:  # type: ignore[override]
+        # TODO: This never checks if it's disabled, so might error
         for pull_request in Repo.get_all_pull_requests(ado_client, repo_id, "all"):
             ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request.pull_request_id)
         return super().delete_by_id(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
             repo_id,
         )
@@ -82,20 +83,19 @@
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo":
+    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo | None":  # type: ignore[return]
         """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
         for repo in cls.get_all(ado_client):
             if repo.name == repo_name:
                 return repo
-        raise ValueError(f"Repo {repo_name} not found")
 
     def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
         request = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
             auth=ado_client.auth,
         )
         if request.status_code == 404:
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/teams.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "Team":
         return cls(data["id"], data["name"], data.get("description", ""), [])
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, team_id: str) -> "Team":
-        resource: Team = super().get_by_id(
+        resource: Team = super().get_by_url(
             ado_client,
             f"/_apis/projects/{ado_client.ado_project}/teams/{team_id}?$expandIdentity={True}&api-version=7.1-preview.1",
         )  # type: ignore[assignment]
         resource.team_members = resource.get_members(ado_client)
         return resource
 
     @classmethod
@@ -59,34 +59,28 @@
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, team_name: str) -> "Team":
-        for team in cls.get_all(ado_client):
-            if team.name == team_name:
-                return team
-        raise ValueError(f"Team {team_name} not found")
+    def get_by_name(cls, ado_client: AdoClient, team_name: str) -> "Team | None":
+        return cls.get_by_abstract_filter(ado_client, lambda team: team.name == team_name)  # type: ignore[return-value, attr-defined]
 
     def get_members(self, ado_client: AdoClient) -> list["TeamMember"]:
         request = requests.get(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/teams/{self.team_id}/members?api-version=7.1-preview.2",
             auth=ado_client.auth,
         ).json()
         if "value" not in request and request.get("message", "").startswith("The team with id "):  # If the team doesn't exist anymore.
             return []
         team_members = [TeamMember.from_request_payload(member) for member in request["value"]]
         self.team_members = team_members
         return team_members
 
-    def delete(self, ado_client: AdoClient, team_id: str) -> None:
-        self.delete_by_id(ado_client, team_id)
-
     # @staticmethod
     # def _recursively_extract_teams(ado_client: AdoClient, team_or_member: Team | TeamMember):
     #     if isinstance(team_or_member, Team):
     #         rint("Found a team!")
     #         team_or_member.get_members(ado_client)
     #         for member in team_or_member.team_members:
     #             Team._recursively_extract_teams(ado_client, member)
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from typing import Literal, Any, TYPE_CHECKING
 from dataclasses import dataclass, field
 
-import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 VOTE_ID_TO_TYPE = {
     10: "approved",
@@ -43,15 +41,15 @@
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> "AdoUser":
         return cls(data["descriptor"], data["displayName"], data["mailAddress"].removeprefix("vstfs:///Classification/TeamProject/"),
                    data["origin"], data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> "AdoUser":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "AdoUser":  # type: ignore[override]
         raise NotImplementedError("Creating a new user is not supported")
@@ -69,28 +67,22 @@
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_email(cls, ado_client: AdoClient, member_email: str) -> "AdoUser":
-        for member in cls.get_all(ado_client):
-            if member.email == member_email:
-                return member
-        raise ValueError(f"Member with email {member_email} not found")
+        user: AdoUser = cls.get_by_abstract_filter(ado_client, lambda user: user.email == member_email)  # type: ignore[attr-defined, assignment]
+        if not user:
+            raise ValueError(f"Member with email {member_email} not found")
+        return user
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, member_name: str) -> "AdoUser":
-        for member in cls.get_all(ado_client):
-            if member.display_name == member_name:
-                return member
-        raise ValueError(f"Member with name {member_name} not found")
-
-    def delete(self, ado_client: AdoClient) -> None:
-        self.delete_by_id(ado_client, self.descriptor_id)
+    def get_by_name(cls, ado_client: AdoClient, member_name: str) -> "AdoUser | None":
+        return cls.get_by_abstract_filter(ado_client, lambda user: user.display_name == member_name)  # type: ignore[return-value, attr-defined]
 
 
 # ======================================================================================================= #
 # ------------------------------------------------------------------------------------------------------- #
 # ======================================================================================================= #
 
 
@@ -103,15 +95,18 @@
     member_id: str  # Static
 
     def __str__(self) -> str:
         return f"{self.name} ({self.email})"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Member":
-        return cls(data["displayName"], data["mailAddress"], data["originId"])
+        # displayName, uniqueName/mailAddress, id/originId
+        # This gets returned slightly differently from different APIs
+        return cls(data["displayName"], data.get("uniqueName") or data.get("mailAddress", "UNKNOWN"),  # type: ignore[arg-type]
+                   data.get("id") or data["originId"])  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, member_id: str) -> "Member":
         raise NotImplementedError("Getting a member by ID is not supported")
 
     @classmethod
     def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "Member":  # type: ignore[override]
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.5/ado_wrapper/resources/variable_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     modified_on: datetime | None = None
 
     def __str__(self) -> str:
         return repr(self)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "VariableGroup":
-        created_by = Member(data["createdBy"]["displayName"], "UNKNOWN", data["createdBy"]["id"])
-        modified_by = Member(data["modifiedBy"]["displayName"], "UNKNOWN", data["modifiedBy"]["id"])
+        created_by = Member.from_request_payload(data["createdBy"])
+        modified_by = Member.from_request_payload(data["modifiedBy"])
         return cls(str(data["id"]), data["name"], data.get("description", ""),
                    {key: value["value"] if isinstance(value, dict) else value for key, value in data["variables"].items()},
                    from_ado_date_string(data["createdOn"]), created_by, modified_by, from_ado_date_string(data.get("modifiedOn")))  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, variable_group_id: str) -> "VariableGroup":
-        return super().get_by_id(
+        return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups/{variable_group_id}?api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def create(  # type: ignore[override]
         cls, ado_client: AdoClient, variable_group_name: str, variable_group_description: str, variables: dict[str, str]  # fmt: skip
@@ -95,16 +95,10 @@
             f"/{ado_client.ado_project}/_apis/distributedtask/variablegroups?api-version=7.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
-    def delete(self, ado_client: AdoClient) -> None:
-        self.delete_by_id(ado_client, self.variable_group_id)
-
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, name: str) -> "VariableGroup | None":
-        for variable_group in cls.get_all(ado_client):
-            if variable_group.name == name:
-                return variable_group
-        return None
+        return cls.get_by_abstract_filter(ado_client, lambda variable_group: variable_group.name == name)  # type: ignore[return-value, attr-defined]
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.5/ado_wrapper/state_managed_abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Any, TYPE_CHECKING, Literal
+from typing import Any, TYPE_CHECKING, Literal, Callable
 from dataclasses import dataclass, fields
 from datetime import datetime
 
 import requests
 
 from ado_wrapper.utils import (
     get_resource_variables, extract_id, get_internal_field_names,
     ResourceAlreadyExists, DeletionFailed, ResourceNotFound, UpdateFailed,  # fmt: skip
 )
+from ado_wrapper.plan_resources.plan_resource import PlannedStateManagedResource
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
 def recursively_convert_to_json(attribute_name: str, attribute_value: Any) -> tuple[str, Any]:
     if isinstance(attribute_value, dict):
@@ -53,31 +54,39 @@
     def from_json(cls, data: dict[str, Any]) -> "StateManagedResource":
         return cls(**recursively_convert_from_json(data))
 
     def to_json(self) -> dict[str, Any]:
         attribute_names = [field_obj.name for field_obj in fields(self)]
         attribute_values = [getattr(self, field_obj.name) for field_obj in fields(self)]
         combined = zip(attribute_names, attribute_values)
-        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined) ####
+        return dict(recursively_convert_to_json(attribute_name, attribute_value) for attribute_name, attribute_value in combined)  ####
 
     @classmethod
-    def get_by_id(cls, ado_client: "AdoClient", url: str) -> "StateManagedResource":
+    def get_by_id(cls, ado_client: "AdoClient", resource_id: str) -> "StateManagedResource":
+        raise NotImplementedError
+
+    @classmethod
+    def get_by_url(cls, ado_client: "AdoClient", url: str) -> "StateManagedResource":
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = requests.get(url, auth=ado_client.auth)
         if request.status_code == 404:
             raise ResourceNotFound(f"No {cls.__name__} found with that identifier!")
         if request.status_code >= 300:
             raise ValueError(f"Error getting {cls.__name__} by id: {request.text}")
         if "value" in request.json():
             return cls.from_request_payload(request.json()["value"][0])
         return cls.from_request_payload(request.json())
 
     @classmethod
-    def create(cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None) -> "StateManagedResource":
+    def create(
+        cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None
+    ) -> "StateManagedResource | PlannedStateManagedResource":
+        if ado_client.plan_mode:
+            return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = requests.post(url, json=payload or {}, auth=ado_client.auth)  # Create a brand new dict
         if request.status_code == 401:
             raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
         if request.status_code == 409:
             raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
@@ -94,27 +103,31 @@
         if request.status_code != 204:
             if request.status_code == 404:
                 print("[ADO_WRAPPER] Resource not found, probably already deleted, removing from state")
             else:
                 raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
         ado_client.state_manager.remove_resource_from_state(cls.__name__, resource_id)  # type: ignore[arg-type]
 
+    def delete(self, ado_client: "AdoClient") -> None:
+        return self.delete_by_id(ado_client, extract_id(self))  # type: ignore[call-arg]
+
     def update(self, ado_client: "AdoClient", update_action: Literal["put", "patch"], url: str,  # pylint: disable=too-many-arguments
                attribute_name: str, attribute_value: Any, params: dict[str, Any]) -> None:  # fmt: skip
         """The params should be a dictionary which will be combined with the internal name and value of the attribute to be updated."""
         interal_names = get_internal_field_names(self.__class__)
         if attribute_name not in get_internal_field_names(self.__class__):
             raise ValueError(f"The attribute `{attribute_name}` is not editable!  Editable attributes are: {list(interal_names.keys())}")
         params |= {interal_names[attribute_name]: attribute_value}
 
-        func = requests.put if update_action == "put" else requests.patch
-        # request = requests.request(update_action, url, json=params, auth=ado_client.auth)
+        if ado_client.plan_mode:
+            return PlannedStateManagedResource.update(self, ado_client, url, attribute_name, attribute_value, params)
+
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
-        request = func(url, json=params, auth=ado_client.auth)
+        request = requests.request(update_action, url, json=params, auth=ado_client.auth)
         if request.status_code != 200:
             raise UpdateFailed(
                 f"Failed to update {self.__class__.__name__} with id {extract_id(self)} and attribute {attribute_name} to {attribute_value}. \nReason:\n{request.text}"
             )
         setattr(self, attribute_name, attribute_value)
         ado_client.state_manager.update_resource_in_state(self.__class__.__name__, extract_id(self), self.to_json())  # type: ignore[arg-type]
 
@@ -122,7 +135,22 @@
     def get_all(cls, ado_client: "AdoClient", url: str) -> list["StateManagedResource"]:
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
         request = requests.get(url, auth=ado_client.auth)
         if request.status_code >= 300:
             raise ValueError(f"Error getting all {cls.__name__}: {request.text}")
         return [cls.from_request_payload(resource) for resource in request.json()["value"]]
+
+    @classmethod
+    def get_by_abstract_filter(
+        cls, ado_client: "AdoClient", func: Callable[["StateManagedResource"], bool]
+    ) -> "StateManagedResource | None":
+        """Used internally for getting resources by a filter function. The function should return True if the resource is the one you want."""
+        resources = cls.get_all(ado_client)  # type: ignore[call-arg]
+        for resource in resources:
+            if func(resource):
+                return resource
+        return None
+
+    def set_lifecycle_policy(self, ado_client: "AdoClient", policy: Literal["prevent_destroy", "ignore_changes"]) -> None:
+        self.life_cycle_policy = policy  # TODO
+        ado_client.state_manager.update_lifecycle_policy(self.__class__.__name__, extract_id(self), policy)  # type: ignore[arg-type]
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.5/ado_wrapper/state_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 import json
 from pathlib import Path
 from datetime import datetime
 from uuid import uuid4
-from typing import Any, TypedDict, TYPE_CHECKING  # , Generator
+from typing import Any, TypedDict, TYPE_CHECKING, Literal
 
 from ado_wrapper.utils import DeletionFailed, get_resource_variables, ResourceType
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 STATE_FILE_VERSION = "1.4"
 
 
 class StateFileType(TypedDict):
     state_file_version: str
     resources: dict[ResourceType, dict[str, Any]]
 
 
+EMPTY_STATE: StateFileType = {
+    "state_file_version": STATE_FILE_VERSION,
+    "resources": {resource: {} for resource in get_resource_variables().keys()},  # type: ignore[misc]
+}
+
+
 class StateManager:
     def __init__(self, ado_client: "AdoClient", state_file_name: str | None = "main.state") -> None:
         self.ado_client = ado_client
         self.state_file_name = state_file_name
         self.run_id = str(uuid4())
 
         # If they have a state file name input, but the file doesn't exist:
         if self.state_file_name is not None and not Path(self.state_file_name).exists():
             self.wipe_state()  # Will automatically create the file
 
+        self.state: StateFileType = self.load_state() if self.state_file_name is not None else EMPTY_STATE
+
     def load_state(self) -> StateFileType:
-        assert self.state_file_name is not None
+        if self.state_file_name is None:
+            return self.state
         with open(self.state_file_name, "r", encoding="utf-8") as state_file:
             try:
                 return json.load(state_file)  # type: ignore[no-any-return]
             except json.JSONDecodeError as exc:
                 raise json.JSONDecodeError("State file is not valid JSON, it might have been corrupted?", exc.doc, exc.pos)
 
     def write_state_file(self, state_data: StateFileType) -> None:
-        assert self.state_file_name is not None
+        if self.state_file_name is None:
+            self.state = state_data
+            return
         with open(self.state_file_name, "w", encoding="utf-8") as state_file:
             json.dump(state_data, state_file, indent=4)
 
     # =======================================================================================================
 
     def add_resource_to_state(self, resource_type: ResourceType, resource_id: str, resource_data: dict[str, Any]) -> None:
-        if self.state_file_name is None:
-            print("[ADO_WRAPPER] Not storing state, so not adding resource to state")
-            return None
         all_states = self.load_state()
         if resource_id in all_states["resources"][resource_type]:
             self.remove_resource_from_state(resource_type, resource_id)
         metadata = {"created_datetime": datetime.now().isoformat(), "run_id": self.run_id}
-        all_data = {resource_id: {"data": resource_data, "metadata": metadata, "lifecycle-policies": {}}}
+        all_data = {resource_id: {"data": resource_data, "metadata": metadata, "lifecycle-policy": {}}}
         all_states["resources"][resource_type] |= all_data
         return self.write_state_file(all_states)
 
     def remove_resource_from_state(self, resource_type: ResourceType, resource_id: str) -> None:
-        if self.state_file_name is None:
-            print("[ADO_WRAPPER] Not storing state, so not removing resource to state")
-            return None
         all_states = self.load_state()
         all_states["resources"][resource_type] = {k: v for k, v in all_states["resources"][resource_type].items() if k != resource_id}
         return self.write_state_file(all_states)
 
     def update_resource_in_state(self, resource_type: ResourceType, resource_id: str, updated_data: dict[str, Any]) -> None:
-        if self.state_file_name is None:
-            print("[ADO_WRAPPER] Not storing state, so not updating resource in state")
-            return None
         all_states = self.load_state()
         all_states["resources"][resource_type][resource_id]["data"] = updated_data
         all_states["resources"][resource_type][resource_id]["metadata"]["updated_datetime"] = datetime.now().isoformat()
         return self.write_state_file(all_states)
 
+    def update_lifecycle_policy(self, resource_type: ResourceType, resource_id: str,
+                                policy: Literal["prevent_destroy", "ignore_changes"]) -> None:  # fmt: skip
+        all_states = self.load_state()
+        all_states["resources"][resource_type][resource_id]["lifecycle-policy"] = policy
+        return self.write_state_file(all_states)
     # =======================================================================================================
 
     def delete_resource(self, resource_type: ResourceType, resource_id: str) -> None:
         all_resource_classes = get_resource_variables()
         class_reference = all_resource_classes[resource_type]
         try:
             class_reference.delete_by_id(self.ado_client, resource_id)  # type: ignore[call-arg]
         except DeletionFailed as exc:
             print(str(exc))
         except (NotImplementedError, TypeError):
-            print(f"[ADO_WRAPPER] Cannot {resource_type} {resource_id} from state or real space, please delete this manually or using code.")
+            print(
+                f"[ADO_WRAPPER] Cannot {resource_type} {resource_id} from state or real space, please delete this manually or using code."
+            )
         else:
             print(f"[ADO_WRAPPER] Deleted {resource_type} {resource_id} from ADO")
             self.remove_resource_from_state(resource_type, resource_id)
 
     def delete_all_resources(self, resource_type_filter: ResourceType | None = None) -> None:
         all_resources = (
             self.load_state()["resources"]
@@ -102,41 +111,32 @@
     def import_into_state(self, resource_type: ResourceType, resource_id: str) -> None:
         class_reference = get_resource_variables()[resource_type]
         data = class_reference.get_by_id(self.ado_client, resource_id).to_json()
         self.add_resource_to_state(resource_type, resource_id, data)
 
     def wipe_state(self) -> None:
         if self.state_file_name is None:
+            self.state = EMPTY_STATE
             return
         with open(self.state_file_name, "w", encoding="utf-8") as state_file:
-            json.dump(
-                {
-                    "state_file_version": STATE_FILE_VERSION,
-                    "resources": {resource: {} for resource in get_resource_variables().keys()},
-                },
-                state_file,
-                indent=4,
-            )
+            json.dump(EMPTY_STATE, state_file, indent=4)
 
     def generate_in_memory_state(self) -> StateFileType:
+        """This method goes through every resource in state and updates it to the latest version in real world space"""
         ALL_RESOURCES = get_resource_variables()
-        # """This method goes through every resource in state and updates it to the latest version in real world space"""
         all_states = self.load_state()
         for resource_type in all_states["resources"]:
             for resource_id in all_states["resources"][resource_type]:
                 instance = ALL_RESOURCES[resource_type].get_by_id(self.ado_client, resource_id)
                 if instance.to_json() != all_states["resources"][resource_type][resource_id]["data"]:
                     all_states["resources"][resource_type][resource_id]["data"] = instance.to_json()
         return all_states
 
     def load_all_resources_with_prefix_into_state(self, prefix: str) -> None:
-        from ado_wrapper.resources.variable_groups import VariableGroup
-        from ado_wrapper.resources.repo import Repo
-        from ado_wrapper.resources.releases import ReleaseDefinition
-        from ado_wrapper.resources.builds import BuildDefinition
+        from ado_wrapper.resources import VariableGroup, Repo, ReleaseDefinition, BuildDefinition, ServiceEndpoint  # type: ignore[attr-defined]
 
         for repo in Repo.get_all(self.ado_client):
             if repo.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("Repo", repo.repo_id)
 
         for variable_group in VariableGroup.get_all(self.ado_client):
             if variable_group.name.startswith(prefix):
@@ -146,12 +146,16 @@
             if release_definition.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("ReleaseDefinition", release_definition.release_definition_id)
 
         for build_definition in BuildDefinition.get_all(self.ado_client):
             if build_definition.name.startswith(prefix):
                 self.ado_client.state_manager.import_into_state("BuildDefinition", build_definition.build_definition_id)
 
+        for service_endpoint in ServiceEndpoint.get_all(self.ado_client):
+            if service_endpoint.name.startswith(prefix):
+                self.ado_client.state_manager.import_into_state("ServiceEndpoint", service_endpoint.service_endpoint_id)
+
     # Unused
     # def all_resources(self) -> Generator[tuple[ResourceType, str], None, None]:
     #     for resource_type in self.load_state()["resources"]:
     #         for resource_id in self.load_state()["resources"][resource_type]:
     #             yield resource_type, resource_id
```

### Comparing `ado_wrapper-0.0.4/ado_wrapper/utils.py` & `ado_wrapper-0.0.5/ado_wrapper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timezone
-from typing import overload, TYPE_CHECKING, Any, Literal
+from typing import overload, TYPE_CHECKING, Literal
 from dataclasses import fields
 
 if TYPE_CHECKING:
     from ado_wrapper.state_managed_abc import StateManagedResource
 
 ResourceType = Literal[
     "Branch", "Build", "BuildDefinition", "Commit", "Project", "PullRequest", "Release", "ReleaseDefinition",
@@ -72,18 +72,18 @@
     for field_name, metadata in get_fields_metadata(cls).items():
         if metadata.get("is_id_field", False):
             # if field_name.endswith("_id"):
             return field_name
     raise ValueError(f"No id field found for {cls.__name__}!")
 
 
-def extract_id(obj: "StateManagedResource") -> Any:
+def extract_id(obj: "StateManagedResource") -> str:
     """Extracts the id from a StateManagedResource object. The id field is defined by the "is_id_field" metadata."""
     id_field_name = get_id_field_name(obj.__class__)
-    return getattr(obj, id_field_name)
+    return getattr(obj, id_field_name)  # type: ignore[no-any-return]
 
 
 def get_editable_fields(cls: type["StateManagedResource"]) -> list[str]:
     """Returns a list of attribute that are marked as editable."""
     return [field_obj.name for field_obj in cls.__dataclass_fields__.values() if field_obj.metadata.get("editable", False)]
 
 
@@ -116,14 +116,15 @@
 class InvalidPermissionsError(Exception):
     pass
 
 
 class UpdateFailed(Exception):
     pass
 
+
 class AuthenticationError(Exception):
     pass
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
```

### Comparing `ado_wrapper-0.0.4/pyproject.toml` & `ado_wrapper-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.4"
+version = "0.0.5"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -45,24 +45,28 @@
     "missing-function-docstring",
     "missing-timeout",
 
     "too-few-public-methods",
     "too-many-instance-attributes",
     "too-many-arguments",
 
+    "fixme",
     "arguments-differ",
     "arguments-renamed",
     "invalid-name",
     "too-many-locals",
     "line-too-long",
     "broad-exception-caught",
     "import-outside-toplevel",
     "attribute-defined-outside-init",
     "cyclic-import",
     "redefined-outer-name",
+    "abstract-method",
+    "pointless-statement",
+    "inconsistent-return-statements",
 ]
 
 [tool.pytest.ini_options]
 log_cli = true
 markers = [
     "wip: mark test as a work in progress",
     "from_request_payload: mark test which convert payloads to resources",
```

### Comparing `ado_wrapper-0.0.4/PKG-INFO` & `ado_wrapper-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -19,7 +19,9 @@
 It is essentially a wrapper for the (horrible to work with) ADO API, and supports OOP principals.
 
 Any resource can be fetched by calling the `<resource>.get_by_id()` function.
 
 It also includes a solution for managing resources created by this script, which is extremely useful for testing the creation of random resources.
 To delete all resources created by this, run the main module with the "--delete-everything" flag.
 
+If you're reading this readme not from the code, here's a link to the [github repo](https://github.com/UP929312/ado-wrapper)
+
```

