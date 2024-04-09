# Comparing `tmp/splight_lib-5.5.5.tar.gz` & `tmp/splight_lib-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight_lib-5.5.5.tar", max compression
+gzip compressed data, was "splight_lib-5.6.0.tar", max compression
```

## Comparing `splight_lib-5.5.5.tar` & `splight_lib-5.6.0.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0        0 2024-04-03 14:07:11.860788 splight_lib-5.5.5/LICENSE.txt
--rw-r--r--   0        0        0     1108 2024-04-03 14:07:11.860788 splight_lib-5.5.5/README.md
--rw-r--r--   0        0        0     1516 2024-04-03 14:07:11.860788 splight_lib-5.5.5/pyproject.toml
--rw-r--r--   0        0        0      114 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/abstract/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/abstract/client.py
--rw-r--r--   0        0        0      160 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/auth/__init__.py
--rw-r--r--   0        0        0      404 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/auth/exceptions.py
--rw-r--r--   0        0        0     2944 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/auth/mac_auth.py
--rw-r--r--   0        0        0      224 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/auth/token.py
--rw-r--r--   0        0        0        0 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/__init__.py
--rw-r--r--   0        0        0      358 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/__init__.py
--rw-r--r--   0        0        0      785 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/abstract.py
--rw-r--r--   0        0        0      582 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/builder.py
--rw-r--r--   0        0        0     1209 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/classmap.py
--rw-r--r--   0        0        0     6192 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/local_client.py
--rw-r--r--   0        0        0    10955 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/database/remote_client.py
--rw-r--r--   0        0        0      474 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/__init__.py
--rw-r--r--   0        0        0     1878 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/abstract.py
--rw-r--r--   0        0        0     1649 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/buffer.py
--rw-r--r--   0        0        0      944 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/builder.py
--rw-r--r--   0        0        0      210 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/exceptions.py
--rw-r--r--   0        0        0     3728 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/local_client.py
--rw-r--r--   0        0        0    13405 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0        0        0     1503 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/datalake/schemas.py
--rw-r--r--   0        0        0      948 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/exceptions.py
--rw-r--r--   0        0        0      981 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/file_handler.py
--rw-r--r--   0        0        0      595 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/filter.py
--rw-r--r--   0        0        0       96 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/hub/__init__.py
--rw-r--r--   0        0        0      803 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/hub/abstract.py
--rw-r--r--   0        0        0     4681 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/hub/client.py
--rw-r--r--   0        0        0     5218 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/tests/test_database.py
--rw-r--r--   0        0        0     1623 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/client/tests/test_datalake.py
--rw-r--r--   0        0        0      105 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/component/__init__.py
--rw-r--r--   0        0        0     6963 2024-04-03 14:07:11.860788 splight_lib-5.5.5/splight_lib/component/abstract.py
--rw-r--r--   0        0        0      480 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/component/exceptions.py
--rw-r--r--   0        0        0     7844 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/component/spec.py
--rw-r--r--   0        0        0       49 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/component/tests/test_abstract.py
--rw-r--r--   0        0        0     4115 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/component/tests/test_spec.py
--rw-r--r--   0        0        0      183 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/constants.py
--rw-r--r--   0        0        0     2002 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/encryption.py
--rw-r--r--   0        0        0      303 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/__init__.py
--rw-r--r--   0        0        0     3988 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/engine.py
--rw-r--r--   0        0        0      282 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/exceptions.py
--rw-r--r--   0        0        0     2990 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/scheduling.py
--rw-r--r--   0        0        0     1932 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/task.py
--rw-r--r--   0        0        0     1034 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/tests/test_execution.py
--rw-r--r--   0        0        0     1048 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/tests/test_scheduling.py
--rw-r--r--   0        0        0     1302 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/execution/trigger.py
--rw-r--r--   0        0        0      192 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/__init__.py
--rw-r--r--   0        0        0     1516 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/_internal.py
--rw-r--r--   0        0        0     1426 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/component.py
--rw-r--r--   0        0        0      130 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/constants.py
--rw-r--r--   0        0        0     4881 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/logging.py
--rw-r--r--   0        0        0     4316 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/logging/tests/test_logging.py
--rw-r--r--   0        0        0     1198 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/__init__.py
--rw-r--r--   0        0        0     7791 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/alert.py
--rw-r--r--   0        0        0     1600 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/asset.py
--rw-r--r--   0        0        0      452 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/attribute.py
--rw-r--r--   0        0        0     6118 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/base.py
--rw-r--r--   0        0        0    18782 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/component.py
--rw-r--r--   0        0        0     2857 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/dashboard.py
--rw-r--r--   0        0        0     1024 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/data_address.py
--rw-r--r--   0        0        0      634 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/exceptions.py
--rw-r--r--   0        0        0     1869 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/file.py
--rw-r--r--   0        0        0     6710 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/function.py
--rw-r--r--   0        0        0      790 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/generic.py
--rw-r--r--   0        0        0     7153 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/hub.py
--rw-r--r--   0        0        0      606 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/metadata.py
--rw-r--r--   0        0        0     2162 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/native.py
--rw-r--r--   0        0        0     2398 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/pipeline.py
--rw-r--r--   0        0        0      487 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/secret.py
--rw-r--r--   0        0        0    11054 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/tests/models.json
--rw-r--r--   0        0        0     2376 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/tests/test_component_object_instance.py
--rw-r--r--   0        0        0     3575 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/tests/test_database_model.py
--rw-r--r--   0        0        0     1389 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/tests/test_metadata.py
--rw-r--r--   0        0        0      823 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/models/tests/test_models.py
--rw-r--r--   0        0        0      212 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/restclient/__init__.py
--rw-r--r--   0        0        0    16872 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/restclient/client.py
--rw-r--r--   0        0        0      964 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/restclient/exceptions.py
--rw-r--r--   0        0        0     1117 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/restclient/tests/test_restclient.py
--rw-r--r--   0        0        0     2386 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/restclient/types.py
--rw-r--r--   0        0        0     3586 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/settings.py
--rw-r--r--   0        0        0      427 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/stringcase.py
--rw-r--r--   0        0        0     2834 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/testing/__init__.py
--rw-r--r--   0        0        0      251 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/tests/FakeProc.py
--rw-r--r--   0        0        0     5885 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/tests/asset_geometries.json
--rw-r--r--   0        0        0     5400 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/tests/test_api_contracts.py
--rw-r--r--   0        0        0       41 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/tests/test_encryption.py
--rw-r--r--   0        0        0        0 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/utils/__init__.py
--rw-r--r--   0        0        0     2297 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/utils/custom_model.py
--rw-r--r--   0        0        0      626 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/utils/hub.py
--rw-r--r--   0        0        0       78 2024-04-03 14:07:11.864788 splight_lib-5.5.5/splight_lib/version.py
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.5.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 13:57:52.603405 splight_lib-5.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1108 2024-04-09 13:57:52.603405 splight_lib-5.6.0/README.md
+-rw-r--r--   0        0        0     1532 2024-04-09 13:57:52.603405 splight_lib-5.6.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/abstract/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/abstract/client.py
+-rw-r--r--   0        0        0      160 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/auth/__init__.py
+-rw-r--r--   0        0        0      404 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/auth/exceptions.py
+-rw-r--r--   0        0        0     2944 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0        0        0      224 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/auth/token.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/abstract.py
+-rw-r--r--   0        0        0      582 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/builder.py
+-rw-r--r--   0        0        0     1277 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/classmap.py
+-rw-r--r--   0        0        0     6192 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/local_client.py
+-rw-r--r--   0        0        0    11810 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/database/remote_client.py
+-rw-r--r--   0        0        0      474 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0        0        0     1878 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0        0        0     1649 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/buffer.py
+-rw-r--r--   0        0        0      944 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0        0        0      210 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/exceptions.py
+-rw-r--r--   0        0        0     3728 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0        0        0    13405 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0        0        0     1503 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/datalake/schemas.py
+-rw-r--r--   0        0        0      948 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/exceptions.py
+-rw-r--r--   0        0        0      981 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/file_handler.py
+-rw-r--r--   0        0        0      595 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/filter.py
+-rw-r--r--   0        0        0       96 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0        0        0     4662 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/hub/client.py
+-rw-r--r--   0        0        0     5218 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/tests/test_database.py
+-rw-r--r--   0        0        0     1623 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/client/tests/test_datalake.py
+-rw-r--r--   0        0        0      105 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/component/__init__.py
+-rw-r--r--   0        0        0     6963 2024-04-09 13:57:52.603405 splight_lib-5.6.0/splight_lib/component/abstract.py
+-rw-r--r--   0        0        0      480 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/component/exceptions.py
+-rw-r--r--   0        0        0     7844 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/component/spec.py
+-rw-r--r--   0        0        0       49 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/component/tests/test_abstract.py
+-rw-r--r--   0        0        0     4115 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/component/tests/test_spec.py
+-rw-r--r--   0        0        0      210 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/constants.py
+-rw-r--r--   0        0        0     2002 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/encryption.py
+-rw-r--r--   0        0        0      303 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/__init__.py
+-rw-r--r--   0        0        0     3988 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/engine.py
+-rw-r--r--   0        0        0      282 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/exceptions.py
+-rw-r--r--   0        0        0     2990 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/scheduling.py
+-rw-r--r--   0        0        0     1932 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/task.py
+-rw-r--r--   0        0        0     1034 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/tests/test_execution.py
+-rw-r--r--   0        0        0     1048 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/tests/test_scheduling.py
+-rw-r--r--   0        0        0     1302 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/execution/trigger.py
+-rw-r--r--   0        0        0      192 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/__init__.py
+-rw-r--r--   0        0        0     1516 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/_internal.py
+-rw-r--r--   0        0        0     1426 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/component.py
+-rw-r--r--   0        0        0      130 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/constants.py
+-rw-r--r--   0        0        0     4881 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/logging.py
+-rw-r--r--   0        0        0     4316 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/logging/tests/test_logging.py
+-rw-r--r--   0        0        0     1271 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/__init__.py
+-rw-r--r--   0        0        0     7791 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/alert.py
+-rw-r--r--   0        0        0     1600 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/asset.py
+-rw-r--r--   0        0        0      452 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/attribute.py
+-rw-r--r--   0        0        0     6362 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/base.py
+-rw-r--r--   0        0        0    18782 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/component.py
+-rw-r--r--   0        0        0     2857 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/dashboard.py
+-rw-r--r--   0        0        0     1024 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/data_address.py
+-rw-r--r--   0        0        0      634 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/exceptions.py
+-rw-r--r--   0        0        0     1869 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/file.py
+-rw-r--r--   0        0        0     6710 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/function.py
+-rw-r--r--   0        0        0      790 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/generic.py
+-rw-r--r--   0        0        0     7153 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/hub.py
+-rw-r--r--   0        0        0     1098 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/hub_solution.py
+-rw-r--r--   0        0        0      606 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/metadata.py
+-rw-r--r--   0        0        0     2162 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/native.py
+-rw-r--r--   0        0        0     2398 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/pipeline.py
+-rw-r--r--   0        0        0      487 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/secret.py
+-rw-r--r--   0        0        0    11054 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/tests/models.json
+-rw-r--r--   0        0        0     2376 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/tests/test_component_object_instance.py
+-rw-r--r--   0        0        0     3575 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/tests/test_database_model.py
+-rw-r--r--   0        0        0     1389 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/tests/test_metadata.py
+-rw-r--r--   0        0        0      823 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/models/tests/test_models.py
+-rw-r--r--   0        0        0      212 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/restclient/__init__.py
+-rw-r--r--   0        0        0    16872 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/restclient/client.py
+-rw-r--r--   0        0        0      964 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0        0        0     1108 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/restclient/tests/test_restclient.py
+-rw-r--r--   0        0        0     2386 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/restclient/types.py
+-rw-r--r--   0        0        0     3586 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/settings.py
+-rw-r--r--   0        0        0      427 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/stringcase.py
+-rw-r--r--   0        0        0     2834 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/testing/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/tests/FakeProc.py
+-rw-r--r--   0        0        0     5885 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/tests/asset_geometries.json
+-rw-r--r--   0        0        0     5400 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/tests/test_api_contracts.py
+-rw-r--r--   0        0        0       41 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/tests/test_encryption.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/utils/__init__.py
+-rw-r--r--   0        0        0     2297 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/utils/custom_model.py
+-rw-r--r--   0        0        0      626 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/utils/hub.py
+-rw-r--r--   0        0        0       78 2024-04-09 13:57:52.607405 splight_lib-5.6.0/splight_lib/version.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.6.0/PKG-INFO
```

### Comparing `splight_lib-5.5.5/README.md` & `splight_lib-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/pyproject.toml` & `splight_lib-5.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splight-lib"
-version = "5.5.5"
+version = "5.6.0"
 description = "Splight Library"
 authors = ["Splight Dev <dev@splight-ae.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 concurrent-log-handler = "0.9.21"
@@ -43,14 +43,15 @@
 flake8 = "^6.1.0"
 pre-commit = "3.2.2"
 pytest = "^7.4.3"
 jsonref = "1.1.0"
 polyfactory = "2.13.0"
 openapi-schema-validator = "0.6.2"
 pytest-mock = "^3.12.0"
+ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `splight_lib-5.5.5/splight_lib/abstract/client.py` & `splight_lib-5.6.0/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/auth/mac_auth.py` & `splight_lib-5.6.0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/database/abstract.py` & `splight_lib-5.6.0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/database/builder.py` & `splight_lib-5.6.0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/database/classmap.py` & `splight_lib-5.6.0/splight_lib/client/database/classmap.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from splight_lib.constants import ENGINE_PREFIX
+from splight_lib.constants import ENGINE_PREFIX, HUB_PREFIX
 
 MODEL_NAME_MAP = {
     "advancedfilter": f"{ENGINE_PREFIX}/alert/advancedfilters/",
     "alert": f"{ENGINE_PREFIX}/alert/alerts/",
     "asset": f"{ENGINE_PREFIX}/assets/",
     "attribute": f"{ENGINE_PREFIX}/attributes/",
     "metadata": f"{ENGINE_PREFIX}/metadata/",
@@ -15,14 +15,15 @@
     "filter": f"{ENGINE_PREFIX}/dashboard/filters/",
     "function": f"{ENGINE_PREFIX}/function/functions/",
     "query": f"{ENGINE_PREFIX}/queries/",
     "routineobject": f"{ENGINE_PREFIX}/component/routines/",
     "secret": f"{ENGINE_PREFIX}/secrets/",
     "setpoint": f"{ENGINE_PREFIX}/setpoints/",
     "tab": f"{ENGINE_PREFIX}/dashboard/tabs/",
+    "hubsolution": f"{HUB_PREFIX}/solution/solutions/",
 }
 
 CUSTOM_PATHS_MAP = {
     "set-asset-attribute": "{prefix}/assets/{asset}/set-attribute/",
     "get-asset-attribute": "{prefix}/assets/{asset}/get-attribute/",
     "decrypt-secret": "{prefix}/secrets/decrypt/",
 }
```

### Comparing `splight_lib-5.5.5/splight_lib/client/database/local_client.py` & `splight_lib-5.6.0/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/database/remote_client.py` & `splight_lib-5.6.0/splight_lib/client/database/remote_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,37 +58,47 @@
         self._restclient = SplightRestClient()
         self._restclient.update_headers(token.header)
         logger.debug(
             "Remote database client initialized.", tags=LogTags.DATABASE
         )
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
-    def save(self, resource_name: str, instance: Dict) -> Dict:
+    def save(
+        self,
+        resource_name: str,
+        instance: Dict,
+        files: Optional[Dict[str, str]] = None,
+    ) -> Dict:
         """Creates or updates a resource depending on the name if
         it contains the id or not.
 
         Parameters
         ----------
         resource_name: str
             The name of the resource to be created or updated.
         instance : Dict
             A dictionary with resource to be created or updated
+        files: Optional[Dict[str, srt]] = None
+            A dictionary with the name and the file path to the files to be
+            pushed
 
         Returns
         -------
         Dict with the created or updated resource.
 
         Raises
         ------
         InvalidModelName thrown when the model name is not correct.
         """
         if instance.get("id"):
-            output = self._update(resource_name, instance["id"], instance)
+            output = self._update(
+                resource_name, instance["id"], instance, files
+            )
         else:
-            output = self._create(resource_name, instance)
+            output = self._create(resource_name, instance, files)
         return output
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def delete(self, resource_name: str, id: str):
         """Deletes a resource from the database
 
         Parameters
@@ -242,43 +252,66 @@
 
     def _list(self, url: furl, **kwargs) -> PaginatedResponse:
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
         response.raise_for_status()
         return response.json()
 
-    def _create(self, resource_name: str, instance: Dict) -> Dict:
+    def _create(
+        self,
+        resource_name: str,
+        instance: Dict,
+        files: Optional[Dict[str, str]] = None,
+    ) -> Dict:
         logger.debug("Saving new instance", tags=LogTags.DATABASE)
         model_name = resource_name.lower()
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path
         if model_name == "file":
             instance = self._create_file(instance, url)
         else:
-            response = self._restclient.post(url, json=instance)
+            files_payload = (
+                {key: open(value, "rb") for key, value in files.items()}
+                if files
+                else None
+            )
+            response = self._restclient.post(
+                url, data=instance, files=files_payload
+            )
             response.raise_for_status()
             instance = response.json()
         logger.debug(
             "Instance %s created", instance["id"], tags=LogTags.DATABASE
         )
         return instance
 
     def _update(
-        self, resource_name: str, resource_id: str, instance: Dict
+        self,
+        resource_name: str,
+        resource_id: str,
+        instance: Dict,
+        files: Optional[Dict[str, str]] = None,
     ) -> Dict:
         logger.debug("Saving instance %s", resource_id, tags=LogTags.DATABASE)
         model_name = resource_name.lower()
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path / f"{resource_id}/"
         if model_name == "file":
             with open(instance["file"], "rb") as f:
                 file = {"file": f}
                 response = self._restclient.put(url, data=instance, files=file)
         else:
-            response = self._restclient.put(url, json=instance)
+            files_payload = (
+                {key: open(value, "rb") for key, value in files.items()}
+                if files
+                else None
+            )
+            response = self._restclient.put(
+                url, data=instance, files=files_payload
+            )
 
         response.raise_for_status()
         return response.json()
 
     def _create_file(self, instance: Dict, url: furl):
         response = self._restclient.post(url, data=instance)
         response.raise_for_status()
```

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/abstract.py` & `splight_lib-5.6.0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/buffer.py` & `splight_lib-5.6.0/splight_lib/client/datalake/buffer.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/builder.py` & `splight_lib-5.6.0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/local_client.py` & `splight_lib-5.6.0/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/remote_client.py` & `splight_lib-5.6.0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/datalake/schemas.py` & `splight_lib-5.6.0/splight_lib/client/datalake/schemas.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/exceptions.py` & `splight_lib-5.6.0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/file_handler.py` & `splight_lib-5.6.0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/filter.py` & `splight_lib-5.6.0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/hub/abstract.py` & `splight_lib-5.6.0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/hub/client.py` & `splight_lib-5.6.0/splight_lib/client/hub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import json
 from tempfile import NamedTemporaryFile
-from typing import Dict, List, Tuple
+from typing import Dict, List
 
 import progressbar
 import requests
 from furl import furl
 from pydantic import BaseModel
 
 from splight_lib.auth import SplightAuthToken
```

### Comparing `splight_lib-5.5.5/splight_lib/client/tests/test_database.py` & `splight_lib-5.6.0/splight_lib/client/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/client/tests/test_datalake.py` & `splight_lib-5.6.0/splight_lib/client/tests/test_datalake.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/component/abstract.py` & `splight_lib-5.6.0/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/component/spec.py` & `splight_lib-5.6.0/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/component/tests/test_spec.py` & `splight_lib-5.6.0/splight_lib/component/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/encryption.py` & `splight_lib-5.6.0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/engine.py` & `splight_lib-5.6.0/splight_lib/execution/engine.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/scheduling.py` & `splight_lib-5.6.0/splight_lib/execution/scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/task.py` & `splight_lib-5.6.0/splight_lib/execution/task.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/tests/test_execution.py` & `splight_lib-5.6.0/splight_lib/execution/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/tests/test_scheduling.py` & `splight_lib-5.6.0/splight_lib/execution/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/execution/trigger.py` & `splight_lib-5.6.0/splight_lib/execution/trigger.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/logging/_internal.py` & `splight_lib-5.6.0/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/logging/component.py` & `splight_lib-5.6.0/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/logging/logging.py` & `splight_lib-5.6.0/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/logging/tests/test_logging.py` & `splight_lib-5.6.0/splight_lib/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/__init__.py` & `splight_lib-5.6.0/splight_lib/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Dashboard,
     Filter,
     Tab,
 )
 from splight_lib.models.file import File
 from splight_lib.models.function import Function, FunctionItem, QueryFilter
 from splight_lib.models.hub import HubComponent
+from splight_lib.models.hub_solution import HubSolution
 from splight_lib.models.metadata import Metadata
 from splight_lib.models.native import Boolean, Number, String
 from splight_lib.models.secret import Secret
 
 __all__ = [
     AdvancedFilter,
     Alert,
@@ -37,16 +38,17 @@
     ComponentObject,
     ComponentObjectInstance,
     Dashboard,
     File,
     Filter,
     Function,
     FunctionItem,
-    QueryFilter,
+    HubSolution,
     HubComponent,
+    QueryFilter,
     Metadata,
     Number,
     RoutineEvaluation,
     String,
     Secret,
     RoutineObject,
     RoutineObjectInstance,
```

### Comparing `splight_lib-5.5.5/splight_lib/models/alert.py` & `splight_lib-5.6.0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/asset.py` & `splight_lib-5.6.0/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/base.py` & `splight_lib-5.6.0/splight_lib/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from datetime import datetime, timezone
-from typing import ClassVar, Dict, List
+from pathlib import Path
+from typing import ClassVar, Dict, List, Optional, TypeVar
 
 import pandas as pd
 from pydantic import BaseModel, ConfigDict, Field, PrivateAttr
 
 from splight_lib.client.database import DatabaseClientBuilder
 from splight_lib.client.database.abstract import AbstractDatabaseClient
 from splight_lib.client.datalake import DatalakeClientBuilder
@@ -15,30 +16,35 @@
 def datalake_model_serializer(data: Dict, default=str, **dumps_kwargs):
     new_data = {
         k: v if not isinstance(v, dict) else v["id"] for k, v in data.items()
     }
     return json.dumps(new_data, default=default, **dumps_kwargs)
 
 
+FilePath = TypeVar("FilePath", str, Path)
+
+
 class SplightDatabaseBaseModel(BaseModel):
     _db_client: AbstractDatabaseClient = PrivateAttr()
 
     def __init__(self, **data):
         super().__init__(**data)
         self._db_client = self.__get_database_client()
 
     @staticmethod
     def get_event_name(type_: str, action: str) -> str:
         return f"{type_.lower()}-{action.lower()}"
 
     def save(self):
+        files_dict = self._get_model_files_dict()
         saved = self._db_client.save(
             self.__class__.__name__,
             # TODO: improve the following line
             json.loads(self.model_dump_json(exclude_none=True)),
+            files=files_dict,
         )
         if not self.id:
             self.id = saved["id"]
 
     def delete(self):
         self._db_client.delete(
             resource_name=self.__class__.__name__, id=self.id
@@ -68,14 +74,17 @@
                 "base_url": settings.SPLIGHT_PLATFORM_API_HOST,
                 "access_id": settings.SPLIGHT_ACCESS_ID,
                 "secret_key": settings.SPLIGHT_SECRET_KEY,
             },
         )
         return db_client
 
+    def _get_model_files_dict(self) -> Optional[Dict]:
+        return None
+
 
 class SplightDatalakeBaseModel(BaseModel):
     timestamp: datetime = Field(
         default_factory=lambda: datetime.now(timezone.utc)
     )
     _collection_name: ClassVar[str] = "DatalakeModel"
     _dl_client: AbstractDatalakeClient = PrivateAttr()
```

### Comparing `splight_lib-5.5.5/splight_lib/models/component.py` & `splight_lib-5.6.0/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/dashboard.py` & `splight_lib-5.6.0/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/data_address.py` & `splight_lib-5.6.0/splight_lib/models/data_address.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/exceptions.py` & `splight_lib-5.6.0/splight_lib/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/file.py` & `splight_lib-5.6.0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/function.py` & `splight_lib-5.6.0/splight_lib/models/function.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/generic.py` & `splight_lib-5.6.0/splight_lib/models/generic.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/hub.py` & `splight_lib-5.6.0/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/metadata.py` & `splight_lib-5.6.0/splight_lib/models/metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/native.py` & `splight_lib-5.6.0/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/pipeline.py` & `splight_lib-5.6.0/splight_lib/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/tests/models.json` & `splight_lib-5.6.0/splight_lib/models/tests/models.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/tests/test_component_object_instance.py` & `splight_lib-5.6.0/splight_lib/models/tests/test_component_object_instance.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/tests/test_database_model.py` & `splight_lib-5.6.0/splight_lib/models/tests/test_database_model.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/tests/test_metadata.py` & `splight_lib-5.6.0/splight_lib/models/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/models/tests/test_models.py` & `splight_lib-5.6.0/splight_lib/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/restclient/client.py` & `splight_lib-5.6.0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/restclient/exceptions.py` & `splight_lib-5.6.0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/restclient/tests/test_restclient.py` & `splight_lib-5.6.0/splight_lib/restclient/tests/test_restclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,10 +26,9 @@
     session_response = getattr(_session, method)(url)
     requests_response = getattr(_requests, method)(url)
 
     assert (
         getattr(restclient_response, attr)
         == getattr(httpx_response, attr)
         == getattr(session_response, attr)
-        == getattr(requests_response, attr),
-        f"Error in {attr} atributte.",
-    )
+        == getattr(requests_response, attr)
+    ), f"Error in {attr} atributte."
```

### Comparing `splight_lib-5.5.5/splight_lib/restclient/types.py` & `splight_lib-5.6.0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/settings.py` & `splight_lib-5.6.0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/testing/__init__.py` & `splight_lib-5.6.0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/tests/asset_geometries.json` & `splight_lib-5.6.0/splight_lib/tests/asset_geometries.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/tests/test_api_contracts.py` & `splight_lib-5.6.0/splight_lib/tests/test_api_contracts.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/utils/custom_model.py` & `splight_lib-5.6.0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/splight_lib/utils/hub.py` & `splight_lib-5.6.0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.5.5/PKG-INFO` & `splight_lib-5.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 5.5.5
+Version: 5.6.0
 Summary: Splight Library
 Author: Splight Dev
 Author-email: dev@splight-ae.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

