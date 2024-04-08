# Comparing `tmp/doppler-sdk-1.2.1.tar.gz` & `tmp/doppler-sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppler-sdk-1.2.1.tar", last modified: Fri Oct  6 16:48:09 2023, max compression
+gzip compressed data, was "doppler-sdk-1.3.0.tar", last modified: Mon Apr  8 22:56:43 2024, max compression
```

## Comparing `doppler-sdk-1.2.1.tar` & `doppler-sdk-1.3.0.tar`

### file list

```diff
@@ -1,208 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:09.011005 doppler-sdk-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-06 16:48:09.011005 doppler-sdk-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 16:48:09.011005 doppler-sdk-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:08.959005 doppler-sdk-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:08.959005 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-06 16:48:08.000000 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2023-10-06 16:48:08.000000 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 16:48:08.000000 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-06 16:48:08.000000 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-06 16:48:08.000000 doppler-sdk-1.2.1/src/doppler_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:08.963005 doppler-sdk-1.2.1/src/dopplersdk/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:08.963005 doppler-sdk-1.2.1/src/dopplersdk/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:09.003005 doppler-sdk-1.2.1/src/dopplersdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsRetrieve200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/AddMemberRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/AddRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/AddResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/AddTrustedIpRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/AddTrustedIpResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/CloneRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/CloneResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsRollback200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsClone200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCloneRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsLock200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsLockRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUnlock200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUnlockRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/CreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/CreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DeleteResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DeleteTrustedIpRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DownloadResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DynamicSecretsRevokeLease200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsRename200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsRenameRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/Format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GetUserResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsType.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/GroupsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsDeleteResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/InvitesListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IssueLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/IssueLeaseResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ListPermissionsResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ListTrustedIpsResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/LockRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/LockResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/MeResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/NameTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/NamesResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesListPermissionsResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RenameRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RenameResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RetrieveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RevokeLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RevokeLeaseResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RevokeRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/RollbackResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsDownload200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsListNames200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateNote200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateNoteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsDeleteResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/SyncsGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UnlockRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UnlockResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UpdateNoteRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UpdateNoteResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UsersGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/UsersListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/V3Me200Response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesCreateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesGetResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceUpdateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:09.003005 doppler-sdk-1.2.1/src/dopplersdk/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10138 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/http_content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/query_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/net/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 16:48:09.011005 doppler-sdk-1.2.1/src/dopplersdk/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/config_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/dynamic_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/invites.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/project_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/project_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/service_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/syncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/trusted_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/v_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/workplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/services/workplace_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-06 16:47:57.000000 doppler-sdk-1.2.1/src/dopplersdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.766404 doppler-sdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-08 22:56:43.766404 doppler-sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:56:43.766404 doppler-sdk-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.730404 doppler-sdk-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.762404 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-08 22:56:43.000000 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-08 22:56:43.000000 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:56:43.000000 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 22:56:43.000000 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 22:56:43.000000 doppler-sdk-1.3.0/src/doppler_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.734404 doppler-sdk-1.3.0/src/dopplersdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.734404 doppler-sdk-1.3.0/src/dopplersdk/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.758404 doppler-sdk-1.3.0/src/dopplersdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsRetrieve200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/AddMemberRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/AddRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/AddResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/AddTrustedIpRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/AddTrustedIpResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/CloneRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/CloneResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsRollback200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsClone200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCloneRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsLock200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsLockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUnlock200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUnlockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/CreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/CreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DeleteResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DeleteTrustedIpRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DisableResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DownloadResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DynamicSecretsRevokeLease200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnableResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsRename200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsRenameRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/Format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GetUserResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/GroupsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsDeleteResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/InvitesListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IssueLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/IssueLeaseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ListPermissionsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ListTrustedIpsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/LockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/LockResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/MeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/MemberResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/MemberType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/NameTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/NamesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/OptionsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesListPermissionsResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RenameRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RenameResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RetrieveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RevokeLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RevokeLeaseResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RevokeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/RollbackResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsDownload200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsListNames200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateNote200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateNoteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountTokensCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountTokensCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountTokensGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountTokensListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsDeleteResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/SyncsGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UnlockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UnlockResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UpdateNoteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UpdateNoteResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UsersGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/UsersListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/V3Me200Response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksAddRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksAddResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksDeleteResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WebhooksUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesCreateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesGetResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceUpdateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.758404 doppler-sdk-1.3.0/src/dopplersdk/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/http_content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/query_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/net/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:43.762404 doppler-sdk-1.3.0/src/dopplersdk/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/config_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/dynamic_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/invites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/project_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/project_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/service_account_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/service_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/trusted_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/v_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/workplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/services/workplace_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 22:56:40.000000 doppler-sdk-1.3.0/src/dopplersdk/setup.py
```

### Comparing `doppler-sdk-1.2.1/LICENSE` & `doppler-sdk-1.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 
+Copyright (c) 2024 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `doppler-sdk-1.2.1/pyproject.toml` & `doppler-sdk-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "doppler-sdk"
-version = "1.2.1"
+version = "1.3.0"
 license = { text = "MIT" }
 description = """"""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
 	"License :: OSI Approved :: Apache Software License",
 	"Programming Language :: Python :: 3 :: Only",
 	"Operating System :: OS Independent",
 	"Topic :: Security"
 ]
 dependencies = [
 	"requests",
-	"http-exceptions",
+	"http-exceptions"
+]
+
+[project.optional-dependencies]
+test = [ 
 	"pytest",
 	"responses"
 ]
-
 [project.urls]
 Documentation = "https://docs.doppler.com/docs/sdk-python"
 Source = "https://github.com/DopplerHQ/python-sdk"
 Tracker = "https://github.com/DopplerHQ/python-sdk/issues"
 Homepage = "https://doppler.com"
```

### Comparing `doppler-sdk-1.2.1/src/doppler_sdk.egg-info/SOURCES.txt` & `doppler-sdk-1.3.0/src/doppler_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,18 +45,20 @@
 src/dopplersdk/models/ConfigsUpdateRequest.py
 src/dopplersdk/models/ConfigsUpdateResponse.py
 src/dopplersdk/models/CreateRequest.py
 src/dopplersdk/models/CreateResponse.py
 src/dopplersdk/models/DeleteRequest.py
 src/dopplersdk/models/DeleteResponse.py
 src/dopplersdk/models/DeleteTrustedIpRequest.py
+src/dopplersdk/models/DisableResponse.py
 src/dopplersdk/models/DownloadResponse.py
 src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py
 src/dopplersdk/models/DynamicSecretsRevokeLease200Response.py
 src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py
+src/dopplersdk/models/EnableResponse.py
 src/dopplersdk/models/EnvironmentsCreate200Response.py
 src/dopplersdk/models/EnvironmentsCreateRequest.py
 src/dopplersdk/models/EnvironmentsCreateResponse.py
 src/dopplersdk/models/EnvironmentsGet200Response.py
 src/dopplersdk/models/EnvironmentsGetResponse.py
 src/dopplersdk/models/EnvironmentsList200Response.py
 src/dopplersdk/models/EnvironmentsListResponse.py
@@ -88,24 +90,29 @@
 src/dopplersdk/models/IssueLeaseResponse.py
 src/dopplersdk/models/ListPermissionsResponse.py
 src/dopplersdk/models/ListResponse.py
 src/dopplersdk/models/ListTrustedIpsResponse.py
 src/dopplersdk/models/LockRequest.py
 src/dopplersdk/models/LockResponse.py
 src/dopplersdk/models/MeResponse.py
+src/dopplersdk/models/MemberResponse.py
+src/dopplersdk/models/MemberType.py
 src/dopplersdk/models/NameTransformer.py
 src/dopplersdk/models/NamesResponse.py
+src/dopplersdk/models/OptionsResponse.py
 src/dopplersdk/models/ProjectMembersGetResponse.py
 src/dopplersdk/models/ProjectMembersListResponse.py
 src/dopplersdk/models/ProjectMembersUpdateRequest.py
 src/dopplersdk/models/ProjectMembersUpdateResponse.py
+src/dopplersdk/models/ProjectRolesCreateRequest.py
 src/dopplersdk/models/ProjectRolesCreateResponse.py
 src/dopplersdk/models/ProjectRolesGetResponse.py
 src/dopplersdk/models/ProjectRolesListPermissionsResponse.py
 src/dopplersdk/models/ProjectRolesListResponse.py
+src/dopplersdk/models/ProjectRolesUpdateRequest.py
 src/dopplersdk/models/ProjectRolesUpdateResponse.py
 src/dopplersdk/models/ProjectsCreate200Response.py
 src/dopplersdk/models/ProjectsCreateRequest.py
 src/dopplersdk/models/ProjectsDeleteRequest.py
 src/dopplersdk/models/ProjectsGet200Response.py
 src/dopplersdk/models/ProjectsGetResponse.py
 src/dopplersdk/models/ProjectsList200Response.py
@@ -125,14 +132,18 @@
 src/dopplersdk/models/SecretsListNames200Response.py
 src/dopplersdk/models/SecretsListResponse.py
 src/dopplersdk/models/SecretsUpdate200Response.py
 src/dopplersdk/models/SecretsUpdateNote200Response.py
 src/dopplersdk/models/SecretsUpdateNoteRequest.py
 src/dopplersdk/models/SecretsUpdateRequest.py
 src/dopplersdk/models/SecretsUpdateResponse.py
+src/dopplersdk/models/ServiceAccountTokensCreateRequest.py
+src/dopplersdk/models/ServiceAccountTokensCreateResponse.py
+src/dopplersdk/models/ServiceAccountTokensGetResponse.py
+src/dopplersdk/models/ServiceAccountTokensListResponse.py
 src/dopplersdk/models/ServiceAccountsCreateRequest.py
 src/dopplersdk/models/ServiceAccountsCreateResponse.py
 src/dopplersdk/models/ServiceAccountsGetResponse.py
 src/dopplersdk/models/ServiceAccountsListResponse.py
 src/dopplersdk/models/ServiceAccountsUpdateRequest.py
 src/dopplersdk/models/ServiceAccountsUpdateResponse.py
 src/dopplersdk/models/ServiceTokensCreateRequest.py
@@ -153,18 +164,27 @@
 src/dopplersdk/models/UpdateNoteRequest.py
 src/dopplersdk/models/UpdateNoteResponse.py
 src/dopplersdk/models/UpdateRequest.py
 src/dopplersdk/models/UpdateResponse.py
 src/dopplersdk/models/UsersGetResponse.py
 src/dopplersdk/models/UsersListResponse.py
 src/dopplersdk/models/V3Me200Response.py
+src/dopplersdk/models/WebhooksAddRequest.py
+src/dopplersdk/models/WebhooksAddResponse.py
+src/dopplersdk/models/WebhooksDeleteResponse.py
+src/dopplersdk/models/WebhooksGetResponse.py
+src/dopplersdk/models/WebhooksListResponse.py
+src/dopplersdk/models/WebhooksUpdateRequest.py
+src/dopplersdk/models/WebhooksUpdateResponse.py
 src/dopplersdk/models/WorkplaceGetResponse.py
+src/dopplersdk/models/WorkplaceRolesCreateRequest.py
 src/dopplersdk/models/WorkplaceRolesCreateResponse.py
 src/dopplersdk/models/WorkplaceRolesGetResponse.py
 src/dopplersdk/models/WorkplaceRolesListResponse.py
+src/dopplersdk/models/WorkplaceRolesUpdateRequest.py
 src/dopplersdk/models/WorkplaceRolesUpdateResponse.py
 src/dopplersdk/models/WorkplaceUpdateRequest.py
 src/dopplersdk/models/WorkplaceUpdateResponse.py
 src/dopplersdk/models/__init__.py
 src/dopplersdk/models/base.py
 src/dopplersdk/net/__init__.py
 src/dopplersdk/net/environment.py
@@ -177,22 +197,26 @@
 src/dopplersdk/services/audit.py
 src/dopplersdk/services/auth.py
 src/dopplersdk/services/base.py
 src/dopplersdk/services/config_logs.py
 src/dopplersdk/services/configs.py
 src/dopplersdk/services/dynamic_secrets.py
 src/dopplersdk/services/environments.py
+src/dopplersdk/services/get.py
 src/dopplersdk/services/groups.py
 src/dopplersdk/services/integrations.py
 src/dopplersdk/services/invites.py
 src/dopplersdk/services/project_members.py
 src/dopplersdk/services/project_roles.py
 src/dopplersdk/services/projects.py
+src/dopplersdk/services/retrieve.py
 src/dopplersdk/services/secrets.py
+src/dopplersdk/services/service_account_tokens.py
 src/dopplersdk/services/service_accounts.py
 src/dopplersdk/services/service_tokens.py
 src/dopplersdk/services/syncs.py
 src/dopplersdk/services/trusted_ips.py
 src/dopplersdk/services/users.py
 src/dopplersdk/services/v_3.py
+src/dopplersdk/services/webhooks.py
 src/dopplersdk/services/workplace.py
 src/dopplersdk/services/workplace_roles.py
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsList200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ActivityLogsRetrieve200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ActivityLogsRetrieve200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/AddMemberRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/AddMemberRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .base import BaseModel
 from enum import Enum
 
 
-class Type(Enum):
+class Type_(Enum):
     WORKPLACE_USER = "workplace_user"
 
     def list():
-        return list(map(lambda x: x.value, Type._member_map_.values()))
+        return list(map(lambda x: x.value, Type_._member_map_.values()))
 
 
 class AddMemberRequest(BaseModel):
-    def __init__(self, type_: Type, slug: str, **kwargs):
+    def __init__(self, type_: Type_, slug: str, **kwargs):
         """
         Initialize AddMemberRequest
         Parameters:
         ----------
             type_: str
             slug: str
                 The member's slug
         """
-        self.type_ = self._enum_matching(type_, Type.list(), "type_")
+        self.type_ = self._enum_matching(type_, Type_.list(), "type_")
         self.slug = slug
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/AddRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/AddRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .base import BaseModel
 from typing import List
 from enum import Enum
 
 
-class Type(Enum):
+class Type_(Enum):
     WORKPLACE_USER = "workplace_user"
     GROUP = "group"
     INVITE = "invite"
     SERVICE_ACCOUNT = "service_account"
 
     def list():
-        return list(map(lambda x: x.value, Type._member_map_.values()))
+        return list(map(lambda x: x.value, Type_._member_map_.values()))
 
 
 class AddRequest(BaseModel):
     def __init__(
         self,
-        type_: Type,
+        type_: Type_,
         slug: str,
         role: str = None,
         environments: List[str] = None,
         **kwargs,
     ):
         """
         Initialize AddRequest
@@ -30,11 +30,11 @@
             slug: str
                 Member's slug
             role: str
                 Identifier of the project role
             environments: list of AddRequestEnvironments
                 Environment slugs to grant the member access to
         """
-        self.type_ = self._enum_matching(type_, Type.list(), "type_")
+        self.type_ = self._enum_matching(type_, Type_.list(), "type_")
         self.slug = slug
         self.role = role
         self.environments = environments
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/AddResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/AddResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/CloneRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/CloneRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/CloneResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/CloneResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsGet200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsList200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigLogsRollback200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigLogsRollback200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsClone200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsClone200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCloneRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCloneRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsGet200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsList200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsLock200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsLock200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUnlock200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUnlock200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ConfigsUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ConfigsUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/CreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/CreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/DownloadResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/DownloadResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsCreate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsGet200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsList200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/EnvironmentsRename200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/EnvironmentsRename200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/RollbackResponse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .base import BaseModel
 from typing import List
 
 
 class LogDiff(BaseModel):
-    def __init__(self, name: str = None, added: str = None, **kwargs):
+    def __init__(self, name: str = None, removed: str = None, **kwargs):
         """
         Initialize LogDiff
         Parameters:
         ----------
             name: str
-            added: str
+            removed: str
         """
         self.name = name
-        self.added = added
+        self.removed = removed
 
 
 class User(BaseModel):
     def __init__(
         self,
         email: str = None,
         name: str = None,
@@ -77,16 +77,16 @@
         self.created_at = created_at
         self.config = config
         self.environment = environment
         self.project = project
         self.user = user
 
 
-class GetResponse(BaseModel):
+class RollbackResponse(BaseModel):
     def __init__(self, log: Log = None, **kwargs):
         """
-        Initialize GetResponse
+        Initialize RollbackResponse
         Parameters:
         ----------
             log: Log
         """
         self.log = log
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GetUserResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/GetUserResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GroupsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/GroupsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GroupsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/GroupsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GroupsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/GroupsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/GroupsUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/GroupsUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsCreateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IntegrationsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IntegrationsListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/InvitesListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/InvitesListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IssueLeaseRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IssueLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/IssueLeaseResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/IssueLeaseResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/LockResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/LockResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/MeResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/MeResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersUpdateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectMembersUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectMembersUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectRolesUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectRolesUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsCreate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsGet200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsList200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ProjectsUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ProjectsUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/RenameResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/RenameResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/RetrieveResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/RetrieveResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/RevokeLeaseRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/RevokeLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/RollbackResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsGetResponse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,67 @@
 from .base import BaseModel
 from typing import List
 
 
-class LogDiff(BaseModel):
-    def __init__(self, name: str = None, removed: str = None, **kwargs):
-        """
-        Initialize LogDiff
-        Parameters:
-        ----------
-            name: str
-            removed: str
-        """
-        self.name = name
-        self.removed = removed
-
-
-class User(BaseModel):
+class WorkplaceRole(BaseModel):
     def __init__(
         self,
-        email: str = None,
         name: str = None,
-        username: str = None,
-        profile_image_url: str = None,
+        permissions: List[str] = None,
+        identifier: str = None,
+        created_at: str = None,
+        is_custom_role: bool = None,
+        is_inline_role: bool = None,
         **kwargs,
     ):
         """
-        Initialize User
+        Initialize WorkplaceRole
         Parameters:
         ----------
-            email: str
             name: str
-            username: str
-            profile_image_url: str
+            permissions: list of WorkplaceRolePermissions
+            identifier: str
+            created_at: str
+            is_custom_role: bool
+            is_inline_role: bool
         """
-        self.email = email
         self.name = name
-        self.username = username
-        self.profile_image_url = profile_image_url
+        self.permissions = permissions
+        self.identifier = identifier
+        self.created_at = created_at
+        self.is_custom_role = is_custom_role
+        self.is_inline_role = is_inline_role
 
 
-class Log(BaseModel):
+class ServiceAccount(BaseModel):
     def __init__(
         self,
-        id: str = None,
-        text: str = None,
-        html: str = None,
-        diff: List[LogDiff] = None,
-        rollback: bool = None,
+        name: str = None,
+        slug: str = None,
         created_at: str = None,
-        config: str = None,
-        environment: str = None,
-        project: str = None,
-        user: User = None,
+        workplace_role: WorkplaceRole = None,
         **kwargs,
     ):
         """
-        Initialize Log
+        Initialize ServiceAccount
         Parameters:
         ----------
-            id: str
-            text: str
-            html: str
-            diff: list of LogDiff
-            rollback: bool
+            name: str
+            slug: str
             created_at: str
-            config: str
-            environment: str
-            project: str
-            user: User
-        """
-        self.id = id
-        self.text = text
-        self.html = html
-        self.diff = diff
-        self.rollback = rollback
+            workplace_role: WorkplaceRole
+        """
+        self.name = name
+        self.slug = slug
         self.created_at = created_at
-        self.config = config
-        self.environment = environment
-        self.project = project
-        self.user = user
+        self.workplace_role = workplace_role
 
 
-class RollbackResponse(BaseModel):
-    def __init__(self, log: Log = None, **kwargs):
+class ServiceAccountsGetResponse(BaseModel):
+    def __init__(self, service_account: ServiceAccount = None, **kwargs):
         """
-        Initialize RollbackResponse
+        Initialize ServiceAccountsGetResponse
         Parameters:
         ----------
-            log: Log
+            service_account: ServiceAccount
         """
-        self.log = log
+        self.service_account = service_account
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsDownload200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsDownload200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsGet200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateResponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -48,57 +48,37 @@
             note: str
         """
         self.raw = raw
         self.computed = computed
         self.note = note
 
 
-class User(BaseModel):
-    def __init__(
-        self, raw: str = None, computed: str = None, note: str = None, **kwargs
-    ):
-        """
-        Initialize User
-        Parameters:
-        ----------
-            raw: str
-            computed: str
-            note: str
-        """
-        self.raw = raw
-        self.computed = computed
-        self.note = note
-
-
 class Secrets(BaseModel):
     def __init__(
         self,
         STRIPE: Stripe = None,
         ALGOLIA: Algolia = None,
         DATABASE: Database = None,
-        USER: User = None,
         **kwargs,
     ):
         """
         Initialize Secrets
         Parameters:
         ----------
             STRIPE: Stripe
             ALGOLIA: Algolia
             DATABASE: Database
-            USER: User
         """
         self.STRIPE = STRIPE
         self.ALGOLIA = ALGOLIA
         self.DATABASE = DATABASE
-        self.USER = USER
 
 
-class SecretsListResponse(BaseModel):
+class SecretsUpdateResponse(BaseModel):
     def __init__(self, secrets: Secrets = None, **kwargs):
         """
-        Initialize SecretsListResponse
+        Initialize SecretsUpdateResponse
         Parameters:
         ----------
             secrets: Secrets
         """
         self.secrets = secrets
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdate200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateNoteRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SecretsUpdateNoteRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SecretsUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsUpdateResponse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,66 @@
 from .base import BaseModel
 
 
-class Stripe(BaseModel):
+class WorkplaceRole(BaseModel):
     def __init__(
-        self, raw: str = None, computed: str = None, note: str = None, **kwargs
-    ):
-        """
-        Initialize Stripe
-        Parameters:
-        ----------
-            raw: str
-            computed: str
-            note: str
-        """
-        self.raw = raw
-        self.computed = computed
-        self.note = note
-
-
-class Algolia(BaseModel):
-    def __init__(
-        self, raw: str = None, computed: str = None, note: str = None, **kwargs
-    ):
-        """
-        Initialize Algolia
-        Parameters:
-        ----------
-            raw: str
-            computed: str
-            note: str
-        """
-        self.raw = raw
-        self.computed = computed
-        self.note = note
-
-
-class Database(BaseModel):
-    def __init__(
-        self, raw: str = None, computed: str = None, note: str = None, **kwargs
+        self,
+        name: str = None,
+        permissions: list = None,
+        identifier: str = None,
+        created_at: str = None,
+        is_custom_role: bool = None,
+        is_inline_role: bool = None,
+        **kwargs,
     ):
         """
-        Initialize Database
+        Initialize WorkplaceRole
         Parameters:
         ----------
-            raw: str
-            computed: str
-            note: str
-        """
-        self.raw = raw
-        self.computed = computed
-        self.note = note
+            name: str
+            permissions: list of objects
+            identifier: str
+            created_at: str
+            is_custom_role: bool
+            is_inline_role: bool
+        """
+        self.name = name
+        self.permissions = permissions
+        self.identifier = identifier
+        self.created_at = created_at
+        self.is_custom_role = is_custom_role
+        self.is_inline_role = is_inline_role
 
 
-class Secrets(BaseModel):
+class ServiceAccount(BaseModel):
     def __init__(
         self,
-        STRIPE: Stripe = None,
-        ALGOLIA: Algolia = None,
-        DATABASE: Database = None,
+        name: str = None,
+        slug: str = None,
+        created_at: str = None,
+        workplace_role: WorkplaceRole = None,
         **kwargs,
     ):
         """
-        Initialize Secrets
+        Initialize ServiceAccount
         Parameters:
         ----------
-            STRIPE: Stripe
-            ALGOLIA: Algolia
-            DATABASE: Database
+            name: str
+            slug: str
+            created_at: str
+            workplace_role: WorkplaceRole
         """
-        self.STRIPE = STRIPE
-        self.ALGOLIA = ALGOLIA
-        self.DATABASE = DATABASE
+        self.name = name
+        self.slug = slug
+        self.created_at = created_at
+        self.workplace_role = workplace_role
 
 
-class SecretsUpdateResponse(BaseModel):
-    def __init__(self, secrets: Secrets = None, **kwargs):
+class ServiceAccountsUpdateResponse(BaseModel):
+    def __init__(self, service_account: ServiceAccount = None, **kwargs):
         """
-        Initialize SecretsUpdateResponse
+        Initialize ServiceAccountsUpdateResponse
         Parameters:
         ----------
-            secrets: Secrets
+            service_account: ServiceAccount
         """
-        self.secrets = secrets
+        self.service_account = service_account
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsCreateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsListResponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,40 +28,44 @@
         self.permissions = permissions
         self.identifier = identifier
         self.created_at = created_at
         self.is_custom_role = is_custom_role
         self.is_inline_role = is_inline_role
 
 
-class ServiceAccount(BaseModel):
+class ServiceAccountsListResponseServiceAccounts(BaseModel):
     def __init__(
         self,
         name: str = None,
         slug: str = None,
         created_at: str = None,
         workplace_role: WorkplaceRole = None,
         **kwargs,
     ):
         """
-        Initialize ServiceAccount
+        Initialize ServiceAccountsListResponseServiceAccounts
         Parameters:
         ----------
             name: str
             slug: str
             created_at: str
             workplace_role: WorkplaceRole
         """
         self.name = name
         self.slug = slug
         self.created_at = created_at
         self.workplace_role = workplace_role
 
 
-class ServiceAccountsGetResponse(BaseModel):
-    def __init__(self, service_account: ServiceAccount = None, **kwargs):
+class ServiceAccountsListResponse(BaseModel):
+    def __init__(
+        self,
+        service_accounts: List[ServiceAccountsListResponseServiceAccounts] = None,
+        **kwargs,
+    ):
         """
-        Initialize ServiceAccountsGetResponse
+        Initialize ServiceAccountsListResponse
         Parameters:
         ----------
-            service_account: ServiceAccount
+            service_accounts: list of ServiceAccountsListResponseServiceAccounts
         """
-        self.service_account = service_account
+        self.service_accounts = service_accounts
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/UsersListResponse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from .base import BaseModel
 from typing import List
 
 
-class WorkplaceRole(BaseModel):
+class User(BaseModel):
     def __init__(
         self,
+        email: str = None,
         name: str = None,
-        permissions: List[str] = None,
-        identifier: str = None,
-        created_at: str = None,
-        is_custom_role: bool = None,
-        is_inline_role: bool = None,
+        username: str = None,
+        profile_image_url: str = None,
         **kwargs,
     ):
         """
-        Initialize WorkplaceRole
+        Initialize User
         Parameters:
         ----------
+            email: str
             name: str
-            permissions: list of WorkplaceRolePermissions
-            identifier: str
-            created_at: str
-            is_custom_role: bool
-            is_inline_role: bool
+            username: str
+            profile_image_url: str
         """
+        self.email = email
         self.name = name
-        self.permissions = permissions
-        self.identifier = identifier
-        self.created_at = created_at
-        self.is_custom_role = is_custom_role
-        self.is_inline_role = is_inline_role
+        self.username = username
+        self.profile_image_url = profile_image_url
 
 
-class ServiceAccountsListResponseServiceAccounts(BaseModel):
+class UsersListResponseWorkplaceUsers(BaseModel):
     def __init__(
         self,
-        name: str = None,
-        slug: str = None,
+        id: str = None,
+        access: str = None,
         created_at: str = None,
-        workplace_role: WorkplaceRole = None,
+        user: User = None,
         **kwargs,
     ):
         """
-        Initialize ServiceAccountsListResponseServiceAccounts
+        Initialize UsersListResponseWorkplaceUsers
         Parameters:
         ----------
-            name: str
-            slug: str
+            id: str
+            access: str
             created_at: str
-            workplace_role: WorkplaceRole
+            user: User
         """
-        self.name = name
-        self.slug = slug
+        self.id = id
+        self.access = access
         self.created_at = created_at
-        self.workplace_role = workplace_role
+        self.user = user
 
 
-class ServiceAccountsListResponse(BaseModel):
+class UsersListResponse(BaseModel):
     def __init__(
         self,
-        service_accounts: List[ServiceAccountsListResponseServiceAccounts] = None,
+        workplace_users: List[UsersListResponseWorkplaceUsers] = None,
+        page: int = None,
+        success: bool = None,
         **kwargs,
     ):
         """
-        Initialize ServiceAccountsListResponse
+        Initialize UsersListResponse
         Parameters:
         ----------
-            service_accounts: list of ServiceAccountsListResponseServiceAccounts
-        """
-        self.service_accounts = service_accounts
+            workplace_users: list of UsersListResponseWorkplaceUsers
+            page: int
+            success: bool
+        """
+        self.workplace_users = workplace_users
+        self.page = page
+        self.success = success
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsUpdateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceAccountsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceAccountsUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesListResponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,43 @@
 from .base import BaseModel
+from typing import List
 
 
-class WorkplaceRole(BaseModel):
+class WorkplaceRolesListResponseRoles(BaseModel):
     def __init__(
         self,
         name: str = None,
-        permissions: list = None,
+        permissions: List[str] = None,
         identifier: str = None,
         created_at: str = None,
         is_custom_role: bool = None,
         is_inline_role: bool = None,
         **kwargs,
     ):
         """
-        Initialize WorkplaceRole
+        Initialize WorkplaceRolesListResponseRoles
         Parameters:
         ----------
             name: str
-            permissions: list of objects
+            permissions: list of WorkplaceRolesListResponseRolesPermissions
             identifier: str
             created_at: str
             is_custom_role: bool
             is_inline_role: bool
         """
         self.name = name
         self.permissions = permissions
         self.identifier = identifier
         self.created_at = created_at
         self.is_custom_role = is_custom_role
         self.is_inline_role = is_inline_role
 
 
-class ServiceAccount(BaseModel):
-    def __init__(
-        self,
-        name: str = None,
-        slug: str = None,
-        created_at: str = None,
-        workplace_role: WorkplaceRole = None,
-        **kwargs,
-    ):
-        """
-        Initialize ServiceAccount
-        Parameters:
-        ----------
-            name: str
-            slug: str
-            created_at: str
-            workplace_role: WorkplaceRole
-        """
-        self.name = name
-        self.slug = slug
-        self.created_at = created_at
-        self.workplace_role = workplace_role
-
-
-class ServiceAccountsUpdateResponse(BaseModel):
-    def __init__(self, service_account: ServiceAccount = None, **kwargs):
+class WorkplaceRolesListResponse(BaseModel):
+    def __init__(self, roles: List[WorkplaceRolesListResponseRoles] = None, **kwargs):
         """
-        Initialize ServiceAccountsUpdateResponse
+        Initialize WorkplaceRolesListResponse
         Parameters:
         ----------
-            service_account: ServiceAccount
+            roles: list of WorkplaceRolesListResponseRoles
         """
-        self.service_account = service_account
+        self.roles = roles
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensCreateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensDeleteRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensDeleteRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/ServiceTokensListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/ServiceTokensListResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SyncsCreateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SyncsCreateRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,27 +18,35 @@
 
     def list():
         return list(map(lambda x: x.value, ImportOption._member_map_.values()))
 
 
 class SyncsCreateRequest(BaseModel):
     def __init__(
-        self, data: Data, integration: str, import_option: ImportOption = None, **kwargs
+        self,
+        data: Data,
+        integration: str,
+        import_option: ImportOption = None,
+        await_initial_sync: bool = None,
+        **kwargs,
     ):
         """
         Initialize SyncsCreateRequest
         Parameters:
         ----------
             data: Data
                 Configuration data for the sync
             integration: str
                 The integration slug which the sync will use
             import_option: str
                 An option indicating if and how Doppler should attempt to import secrets from the sync destination
+            await_initial_sync: bool
+                Causes sync creation to wait for the initial sync to complete before returning.
         """
         self.data = data
         self.integration = integration
         self.import_option = (
             self._enum_matching(import_option, ImportOption.list(), "import_option")
             if import_option
             else None
         )
+        self.await_initial_sync = await_initial_sync
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SyncsCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SyncsCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/SyncsGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/SyncsGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/UnlockResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/UnlockResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/UpdateNoteRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/UpdateNoteRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from .base import BaseModel
 
 
 class UpdateNoteRequest(BaseModel):
-    def __init__(self, note: str, secret: str, config: str, project: str, **kwargs):
+    def __init__(
+        self, note: str, secret: str, project: str, config: str = None, **kwargs
+    ):
         """
         Initialize UpdateNoteRequest
         Parameters:
         ----------
             note: str
+                The note you want to set on the secret. This note will be applied to the specified secret in all environments.
             secret: str
-            config: str
-                Name of the config object.
+                The name of the secret
             project: str
                 Unique identifier for the project object.
+            config: str
+                Deprecated: Config is no longer required as notes have always been set at the project level.
         """
         self.note = note
         self.secret = secret
-        self.config = config
         self.project = project
+        self.config = config
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/UsersGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/UsersGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/UsersListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/MemberResponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,93 @@
 from .base import BaseModel
 from typing import List
 
 
-class User(BaseModel):
-    def __init__(
-        self,
-        email: str = None,
-        name: str = None,
-        username: str = None,
-        profile_image_url: str = None,
-        **kwargs,
-    ):
+class DefaultProjectRole(BaseModel):
+    def __init__(self, identifier: str = None, **kwargs):
+        """
+        Initialize DefaultProjectRole
+        Parameters:
+        ----------
+            identifier: str
+        """
+        self.identifier = identifier
+
+
+class Role(BaseModel):
+    def __init__(self, identifier: str = None, **kwargs):
+        """
+        Initialize Role
+        Parameters:
+        ----------
+            identifier: str
+        """
+        self.identifier = identifier
+
+
+class GroupProjects(BaseModel):
+    def __init__(self, name: str = None, slug: str = None, role: Role = None, **kwargs):
         """
-        Initialize User
+        Initialize GroupProjects
         Parameters:
         ----------
-            email: str
             name: str
-            username: str
-            profile_image_url: str
+            slug: str
+            role: Role
         """
-        self.email = email
         self.name = name
-        self.username = username
-        self.profile_image_url = profile_image_url
+        self.slug = slug
+        self.role = role
+
+
+class GroupMembers(BaseModel):
+    def __init__(self, slug: str = None, type_: str = None, **kwargs):
+        """
+        Initialize GroupMembers
+        Parameters:
+        ----------
+            slug: str
+            type_: str
+        """
+        self.slug = slug
+        self.type_ = type_
 
 
-class UsersListResponseWorkplaceUsers(BaseModel):
+class Group(BaseModel):
     def __init__(
         self,
-        id: str = None,
-        access: str = None,
+        name: str = None,
+        slug: str = None,
         created_at: str = None,
-        user: User = None,
+        default_project_role: DefaultProjectRole = None,
+        projects: List[GroupProjects] = None,
+        members: List[GroupMembers] = None,
         **kwargs,
     ):
         """
-        Initialize UsersListResponseWorkplaceUsers
+        Initialize Group
         Parameters:
         ----------
-            id: str
-            access: str
+            name: str
+            slug: str
             created_at: str
-            user: User
+            default_project_role: DefaultProjectRole
+            projects: list of GroupProjects
+            members: list of GroupMembers
         """
-        self.id = id
-        self.access = access
+        self.name = name
+        self.slug = slug
         self.created_at = created_at
-        self.user = user
+        self.default_project_role = default_project_role
+        self.projects = projects
+        self.members = members
 
 
-class UsersListResponse(BaseModel):
-    def __init__(
-        self,
-        workplace_users: List[UsersListResponseWorkplaceUsers] = None,
-        page: int = None,
-        success: bool = None,
-        **kwargs,
-    ):
+class MemberResponse(BaseModel):
+    def __init__(self, group: Group = None, **kwargs):
         """
-        Initialize UsersListResponse
+        Initialize MemberResponse
         Parameters:
         ----------
-            workplace_users: list of UsersListResponseWorkplaceUsers
-            page: int
-            success: bool
+            group: Group
         """
-        self.workplace_users = workplace_users
-        self.page = page
-        self.success = success
+        self.group = group
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/V3Me200Response.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/V3Me200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesCreateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesCreateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesGetResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesGetResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesListResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceRolesUpdateResponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from .base import BaseModel
 from typing import List
 
 
-class WorkplaceRolesListResponseRoles(BaseModel):
+class Role(BaseModel):
     def __init__(
         self,
         name: str = None,
         permissions: List[str] = None,
         identifier: str = None,
         created_at: str = None,
         is_custom_role: bool = None,
         is_inline_role: bool = None,
         **kwargs,
     ):
         """
-        Initialize WorkplaceRolesListResponseRoles
+        Initialize Role
         Parameters:
         ----------
             name: str
-            permissions: list of WorkplaceRolesListResponseRolesPermissions
+            permissions: list of RolePermissions
             identifier: str
             created_at: str
             is_custom_role: bool
             is_inline_role: bool
         """
         self.name = name
         self.permissions = permissions
         self.identifier = identifier
         self.created_at = created_at
         self.is_custom_role = is_custom_role
         self.is_inline_role = is_inline_role
 
 
-class WorkplaceRolesListResponse(BaseModel):
-    def __init__(self, roles: List[WorkplaceRolesListResponseRoles] = None, **kwargs):
+class WorkplaceRolesUpdateResponse(BaseModel):
+    def __init__(self, role: Role = None, **kwargs):
         """
-        Initialize WorkplaceRolesListResponse
+        Initialize WorkplaceRolesUpdateResponse
         Parameters:
         ----------
-            roles: list of WorkplaceRolesListResponseRoles
+            role: Role
         """
-        self.roles = roles
+        self.role = role
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceRolesUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/UpdateResponse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from .base import BaseModel
-from typing import List
 
 
-class Role(BaseModel):
+class Project(BaseModel):
     def __init__(
         self,
+        id: str = None,
         name: str = None,
-        permissions: List[str] = None,
-        identifier: str = None,
+        description: str = None,
         created_at: str = None,
-        is_custom_role: bool = None,
-        is_inline_role: bool = None,
         **kwargs,
     ):
         """
-        Initialize Role
+        Initialize Project
         Parameters:
         ----------
+            id: str
             name: str
-            permissions: list of RolePermissions
-            identifier: str
+            description: str
             created_at: str
-            is_custom_role: bool
-            is_inline_role: bool
         """
+        self.id = id
         self.name = name
-        self.permissions = permissions
-        self.identifier = identifier
+        self.description = description
         self.created_at = created_at
-        self.is_custom_role = is_custom_role
-        self.is_inline_role = is_inline_role
 
 
-class WorkplaceRolesUpdateResponse(BaseModel):
-    def __init__(self, role: Role = None, **kwargs):
+class UpdateResponse(BaseModel):
+    def __init__(self, project: Project = None, **kwargs):
         """
-        Initialize WorkplaceRolesUpdateResponse
+        Initialize UpdateResponse
         Parameters:
         ----------
-            role: Role
+            project: Project
         """
-        self.role = role
+        self.project = project
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceUpdateRequest.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/WorkplaceUpdateResponse.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/WorkplaceUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/__init__.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,125 @@
 from .Format import Format
 from .NameTransformer import NameTransformer
 from .Type import Type
 from .GroupsType import GroupsType
+from .MemberType import MemberType
 from .ListResponse import ListResponse
 from .CreateResponse import CreateResponse
-from .SecretsListResponse import SecretsListResponse
-from .UpdateResponse import UpdateResponse
-from .ConfigLogsListResponse import ConfigLogsListResponse
+from .EnvironmentsListResponse import EnvironmentsListResponse
+from .EnvironmentsCreateResponse import EnvironmentsCreateResponse
 from .GetResponse import GetResponse
+from .UpdateResponse import UpdateResponse
+from .ConfigsGetResponse import ConfigsGetResponse
+from .ConfigsUpdateResponse import ConfigsUpdateResponse
+from .DeleteResponse import DeleteResponse
 from .EnvironmentsGetResponse import EnvironmentsGetResponse
 from .RenameResponse import RenameResponse
-from .ProjectsGetResponse import ProjectsGetResponse
-from .ProjectsUpdateResponse import ProjectsUpdateResponse
 from .ConfigsListResponse import ConfigsListResponse
 from .ConfigsCreateResponse import ConfigsCreateResponse
-from .ConfigsGetResponse import ConfigsGetResponse
-from .ConfigsUpdateResponse import ConfigsUpdateResponse
-from .DeleteResponse import DeleteResponse
-from .EnvironmentsListResponse import EnvironmentsListResponse
-from .EnvironmentsCreateResponse import EnvironmentsCreateResponse
-from .RollbackResponse import RollbackResponse
-from .RetrieveResponse import RetrieveResponse
+from .ConfigLogsGetResponse import ConfigLogsGetResponse
+from .ConfigLogsListResponse import ConfigLogsListResponse
+from .SecretsListResponse import SecretsListResponse
+from .SecretsUpdateResponse import SecretsUpdateResponse
 from .WorkplaceGetResponse import WorkplaceGetResponse
 from .WorkplaceUpdateResponse import WorkplaceUpdateResponse
 from .ActivityLogsListResponse import ActivityLogsListResponse
+from .RetrieveResponse import RetrieveResponse
 from .SecretsGetResponse import SecretsGetResponse
 from .ServiceTokensListResponse import ServiceTokensListResponse
 from .ServiceTokensCreateResponse import ServiceTokensCreateResponse
+from .RollbackResponse import RollbackResponse
+from .UnlockResponse import UnlockResponse
 from .CloneResponse import CloneResponse
 from .LockResponse import LockResponse
-from .UnlockResponse import UnlockResponse
-from .GetUserResponse import GetUserResponse
 from .DownloadResponse import DownloadResponse
-from .IssueLeaseResponse import IssueLeaseResponse
+from .GetUserResponse import GetUserResponse
 from .RevokeLeaseResponse import RevokeLeaseResponse
-from .NamesResponse import NamesResponse
+from .IssueLeaseResponse import IssueLeaseResponse
 from .UpdateNoteResponse import UpdateNoteResponse
-from .IntegrationsListResponse import IntegrationsListResponse
-from .IntegrationsCreateResponse import IntegrationsCreateResponse
+from .NamesResponse import NamesResponse
 from .IntegrationsGetResponse import IntegrationsGetResponse
 from .IntegrationsUpdateResponse import IntegrationsUpdateResponse
 from .IntegrationsDeleteResponse import IntegrationsDeleteResponse
 from .SyncsCreateResponse import SyncsCreateResponse
 from .SyncsGetResponse import SyncsGetResponse
 from .SyncsDeleteResponse import SyncsDeleteResponse
 from .MeResponse import MeResponse
+from .IntegrationsListResponse import IntegrationsListResponse
+from .IntegrationsCreateResponse import IntegrationsCreateResponse
 from .ListTrustedIpsResponse import ListTrustedIpsResponse
 from .AddTrustedIpResponse import AddTrustedIpResponse
 from .WorkplaceRolesListResponse import WorkplaceRolesListResponse
 from .WorkplaceRolesCreateResponse import WorkplaceRolesCreateResponse
-from .ListPermissionsResponse import ListPermissionsResponse
 from .WorkplaceRolesGetResponse import WorkplaceRolesGetResponse
 from .WorkplaceRolesUpdateResponse import WorkplaceRolesUpdateResponse
-from .ProjectRolesListResponse import ProjectRolesListResponse
-from .ProjectRolesCreateResponse import ProjectRolesCreateResponse
 from .ProjectRolesGetResponse import ProjectRolesGetResponse
 from .ProjectRolesUpdateResponse import ProjectRolesUpdateResponse
-from .ProjectRolesListPermissionsResponse import ProjectRolesListPermissionsResponse
+from .ListPermissionsResponse import ListPermissionsResponse
 from .ProjectMembersListResponse import ProjectMembersListResponse
 from .AddResponse import AddResponse
+from .InvitesListResponse import InvitesListResponse
+from .ProjectRolesListResponse import ProjectRolesListResponse
+from .ProjectRolesCreateResponse import ProjectRolesCreateResponse
 from .ProjectMembersGetResponse import ProjectMembersGetResponse
 from .ProjectMembersUpdateResponse import ProjectMembersUpdateResponse
-from .InvitesListResponse import InvitesListResponse
-from .ServiceAccountsListResponse import ServiceAccountsListResponse
-from .ServiceAccountsCreateResponse import ServiceAccountsCreateResponse
 from .ServiceAccountsGetResponse import ServiceAccountsGetResponse
 from .ServiceAccountsUpdateResponse import ServiceAccountsUpdateResponse
-from .GroupsListResponse import GroupsListResponse
-from .GroupsCreateResponse import GroupsCreateResponse
+from .ProjectRolesListPermissionsResponse import ProjectRolesListPermissionsResponse
 from .GroupsGetResponse import GroupsGetResponse
 from .GroupsUpdateResponse import GroupsUpdateResponse
+from .ServiceAccountsListResponse import ServiceAccountsListResponse
+from .ServiceAccountsCreateResponse import ServiceAccountsCreateResponse
+from .GroupsListResponse import GroupsListResponse
+from .GroupsCreateResponse import GroupsCreateResponse
 from .UsersListResponse import UsersListResponse
 from .UsersGetResponse import UsersGetResponse
+from .OptionsResponse import OptionsResponse
+from .MemberResponse import MemberResponse
+from .WebhooksListResponse import WebhooksListResponse
+from .WebhooksAddResponse import WebhooksAddResponse
+from .WebhooksGetResponse import WebhooksGetResponse
+from .WebhooksUpdateResponse import WebhooksUpdateResponse
+from .WebhooksDeleteResponse import WebhooksDeleteResponse
+from .EnableResponse import EnableResponse
+from .DisableResponse import DisableResponse
+from .ServiceAccountTokensListResponse import ServiceAccountTokensListResponse
+from .ServiceAccountTokensCreateResponse import ServiceAccountTokensCreateResponse
+from .ServiceAccountTokensGetResponse import ServiceAccountTokensGetResponse
 from .CreateRequest import CreateRequest
+from .EnvironmentsCreateRequest import EnvironmentsCreateRequest
 from .UpdateRequest import UpdateRequest
-from .RenameRequest import RenameRequest
-from .ProjectsUpdateRequest import ProjectsUpdateRequest
 from .DeleteRequest import DeleteRequest
-from .ConfigsCreateRequest import ConfigsCreateRequest
 from .ConfigsUpdateRequest import ConfigsUpdateRequest
 from .ConfigsDeleteRequest import ConfigsDeleteRequest
-from .EnvironmentsCreateRequest import EnvironmentsCreateRequest
+from .RenameRequest import RenameRequest
+from .ConfigsCreateRequest import ConfigsCreateRequest
+from .SecretsUpdateRequest import SecretsUpdateRequest
 from .WorkplaceUpdateRequest import WorkplaceUpdateRequest
-from .ServiceTokensCreateRequest import ServiceTokensCreateRequest
 from .ServiceTokensDeleteRequest import ServiceTokensDeleteRequest
+from .ServiceTokensCreateRequest import ServiceTokensCreateRequest
+from .UnlockRequest import UnlockRequest
 from .CloneRequest import CloneRequest
 from .LockRequest import LockRequest
-from .UnlockRequest import UnlockRequest
-from .IssueLeaseRequest import IssueLeaseRequest
 from .RevokeLeaseRequest import RevokeLeaseRequest
 from .RevokeRequest import RevokeRequest
+from .IssueLeaseRequest import IssueLeaseRequest
 from .UpdateNoteRequest import UpdateNoteRequest
-from .IntegrationsCreateRequest import IntegrationsCreateRequest
 from .IntegrationsUpdateRequest import IntegrationsUpdateRequest
 from .SyncsCreateRequest import SyncsCreateRequest
+from .IntegrationsCreateRequest import IntegrationsCreateRequest
 from .AddTrustedIpRequest import AddTrustedIpRequest
 from .DeleteTrustedIpRequest import DeleteTrustedIpRequest
+from .WorkplaceRolesCreateRequest import WorkplaceRolesCreateRequest
+from .WorkplaceRolesUpdateRequest import WorkplaceRolesUpdateRequest
+from .ProjectRolesUpdateRequest import ProjectRolesUpdateRequest
 from .AddRequest import AddRequest
+from .ProjectRolesCreateRequest import ProjectRolesCreateRequest
 from .ProjectMembersUpdateRequest import ProjectMembersUpdateRequest
-from .ServiceAccountsCreateRequest import ServiceAccountsCreateRequest
 from .ServiceAccountsUpdateRequest import ServiceAccountsUpdateRequest
-from .GroupsCreateRequest import GroupsCreateRequest
 from .GroupsUpdateRequest import GroupsUpdateRequest
+from .ServiceAccountsCreateRequest import ServiceAccountsCreateRequest
+from .GroupsCreateRequest import GroupsCreateRequest
 from .AddMemberRequest import AddMemberRequest
+from .WebhooksAddRequest import WebhooksAddRequest
+from .WebhooksUpdateRequest import WebhooksUpdateRequest
+from .ServiceAccountTokensCreateRequest import ServiceAccountTokensCreateRequest
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/models/base.py` & `doppler-sdk-1.3.0/src/dopplersdk/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from typing import List, Union
 from enum import Enum
 
 
 class BaseModel:
     """
-    A base class that all models in the SDK inherite from (expect for Enum models).
+    A base class that all models in the SDK inherit from (expect for Enum models).
 
     Methods
     -------
     _pattern_matching(cls, value: str, pattern: str, variable_name: str) -> str:
         Checks if a value matches a regex pattern.
         Returns the value if there's a match, otherwise throws an error.
     _enum_matching(cls, value: Union[str,Enum], enum_values: List[str], variable_name: str) -> str:
         Checks if a value (str or enum) matches the required enum values.
         Returns the value if there's a match, otherwise throws an error.
     _one_of(cls, required_array, all_array, functions_array, input_data):
-        Validates wheter an input_data satisfies the oneOf requirments.
+        Validates whether an input_data satisfies the oneOf requirements.
     """
 
     def __init__(self):
         pass
 
     def _pattern_matching(cls, value: str, pattern: str, variable_name: str):
         if re.match(r"{}".format(pattern), value):
@@ -39,21 +39,22 @@
                 f"Invalid value for {variable_name}: must match one of {enum_values}"
             )
 
     @classmethod
     def _one_of(cls, required_array, all_array, functions_array, input_data):
         input_array = list(input_data.keys())
         for model, fields in required_array.items():
+            input_copy = input_array.copy()
             matches_required = True
             for param in fields:
-                if param not in input_array:
+                if param not in input_copy:
                     matches_required = False
                     break
-                input_array.remove(param)
+                input_copy.remove(param)
             if matches_required:
                 matches_all = True
-                for input in input_array:
+                for input in input_copy:
                     if input not in all_array[model]:
                         matches_all = False
                         break
                 if matches_all:
                     return functions_array[model](input_data)
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/net/http_client.py` & `doppler-sdk-1.3.0/src/dopplersdk/net/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             headers : dict
                 The http call's headers
             body_input : Any
                 The request's body
         """
         request_method = getattr(requests, method)
         serialized_body = rename_to_reserved_keys(to_serialize(body_input))
-        if "Content-type" in headers:
-            data_type, subtype = headers["Content-type"].split("/")
+        if "Content-Type" in headers:
+            data_type, subtype = headers["Content-Type"].split("/")
             if data_type == "multipart":
                 return multipart_form_data_request(
                     method, endpoint_url, headers, serialized_body
                 )
             if data_type in ["text", "image"]:
                 return request_method(
                     endpoint_url, headers=headers, data=serialized_body
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/net/http_content_types.py` & `doppler-sdk-1.3.0/src/dopplersdk/net/http_content_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Collection of API calls according to the HTTP method and content type.
 
 Functions:
     multipart_form_data_request
 """
+
 import requests
 import io
 from mimetypes import guess_type
 
 
 def multipart_form_data_request(method, endpoint_url, headers, body_input):
     """
@@ -23,15 +24,15 @@
             The http call's headers
         body_input : Any
             The request's body
     """
     data = {}
     files = {}
     request_method = getattr(requests, method)
-    del headers["Content-type"]
+    del headers["Content-Type"]
     for key, value in body_input.items():
         if isinstance(value, (io.TextIOWrapper, io.BufferedIOBase)):
             mime_type, encoding = guess_type(value.name)
             file_tuple = (
                 (value.name, value, mime_type) if mime_type else (value.name, value)
             )
             files[key] = file_tuple
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/net/query_serializer.py` & `doppler-sdk-1.3.0/src/dopplersdk/net/query_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 from typing import Any, Dict, List
+from enum import Enum
 
 explode = bool
 
 
 def simple(value: Any, explode: bool) -> str:
-    # Check if the value is a list
+    if value is None:
+        return "null"
+
+    if isinstance(value, Enum):
+        return str(value.value)
+
+    if isinstance(value, bool):
+        return str(value).lower()
+
     if isinstance(value, list):
-        return ",".join(value) if explode else "".join(value)
+        serialized_list = [simple(item, explode) for item in value]
+        return ",".join(serialized_list)
 
     if isinstance(value, dict):
         if explode:
             # Serialize object with exploded format: "key=value,key2=value2"
-            return ",".join([f"{k}={v}" for k, v in value.items()])
+            return ",".join([f"{k}={simple(v, explode)}" for k, v in value.items()])
         else:
             # Serialize object with non-exploded format: "key,value,key2,value2"
             return ",".join(
-                [str(item) for sublist in value.items() for item in sublist]
+                [simple(item, explode) for sublist in value.items() for item in sublist]
             )
 
     return str(value)
 
 
 def form(parameter_name: str, parameter_value: Any, explode: bool) -> str:
+    if isinstance(parameter_value, Enum):
+        return f"{parameter_name}=" + str(parameter_value.value)
+
     if isinstance(parameter_value, list):
         return (
             "&".join([f"{parameter_name}={v}" for v in parameter_value])
             if explode
             else f"{parameter_name}=" + ",".join([str(v) for v in parameter_value])
         )
 
@@ -52,14 +65,16 @@
     method = style_methods.get(parameter_style)
     return method(key, parameter_value, explode) if method else ""
 
 
 def serialize_header(explode: bool, parameter_value: Any):
     if not style_methods.get("simple"):
         return ""
+    if hasattr(parameter_value, "__dict__"):
+        parameter_value = parameter_value.__dict__
     return style_methods["simple"](parameter_value, explode)
 
 
 def serialize_path(
     parameter_style, explode: bool, parameter_value: Any, parameter_key=None
 ):
     method = style_methods.get(parameter_style)
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/net/utils.py` & `doppler-sdk-1.3.0/src/dopplersdk/net/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,20 @@
         obj, (io.TextIOWrapper, io.BufferedIOBase)
     ):
         return obj
     iter_obj = obj.__dict__.items() if hasattr(obj, "__dict__") else obj.items()
     for key, value in iter_obj:
         if isinstance(value, (io.TextIOWrapper, io.BufferedIOBase)):
             result[key] = value
-        if isinstance(value, Enum):
+        elif isinstance(value, Enum):
             result[key] = value.value
+        elif isinstance(value, (list, set, tuple)):
+            for i in range(len(value)):
+                value[i] = to_serialize(value[i])
+            result[key] = value
         elif hasattr(value, "__dict__"):
             result[key] = to_serialize(value)
         else:
             result[key] = value
     return result
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/sdk.py` & `doppler-sdk-1.3.0/src/dopplersdk/sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 """
 Creates a DopplerSDK class.
 Generates the main SDK with all available queries as attributes.
 
 Class:
     DopplerSDK
 """
+
 from .net.environment import Environment
-from .services.projects import Projects
-from .services.secrets import Secrets
-from .services.config_logs import ConfigLogs
-from .services.environments import Environments
-from .services.configs import Configs
+
 from .services.activity_logs import ActivityLogs
-from .services.workplace import Workplace
-from .services.service_tokens import ServiceTokens
 from .services.audit import Audit
-from .services.dynamic_secrets import DynamicSecrets
 from .services.auth import Auth
+from .services.config_logs import ConfigLogs
+from .services.configs import Configs
+from .services.dynamic_secrets import DynamicSecrets
+from .services.environments import Environments
+from .services.get import Get
+from .services.groups import Groups
 from .services.integrations import Integrations
-from .services.syncs import Syncs
-from .services.workplace_roles import WorkplaceRoles
-from .services.project_roles import ProjectRoles
-from .services.project_members import ProjectMembers
 from .services.invites import Invites
+from .services.project_members import ProjectMembers
+from .services.project_roles import ProjectRoles
+from .services.projects import Projects
+from .services.retrieve import Retrieve
+from .services.secrets import Secrets
+from .services.service_account_tokens import ServiceAccountTokens
 from .services.service_accounts import ServiceAccounts
-from .services.groups import Groups
+from .services.service_tokens import ServiceTokens
+from .services.syncs import Syncs
 from .services.users import Users
+from .services.webhooks import Webhooks
+from .services.workplace import Workplace
+from .services.workplace_roles import WorkplaceRoles
 
 
 class DopplerSDK:
     """
     A class representing the full DopplerSDK SDK
 
     Attributes
     ----------
-    projects : Projects
-    secrets : Secrets
-    config_logs : ConfigLogs
-    environments : Environments
-    configs : Configs
     activity_logs : ActivityLogs
-    workplace : Workplace
-    service_tokens : ServiceTokens
     audit : Audit
-    dynamic_secrets : DynamicSecrets
     auth : Auth
+    config_logs : ConfigLogs
+    configs : Configs
+    dynamic_secrets : DynamicSecrets
+    environments : Environments
+    get : Get
+    groups : Groups
     integrations : Integrations
-    syncs : Syncs
-    workplace_roles : WorkplaceRoles
-    project_roles : ProjectRoles
-    project_members : ProjectMembers
     invites : Invites
+    project_members : ProjectMembers
+    project_roles : ProjectRoles
+    projects : Projects
+    retrieve : Retrieve
+    secrets : Secrets
+    service_account_tokens : ServiceAccountTokens
     service_accounts : ServiceAccounts
-    groups : Groups
+    service_tokens : ServiceTokens
+    syncs : Syncs
     users : Users
+    webhooks : Webhooks
+    workplace : Workplace
+    workplace_roles : WorkplaceRoles
 
     Methods
     -------
     set_base_url(url: str)
         Sets the end URL
     set_access_token(access_token)
         Set the access token
@@ -69,89 +79,104 @@
         Parameters
         ----------
         environment: str
             The environment that the SDK is accessing
         access_token : str
             The access token
         """
-        self.projects = Projects(access_token)
-        self.secrets = Secrets(access_token)
-        self.config_logs = ConfigLogs(access_token)
-        self.environments = Environments(access_token)
-        self.configs = Configs(access_token)
         self.activity_logs = ActivityLogs(access_token)
-        self.workplace = Workplace(access_token)
-        self.service_tokens = ServiceTokens(access_token)
         self.audit = Audit(access_token)
-        self.dynamic_secrets = DynamicSecrets(access_token)
         self.auth = Auth(access_token)
+        self.config_logs = ConfigLogs(access_token)
+        self.configs = Configs(access_token)
+        self.dynamic_secrets = DynamicSecrets(access_token)
+        self.environments = Environments(access_token)
+        self.get = Get(access_token)
+        self.groups = Groups(access_token)
         self.integrations = Integrations(access_token)
-        self.syncs = Syncs(access_token)
-        self.workplace_roles = WorkplaceRoles(access_token)
-        self.project_roles = ProjectRoles(access_token)
-        self.project_members = ProjectMembers(access_token)
         self.invites = Invites(access_token)
+        self.project_members = ProjectMembers(access_token)
+        self.project_roles = ProjectRoles(access_token)
+        self.projects = Projects(access_token)
+        self.retrieve = Retrieve(access_token)
+        self.secrets = Secrets(access_token)
+        self.service_account_tokens = ServiceAccountTokens(access_token)
         self.service_accounts = ServiceAccounts(access_token)
-        self.groups = Groups(access_token)
+        self.service_tokens = ServiceTokens(access_token)
+        self.syncs = Syncs(access_token)
         self.users = Users(access_token)
+        self.webhooks = Webhooks(access_token)
+        self.workplace = Workplace(access_token)
+        self.workplace_roles = WorkplaceRoles(access_token)
 
         self.set_base_url(environment.value)
 
     def set_base_url(self, url: str) -> None:
         """
         Sets the end URL
 
         Parameters
         ----------
             url:
                 The end URL
         """
-        self.projects.set_base_url(url)
-        self.secrets.set_base_url(url)
-        self.config_logs.set_base_url(url)
-        self.environments.set_base_url(url)
-        self.configs.set_base_url(url)
         self.activity_logs.set_base_url(url)
-        self.workplace.set_base_url(url)
-        self.service_tokens.set_base_url(url)
         self.audit.set_base_url(url)
-        self.dynamic_secrets.set_base_url(url)
         self.auth.set_base_url(url)
+        self.config_logs.set_base_url(url)
+        self.configs.set_base_url(url)
+        self.dynamic_secrets.set_base_url(url)
+        self.environments.set_base_url(url)
+        self.get.set_base_url(url)
+        self.groups.set_base_url(url)
         self.integrations.set_base_url(url)
-        self.syncs.set_base_url(url)
-        self.workplace_roles.set_base_url(url)
-        self.project_roles.set_base_url(url)
-        self.project_members.set_base_url(url)
         self.invites.set_base_url(url)
+        self.project_members.set_base_url(url)
+        self.project_roles.set_base_url(url)
+        self.projects.set_base_url(url)
+        self.retrieve.set_base_url(url)
+        self.secrets.set_base_url(url)
+        self.service_account_tokens.set_base_url(url)
         self.service_accounts.set_base_url(url)
-        self.groups.set_base_url(url)
+        self.service_tokens.set_base_url(url)
+        self.syncs.set_base_url(url)
         self.users.set_base_url(url)
+        self.webhooks.set_base_url(url)
+        self.workplace.set_base_url(url)
+        self.workplace_roles.set_base_url(url)
 
     def set_access_token(self, token: str) -> None:
         """
         Sets auth token key
 
         Parameters
         ----------
         token: string
             Auth token value
         """
-        self.projects.set_access_token(token)
-        self.secrets.set_access_token(token)
-        self.config_logs.set_access_token(token)
-        self.environments.set_access_token(token)
-        self.configs.set_access_token(token)
         self.activity_logs.set_access_token(token)
-        self.workplace.set_access_token(token)
-        self.service_tokens.set_access_token(token)
         self.audit.set_access_token(token)
-        self.dynamic_secrets.set_access_token(token)
         self.auth.set_access_token(token)
+        self.config_logs.set_access_token(token)
+        self.configs.set_access_token(token)
+        self.dynamic_secrets.set_access_token(token)
+        self.environments.set_access_token(token)
+        self.get.set_access_token(token)
+        self.groups.set_access_token(token)
         self.integrations.set_access_token(token)
-        self.syncs.set_access_token(token)
-        self.workplace_roles.set_access_token(token)
-        self.project_roles.set_access_token(token)
-        self.project_members.set_access_token(token)
         self.invites.set_access_token(token)
+        self.project_members.set_access_token(token)
+        self.project_roles.set_access_token(token)
+        self.projects.set_access_token(token)
+        self.retrieve.set_access_token(token)
+        self.secrets.set_access_token(token)
+        self.service_account_tokens.set_access_token(token)
         self.service_accounts.set_access_token(token)
-        self.groups.set_access_token(token)
+        self.service_tokens.set_access_token(token)
+        self.syncs.set_access_token(token)
         self.users.set_access_token(token)
+        self.webhooks.set_access_token(token)
+        self.workplace.set_access_token(token)
+        self.workplace_roles.set_access_token(token)
+
+
+# c029837e0e474b76bc487506e8799df5e3335891efe4fb02bda7a1441840310c
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/activity_logs.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/activity_logs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,17 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.RetrieveResponse import RetrieveResponse as RetrieveResponseModel
 from ..models.ActivityLogsListResponse import (
     ActivityLogsListResponse as ActivityLogsListResponseModel,
 )
+from ..models.RetrieveResponse import RetrieveResponse as RetrieveResponseModel
 
 
 class ActivityLogs(BaseService):
-    def retrieve(self, log: str) -> RetrieveResponseModel:
-        """
-        Retrieve
-        Parameters:
-        ----------
-            log: str
-                Unique identifier for the log object.
-        """
-
-        url_endpoint = "/v3/logs/log"
-        headers = {}
-        query_params = []
-        self._add_required_headers(headers)
-        if not log:
-            raise ValueError("Parameter log is required, cannot be empty or blank.")
-        query_params.append(query_serializer.serialize_query("form", False, "log", log))
-        final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return RetrieveResponseModel(**res)
-        return res
-
     def list(
         self, page: str = None, per_page: int = None
     ) -> ActivityLogsListResponseModel:
         """
         List
         Parameters:
         ----------
@@ -58,7 +36,29 @@
         final_url = self._url_prefix + url_endpoint
         if len(query_params) > 0:
             final_url += "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return ActivityLogsListResponseModel(**res)
         return res
+
+    def retrieve(self, log: str) -> RetrieveResponseModel:
+        """
+        Retrieve
+        Parameters:
+        ----------
+            log: str
+                Unique identifier for the log object.
+        """
+
+        url_endpoint = "/v3/logs/log"
+        headers = {}
+        query_params = []
+        self._add_required_headers(headers)
+        if not log:
+            raise ValueError("Parameter log is required, cannot be empty or blank.")
+        query_params.append(query_serializer.serialize_query("form", False, "log", log))
+        final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return RetrieveResponseModel(**res)
+        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/audit.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/audit.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/auth.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Auth(BaseService):
     def revoke(self, request_input: RevokeRequestModel = None):
         """
         Revoke
         """
 
         url_endpoint = "/v3/auth/revoke"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         return res
 
     def me(self) -> MeResponseModel:
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/base.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Creates a BaseService class.
 Performs API calls,sets authentication tokens and handles http exceptions.
 
 Class:
     BaseService
 """
+
+import platform
 from typing import List, Union
 from enum import Enum
 import re
 from ..net.http_client import HTTPClient
 
 
 class BaseService:
@@ -89,10 +91,10 @@
         Request authorization headers
 
         Parameters
         ----------
         headers: dict
             Headers dict to add auth headers to
         """
-        headers["User-Agent"] = "liblab/0.1.20 DopplerSDK/1.2.1 python/2.7"
+        headers["User-Agent"] = f"DopplerSDK/1.3.0 Python/{platform.python_version()}"
         headers["Authorization"] = f"Bearer {self._access_token}"
         return headers
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/config_logs.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/config_logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
+from ..models.ConfigLogsGetResponse import (
+    ConfigLogsGetResponse as ConfigLogsGetResponseModel,
+)
 from ..models.ConfigLogsListResponse import (
     ConfigLogsListResponse as ConfigLogsListResponseModel,
 )
-from ..models.GetResponse import GetResponse as GetResponseModel
 from ..models.RollbackResponse import RollbackResponse as RollbackResponseModel
 
 
 class ConfigLogs(BaseService):
-    def list(
-        self, config: str, project: str, page: int = None, per_page: int = None
-    ) -> ConfigLogsListResponseModel:
+    def get(self, log: str, config: str, project: str) -> ConfigLogsGetResponseModel:
         """
-        List
+        Retrieve
         Parameters:
         ----------
             project: str
                 Unique identifier for the project object.
             config: str
                 Name of the config object.
-            page: int
-                Page number
-            per_page: int
-                Items per page
+            log: str
+                Unique identifier for the log object.
         """
 
-        url_endpoint = "/v3/configs/config/logs"
+        url_endpoint = "/v3/configs/config/logs/log"
         headers = {}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
         if not config:
             raise ValueError("Parameter config is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "config", config)
         )
-        if page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "page", page)
-            )
-        if per_page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "per_page", per_page)
-            )
+        if not log:
+            raise ValueError("Parameter log is required, cannot be empty or blank.")
+        query_params.append(query_serializer.serialize_query("form", False, "log", log))
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
-            return ConfigLogsListResponseModel(**res)
+            return ConfigLogsGetResponseModel(**res)
         return res
 
-    def get(self, log: str, config: str, project: str) -> GetResponseModel:
+    def list(
+        self, config: str, project: str, page: int = None, per_page: int = None
+    ) -> ConfigLogsListResponseModel:
         """
-        Retrieve
+        List
         Parameters:
         ----------
             project: str
                 Unique identifier for the project object.
             config: str
                 Name of the config object.
-            log: str
-                Unique identifier for the log object.
+            page: int
+                Page number
+            per_page: int
+                Items per page
         """
 
-        url_endpoint = "/v3/configs/config/logs/log"
+        url_endpoint = "/v3/configs/config/logs"
         headers = {}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
         if not config:
             raise ValueError("Parameter config is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "config", config)
         )
-        if not log:
-            raise ValueError("Parameter log is required, cannot be empty or blank.")
-        query_params.append(query_serializer.serialize_query("form", False, "log", log))
+        if page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "page", page)
+            )
+        if per_page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "per_page", per_page)
+            )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
-            return GetResponseModel(**res)
+            return ConfigLogsListResponseModel(**res)
         return res
 
     def rollback(self, log: str, config: str, project: str) -> RollbackResponseModel:
         """
         Rollback
         Parameters:
         ----------
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/configs.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,112 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.ConfigsListResponse import ConfigsListResponse as ConfigsListResponseModel
-from ..models.ConfigsCreateRequest import (
-    ConfigsCreateRequest as ConfigsCreateRequestModel,
-)
-from ..models.ConfigsCreateResponse import (
-    ConfigsCreateResponse as ConfigsCreateResponseModel,
-)
 from ..models.ConfigsGetResponse import ConfigsGetResponse as ConfigsGetResponseModel
 from ..models.ConfigsUpdateRequest import (
     ConfigsUpdateRequest as ConfigsUpdateRequestModel,
 )
 from ..models.ConfigsUpdateResponse import (
     ConfigsUpdateResponse as ConfigsUpdateResponseModel,
 )
 from ..models.ConfigsDeleteRequest import (
     ConfigsDeleteRequest as ConfigsDeleteRequestModel,
 )
 from ..models.DeleteResponse import DeleteResponse as DeleteResponseModel
+from ..models.ConfigsListResponse import ConfigsListResponse as ConfigsListResponseModel
+from ..models.ConfigsCreateRequest import (
+    ConfigsCreateRequest as ConfigsCreateRequestModel,
+)
+from ..models.ConfigsCreateResponse import (
+    ConfigsCreateResponse as ConfigsCreateResponseModel,
+)
+from ..models.UnlockRequest import UnlockRequest as UnlockRequestModel
+from ..models.UnlockResponse import UnlockResponse as UnlockResponseModel
 from ..models.CloneRequest import CloneRequest as CloneRequestModel
 from ..models.CloneResponse import CloneResponse as CloneResponseModel
 from ..models.LockRequest import LockRequest as LockRequestModel
 from ..models.LockResponse import LockResponse as LockResponseModel
-from ..models.UnlockRequest import UnlockRequest as UnlockRequestModel
-from ..models.UnlockResponse import UnlockResponse as UnlockResponseModel
 from ..models.ListTrustedIpsResponse import (
     ListTrustedIpsResponse as ListTrustedIpsResponseModel,
 )
 from ..models.AddTrustedIpRequest import AddTrustedIpRequest as AddTrustedIpRequestModel
 from ..models.AddTrustedIpResponse import (
     AddTrustedIpResponse as AddTrustedIpResponseModel,
 )
 from ..models.DeleteTrustedIpRequest import (
     DeleteTrustedIpRequest as DeleteTrustedIpRequestModel,
 )
 
 
 class Configs(BaseService):
+    def get(self, config: str, project: str) -> ConfigsGetResponseModel:
+        """
+        Retrieve
+        Parameters:
+        ----------
+            project: str
+                Unique identifier for the project object.
+            config: str
+                Name of the config object.
+        """
+
+        url_endpoint = "/v3/configs/config"
+        headers = {}
+        query_params = []
+        self._add_required_headers(headers)
+        if not project:
+            raise ValueError("Parameter project is required, cannot be empty or blank.")
+        query_params.append(
+            query_serializer.serialize_query("form", False, "project", project)
+        )
+        if not config:
+            raise ValueError("Parameter config is required, cannot be empty or blank.")
+        query_params.append(
+            query_serializer.serialize_query("form", False, "config", config)
+        )
+        final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return ConfigsGetResponseModel(**res)
+        return res
+
+    def update(
+        self, request_input: ConfigsUpdateRequestModel = None
+    ) -> ConfigsUpdateResponseModel:
+        """
+        Update
+        """
+
+        url_endpoint = "/v3/configs/config"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return ConfigsUpdateResponseModel(**res)
+        return res
+
+    def delete(
+        self, request_input: ConfigsDeleteRequestModel = None
+    ) -> DeleteResponseModel:
+        """
+        Delete
+        """
+
+        url_endpoint = "/v3/configs/config"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.delete(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return DeleteResponseModel(**res)
+        return res
+
     def list(
         self,
         project: str,
         environment: str = None,
         page: int = None,
         per_page: int = None,
     ) -> ConfigsListResponseModel:
@@ -92,133 +157,68 @@
         self, request_input: ConfigsCreateRequestModel = None
     ) -> ConfigsCreateResponseModel:
         """
         Create
         """
 
         url_endpoint = "/v3/configs"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return ConfigsCreateResponseModel(**res)
         return res
 
-    def get(self, config: str, project: str) -> ConfigsGetResponseModel:
-        """
-        Retrieve
-        Parameters:
-        ----------
-            project: str
-                Unique identifier for the project object.
-            config: str
-                Name of the config object.
-        """
-
-        url_endpoint = "/v3/configs/config"
-        headers = {}
-        query_params = []
-        self._add_required_headers(headers)
-        if not project:
-            raise ValueError("Parameter project is required, cannot be empty or blank.")
-        query_params.append(
-            query_serializer.serialize_query("form", False, "project", project)
-        )
-        if not config:
-            raise ValueError("Parameter config is required, cannot be empty or blank.")
-        query_params.append(
-            query_serializer.serialize_query("form", False, "config", config)
-        )
-        final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return ConfigsGetResponseModel(**res)
-        return res
-
-    def update(
-        self, request_input: ConfigsUpdateRequestModel = None
-    ) -> ConfigsUpdateResponseModel:
+    def unlock(self, request_input: UnlockRequestModel = None) -> UnlockResponseModel:
         """
-        Update
+        Unlock
         """
 
-        url_endpoint = "/v3/configs/config"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/configs/config/unlock"
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return ConfigsUpdateResponseModel(**res)
-        return res
-
-    def delete(
-        self, request_input: ConfigsDeleteRequestModel = None
-    ) -> DeleteResponseModel:
-        """
-        Delete
-        """
-
-        url_endpoint = "/v3/configs/config"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.delete(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return DeleteResponseModel(**res)
+            return UnlockResponseModel(**res)
         return res
 
     def clone(self, request_input: CloneRequestModel = None) -> CloneResponseModel:
         """
         Clone
         """
 
         url_endpoint = "/v3/configs/config/clone"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return CloneResponseModel(**res)
         return res
 
     def lock(self, request_input: LockRequestModel = None) -> LockResponseModel:
         """
         Lock
         """
 
         url_endpoint = "/v3/configs/config/lock"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return LockResponseModel(**res)
         return res
 
-    def unlock(self, request_input: UnlockRequestModel = None) -> UnlockResponseModel:
-        """
-        Unlock
-        """
-
-        url_endpoint = "/v3/configs/config/unlock"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return UnlockResponseModel(**res)
-        return res
-
     def list_trusted_ips(
         self, config: str, project: str
     ) -> ListTrustedIpsResponseModel:
         """
         List
         Parameters:
         ----------
@@ -254,15 +254,15 @@
         Parameters:
         ----------
             project: str
             config: str
         """
 
         url_endpoint = "/v3/configs/config/trusted_ips"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
@@ -288,15 +288,15 @@
         Parameters:
         ----------
             project: str
             config: str
         """
 
         url_endpoint = "/v3/configs/config/trusted_ips"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/dynamic_secrets.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/dynamic_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from urllib.parse import quote
 
 from .base import BaseService
-from ..models.IssueLeaseRequest import IssueLeaseRequest as IssueLeaseRequestModel
-from ..models.IssueLeaseResponse import IssueLeaseResponse as IssueLeaseResponseModel
 from ..models.RevokeLeaseRequest import RevokeLeaseRequest as RevokeLeaseRequestModel
 from ..models.RevokeLeaseResponse import RevokeLeaseResponse as RevokeLeaseResponseModel
+from ..models.IssueLeaseRequest import IssueLeaseRequest as IssueLeaseRequestModel
+from ..models.IssueLeaseResponse import IssueLeaseResponse as IssueLeaseResponseModel
 
 
 class DynamicSecrets(BaseService):
-    def issue_lease(
-        self, request_input: IssueLeaseRequestModel = None
-    ) -> IssueLeaseResponseModel:
+    def revoke_lease(
+        self, request_input: RevokeLeaseRequestModel = None
+    ) -> RevokeLeaseResponseModel:
         """
-        Issue Lease
+        Revoke Lease
         """
 
-        url_endpoint = "/v3/configs/config/dynamic_secrets/dynamic_secret/leases"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/configs/config/dynamic_secrets/dynamic_secret/leases/lease"
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
+        res = self._http.delete(final_url, headers, True)
         if res and isinstance(res, dict):
-            return IssueLeaseResponseModel(**res)
+            return RevokeLeaseResponseModel(**res)
         return res
 
-    def revoke_lease(
-        self, request_input: RevokeLeaseRequestModel = None
-    ) -> RevokeLeaseResponseModel:
+    def issue_lease(
+        self, request_input: IssueLeaseRequestModel = None
+    ) -> IssueLeaseResponseModel:
         """
-        Revoke Lease
+        Issue Lease
         """
 
-        url_endpoint = "/v3/configs/config/dynamic_secrets/dynamic_secret/leases/lease"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/configs/config/dynamic_secrets/dynamic_secret/leases"
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
-        res = self._http.delete(final_url, headers, True)
+        res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return RevokeLeaseResponseModel(**res)
+            return IssueLeaseResponseModel(**res)
         return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/environments.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/environments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,98 +1,80 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.EnvironmentsGetResponse import (
-    EnvironmentsGetResponse as EnvironmentsGetResponseModel,
-)
-from ..models.RenameRequest import RenameRequest as RenameRequestModel
-from ..models.RenameResponse import RenameResponse as RenameResponseModel
 from ..models.EnvironmentsListResponse import (
     EnvironmentsListResponse as EnvironmentsListResponseModel,
 )
 from ..models.EnvironmentsCreateRequest import (
     EnvironmentsCreateRequest as EnvironmentsCreateRequestModel,
 )
 from ..models.EnvironmentsCreateResponse import (
     EnvironmentsCreateResponse as EnvironmentsCreateResponseModel,
 )
+from ..models.EnvironmentsGetResponse import (
+    EnvironmentsGetResponse as EnvironmentsGetResponseModel,
+)
+from ..models.RenameRequest import RenameRequest as RenameRequestModel
+from ..models.RenameResponse import RenameResponse as RenameResponseModel
 
 
 class Environments(BaseService):
-    def get(self, environment: str, project: str) -> EnvironmentsGetResponseModel:
+    def list(self, project: str) -> EnvironmentsListResponseModel:
         """
-        Retrieve
+        List
         Parameters:
         ----------
             project: str
                 The project's name
-            environment: str
-                The environment's slug
         """
 
-        url_endpoint = "/v3/environments/environment"
+        url_endpoint = "/v3/environments"
         headers = {}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
-        if not environment:
-            raise ValueError(
-                "Parameter environment is required, cannot be empty or blank."
-            )
-        query_params.append(
-            query_serializer.serialize_query("form", False, "environment", environment)
-        )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
-            return EnvironmentsGetResponseModel(**res)
+            return EnvironmentsListResponseModel(**res)
         return res
 
-    def rename(
-        self, environment: str, project: str, request_input: RenameRequestModel = None
-    ) -> RenameResponseModel:
+    def create(
+        self, project: str, request_input: EnvironmentsCreateRequestModel = None
+    ) -> EnvironmentsCreateResponseModel:
         """
-        Rename
+        Create
         Parameters:
         ----------
             project: str
                 The project's name
-            environment: str
-                The environment's slug
         """
 
-        url_endpoint = "/v3/environments/environment"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/environments"
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
-        if not environment:
-            raise ValueError(
-                "Parameter environment is required, cannot be empty or blank."
-            )
-        query_params.append(
-            query_serializer.serialize_query("form", False, "environment", environment)
-        )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.put(final_url, headers, request_input, True)
+        res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return RenameResponseModel(**res)
+            return EnvironmentsCreateResponseModel(**res)
         return res
 
-    def delete(self, environment: str, project: str):
+    def get(self, environment: str, project: str) -> EnvironmentsGetResponseModel:
         """
-        Delete
+        Retrieve
         Parameters:
         ----------
             project: str
                 The project's name
             environment: str
                 The environment's slug
         """
@@ -110,59 +92,77 @@
             raise ValueError(
                 "Parameter environment is required, cannot be empty or blank."
             )
         query_params.append(
             query_serializer.serialize_query("form", False, "environment", environment)
         )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.delete(final_url, headers, True)
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return EnvironmentsGetResponseModel(**res)
         return res
 
-    def list(self, project: str) -> EnvironmentsListResponseModel:
+    def rename(
+        self, environment: str, project: str, request_input: RenameRequestModel = None
+    ) -> RenameResponseModel:
         """
-        List
+        Rename
         Parameters:
         ----------
             project: str
                 The project's name
+            environment: str
+                The environment's slug
         """
 
-        url_endpoint = "/v3/environments"
-        headers = {}
+        url_endpoint = "/v3/environments/environment"
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
+        if not environment:
+            raise ValueError(
+                "Parameter environment is required, cannot be empty or blank."
+            )
+        query_params.append(
+            query_serializer.serialize_query("form", False, "environment", environment)
+        )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.get(final_url, headers, True)
+        res = self._http.put(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return EnvironmentsListResponseModel(**res)
+            return RenameResponseModel(**res)
         return res
 
-    def create(
-        self, project: str, request_input: EnvironmentsCreateRequestModel = None
-    ) -> EnvironmentsCreateResponseModel:
+    def delete(self, environment: str, project: str):
         """
-        Create
+        Delete
         Parameters:
         ----------
             project: str
                 The project's name
+            environment: str
+                The environment's slug
         """
 
-        url_endpoint = "/v3/environments"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/environments/environment"
+        headers = {}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
+        if not environment:
+            raise ValueError(
+                "Parameter environment is required, cannot be empty or blank."
+            )
+        query_params.append(
+            query_serializer.serialize_query("form", False, "environment", environment)
+        )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return EnvironmentsCreateResponseModel(**res)
+        res = self._http.delete(final_url, headers, True)
         return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/groups.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,71 +1,25 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.GroupsListResponse import GroupsListResponse as GroupsListResponseModel
-from ..models.GroupsCreateRequest import GroupsCreateRequest as GroupsCreateRequestModel
-from ..models.GroupsCreateResponse import (
-    GroupsCreateResponse as GroupsCreateResponseModel,
-)
 from ..models.GroupsGetResponse import GroupsGetResponse as GroupsGetResponseModel
 from ..models.GroupsUpdateRequest import GroupsUpdateRequest as GroupsUpdateRequestModel
 from ..models.GroupsUpdateResponse import (
     GroupsUpdateResponse as GroupsUpdateResponseModel,
 )
-from ..models.AddMemberRequest import AddMemberRequest as AddMemberRequestModel
+from ..models.GroupsListResponse import GroupsListResponse as GroupsListResponseModel
+from ..models.GroupsCreateRequest import GroupsCreateRequest as GroupsCreateRequestModel
+from ..models.GroupsCreateResponse import (
+    GroupsCreateResponse as GroupsCreateResponseModel,
+)
 from ..models.GroupsType import GroupsType as GroupsTypeModel
+from ..models.AddMemberRequest import AddMemberRequest as AddMemberRequestModel
 
 
 class Groups(BaseService):
-    def list(self, page: int = None, per_page: int = None) -> GroupsListResponseModel:
-        """
-        List
-        Parameters:
-        ----------
-            page: int
-            per_page: int
-        """
-
-        url_endpoint = "/v3/workplace/groups"
-        headers = {}
-        query_params = []
-        self._add_required_headers(headers)
-        if page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "page", page)
-            )
-        if per_page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "per_page", per_page)
-            )
-        final_url = self._url_prefix + url_endpoint
-        if len(query_params) > 0:
-            final_url += "?" + "&".join(query_params)
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return GroupsListResponseModel(**res)
-        return res
-
-    def create(
-        self, request_input: GroupsCreateRequestModel = None
-    ) -> GroupsCreateResponseModel:
-        """
-        Create
-        """
-
-        url_endpoint = "/v3/workplace/groups"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return GroupsCreateResponseModel(**res)
-        return res
-
     def get(self, slug: str) -> GroupsGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             slug: str
                 The group's slug
@@ -94,15 +48,15 @@
         Parameters:
         ----------
             slug: str
                 The group's slug
         """
 
         url_endpoint = "/v3/workplace/groups/group/{slug}"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
         if not slug:
             raise ValueError("Parameter slug is required, cannot be empty or blank.")
         url_endpoint = url_endpoint.replace(
             "{slug}",
             quote(str(query_serializer.serialize_path("simple", False, slug, None))),
         )
@@ -130,44 +84,68 @@
             "{slug}",
             quote(str(query_serializer.serialize_path("simple", False, slug, None))),
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
 
-    def add_member(self, slug: str, request_input: AddMemberRequestModel = None):
+    def list(self, page: int = None, per_page: int = None) -> GroupsListResponseModel:
         """
-        Add Member
+        List
         Parameters:
         ----------
-            slug: str
-                The group's slug
+            page: int
+            per_page: int
         """
 
-        url_endpoint = "/v3/workplace/groups/group/{slug}/members"
-        headers = {"Content-type": "application/json"}
+        url_endpoint = "/v3/workplace/groups"
+        headers = {}
+        query_params = []
         self._add_required_headers(headers)
-        if not slug:
-            raise ValueError("Parameter slug is required, cannot be empty or blank.")
-        url_endpoint = url_endpoint.replace(
-            "{slug}",
-            quote(str(query_serializer.serialize_path("simple", False, slug, None))),
-        )
+        if page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "page", page)
+            )
+        if per_page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "per_page", per_page)
+            )
+        final_url = self._url_prefix + url_endpoint
+        if len(query_params) > 0:
+            final_url += "?" + "&".join(query_params)
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return GroupsListResponseModel(**res)
+        return res
+
+    def create(
+        self, request_input: GroupsCreateRequestModel = None
+    ) -> GroupsCreateResponseModel:
+        """
+        Create
+        """
+
+        url_endpoint = "/v3/workplace/groups"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return GroupsCreateResponseModel(**res)
         return res
 
     def delete_member(self, member_slug: str, type_: GroupsTypeModel, slug: str):
         """
         Delete Member
         Parameters:
         ----------
             slug: str
                 The group's slug
-            type: GroupsType
+            type_: GroupsType
             member_slug: str
                 The member's slug
         """
 
         url_endpoint = "/v3/workplace/groups/group/{slug}/members/{type_}/{member_slug}"
         headers = {}
         self._add_required_headers(headers)
@@ -199,7 +177,29 @@
             quote(
                 str(query_serializer.serialize_path("simple", False, member_slug, None))
             ),
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
+
+    def add_member(self, slug: str, request_input: AddMemberRequestModel = None):
+        """
+        Add Member
+        Parameters:
+        ----------
+            slug: str
+                The group's slug
+        """
+
+        url_endpoint = "/v3/workplace/groups/group/{slug}/members"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+        if not slug:
+            raise ValueError("Parameter slug is required, cannot be empty or blank.")
+        url_endpoint = url_endpoint.replace(
+            "{slug}",
+            quote(str(query_serializer.serialize_path("simple", False, slug, None))),
+        )
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/integrations.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/integrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,66 +1,34 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.IntegrationsListResponse import (
-    IntegrationsListResponse as IntegrationsListResponseModel,
-)
-from ..models.IntegrationsCreateRequest import (
-    IntegrationsCreateRequest as IntegrationsCreateRequestModel,
-)
-from ..models.IntegrationsCreateResponse import (
-    IntegrationsCreateResponse as IntegrationsCreateResponseModel,
-)
 from ..models.IntegrationsGetResponse import (
     IntegrationsGetResponse as IntegrationsGetResponseModel,
 )
 from ..models.IntegrationsUpdateRequest import (
     IntegrationsUpdateRequest as IntegrationsUpdateRequestModel,
 )
 from ..models.IntegrationsUpdateResponse import (
     IntegrationsUpdateResponse as IntegrationsUpdateResponseModel,
 )
 from ..models.IntegrationsDeleteResponse import (
     IntegrationsDeleteResponse as IntegrationsDeleteResponseModel,
 )
+from ..models.IntegrationsListResponse import (
+    IntegrationsListResponse as IntegrationsListResponseModel,
+)
+from ..models.IntegrationsCreateRequest import (
+    IntegrationsCreateRequest as IntegrationsCreateRequestModel,
+)
+from ..models.IntegrationsCreateResponse import (
+    IntegrationsCreateResponse as IntegrationsCreateResponseModel,
+)
 
 
 class Integrations(BaseService):
-    def list(self) -> IntegrationsListResponseModel:
-        """
-        List
-        """
-
-        url_endpoint = "/v3/integrations"
-        headers = {}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return IntegrationsListResponseModel(**res)
-        return res
-
-    def create(
-        self, request_input: IntegrationsCreateRequestModel = None
-    ) -> IntegrationsCreateResponseModel:
-        """
-        Create
-        """
-
-        url_endpoint = "/v3/integrations"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return IntegrationsCreateResponseModel(**res)
-        return res
-
     def get(self, integration: str) -> IntegrationsGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             integration: str
                 The integration slug
@@ -91,15 +59,15 @@
         Parameters:
         ----------
             integration: str
                 The slug of the integration to update
         """
 
         url_endpoint = "/v3/integrations/integration"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not integration:
             raise ValueError(
                 "Parameter integration is required, cannot be empty or blank."
             )
         query_params.append(
@@ -132,7 +100,39 @@
             query_serializer.serialize_query("form", False, "integration", integration)
         )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.delete(final_url, headers, True)
         if res and isinstance(res, dict):
             return IntegrationsDeleteResponseModel(**res)
         return res
+
+    def list(self) -> IntegrationsListResponseModel:
+        """
+        List
+        """
+
+        url_endpoint = "/v3/integrations"
+        headers = {}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return IntegrationsListResponseModel(**res)
+        return res
+
+    def create(
+        self, request_input: IntegrationsCreateRequestModel = None
+    ) -> IntegrationsCreateResponseModel:
+        """
+        Create
+        """
+
+        url_endpoint = "/v3/integrations"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return IntegrationsCreateResponseModel(**res)
+        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/invites.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/invites.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/project_members.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/project_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Parameters:
         ----------
             project: str
                 Project slug
         """
 
         url_endpoint = "/v3/projects/project/members"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
@@ -86,15 +86,15 @@
     ) -> ProjectMembersGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             project: str
                 Project slug
-            type: Type
+            type_: Type
             slug: str
                 Member's slug
         """
 
         url_endpoint = "/v3/projects/project/members/member/{type_}/{slug}"
         headers = {}
         query_params = []
@@ -136,23 +136,23 @@
         type_: TypeModel,
         request_input: ProjectMembersUpdateRequestModel = None,
     ) -> ProjectMembersUpdateResponseModel:
         """
         Update
         Parameters:
         ----------
-            type: Type
+            type_: Type
             slug: str
                 Member's slug
             project: str
                 Project slug
         """
 
         url_endpoint = "/v3/projects/project/members/member/{type_}/{slug}"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not type_:
             raise ValueError("Parameter type_ is required, cannot be empty or blank.")
         validated_type_ = self._enum_matching(type_, TypeModel.list(), "type_")
         url_endpoint = url_endpoint.replace(
             "{type_}",
@@ -182,15 +182,15 @@
         return res
 
     def delete(self, project: str, slug: str, type_: TypeModel):
         """
         Delete
         Parameters:
         ----------
-            type: Type
+            type_: Type
             slug: str
                 Member's slug
             project: str
                 Project slug
         """
 
         url_endpoint = "/v3/projects/project/members/member/{type_}/{slug}"
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/project_roles.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/project_roles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,34 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.ProjectRolesListResponse import (
-    ProjectRolesListResponse as ProjectRolesListResponseModel,
-)
-from ..models.ProjectRolesCreateResponse import (
-    ProjectRolesCreateResponse as ProjectRolesCreateResponseModel,
-)
 from ..models.ProjectRolesGetResponse import (
     ProjectRolesGetResponse as ProjectRolesGetResponseModel,
 )
+from ..models.ProjectRolesUpdateRequest import (
+    ProjectRolesUpdateRequest as ProjectRolesUpdateRequestModel,
+)
 from ..models.ProjectRolesUpdateResponse import (
     ProjectRolesUpdateResponse as ProjectRolesUpdateResponseModel,
 )
+from ..models.ProjectRolesListResponse import (
+    ProjectRolesListResponse as ProjectRolesListResponseModel,
+)
+from ..models.ProjectRolesCreateRequest import (
+    ProjectRolesCreateRequest as ProjectRolesCreateRequestModel,
+)
+from ..models.ProjectRolesCreateResponse import (
+    ProjectRolesCreateResponse as ProjectRolesCreateResponseModel,
+)
 from ..models.ProjectRolesListPermissionsResponse import (
     ProjectRolesListPermissionsResponse as ProjectRolesListPermissionsResponseModel,
 )
 
 
 class ProjectRoles(BaseService):
-    def list(self) -> ProjectRolesListResponseModel:
-        """
-        List
-        """
-
-        url_endpoint = "/v3/projects/roles"
-        headers = {}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return ProjectRolesListResponseModel(**res)
-        return res
-
-    def create(self) -> ProjectRolesCreateResponseModel:
-        """
-        Create
-        """
-
-        url_endpoint = "/v3/projects/roles"
-        headers = {}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, {}, True)
-        if res and isinstance(res, dict):
-            return ProjectRolesCreateResponseModel(**res)
-        return res
-
     def get(self, role: str) -> ProjectRolesGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             role: str
                 The role's unique identifier
@@ -69,34 +45,36 @@
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return ProjectRolesGetResponseModel(**res)
         return res
 
-    def update(self, role: str) -> ProjectRolesUpdateResponseModel:
+    def update(
+        self, role: str, request_input: ProjectRolesUpdateRequestModel = None
+    ) -> ProjectRolesUpdateResponseModel:
         """
         Update
         Parameters:
         ----------
             role: str
                 The role's unique identifier
         """
 
         url_endpoint = "/v3/projects/roles/role/{role}"
-        headers = {}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
         if not role:
             raise ValueError("Parameter role is required, cannot be empty or blank.")
         url_endpoint = url_endpoint.replace(
             "{role}",
             quote(str(query_serializer.serialize_path("simple", False, role, None))),
         )
         final_url = self._url_prefix + url_endpoint
-        res = self._http.patch(final_url, headers, {}, True)
+        res = self._http.patch(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return ProjectRolesUpdateResponseModel(**res)
         return res
 
     def delete(self, role: str):
         """
         Delete
@@ -115,14 +93,46 @@
             "{role}",
             quote(str(query_serializer.serialize_path("simple", False, role, None))),
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
 
+    def list(self) -> ProjectRolesListResponseModel:
+        """
+        List
+        """
+
+        url_endpoint = "/v3/projects/roles"
+        headers = {}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return ProjectRolesListResponseModel(**res)
+        return res
+
+    def create(
+        self, request_input: ProjectRolesCreateRequestModel = None
+    ) -> ProjectRolesCreateResponseModel:
+        """
+        Create
+        """
+
+        url_endpoint = "/v3/projects/roles"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return ProjectRolesCreateResponseModel(**res)
+        return res
+
     def list_permissions(self) -> ProjectRolesListPermissionsResponseModel:
         """
         List Permissions
         """
 
         url_endpoint = "/v3/projects/permissions"
         headers = {}
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/projects.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/projects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
 from ..models.ListResponse import ListResponse as ListResponseModel
 from ..models.CreateRequest import CreateRequest as CreateRequestModel
 from ..models.CreateResponse import CreateResponse as CreateResponseModel
-from ..models.ProjectsGetResponse import ProjectsGetResponse as ProjectsGetResponseModel
-from ..models.ProjectsUpdateRequest import (
-    ProjectsUpdateRequest as ProjectsUpdateRequestModel,
-)
-from ..models.ProjectsUpdateResponse import (
-    ProjectsUpdateResponse as ProjectsUpdateResponseModel,
-)
+from ..models.GetResponse import GetResponse as GetResponseModel
+from ..models.UpdateRequest import UpdateRequest as UpdateRequestModel
+from ..models.UpdateResponse import UpdateResponse as UpdateResponseModel
 from ..models.DeleteRequest import DeleteRequest as DeleteRequestModel
 
 
 class Projects(BaseService):
     def list(self, page: int = None, per_page: int = None) -> ListResponseModel:
         """
         List
@@ -48,24 +44,24 @@
 
     def create(self, request_input: CreateRequestModel = None) -> CreateResponseModel:
         """
         Create
         """
 
         url_endpoint = "/v3/projects"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return CreateResponseModel(**res)
         return res
 
-    def get(self, project: str) -> ProjectsGetResponseModel:
+    def get(self, project: str) -> GetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             project: str
                 Unique identifier for the project object.
         """
@@ -78,39 +74,37 @@
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
-            return ProjectsGetResponseModel(**res)
+            return GetResponseModel(**res)
         return res
 
-    def update(
-        self, request_input: ProjectsUpdateRequestModel = None
-    ) -> ProjectsUpdateResponseModel:
+    def update(self, request_input: UpdateRequestModel = None) -> UpdateResponseModel:
         """
         Update
         """
 
         url_endpoint = "/v3/projects/project"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return ProjectsUpdateResponseModel(**res)
+            return UpdateResponseModel(**res)
         return res
 
     def delete(self, request_input: DeleteRequestModel = None):
         """
         Delete
         """
 
         url_endpoint = "/v3/projects/project"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/secrets.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
 from ..models.SecretsListResponse import SecretsListResponse as SecretsListResponseModel
-from ..models.UpdateRequest import UpdateRequest as UpdateRequestModel
-from ..models.UpdateResponse import UpdateResponse as UpdateResponseModel
+from ..models.SecretsUpdateRequest import (
+    SecretsUpdateRequest as SecretsUpdateRequestModel,
+)
+from ..models.SecretsUpdateResponse import (
+    SecretsUpdateResponse as SecretsUpdateResponseModel,
+)
 from ..models.SecretsGetResponse import SecretsGetResponse as SecretsGetResponseModel
 from ..models.Format import Format as FormatModel
 from ..models.NameTransformer import NameTransformer as NameTransformerModel
 from ..models.DownloadResponse import DownloadResponse as DownloadResponseModel
-from ..models.NamesResponse import NamesResponse as NamesResponseModel
 from ..models.UpdateNoteRequest import UpdateNoteRequest as UpdateNoteRequestModel
 from ..models.UpdateNoteResponse import UpdateNoteResponse as UpdateNoteResponseModel
+from ..models.NamesResponse import NamesResponse as NamesResponseModel
 
 
 class Secrets(BaseService):
     def list(
         self,
         config: str,
         project: str,
@@ -83,27 +87,29 @@
             )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return SecretsListResponseModel(**res)
         return res
 
-    def update(self, request_input: UpdateRequestModel = None) -> UpdateResponseModel:
+    def update(
+        self, request_input: SecretsUpdateRequestModel = None
+    ) -> SecretsUpdateResponseModel:
         """
         Update
         """
 
         url_endpoint = "/v3/configs/config/secrets"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
-            return UpdateResponseModel(**res)
+            return SecretsUpdateResponseModel(**res)
         return res
 
     def get(self, name: str, config: str, project: str) -> SecretsGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
@@ -180,14 +186,15 @@
         self,
         config: str,
         project: str,
         format: FormatModel = None,
         name_transformer: NameTransformerModel = None,
         include_dynamic_secrets: bool = None,
         dynamic_secrets_ttl_sec: int = None,
+        secrets: str = None,
     ) -> DownloadResponseModel:
         """
         Download
         Parameters:
         ----------
             project: str
                 Unique identifier for the project object. Not required if using a Service Token.
@@ -196,14 +203,16 @@
             format: Format
             name_transformer: NameTransformer
                 Transform secret names to a different case
             include_dynamic_secrets: bool
                 Whether or not to issue leases and include dynamic secret values for the config
             dynamic_secrets_ttl_sec: int
                 The number of seconds until dynamic leases expire. Must be used with `include_dynamic_secrets`. Defaults to 1800 (30 minutes).
+            secrets: str
+                Comma-delimited list of secrets to include in the download. Defaults to all secrets if left unspecified.
         """
 
         url_endpoint = "/v3/configs/config/secrets/download"
         headers = {}
         query_params = []
         self._add_required_headers(headers)
         if not project:
@@ -240,20 +249,41 @@
             )
         if dynamic_secrets_ttl_sec:
             query_params.append(
                 query_serializer.serialize_query(
                     "form", False, "dynamic_secrets_ttl_sec", dynamic_secrets_ttl_sec
                 )
             )
+        if secrets:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "secrets", secrets)
+            )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return DownloadResponseModel(**res)
         return res
 
+    def update_note(
+        self, request_input: UpdateNoteRequestModel = None
+    ) -> UpdateNoteResponseModel:
+        """
+        Update Note
+        """
+
+        url_endpoint = "/v3/configs/config/secrets/note"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return UpdateNoteResponseModel(**res)
+        return res
+
     def names(
         self,
         config: str,
         project: str,
         include_dynamic_secrets: bool = None,
         include_managed_secrets: bool = None,
     ) -> NamesResponseModel:
@@ -298,24 +328,7 @@
                 )
             )
         final_url = self._url_prefix + url_endpoint + "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return NamesResponseModel(**res)
         return res
-
-    def update_note(
-        self, request_input: UpdateNoteRequestModel = None
-    ) -> UpdateNoteResponseModel:
-        """
-        Update Note
-        """
-
-        url_endpoint = "/v3/configs/config/secrets/note"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return UpdateNoteResponseModel(**res)
-        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/service_accounts.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/service_accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,79 +1,31 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
-from ..models.ServiceAccountsListResponse import (
-    ServiceAccountsListResponse as ServiceAccountsListResponseModel,
-)
-from ..models.ServiceAccountsCreateRequest import (
-    ServiceAccountsCreateRequest as ServiceAccountsCreateRequestModel,
-)
-from ..models.ServiceAccountsCreateResponse import (
-    ServiceAccountsCreateResponse as ServiceAccountsCreateResponseModel,
-)
 from ..models.ServiceAccountsGetResponse import (
     ServiceAccountsGetResponse as ServiceAccountsGetResponseModel,
 )
 from ..models.ServiceAccountsUpdateRequest import (
     ServiceAccountsUpdateRequest as ServiceAccountsUpdateRequestModel,
 )
 from ..models.ServiceAccountsUpdateResponse import (
     ServiceAccountsUpdateResponse as ServiceAccountsUpdateResponseModel,
 )
+from ..models.ServiceAccountsListResponse import (
+    ServiceAccountsListResponse as ServiceAccountsListResponseModel,
+)
+from ..models.ServiceAccountsCreateRequest import (
+    ServiceAccountsCreateRequest as ServiceAccountsCreateRequestModel,
+)
+from ..models.ServiceAccountsCreateResponse import (
+    ServiceAccountsCreateResponse as ServiceAccountsCreateResponseModel,
+)
 
 
 class ServiceAccounts(BaseService):
-    def list(
-        self, page: int = None, per_page: int = None
-    ) -> ServiceAccountsListResponseModel:
-        """
-        List
-        Parameters:
-        ----------
-            page: int
-            per_page: int
-        """
-
-        url_endpoint = "/v3/workplace/service_accounts"
-        headers = {}
-        query_params = []
-        self._add_required_headers(headers)
-        if page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "page", page)
-            )
-        if per_page:
-            query_params.append(
-                query_serializer.serialize_query("form", False, "per_page", per_page)
-            )
-        final_url = self._url_prefix + url_endpoint
-        if len(query_params) > 0:
-            final_url += "?" + "&".join(query_params)
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return ServiceAccountsListResponseModel(**res)
-        return res
-
-    def create(
-        self, request_input: ServiceAccountsCreateRequestModel = None
-    ) -> ServiceAccountsCreateResponseModel:
-        """
-        Create
-        """
-
-        url_endpoint = "/v3/workplace/service_accounts"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, request_input, True)
-        if res and isinstance(res, dict):
-            return ServiceAccountsCreateResponseModel(**res)
-        return res
-
     def get(self, slug: str) -> ServiceAccountsGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             slug: str
                 Slug of the service account
@@ -102,15 +54,15 @@
         Parameters:
         ----------
             slug: str
                 Slug of the service account
         """
 
         url_endpoint = "/v3/workplace/service_accounts/service_account/{slug}"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
         if not slug:
             raise ValueError("Parameter slug is required, cannot be empty or blank.")
         url_endpoint = url_endpoint.replace(
             "{slug}",
             quote(str(query_serializer.serialize_path("simple", False, slug, None))),
         )
@@ -137,7 +89,55 @@
         url_endpoint = url_endpoint.replace(
             "{slug}",
             quote(str(query_serializer.serialize_path("simple", False, slug, None))),
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
+
+    def list(
+        self, page: int = None, per_page: int = None
+    ) -> ServiceAccountsListResponseModel:
+        """
+        List
+        Parameters:
+        ----------
+            page: int
+            per_page: int
+        """
+
+        url_endpoint = "/v3/workplace/service_accounts"
+        headers = {}
+        query_params = []
+        self._add_required_headers(headers)
+        if page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "page", page)
+            )
+        if per_page:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "per_page", per_page)
+            )
+        final_url = self._url_prefix + url_endpoint
+        if len(query_params) > 0:
+            final_url += "?" + "&".join(query_params)
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return ServiceAccountsListResponseModel(**res)
+        return res
+
+    def create(
+        self, request_input: ServiceAccountsCreateRequestModel = None
+    ) -> ServiceAccountsCreateResponseModel:
+        """
+        Create
+        """
+
+        url_endpoint = "/v3/workplace/service_accounts"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.post(final_url, headers, request_input, True)
+        if res and isinstance(res, dict):
+            return ServiceAccountsCreateResponseModel(**res)
+        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/service_tokens.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/service_tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
+from ..models.ServiceTokensDeleteRequest import (
+    ServiceTokensDeleteRequest as ServiceTokensDeleteRequestModel,
+)
+from ..models.DeleteResponse import DeleteResponse as DeleteResponseModel
 from ..models.ServiceTokensListResponse import (
     ServiceTokensListResponse as ServiceTokensListResponseModel,
 )
 from ..models.ServiceTokensCreateRequest import (
     ServiceTokensCreateRequest as ServiceTokensCreateRequestModel,
 )
 from ..models.ServiceTokensCreateResponse import (
     ServiceTokensCreateResponse as ServiceTokensCreateResponseModel,
 )
-from ..models.ServiceTokensDeleteRequest import (
-    ServiceTokensDeleteRequest as ServiceTokensDeleteRequestModel,
-)
-from ..models.DeleteResponse import DeleteResponse as DeleteResponseModel
 
 
 class ServiceTokens(BaseService):
+    def delete(
+        self, request_input: ServiceTokensDeleteRequestModel = None
+    ) -> DeleteResponseModel:
+        """
+        Delete
+        """
+
+        url_endpoint = "/v3/configs/config/tokens/token"
+        headers = {"Content-Type": "application/json"}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.delete(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return DeleteResponseModel(**res)
+        return res
+
     def list(self, config: str, project: str) -> ServiceTokensListResponseModel:
         """
         List
         Parameters:
         ----------
             project: str
                 Unique identifier for the project object.
@@ -52,32 +69,15 @@
         self, request_input: ServiceTokensCreateRequestModel = None
     ) -> ServiceTokensCreateResponseModel:
         """
         Create
         """
 
         url_endpoint = "/v3/configs/config/tokens"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return ServiceTokensCreateResponseModel(**res)
         return res
-
-    def delete(
-        self, request_input: ServiceTokensDeleteRequestModel = None
-    ) -> DeleteResponseModel:
-        """
-        Delete
-        """
-
-        url_endpoint = "/v3/configs/config/tokens/token"
-        headers = {"Content-type": "application/json"}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.delete(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return DeleteResponseModel(**res)
-        return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/syncs.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/syncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             project: str
                 The project slug
             config: str
                 The config slug
         """
 
         url_endpoint = "/v3/configs/config/syncs"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         query_params = []
         self._add_required_headers(headers)
         if not project:
             raise ValueError("Parameter project is required, cannot be empty or blank.")
         query_params.append(
             query_serializer.serialize_query("form", False, "project", project)
         )
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/trusted_ips.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/trusted_ips.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/users.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/users.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 from ..net import query_serializer
 from .base import BaseService
 from ..models.UsersListResponse import UsersListResponse as UsersListResponseModel
 from ..models.UsersGetResponse import UsersGetResponse as UsersGetResponseModel
 
 
 class Users(BaseService):
-    def list(self, page: int = None) -> UsersListResponseModel:
+    def list(self, page: int = None, email: str = None) -> UsersListResponseModel:
         """
         List
         Parameters:
         ----------
             page: int
                 The page of users to fetch
+            email: str
+                Filter results to only include the user with the provided email address
         """
 
         url_endpoint = "/v3/workplace/users"
         headers = {}
         query_params = []
         self._add_required_headers(headers)
         if page:
             query_params.append(
                 query_serializer.serialize_query("form", False, "page", page)
             )
+        if email:
+            query_params.append(
+                query_serializer.serialize_query("form", False, "email", email)
+            )
         final_url = self._url_prefix + url_endpoint
         if len(query_params) > 0:
             final_url += "?" + "&".join(query_params)
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return UsersListResponseModel(**res)
         return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/v_3.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/v_3.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/workplace.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/workplace.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self, request_input: WorkplaceUpdateRequestModel = None
     ) -> WorkplaceUpdateResponseModel:
         """
         Update
         """
 
         url_endpoint = "/v3/workplace"
-        headers = {"Content-type": "application/json"}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return WorkplaceUpdateResponseModel(**res)
         return res
```

### Comparing `doppler-sdk-1.2.1/src/dopplersdk/services/workplace_roles.py` & `doppler-sdk-1.3.0/src/dopplersdk/services/workplace_roles.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from urllib.parse import quote
 from ..net import query_serializer
 from .base import BaseService
 from ..models.WorkplaceRolesListResponse import (
     WorkplaceRolesListResponse as WorkplaceRolesListResponseModel,
 )
+from ..models.WorkplaceRolesCreateRequest import (
+    WorkplaceRolesCreateRequest as WorkplaceRolesCreateRequestModel,
+)
 from ..models.WorkplaceRolesCreateResponse import (
     WorkplaceRolesCreateResponse as WorkplaceRolesCreateResponseModel,
 )
-from ..models.ListPermissionsResponse import (
-    ListPermissionsResponse as ListPermissionsResponseModel,
-)
 from ..models.WorkplaceRolesGetResponse import (
     WorkplaceRolesGetResponse as WorkplaceRolesGetResponseModel,
 )
+from ..models.WorkplaceRolesUpdateRequest import (
+    WorkplaceRolesUpdateRequest as WorkplaceRolesUpdateRequestModel,
+)
 from ..models.WorkplaceRolesUpdateResponse import (
     WorkplaceRolesUpdateResponse as WorkplaceRolesUpdateResponseModel,
 )
+from ..models.ListPermissionsResponse import (
+    ListPermissionsResponse as ListPermissionsResponseModel,
+)
 
 
 class WorkplaceRoles(BaseService):
     def list(self) -> WorkplaceRolesListResponseModel:
         """
         List
         """
@@ -30,44 +36,31 @@
 
         final_url = self._url_prefix + url_endpoint
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return WorkplaceRolesListResponseModel(**res)
         return res
 
-    def create(self) -> WorkplaceRolesCreateResponseModel:
+    def create(
+        self, request_input: WorkplaceRolesCreateRequestModel = None
+    ) -> WorkplaceRolesCreateResponseModel:
         """
         Create
         """
 
         url_endpoint = "/v3/workplace/roles"
-        headers = {}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
 
         final_url = self._url_prefix + url_endpoint
-        res = self._http.post(final_url, headers, {}, True)
+        res = self._http.post(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return WorkplaceRolesCreateResponseModel(**res)
         return res
 
-    def list_permissions(self) -> ListPermissionsResponseModel:
-        """
-        List Permissions
-        """
-
-        url_endpoint = "/v3/workplace/permissions"
-        headers = {}
-        self._add_required_headers(headers)
-
-        final_url = self._url_prefix + url_endpoint
-        res = self._http.get(final_url, headers, True)
-        if res and isinstance(res, dict):
-            return ListPermissionsResponseModel(**res)
-        return res
-
     def get(self, role: str) -> WorkplaceRolesGetResponseModel:
         """
         Retrieve
         Parameters:
         ----------
             role: str
                 The role's unique identifier
@@ -84,34 +77,36 @@
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.get(final_url, headers, True)
         if res and isinstance(res, dict):
             return WorkplaceRolesGetResponseModel(**res)
         return res
 
-    def update(self, role: str) -> WorkplaceRolesUpdateResponseModel:
+    def update(
+        self, role: str, request_input: WorkplaceRolesUpdateRequestModel = None
+    ) -> WorkplaceRolesUpdateResponseModel:
         """
         Update
         Parameters:
         ----------
             role: str
-                The role's unique identifier
+                The role's unique identifier, which is the initial name the role was given
         """
 
         url_endpoint = "/v3/workplace/roles/role/{role}"
-        headers = {}
+        headers = {"Content-Type": "application/json"}
         self._add_required_headers(headers)
         if not role:
             raise ValueError("Parameter role is required, cannot be empty or blank.")
         url_endpoint = url_endpoint.replace(
             "{role}",
             quote(str(query_serializer.serialize_path("simple", False, role, None))),
         )
         final_url = self._url_prefix + url_endpoint
-        res = self._http.patch(final_url, headers, {}, True)
+        res = self._http.patch(final_url, headers, request_input, True)
         if res and isinstance(res, dict):
             return WorkplaceRolesUpdateResponseModel(**res)
         return res
 
     def delete(self, role: str):
         """
         Delete
@@ -129,7 +124,22 @@
         url_endpoint = url_endpoint.replace(
             "{role}",
             quote(str(query_serializer.serialize_path("simple", False, role, None))),
         )
         final_url = self._url_prefix + url_endpoint
         res = self._http.delete(final_url, headers, True)
         return res
+
+    def list_permissions(self) -> ListPermissionsResponseModel:
+        """
+        List Permissions
+        """
+
+        url_endpoint = "/v3/workplace/permissions"
+        headers = {}
+        self._add_required_headers(headers)
+
+        final_url = self._url_prefix + url_endpoint
+        res = self._http.get(final_url, headers, True)
+        if res and isinstance(res, dict):
+            return ListPermissionsResponseModel(**res)
+        return res
```

