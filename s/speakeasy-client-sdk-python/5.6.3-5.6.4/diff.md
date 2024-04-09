# Comparing `tmp/speakeasy-client-sdk-python-5.6.3.tar.gz` & `tmp/speakeasy-client-sdk-python-5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.6.3.tar", last modified: Sat Apr  6 00:11:52 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.6.4.tar", last modified: Tue Apr  9 00:13:09 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.6.3.tar` & `speakeasy-client-sdk-python-5.6.4.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.790147 speakeasy-client-sdk-python-5.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-06 00:11:52.790147 speakeasy-client-sdk-python-5.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:52.790147 speakeasy-client-sdk-python-5.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.774147 speakeasy-client-sdk-python-5.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.778147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.778147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29324 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    22128 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.778147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.778147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.782147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.786147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28780 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.786147 speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-06 00:11:43.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:52.790147 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-06 00:11:52.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-06 00:11:52.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:52.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 00:11:52.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 00:11:52.000000 speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.000119 speakeasy-client-sdk-python-5.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.000119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.004119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.008119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.012119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.012119 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-09 00:12:53.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:13:09.016119 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 00:13:08.000000 speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.6.3/PKG-INFO` & `speakeasy-client-sdk-python-5.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.3
+Version: 5.6.4
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.3/README.md` & `speakeasy-client-sdk-python-5.6.4/README.md`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/setup.py` & `speakeasy-client-sdk-python-5.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.6.3',
+    version='5.6.4',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/apiendpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def delete_api_endpoint(self, request: operations.DeleteAPIEndpointRequest) -> operations.DeleteAPIEndpointResponse:
         r"""Delete an ApiEndpoint.
         Delete an ApiEndpoint. This will also delete all associated Request Logs (if using a Postgres datastore).
         """
         hook_ctx = HookContext(operation_id='deleteApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -81,15 +81,15 @@
         r"""Find an ApiEndpoint via its displayName.
         Find an ApiEndpoint via its displayName (set by operationId from a registered OpenAPI schema).
         This is useful for finding the ID of an ApiEndpoint to use in the /v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID} endpoints.
         """
         hook_ctx = HookContext(operation_id='findApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.FindAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/find/{displayName}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/find/{displayName}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -143,15 +143,15 @@
         r"""Generate an OpenAPI specification for a particular ApiEndpoint.
         This endpoint will generate a new operation in any registered OpenAPI document if the operation does not already exist in the document.
         Returns the original document and the newly generated document allowing a diff to be performed to see what has changed.
         """
         hook_ctx = HookContext(operation_id='generateOpenApiSpecForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GenerateOpenAPISpecForAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/openapi', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/openapi', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -204,15 +204,15 @@
     def generate_postman_collection_for_api_endpoint(self, request: operations.GeneratePostmanCollectionForAPIEndpointRequest, accept_header_override: Optional[GeneratePostmanCollectionForApiEndpointAcceptEnum] = None) -> operations.GeneratePostmanCollectionForAPIEndpointResponse:
         r"""Generate a Postman collection for a particular ApiEndpoint.
         Generates a postman collection that allows the endpoint to be called from postman variables produced for any path/query/header parameters included in the OpenAPI document.
         """
         hook_ctx = HookContext(operation_id='generatePostmanCollectionForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GeneratePostmanCollectionForAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/postman', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/postman', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         if accept_header_override is not None:
@@ -265,15 +265,15 @@
     
     
     def get_all_api_endpoints(self, request: operations.GetAllAPIEndpointsRequest) -> operations.GetAllAPIEndpointsResponse:
         r"""Get all Api endpoints for a particular apiID."""
         hook_ctx = HookContext(operation_id='getAllApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAllAPIEndpointsRequest, base_url, '/v1/apis/{apiID}/api_endpoints', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/api_endpoints', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -324,15 +324,15 @@
     
     
     def get_all_for_version_api_endpoints(self, request: operations.GetAllForVersionAPIEndpointsRequest) -> operations.GetAllForVersionAPIEndpointsResponse:
         r"""Get all ApiEndpoints for a particular apiID and versionID."""
         hook_ctx = HookContext(operation_id='getAllForVersionApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAllForVersionAPIEndpointsRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -383,15 +383,15 @@
     
     
     def get_api_endpoint(self, request: operations.GetAPIEndpointRequest) -> operations.GetAPIEndpointResponse:
         r"""Get an ApiEndpoint."""
         hook_ctx = HookContext(operation_id='getApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -444,15 +444,15 @@
     def upsert_api_endpoint(self, request: operations.UpsertAPIEndpointRequest) -> operations.UpsertAPIEndpointResponse:
         r"""Upsert an ApiEndpoint.
         Upsert an ApiEndpoint. If the ApiEndpoint does not exist it will be created, otherwise it will be updated.
         """
         hook_ctx = HookContext(operation_id='upsertApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpsertAPIEndpointRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpsertAPIEndpointRequest, "api_endpoint", False, False, 'json')
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def delete_api(self, request: operations.DeleteAPIRequest) -> operations.DeleteAPIResponse:
         r"""Delete an Api.
         Delete a particular version of an Api. The will also delete all associated ApiEndpoints, Metadata, Schemas & Request Logs (if using a Postgres datastore).
         """
         hook_ctx = HookContext(operation_id='deleteApi', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteAPIRequest, base_url, '/v1/apis/{apiID}/version/{versionID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -81,15 +81,15 @@
         r"""Generate an OpenAPI specification for a particular Api.
         This endpoint will generate any missing operations in any registered OpenAPI document if the operation does not already exist in the document.
         Returns the original document and the newly generated document allowing a diff to be performed to see what has changed.
         """
         hook_ctx = HookContext(operation_id='generateOpenApiSpec', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GenerateOpenAPISpecRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/generate/openapi', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/generate/openapi', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -142,15 +142,15 @@
     def generate_postman_collection(self, request: operations.GeneratePostmanCollectionRequest, accept_header_override: Optional[GeneratePostmanCollectionAcceptEnum] = None) -> operations.GeneratePostmanCollectionResponse:
         r"""Generate a Postman collection for a particular Api.
         Generates a postman collection containing all endpoints for a particular API. Includes variables produced for any path/query/header parameters included in the OpenAPI document.
         """
         hook_ctx = HookContext(operation_id='generatePostmanCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GeneratePostmanCollectionRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/generate/postman', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/generate/postman', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         if accept_header_override is not None:
@@ -206,22 +206,22 @@
         r"""Get all Api versions for a particular ApiEndpoint.
         Get all Api versions for a particular ApiEndpoint.
         Supports filtering the versions based on metadata attributes.
         """
         hook_ctx = HookContext(operation_id='getAllApiVersions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAllAPIVersionsRequest, base_url, '/v1/apis/{apiID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAllAPIVersionsRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -276,15 +276,15 @@
         url = base_url + '/v1/apis'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetApisRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -332,15 +332,15 @@
         r"""Upsert an Api
         Upsert an Api. If the Api does not exist, it will be created.
         If the Api exists, it will be updated.
         """
         hook_ctx = HookContext(operation_id='upsertApi', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpsertAPIRequest, base_url, '/v1/apis/{apiID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpsertAPIRequest, "api", False, False, 'json')
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/v1/auth/access_token'
         
         headers = {}
         query_params = {}
         
-        query_params = { **utils.get_query_params(operations.GetAccessTokenRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -143,15 +143,15 @@
         url = base_url + '/v1/workspace/access'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetWorkspaceAccessRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/embeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         url = base_url + '/v1/workspace/embed-access-token'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetEmbedAccessTokenRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -139,15 +139,15 @@
     
     
     def revoke_embed_access_token(self, request: operations.RevokeEmbedAccessTokenRequest) -> operations.RevokeEmbedAccessTokenResponse:
         r"""Revoke an embed access EmbedToken."""
         hook_ctx = HookContext(operation_id='revokeEmbedAccessToken', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RevokeEmbedAccessTokenRequest, base_url, '/v1/workspace/embed-access-tokens/{tokenID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/workspace/embed-access-tokens/{tokenID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,29 @@
         self.sdk_configuration = sdk_config
         
     
     
     def get_workspace_events(self, request: operations.GetWorkspaceEventsRequest) -> operations.GetWorkspaceEventsResponse:
         r"""Load recent events for a particular workspace"""
         hook_ctx = HookContext(operation_id='getWorkspaceEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetWorkspaceEventsGlobals(
+            workspace_id=self.sdk_configuration.globals.workspace_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetWorkspaceEventsRequest, base_url, '/v1/workspace/{workspaceID}/events', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetWorkspaceEventsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -77,24 +82,29 @@
         return res
 
     
     
     def get_workspace_targets(self, request: operations.GetWorkspaceTargetsRequest) -> operations.GetWorkspaceTargetsResponse:
         r"""Load targets for a particular workspace"""
         hook_ctx = HookContext(operation_id='getWorkspaceTargets', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.GetWorkspaceTargetsGlobals(
+            workspace_id=self.sdk_configuration.globals.workspace_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetWorkspaceTargetsRequest, base_url, '/v1/workspace/{workspaceID}/events/targets', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events/targets', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetWorkspaceTargetsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -141,28 +151,34 @@
     
     
     def post_workspace_events(self, request: operations.PostWorkspaceEventsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostWorkspaceEventsResponse:
         r"""Post events for a specific workspace
         Sends an array of events to be stored for a particular workspace.
         """
         hook_ctx = HookContext(operation_id='postWorkspaceEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.PostWorkspaceEventsGlobals(
+            workspace_id=self.sdk_configuration.globals.workspace_id,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PostWorkspaceEventsRequest, base_url, '/v1/workspace/{workspaceID}/events', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/workspace/{workspaceID}/events', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.PostWorkspaceEventsRequest, "request_body", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         global_retry_config = self.sdk_configuration.retry_config
         retry_config = retries
         if retry_config is None:
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     
     
     def delete_version_metadata(self, request: operations.DeleteVersionMetadataRequest) -> operations.DeleteVersionMetadataResponse:
         r"""Delete metadata for a particular apiID and versionID."""
         hook_ctx = HookContext(operation_id='deleteVersionMetadata', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteVersionMetadataRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/metadata/{metaKey}/{metaValue}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/metadata/{metaKey}/{metaValue}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -71,15 +71,15 @@
     
     
     def get_version_metadata(self, request: operations.GetVersionMetadataRequest) -> operations.GetVersionMetadataResponse:
         r"""Get all metadata for a particular apiID and versionID."""
         hook_ctx = HookContext(operation_id='getVersionMetadata', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetVersionMetadataRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/metadata', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/metadata', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -130,15 +130,15 @@
     
     
     def insert_version_metadata(self, request: operations.InsertVersionMetadataRequest) -> operations.InsertVersionMetadataResponse:
         r"""Insert metadata for a particular apiID and versionID."""
         hook_ctx = HookContext(operation_id='insertVersionMetadata', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.InsertVersionMetadataRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/metadata', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/metadata', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.InsertVersionMetadataRequest, "version_metadata", False, False, 'json')
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 from .queryeventlog import *
 from .registerschema import *
 from .revokeembedaccesstoken import *
 from .upsertapi import *
 from .upsertapiendpoint import *
 from .validateapikey import *
 
-__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
+__all__ = ["DeleteAPIEndpointRequest","DeleteAPIEndpointResponse","DeleteAPIRequest","DeleteAPIResponse","DeleteSchemaRequest","DeleteSchemaResponse","DeleteVersionMetadataRequest","DeleteVersionMetadataResponse","DownloadSchemaRequest","DownloadSchemaResponse","DownloadSchemaRevisionRequest","DownloadSchemaRevisionResponse","File","FindAPIEndpointRequest","FindAPIEndpointResponse","GenerateOpenAPISpecForAPIEndpointRequest","GenerateOpenAPISpecForAPIEndpointResponse","GenerateOpenAPISpecRequest","GenerateOpenAPISpecResponse","GeneratePostmanCollectionForAPIEndpointRequest","GeneratePostmanCollectionForAPIEndpointResponse","GeneratePostmanCollectionRequest","GeneratePostmanCollectionResponse","GenerateRequestPostmanCollectionRequest","GenerateRequestPostmanCollectionResponse","GetAPIEndpointRequest","GetAPIEndpointResponse","GetAccessTokenRequest","GetAccessTokenResponse","GetAllAPIEndpointsRequest","GetAllAPIEndpointsResponse","GetAllAPIVersionsRequest","GetAllAPIVersionsResponse","GetAllForVersionAPIEndpointsRequest","GetAllForVersionAPIEndpointsResponse","GetApisRequest","GetApisResponse","GetEmbedAccessTokenRequest","GetEmbedAccessTokenResponse","GetOrganizationsResponse","GetRequestFromEventLogRequest","GetRequestFromEventLogResponse","GetSchemaDiffRequest","GetSchemaDiffResponse","GetSchemaRequest","GetSchemaResponse","GetSchemaRevisionRequest","GetSchemaRevisionResponse","GetSchemasRequest","GetSchemasResponse","GetUserResponse","GetValidEmbedAccessTokensResponse","GetVersionMetadataRequest","GetVersionMetadataResponse","GetWorkspaceAccessRequest","GetWorkspaceAccessResponse","GetWorkspaceEventsGlobals","GetWorkspaceEventsRequest","GetWorkspaceEventsResponse","GetWorkspaceTargetsGlobals","GetWorkspaceTargetsRequest","GetWorkspaceTargetsResponse","InsertVersionMetadataRequest","InsertVersionMetadataResponse","Op","PostWorkspaceEventsGlobals","PostWorkspaceEventsRequest","PostWorkspaceEventsResponse","QueryEventLogRequest","QueryEventLogResponse","QueryParamOp","RegisterSchemaRequest","RegisterSchemaRequestBody","RegisterSchemaResponse","RevokeEmbedAccessTokenRequest","RevokeEmbedAccessTokenResponse","UpsertAPIEndpointRequest","UpsertAPIEndpointResponse","UpsertAPIRequest","UpsertAPIResponse","ValidateAPIKeyResponse"]
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspaceevents.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from ...models.shared import clievent as shared_clievent
 from datetime import datetime
 from typing import List, Optional
 
 
 @dataclasses.dataclass
+class GetWorkspaceEventsGlobals:
+    workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class GetWorkspaceEventsRequest:
     after_created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after_created_at', 'style': 'form', 'explode': True }})
     r"""Filter to only return events created after this timestamp"""
     generate_gen_lock_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'generate_gen_lock_id', 'style': 'form', 'explode': True }})
     r"""Filter to only return events corresponding to a particular gen_lock_id (gen_lock_id uniquely identifies a target)"""
     workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
     r"""Unique identifier of the workspace."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 import requests as requests_http
 from ...models.shared import targetsdk as shared_targetsdk
 from datetime import datetime
 from typing import List, Optional
 
 
 @dataclasses.dataclass
+class GetWorkspaceTargetsGlobals:
+    workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
+    
+
+
+
+@dataclasses.dataclass
 class GetWorkspaceTargetsRequest:
     after_last_event_created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'after_last_event_created_at', 'style': 'form', 'explode': True }})
     r"""Filter to only return targets with events created after this timestamp"""
     workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
     r"""Unique identifier of the workspace."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import clievent as shared_clievent
-from typing import List, Optional
+from ...models.errors import error as errors_error
+from ...models.shared import api as shared_api
+from ...models.shared import api_input as shared_api_input
+from typing import Optional
 
 
 @dataclasses.dataclass
-class PostWorkspaceEventsRequest:
-    request_body: List[shared_clievent.CliEvent] = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    workspace_id: Optional[str] = dataclasses.field(default=None, metadata={'path_param': { 'field_name': 'workspaceID', 'style': 'simple', 'explode': False }})
-    r"""Unique identifier of the workspace."""
+class UpsertAPIRequest:
+    api: shared_api_input.APIInput = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    r"""A JSON representation of the Api to upsert"""
+    api_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'apiID', 'style': 'simple', 'explode': False }})
+    r"""The ID of the Api to upsert."""
     
 
 
 
 @dataclasses.dataclass
-class PostWorkspaceEventsResponse:
+class UpsertAPIResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
+    api: Optional[shared_api.API] = dataclasses.field(default=None)
+    r"""OK"""
+    error: Optional[errors_error.Error] = dataclasses.field(default=None)
+    r"""Default error response"""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ...models.errors import error as errors_error
-from ...models.shared import api as shared_api
-from ...models.shared import api_input as shared_api_input
+from ...models.shared import apiendpoint as shared_apiendpoint
+from ...models.shared import apiendpoint_input as shared_apiendpoint_input
 from typing import Optional
 
 
 @dataclasses.dataclass
-class UpsertAPIRequest:
-    api: shared_api_input.APIInput = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    r"""A JSON representation of the Api to upsert"""
+class UpsertAPIEndpointRequest:
+    api_endpoint: shared_apiendpoint_input.APIEndpointInput = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
+    r"""A JSON representation of the ApiEndpoint to upsert."""
+    api_endpoint_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'apiEndpointID', 'style': 'simple', 'explode': False }})
+    r"""The ID of the ApiEndpoint to upsert."""
     api_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'apiID', 'style': 'simple', 'explode': False }})
-    r"""The ID of the Api to upsert."""
+    r"""The ID of the Api the ApiEndpoint belongs to."""
+    version_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'versionID', 'style': 'simple', 'explode': False }})
+    r"""The version ID of the Api the ApiEndpoint belongs to."""
     
 
 
 
 @dataclasses.dataclass
-class UpsertAPIResponse:
+class UpsertAPIEndpointResponse:
     content_type: str = dataclasses.field()
     r"""HTTP response content type for this operation"""
     status_code: int = dataclasses.field()
     r"""HTTP response status code for this operation"""
     raw_response: requests_http.Response = dataclasses.field()
     r"""Raw HTTP response; suitable for custom response parsing"""
-    api: Optional[shared_api.API] = dataclasses.field(default=None)
+    api_endpoint: Optional[shared_apiendpoint.APIEndpoint] = dataclasses.field(default=None)
     r"""OK"""
     error: Optional[errors_error.Error] = dataclasses.field(default=None)
     r"""Default error response"""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api_input.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ...models.errors import error as errors_error
-from ...models.shared import apiendpoint as shared_apiendpoint
-from ...models.shared import apiendpoint_input as shared_apiendpoint_input
-from typing import Optional
+from dataclasses_json import Undefined, dataclass_json
+from speakeasy import utils
+from typing import Dict, List, Optional
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UpsertAPIEndpointRequest:
-    api_endpoint: shared_apiendpoint_input.APIEndpointInput = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
-    r"""A JSON representation of the ApiEndpoint to upsert."""
-    api_endpoint_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'apiEndpointID', 'style': 'simple', 'explode': False }})
-    r"""The ID of the ApiEndpoint to upsert."""
-    api_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'apiID', 'style': 'simple', 'explode': False }})
-    r"""The ID of the Api the ApiEndpoint belongs to."""
-    version_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'versionID', 'style': 'simple', 'explode': False }})
-    r"""The version ID of the Api the ApiEndpoint belongs to."""
-    
-
-
-
-@dataclasses.dataclass
-class UpsertAPIEndpointResponse:
-    content_type: str = dataclasses.field()
-    r"""HTTP response content type for this operation"""
-    status_code: int = dataclasses.field()
-    r"""HTTP response status code for this operation"""
-    raw_response: requests_http.Response = dataclasses.field()
-    r"""Raw HTTP response; suitable for custom response parsing"""
-    api_endpoint: Optional[shared_apiendpoint.APIEndpoint] = dataclasses.field(default=None)
-    r"""OK"""
-    error: Optional[errors_error.Error] = dataclasses.field(default=None)
-    r"""Default error response"""
+class APIInput:
+    r"""An Api is representation of a API (a collection of API Endpoints) within the Speakeasy Platform."""
+    api_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_id') }})
+    r"""The ID of this Api. This is a human-readable name (subject to change)."""
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
+    r"""A detailed description of the Api."""
+    version_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version_id') }})
+    r"""The version ID of this Api. This is semantic version identifier."""
+    meta_data: Optional[Dict[str, List[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_data'), 'exclude': lambda f: f is None }})
+    r"""A set of values associated with a meta_data key. This field is only set on get requests."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filter_.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from speakeasy import utils
-from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class APIInput:
-    r"""An Api is representation of a API (a collection of API Endpoints) within the Speakeasy Platform."""
-    api_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_id') }})
-    r"""The ID of this Api. This is a human-readable name (subject to change)."""
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    r"""A detailed description of the Api."""
-    version_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version_id') }})
-    r"""The version ID of this Api. This is semantic version identifier."""
-    meta_data: Optional[Dict[str, List[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_data'), 'exclude': lambda f: f is None }})
-    r"""A set of values associated with a meta_data key. This field is only set on get requests."""
+class Filter:
+    r"""A filter is a key-value pair that can be used to filter a list of requests."""
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
+    r"""The key of the filter."""
+    operator: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('operator') }})
+    r"""The operator of the filter."""
+    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
+    r"""The value of the filter."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from speakeasy import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Filter:
-    r"""A filter is a key-value pair that can be used to filter a list of requests."""
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    r"""The key of the filter."""
-    operator: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('operator') }})
-    r"""The operator of the filter."""
-    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    r"""The value of the filter."""
+class UnboundedRequest:
+    r"""An UnboundedRequest represents the HAR content capture by Speakeasy when logging a request."""
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    r"""Creation timestamp."""
+    har: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('har') }})
+    r"""The HAR content of the request."""
+    har_size_bytes: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('har_size_bytes') }})
+    r"""The size of the HAR content in bytes."""
+    request_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('request_id') }})
+    r"""The ID of this request."""
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_id') }})
+    r"""The workspace ID this request was made to."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from speakeasy import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UnboundedRequest:
-    r"""An UnboundedRequest represents the HAR content capture by Speakeasy when logging a request."""
+class VersionMetadata:
+    r"""A set of keys and associated values, attached to a particular version of an Api."""
+    api_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_id') }})
+    r"""The ID of the Api this Metadata belongs to."""
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     r"""Creation timestamp."""
-    har: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('har') }})
-    r"""The HAR content of the request."""
-    har_size_bytes: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('har_size_bytes') }})
-    r"""The size of the HAR content in bytes."""
-    request_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('request_id') }})
-    r"""The ID of this request."""
+    meta_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_key') }})
+    r"""The key for this metadata."""
+    meta_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_value') }})
+    r"""One of the values for this metadata."""
+    version_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version_id') }})
+    r"""The version ID of the Api this Metadata belongs to."""
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_id') }})
-    r"""The workspace ID this request was made to."""
+    r"""The workspace ID this Metadata belongs to."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from speakeasy import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class VersionMetadata:
+class VersionMetadataInput:
     r"""A set of keys and associated values, attached to a particular version of an Api."""
-    api_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_id') }})
-    r"""The ID of the Api this Metadata belongs to."""
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    r"""Creation timestamp."""
     meta_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_key') }})
     r"""The key for this metadata."""
     meta_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('meta_value') }})
     r"""One of the values for this metadata."""
-    version_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version_id') }})
-    r"""The version ID of the Api this Metadata belongs to."""
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace_id') }})
-    r"""The workspace ID this Metadata belongs to."""
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         r"""Generate a Postman collection for a particular request.
         Generates a Postman collection for a particular request. 
         Allowing it to be replayed with the same inputs that were captured by the SDK.
         """
         hook_ctx = HookContext(operation_id='generateRequestPostmanCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GenerateRequestPostmanCollectionRequest, base_url, '/v1/eventlog/{requestID}/generate/postman', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/eventlog/{requestID}/generate/postman', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         if accept_header_override is not None:
@@ -86,15 +86,15 @@
     
     
     def get_request_from_event_log(self, request: operations.GetRequestFromEventLogRequest) -> operations.GetRequestFromEventLogResponse:
         r"""Get information about a particular request."""
         hook_ctx = HookContext(operation_id='getRequestFromEventLog', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRequestFromEventLogRequest, base_url, '/v1/eventlog/{requestID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/eventlog/{requestID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -155,15 +155,15 @@
         url = base_url + '/v1/eventlog/query'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.QueryEventLogRequest, request, self.sdk_configuration.globals), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     
     def delete_schema(self, request: operations.DeleteSchemaRequest) -> operations.DeleteSchemaResponse:
         r"""Delete a particular schema revision for an Api."""
         hook_ctx = HookContext(operation_id='deleteSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteSchemaRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -80,15 +80,15 @@
     
     
     def download_schema(self, request: operations.DownloadSchemaRequest, accept_header_override: Optional[DownloadSchemaAcceptEnum] = None) -> operations.DownloadSchemaResponse:
         r"""Download the latest schema for a particular apiID."""
         hook_ctx = HookContext(operation_id='downloadSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DownloadSchemaRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema/download', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/download', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         if accept_header_override is not None:
@@ -143,15 +143,15 @@
     
     
     def download_schema_revision(self, request: operations.DownloadSchemaRevisionRequest, accept_header_override: Optional[DownloadSchemaRevisionAcceptEnum] = None) -> operations.DownloadSchemaRevisionResponse:
         r"""Download a particular schema revision for an Api."""
         hook_ctx = HookContext(operation_id='downloadSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DownloadSchemaRevisionRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}/download', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}/download', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         if accept_header_override is not None:
@@ -209,15 +209,15 @@
         r"""Get information about the latest schema.
         Returns information about the last uploaded schema for a particular API version. 
         This won't include the schema itself, that can be retrieved via the downloadSchema operation.
         """
         hook_ctx = HookContext(operation_id='getSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSchemaRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -268,15 +268,15 @@
     
     
     def get_schema_diff(self, request: operations.GetSchemaDiffRequest) -> operations.GetSchemaDiffResponse:
         r"""Get a diff of two schema revisions for an Api."""
         hook_ctx = HookContext(operation_id='getSchemaDiff', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSchemaDiffRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{baseRevisionID}/diff/{targetRevisionID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{baseRevisionID}/diff/{targetRevisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -330,15 +330,15 @@
         r"""Get information about a particular schema revision for an Api.
         Returns information about the last uploaded schema for a particular schema revision. 
         This won't include the schema itself, that can be retrieved via the downloadSchema operation.
         """
         hook_ctx = HookContext(operation_id='getSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSchemaRevisionRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -392,15 +392,15 @@
         r"""Get information about all schemas associated with a particular apiID.
         Returns information the schemas associated with a particular apiID. 
         This won't include the schemas themselves, they can be retrieved via the downloadSchema operation.
         """
         hook_ctx = HookContext(operation_id='getSchemas', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetSchemasRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schemas', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schemas', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -454,15 +454,15 @@
         r"""Register a schema.
         Allows uploading a schema for a particular API version.
         This will be used to populate ApiEndpoints and used as a base for any schema generation if present.
         """
         hook_ctx = HookContext(operation_id='registerSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RegisterSchemaRequest, base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterSchemaRequest, "request_body", False, False, 'multipart')
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .organizations import Organizations
 from .requests import Requests
 from .schemas import Schemas
 from .sdkconfiguration import SDKConfiguration
 from .utils.retries import RetryConfig
 from speakeasy import utils
 from speakeasy._hooks import SDKHooks
-from speakeasy.models import shared
+from speakeasy.models import internal, shared
 from typing import Callable, Dict, Optional, Union
 
 class Speakeasy:
     r"""Speakeasy API: The Speakeasy API allows teams to manage common operations with their APIs
     /docs - The Speakeasy Platform Documentation
     """
     apis: Apis
@@ -69,44 +69,37 @@
         """
         if client is None:
             client = requests_http.Session()
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
-        global_params = {
-            'parameters': {
-                'queryParam': {
-                },
-                'pathParam': {
-                    'workspace_id': workspace_id,
-                },
-                'header': {
-                },
-            },
-        }
+    
+        _globals = internal.Globals(
+            workspace_id=workspace_id,
+        )
 
         self.sdk_configuration = SDKConfiguration(
             client,
+            _globals,
             security,
             server_url,
             server,
-            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.apis = Apis(self.sdk_configuration)
         self.api_endpoints = APIEndpoints(self.sdk_configuration)
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/sdkconfiguration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
-from dataclasses import dataclass, field
-from speakeasy.models import shared
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from dataclasses import dataclass
+from speakeasy.models import internal, shared
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVER_PROD = 'prod'
 SERVERS = {
 	SERVER_PROD: 'https://api.prod.speakeasyapi.dev',
 }
 """Contains the list of servers available to the SDK"""
 
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
+    globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
-    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.6.3'
-    gen_version: str = '2.300.0'
-    user_agent: str = 'speakeasy-sdk/python 5.6.3 2.300.0 0.4.0 speakeasy-client-sdk-python'
+    sdk_version: str = '5.6.4'
+    gen_version: str = '2.301.0'
+    user_agent: str = 'speakeasy-sdk/python 5.6.4 2.301.0 0.4.0 speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
-    _hooks: Optional[SDKHooks] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if not self.server:
             self.server = SERVER_PROD
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _populate_from_globals(field.name, getattr(headers_params, field.name), 'header', gbls)
-        value = _serialize_header(metadata.get('explode', False), value)
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.shared'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.shared"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.3
+Version: 5.6.4
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.3/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.6.4/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 src/speakeasy/_hooks/registration.py
 src/speakeasy/_hooks/sdkhooks.py
 src/speakeasy/_hooks/types.py
 src/speakeasy/models/__init__.py
 src/speakeasy/models/errors/__init__.py
 src/speakeasy/models/errors/error.py
 src/speakeasy/models/errors/sdkerror.py
+src/speakeasy/models/internal/__init__.py
+src/speakeasy/models/internal/globals.py
 src/speakeasy/models/operations/__init__.py
 src/speakeasy/models/operations/deleteapi.py
 src/speakeasy/models/operations/deleteapiendpoint.py
 src/speakeasy/models/operations/deleteschema.py
 src/speakeasy/models/operations/deleteversionmetadata.py
 src/speakeasy/models/operations/downloadschema.py
 src/speakeasy/models/operations/downloadschemarevision.py
```

