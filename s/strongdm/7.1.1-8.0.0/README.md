# Comparing `tmp/strongdm-7.1.1.zip` & `tmp/strongdm-8.0.0.zip`

## zipinfo {}

```diff
@@ -1,132 +1,132 @@
-Zip file size: 375388 bytes, number of entries: 130
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 15:58 strongdm-7.1.1/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-26 15:58 strongdm-7.1.1/strongdm/
--rw-r--r--  2.0 unx     1908 b- defN 24-Mar-26 15:58 strongdm-7.1.1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-26 15:58 strongdm-7.1.1/setup.cfg
--rw-r--r--  2.0 unx     3599 b- defN 24-Mar-26 15:58 strongdm-7.1.1/PKG-INFO
--rw-r--r--  2.0 unx     2875 b- defN 24-Mar-26 15:58 strongdm-7.1.1/README.md
--rw-r--r--  2.0 unx    11342 b- defN 24-Mar-26 15:58 strongdm-7.1.1/LICENSE
--rw-r--r--  2.0 unx       50 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/requires.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     4399 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     3599 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx    17034 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/organization_history_pb2.py
--rw-r--r--  2.0 unx    27020 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/client.py
--rw-r--r--  2.0 unx    16079 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_roles_pb2.py
--rw-r--r--  2.0 unx    20122 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflows_pb2.py
--rw-r--r--  2.0 unx     8808 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     6598 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/control_panel_pb2_grpc.py
--rw-r--r--  2.0 unx    15297 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_groups_pb2.py
--rw-r--r--  2.0 unx     6176 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identity_groups_pb2_grpc.py
--rw-r--r--  2.0 unx    16380 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_nodes_pb2.py
--rw-r--r--  2.0 unx     8646 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_requests_history_pb2.py
--rw-r--r--  2.0 unx     8650 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identities_history_pb2.py
--rw-r--r--  2.0 unx    16423 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_peers_pb2.py
--rw-r--r--  2.0 unx     9113 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2.py
--rw-r--r--  2.0 unx    15880 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/spec_pb2.py
--rw-r--r--  2.0 unx     7818 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/roles_history_pb2.py
--rw-r--r--  2.0 unx    16584 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_grants_pb2.py
--rw-r--r--  2.0 unx    75244 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_store_types_pb2.py
--rw-r--r--  2.0 unx     7476 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/role_resources_pb2.py
--rw-r--r--  2.0 unx     3295 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/role_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     5092 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/activities_pb2_grpc.py
--rw-r--r--  2.0 unx    27332 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/accounts_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/options_pb2_grpc.py
--rw-r--r--  2.0 unx     9837 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     9665 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     8550 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_grants_history_pb2.py
--rw-r--r--  2.0 unx    17204 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_approvers_pb2.py
--rw-r--r--  2.0 unx    18708 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2.py
--rw-r--r--  2.0 unx     3223 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3561 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_assignments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3470 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_permissions_pb2_grpc.py
--rw-r--r--  2.0 unx     9027 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2.py
--rw-r--r--  2.0 unx     8140 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflows_history_pb2.py
--rw-r--r--  2.0 unx     8708 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx     8773 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_resources_history_pb2.py
--rw-r--r--  2.0 unx     7818 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/nodes_history_pb2.py
--rw-r--r--  2.0 unx     8396 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_permissions_pb2.py
--rw-r--r--  2.0 unx     7932 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_groups_pb2_grpc.py
--rw-r--r--  2.0 unx     8546 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     4600 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/tags_pb2.py
--rw-r--r--  2.0 unx     3561 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3353 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_grants_history_pb2_grpc.py
--rw-r--r--  2.0 unx    17070 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_steps_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/drivers_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/tags_pb2_grpc.py
--rw-r--r--  2.0 unx    20009 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflows_pb2.py
--rw-r--r--  2.0 unx     8132 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/resources_history_pb2.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_attachments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8412 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_stores_history_pb2.py
--rw-r--r--  2.0 unx    17173 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_resources_pb2.py
--rw-r--r--  2.0 unx     3557 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_request_events_history_pb2_grpc.py
--rw-r--r--  2.0 unx    19200 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/queries_pb2.py
--rw-r--r--  2.0 unx      808 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/__init__.py
--rw-r--r--  2.0 unx     3417 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_requests_history_pb2_grpc.py
--rw-r--r--  2.0 unx    12455 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/resources_pb2_grpc.py
--rw-r--r--  2.0 unx     6849 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_store_healths_pb2_grpc.py
--rw-r--r--  2.0 unx   784386 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/models.py
--rw-r--r--  2.0 unx   893989 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/drivers_pb2.py
--rw-r--r--  2.0 unx    29937 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/nodes_pb2.py
--rw-r--r--  2.0 unx     8961 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_assignments_history_pb2.py
--rw-r--r--  2.0 unx     9042 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/roles_pb2_grpc.py
--rw-r--r--  2.0 unx     3350 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/role_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx    14899 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/options_pb2.py
--rw-r--r--  2.0 unx     7340 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_assignments_pb2.py
--rw-r--r--  2.0 unx     3180 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_requests_pb2_grpc.py
--rw-r--r--  2.0 unx     3322 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_stores_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3505 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     9376 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_stores_pb2_grpc.py
--rw-r--r--  2.0 unx     8102 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_attachments_pb2_grpc.py
--rw-r--r--  2.0 unx     8983 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_request_events_history_pb2.py
--rw-r--r--  2.0 unx     9494 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/accounts_pb2_grpc.py
--rw-r--r--  2.0 unx     9971 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identity_groups_pb2.py
--rw-r--r--  2.0 unx     3420 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/queries_pb2_grpc.py
--rw-r--r--  2.0 unx     3424 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identities_history_pb2_grpc.py
--rw-r--r--  2.0 unx    15576 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/access_requests_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_store_types_pb2_grpc.py
--rw-r--r--  2.0 unx     3479 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_assignments_pb2_grpc.py
--rw-r--r--  2.0 unx     3434 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx   431899 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/plumbing.py
--rw-r--r--  2.0 unx     3198 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/accounts_history_pb2_grpc.py
--rw-r--r--  2.0 unx    11611 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/control_panel_pb2.py
--rw-r--r--  2.0 unx     8138 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/accounts_history_pb2.py
--rw-r--r--  2.0 unx     3390 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3465 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx    18385 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/roles_pb2.py
--rw-r--r--  2.0 unx    17214 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_stores_pb2.py
--rw-r--r--  2.0 unx    17037 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_attachments_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/nodes_history_pb2_grpc.py
--rw-r--r--  2.0 unx    19858 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identities_pb2.py
--rw-r--r--  2.0 unx     8255 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     8167 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/peering_group_peers_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_resources_pb2.py
--rw-r--r--  2.0 unx     8506 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_roles_history_pb2.py
--rw-r--r--  2.0 unx     3592 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3704 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx    16005 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/secret_store_healths_pb2.py
--rw-r--r--  2.0 unx    16300 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/activities_pb2.py
--rw-r--r--  2.0 unx     8478 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/role_resources_history_pb2.py
--rw-r--r--  2.0 unx     9960 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     2196 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/errors.py
--rw-r--r--  2.0 unx   202595 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/svc.py
--rw-r--r--  2.0 unx      741 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/spec_pb2_grpc.py
--rw-r--r--  2.0 unx     3361 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/replays_pb2_grpc.py
--rw-r--r--  2.0 unx     3388 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/organization_history_pb2_grpc.py
--rwxr-xr-x  2.0 unx    18511 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/constants.py
--rw-r--r--  2.0 unx    22207 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/resources_pb2.py
--rw-r--r--  2.0 unx     8792 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflows_history_pb2.py
--rw-r--r--  2.0 unx     8320 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/replays_pb2.py
--rw-r--r--  2.0 unx     9790 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/remote_identities_pb2_grpc.py
--rw-r--r--  2.0 unx     8901 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_attachments_history_pb2.py
--rw-r--r--  2.0 unx     7980 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/account_grants_pb2_grpc.py
--rw-r--r--  2.0 unx     8071 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_roles_pb2_grpc.py
--rw-r--r--  2.0 unx     3259 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8404 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_steps_pb2_grpc.py
--rw-r--r--  2.0 unx     9416 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8165 b- defN 24-Mar-26 15:58 strongdm-7.1.1/strongdm/workflow_approvers_pb2_grpc.py
-130 files, 3446370 bytes uncompressed, 352948 bytes compressed:  89.8%
+Zip file size: 376498 bytes, number of entries: 130
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/strongdm/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/
+-rw-r--r--  2.0 unx     2875 b- defN 24-Apr-09 19:46 strongdm-8.0.0/README.md
+-rw-r--r--  2.0 unx    11342 b- defN 24-Apr-09 19:46 strongdm-8.0.0/LICENSE
+-rw-r--r--  2.0 unx     1908 b- defN 24-Apr-09 19:47 strongdm-8.0.0/setup.py
+-rw-r--r--  2.0 unx     3599 b- defN 24-Apr-09 19:47 strongdm-8.0.0/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-09 19:47 strongdm-8.0.0/setup.cfg
+-rw-r--r--  2.0 unx     8792 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py
+-rw-r--r--  2.0 unx     3361 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/replays_pb2_grpc.py
+-rw-r--r--  2.0 unx     5092 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/activities_pb2_grpc.py
+-rw-r--r--  2.0 unx    29219 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/accounts_pb2.py
+-rw-r--r--  2.0 unx     7476 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_pb2.py
+-rw-r--r--  2.0 unx    17204 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx     6849 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py
+-rw-r--r--  2.0 unx      808 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/__init__.py
+-rw-r--r--  2.0 unx     3424 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3505 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_pb2.py
+-rw-r--r--  2.0 unx    18385 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_pb2.py
+-rw-r--r--  2.0 unx     9416 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/options_pb2_grpc.py
+-rw-r--r--  2.0 unx   433936 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/plumbing.py
+-rw-r--r--  2.0 unx    12455 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/spec_pb2_grpc.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/queries_pb2_grpc.py
+-rw-r--r--  2.0 unx     7932 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8550 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_history_pb2.py
+-rw-r--r--  2.0 unx    17034 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/organization_history_pb2.py
+-rw-r--r--  2.0 unx     8412 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_history_pb2.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     6176 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx    17214 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_pb2.py
+-rw-r--r--  2.0 unx     3479 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py
+-rw-r--r--  2.0 unx     8773 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_history_pb2.py
+-rw-r--r--  2.0 unx    27237 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/client.py
+-rw-r--r--  2.0 unx    16423 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_peers_pb2.py
+-rw-r--r--  2.0 unx     8708 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx     9790 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/drivers_pb2_grpc.py
+-rw-r--r--  2.0 unx     3470 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py
+-rw-r--r--  2.0 unx     8983 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_request_events_history_pb2.py
+-rw-r--r--  2.0 unx    29937 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_pb2.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx   893989 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/drivers_pb2.py
+-rw-r--r--  2.0 unx    16584 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_pb2.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    15576 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_pb2.py
+-rw-r--r--  2.0 unx     9837 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     9376 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py
+-rw-r--r--  2.0 unx     3295 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    17173 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_resources_pb2.py
+-rw-r--r--  2.0 unx     8102 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py
+-rw-r--r--  2.0 unx     8478 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_history_pb2.py
+-rw-r--r--  2.0 unx     8167 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py
+-rw-r--r--  2.0 unx     9665 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     8646 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_history_pb2.py
+-rw-r--r--  2.0 unx     8961 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     6598 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py
+-rw-r--r--  2.0 unx     3198 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3465 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3390 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3417 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    16079 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_pb2.py
+-rw-r--r--  2.0 unx     4600 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/tags_pb2.py
+-rw-r--r--  2.0 unx     8650 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_history_pb2.py
+-rw-r--r--  2.0 unx     8320 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/replays_pb2.py
+-rw-r--r--  2.0 unx    16300 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/activities_pb2.py
+-rw-r--r--  2.0 unx     7340 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_pb2.py
+-rw-r--r--  2.0 unx     3353 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py
+-rw-r--r--  2.0 unx   202826 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/svc.py
+-rw-r--r--  2.0 unx     3592 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+-rwxr-xr-x  2.0 unx    18511 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/constants.py
+-rw-r--r--  2.0 unx     8255 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     9027 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/tags_pb2_grpc.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    15297 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_groups_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py
+-rw-r--r--  2.0 unx     7980 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py
+-rw-r--r--  2.0 unx    20122 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_pb2.py
+-rw-r--r--  2.0 unx     8404 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py
+-rw-r--r--  2.0 unx    17037 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_pb2.py
+-rw-r--r--  2.0 unx     3350 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    19200 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/queries_pb2.py
+-rw-r--r--  2.0 unx    14899 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/options_pb2.py
+-rw-r--r--  2.0 unx    17070 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py
+-rw-r--r--  2.0 unx    18708 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx     9758 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/accounts_pb2_grpc.py
+-rw-r--r--  2.0 unx     8546 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_attachments_history_pb2.py
+-rw-r--r--  2.0 unx    75244 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_types_pb2.py
+-rw-r--r--  2.0 unx     8396 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_permissions_pb2.py
+-rw-r--r--  2.0 unx     3434 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    15880 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/spec_pb2.py
+-rw-r--r--  2.0 unx     2196 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/errors.py
+-rw-r--r--  2.0 unx     3704 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8506 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py
+-rw-r--r--  2.0 unx    22207 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_pb2.py
+-rw-r--r--  2.0 unx    11611 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/control_panel_pb2.py
+-rw-r--r--  2.0 unx   788329 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm/models.py
+-rw-r--r--  2.0 unx    16005 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/secret_store_healths_pb2.py
+-rw-r--r--  2.0 unx     8138 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/accounts_history_pb2.py
+-rw-r--r--  2.0 unx     9042 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_pb2_grpc.py
+-rw-r--r--  2.0 unx     8140 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflows_history_pb2.py
+-rw-r--r--  2.0 unx    20009 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflows_pb2.py
+-rw-r--r--  2.0 unx    16380 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9113 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py
+-rw-r--r--  2.0 unx     8165 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx    19858 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identities_pb2.py
+-rw-r--r--  2.0 unx     8808 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     8132 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/resources_history_pb2.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/roles_history_pb2.py
+-rw-r--r--  2.0 unx     9971 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-Apr-09 19:46 strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py
+-rw-r--r--  2.0 unx       50 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/requires.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3599 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     4399 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-09 19:47 strongdm-8.0.0/strongdm.egg-info/dependency_links.txt
+130 files, 3454949 bytes uncompressed, 354058 bytes compressed:  89.8%
```

## zipnote {}

```diff
@@ -1,391 +1,391 @@
-Filename: strongdm-7.1.1/
+Filename: strongdm-8.0.0/
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/
+Filename: strongdm-8.0.0/strongdm/
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/
+Filename: strongdm-8.0.0/strongdm.egg-info/
 Comment: 
 
-Filename: strongdm-7.1.1/setup.py
+Filename: strongdm-8.0.0/README.md
 Comment: 
 
-Filename: strongdm-7.1.1/setup.cfg
+Filename: strongdm-8.0.0/LICENSE
 Comment: 
 
-Filename: strongdm-7.1.1/PKG-INFO
+Filename: strongdm-8.0.0/setup.py
 Comment: 
 
-Filename: strongdm-7.1.1/README.md
+Filename: strongdm-8.0.0/PKG-INFO
 Comment: 
 
-Filename: strongdm-7.1.1/LICENSE
+Filename: strongdm-8.0.0/setup.cfg
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/requires.txt
+Filename: strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/top_level.txt
+Filename: strongdm-8.0.0/strongdm/replays_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/SOURCES.txt
+Filename: strongdm-8.0.0/strongdm/activities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/dependency_links.txt
+Filename: strongdm-8.0.0/strongdm/accounts_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm.egg-info/PKG-INFO
+Filename: strongdm-8.0.0/strongdm/role_resources_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/organization_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/client.py
+Filename: strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_roles_pb2.py
+Filename: strongdm-8.0.0/strongdm/__init__.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflows_pb2.py
+Filename: strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_approvers_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/control_panel_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_resources_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_groups_pb2.py
+Filename: strongdm-8.0.0/strongdm/roles_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identity_groups_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_nodes_pb2.py
+Filename: strongdm-8.0.0/strongdm/options_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_requests_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/plumbing.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identities_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_peers_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/nodes_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/spec_pb2.py
+Filename: strongdm-8.0.0/strongdm/spec_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/roles_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_grants_pb2.py
+Filename: strongdm-8.0.0/strongdm/queries_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_store_types_pb2.py
+Filename: strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/role_resources_pb2.py
+Filename: strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/role_resources_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_grants_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/activities_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/organization_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/accounts_pb2.py
+Filename: strongdm-8.0.0/strongdm/secret_stores_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/options_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/nodes_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflows_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/secret_stores_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_grants_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_approvers_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2.py
+Filename: strongdm-8.0.0/strongdm/client.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/resources_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/peering_group_peers_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_assignments_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_permissions_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/drivers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflows_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/access_request_events_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_resources_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/nodes_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/nodes_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_permissions_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_groups_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/drivers_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_resources_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_grants_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/tags_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/access_requests_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_grants_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_steps_pb2.py
+Filename: strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/drivers_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/tags_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/peering_group_resources_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflows_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/resources_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/role_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_attachments_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_stores_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_resources_pb2.py
+Filename: strongdm-8.0.0/strongdm/access_requests_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_request_events_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/queries_pb2.py
+Filename: strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/__init__.py
+Filename: strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_requests_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/resources_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_store_healths_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/models.py
+Filename: strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/drivers_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_roles_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/nodes_pb2.py
+Filename: strongdm-8.0.0/strongdm/tags_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_assignments_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/remote_identities_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/roles_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/replays_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/role_resources_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/activities_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/options_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_assignments_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_assignments_pb2.py
+Filename: strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_requests_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/svc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_stores_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/constants.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_stores_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_attachments_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_request_events_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/tags_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/accounts_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identity_groups_pb2.py
+Filename: strongdm-8.0.0/strongdm/peering_groups_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/queries_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identities_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/access_requests_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflows_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_store_types_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_assignments_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_resources_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/plumbing.py
+Filename: strongdm-8.0.0/strongdm/account_attachments_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/accounts_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/control_panel_pb2.py
+Filename: strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/accounts_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/queries_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_roles_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/options_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflows_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/roles_pb2.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_stores_pb2.py
+Filename: strongdm-8.0.0/strongdm/accounts_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_attachments_pb2.py
+Filename: strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/nodes_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_attachments_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identities_pb2.py
+Filename: strongdm-8.0.0/strongdm/secret_store_types_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_nodes_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_permissions_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/peering_group_peers_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_resources_pb2.py
+Filename: strongdm-8.0.0/strongdm/spec_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_roles_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/errors.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/secret_store_healths_pb2.py
+Filename: strongdm-8.0.0/strongdm/resources_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/activities_pb2.py
+Filename: strongdm-8.0.0/strongdm/control_panel_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/role_resources_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/models.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflows_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/secret_store_healths_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/errors.py
+Filename: strongdm-8.0.0/strongdm/accounts_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/svc.py
+Filename: strongdm-8.0.0/strongdm/roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/spec_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/replays_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/approval_workflows_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_resources_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/organization_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/constants.py
+Filename: strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/resources_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflows_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/remote_identities_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/replays_pb2.py
+Filename: strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/remote_identities_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_attachments_history_pb2.py
+Filename: strongdm-8.0.0/strongdm/roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/account_grants_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_roles_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflows_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm.egg-info/requires.txt
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_steps_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm.egg-info/top_level.txt
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2.py
+Filename: strongdm-8.0.0/strongdm.egg-info/PKG-INFO
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/roles_history_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: strongdm-7.1.1/strongdm/workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.0.0/strongdm.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `strongdm-7.1.1/setup.py` & `strongdm-8.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from setuptools import setup
 setup(
     name='strongdm',
     packages=['strongdm'],
-    version='7.1.1',
+    version='8.0.0',
     license='apache-2.0',
     description='strongDM SDK for the Python programming language.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='strongDM Team',
     author_email='sdk-feedback@strongdm.com',
     url='https://github.com/strongdm/strongdm-sdk-python',
     download_url=
-    'https://github.com/strongdm/strongdm-sdk-python/archive/v7.1.1.tar.gz',
+    'https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz',
     keywords=[
         'strongDM', 'sdm', 'api', 'automation', 'security', 'audit',
         'database', 'server', 'ssh', 'rdp'
     ],
     install_requires=[
         'grpcio>=1.42.0',
         'googleapis-common-protos>1.56.2,<2',
```

## Comparing `strongdm-7.1.1/PKG-INFO` & `strongdm-8.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 7.1.1
+Version: 8.0.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v7.1.1.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-7.1.1/README.md` & `strongdm-8.0.0/README.md`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/LICENSE` & `strongdm-8.0.0/LICENSE`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm.egg-info/SOURCES.txt` & `strongdm-8.0.0/strongdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm.egg-info/PKG-INFO` & `strongdm-8.0.0/strongdm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 7.1.1
+Version: 8.0.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v7.1.1.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.0.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-7.1.1/strongdm/organization_history_pb2.py` & `strongdm-8.0.0/strongdm/organization_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/client.py` & `strongdm-8.0.0/strongdm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from . import svc
 
 # These defaults are taken from AWS. Customization of these values
 # is a future step in the API.
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_BASE_RETRY_DELAY = 0.0030  # 30 ms
 DEFAULT_MAX_RETRY_DELAY = 300  # 300 seconds
-API_VERSION = '2024-03-14'
-USER_AGENT = 'strongdm-sdk-python/7.1.1'
+API_VERSION = '2024-03-28'
+USER_AGENT = 'strongdm-sdk-python/8.0.0'
 
 
 class Client:
     '''Client interacts with the strongDM API.'''
     def __init__(self,
                  api_access_key,
                  api_secret,
@@ -135,14 +135,15 @@
         See `strongdm.svc.AccountResourcesHistory`.
         '''
         self.accounts = svc.Accounts(channel, self)
         '''
          Accounts are users that have access to strongDM. There are two types of accounts:
          1. **Users:** humans who are authenticated through username and password or SSO.
          2. **Service Accounts:** machines that are authenticated using a service token.
+         3. **Tokens** are access keys with permissions that can be used for authentication.
 
         See `strongdm.svc.Accounts`.
         '''
         self.accounts_history = svc.AccountsHistory(channel, self)
         '''
          AccountsHistory records all changes to the state of an Account.
 
@@ -422,15 +423,16 @@
         ]
 
     def sign(self, method_name, request_bytes):
         def hmac_digest(key, msg_byte_string):
             return hmac.new(key, msg=msg_byte_string,
                             digestmod=hashlib.sha256).digest()
 
-        current_utc_date = datetime.datetime.utcnow().strftime('%Y-%m-%d')
+        current_utc_date = datetime.datetime.now(
+            datetime.timezone.utc).strftime('%Y-%m-%d')
         signing_key = hmac_digest(self.api_secret, current_utc_date.encode())
         signing_key = hmac_digest(signing_key, b'sdm_api_v1')
 
         hash = hashlib.sha256()
 
         hash.update(method_name.encode())
         hash.update(b'\n')
@@ -545,14 +547,15 @@
         See `strongdm.svc.SnapshotAccountResources`.
         '''
         self.accounts = svc.SnapshotAccounts(client.accounts)
         '''
          Accounts are users that have access to strongDM. There are two types of accounts:
          1. **Users:** humans who are authenticated through username and password or SSO.
          2. **Service Accounts:** machines that are authenticated using a service token.
+         3. **Tokens** are access keys with permissions that can be used for authentication.
 
         See `strongdm.svc.SnapshotAccounts`.
         '''
         self.approval_workflow_approvers = svc.SnapshotApprovalWorkflowApprovers(
             client.approval_workflow_approvers)
         '''
          ApprovalWorkflowApprovers link approval workflow approvers to an ApprovalWorkflowStep
```

## Comparing `strongdm-7.1.1/strongdm/workflow_roles_pb2.py` & `strongdm-8.0.0/strongdm/workflow_roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflows_pb2.py` & `strongdm-8.0.0/strongdm/workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_approvers_history_pb2.py` & `strongdm-8.0.0/strongdm/workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/control_panel_pb2_grpc.py` & `strongdm-8.0.0/strongdm/control_panel_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_groups_pb2.py` & `strongdm-8.0.0/strongdm/peering_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identity_groups_pb2_grpc.py` & `strongdm-8.0.0/strongdm/remote_identity_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_nodes_pb2.py` & `strongdm-8.0.0/strongdm/peering_group_nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_requests_history_pb2.py` & `strongdm-8.0.0/strongdm/access_requests_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identities_history_pb2.py` & `strongdm-8.0.0/strongdm/remote_identities_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_peers_pb2.py` & `strongdm-8.0.0/strongdm/peering_group_peers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/spec_pb2.py` & `strongdm-8.0.0/strongdm/spec_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/roles_history_pb2.py` & `strongdm-8.0.0/strongdm/roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_grants_pb2.py` & `strongdm-8.0.0/strongdm/account_grants_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_store_types_pb2.py` & `strongdm-8.0.0/strongdm/secret_store_types_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/role_resources_pb2.py` & `strongdm-8.0.0/strongdm/role_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/role_resources_pb2_grpc.py` & `strongdm-8.0.0/strongdm/role_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/activities_pb2_grpc.py` & `strongdm-8.0.0/strongdm/activities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/accounts_pb2.py` & `strongdm-8.0.0/strongdm/accounts_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import options_pb2 as options__pb2
 from . import spec_pb2 as spec__pb2
 from . import tags_pb2 as tags__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61\x63\x63ounts.proto\x12\x02v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\roptions.proto\x1a\nspec.proto\x1a\ntags.proto\"i\n\x14\x41\x63\x63ountCreateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.CreateRequestMetadata\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xfc\x01\n\x15\x41\x63\x63ountCreateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.CreateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05token\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xf0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x04 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"Q\n\x11\x41\x63\x63ountGetRequest\x12$\n\x04meta\x18\x01 \x01(\x0b\x32\x16.v1.GetRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xd6\x01\n\x12\x41\x63\x63ountGetResponse\x12\x31\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.GetResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"u\n\x14\x41\x63\x63ountUpdateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.UpdateRequestMetadata\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xdc\x01\n\x15\x41\x63\x63ountUpdateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.UpdateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x14\x41\x63\x63ountDeleteRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.DeleteRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xb2\x01\n\x15\x41\x63\x63ountDeleteResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.DeleteResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x02 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x12\x41\x63\x63ountListRequest\x12%\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.ListRequestMetadata\x12\x1a\n\x06\x66ilter\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xc1\x01\n\x13\x41\x63\x63ountListResponse\x12&\n\x04meta\x18\x01 \x01(\x0b\x32\x18.v1.ListResponseMetadata\x12)\n\x08\x61\x63\x63ounts\x18\x02 \x03(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb8\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\"\x9e\x02\n\x07\x41\x63\x63ount\x12$\n\x04user\x18\x01 \x01(\x0b\x32\x08.v1.UserB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12*\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.ServiceB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x30\n\x05token\x18\x03 \x01(\x0b\x32\t.v1.TokenB\x14\xf2\xf8\xb3\x07\x0f\xb2\xf4\xb3\x07\ngo_privateH\x00:a\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\xfa\xf8\xb3\x07R\xc2\xf3\xb3\x07M\xa2\xf3\xb3\x07 tf_examples/account_resource.txt\xaa\xf3\xb3\x07#tf_examples/account_data_source.txtB,\n\x07\x61\x63\x63ount\x12!\xaa\xf8\xb3\x07\x0e\xaa\xf8\xb3\x07\tsuspended\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\"\xd2\x06\n\x04User\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05\x65mail\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12#\n\nfirst_name\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\"\n\tlast_name\x18\x04 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12*\n\tsuspended\x18\x05 \x01(\x08\x42\x17\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12\"\n\x04tags\x18\x06 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x36\n\x10permission_level\x18\x07 \x01(\tB\x1c\xf2\xf8\xb3\x07\x17\x98\xf4\xb3\x07\x01\xb2\xf4\xb3\x07\r!json_gateway\x12#\n\nmanaged_by\x18\x08 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\x98\xf4\xb3\x07\x01\x12\x1f\n\x0b\x65xternal_id\x18\t \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\xdb\x01\n\x0bsuspendedRO\x18\n \x01(\x08\x42\xc5\x01\xf2\xf8\xb3\x07\xbf\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xaf\x01\xc2\xf4\xb3\x07\x0f\n\x02go\x12\tSuspended\xc2\xf4\xb3\x07\x10\n\x03\x63li\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04ruby\x12\tsuspended\xc2\xf4\xb3\x07\x13\n\x06python\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04java\x12\tSuspended\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tsuspended\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tsuspended\x98\xf4\xb3\x07\x01\x12\x90\x02\n\x12permission_levelRW\x18\x0b \x01(\tB\xf3\x01\xf2\xf8\xb3\x07\xed\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xdd\x01\xc2\xf4\xb3\x07\x15\n\x02go\x12\x0fPermissionLevel\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10permission-level\xc2\xf4\xb3\x07\x18\n\x04ruby\x12\x10permission_level\xc2\xf4\xb3\x07\x1a\n\x06python\x12\x10permission_level\xc2\xf4\xb3\x07\x17\n\x04java\x12\x0fPermissionLevel\xc2\xf4\xb3\x07&\n\x12terraform-provider\x12\x10permission_level\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fpermissionLevel\xd0\xf4\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x8f\x01\n\x07Service\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x8f\x02\n\x05Token\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x07rekeyed\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x38\n\x08\x64\x65\x61\x64line\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x19\xfa\xf8\xb3\x07\x14\xa8\xf3\xb3\x07\x01\xd2\xf3\xb3\x07\ngo_private2\xa1\x04\n\x08\x41\x63\x63ounts\x12\x63\n\x06\x43reate\x12\x18.v1.AccountCreateRequest\x1a\x19.v1.AccountCreateResponse\"$\x82\xf9\xb3\x07\t\xa2\xf3\xb3\x07\x04post\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x12^\n\x03Get\x12\x15.v1.AccountGetRequest\x1a\x16.v1.AccountGetResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12g\n\x06Update\x12\x18.v1.AccountUpdateRequest\x1a\x19.v1.AccountUpdateResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03put\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12j\n\x06\x44\x65lete\x12\x18.v1.AccountDeleteRequest\x1a\x19.v1.AccountDeleteResponse\"+\x82\xf9\xb3\x07\x0b\xa2\xf3\xb3\x07\x06\x64\x65lete\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12\\\n\x04List\x12\x16.v1.AccountListRequest\x1a\x17.v1.AccountListResponse\"#\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x1a\x1d\xca\xf9\xb3\x07\x0c\xc2\xf9\xb3\x07\x07\x41\x63\x63ount\xca\xf9\xb3\x07\x07\xd2\xf9\xb3\x07\x02\x61-Bd\n\x19\x63om.strongdm.api.plumbingB\x10\x41\x63\x63ountsPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61\x63\x63ounts.proto\x12\x02v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\roptions.proto\x1a\nspec.proto\x1a\ntags.proto\"i\n\x14\x41\x63\x63ountCreateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.CreateRequestMetadata\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xf8\x02\n\x15\x41\x63\x63ountCreateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.CreateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05token\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xf0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x04 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12<\n\naccess_key\x18\x05 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider\x12<\n\nsecret_key\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-provider:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"Q\n\x11\x41\x63\x63ountGetRequest\x12$\n\x04meta\x18\x01 \x01(\x0b\x32\x16.v1.GetRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xd6\x01\n\x12\x41\x63\x63ountGetResponse\x12\x31\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.GetResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"u\n\x14\x41\x63\x63ountUpdateRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.UpdateRequestMetadata\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\x07\x61\x63\x63ount\x18\x03 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xdc\x01\n\x15\x41\x63\x63ountUpdateResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.UpdateResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12(\n\x07\x61\x63\x63ount\x18\x02 \x01(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x14\x41\x63\x63ountDeleteRequest\x12\'\n\x04meta\x18\x01 \x01(\x0b\x32\x19.v1.DeleteRequestMetadata\x12\x16\n\x02id\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xb2\x01\n\x15\x41\x63\x63ountDeleteResponse\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32\x1a.v1.DeleteResponseMetadataB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x02 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"W\n\x12\x41\x63\x63ountListRequest\x12%\n\x04meta\x18\x01 \x01(\x0b\x32\x17.v1.ListRequestMetadata\x12\x1a\n\x06\x66ilter\x18\x02 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\"\xc1\x01\n\x13\x41\x63\x63ountListResponse\x12&\n\x04meta\x18\x01 \x01(\x0b\x32\x18.v1.ListResponseMetadata\x12)\n\x08\x61\x63\x63ounts\x18\x02 \x03(\x0b\x32\x0b.v1.AccountB\n\xf2\xf8\xb3\x07\x05\xb8\xf3\xb3\x07\x01\x12W\n\nrate_limit\x18\x03 \x01(\x0b\x32\x15.v1.RateLimitMetadataB,\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\xf2\xf8\xb3\x07\x06\xb2\xf4\xb3\x07\x01*\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\"\xb2\x02\n\x07\x41\x63\x63ount\x12$\n\x04user\x18\x01 \x01(\x0b\x32\x08.v1.UserB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12*\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.ServiceB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x44\n\x05token\x18\x03 \x01(\x0b\x32\t.v1.TokenB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xb2\xf4\xb3\x07\x01*\xb2\xf4\xb3\x07\x13!terraform-providerH\x00:a\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\xfa\xf8\xb3\x07R\xc2\xf3\xb3\x07M\xa2\xf3\xb3\x07 tf_examples/account_resource.txt\xaa\xf3\xb3\x07#tf_examples/account_data_source.txtB,\n\x07\x61\x63\x63ount\x12!\xaa\xf8\xb3\x07\x0e\xaa\xf8\xb3\x07\tsuspended\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\"\xd2\x06\n\x04User\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1e\n\x05\x65mail\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12#\n\nfirst_name\x18\x03 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\"\n\tlast_name\x18\x04 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12*\n\tsuspended\x18\x05 \x01(\x08\x42\x17\xf2\xf8\xb3\x07\x12\xb2\xf4\xb3\x07\r!json_gateway\x12\"\n\x04tags\x18\x06 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x36\n\x10permission_level\x18\x07 \x01(\tB\x1c\xf2\xf8\xb3\x07\x17\x98\xf4\xb3\x07\x01\xb2\xf4\xb3\x07\r!json_gateway\x12#\n\nmanaged_by\x18\x08 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\x98\xf4\xb3\x07\x01\x12\x1f\n\x0b\x65xternal_id\x18\t \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\xdb\x01\n\x0bsuspendedRO\x18\n \x01(\x08\x42\xc5\x01\xf2\xf8\xb3\x07\xbf\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xaf\x01\xc2\xf4\xb3\x07\x0f\n\x02go\x12\tSuspended\xc2\xf4\xb3\x07\x10\n\x03\x63li\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04ruby\x12\tsuspended\xc2\xf4\xb3\x07\x13\n\x06python\x12\tsuspended\xc2\xf4\xb3\x07\x11\n\x04java\x12\tSuspended\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tsuspended\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tsuspended\x98\xf4\xb3\x07\x01\x12\x90\x02\n\x12permission_levelRW\x18\x0b \x01(\tB\xf3\x01\xf2\xf8\xb3\x07\xed\x01\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\xdd\x01\xc2\xf4\xb3\x07\x15\n\x02go\x12\x0fPermissionLevel\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10permission-level\xc2\xf4\xb3\x07\x18\n\x04ruby\x12\x10permission_level\xc2\xf4\xb3\x07\x1a\n\x06python\x12\x10permission_level\xc2\xf4\xb3\x07\x17\n\x04java\x12\x0fPermissionLevel\xc2\xf4\xb3\x07&\n\x12terraform-provider\x12\x10permission_level\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fpermissionLevel\xd0\xf4\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x8f\x01\n\x07Service\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\"\x9a\x03\n\x05Token\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x1d\n\tsuspended\x18\x03 \x01(\x08\x42\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x07rekeyed\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x38\n\x08\x64\x65\x61\x64line\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12 \n\x0c\x61\x63\x63ount_type\x18\x07 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1f\n\x0bpermissions\x18\x08 \x03(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x37\n\x08\x64uration\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:(\xfa\xf8\xb3\x07#\xa8\xf3\xb3\x07\x01\xd2\xf3\xb3\x07\x01*\xd2\xf3\xb3\x07\x13!terraform-provider2\xab\x04\n\x08\x41\x63\x63ounts\x12\x63\n\x06\x43reate\x12\x18.v1.AccountCreateRequest\x1a\x19.v1.AccountCreateResponse\"$\x82\xf9\xb3\x07\t\xa2\xf3\xb3\x07\x04post\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x12^\n\x03Get\x12\x15.v1.AccountGetRequest\x1a\x16.v1.AccountGetResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12g\n\x06Update\x12\x18.v1.AccountUpdateRequest\x1a\x19.v1.AccountUpdateResponse\"(\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03put\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12j\n\x06\x44\x65lete\x12\x18.v1.AccountDeleteRequest\x1a\x19.v1.AccountDeleteResponse\"+\x82\xf9\xb3\x07\x0b\xa2\xf3\xb3\x07\x06\x64\x65lete\x82\xf9\xb3\x07\x16\xaa\xf3\xb3\x07\x11/v1/accounts/{id}\x12\\\n\x04List\x12\x16.v1.AccountListRequest\x1a\x17.v1.AccountListResponse\"#\x82\xf9\xb3\x07\x08\xa2\xf3\xb3\x07\x03get\x82\xf9\xb3\x07\x11\xaa\xf3\xb3\x07\x0c/v1/accounts\x1a\'\xca\xf9\xb3\x07\x0c\xc2\xf9\xb3\x07\x07\x41\x63\x63ount\xca\xf9\xb3\x07\x07\xd2\xf9\xb3\x07\x02\x61-\xca\xf9\xb3\x07\x05\xe0\xf9\xb3\x07\x01\x42\x64\n\x19\x63om.strongdm.api.plumbingB\x10\x41\x63\x63ountsPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 
 _ACCOUNTCREATEREQUEST = DESCRIPTOR.message_types_by_name['AccountCreateRequest']
 _ACCOUNTCREATERESPONSE = DESCRIPTOR.message_types_by_name['AccountCreateResponse']
 _ACCOUNTGETREQUEST = DESCRIPTOR.message_types_by_name['AccountGetRequest']
 _ACCOUNTGETRESPONSE = DESCRIPTOR.message_types_by_name['AccountGetResponse']
@@ -159,14 +160,18 @@
   _ACCOUNTCREATERESPONSE.fields_by_name['meta']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNTCREATERESPONSE.fields_by_name['account']._options = None
   _ACCOUNTCREATERESPONSE.fields_by_name['account']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNTCREATERESPONSE.fields_by_name['token']._options = None
   _ACCOUNTCREATERESPONSE.fields_by_name['token']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\360\363\263\007\001'
   _ACCOUNTCREATERESPONSE.fields_by_name['rate_limit']._options = None
   _ACCOUNTCREATERESPONSE.fields_by_name['rate_limit']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001\362\370\263\007\006\262\364\263\007\001*\362\370\263\007\022\262\364\263\007\r!json_gateway'
+  _ACCOUNTCREATERESPONSE.fields_by_name['access_key']._options = None
+  _ACCOUNTCREATERESPONSE.fields_by_name['access_key']._serialized_options = b'\362\370\263\007#\260\363\263\007\001\262\364\263\007\001*\262\364\263\007\023!terraform-provider'
+  _ACCOUNTCREATERESPONSE.fields_by_name['secret_key']._options = None
+  _ACCOUNTCREATERESPONSE.fields_by_name['secret_key']._serialized_options = b'\362\370\263\007#\260\363\263\007\001\262\364\263\007\001*\262\364\263\007\023!terraform-provider'
   _ACCOUNTCREATERESPONSE._options = None
   _ACCOUNTCREATERESPONSE._serialized_options = b'\372\370\263\007\005\250\363\263\007\001'
   _ACCOUNTGETREQUEST.fields_by_name['id']._options = None
   _ACCOUNTGETREQUEST.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNTGETRESPONSE.fields_by_name['meta']._options = None
   _ACCOUNTGETRESPONSE.fields_by_name['meta']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNTGETRESPONSE.fields_by_name['account']._options = None
@@ -202,15 +207,15 @@
   _ACCOUNT.oneofs_by_name['account']._options = None
   _ACCOUNT.oneofs_by_name['account']._serialized_options = b'\252\370\263\007\016\252\370\263\007\tsuspended\252\370\263\007\t\252\370\263\007\004tags'
   _ACCOUNT.fields_by_name['user']._options = None
   _ACCOUNT.fields_by_name['user']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNT.fields_by_name['service']._options = None
   _ACCOUNT.fields_by_name['service']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _ACCOUNT.fields_by_name['token']._options = None
-  _ACCOUNT.fields_by_name['token']._serialized_options = b'\362\370\263\007\017\262\364\263\007\ngo_private'
+  _ACCOUNT.fields_by_name['token']._serialized_options = b'\362\370\263\007#\260\363\263\007\001\262\364\263\007\001*\262\364\263\007\023!terraform-provider'
   _ACCOUNT._options = None
   _ACCOUNT._serialized_options = b'\372\370\263\007\005\250\363\263\007\001\372\370\263\007R\302\363\263\007M\242\363\263\007 tf_examples/account_resource.txt\252\363\263\007#tf_examples/account_data_source.txt'
   _USER.fields_by_name['id']._options = None
   _USER.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _USER.fields_by_name['email']._options = None
   _USER.fields_by_name['email']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
   _USER.fields_by_name['first_name']._options = None
@@ -251,52 +256,58 @@
   _TOKEN.fields_by_name['suspended']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN.fields_by_name['tags']._options = None
   _TOKEN.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN.fields_by_name['rekeyed']._options = None
   _TOKEN.fields_by_name['rekeyed']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN.fields_by_name['deadline']._options = None
   _TOKEN.fields_by_name['deadline']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _TOKEN.fields_by_name['account_type']._options = None
+  _TOKEN.fields_by_name['account_type']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _TOKEN.fields_by_name['permissions']._options = None
+  _TOKEN.fields_by_name['permissions']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _TOKEN.fields_by_name['duration']._options = None
+  _TOKEN.fields_by_name['duration']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _TOKEN._options = None
-  _TOKEN._serialized_options = b'\372\370\263\007\024\250\363\263\007\001\322\363\263\007\ngo_private'
+  _TOKEN._serialized_options = b'\372\370\263\007#\250\363\263\007\001\322\363\263\007\001*\322\363\263\007\023!terraform-provider'
   _ACCOUNTS._options = None
-  _ACCOUNTS._serialized_options = b'\312\371\263\007\014\302\371\263\007\007Account\312\371\263\007\007\322\371\263\007\002a-'
+  _ACCOUNTS._serialized_options = b'\312\371\263\007\014\302\371\263\007\007Account\312\371\263\007\007\322\371\263\007\002a-\312\371\263\007\005\340\371\263\007\001'
   _ACCOUNTS.methods_by_name['Create']._options = None
   _ACCOUNTS.methods_by_name['Create']._serialized_options = b'\202\371\263\007\t\242\363\263\007\004post\202\371\263\007\021\252\363\263\007\014/v1/accounts'
   _ACCOUNTS.methods_by_name['Get']._options = None
   _ACCOUNTS.methods_by_name['Get']._serialized_options = b'\202\371\263\007\010\242\363\263\007\003get\202\371\263\007\026\252\363\263\007\021/v1/accounts/{id}'
   _ACCOUNTS.methods_by_name['Update']._options = None
   _ACCOUNTS.methods_by_name['Update']._serialized_options = b'\202\371\263\007\010\242\363\263\007\003put\202\371\263\007\026\252\363\263\007\021/v1/accounts/{id}'
   _ACCOUNTS.methods_by_name['Delete']._options = None
   _ACCOUNTS.methods_by_name['Delete']._serialized_options = b'\202\371\263\007\013\242\363\263\007\006delete\202\371\263\007\026\252\363\263\007\021/v1/accounts/{id}'
   _ACCOUNTS.methods_by_name['List']._options = None
   _ACCOUNTS.methods_by_name['List']._serialized_options = b'\202\371\263\007\010\242\363\263\007\003get\202\371\263\007\021\252\363\263\007\014/v1/accounts'
-  _ACCOUNTCREATEREQUEST._serialized_start=94
-  _ACCOUNTCREATEREQUEST._serialized_end=199
-  _ACCOUNTCREATERESPONSE._serialized_start=202
-  _ACCOUNTCREATERESPONSE._serialized_end=454
-  _ACCOUNTGETREQUEST._serialized_start=456
-  _ACCOUNTGETREQUEST._serialized_end=537
-  _ACCOUNTGETRESPONSE._serialized_start=540
-  _ACCOUNTGETRESPONSE._serialized_end=754
-  _ACCOUNTUPDATEREQUEST._serialized_start=756
-  _ACCOUNTUPDATEREQUEST._serialized_end=873
-  _ACCOUNTUPDATERESPONSE._serialized_start=876
-  _ACCOUNTUPDATERESPONSE._serialized_end=1096
-  _ACCOUNTDELETEREQUEST._serialized_start=1098
-  _ACCOUNTDELETEREQUEST._serialized_end=1185
-  _ACCOUNTDELETERESPONSE._serialized_start=1188
-  _ACCOUNTDELETERESPONSE._serialized_end=1366
-  _ACCOUNTLISTREQUEST._serialized_start=1368
-  _ACCOUNTLISTREQUEST._serialized_end=1455
-  _ACCOUNTLISTRESPONSE._serialized_start=1458
-  _ACCOUNTLISTRESPONSE._serialized_end=1651
-  _ACCOUNT._serialized_start=1654
-  _ACCOUNT._serialized_end=1940
-  _USER._serialized_start=1943
-  _USER._serialized_end=2793
-  _SERVICE._serialized_start=2796
-  _SERVICE._serialized_end=2939
-  _TOKEN._serialized_start=2942
-  _TOKEN._serialized_end=3213
-  _ACCOUNTS._serialized_start=3216
-  _ACCOUNTS._serialized_end=3761
+  _ACCOUNTCREATEREQUEST._serialized_start=126
+  _ACCOUNTCREATEREQUEST._serialized_end=231
+  _ACCOUNTCREATERESPONSE._serialized_start=234
+  _ACCOUNTCREATERESPONSE._serialized_end=610
+  _ACCOUNTGETREQUEST._serialized_start=612
+  _ACCOUNTGETREQUEST._serialized_end=693
+  _ACCOUNTGETRESPONSE._serialized_start=696
+  _ACCOUNTGETRESPONSE._serialized_end=910
+  _ACCOUNTUPDATEREQUEST._serialized_start=912
+  _ACCOUNTUPDATEREQUEST._serialized_end=1029
+  _ACCOUNTUPDATERESPONSE._serialized_start=1032
+  _ACCOUNTUPDATERESPONSE._serialized_end=1252
+  _ACCOUNTDELETEREQUEST._serialized_start=1254
+  _ACCOUNTDELETEREQUEST._serialized_end=1341
+  _ACCOUNTDELETERESPONSE._serialized_start=1344
+  _ACCOUNTDELETERESPONSE._serialized_end=1522
+  _ACCOUNTLISTREQUEST._serialized_start=1524
+  _ACCOUNTLISTREQUEST._serialized_end=1611
+  _ACCOUNTLISTRESPONSE._serialized_start=1614
+  _ACCOUNTLISTRESPONSE._serialized_end=1807
+  _ACCOUNT._serialized_start=1810
+  _ACCOUNT._serialized_end=2116
+  _USER._serialized_start=2119
+  _USER._serialized_end=2969
+  _SERVICE._serialized_start=2972
+  _SERVICE._serialized_end=3115
+  _TOKEN._serialized_start=3118
+  _TOKEN._serialized_end=3528
+  _ACCOUNTS._serialized_start=3531
+  _ACCOUNTS._serialized_end=4086
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-7.1.1/strongdm/options_pb2_grpc.py` & `strongdm-8.0.0/strongdm/options_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/nodes_pb2_grpc.py` & `strongdm-8.0.0/strongdm/nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflows_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_grants_history_pb2.py` & `strongdm-8.0.0/strongdm/account_grants_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_approvers_pb2.py` & `strongdm-8.0.0/strongdm/workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/resources_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_assignments_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_assignments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_permissions_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_permissions_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2.py` & `strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflows_history_pb2.py` & `strongdm-8.0.0/strongdm/workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_approvers_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_resources_history_pb2.py` & `strongdm-8.0.0/strongdm/account_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/nodes_history_pb2.py` & `strongdm-8.0.0/strongdm/nodes_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_permissions_pb2.py` & `strongdm-8.0.0/strongdm/account_permissions_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_groups_pb2_grpc.py` & `strongdm-8.0.0/strongdm/peering_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_resources_pb2_grpc.py` & `strongdm-8.0.0/strongdm/peering_group_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/tags_pb2.py` & `strongdm-8.0.0/strongdm/tags_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identity_groups_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/remote_identity_groups_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_grants_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_grants_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_steps_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflow_steps_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/drivers_pb2_grpc.py` & `strongdm-8.0.0/strongdm/spec_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/tags_pb2_grpc.py` & `strongdm-8.0.0/strongdm/drivers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflows_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/resources_history_pb2.py` & `strongdm-8.0.0/strongdm/resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_attachments_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_attachments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_stores_history_pb2.py` & `strongdm-8.0.0/strongdm/secret_stores_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_resources_pb2.py` & `strongdm-8.0.0/strongdm/peering_group_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_request_events_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/access_request_events_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/queries_pb2.py` & `strongdm-8.0.0/strongdm/queries_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/__init__.py` & `strongdm-8.0.0/strongdm/__init__.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_requests_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/access_requests_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/resources_pb2_grpc.py` & `strongdm-8.0.0/strongdm/resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_store_healths_pb2_grpc.py` & `strongdm-8.0.0/strongdm/secret_store_healths_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/models.py` & `strongdm-8.0.0/strongdm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2149,67 +2149,85 @@
 
 
 class AccountCreateResponse:
     '''
          AccountCreateResponse reports how the Accounts were created in the system.
     '''
     __slots__ = [
+        'access_key',
         'account',
         'meta',
         'rate_limit',
+        'secret_key',
         'token',
     ]
 
     def __init__(
         self,
+        access_key=None,
         account=None,
         meta=None,
         rate_limit=None,
+        secret_key=None,
         token=None,
     ):
+        self.access_key = access_key if access_key is not None else ''
+        '''
+         ID part of the API key.
+        '''
         self.account = account if account is not None else None
         '''
          The created Account.
         '''
         self.meta = meta if meta is not None else None
         '''
          Reserved for future use.
         '''
         self.rate_limit = rate_limit if rate_limit is not None else None
         '''
          Rate limit information.
         '''
+        self.secret_key = secret_key if secret_key is not None else ''
+        '''
+         Secret part of the API key.
+        '''
         self.token = token if token is not None else ''
         '''
          The auth token generated for the Account. The Account will use this token to
          authenticate with the strongDM API.
         '''
 
     def __repr__(self):
         return '<sdm.AccountCreateResponse ' + \
+            'access_key: ' + repr(self.access_key) + ' ' +\
             'account: ' + repr(self.account) + ' ' +\
             'meta: ' + repr(self.meta) + ' ' +\
             'rate_limit: ' + repr(self.rate_limit) + ' ' +\
+            'secret_key: ' + repr(self.secret_key) + ' ' +\
             'token: ' + repr(self.token) + ' ' +\
             '>'
 
     def to_dict(self):
         return {
+            'access_key': self.access_key,
             'account': self.account,
             'meta': self.meta,
             'rate_limit': self.rate_limit,
+            'secret_key': self.secret_key,
             'token': self.token,
         }
 
     @classmethod
     def from_dict(cls, d):
         return cls(
+            access_key=d.get('access_key'),
             account=d.get('account'),
             meta=d.get('meta'),
             rate_limit=d.get('rate_limit'),
+            secret_key=d.get('secret_key'),
             token=d.get('token'),
         )
 
 
 class AccountDeleteResponse:
     '''
          AccountDeleteResponse returns information about a Account that was deleted.
@@ -20822,14 +20840,121 @@
             secret_store_id=d.get('secret_store_id'),
             subdomain=d.get('subdomain'),
             tags=d.get('tags'),
             username=d.get('username'),
         )
 
 
+class Token:
+    '''
+         A Token is an account providing tokenized access for automation or integration use.
+     Tokens include admin tokens, API keys, and SCIM tokens.
+    '''
+    __slots__ = [
+        'account_type',
+        'deadline',
+        'duration',
+        'id',
+        'name',
+        'permissions',
+        'rekeyed',
+        'suspended',
+        'tags',
+    ]
+
+    def __init__(
+        self,
+        account_type=None,
+        deadline=None,
+        duration=None,
+        id=None,
+        name=None,
+        permissions=None,
+        rekeyed=None,
+        suspended=None,
+        tags=None,
+    ):
+        self.account_type = account_type if account_type is not None else ''
+        '''
+         Corresponds to the type of token, e.g. api or admin-token.
+        '''
+        self.deadline = deadline if deadline is not None else None
+        '''
+         The timestamp when the Token will expire.
+        '''
+        self.duration = duration if duration is not None else None
+        '''
+         Duration from token creation to expiration.
+        '''
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the Token.
+        '''
+        self.name = name if name is not None else ''
+        '''
+         Unique human-readable name of the Token.
+        '''
+        self.permissions = permissions if permissions is not None else []
+        '''
+         Permissions assigned to the token, e.g. role:create.
+        '''
+        self.rekeyed = rekeyed if rekeyed is not None else None
+        '''
+         The timestamp when the Token was last rekeyed.
+        '''
+        self.suspended = suspended if suspended is not None else False
+        '''
+         Reserved for future use.  Always false for tokens.
+        '''
+        self.tags = tags if tags is not None else _porcelain_zero_value_tags()
+        '''
+         Tags is a map of key, value pairs.
+        '''
+
+    def __repr__(self):
+        return '<sdm.Token ' + \
+            'account_type: ' + repr(self.account_type) + ' ' +\
+            'deadline: ' + repr(self.deadline) + ' ' +\
+            'duration: ' + repr(self.duration) + ' ' +\
+            'id: ' + repr(self.id) + ' ' +\
+            'name: ' + repr(self.name) + ' ' +\
+            'permissions: ' + repr(self.permissions) + ' ' +\
+            'rekeyed: ' + repr(self.rekeyed) + ' ' +\
+            'suspended: ' + repr(self.suspended) + ' ' +\
+            'tags: ' + repr(self.tags) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'account_type': self.account_type,
+            'deadline': self.deadline,
+            'duration': self.duration,
+            'id': self.id,
+            'name': self.name,
+            'permissions': self.permissions,
+            'rekeyed': self.rekeyed,
+            'suspended': self.suspended,
+            'tags': self.tags,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            account_type=d.get('account_type'),
+            deadline=d.get('deadline'),
+            duration=d.get('duration'),
+            id=d.get('id'),
+            name=d.get('name'),
+            permissions=d.get('permissions'),
+            rekeyed=d.get('rekeyed'),
+            suspended=d.get('suspended'),
+            tags=d.get('tags'),
+        )
+
+
 class Trino:
     '''
     Trino is currently unstable, and its API may change, or it may be removed,
     without a major version bump.
     '''
     __slots__ = [
         'bind_interface',
```

## Comparing `strongdm-7.1.1/strongdm/drivers_pb2.py` & `strongdm-8.0.0/strongdm/drivers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/nodes_pb2.py` & `strongdm-8.0.0/strongdm/nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_assignments_history_pb2.py` & `strongdm-8.0.0/strongdm/workflow_assignments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/roles_pb2_grpc.py` & `strongdm-8.0.0/strongdm/roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/role_resources_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/role_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/options_pb2.py` & `strongdm-8.0.0/strongdm/options_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_assignments_pb2.py` & `strongdm-8.0.0/strongdm/workflow_assignments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_requests_pb2_grpc.py` & `strongdm-8.0.0/strongdm/access_requests_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_stores_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/secret_stores_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_approvers_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_stores_pb2_grpc.py` & `strongdm-8.0.0/strongdm/secret_stores_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_attachments_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_attachments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_request_events_history_pb2.py` & `strongdm-8.0.0/strongdm/access_request_events_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/accounts_pb2_grpc.py` & `strongdm-8.0.0/strongdm/accounts_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from . import accounts_pb2 as accounts__pb2
 
 
 class AccountsStub(object):
     """Accounts are users that have access to strongDM. There are two types of accounts:
     1. **Users:** humans who are authenticated through username and password or SSO.
     2. **Service Accounts:** machines that are authenticated using a service token.
+    3. **Tokens** are access keys with permissions that can be used for authentication.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -58,14 +59,15 @@
                 )
 
 
 class AccountsServicer(object):
     """Accounts are users that have access to strongDM. There are two types of accounts:
     1. **Users:** humans who are authenticated through username and password or SSO.
     2. **Service Accounts:** machines that are authenticated using a service token.
+    3. **Tokens** are access keys with permissions that can be used for authentication.
     """
 
     def Create(self, request, context):
         """Create registers a new Account.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -134,14 +136,15 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class Accounts(object):
     """Accounts are users that have access to strongDM. There are two types of accounts:
     1. **Users:** humans who are authenticated through username and password or SSO.
     2. **Service Accounts:** machines that are authenticated using a service token.
+    3. **Tokens** are access keys with permissions that can be used for authentication.
     """
 
     @staticmethod
     def Create(request,
             target,
             options=(),
             channel_credentials=None,
```

## Comparing `strongdm-7.1.1/strongdm/remote_identity_groups_pb2.py` & `strongdm-8.0.0/strongdm/remote_identity_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/queries_pb2_grpc.py` & `strongdm-8.0.0/strongdm/queries_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identities_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/remote_identities_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/access_requests_pb2.py` & `strongdm-8.0.0/strongdm/access_requests_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_store_types_pb2_grpc.py` & `strongdm-8.0.0/strongdm/tags_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_assignments_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_assignments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_resources_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/plumbing.py` & `strongdm-8.0.0/strongdm/plumbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,24 +960,28 @@
 
 def convert_account_to_plumbing(porcelain):
     plumbing = Account()
     if porcelain is None:
         return plumbing
     if isinstance(porcelain, models.Service):
         plumbing.service.CopyFrom(convert_service_to_plumbing(porcelain))
+    if isinstance(porcelain, models.Token):
+        plumbing.token.CopyFrom(convert_token_to_plumbing(porcelain))
     if isinstance(porcelain, models.User):
         plumbing.user.CopyFrom(convert_user_to_plumbing(porcelain))
     return plumbing
 
 
 def convert_account_to_porcelain(plumbing):
     if plumbing is None:
         return None
     if plumbing.HasField('service'):
         return convert_service_to_porcelain(plumbing.service)
+    if plumbing.HasField('token'):
+        return convert_token_to_porcelain(plumbing.token)
     if plumbing.HasField('user'):
         return convert_user_to_porcelain(plumbing.user)
     raise errors.UnknownError(
         "unknown polymorphic type, please upgrade your SDK")
 
 
 def convert_repeated_account_to_plumbing(porcelains):
@@ -1181,32 +1185,36 @@
     ]
 
 
 def convert_account_create_response_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.AccountCreateResponse()
+    porcelain.access_key = (plumbing.access_key)
     porcelain.account = convert_account_to_porcelain(plumbing.account)
     porcelain.meta = convert_create_response_metadata_to_porcelain(
         plumbing.meta)
     porcelain.rate_limit = convert_rate_limit_metadata_to_porcelain(
         plumbing.rate_limit)
+    porcelain.secret_key = (plumbing.secret_key)
     porcelain.token = (plumbing.token)
     return porcelain
 
 
 def convert_account_create_response_to_plumbing(porcelain):
     plumbing = AccountCreateResponse()
     if porcelain is None:
         return plumbing
+    plumbing.access_key = (porcelain.access_key)
     plumbing.account.CopyFrom(convert_account_to_plumbing(porcelain.account))
     plumbing.meta.CopyFrom(
         convert_create_response_metadata_to_plumbing(porcelain.meta))
     plumbing.rate_limit.CopyFrom(
         convert_rate_limit_metadata_to_plumbing(porcelain.rate_limit))
+    plumbing.secret_key = (porcelain.secret_key)
     plumbing.token = (porcelain.token)
     return plumbing
 
 
 def convert_repeated_account_create_response_to_plumbing(porcelains):
     return [
         convert_account_create_response_to_plumbing(porcelain)
@@ -10402,14 +10410,57 @@
     ]
 
 
 def convert_repeated_teradata_to_porcelain(plumbings):
     return [convert_teradata_to_porcelain(plumbing) for plumbing in plumbings]
 
 
+def convert_token_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.Token()
+    porcelain.account_type = (plumbing.account_type)
+    porcelain.deadline = convert_timestamp_to_porcelain(plumbing.deadline)
+    porcelain.duration = convert_duration_to_porcelain(plumbing.duration)
+    porcelain.id = (plumbing.id)
+    porcelain.name = (plumbing.name)
+    porcelain.permissions = (plumbing.permissions)
+    porcelain.rekeyed = convert_timestamp_to_porcelain(plumbing.rekeyed)
+    porcelain.suspended = (plumbing.suspended)
+    porcelain.tags = convert_tags_to_porcelain(plumbing.tags)
+    return porcelain
+
+
+def convert_token_to_plumbing(porcelain):
+    plumbing = Token()
+    if porcelain is None:
+        return plumbing
+    plumbing.account_type = (porcelain.account_type)
+    plumbing.deadline.CopyFrom(
+        convert_timestamp_to_plumbing(porcelain.deadline))
+    plumbing.duration.CopyFrom(convert_duration_to_plumbing(
+        porcelain.duration))
+    plumbing.id = (porcelain.id)
+    plumbing.name = (porcelain.name)
+    del plumbing.permissions[:]
+    plumbing.permissions.extend((porcelain.permissions))
+    plumbing.rekeyed.CopyFrom(convert_timestamp_to_plumbing(porcelain.rekeyed))
+    plumbing.suspended = (porcelain.suspended)
+    plumbing.tags.CopyFrom(convert_tags_to_plumbing(porcelain.tags))
+    return plumbing
+
+
+def convert_repeated_token_to_plumbing(porcelains):
+    return [convert_token_to_plumbing(porcelain) for porcelain in porcelains]
+
+
+def convert_repeated_token_to_porcelain(plumbings):
+    return [convert_token_to_porcelain(plumbing) for plumbing in plumbings]
+
+
 def convert_trino_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.Trino()
     porcelain.bind_interface = (plumbing.bind_interface)
     porcelain.database = (plumbing.database)
     porcelain.egress_filter = (plumbing.egress_filter)
```

## Comparing `strongdm-7.1.1/strongdm/accounts_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/accounts_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/control_panel_pb2.py` & `strongdm-8.0.0/strongdm/control_panel_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/accounts_history_pb2.py` & `strongdm-8.0.0/strongdm/accounts_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_roles_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflows_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/roles_pb2.py` & `strongdm-8.0.0/strongdm/roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_stores_pb2.py` & `strongdm-8.0.0/strongdm/secret_stores_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_attachments_pb2.py` & `strongdm-8.0.0/strongdm/account_attachments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/nodes_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/nodes_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identities_pb2.py` & `strongdm-8.0.0/strongdm/remote_identities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_nodes_pb2_grpc.py` & `strongdm-8.0.0/strongdm/peering_group_nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/peering_group_peers_pb2_grpc.py` & `strongdm-8.0.0/strongdm/peering_group_peers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_resources_pb2.py` & `strongdm-8.0.0/strongdm/account_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_roles_history_pb2.py` & `strongdm-8.0.0/strongdm/workflow_roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_steps_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflow_steps_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/secret_store_healths_pb2.py` & `strongdm-8.0.0/strongdm/secret_store_healths_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/activities_pb2.py` & `strongdm-8.0.0/strongdm/activities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/role_resources_history_pb2.py` & `strongdm-8.0.0/strongdm/role_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflows_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/errors.py` & `strongdm-8.0.0/strongdm/errors.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/svc.py` & `strongdm-8.0.0/strongdm/svc.py`

 * *Files 0% similar despite different names*

```diff
@@ -921,16 +921,18 @@
 
 
 class Accounts:
     '''
      Accounts are users that have access to strongDM. There are two types of accounts:
      1. **Users:** humans who are authenticated through username and password or SSO.
      2. **Service Accounts:** machines that are authenticated using a service token.
+     3. **Tokens** are access keys with permissions that can be used for authentication.
     See:
     `strongdm.models.Service`
+    `strongdm.models.Token`
     `strongdm.models.User`
     '''
     def __init__(self, channel, client):
         self.parent = client
         self.stub = AccountsStub(channel)
 
     def create(self, account, timeout=None):
@@ -954,20 +956,22 @@
                     tries += 1
                     self.parent.jitterSleep(tries)
                     continue
                 raise plumbing.convert_error_to_porcelain(e) from e
             break
 
         resp = models.AccountCreateResponse()
+        resp.access_key = (plumbing_response.access_key)
         resp.account = plumbing.convert_account_to_porcelain(
             plumbing_response.account)
         resp.meta = plumbing.convert_create_response_metadata_to_porcelain(
             plumbing_response.meta)
         resp.rate_limit = plumbing.convert_rate_limit_metadata_to_porcelain(
             plumbing_response.rate_limit)
+        resp.secret_key = (plumbing_response.secret_key)
         resp.token = (plumbing_response.token)
         return resp
 
     def get(self, id, timeout=None):
         '''
          Get reads one Account by ID.
         '''
```

## Comparing `strongdm-7.1.1/strongdm/spec_pb2_grpc.py` & `strongdm-8.0.0/strongdm/secret_store_types_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/replays_pb2_grpc.py` & `strongdm-8.0.0/strongdm/replays_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_resources_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/organization_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/organization_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/constants.py` & `strongdm-8.0.0/strongdm/constants.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/resources_pb2.py` & `strongdm-8.0.0/strongdm/resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflows_history_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/replays_pb2.py` & `strongdm-8.0.0/strongdm/replays_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/remote_identities_pb2_grpc.py` & `strongdm-8.0.0/strongdm/remote_identities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_attachments_history_pb2.py` & `strongdm-8.0.0/strongdm/account_attachments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/account_grants_pb2_grpc.py` & `strongdm-8.0.0/strongdm/account_grants_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_roles_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflows_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_steps_pb2_grpc.py` & `strongdm-8.0.0/strongdm/approval_workflow_steps_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/approval_workflow_approvers_history_pb2.py` & `strongdm-8.0.0/strongdm/approval_workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/roles_history_pb2_grpc.py` & `strongdm-8.0.0/strongdm/roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-7.1.1/strongdm/workflow_approvers_pb2_grpc.py` & `strongdm-8.0.0/strongdm/workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

