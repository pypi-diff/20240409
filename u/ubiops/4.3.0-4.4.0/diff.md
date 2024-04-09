# Comparing `tmp/ubiops-4.3.0.tar.gz` & `tmp/ubiops-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiops-4.3.0.tar", last modified: Thu Jan 25 09:53:31 2024, max compression
+gzip compressed data, was "ubiops-4.4.0.tar", last modified: Tue Apr  9 07:52:46 2024, max compression
```

## Comparing `ubiops-4.3.0.tar` & `ubiops-4.4.0.tar`

### file list

```diff
@@ -1,220 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.512558 ubiops-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-25 09:53:19.000000 ubiops-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-25 09:53:31.512558 ubiops-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47820 2024-01-25 09:53:19.000000 ubiops-4.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-25 09:53:31.512558 ubiops-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-01-25 09:53:19.000000 ubiops-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.480558 ubiops-4.3.0/ubiops/
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.488558 ubiops-4.3.0/ubiops/api/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/blobs.py
--rw-r--r--   0 runner    (1001) docker     (127)   282293 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    90527 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/deployment_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)   139344 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    68268 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    43724 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/imports_and_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    41920 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    85253 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/pipeline_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    56252 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/request_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)    38898 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    24173 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/service_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    28746 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23968 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.508558 ubiops-4.3.0/ubiops/models/
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/attachment_fields_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/attachment_sources_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/attachments_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/attachments_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/audit_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/blob_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/bucket_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/bucket_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/bucket_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/bucket_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/build_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_output_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_batch_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_batch_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_single_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_request_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    20769 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_version_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    32804 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_version_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/deployment_version_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/direct_pipeline_request_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/direct_pipeline_request_operator_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/direct_pipeline_request_pipeline_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_build_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_build_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_build_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_revision_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_revision_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_variable_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_variable_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/environment_variable_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/export_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/export_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/export_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/expression_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/expression_evaluate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/expression_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/file_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/file_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/file_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/import_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/import_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/inherited_environment_variable_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/input_field_widget_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/input_output_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/input_output_field_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/input_output_field_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/input_output_widget_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/logs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/metric_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/metric_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/metric_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/notification_group_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/notification_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/notification_group_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/notification_group_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14399 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/operator_request_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_project_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/organization_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/output_field_widget_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/output_value_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/permission_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_input_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_output_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_batch_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_deployment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18204 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_operator_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_pipeline_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    20488 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_request_single_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_object_configuration_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_object_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_object_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/pipeline_version_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_deployment_version_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/project_user_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/quota_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/requests_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/resource_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/revision_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/revision_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_assignment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_detail_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/schedule_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/schedule_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/service_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/service_user_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/service_user_token_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/service_user_token_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/template_deployment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/time_series_data_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/time_series_data_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/time_series_data_point_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/time_series_data_point_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/time_series_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/user_pending_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/user_pending_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_test_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/models/webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.512558 ubiops-4.3.0/ubiops/training/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_run_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/experiment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    38546 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/training/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.512558 ubiops-4.3.0/ubiops/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.512558 ubiops-4.3.0/ubiops/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/metrics/metric_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/metrics/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/run_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.512558 ubiops-4.3.0/ubiops/utils/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/validators/validate_requirements_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/validators/validate_yaml_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-01-25 09:53:19.000000 ubiops-4.3.0/ubiops/utils/wait_for.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 09:53:31.480558 ubiops-4.3.0/ubiops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-25 09:53:31.000000 ubiops-4.3.0/ubiops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-01-25 09:53:31.000000 ubiops-4.3.0/ubiops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 09:53:31.000000 ubiops-4.3.0/ubiops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-25 09:53:31.000000 ubiops-4.3.0/ubiops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-25 09:53:31.000000 ubiops-4.3.0/ubiops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 07:52:36.000000 ubiops-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 07:52:46.221026 ubiops-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48602 2024-04-09 07:52:36.000000 ubiops-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 07:52:46.221026 ubiops-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 07:52:36.000000 ubiops-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.189026 ubiops-4.4.0/ubiops/
+-rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.197026 ubiops-4.4.0/ubiops/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286653 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90527 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/deployment_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139344 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68268 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53403 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43724 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/imports_and_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45097 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85253 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/pipeline_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56252 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83552 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/request_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38898 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24173 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/service_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28746 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23968 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.217026 ubiops-4.4.0/ubiops/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachment_fields_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachment_sources_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachments_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/attachments_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/audit_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/blob_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/bucket_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/build_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_output_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_batch_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_batch_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_single_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_request_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33911 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30739 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21760 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/deployment_version_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_operator_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/direct_pipeline_request_pipeline_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_build_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20218 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_revision_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_revision_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/environment_variable_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/export_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_evaluate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/expression_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_complete_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/file_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/import_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/inherited_environment_variable_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_field_widget_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_field_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/input_output_widget_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/logs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/metric_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/notification_group_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14399 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/operator_request_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/organization_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/output_field_widget_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/output_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/permission_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_input_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_output_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_batch_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_deployment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18204 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_operator_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_pipeline_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20488 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_request_single_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17386 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_configuration_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_object_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/pipeline_version_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_deployment_version_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/project_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/quota_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/requests_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/resource_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/revision_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/revision_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_assignment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_detail_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/schedule_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_token_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/service_user_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/template_deployment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_point_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_data_point_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/time_series_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/user_pending_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/user_pending_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/voucher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_test_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/models/webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_run_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/experiment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39257 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/training/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14550 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/metric_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/metrics/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/run_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.221026 ubiops-4.4.0/ubiops/utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/validate_requirements_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/validators/validate_yaml_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33908 2024-04-09 07:52:36.000000 ubiops-4.4.0/ubiops/utils/wait_for.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:52:46.193026 ubiops-4.4.0/ubiops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-09 07:52:46.000000 ubiops-4.4.0/ubiops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 07:52:45.000000 ubiops-4.4.0/ubiops.egg-info/top_level.txt
```

### Comparing `ubiops-4.3.0/LICENSE` & `ubiops-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/PKG-INFO` & `ubiops-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 4.3.0
+Version: 4.4.0
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-4.3.0/README.md` & `ubiops-4.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [www.ubiops.com](https://ubiops.com)
 
 Client Library to interact with the UbiOps API.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v2.1
-- Package version: 4.3.0
+- Package version: 4.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://ubiops.com/docs](https://ubiops.com/docs)
 
 ## Requirements.
 
 Python 3.7+
@@ -180,18 +180,20 @@
 *Environments* | [**environments_update**](docs/Environments.md#environments_update) | **PATCH** /projects/{project_name}/environments/{environment_name} | Update environment
 *Environments* | [**environments_usage**](docs/Environments.md#environments_usage) | **GET** /projects/{project_name}/environments/{environment_name}/usage | List usage of environment
 *Files* | [**buckets_create**](docs/Files.md#buckets_create) | **POST** /projects/{project_name}/buckets | Create bucket
 *Files* | [**buckets_delete**](docs/Files.md#buckets_delete) | **DELETE** /projects/{project_name}/buckets/{bucket_name} | Delete a bucket
 *Files* | [**buckets_get**](docs/Files.md#buckets_get) | **GET** /projects/{project_name}/buckets/{bucket_name} | Get details of a bucket
 *Files* | [**buckets_list**](docs/Files.md#buckets_list) | **GET** /projects/{project_name}/buckets | List buckets
 *Files* | [**buckets_update**](docs/Files.md#buckets_update) | **PATCH** /projects/{project_name}/buckets/{bucket_name} | Update a bucket
+*Files* | [**files_complete_multipart_upload**](docs/Files.md#files_complete_multipart_upload) | **POST** /projects/{project_name}/buckets/{bucket_name}/files/{file}/complete-multipart-upload | Complete multipart upload
 *Files* | [**files_delete**](docs/Files.md#files_delete) | **DELETE** /projects/{project_name}/buckets/{bucket_name}/files/{file} | Delete a file
 *Files* | [**files_download**](docs/Files.md#files_download) | **GET** /projects/{project_name}/buckets/{bucket_name}/files/{file}/download | Download a file
 *Files* | [**files_get**](docs/Files.md#files_get) | **GET** /projects/{project_name}/buckets/{bucket_name}/files/{file} | Get a file
 *Files* | [**files_list**](docs/Files.md#files_list) | **GET** /projects/{project_name}/buckets/{bucket_name}/files | List files
+*Files* | [**files_start_multipart_upload**](docs/Files.md#files_start_multipart_upload) | **POST** /projects/{project_name}/buckets/{bucket_name}/files/{file}/start-multipart-upload | Start multipart upload
 *Files* | [**files_upload**](docs/Files.md#files_upload) | **POST** /projects/{project_name}/buckets/{bucket_name}/files/{file} | Upload a file
 *ImportsAndExports* | [**exports_create**](docs/ImportsAndExports.md#exports_create) | **POST** /projects/{project_name}/exports | Create an export
 *ImportsAndExports* | [**exports_delete**](docs/ImportsAndExports.md#exports_delete) | **DELETE** /projects/{project_name}/exports/{export_id} | Delete an export
 *ImportsAndExports* | [**exports_download**](docs/ImportsAndExports.md#exports_download) | **GET** /projects/{project_name}/exports/{export_id}/download | Download an export
 *ImportsAndExports* | [**exports_get**](docs/ImportsAndExports.md#exports_get) | **GET** /projects/{project_name}/exports/{export_id} | Get an export
 *ImportsAndExports* | [**exports_list**](docs/ImportsAndExports.md#exports_list) | **GET** /projects/{project_name}/exports | List exports
 *ImportsAndExports* | [**imports_create**](docs/ImportsAndExports.md#imports_create) | **POST** /projects/{project_name}/imports | Create an import
@@ -222,14 +224,15 @@
 *Organizations* | [**organization_users_update**](docs/Organizations.md#organization_users_update) | **PATCH** /organizations/{organization_name}/users/{user_id} | Update details of a user in an organization
 *Organizations* | [**organizations_create**](docs/Organizations.md#organizations_create) | **POST** /organizations | Create organizations
 *Organizations* | [**organizations_get**](docs/Organizations.md#organizations_get) | **GET** /organizations/{organization_name} | Get details of an organization
 *Organizations* | [**organizations_list**](docs/Organizations.md#organizations_list) | **GET** /organizations | List organizations
 *Organizations* | [**organizations_resource_usage**](docs/Organizations.md#organizations_resource_usage) | **GET** /organizations/{organization_name}/resources | Get resource usage
 *Organizations* | [**organizations_update**](docs/Organizations.md#organizations_update) | **PATCH** /organizations/{organization_name} | Update details of an organization
 *Organizations* | [**organizations_usage_get**](docs/Organizations.md#organizations_usage_get) | **GET** /organizations/{organization_name}/usage | Get organization usage
+*Organizations* | [**vouchers_get**](docs/Organizations.md#vouchers_get) | **GET** /vouchers/{code} | Get voucher
 *PipelineRequests* | [**batch_pipeline_requests_create**](docs/PipelineRequests.md#batch_pipeline_requests_create) | **POST** /projects/{project_name}/pipelines/{pipeline_name}/requests/batch | Create a batch pipeline request
 *PipelineRequests* | [**batch_pipeline_version_requests_create**](docs/PipelineRequests.md#batch_pipeline_version_requests_create) | **POST** /projects/{project_name}/pipelines/{pipeline_name}/versions/{version}/requests/batch | Create a batch pipeline version request
 *PipelineRequests* | [**pipeline_requests_batch_delete**](docs/PipelineRequests.md#pipeline_requests_batch_delete) | **POST** /projects/{project_name}/pipelines/{pipeline_name}/requests/delete | Delete multiple pipeline requests
 *PipelineRequests* | [**pipeline_requests_batch_get**](docs/PipelineRequests.md#pipeline_requests_batch_get) | **POST** /projects/{project_name}/pipelines/{pipeline_name}/requests/collect | Retrieve multiple pipeline requests
 *PipelineRequests* | [**pipeline_requests_create**](docs/PipelineRequests.md#pipeline_requests_create) | **POST** /projects/{project_name}/pipelines/{pipeline_name}/requests | Create a pipeline request
 *PipelineRequests* | [**pipeline_requests_delete**](docs/PipelineRequests.md#pipeline_requests_delete) | **DELETE** /projects/{project_name}/pipelines/{pipeline_name}/requests/{request_id} | Delete a pipeline request
 *PipelineRequests* | [**pipeline_requests_get**](docs/PipelineRequests.md#pipeline_requests_get) | **GET** /projects/{project_name}/pipelines/{pipeline_name}/requests/{request_id} | Get a pipeline request
@@ -335,14 +338,15 @@
  - [DeploymentRequestSingleDetail](docs/models/DeploymentRequestSingleDetail.md)
  - [DeploymentRequestUpdate](docs/models/DeploymentRequestUpdate.md)
  - [DeploymentRequestUpdateResponse](docs/models/DeploymentRequestUpdateResponse.md)
  - [DeploymentUpdate](docs/models/DeploymentUpdate.md)
  - [DeploymentVersionCreate](docs/models/DeploymentVersionCreate.md)
  - [DeploymentVersionDetail](docs/models/DeploymentVersionDetail.md)
  - [DeploymentVersionList](docs/models/DeploymentVersionList.md)
+ - [DeploymentVersionPort](docs/models/DeploymentVersionPort.md)
  - [DeploymentVersionUpdate](docs/models/DeploymentVersionUpdate.md)
  - [DirectPipelineRequestDeploymentRequest](docs/models/DirectPipelineRequestDeploymentRequest.md)
  - [DirectPipelineRequestOperatorRequest](docs/models/DirectPipelineRequestOperatorRequest.md)
  - [DirectPipelineRequestPipelineRequest](docs/models/DirectPipelineRequestPipelineRequest.md)
  - [EnvironmentBuildDependency](docs/models/EnvironmentBuildDependency.md)
  - [EnvironmentBuildList](docs/models/EnvironmentBuildList.md)
  - [EnvironmentBuildUpdate](docs/models/EnvironmentBuildUpdate.md)
@@ -358,16 +362,18 @@
  - [EnvironmentVariableList](docs/models/EnvironmentVariableList.md)
  - [ExportCreate](docs/models/ExportCreate.md)
  - [ExportDetail](docs/models/ExportDetail.md)
  - [ExportList](docs/models/ExportList.md)
  - [ExpressionEvaluate](docs/models/ExpressionEvaluate.md)
  - [ExpressionEvaluateResponse](docs/models/ExpressionEvaluateResponse.md)
  - [ExpressionInputFieldCreate](docs/models/ExpressionInputFieldCreate.md)
+ - [FileCompleteMultipartUpload](docs/models/FileCompleteMultipartUpload.md)
  - [FileDetail](docs/models/FileDetail.md)
  - [FileItem](docs/models/FileItem.md)
+ - [FileMultipartUpload](docs/models/FileMultipartUpload.md)
  - [FileUploadResponse](docs/models/FileUploadResponse.md)
  - [ImportDetail](docs/models/ImportDetail.md)
  - [ImportList](docs/models/ImportList.md)
  - [ImportUpdate](docs/models/ImportUpdate.md)
  - [InheritedEnvironmentVariableList](docs/models/InheritedEnvironmentVariableList.md)
  - [InputFieldWidgetCreate](docs/models/InputFieldWidgetCreate.md)
  - [InputOutputFieldBase](docs/models/InputOutputFieldBase.md)
@@ -450,14 +456,15 @@
  - [TimeSeriesDataCreate](docs/models/TimeSeriesDataCreate.md)
  - [TimeSeriesDataList](docs/models/TimeSeriesDataList.md)
  - [TimeSeriesDataPointCreate](docs/models/TimeSeriesDataPointCreate.md)
  - [TimeSeriesDataPointList](docs/models/TimeSeriesDataPointList.md)
  - [TimeSeriesSearch](docs/models/TimeSeriesSearch.md)
  - [UserPendingCreate](docs/models/UserPendingCreate.md)
  - [UserPendingDetail](docs/models/UserPendingDetail.md)
+ - [Voucher](docs/models/Voucher.md)
  - [WebhookCreate](docs/models/WebhookCreate.md)
  - [WebhookDetail](docs/models/WebhookDetail.md)
  - [WebhookHeader](docs/models/WebhookHeader.md)
  - [WebhookTestCreate](docs/models/WebhookTestCreate.md)
  - [WebhookTestDetail](docs/models/WebhookTestDetail.md)
  - [WebhookUpdate](docs/models/WebhookUpdate.md)
```

### Comparing `ubiops-4.3.0/setup.py` & `ubiops-4.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ubiops"
-VERSION = "4.3.0"
+VERSION = "4.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ubiops-4.3.0/ubiops/__init__.py` & `ubiops-4.4.0/ubiops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v2.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "4.3.0"
+__version__ = "4.4.0"
 
 # import CoreApi
 from ubiops.api.core_api import CoreApi
 
 # import Training
 from ubiops.training.training import Training
 from ubiops.training.experiment_create import ExperimentCreate
@@ -73,14 +73,15 @@
 from ubiops.models.deployment_request_single_detail import DeploymentRequestSingleDetail
 from ubiops.models.deployment_request_update import DeploymentRequestUpdate
 from ubiops.models.deployment_request_update_response import DeploymentRequestUpdateResponse
 from ubiops.models.deployment_update import DeploymentUpdate
 from ubiops.models.deployment_version_create import DeploymentVersionCreate
 from ubiops.models.deployment_version_detail import DeploymentVersionDetail
 from ubiops.models.deployment_version_list import DeploymentVersionList
+from ubiops.models.deployment_version_port import DeploymentVersionPort
 from ubiops.models.deployment_version_update import DeploymentVersionUpdate
 from ubiops.models.direct_pipeline_request_deployment_request import DirectPipelineRequestDeploymentRequest
 from ubiops.models.direct_pipeline_request_operator_request import DirectPipelineRequestOperatorRequest
 from ubiops.models.direct_pipeline_request_pipeline_request import DirectPipelineRequestPipelineRequest
 from ubiops.models.environment_build_dependency import EnvironmentBuildDependency
 from ubiops.models.environment_build_list import EnvironmentBuildList
 from ubiops.models.environment_build_update import EnvironmentBuildUpdate
@@ -96,16 +97,18 @@
 from ubiops.models.environment_variable_list import EnvironmentVariableList
 from ubiops.models.export_create import ExportCreate
 from ubiops.models.export_detail import ExportDetail
 from ubiops.models.export_list import ExportList
 from ubiops.models.expression_evaluate import ExpressionEvaluate
 from ubiops.models.expression_evaluate_response import ExpressionEvaluateResponse
 from ubiops.models.expression_input_field_create import ExpressionInputFieldCreate
+from ubiops.models.file_complete_multipart_upload import FileCompleteMultipartUpload
 from ubiops.models.file_detail import FileDetail
 from ubiops.models.file_item import FileItem
+from ubiops.models.file_multipart_upload import FileMultipartUpload
 from ubiops.models.file_upload_response import FileUploadResponse
 from ubiops.models.import_detail import ImportDetail
 from ubiops.models.import_list import ImportList
 from ubiops.models.import_update import ImportUpdate
 from ubiops.models.inherited_environment_variable_list import InheritedEnvironmentVariableList
 from ubiops.models.input_field_widget_create import InputFieldWidgetCreate
 from ubiops.models.input_output_field_base import InputOutputFieldBase
@@ -188,14 +191,15 @@
 from ubiops.models.time_series_data_create import TimeSeriesDataCreate
 from ubiops.models.time_series_data_list import TimeSeriesDataList
 from ubiops.models.time_series_data_point_create import TimeSeriesDataPointCreate
 from ubiops.models.time_series_data_point_list import TimeSeriesDataPointList
 from ubiops.models.time_series_search import TimeSeriesSearch
 from ubiops.models.user_pending_create import UserPendingCreate
 from ubiops.models.user_pending_detail import UserPendingDetail
+from ubiops.models.voucher import Voucher
 from ubiops.models.webhook_create import WebhookCreate
 from ubiops.models.webhook_detail import WebhookDetail
 from ubiops.models.webhook_header import WebhookHeader
 from ubiops.models.webhook_test_create import WebhookTestCreate
 from ubiops.models.webhook_test_detail import WebhookTestDetail
 from ubiops.models.webhook_update import WebhookUpdate
```

### Comparing `ubiops-4.3.0/ubiops/api/blobs.py` & `ubiops-4.4.0/ubiops/api/blobs.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/core_api.py` & `ubiops-4.4.0/ubiops/api/core_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2283,14 +2283,46 @@
              If the method is called asynchronously, returns the request thread.
         """
 
         kwargs["_return_http_data_only"] = True
 
         return self.files.buckets_update_with_http_info(project_name, bucket_name, data, **kwargs)
 
+    def files_complete_multipart_upload(self, project_name, bucket_name, file, data, **kwargs):
+        """
+        Complete multipart upload
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
+        async_req=True
+        >>> thread = CoreApi.files_complete_multipart_upload(
+                project_name, bucket_name, file, data, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
+        :param FileCompleteMultipartUpload data: (required)
+        :param kwargs:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(FileMultipartUpload, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        kwargs["_return_http_data_only"] = True
+
+        return self.files.files_complete_multipart_upload_with_http_info(
+            project_name, bucket_name, file, data, **kwargs
+        )
+
     def files_delete(self, project_name, bucket_name, file, **kwargs):
         """
         Delete a file
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
         async_req=True
         >>> thread = CoreApi.files_delete(
@@ -2402,14 +2434,44 @@
              If the method is called asynchronously, returns the request thread.
         """
 
         kwargs["_return_http_data_only"] = True
 
         return self.files.files_list_with_http_info(project_name, bucket_name, **kwargs)
 
+    def files_start_multipart_upload(self, project_name, bucket_name, file, **kwargs):
+        """
+        Start multipart upload
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
+        async_req=True
+        >>> thread = CoreApi.files_start_multipart_upload(
+                project_name, bucket_name, file, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
+        :param kwargs:
+            - object data:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(FileMultipartUpload, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        kwargs["_return_http_data_only"] = True
+
+        return self.files.files_start_multipart_upload_with_http_info(project_name, bucket_name, file, **kwargs)
+
     def files_upload(self, project_name, bucket_name, file, **kwargs):
         """
         Upload a file
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
         async_req=True
         >>> thread = CoreApi.files_upload(
@@ -2417,14 +2479,16 @@
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
         :param str bucket_name: (required)
         :param str file: (required)
         :param kwargs:
+            - str upload_id:
+            - str part_number:
             - object data:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
@@ -3483,14 +3547,41 @@
              If the method is called asynchronously, returns the request thread.
         """
 
         kwargs["_return_http_data_only"] = True
 
         return self.organizations.organizations_usage_get_with_http_info(organization_name, **kwargs)
 
+    def vouchers_get(self, code, **kwargs):
+        """
+        Get voucher
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
+        async_req=True
+        >>> thread = CoreApi.vouchers_get(
+                code, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str code: (required)
+        :param kwargs:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(Voucher, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        kwargs["_return_http_data_only"] = True
+
+        return self.organizations.vouchers_get_with_http_info(code, **kwargs)
+
     def batch_pipeline_requests_create(self, project_name, pipeline_name, data, **kwargs):
         """
         Create a batch pipeline request
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please pass
         async_req=True
         >>> thread = CoreApi.batch_pipeline_requests_create(
```

### Comparing `ubiops-4.3.0/ubiops/api/deployment_requests.py` & `ubiops-4.4.0/ubiops/api/deployment_requests.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/deployments.py` & `ubiops-4.4.0/ubiops/api/deployments.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/environments.py` & `ubiops-4.4.0/ubiops/api/environments.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/files.py` & `ubiops-4.4.0/ubiops/api/imports_and_exports.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,53 +10,53 @@
 """
 
 
 from ubiops.api_client import ApiClient
 from ubiops.exceptions import ApiTypeError, ApiValueError  # noqa: F401
 
 
-class Files(object):
+class ImportsAndExports(object):
     """
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def buckets_create_with_http_info(self, project_name, data, **kwargs):
+    def exports_create_with_http_info(self, project_name, data, **kwargs):
         """
-        Create bucket
+        Create an export
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.buckets_create_with_http_info(
+        >>> thread = ImportsAndExports.exports_create_with_http_info(
                 project_name, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param BucketCreate data: (required)
+        :param ExportCreate data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(BucketList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ExportList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "buckets_create"
+        method_name = "exports_create"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -72,17 +72,17 @@
         if self.api_client.client_side_validation and data is None:
             raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if isinstance(data, dict):
-                from ubiops.models.bucket_create import BucketCreate
+                from ubiops.models.export_create import ExportCreate
 
-                data = BucketCreate(**data)
+                data = ExportCreate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
@@ -94,61 +94,61 @@
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
         header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/buckets"  # noqa: E501
+        url = "/projects/{project_name}/exports"  # noqa: E501
         return self.api_client.call_api(
             url,
             "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="BucketList",
+            response_type="ExportList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def buckets_delete_with_http_info(self, project_name, bucket_name, **kwargs):
+    def exports_delete_with_http_info(self, project_name, export_id, **kwargs):
         """
-        Delete a bucket
+        Delete an export
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.buckets_delete_with_http_info(
-                project_name, bucket_name, async_req=True
+        >>> thread = ImportsAndExports.exports_delete_with_http_info(
+                project_name, export_id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
+        :param str export_id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
         :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "buckets_delete"
+        method_name = "exports_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -157,35 +157,35 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and export_id is None:
+            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+            if not isinstance(export_id, str):
+                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
+        path_params["export_id"] = export_id
 
-        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
+        url = "/projects/{project_name}/exports/{export_id}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -198,40 +198,126 @@
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def buckets_get_with_http_info(self, project_name, bucket_name, **kwargs):
+    def exports_download_with_http_info(self, project_name, export_id, **kwargs):
         """
-        Get details of a bucket
+        Download an export
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.buckets_get_with_http_info(
-                project_name, bucket_name, async_req=True
+        >>> thread = ImportsAndExports.exports_download_with_http_info(
+                project_name, export_id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
+        :param str export_id: (required)
+        :param kwargs:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if True, the file will be downloaded in a folder, which can be defined by
+                api_client.configuration.temp_folder_path. Default is False.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(file, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        method_name = "exports_download"
+        optional_params = []
+        additional_params = [
+            "async_req",
+            "_return_http_data_only",
+            "_preload_content",
+            "_request_timeout",
+            "_request_stream",
+            "_progress_bar",
+        ]
+
+        for key, val in kwargs.items():
+            if key not in optional_params + additional_params:
+                raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
+
+        if self.api_client.client_side_validation and project_name is None:
+            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and export_id is None:
+            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(project_name, str):
+                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(export_id, str):
+                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
+
+        collection_formats = {}
+        path_params = {}
+        query_params = []
+        header_params = {}
+        form_params = []
+        files = {}
+        body_params = None
+
+        path_params["project_name"] = project_name
+        path_params["export_id"] = export_id
+
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        url = "/projects/{project_name}/exports/{export_id}/download"  # noqa: E501
+        return self.api_client.call_api(
+            url,
+            "GET",
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=files,
+            response_type="file",
+            auth_settings=["api_key"],
+            async_req=kwargs.get("async_req", False),
+            _return_http_data_only=kwargs.get("_return_http_data_only", True),
+            _preload_content=kwargs.get("_preload_content", False),
+            _request_timeout=kwargs.get("_request_timeout", None),
+            stream=kwargs.get("_request_stream", True),
+            collection_formats=collection_formats,
+            progress_bar=kwargs.get("_progress_bar", True),
+        )
+
+    def exports_get_with_http_info(self, project_name, export_id, **kwargs):
+        """
+        Get an export
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
+        pass async_req=True.
+
+        >>> thread = ImportsAndExports.exports_get_with_http_info(
+                project_name, export_id, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str project_name: (required)
+        :param str export_id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(BucketDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ExportDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "buckets_get"
+        method_name = "exports_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -240,85 +326,85 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and export_id is None:
+            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+            if not isinstance(export_id, str):
+                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
+        path_params["export_id"] = export_id
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
+        url = "/projects/{project_name}/exports/{export_id}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="BucketDetail",
+            response_type="ExportDetail",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def buckets_list_with_http_info(self, project_name, **kwargs):
+    def exports_list_with_http_info(self, project_name, **kwargs):
         """
-        List buckets
+        List exports
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.buckets_list_with_http_info(
+        >>> thread = ImportsAndExports.exports_list_with_http_info(
                 project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
         :param kwargs:
-            - str labels:
+            - str status:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[BucketList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[ExportList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "buckets_list"
-        optional_params = ["labels"]
+        method_name = "exports_list"
+        optional_params = ["status"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -329,83 +415,85 @@
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "labels" in kwargs and kwargs["labels"] is not None:
-            if not isinstance(kwargs["labels"], str):
-                raise ApiValueError(f"Parameter `labels` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "status" in kwargs and kwargs["status"] is not None:
+            if not isinstance(kwargs["status"], str):
+                raise ApiValueError(f"Parameter `status` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
 
-        if "labels" in kwargs and kwargs["labels"] is not None:
-            query_params.append(("labels", kwargs["labels"]))
+        if "status" in kwargs and kwargs["status"] is not None:
+            query_params.append(("status", kwargs["status"]))
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/buckets"  # noqa: E501
+        url = "/projects/{project_name}/exports"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[BucketList]",
+            response_type="list[ExportList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def buckets_update_with_http_info(self, project_name, bucket_name, data, **kwargs):
+    def imports_create_with_http_info(self, project_name, **kwargs):
         """
-        Update a bucket
+        Create an import
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.buckets_update_with_http_info(
-                project_name, bucket_name, data, async_req=True
+        >>> thread = ImportsAndExports.imports_create_with_http_info(
+                project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
-        :param BucketUpdate data: (required)
         :param kwargs:
+            - file file:
+            - str import_link:
+            - str export_id:
+            - bool skip_confirmation:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(BucketDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ImportList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "buckets_update"
-        optional_params = []
+        method_name = "imports_create"
+        optional_params = ["file", "import_link", "export_id", "skip_confirmation"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -413,97 +501,106 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and data is None:
-            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if isinstance(data, dict):
-                from ubiops.models.bucket_update import BucketUpdate
-
-                data = BucketUpdate(**data)
+        if self.api_client.client_side_validation and "import_link" in kwargs:
+            if not isinstance(kwargs["import_link"], str):
+                raise ApiValueError(f"Parameter `import_link` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "skip_confirmation" in kwargs:
+            if not isinstance(kwargs["skip_confirmation"], bool):
+                raise ApiValueError(f"Parameter `skip_confirmation` must be a boolean when calling `{method_name}`")
+        if (
+            self.api_client.client_side_validation
+            and "import_link" in kwargs
+            and kwargs["import_link"] is not None
+            and len(kwargs["import_link"]) < 1
+        ):
+            raise ApiValueError(
+                f"Invalid value for parameter `import_link` when calling `{method_name}`,"
+                " length must be greater than or equal to `1`"
+            )
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
 
-        body_params = data
+        if "file" in kwargs:
+            files["file"] = kwargs["file"]
+        if "import_link" in kwargs:
+            form_params.append(("import_link", kwargs["import_link"]))
+        if "export_id" in kwargs:
+            form_params.append(("export_id", kwargs["export_id"]))
+        if "skip_confirmation" in kwargs:
+            form_params.append(("skip_confirmation", kwargs["skip_confirmation"]))
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
-        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["multipart/form-data"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
+        url = "/projects/{project_name}/imports"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "PATCH",
+            "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="BucketDetail",
+            response_type="ImportList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
-            progress_bar=kwargs.get("_progress_bar", False),
+            progress_bar=kwargs.get("_progress_bar", True),
         )
 
-    def files_delete_with_http_info(self, project_name, bucket_name, file, **kwargs):
+    def imports_delete_with_http_info(self, project_name, import_id, **kwargs):
         """
-        Delete a file
+        Delete an import
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.files_delete_with_http_info(
-                project_name, bucket_name, file, async_req=True
+        >>> thread = ImportsAndExports.imports_delete_with_http_info(
+                project_name, import_id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
-        :param str file: (required)
+        :param str import_id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
         :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "files_delete"
+        method_name = "imports_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -512,41 +609,35 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and file is None:
-            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
+        if self.api_client.client_side_validation and import_id is None:
+            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(file, str):
-                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+            if not isinstance(import_id, str):
+                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
-        path_params["file"] = file
+        path_params["import_id"] = import_id
 
-        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
+        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -559,41 +650,40 @@
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def files_download_with_http_info(self, project_name, bucket_name, file, **kwargs):
+    def imports_download_with_http_info(self, project_name, import_id, **kwargs):
         """
-        Download a file
+        Download an import
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.files_download_with_http_info(
-                project_name, bucket_name, file, async_req=True
+        >>> thread = ImportsAndExports.imports_download_with_http_info(
+                project_name, import_id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
-        :param str file: (required)
+        :param str import_id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
-            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
-                response data. Default is True.
+            - bool _preload_content: if True, the file will be downloaded in a folder, which can be defined by
+                api_client.configuration.temp_folder_path. Default is False.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(FileUploadResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(file, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "files_download"
+        method_name = "imports_download"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -602,91 +692,84 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and file is None:
-            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
+        if self.api_client.client_side_validation and import_id is None:
+            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(file, str):
-                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+            if not isinstance(import_id, str):
+                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
-        path_params["file"] = file
+        path_params["import_id"] = import_id
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}/download"  # noqa: E501
+        url = "/projects/{project_name}/imports/{import_id}/download"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="FileUploadResponse",
+            response_type="file",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
-            _preload_content=kwargs.get("_preload_content", True),
+            _preload_content=kwargs.get("_preload_content", False),
             _request_timeout=kwargs.get("_request_timeout", None),
-            stream=kwargs.get("_request_stream", False),
+            stream=kwargs.get("_request_stream", True),
             collection_formats=collection_formats,
-            progress_bar=kwargs.get("_progress_bar", False),
+            progress_bar=kwargs.get("_progress_bar", True),
         )
 
-    def files_get_with_http_info(self, project_name, bucket_name, file, **kwargs):
+    def imports_get_with_http_info(self, project_name, import_id, **kwargs):
         """
-        Get a file
+        Get an import
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.files_get_with_http_info(
-                project_name, bucket_name, file, async_req=True
+        >>> thread = ImportsAndExports.imports_get_with_http_info(
+                project_name, import_id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
-        :param str file: (required)
+        :param str import_id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(FileItem, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ImportDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "files_get"
+        method_name = "imports_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -695,95 +778,85 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and file is None:
-            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
+        if self.api_client.client_side_validation and import_id is None:
+            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(file, str):
-                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+            if not isinstance(import_id, str):
+                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
-        path_params["file"] = file
+        path_params["import_id"] = import_id
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
+        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="FileItem",
+            response_type="ImportDetail",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def files_list_with_http_info(self, project_name, bucket_name, **kwargs):
+    def imports_list_with_http_info(self, project_name, **kwargs):
         """
-        List files
+        List imports
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.files_list_with_http_info(
-                project_name, bucket_name, async_req=True
+        >>> thread = ImportsAndExports.imports_list_with_http_info(
+                project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
         :param kwargs:
-            - str prefix:
-            - str delimiter:
-            - str continuation_token:
-            - int limit:
+            - str status:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(FileDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[ImportList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "files_list"
-        optional_params = ["prefix", "delimiter", "continuation_token", "limit"]
+        method_name = "imports_list"
+        optional_params = ["status"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -791,112 +864,86 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "prefix" in kwargs and kwargs["prefix"] is not None:
-            if not isinstance(kwargs["prefix"], str):
-                raise ApiValueError(f"Parameter `prefix` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "delimiter" in kwargs and kwargs["delimiter"] is not None:
-            if not isinstance(kwargs["delimiter"], str):
-                raise ApiValueError(f"Parameter `delimiter` must be a string when calling `{method_name}`")
-        if (
-            self.api_client.client_side_validation
-            and "continuation_token" in kwargs
-            and kwargs["continuation_token"] is not None
-        ):
-            if not isinstance(kwargs["continuation_token"], str):
-                raise ApiValueError(f"Parameter `continuation_token` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "limit" in kwargs and kwargs["limit"] is not None:
-            if not isinstance(kwargs["limit"], int):
-                raise ApiValueError(f"Parameter `limit` must be an integer when calling `{method_name}`")
+        if self.api_client.client_side_validation and "status" in kwargs and kwargs["status"] is not None:
+            if not isinstance(kwargs["status"], str):
+                raise ApiValueError(f"Parameter `status` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
 
-        if "prefix" in kwargs and kwargs["prefix"] is not None:
-            query_params.append(("prefix", kwargs["prefix"]))
-        if "delimiter" in kwargs and kwargs["delimiter"] is not None:
-            query_params.append(("delimiter", kwargs["delimiter"]))
-        if "continuation_token" in kwargs and kwargs["continuation_token"] is not None:
-            query_params.append(("continuation_token", kwargs["continuation_token"]))
-        if "limit" in kwargs and kwargs["limit"] is not None:
-            query_params.append(("limit", kwargs["limit"]))
+        if "status" in kwargs and kwargs["status"] is not None:
+            query_params.append(("status", kwargs["status"]))
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}/files"  # noqa: E501
+        url = "/projects/{project_name}/imports"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="FileDetail",
+            response_type="list[ImportList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def files_upload_with_http_info(self, project_name, bucket_name, file, **kwargs):
+    def imports_update_with_http_info(self, project_name, import_id, data, **kwargs):
         """
-        Upload a file
+        Confirm an import
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Files.files_upload_with_http_info(
-                project_name, bucket_name, file, async_req=True
+        >>> thread = ImportsAndExports.imports_update_with_http_info(
+                project_name, import_id, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str bucket_name: (required)
-        :param str file: (required)
+        :param str import_id: (required)
+        :param ImportUpdate data: (required)
         :param kwargs:
-            - object data:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(FileUploadResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(ImportDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "files_upload"
-        optional_params = ["data"]
+        method_name = "imports_update"
+        optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -904,60 +951,60 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and bucket_name is None:
-            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and file is None:
-            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
+        if self.api_client.client_side_validation and import_id is None:
+            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and data is None:
+            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(bucket_name, str):
-                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+            if not isinstance(import_id, str):
+                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(file, str):
-                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+            if isinstance(data, dict):
+                from ubiops.models.import_update import ImportUpdate
+
+                data = ImportUpdate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["bucket_name"] = bucket_name
-        path_params["file"] = file
+        path_params["import_id"] = import_id
 
-        if "data" in kwargs:
-            body_params = kwargs["data"]
+        body_params = data
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
         header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
+        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "POST",
+            "PATCH",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="FileUploadResponse",
+            response_type="ImportDetail",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
```

### Comparing `ubiops-4.3.0/ubiops/api/imports_and_exports.py` & `ubiops-4.4.0/ubiops/api/roles.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,145 +10,123 @@
 """
 
 
 from ubiops.api_client import ApiClient
 from ubiops.exceptions import ApiTypeError, ApiValueError  # noqa: F401
 
 
-class ImportsAndExports(object):
+class Roles(object):
     """
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def exports_create_with_http_info(self, project_name, data, **kwargs):
+    def permissions_list_with_http_info(self, **kwargs):
         """
-        Create an export
+        List the available permissions
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.exports_create_with_http_info(
-                project_name, data, async_req=True
+        >>> thread = Roles.permissions_list_with_http_info(
+                async_req=True
             )
         >>> result = thread.get()
 
-        :param str project_name: (required)
-        :param ExportCreate data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(ExportList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[PermissionList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "exports_create"
+        method_name = "permissions_list"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
         ]
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
-        if self.api_client.client_side_validation and project_name is None:
-            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and data is None:
-            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(project_name, str):
-                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if isinstance(data, dict):
-                from ubiops.models.export_create import ExportCreate
-
-                data = ExportCreate(**data)
-
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
-        path_params["project_name"] = project_name
-
-        body_params = data
-
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        # HTTP header `Content-Type`
-        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
-
-        url = "/projects/{project_name}/exports"  # noqa: E501
+        url = "/permissions"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "POST",
+            "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="ExportList",
+            response_type="list[PermissionList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def exports_delete_with_http_info(self, project_name, export_id, **kwargs):
+    def role_assignments_create_with_http_info(self, project_name, data, **kwargs):
         """
-        Delete an export
+        Assign role to user/object
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.exports_delete_with_http_info(
-                project_name, export_id, async_req=True
+        >>> thread = Roles.role_assignments_create_with_http_info(
+                project_name, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str export_id: (required)
+        :param RoleAssignmentCreate data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: None
+        :return: tuple(RoleAssignmentList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "exports_delete"
+        method_name = "role_assignments_create"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -157,81 +135,90 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and export_id is None:
-            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and data is None:
+            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(export_id, str):
-                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
+            if isinstance(data, dict):
+                from ubiops.models.role_assignment_create import RoleAssignmentCreate
+
+                data = RoleAssignmentCreate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["export_id"] = export_id
 
-        url = "/projects/{project_name}/exports/{export_id}"  # noqa: E501
+        body_params = data
+
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        # HTTP header `Content-Type`
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
+
+        url = "/projects/{project_name}/role-assignments"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "DELETE",
+            "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type=None,
+            response_type="RoleAssignmentList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def exports_download_with_http_info(self, project_name, export_id, **kwargs):
+    def role_assignments_delete_with_http_info(self, project_name, id, **kwargs):
         """
-        Download an export
+        Delete role of user
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.exports_download_with_http_info(
-                project_name, export_id, async_req=True
+        >>> thread = Roles.role_assignments_delete_with_http_info(
+                project_name, id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str export_id: (required)
+        :param str id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
-            - bool _preload_content: if True, the file will be downloaded in a folder, which can be defined by
-                api_client.configuration.temp_folder_path. Default is False.
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(file, status_code(int), headers(HTTPHeaderDict))
+        :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "exports_download"
+        method_name = "role_assignments_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -240,84 +227,81 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and export_id is None:
-            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and id is None:
+            raise ApiValueError(f"Missing the required parameter `id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(export_id, str):
-                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
+            if not isinstance(id, str):
+                raise ApiValueError(f"Parameter `id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["export_id"] = export_id
+        path_params["id"] = id
 
-        # HTTP header `Accept`
-        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
-
-        url = "/projects/{project_name}/exports/{export_id}/download"  # noqa: E501
+        url = "/projects/{project_name}/role-assignments/{id}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "GET",
+            "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="file",
+            response_type=None,
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
-            _preload_content=kwargs.get("_preload_content", False),
+            _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
-            stream=kwargs.get("_request_stream", True),
+            stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
-            progress_bar=kwargs.get("_progress_bar", True),
+            progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def exports_get_with_http_info(self, project_name, export_id, **kwargs):
+    def role_assignments_get_with_http_info(self, project_name, id, **kwargs):
         """
-        Get an export
+        Get role assignment
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.exports_get_with_http_info(
-                project_name, export_id, async_req=True
+        >>> thread = Roles.role_assignments_get_with_http_info(
+                project_name, id, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str export_id: (required)
+        :param str id: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(ExportDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RoleAssignmentList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "exports_get"
+        method_name = "role_assignments_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -326,85 +310,88 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and export_id is None:
-            raise ApiValueError(f"Missing the required parameter `export_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and id is None:
+            raise ApiValueError(f"Missing the required parameter `id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(export_id, str):
-                raise ApiValueError(f"Parameter `export_id` must be a string when calling `{method_name}`")
+            if not isinstance(id, str):
+                raise ApiValueError(f"Parameter `id` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["export_id"] = export_id
+        path_params["id"] = id
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/exports/{export_id}"  # noqa: E501
+        url = "/projects/{project_name}/role-assignments/{id}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="ExportDetail",
+            response_type="RoleAssignmentList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def exports_list_with_http_info(self, project_name, **kwargs):
+    def role_assignments_per_object_list_with_http_info(self, project_name, **kwargs):
         """
-        List exports
+        List roles on object/user
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.exports_list_with_http_info(
+        >>> thread = Roles.role_assignments_per_object_list_with_http_info(
                 project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
         :param kwargs:
-            - str status:
+            - str resource:
+            - str resource_type:
+            - str assignee:
+            - str assignee_type:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[ExportList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[RoleAssignmentList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "exports_list"
-        optional_params = ["status"]
+        method_name = "role_assignments_per_object_list"
+        optional_params = ["resource", "resource_type", "assignee", "assignee_type"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -415,85 +402,97 @@
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "status" in kwargs and kwargs["status"] is not None:
-            if not isinstance(kwargs["status"], str):
-                raise ApiValueError(f"Parameter `status` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "resource" in kwargs and kwargs["resource"] is not None:
+            if not isinstance(kwargs["resource"], str):
+                raise ApiValueError(f"Parameter `resource` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "resource_type" in kwargs and kwargs["resource_type"] is not None:
+            if not isinstance(kwargs["resource_type"], str):
+                raise ApiValueError(f"Parameter `resource_type` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "assignee" in kwargs and kwargs["assignee"] is not None:
+            if not isinstance(kwargs["assignee"], str):
+                raise ApiValueError(f"Parameter `assignee` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "assignee_type" in kwargs and kwargs["assignee_type"] is not None:
+            if not isinstance(kwargs["assignee_type"], str):
+                raise ApiValueError(f"Parameter `assignee_type` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
 
-        if "status" in kwargs and kwargs["status"] is not None:
-            query_params.append(("status", kwargs["status"]))
+        if "resource" in kwargs and kwargs["resource"] is not None:
+            query_params.append(("resource", kwargs["resource"]))
+        if "resource_type" in kwargs and kwargs["resource_type"] is not None:
+            query_params.append(("resource_type", kwargs["resource_type"]))
+        if "assignee" in kwargs and kwargs["assignee"] is not None:
+            query_params.append(("assignee", kwargs["assignee"]))
+        if "assignee_type" in kwargs and kwargs["assignee_type"] is not None:
+            query_params.append(("assignee_type", kwargs["assignee_type"]))
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/exports"  # noqa: E501
+        url = "/projects/{project_name}/role-assignments"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[ExportList]",
+            response_type="list[RoleAssignmentList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def imports_create_with_http_info(self, project_name, **kwargs):
+    def roles_create_with_http_info(self, project_name, data, **kwargs):
         """
-        Create an import
+        Create a custom role scoped in a project
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.imports_create_with_http_info(
-                project_name, async_req=True
+        >>> thread = Roles.roles_create_with_http_info(
+                project_name, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
+        :param RoleCreate data: (required)
         :param kwargs:
-            - file file:
-            - str import_link:
-            - str export_id:
-            - bool skip_confirmation:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(ImportList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "imports_create"
-        optional_params = ["file", "import_link", "export_id", "skip_confirmation"]
+        method_name = "roles_create"
+        optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -501,106 +500,90 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and data is None:
+            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "import_link" in kwargs:
-            if not isinstance(kwargs["import_link"], str):
-                raise ApiValueError(f"Parameter `import_link` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "skip_confirmation" in kwargs:
-            if not isinstance(kwargs["skip_confirmation"], bool):
-                raise ApiValueError(f"Parameter `skip_confirmation` must be a boolean when calling `{method_name}`")
-        if (
-            self.api_client.client_side_validation
-            and "import_link" in kwargs
-            and kwargs["import_link"] is not None
-            and len(kwargs["import_link"]) < 1
-        ):
-            raise ApiValueError(
-                f"Invalid value for parameter `import_link` when calling `{method_name}`,"
-                " length must be greater than or equal to `1`"
-            )
+        if self.api_client.client_side_validation:
+            if isinstance(data, dict):
+                from ubiops.models.role_create import RoleCreate
+
+                data = RoleCreate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
 
-        if "file" in kwargs:
-            files["file"] = kwargs["file"]
-        if "import_link" in kwargs:
-            form_params.append(("import_link", kwargs["import_link"]))
-        if "export_id" in kwargs:
-            form_params.append(("export_id", kwargs["export_id"]))
-        if "skip_confirmation" in kwargs:
-            form_params.append(("skip_confirmation", kwargs["skip_confirmation"]))
+        body_params = data
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
-        header_params["Content-Type"] = self.api_client.select_header_content_type(["multipart/form-data"])
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/imports"  # noqa: E501
+        url = "/projects/{project_name}/roles"  # noqa: E501
         return self.api_client.call_api(
             url,
             "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="ImportList",
+            response_type="RoleDetailList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
-            progress_bar=kwargs.get("_progress_bar", True),
+            progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def imports_delete_with_http_info(self, project_name, import_id, **kwargs):
+    def roles_delete_with_http_info(self, project_name, role_name, **kwargs):
         """
-        Delete an import
+        Delete a role from a project
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.imports_delete_with_http_info(
-                project_name, import_id, async_req=True
+        >>> thread = Roles.roles_delete_with_http_info(
+                project_name, role_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str import_id: (required)
+        :param str role_name: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
         :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "imports_delete"
+        method_name = "roles_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -609,35 +592,35 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and import_id is None:
-            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and role_name is None:
+            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(import_id, str):
-                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
+            if not isinstance(role_name, str):
+                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["import_id"] = import_id
+        path_params["role_name"] = role_name
 
-        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
+        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -650,126 +633,40 @@
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def imports_download_with_http_info(self, project_name, import_id, **kwargs):
-        """
-        Download an import
-
-        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
-        pass async_req=True.
-
-        >>> thread = ImportsAndExports.imports_download_with_http_info(
-                project_name, import_id, async_req=True
-            )
-        >>> result = thread.get()
-
-        :param str project_name: (required)
-        :param str import_id: (required)
-        :param kwargs:
-            - bool _return_http_data_only: response data without head status code and headers
-            - bool _preload_content: if True, the file will be downloaded in a folder, which can be defined by
-                api_client.configuration.temp_folder_path. Default is False.
-            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
-                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
-            - bool async_req: execute request asynchronously
-        :return: tuple(file, status_code(int), headers(HTTPHeaderDict))
-             If the method is called asynchronously, returns the request thread.
-        """
-
-        method_name = "imports_download"
-        optional_params = []
-        additional_params = [
-            "async_req",
-            "_return_http_data_only",
-            "_preload_content",
-            "_request_timeout",
-            "_request_stream",
-            "_progress_bar",
-        ]
-
-        for key, val in kwargs.items():
-            if key not in optional_params + additional_params:
-                raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
-
-        if self.api_client.client_side_validation and project_name is None:
-            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and import_id is None:
-            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(project_name, str):
-                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(import_id, str):
-                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
-
-        collection_formats = {}
-        path_params = {}
-        query_params = []
-        header_params = {}
-        form_params = []
-        files = {}
-        body_params = None
-
-        path_params["project_name"] = project_name
-        path_params["import_id"] = import_id
-
-        # HTTP header `Accept`
-        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
-
-        url = "/projects/{project_name}/imports/{import_id}/download"  # noqa: E501
-        return self.api_client.call_api(
-            url,
-            "GET",
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=files,
-            response_type="file",
-            auth_settings=["api_key"],
-            async_req=kwargs.get("async_req", False),
-            _return_http_data_only=kwargs.get("_return_http_data_only", True),
-            _preload_content=kwargs.get("_preload_content", False),
-            _request_timeout=kwargs.get("_request_timeout", None),
-            stream=kwargs.get("_request_stream", True),
-            collection_formats=collection_formats,
-            progress_bar=kwargs.get("_progress_bar", True),
-        )
-
-    def imports_get_with_http_info(self, project_name, import_id, **kwargs):
+    def roles_get_with_http_info(self, project_name, role_name, **kwargs):
         """
-        Get an import
+        Get details of a role
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.imports_get_with_http_info(
-                project_name, import_id, async_req=True
+        >>> thread = Roles.roles_get_with_http_info(
+                project_name, role_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str import_id: (required)
+        :param str role_name: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(ImportDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "imports_get"
+        method_name = "roles_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -778,85 +675,84 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and import_id is None:
-            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and role_name is None:
+            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(import_id, str):
-                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
+            if not isinstance(role_name, str):
+                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["import_id"] = import_id
+        path_params["role_name"] = role_name
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
+        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="ImportDetail",
+            response_type="RoleDetailList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def imports_list_with_http_info(self, project_name, **kwargs):
+    def roles_list_with_http_info(self, project_name, **kwargs):
         """
-        List imports
+        List the available roles in a project
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.imports_list_with_http_info(
+        >>> thread = Roles.roles_list_with_http_info(
                 project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
         :param kwargs:
-            - str status:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[ImportList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[RoleList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "imports_list"
-        optional_params = ["status"]
+        method_name = "roles_list"
+        optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -867,82 +763,76 @@
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "status" in kwargs and kwargs["status"] is not None:
-            if not isinstance(kwargs["status"], str):
-                raise ApiValueError(f"Parameter `status` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
 
-        if "status" in kwargs and kwargs["status"] is not None:
-            query_params.append(("status", kwargs["status"]))
-
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/imports"  # noqa: E501
+        url = "/projects/{project_name}/roles"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[ImportList]",
+            response_type="list[RoleList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def imports_update_with_http_info(self, project_name, import_id, data, **kwargs):
+    def roles_update_with_http_info(self, project_name, role_name, data, **kwargs):
         """
-        Confirm an import
+        Update a role in a project
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = ImportsAndExports.imports_update_with_http_info(
-                project_name, import_id, data, async_req=True
+        >>> thread = Roles.roles_update_with_http_info(
+                project_name, role_name, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str import_id: (required)
-        :param ImportUpdate data: (required)
+        :param str role_name: (required)
+        :param RoleUpdate data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(ImportDetail, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "imports_update"
+        method_name = "roles_update"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -951,60 +841,60 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and import_id is None:
-            raise ApiValueError(f"Missing the required parameter `import_id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and role_name is None:
+            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
         if self.api_client.client_side_validation and data is None:
             raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(import_id, str):
-                raise ApiValueError(f"Parameter `import_id` must be a string when calling `{method_name}`")
+            if not isinstance(role_name, str):
+                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if isinstance(data, dict):
-                from ubiops.models.import_update import ImportUpdate
+                from ubiops.models.role_update import RoleUpdate
 
-                data = ImportUpdate(**data)
+                data = RoleUpdate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["import_id"] = import_id
+        path_params["role_name"] = role_name
 
         body_params = data
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
         header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/imports/{import_id}"  # noqa: E501
+        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "PATCH",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="ImportDetail",
+            response_type="RoleDetailList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
```

### Comparing `ubiops-4.3.0/ubiops/api/metrics.py` & `ubiops-4.4.0/ubiops/api/metrics.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/monitoring.py` & `ubiops-4.4.0/ubiops/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/organizations.py` & `ubiops-4.4.0/ubiops/api/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -963,7 +963,86 @@
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
+
+    def vouchers_get_with_http_info(self, code, **kwargs):
+        """
+        Get voucher
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
+        pass async_req=True.
+
+        >>> thread = Organizations.vouchers_get_with_http_info(
+                code, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str code: (required)
+        :param kwargs:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(Voucher, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        method_name = "vouchers_get"
+        optional_params = []
+        additional_params = [
+            "async_req",
+            "_return_http_data_only",
+            "_preload_content",
+            "_request_timeout",
+            "_request_stream",
+            "_progress_bar",
+        ]
+
+        for key, val in kwargs.items():
+            if key not in optional_params + additional_params:
+                raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
+
+        if self.api_client.client_side_validation and code is None:
+            raise ApiValueError(f"Missing the required parameter `code` when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(code, str):
+                raise ApiValueError(f"Parameter `code` must be a string when calling `{method_name}`")
+
+        collection_formats = {}
+        path_params = {}
+        query_params = []
+        header_params = {}
+        form_params = []
+        files = {}
+        body_params = None
+
+        path_params["code"] = code
+
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        url = "/vouchers/{code}"  # noqa: E501
+        return self.api_client.call_api(
+            url,
+            "GET",
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=files,
+            response_type="Voucher",
+            auth_settings=["api_key"],
+            async_req=kwargs.get("async_req", False),
+            _return_http_data_only=kwargs.get("_return_http_data_only", True),
+            _preload_content=kwargs.get("_preload_content", True),
+            _request_timeout=kwargs.get("_request_timeout", None),
+            stream=kwargs.get("_request_stream", False),
+            collection_formats=collection_formats,
+            progress_bar=kwargs.get("_progress_bar", False),
+        )
```

### Comparing `ubiops-4.3.0/ubiops/api/pipeline_requests.py` & `ubiops-4.4.0/ubiops/api/pipeline_requests.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/pipelines.py` & `ubiops-4.4.0/ubiops/api/pipelines.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/projects.py` & `ubiops-4.4.0/ubiops/api/projects.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/request_schedules.py` & `ubiops-4.4.0/ubiops/api/request_schedules.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/roles.py` & `ubiops-4.4.0/ubiops/api/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,123 +10,145 @@
 """
 
 
 from ubiops.api_client import ApiClient
 from ubiops.exceptions import ApiTypeError, ApiValueError  # noqa: F401
 
 
-class Roles(object):
+class Files(object):
     """
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def permissions_list_with_http_info(self, **kwargs):
+    def buckets_create_with_http_info(self, project_name, data, **kwargs):
         """
-        List the available permissions
+        Create bucket
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.permissions_list_with_http_info(
-                async_req=True
+        >>> thread = Files.buckets_create_with_http_info(
+                project_name, data, async_req=True
             )
         >>> result = thread.get()
 
+        :param str project_name: (required)
+        :param BucketCreate data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[PermissionList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(BucketList, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "permissions_list"
+        method_name = "buckets_create"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
         ]
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
+        if self.api_client.client_side_validation and project_name is None:
+            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and data is None:
+            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(project_name, str):
+                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if isinstance(data, dict):
+                from ubiops.models.bucket_create import BucketCreate
+
+                data = BucketCreate(**data)
+
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
+        path_params["project_name"] = project_name
+
+        body_params = data
+
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/permissions"  # noqa: E501
+        # HTTP header `Content-Type`
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
+
+        url = "/projects/{project_name}/buckets"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "GET",
+            "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[PermissionList]",
+            response_type="BucketList",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def role_assignments_create_with_http_info(self, project_name, data, **kwargs):
+    def buckets_delete_with_http_info(self, project_name, bucket_name, **kwargs):
         """
-        Assign role to user/object
+        Delete a bucket
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.role_assignments_create_with_http_info(
-                project_name, data, async_req=True
+        >>> thread = Files.buckets_delete_with_http_info(
+                project_name, bucket_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param RoleAssignmentCreate data: (required)
+        :param str bucket_name: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(RoleAssignmentList, status_code(int), headers(HTTPHeaderDict))
+        :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "role_assignments_create"
+        method_name = "buckets_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -135,90 +157,81 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and data is None:
-            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if isinstance(data, dict):
-                from ubiops.models.role_assignment_create import RoleAssignmentCreate
-
-                data = RoleAssignmentCreate(**data)
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
 
-        body_params = data
-
-        # HTTP header `Accept`
-        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
-
-        # HTTP header `Content-Type`
-        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
-
-        url = "/projects/{project_name}/role-assignments"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "POST",
+            "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="RoleAssignmentList",
+            response_type=None,
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def role_assignments_delete_with_http_info(self, project_name, id, **kwargs):
+    def buckets_get_with_http_info(self, project_name, bucket_name, **kwargs):
         """
-        Delete role of user
+        Get details of a bucket
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.role_assignments_delete_with_http_info(
-                project_name, id, async_req=True
+        >>> thread = Files.buckets_get_with_http_info(
+                project_name, bucket_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str id: (required)
+        :param str bucket_name: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: None
+        :return: tuple(BucketDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "role_assignments_delete"
+        method_name = "buckets_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -227,82 +240,85 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and id is None:
-            raise ApiValueError(f"Missing the required parameter `id` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(id, str):
-                raise ApiValueError(f"Parameter `id` must be a string when calling `{method_name}`")
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["id"] = id
+        path_params["bucket_name"] = bucket_name
+
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/role-assignments/{id}"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "DELETE",
+            "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type=None,
+            response_type="BucketDetail",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def role_assignments_get_with_http_info(self, project_name, id, **kwargs):
+    def buckets_list_with_http_info(self, project_name, **kwargs):
         """
-        Get role assignment
+        List buckets
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.role_assignments_get_with_http_info(
-                project_name, id, async_req=True
+        >>> thread = Files.buckets_list_with_http_info(
+                project_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str id: (required)
         :param kwargs:
+            - str labels:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(RoleAssignmentList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(list[BucketList], status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "role_assignments_get"
-        optional_params = []
+        method_name = "buckets_list"
+        optional_params = ["labels"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -310,88 +326,86 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and id is None:
-            raise ApiValueError(f"Missing the required parameter `id` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation:
-            if not isinstance(id, str):
-                raise ApiValueError(f"Parameter `id` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "labels" in kwargs and kwargs["labels"] is not None:
+            if not isinstance(kwargs["labels"], str):
+                raise ApiValueError(f"Parameter `labels` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["id"] = id
+
+        if "labels" in kwargs and kwargs["labels"] is not None:
+            query_params.append(("labels", kwargs["labels"]))
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/role-assignments/{id}"  # noqa: E501
+        url = "/projects/{project_name}/buckets"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="RoleAssignmentList",
+            response_type="list[BucketList]",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def role_assignments_per_object_list_with_http_info(self, project_name, **kwargs):
+    def buckets_update_with_http_info(self, project_name, bucket_name, data, **kwargs):
         """
-        List roles on object/user
+        Update a bucket
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.role_assignments_per_object_list_with_http_info(
-                project_name, async_req=True
+        >>> thread = Files.buckets_update_with_http_info(
+                project_name, bucket_name, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param BucketUpdate data: (required)
         :param kwargs:
-            - str resource:
-            - str resource_type:
-            - str assignee:
-            - str assignee_type:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[RoleAssignmentList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(BucketDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "role_assignments_per_object_list"
-        optional_params = ["resource", "resource_type", "assignee", "assignee_type"]
+        method_name = "buckets_update"
+        optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -399,99 +413,98 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and data is None:
+            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "resource" in kwargs and kwargs["resource"] is not None:
-            if not isinstance(kwargs["resource"], str):
-                raise ApiValueError(f"Parameter `resource` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "resource_type" in kwargs and kwargs["resource_type"] is not None:
-            if not isinstance(kwargs["resource_type"], str):
-                raise ApiValueError(f"Parameter `resource_type` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "assignee" in kwargs and kwargs["assignee"] is not None:
-            if not isinstance(kwargs["assignee"], str):
-                raise ApiValueError(f"Parameter `assignee` must be a string when calling `{method_name}`")
-        if self.api_client.client_side_validation and "assignee_type" in kwargs and kwargs["assignee_type"] is not None:
-            if not isinstance(kwargs["assignee_type"], str):
-                raise ApiValueError(f"Parameter `assignee_type` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if isinstance(data, dict):
+                from ubiops.models.bucket_update import BucketUpdate
+
+                data = BucketUpdate(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
 
-        if "resource" in kwargs and kwargs["resource"] is not None:
-            query_params.append(("resource", kwargs["resource"]))
-        if "resource_type" in kwargs and kwargs["resource_type"] is not None:
-            query_params.append(("resource_type", kwargs["resource_type"]))
-        if "assignee" in kwargs and kwargs["assignee"] is not None:
-            query_params.append(("assignee", kwargs["assignee"]))
-        if "assignee_type" in kwargs and kwargs["assignee_type"] is not None:
-            query_params.append(("assignee_type", kwargs["assignee_type"]))
+        body_params = data
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/role-assignments"  # noqa: E501
+        # HTTP header `Content-Type`
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
+
+        url = "/projects/{project_name}/buckets/{bucket_name}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "GET",
+            "PATCH",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[RoleAssignmentList]",
+            response_type="BucketDetail",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def roles_create_with_http_info(self, project_name, data, **kwargs):
+    def files_complete_multipart_upload_with_http_info(self, project_name, bucket_name, file, data, **kwargs):
         """
-        Create a custom role scoped in a project
+        Complete multipart upload
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.roles_create_with_http_info(
-                project_name, data, async_req=True
+        >>> thread = Files.files_complete_multipart_upload_with_http_info(
+                project_name, bucket_name, file, data, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param RoleCreate data: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
+        :param FileCompleteMultipartUpload data: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileMultipartUpload, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "roles_create"
+        method_name = "files_complete_multipart_upload"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -500,90 +513,103 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
         if self.api_client.client_side_validation and data is None:
             raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
             if isinstance(data, dict):
-                from ubiops.models.role_create import RoleCreate
+                from ubiops.models.file_complete_multipart_upload import FileCompleteMultipartUpload
 
-                data = RoleCreate(**data)
+                data = FileCompleteMultipartUpload(**data)
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
 
         body_params = data
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
         header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/roles"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}/complete-multipart-upload"  # noqa: E501
         return self.api_client.call_api(
             url,
             "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="RoleDetailList",
+            response_type="FileMultipartUpload",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def roles_delete_with_http_info(self, project_name, role_name, **kwargs):
+    def files_delete_with_http_info(self, project_name, bucket_name, file, **kwargs):
         """
-        Delete a role from a project
+        Delete a file
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.roles_delete_with_http_info(
-                project_name, role_name, async_req=True
+        >>> thread = Files.files_delete_with_http_info(
+                project_name, bucket_name, file, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str role_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
         :return: None
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "roles_delete"
+        method_name = "files_delete"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -592,35 +618,41 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and role_name is None:
-            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(role_name, str):
-                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["role_name"] = role_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
 
-        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "DELETE",
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -633,40 +665,41 @@
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def roles_get_with_http_info(self, project_name, role_name, **kwargs):
+    def files_download_with_http_info(self, project_name, bucket_name, file, **kwargs):
         """
-        Get details of a role
+        Download a file
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.roles_get_with_http_info(
-                project_name, role_name, async_req=True
+        >>> thread = Files.files_download_with_http_info(
+                project_name, bucket_name, file, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str role_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileUploadResponse, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "roles_get"
+        method_name = "files_download"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -675,83 +708,91 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and role_name is None:
-            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(role_name, str):
-                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["role_name"] = role_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}/download"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="RoleDetailList",
+            response_type="FileUploadResponse",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def roles_list_with_http_info(self, project_name, **kwargs):
+    def files_get_with_http_info(self, project_name, bucket_name, file, **kwargs):
         """
-        List the available roles in a project
+        Get a file
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.roles_list_with_http_info(
-                project_name, async_req=True
+        >>> thread = Files.files_get_with_http_info(
+                project_name, bucket_name, file, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
         :param kwargs:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(list[RoleList], status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileItem, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "roles_list"
+        method_name = "files_get"
         optional_params = []
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
@@ -760,80 +801,95 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
-        url = "/projects/{project_name}/roles"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
         return self.api_client.call_api(
             url,
             "GET",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="list[RoleList]",
+            response_type="FileItem",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
             progress_bar=kwargs.get("_progress_bar", False),
         )
 
-    def roles_update_with_http_info(self, project_name, role_name, data, **kwargs):
+    def files_list_with_http_info(self, project_name, bucket_name, **kwargs):
         """
-        Update a role in a project
+        List files
 
         This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
         pass async_req=True.
 
-        >>> thread = Roles.roles_update_with_http_info(
-                project_name, role_name, data, async_req=True
+        >>> thread = Files.files_list_with_http_info(
+                project_name, bucket_name, async_req=True
             )
         >>> result = thread.get()
 
         :param str project_name: (required)
-        :param str role_name: (required)
-        :param RoleUpdate data: (required)
+        :param str bucket_name: (required)
         :param kwargs:
+            - str prefix:
+            - str delimiter:
+            - str continuation_token:
+            - int limit:
             - bool _return_http_data_only: response data without head status code and headers
             - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
                 response data. Default is True.
             - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
                 request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
             - bool async_req: execute request asynchronously
-        :return: tuple(RoleDetailList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(FileDetail, status_code(int), headers(HTTPHeaderDict))
              If the method is called asynchronously, returns the request thread.
         """
 
-        method_name = "roles_update"
-        optional_params = []
+        method_name = "files_list"
+        optional_params = ["prefix", "delimiter", "continuation_token", "limit"]
         additional_params = [
             "async_req",
             "_return_http_data_only",
             "_preload_content",
             "_request_timeout",
             "_request_stream",
             "_progress_bar",
@@ -841,60 +897,286 @@
 
         for key, val in kwargs.items():
             if key not in optional_params + additional_params:
                 raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
 
         if self.api_client.client_side_validation and project_name is None:
             raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and role_name is None:
-            raise ApiValueError(f"Missing the required parameter `role_name` when calling `{method_name}`")
-        if self.api_client.client_side_validation and data is None:
-            raise ApiValueError(f"Missing the required parameter `data` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
         if self.api_client.client_side_validation:
             if not isinstance(project_name, str):
                 raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if not isinstance(role_name, str):
-                raise ApiValueError(f"Parameter `role_name` must be a string when calling `{method_name}`")
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "prefix" in kwargs and kwargs["prefix"] is not None:
+            if not isinstance(kwargs["prefix"], str):
+                raise ApiValueError(f"Parameter `prefix` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "delimiter" in kwargs and kwargs["delimiter"] is not None:
+            if not isinstance(kwargs["delimiter"], str):
+                raise ApiValueError(f"Parameter `delimiter` must be a string when calling `{method_name}`")
+        if (
+            self.api_client.client_side_validation
+            and "continuation_token" in kwargs
+            and kwargs["continuation_token"] is not None
+        ):
+            if not isinstance(kwargs["continuation_token"], str):
+                raise ApiValueError(f"Parameter `continuation_token` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "limit" in kwargs and kwargs["limit"] is not None:
+            if not isinstance(kwargs["limit"], int):
+                raise ApiValueError(f"Parameter `limit` must be an integer when calling `{method_name}`")
+
+        collection_formats = {}
+        path_params = {}
+        query_params = []
+        header_params = {}
+        form_params = []
+        files = {}
+        body_params = None
+
+        path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
+
+        if "prefix" in kwargs and kwargs["prefix"] is not None:
+            query_params.append(("prefix", kwargs["prefix"]))
+        if "delimiter" in kwargs and kwargs["delimiter"] is not None:
+            query_params.append(("delimiter", kwargs["delimiter"]))
+        if "continuation_token" in kwargs and kwargs["continuation_token"] is not None:
+            query_params.append(("continuation_token", kwargs["continuation_token"]))
+        if "limit" in kwargs and kwargs["limit"] is not None:
+            query_params.append(("limit", kwargs["limit"]))
+
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        url = "/projects/{project_name}/buckets/{bucket_name}/files"  # noqa: E501
+        return self.api_client.call_api(
+            url,
+            "GET",
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=files,
+            response_type="FileDetail",
+            auth_settings=["api_key"],
+            async_req=kwargs.get("async_req", False),
+            _return_http_data_only=kwargs.get("_return_http_data_only", True),
+            _preload_content=kwargs.get("_preload_content", True),
+            _request_timeout=kwargs.get("_request_timeout", None),
+            stream=kwargs.get("_request_stream", False),
+            collection_formats=collection_formats,
+            progress_bar=kwargs.get("_progress_bar", False),
+        )
+
+    def files_start_multipart_upload_with_http_info(self, project_name, bucket_name, file, **kwargs):
+        """
+        Start multipart upload
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
+        pass async_req=True.
+
+        >>> thread = Files.files_start_multipart_upload_with_http_info(
+                project_name, bucket_name, file, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
+        :param kwargs:
+            - object data:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(FileMultipartUpload, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        method_name = "files_start_multipart_upload"
+        optional_params = ["data"]
+        additional_params = [
+            "async_req",
+            "_return_http_data_only",
+            "_preload_content",
+            "_request_timeout",
+            "_request_stream",
+            "_progress_bar",
+        ]
+
+        for key, val in kwargs.items():
+            if key not in optional_params + additional_params:
+                raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
+
+        if self.api_client.client_side_validation and project_name is None:
+            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
         if self.api_client.client_side_validation:
-            if isinstance(data, dict):
-                from ubiops.models.role_update import RoleUpdate
+            if not isinstance(project_name, str):
+                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+
+        collection_formats = {}
+        path_params = {}
+        query_params = []
+        header_params = {}
+        form_params = []
+        files = {}
+        body_params = None
+
+        path_params["project_name"] = project_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
+
+        if "data" in kwargs:
+            body_params = kwargs["data"]
 
-                data = RoleUpdate(**data)
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
+
+        # HTTP header `Content-Type`
+        header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
+
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}/start-multipart-upload"  # noqa: E501
+        return self.api_client.call_api(
+            url,
+            "POST",
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=files,
+            response_type="FileMultipartUpload",
+            auth_settings=["api_key"],
+            async_req=kwargs.get("async_req", False),
+            _return_http_data_only=kwargs.get("_return_http_data_only", True),
+            _preload_content=kwargs.get("_preload_content", True),
+            _request_timeout=kwargs.get("_request_timeout", None),
+            stream=kwargs.get("_request_stream", False),
+            collection_formats=collection_formats,
+            progress_bar=kwargs.get("_progress_bar", False),
+        )
+
+    def files_upload_with_http_info(self, project_name, bucket_name, file, **kwargs):
+        """
+        Upload a file
+
+        This method makes a synchronous HTTP request by default. To make an asynchronous HTTP request, please
+        pass async_req=True.
+
+        >>> thread = Files.files_upload_with_http_info(
+                project_name, bucket_name, file, async_req=True
+            )
+        >>> result = thread.get()
+
+        :param str project_name: (required)
+        :param str bucket_name: (required)
+        :param str file: (required)
+        :param kwargs:
+            - str upload_id:
+            - str part_number:
+            - object data:
+            - bool _return_http_data_only: response data without head status code and headers
+            - bool _preload_content: if False, the requests.Response object will be returned without reading/decoding
+                response data. Default is True.
+            - int|tuple _request_timeout: timeout setting for this request. If one number provided, it will be total
+                request timeout. It can also be a pair (tuple) of (connection, read) timeouts.
+            - bool async_req: execute request asynchronously
+        :return: tuple(FileUploadResponse, status_code(int), headers(HTTPHeaderDict))
+             If the method is called asynchronously, returns the request thread.
+        """
+
+        method_name = "files_upload"
+        optional_params = ["upload_id", "part_number", "data"]
+        additional_params = [
+            "async_req",
+            "_return_http_data_only",
+            "_preload_content",
+            "_request_timeout",
+            "_request_stream",
+            "_progress_bar",
+        ]
+
+        for key, val in kwargs.items():
+            if key not in optional_params + additional_params:
+                raise ApiTypeError(f"Got an unexpected keyword argument '{key}' to method `{method_name}`")
+
+        if self.api_client.client_side_validation and project_name is None:
+            raise ApiValueError(f"Missing the required parameter `project_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and bucket_name is None:
+            raise ApiValueError(f"Missing the required parameter `bucket_name` when calling `{method_name}`")
+        if self.api_client.client_side_validation and file is None:
+            raise ApiValueError(f"Missing the required parameter `file` when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(project_name, str):
+                raise ApiValueError(f"Parameter `project_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(bucket_name, str):
+                raise ApiValueError(f"Parameter `bucket_name` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation:
+            if not isinstance(file, str):
+                raise ApiValueError(f"Parameter `file` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "upload_id" in kwargs and kwargs["upload_id"] is not None:
+            if not isinstance(kwargs["upload_id"], str):
+                raise ApiValueError(f"Parameter `upload_id` must be a string when calling `{method_name}`")
+        if self.api_client.client_side_validation and "part_number" in kwargs and kwargs["part_number"] is not None:
+            if not isinstance(kwargs["part_number"], str):
+                raise ApiValueError(f"Parameter `part_number` must be a string when calling `{method_name}`")
 
         collection_formats = {}
         path_params = {}
         query_params = []
         header_params = {}
         form_params = []
         files = {}
         body_params = None
 
         path_params["project_name"] = project_name
-        path_params["role_name"] = role_name
+        path_params["bucket_name"] = bucket_name
+        path_params["file"] = file
 
-        body_params = data
+        if "upload_id" in kwargs and kwargs["upload_id"] is not None:
+            query_params.append(("upload_id", kwargs["upload_id"]))
+        if "part_number" in kwargs and kwargs["part_number"] is not None:
+            query_params.append(("part_number", kwargs["part_number"]))
+
+        if "data" in kwargs:
+            body_params = kwargs["data"]
 
         # HTTP header `Accept`
         header_params["Accept"] = self.api_client.select_header_accept(["application/json"])
 
         # HTTP header `Content-Type`
         header_params["Content-Type"] = self.api_client.select_header_content_type(["application/json"])
 
-        url = "/projects/{project_name}/roles/{role_name}"  # noqa: E501
+        url = "/projects/{project_name}/buckets/{bucket_name}/files/{file}"  # noqa: E501
         return self.api_client.call_api(
             url,
-            "PATCH",
+            "POST",
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=files,
-            response_type="RoleDetailList",
+            response_type="FileUploadResponse",
             auth_settings=["api_key"],
             async_req=kwargs.get("async_req", False),
             _return_http_data_only=kwargs.get("_return_http_data_only", True),
             _preload_content=kwargs.get("_preload_content", True),
             _request_timeout=kwargs.get("_request_timeout", None),
             stream=kwargs.get("_request_stream", False),
             collection_formats=collection_formats,
```

### Comparing `ubiops-4.3.0/ubiops/api/service_users.py` & `ubiops-4.4.0/ubiops/api/service_users.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/status.py` & `ubiops-4.4.0/ubiops/api/status.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/user.py` & `ubiops-4.4.0/ubiops/api/user.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api/webhooks.py` & `ubiops-4.4.0/ubiops/api/webhooks.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/api_client.py` & `ubiops-4.4.0/ubiops/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
 
         self.cookie = cookie
-        self.user_agent = "UbiOps/python/4.3.0"
+        self.user_agent = "UbiOps/python/4.4.0"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ubiops-4.3.0/ubiops/configuration.py` & `ubiops-4.4.0/ubiops/configuration.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/exceptions.py` & `ubiops-4.4.0/ubiops/exceptions.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/__init__.py` & `ubiops-4.4.0/ubiops/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from ubiops.models.deployment_request_single_detail import DeploymentRequestSingleDetail
 from ubiops.models.deployment_request_update import DeploymentRequestUpdate
 from ubiops.models.deployment_request_update_response import DeploymentRequestUpdateResponse
 from ubiops.models.deployment_update import DeploymentUpdate
 from ubiops.models.deployment_version_create import DeploymentVersionCreate
 from ubiops.models.deployment_version_detail import DeploymentVersionDetail
 from ubiops.models.deployment_version_list import DeploymentVersionList
+from ubiops.models.deployment_version_port import DeploymentVersionPort
 from ubiops.models.deployment_version_update import DeploymentVersionUpdate
 from ubiops.models.direct_pipeline_request_deployment_request import DirectPipelineRequestDeploymentRequest
 from ubiops.models.direct_pipeline_request_operator_request import DirectPipelineRequestOperatorRequest
 from ubiops.models.direct_pipeline_request_pipeline_request import DirectPipelineRequestPipelineRequest
 from ubiops.models.environment_build_dependency import EnvironmentBuildDependency
 from ubiops.models.environment_build_list import EnvironmentBuildList
 from ubiops.models.environment_build_update import EnvironmentBuildUpdate
@@ -60,16 +61,18 @@
 from ubiops.models.environment_variable_list import EnvironmentVariableList
 from ubiops.models.export_create import ExportCreate
 from ubiops.models.export_detail import ExportDetail
 from ubiops.models.export_list import ExportList
 from ubiops.models.expression_evaluate import ExpressionEvaluate
 from ubiops.models.expression_evaluate_response import ExpressionEvaluateResponse
 from ubiops.models.expression_input_field_create import ExpressionInputFieldCreate
+from ubiops.models.file_complete_multipart_upload import FileCompleteMultipartUpload
 from ubiops.models.file_detail import FileDetail
 from ubiops.models.file_item import FileItem
+from ubiops.models.file_multipart_upload import FileMultipartUpload
 from ubiops.models.file_upload_response import FileUploadResponse
 from ubiops.models.import_detail import ImportDetail
 from ubiops.models.import_list import ImportList
 from ubiops.models.import_update import ImportUpdate
 from ubiops.models.inherited_environment_variable_list import InheritedEnvironmentVariableList
 from ubiops.models.input_field_widget_create import InputFieldWidgetCreate
 from ubiops.models.input_output_field_base import InputOutputFieldBase
@@ -152,13 +155,14 @@
 from ubiops.models.time_series_data_create import TimeSeriesDataCreate
 from ubiops.models.time_series_data_list import TimeSeriesDataList
 from ubiops.models.time_series_data_point_create import TimeSeriesDataPointCreate
 from ubiops.models.time_series_data_point_list import TimeSeriesDataPointList
 from ubiops.models.time_series_search import TimeSeriesSearch
 from ubiops.models.user_pending_create import UserPendingCreate
 from ubiops.models.user_pending_detail import UserPendingDetail
+from ubiops.models.voucher import Voucher
 from ubiops.models.webhook_create import WebhookCreate
 from ubiops.models.webhook_detail import WebhookDetail
 from ubiops.models.webhook_header import WebhookHeader
 from ubiops.models.webhook_test_create import WebhookTestCreate
 from ubiops.models.webhook_test_detail import WebhookTestDetail
 from ubiops.models.webhook_update import WebhookUpdate
```

### Comparing `ubiops-4.3.0/ubiops/models/attachment_fields_list.py` & `ubiops-4.4.0/ubiops/models/attachment_fields_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/attachment_sources_list.py` & `ubiops-4.4.0/ubiops/models/attachment_sources_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/attachments_create.py` & `ubiops-4.4.0/ubiops/models/attachments_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/attachments_list.py` & `ubiops-4.4.0/ubiops/models/attachments_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/audit_list.py` & `ubiops-4.4.0/ubiops/models/audit_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/blob_list.py` & `ubiops-4.4.0/ubiops/models/blob_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/bucket_create.py` & `ubiops-4.4.0/ubiops/models/bucket_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/bucket_detail.py` & `ubiops-4.4.0/ubiops/models/bucket_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/bucket_list.py` & `ubiops-4.4.0/ubiops/models/bucket_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/bucket_update.py` & `ubiops-4.4.0/ubiops/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/build_list.py` & `ubiops-4.4.0/ubiops/models/build_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_create.py` & `ubiops-4.4.0/ubiops/models/deployment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_create_response.py` & `ubiops-4.4.0/ubiops/models/deployment_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_detail.py` & `ubiops-4.4.0/ubiops/models/deployment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_input_field_create.py` & `ubiops-4.4.0/ubiops/models/deployment_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_instance_type.py` & `ubiops-4.4.0/ubiops/models/deployment_instance_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,39 +33,42 @@
         "display_name": "str",
         "memory_allocation": "int",
         "cpu_allocation": "int",
         "gpu_allocation": "int",
         "storage_allocation": "int",
         "credit_rate": "float",
         "accelerator": "bool",
+        "dedicated_node": "bool",
     }
 
     attribute_map = {
         "id": "id",
         "name": "name",
         "display_name": "display_name",
         "memory_allocation": "memory_allocation",
         "cpu_allocation": "cpu_allocation",
         "gpu_allocation": "gpu_allocation",
         "storage_allocation": "storage_allocation",
         "credit_rate": "credit_rate",
         "accelerator": "accelerator",
+        "dedicated_node": "dedicated_node",
     }
 
     def __init__(
         self,
         id=None,
         name=None,
         display_name=None,
         memory_allocation=None,
         cpu_allocation=None,
         gpu_allocation=None,
         storage_allocation=None,
         credit_rate=None,
         accelerator=None,
+        dedicated_node=None,
         **kwargs,
     ):
         """
         DeploymentInstanceType - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
@@ -77,14 +80,15 @@
         self._display_name = None
         self._memory_allocation = None
         self._cpu_allocation = None
         self._gpu_allocation = None
         self._storage_allocation = None
         self._credit_rate = None
         self._accelerator = None
+        self._dedicated_node = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.name = name
         self.display_name = display_name
         if memory_allocation is not None:
@@ -95,14 +99,16 @@
             self.gpu_allocation = gpu_allocation
         if storage_allocation is not None:
             self.storage_allocation = storage_allocation
         if credit_rate is not None:
             self.credit_rate = credit_rate
         if accelerator is not None:
             self.accelerator = accelerator
+        if dedicated_node is not None:
+            self.dedicated_node = dedicated_node
 
     @property
     def id(self):
         """
         Gets the id of this DeploymentInstanceType
 
         :return: the id of this DeploymentInstanceType
@@ -331,14 +337,39 @@
         """
 
         if self.client_side_validation and (accelerator is not None and not isinstance(accelerator, bool)):
             raise ValueError("Parameter `accelerator` must be a boolean")
 
         self._accelerator = accelerator
 
+    @property
+    def dedicated_node(self):
+        """
+        Gets the dedicated_node of this DeploymentInstanceType
+
+        :return: the dedicated_node of this DeploymentInstanceType
+        :rtype: bool
+        """
+
+        return self._dedicated_node
+
+    @dedicated_node.setter
+    def dedicated_node(self, dedicated_node):
+        """
+        Sets the dedicated_node of this DeploymentInstanceType
+
+        :param dedicated_node: the dedicated_node of this DeploymentInstanceType
+        :type: bool
+        """
+
+        if self.client_side_validation and (dedicated_node is not None and not isinstance(dedicated_node, bool)):
+            raise ValueError("Parameter `dedicated_node` must be a boolean")
+
+        self._dedicated_node = dedicated_node
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/deployment_list.py` & `ubiops-4.4.0/ubiops/models/deployment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_output_field_create.py` & `ubiops-4.4.0/ubiops/models/deployment_output_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_batch_create_response.py` & `ubiops-4.4.0/ubiops/models/deployment_request_batch_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_batch_detail.py` & `ubiops-4.4.0/ubiops/models/deployment_request_batch_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_create_response.py` & `ubiops-4.4.0/ubiops/models/deployment_request_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_list.py` & `ubiops-4.4.0/ubiops/models/deployment_request_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_single_detail.py` & `ubiops-4.4.0/ubiops/models/deployment_request_single_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_update.py` & `ubiops-4.4.0/ubiops/models/deployment_request_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_request_update_response.py` & `ubiops-4.4.0/ubiops/models/deployment_request_update_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_update.py` & `ubiops-4.4.0/ubiops/models/deployment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/deployment_version_create.py` & `ubiops-4.4.0/ubiops/models/deployment_version_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "request_retention_time": "int",
         "request_retention_mode": "str",
         "default_notification_group": "str",
         "maximum_queue_size_express": "int",
         "maximum_queue_size_batch": "int",
         "static_ip": "bool",
         "restart_request_interruption": "bool",
+        "ports": "list[DeploymentVersionPort]",
     }
 
     attribute_map = {
         "version": "version",
         "environment": "environment",
         "instance_type": "instance_type",
         "maximum_instances": "maximum_instances",
@@ -59,14 +60,15 @@
         "request_retention_time": "request_retention_time",
         "request_retention_mode": "request_retention_mode",
         "default_notification_group": "default_notification_group",
         "maximum_queue_size_express": "maximum_queue_size_express",
         "maximum_queue_size_batch": "maximum_queue_size_batch",
         "static_ip": "static_ip",
         "restart_request_interruption": "restart_request_interruption",
+        "ports": "ports",
     }
 
     def __init__(
         self,
         version=None,
         environment="python3-10",
         instance_type=None,
@@ -79,14 +81,15 @@
         request_retention_time=None,
         request_retention_mode="full",
         default_notification_group=None,
         maximum_queue_size_express=None,
         maximum_queue_size_batch=None,
         static_ip=False,
         restart_request_interruption=False,
+        ports=None,
         **kwargs,
     ):
         """
         DeploymentVersionCreate - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
@@ -105,14 +108,15 @@
         self._request_retention_time = None
         self._request_retention_mode = None
         self._default_notification_group = None
         self._maximum_queue_size_express = None
         self._maximum_queue_size_batch = None
         self._static_ip = None
         self._restart_request_interruption = None
+        self._ports = None
         self.discriminator = None
 
         self.version = version
         if environment is not None:
             self.environment = environment
         if instance_type is not None:
             self.instance_type = instance_type
@@ -136,14 +140,16 @@
             self.maximum_queue_size_express = maximum_queue_size_express
         if maximum_queue_size_batch is not None:
             self.maximum_queue_size_batch = maximum_queue_size_batch
         if static_ip is not None:
             self.static_ip = static_ip
         if restart_request_interruption is not None:
             self.restart_request_interruption = restart_request_interruption
+        if ports is not None:
+            self.ports = ports
 
     @property
     def version(self):
         """
         Gets the version of this DeploymentVersionCreate
 
         :return: the version of this DeploymentVersionCreate
@@ -570,14 +576,43 @@
         if self.client_side_validation and (
             restart_request_interruption is not None and not isinstance(restart_request_interruption, bool)
         ):
             raise ValueError("Parameter `restart_request_interruption` must be a boolean")
 
         self._restart_request_interruption = restart_request_interruption
 
+    @property
+    def ports(self):
+        """
+        Gets the ports of this DeploymentVersionCreate
+
+        :return: the ports of this DeploymentVersionCreate
+        :rtype: list[DeploymentVersionPort]
+        """
+
+        return self._ports
+
+    @ports.setter
+    def ports(self, ports):
+        """
+        Sets the ports of this DeploymentVersionCreate
+
+        :param ports: the ports of this DeploymentVersionCreate
+        :type: list[DeploymentVersionPort]
+        """
+
+        if self.client_side_validation and (ports is not None and not isinstance(ports, list)):
+            raise ValueError("Parameter `ports` must be a list")
+        if self.client_side_validation and ports is not None:
+            from ubiops.models.deployment_version_port import DeploymentVersionPort
+
+            ports = [DeploymentVersionPort(**item) if isinstance(item, dict) else item for item in ports]
+
+        self._ports = ports
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/deployment_version_detail.py` & `ubiops-4.4.0/ubiops/models/deployment_version_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         "request_retention_mode": "str",
         "monitoring": "str",
         "default_notification_group": "str",
         "maximum_queue_size_express": "int",
         "maximum_queue_size_batch": "int",
         "static_ip": "bool",
         "restart_request_interruption": "bool",
+        "ports": "list[DeploymentVersionPort]",
         "last_file_upload": "datetime",
         "has_request_method": "bool",
         "has_requests_method": "bool",
     }
 
     attribute_map = {
         "id": "id",
@@ -80,14 +81,15 @@
         "request_retention_mode": "request_retention_mode",
         "monitoring": "monitoring",
         "default_notification_group": "default_notification_group",
         "maximum_queue_size_express": "maximum_queue_size_express",
         "maximum_queue_size_batch": "maximum_queue_size_batch",
         "static_ip": "static_ip",
         "restart_request_interruption": "restart_request_interruption",
+        "ports": "ports",
         "last_file_upload": "last_file_upload",
         "has_request_method": "has_request_method",
         "has_requests_method": "has_requests_method",
     }
 
     def __init__(
         self,
@@ -112,14 +114,15 @@
         request_retention_mode=None,
         monitoring=None,
         default_notification_group=None,
         maximum_queue_size_express=None,
         maximum_queue_size_batch=None,
         static_ip=None,
         restart_request_interruption=None,
+        ports=None,
         last_file_upload=None,
         has_request_method=None,
         has_requests_method=None,
         **kwargs,
     ):
         """
         DeploymentVersionDetail - a model defined in OpenAPI
@@ -150,14 +153,15 @@
         self._request_retention_mode = None
         self._monitoring = None
         self._default_notification_group = None
         self._maximum_queue_size_express = None
         self._maximum_queue_size_batch = None
         self._static_ip = None
         self._restart_request_interruption = None
+        self._ports = None
         self._last_file_upload = None
         self._has_request_method = None
         self._has_requests_method = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
@@ -200,14 +204,16 @@
             self.maximum_queue_size_express = maximum_queue_size_express
         if maximum_queue_size_batch is not None:
             self.maximum_queue_size_batch = maximum_queue_size_batch
         if static_ip is not None:
             self.static_ip = static_ip
         if restart_request_interruption is not None:
             self.restart_request_interruption = restart_request_interruption
+        if ports is not None:
+            self.ports = ports
         self.last_file_upload = last_file_upload
         self.has_request_method = has_request_method
         self.has_requests_method = has_requests_method
 
     @property
     def id(self):
         """
@@ -871,14 +877,43 @@
             restart_request_interruption is not None and not isinstance(restart_request_interruption, bool)
         ):
             raise ValueError("Parameter `restart_request_interruption` must be a boolean")
 
         self._restart_request_interruption = restart_request_interruption
 
     @property
+    def ports(self):
+        """
+        Gets the ports of this DeploymentVersionDetail
+
+        :return: the ports of this DeploymentVersionDetail
+        :rtype: list[DeploymentVersionPort]
+        """
+
+        return self._ports
+
+    @ports.setter
+    def ports(self, ports):
+        """
+        Sets the ports of this DeploymentVersionDetail
+
+        :param ports: the ports of this DeploymentVersionDetail
+        :type: list[DeploymentVersionPort]
+        """
+
+        if self.client_side_validation and (ports is not None and not isinstance(ports, list)):
+            raise ValueError("Parameter `ports` must be a list")
+        if self.client_side_validation and ports is not None:
+            from ubiops.models.deployment_version_port import DeploymentVersionPort
+
+            ports = [DeploymentVersionPort(**item) if isinstance(item, dict) else item for item in ports]
+
+        self._ports = ports
+
+    @property
     def last_file_upload(self):
         """
         Gets the last_file_upload of this DeploymentVersionDetail
 
         :return: the last_file_upload of this DeploymentVersionDetail
         :rtype: datetime
         """
```

### Comparing `ubiops-4.3.0/ubiops/models/deployment_version_list.py` & `ubiops-4.4.0/ubiops/models/deployment_version_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         "request_retention_mode": "str",
         "monitoring": "str",
         "default_notification_group": "str",
         "maximum_queue_size_express": "int",
         "maximum_queue_size_batch": "int",
         "static_ip": "bool",
         "restart_request_interruption": "bool",
+        "ports": "list[DeploymentVersionPort]",
     }
 
     attribute_map = {
         "id": "id",
         "deployment": "deployment",
         "version": "version",
         "default": "default",
@@ -77,14 +78,15 @@
         "request_retention_mode": "request_retention_mode",
         "monitoring": "monitoring",
         "default_notification_group": "default_notification_group",
         "maximum_queue_size_express": "maximum_queue_size_express",
         "maximum_queue_size_batch": "maximum_queue_size_batch",
         "static_ip": "static_ip",
         "restart_request_interruption": "restart_request_interruption",
+        "ports": "ports",
     }
 
     def __init__(
         self,
         id=None,
         deployment=None,
         version=None,
@@ -106,14 +108,15 @@
         request_retention_mode=None,
         monitoring=None,
         default_notification_group=None,
         maximum_queue_size_express=None,
         maximum_queue_size_batch=None,
         static_ip=None,
         restart_request_interruption=None,
+        ports=None,
         **kwargs,
     ):
         """
         DeploymentVersionList - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
@@ -141,14 +144,15 @@
         self._request_retention_mode = None
         self._monitoring = None
         self._default_notification_group = None
         self._maximum_queue_size_express = None
         self._maximum_queue_size_batch = None
         self._static_ip = None
         self._restart_request_interruption = None
+        self._ports = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.deployment = deployment
         self.version = version
         self.default = default
@@ -188,14 +192,16 @@
             self.maximum_queue_size_express = maximum_queue_size_express
         if maximum_queue_size_batch is not None:
             self.maximum_queue_size_batch = maximum_queue_size_batch
         if static_ip is not None:
             self.static_ip = static_ip
         if restart_request_interruption is not None:
             self.restart_request_interruption = restart_request_interruption
+        if ports is not None:
+            self.ports = ports
 
     @property
     def id(self):
         """
         Gets the id of this DeploymentVersionList
 
         :return: the id of this DeploymentVersionList
@@ -855,14 +861,43 @@
         if self.client_side_validation and (
             restart_request_interruption is not None and not isinstance(restart_request_interruption, bool)
         ):
             raise ValueError("Parameter `restart_request_interruption` must be a boolean")
 
         self._restart_request_interruption = restart_request_interruption
 
+    @property
+    def ports(self):
+        """
+        Gets the ports of this DeploymentVersionList
+
+        :return: the ports of this DeploymentVersionList
+        :rtype: list[DeploymentVersionPort]
+        """
+
+        return self._ports
+
+    @ports.setter
+    def ports(self, ports):
+        """
+        Sets the ports of this DeploymentVersionList
+
+        :param ports: the ports of this DeploymentVersionList
+        :type: list[DeploymentVersionPort]
+        """
+
+        if self.client_side_validation and (ports is not None and not isinstance(ports, list)):
+            raise ValueError("Parameter `ports` must be a list")
+        if self.client_side_validation and ports is not None:
+            from ubiops.models.deployment_version_port import DeploymentVersionPort
+
+            ports = [DeploymentVersionPort(**item) if isinstance(item, dict) else item for item in ports]
+
+        self._ports = ports
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/deployment_version_update.py` & `ubiops-4.4.0/ubiops/models/deployment_version_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "request_retention_time": "int",
         "request_retention_mode": "str",
         "default_notification_group": "str",
         "maximum_queue_size_express": "int",
         "maximum_queue_size_batch": "int",
         "static_ip": "bool",
         "restart_request_interruption": "bool",
+        "ports": "list[DeploymentVersionPort]",
     }
 
     attribute_map = {
         "version": "version",
         "environment": "environment",
         "instance_type": "instance_type",
         "maximum_instances": "maximum_instances",
@@ -59,14 +60,15 @@
         "request_retention_time": "request_retention_time",
         "request_retention_mode": "request_retention_mode",
         "default_notification_group": "default_notification_group",
         "maximum_queue_size_express": "maximum_queue_size_express",
         "maximum_queue_size_batch": "maximum_queue_size_batch",
         "static_ip": "static_ip",
         "restart_request_interruption": "restart_request_interruption",
+        "ports": "ports",
     }
 
     def __init__(
         self,
         version=None,
         environment=None,
         instance_type=None,
@@ -79,14 +81,15 @@
         request_retention_time=None,
         request_retention_mode=None,
         default_notification_group=None,
         maximum_queue_size_express=None,
         maximum_queue_size_batch=None,
         static_ip=None,
         restart_request_interruption=None,
+        ports=None,
         **kwargs,
     ):
         """
         DeploymentVersionUpdate - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
@@ -105,14 +108,15 @@
         self._request_retention_time = None
         self._request_retention_mode = None
         self._default_notification_group = None
         self._maximum_queue_size_express = None
         self._maximum_queue_size_batch = None
         self._static_ip = None
         self._restart_request_interruption = None
+        self._ports = None
         self.discriminator = None
 
         if version is not None:
             self.version = version
         if environment is not None:
             self.environment = environment
         if instance_type is not None:
@@ -137,14 +141,16 @@
             self.maximum_queue_size_express = maximum_queue_size_express
         if maximum_queue_size_batch is not None:
             self.maximum_queue_size_batch = maximum_queue_size_batch
         if static_ip is not None:
             self.static_ip = static_ip
         if restart_request_interruption is not None:
             self.restart_request_interruption = restart_request_interruption
+        if ports is not None:
+            self.ports = ports
 
     @property
     def version(self):
         """
         Gets the version of this DeploymentVersionUpdate
 
         :return: the version of this DeploymentVersionUpdate
@@ -569,14 +575,43 @@
         if self.client_side_validation and (
             restart_request_interruption is not None and not isinstance(restart_request_interruption, bool)
         ):
             raise ValueError("Parameter `restart_request_interruption` must be a boolean")
 
         self._restart_request_interruption = restart_request_interruption
 
+    @property
+    def ports(self):
+        """
+        Gets the ports of this DeploymentVersionUpdate
+
+        :return: the ports of this DeploymentVersionUpdate
+        :rtype: list[DeploymentVersionPort]
+        """
+
+        return self._ports
+
+    @ports.setter
+    def ports(self, ports):
+        """
+        Sets the ports of this DeploymentVersionUpdate
+
+        :param ports: the ports of this DeploymentVersionUpdate
+        :type: list[DeploymentVersionPort]
+        """
+
+        if self.client_side_validation and (ports is not None and not isinstance(ports, list)):
+            raise ValueError("Parameter `ports` must be a list")
+        if self.client_side_validation and ports is not None:
+            from ubiops.models.deployment_version_port import DeploymentVersionPort
+
+            ports = [DeploymentVersionPort(**item) if isinstance(item, dict) else item for item in ports]
+
+        self._ports = ports
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/direct_pipeline_request_deployment_request.py` & `ubiops-4.4.0/ubiops/models/direct_pipeline_request_deployment_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/direct_pipeline_request_operator_request.py` & `ubiops-4.4.0/ubiops/models/direct_pipeline_request_operator_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/direct_pipeline_request_pipeline_request.py` & `ubiops-4.4.0/ubiops/models/direct_pipeline_request_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_build_dependency.py` & `ubiops-4.4.0/ubiops/models/environment_build_dependency.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_build_list.py` & `ubiops-4.4.0/ubiops/models/environment_build_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_build_update.py` & `ubiops-4.4.0/ubiops/models/environment_build_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_create.py` & `ubiops-4.4.0/ubiops/models/environment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_detail.py` & `ubiops-4.4.0/ubiops/models/environment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_list.py` & `ubiops-4.4.0/ubiops/models/environment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_revision_create.py` & `ubiops-4.4.0/ubiops/models/environment_revision_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_revision_detail.py` & `ubiops-4.4.0/ubiops/models/environment_revision_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_update.py` & `ubiops-4.4.0/ubiops/models/environment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_usage.py` & `ubiops-4.4.0/ubiops/models/environment_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_variable_copy.py` & `ubiops-4.4.0/ubiops/models/environment_variable_copy.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/environment_variable_create.py` & `ubiops-4.4.0/ubiops/models/environment_variable_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 
         self._name = None
         self._value = None
         self._secret = None
         self.discriminator = None
 
         self.name = name
-        if value is not None:
-            self.value = value
+        self.value = value
         self.secret = secret
 
     @property
     def name(self):
         """
         Gets the name of this EnvironmentVariableCreate
 
@@ -98,14 +97,16 @@
         """
         Sets the value of this EnvironmentVariableCreate
 
         :param value: the value of this EnvironmentVariableCreate
         :type: str
         """
 
+        if self.client_side_validation and value is None:
+            raise ValueError("Invalid value for `value`, must not be `None`")
         if self.client_side_validation and (value is not None and not isinstance(value, str)):
             raise ValueError("Parameter `value` must be a string")
 
         self._value = value
 
     @property
     def secret(self):
```

### Comparing `ubiops-4.3.0/ubiops/models/environment_variable_list.py` & `ubiops-4.4.0/ubiops/models/environment_variable_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/export_create.py` & `ubiops-4.4.0/ubiops/models/export_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/export_detail.py` & `ubiops-4.4.0/ubiops/models/export_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/export_list.py` & `ubiops-4.4.0/ubiops/models/export_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/expression_evaluate.py` & `ubiops-4.4.0/ubiops/models/expression_evaluate.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/expression_evaluate_response.py` & `ubiops-4.4.0/ubiops/models/expression_evaluate_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/expression_input_field_create.py` & `ubiops-4.4.0/ubiops/models/expression_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/file_detail.py` & `ubiops-4.4.0/ubiops/models/file_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/file_item.py` & `ubiops-4.4.0/ubiops/models/file_item.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/file_upload_response.py` & `ubiops-4.4.0/ubiops/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/import_detail.py` & `ubiops-4.4.0/ubiops/models/import_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/import_list.py` & `ubiops-4.4.0/ubiops/models/import_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/import_update.py` & `ubiops-4.4.0/ubiops/models/import_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/inherited_environment_variable_list.py` & `ubiops-4.4.0/ubiops/models/inherited_environment_variable_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/input_field_widget_create.py` & `ubiops-4.4.0/ubiops/models/input_field_widget_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/input_output_field_base.py` & `ubiops-4.4.0/ubiops/models/input_output_field_base.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/input_output_field_detail.py` & `ubiops-4.4.0/ubiops/models/input_output_field_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/input_output_field_list.py` & `ubiops-4.4.0/ubiops/models/input_output_field_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/input_output_widget_list.py` & `ubiops-4.4.0/ubiops/models/input_output_widget_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/logs.py` & `ubiops-4.4.0/ubiops/models/logs.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/logs_create.py` & `ubiops-4.4.0/ubiops/models/logs_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/metric_create.py` & `ubiops-4.4.0/ubiops/models/metric_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/metric_detail.py` & `ubiops-4.4.0/ubiops/models/metric_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/metric_update.py` & `ubiops-4.4.0/ubiops/models/metric_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/notification_group_contact.py` & `ubiops-4.4.0/ubiops/models/notification_group_contact.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/notification_group_create.py` & `ubiops-4.4.0/ubiops/models/notification_group_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/notification_group_list.py` & `ubiops-4.4.0/ubiops/models/notification_group_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/notification_group_update.py` & `ubiops-4.4.0/ubiops/models/notification_group_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/operator_request_detail.py` & `ubiops-4.4.0/ubiops/models/operator_request_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_create.py` & `ubiops-4.4.0/ubiops/models/organization_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,35 +23,44 @@
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name and the value is attribute type
       attribute_map (dict): The key is attribute name and the value is json key in definition
     """
 
-    openapi_types = {"name": "str", "subscription": "str", "subscription_end_date": "date"}
+    openapi_types = {"name": "str", "subscription": "str", "subscription_end_date": "date", "voucher": "str"}
 
-    attribute_map = {"name": "name", "subscription": "subscription", "subscription_end_date": "subscription_end_date"}
+    attribute_map = {
+        "name": "name",
+        "subscription": "subscription",
+        "subscription_end_date": "subscription_end_date",
+        "voucher": "voucher",
+    }
 
-    def __init__(self, name=None, subscription=None, subscription_end_date=None, **kwargs):
+    def __init__(self, name=None, subscription=None, subscription_end_date=None, voucher=None, **kwargs):
         """
         OrganizationCreate - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
         if "local_vars_configuration" in kwargs and kwargs["local_vars_configuration"] is not None:
             self.client_side_validation = kwargs["local_vars_configuration"].client_side_validation
 
         self._name = None
         self._subscription = None
         self._subscription_end_date = None
+        self._voucher = None
         self.discriminator = None
 
         self.name = name
-        self.subscription = subscription
+        if subscription is not None:
+            self.subscription = subscription
         self.subscription_end_date = subscription_end_date
+        if voucher is not None:
+            self.voucher = voucher
 
     @property
     def name(self):
         """
         Gets the name of this OrganizationCreate
 
         :return: the name of this OrganizationCreate
@@ -97,16 +106,14 @@
         """
         Sets the subscription of this OrganizationCreate
 
         :param subscription: the subscription of this OrganizationCreate
         :type: str
         """
 
-        if self.client_side_validation and subscription is None:
-            raise ValueError("Invalid value for `subscription`, must not be `None`")
         if self.client_side_validation and (subscription is not None and not isinstance(subscription, str)):
             raise ValueError("Parameter `subscription` must be a string")
 
         if self.client_side_validation and (subscription is not None and len(subscription) < 1):
             raise ValueError("Invalid value for `subscription`, length must be greater than or equal to `1`")
 
         self._subscription = subscription
@@ -129,14 +136,42 @@
 
         :param subscription_end_date: the subscription_end_date of this OrganizationCreate
         :type: date
         """
 
         self._subscription_end_date = subscription_end_date
 
+    @property
+    def voucher(self):
+        """
+        Gets the voucher of this OrganizationCreate
+
+        :return: the voucher of this OrganizationCreate
+        :rtype: str
+        """
+
+        return self._voucher
+
+    @voucher.setter
+    def voucher(self, voucher):
+        """
+        Sets the voucher of this OrganizationCreate
+
+        :param voucher: the voucher of this OrganizationCreate
+        :type: str
+        """
+
+        if self.client_side_validation and (voucher is not None and not isinstance(voucher, str)):
+            raise ValueError("Parameter `voucher` must be a string")
+
+        if self.client_side_validation and (voucher is not None and len(voucher) < 1):
+            raise ValueError("Invalid value for `voucher`, length must be greater than or equal to `1`")
+
+        self._voucher = voucher
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/organization_detail.py` & `ubiops-4.4.0/ubiops/models/organization_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,47 +23,47 @@
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name and the value is attribute type
       attribute_map (dict): The key is attribute name and the value is json key in definition
     """
 
-    openapi_types = {"id": "str", "name": "str", "creation_date": "datetime", "subscription": "str", "status": "str"}
+    openapi_types = {"id": "str", "name": "str", "creation_date": "datetime", "status": "str", "subscription": "str"}
 
     attribute_map = {
         "id": "id",
         "name": "name",
         "creation_date": "creation_date",
-        "subscription": "subscription",
         "status": "status",
+        "subscription": "subscription",
     }
 
-    def __init__(self, id=None, name=None, creation_date=None, subscription=None, status=None, **kwargs):
+    def __init__(self, id=None, name=None, creation_date=None, status=None, subscription=None, **kwargs):
         """
         OrganizationDetail - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
         if "local_vars_configuration" in kwargs and kwargs["local_vars_configuration"] is not None:
             self.client_side_validation = kwargs["local_vars_configuration"].client_side_validation
 
         self._id = None
         self._name = None
         self._creation_date = None
-        self._subscription = None
         self._status = None
+        self._subscription = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.name = name
         if creation_date is not None:
             self.creation_date = creation_date
-        self.subscription = subscription
         self.status = status
+        self.subscription = subscription
 
     @property
     def id(self):
         """
         Gets the id of this OrganizationDetail
 
         :return: the id of this OrganizationDetail
@@ -137,44 +137,14 @@
         :param creation_date: the creation_date of this OrganizationDetail
         :type: datetime
         """
 
         self._creation_date = creation_date
 
     @property
-    def subscription(self):
-        """
-        Gets the subscription of this OrganizationDetail
-
-        :return: the subscription of this OrganizationDetail
-        :rtype: str
-        """
-
-        return self._subscription
-
-    @subscription.setter
-    def subscription(self, subscription):
-        """
-        Sets the subscription of this OrganizationDetail
-
-        :param subscription: the subscription of this OrganizationDetail
-        :type: str
-        """
-
-        if self.client_side_validation and subscription is None:
-            raise ValueError("Invalid value for `subscription`, must not be `None`")
-        if self.client_side_validation and (subscription is not None and not isinstance(subscription, str)):
-            raise ValueError("Parameter `subscription` must be a string")
-
-        if self.client_side_validation and (subscription is not None and len(subscription) < 1):
-            raise ValueError("Invalid value for `subscription`, length must be greater than or equal to `1`")
-
-        self._subscription = subscription
-
-    @property
     def status(self):
         """
         Gets the status of this OrganizationDetail
 
         :return: the status of this OrganizationDetail
         :rtype: str
         """
@@ -196,14 +166,44 @@
             raise ValueError("Parameter `status` must be a string")
 
         if self.client_side_validation and (status is not None and len(status) < 1):
             raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")
 
         self._status = status
 
+    @property
+    def subscription(self):
+        """
+        Gets the subscription of this OrganizationDetail
+
+        :return: the subscription of this OrganizationDetail
+        :rtype: str
+        """
+
+        return self._subscription
+
+    @subscription.setter
+    def subscription(self, subscription):
+        """
+        Sets the subscription of this OrganizationDetail
+
+        :param subscription: the subscription of this OrganizationDetail
+        :type: str
+        """
+
+        if self.client_side_validation and subscription is None:
+            raise ValueError("Invalid value for `subscription`, must not be `None`")
+        if self.client_side_validation and (subscription is not None and not isinstance(subscription, str)):
+            raise ValueError("Parameter `subscription` must be a string")
+
+        if self.client_side_validation and (subscription is not None and len(subscription) < 1):
+            raise ValueError("Invalid value for `subscription`, length must be greater than or equal to `1`")
+
+        self._subscription = subscription
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/organization_list.py` & `ubiops-4.4.0/ubiops/models/organization_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,37 +23,39 @@
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name and the value is attribute type
       attribute_map (dict): The key is attribute name and the value is json key in definition
     """
 
-    openapi_types = {"id": "str", "name": "str", "creation_date": "datetime"}
+    openapi_types = {"id": "str", "name": "str", "creation_date": "datetime", "status": "str"}
 
-    attribute_map = {"id": "id", "name": "name", "creation_date": "creation_date"}
+    attribute_map = {"id": "id", "name": "name", "creation_date": "creation_date", "status": "status"}
 
-    def __init__(self, id=None, name=None, creation_date=None, **kwargs):
+    def __init__(self, id=None, name=None, creation_date=None, status=None, **kwargs):
         """
         OrganizationList - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
         if "local_vars_configuration" in kwargs and kwargs["local_vars_configuration"] is not None:
             self.client_side_validation = kwargs["local_vars_configuration"].client_side_validation
 
         self._id = None
         self._name = None
         self._creation_date = None
+        self._status = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
         self.name = name
         if creation_date is not None:
             self.creation_date = creation_date
+        self.status = status
 
     @property
     def id(self):
         """
         Gets the id of this OrganizationList
 
         :return: the id of this OrganizationList
@@ -126,14 +128,44 @@
 
         :param creation_date: the creation_date of this OrganizationList
         :type: datetime
         """
 
         self._creation_date = creation_date
 
+    @property
+    def status(self):
+        """
+        Gets the status of this OrganizationList
+
+        :return: the status of this OrganizationList
+        :rtype: str
+        """
+
+        return self._status
+
+    @status.setter
+    def status(self, status):
+        """
+        Sets the status of this OrganizationList
+
+        :param status: the status of this OrganizationList
+        :type: str
+        """
+
+        if self.client_side_validation and status is None:
+            raise ValueError("Invalid value for `status`, must not be `None`")
+        if self.client_side_validation and (status is not None and not isinstance(status, str)):
+            raise ValueError("Parameter `status` must be a string")
+
+        if self.client_side_validation and (status is not None and len(status) < 1):
+            raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")
+
+        self._status = status
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/organization_project_usage.py` & `ubiops-4.4.0/ubiops/models/organization_project_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_update.py` & `ubiops-4.4.0/ubiops/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_usage.py` & `ubiops-4.4.0/ubiops/models/organization_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_user_create.py` & `ubiops-4.4.0/ubiops/models/organization_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_user_detail.py` & `ubiops-4.4.0/ubiops/models/organization_user_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/organization_user_update.py` & `ubiops-4.4.0/ubiops/models/organization_user_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/output_field_widget_create.py` & `ubiops-4.4.0/ubiops/models/output_field_widget_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/output_value_list.py` & `ubiops-4.4.0/ubiops/models/output_value_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/permission_list.py` & `ubiops-4.4.0/ubiops/models/permission_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_create.py` & `ubiops-4.4.0/ubiops/models/pipeline_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_create_response.py` & `ubiops-4.4.0/ubiops/models/pipeline_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_detail.py` & `ubiops-4.4.0/ubiops/models/pipeline_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_input_field_create.py` & `ubiops-4.4.0/ubiops/models/pipeline_input_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_list.py` & `ubiops-4.4.0/ubiops/models/pipeline_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_output_field_create.py` & `ubiops-4.4.0/ubiops/models/pipeline_output_field_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_batch_create_response.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_batch_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_create_response.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_create_response.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_deployment_request.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_deployment_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_detail.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_list.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_operator_request.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_operator_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_pipeline_request.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_request_single_detail.py` & `ubiops-4.4.0/ubiops/models/pipeline_request_single_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_update.py` & `ubiops-4.4.0/ubiops/models/pipeline_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_create.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_detail.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_list.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_object_configuration_list.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_object_configuration_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_object_create.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_object_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_object_list.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_object_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/pipeline_version_update.py` & `ubiops-4.4.0/ubiops/models/pipeline_version_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_create.py` & `ubiops-4.4.0/ubiops/models/project_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_deployment_version_usage.py` & `ubiops-4.4.0/ubiops/models/project_deployment_version_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_detail.py` & `ubiops-4.4.0/ubiops/models/project_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_list.py` & `ubiops-4.4.0/ubiops/models/project_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_resource_usage.py` & `ubiops-4.4.0/ubiops/models/project_resource_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_update.py` & `ubiops-4.4.0/ubiops/models/project_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_usage.py` & `ubiops-4.4.0/ubiops/models/project_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_user_create.py` & `ubiops-4.4.0/ubiops/models/project_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/project_user_list.py` & `ubiops-4.4.0/ubiops/models/project_user_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/quota_detail.py` & `ubiops-4.4.0/ubiops/models/quota_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/requests_overview.py` & `ubiops-4.4.0/ubiops/models/requests_overview.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/resource_usage.py` & `ubiops-4.4.0/ubiops/models/resource_usage.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/revision_create.py` & `ubiops-4.4.0/ubiops/models/revision_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/revision_list.py` & `ubiops-4.4.0/ubiops/models/revision_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_assignment_create.py` & `ubiops-4.4.0/ubiops/models/role_assignment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_assignment_list.py` & `ubiops-4.4.0/ubiops/models/role_assignment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_create.py` & `ubiops-4.4.0/ubiops/models/role_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_detail_list.py` & `ubiops-4.4.0/ubiops/models/role_detail_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_list.py` & `ubiops-4.4.0/ubiops/models/role_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/role_update.py` & `ubiops-4.4.0/ubiops/models/role_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/schedule_create.py` & `ubiops-4.4.0/ubiops/models/schedule_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/schedule_list.py` & `ubiops-4.4.0/ubiops/models/schedule_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/schedule_update.py` & `ubiops-4.4.0/ubiops/models/schedule_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/service_user_create.py` & `ubiops-4.4.0/ubiops/models/service_user_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/service_user_list.py` & `ubiops-4.4.0/ubiops/models/service_user_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/service_user_token_detail.py` & `ubiops-4.4.0/ubiops/models/service_user_token_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/service_user_token_list.py` & `ubiops-4.4.0/ubiops/models/service_user_token_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/status.py` & `ubiops-4.4.0/ubiops/models/status.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/template_deployment_list.py` & `ubiops-4.4.0/ubiops/models/template_deployment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/time_series_data_create.py` & `ubiops-4.4.0/ubiops/models/time_series_data_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/time_series_data_list.py` & `ubiops-4.4.0/ubiops/models/time_series_data_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/time_series_data_point_create.py` & `ubiops-4.4.0/ubiops/models/time_series_data_point_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/time_series_data_point_list.py` & `ubiops-4.4.0/ubiops/models/time_series_data_point_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/time_series_search.py` & `ubiops-4.4.0/ubiops/models/time_series_search.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/user_pending_create.py` & `ubiops-4.4.0/ubiops/models/user_pending_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,37 +23,39 @@
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name and the value is attribute type
       attribute_map (dict): The key is attribute name and the value is json key in definition
     """
 
-    openapi_types = {"email": "str", "password": "str", "name": "str", "surname": "str"}
+    openapi_types = {"email": "str", "password": "str", "name": "str", "surname": "str", "phone": "str"}
 
-    attribute_map = {"email": "email", "password": "password", "name": "name", "surname": "surname"}
+    attribute_map = {"email": "email", "password": "password", "name": "name", "surname": "surname", "phone": "phone"}
 
-    def __init__(self, email=None, password=None, name=None, surname=None, **kwargs):
+    def __init__(self, email=None, password=None, name=None, surname=None, phone=None, **kwargs):
         """
         UserPendingCreate - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
         if "local_vars_configuration" in kwargs and kwargs["local_vars_configuration"] is not None:
             self.client_side_validation = kwargs["local_vars_configuration"].client_side_validation
 
         self._email = None
         self._password = None
         self._name = None
         self._surname = None
+        self._phone = None
         self.discriminator = None
 
         self.email = email
         self.password = password
         self.name = name
         self.surname = surname
+        self.phone = phone
 
     @property
     def email(self):
         """
         Gets the email of this UserPendingCreate
 
         :return: the email of this UserPendingCreate
@@ -167,14 +169,42 @@
             raise ValueError("Parameter `surname` must be a string")
 
         if self.client_side_validation and (surname is not None and len(surname) > 256):
             raise ValueError("Invalid value for `surname`, length must be less than or equal to `256`")
 
         self._surname = surname
 
+    @property
+    def phone(self):
+        """
+        Gets the phone of this UserPendingCreate
+
+        :return: the phone of this UserPendingCreate
+        :rtype: str
+        """
+
+        return self._phone
+
+    @phone.setter
+    def phone(self, phone):
+        """
+        Sets the phone of this UserPendingCreate
+
+        :param phone: the phone of this UserPendingCreate
+        :type: str
+        """
+
+        if self.client_side_validation and (phone is not None and not isinstance(phone, str)):
+            raise ValueError("Parameter `phone` must be a string")
+
+        if self.client_side_validation and (phone is not None and len(phone) > 17):
+            raise ValueError("Invalid value for `phone`, length must be less than or equal to `17`")
+
+        self._phone = phone
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/user_pending_detail.py` & `ubiops-4.4.0/ubiops/models/user_pending_detail.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,35 +23,37 @@
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name and the value is attribute type
       attribute_map (dict): The key is attribute name and the value is json key in definition
     """
 
-    openapi_types = {"email": "str", "name": "str", "surname": "str"}
+    openapi_types = {"email": "str", "name": "str", "surname": "str", "phone": "str"}
 
-    attribute_map = {"email": "email", "name": "name", "surname": "surname"}
+    attribute_map = {"email": "email", "name": "name", "surname": "surname", "phone": "phone"}
 
-    def __init__(self, email=None, name=None, surname=None, **kwargs):
+    def __init__(self, email=None, name=None, surname=None, phone=None, **kwargs):
         """
         UserPendingDetail - a model defined in OpenAPI
         """
 
         self.client_side_validation = True
         if "local_vars_configuration" in kwargs and kwargs["local_vars_configuration"] is not None:
             self.client_side_validation = kwargs["local_vars_configuration"].client_side_validation
 
         self._email = None
         self._name = None
         self._surname = None
+        self._phone = None
         self.discriminator = None
 
         self.email = email
         self.name = name
         self.surname = surname
+        self.phone = phone
 
     @property
     def email(self):
         """
         Gets the email of this UserPendingDetail
 
         :return: the email of this UserPendingDetail
@@ -133,14 +135,42 @@
             raise ValueError("Parameter `surname` must be a string")
 
         if self.client_side_validation and (surname is not None and len(surname) > 256):
             raise ValueError("Invalid value for `surname`, length must be less than or equal to `256`")
 
         self._surname = surname
 
+    @property
+    def phone(self):
+        """
+        Gets the phone of this UserPendingDetail
+
+        :return: the phone of this UserPendingDetail
+        :rtype: str
+        """
+
+        return self._phone
+
+    @phone.setter
+    def phone(self, phone):
+        """
+        Sets the phone of this UserPendingDetail
+
+        :param phone: the phone of this UserPendingDetail
+        :type: str
+        """
+
+        if self.client_side_validation and (phone is not None and not isinstance(phone, str)):
+            raise ValueError("Parameter `phone` must be a string")
+
+        if self.client_side_validation and (phone is not None and len(phone) > 17):
+            raise ValueError("Invalid value for `phone`, length must be less than or equal to `17`")
+
+        self._phone = phone
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
 
         result = {}
```

### Comparing `ubiops-4.3.0/ubiops/models/webhook_create.py` & `ubiops-4.4.0/ubiops/models/webhook_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/webhook_detail.py` & `ubiops-4.4.0/ubiops/models/webhook_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/webhook_header.py` & `ubiops-4.4.0/ubiops/models/webhook_header.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/webhook_test_create.py` & `ubiops-4.4.0/ubiops/models/webhook_test_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/webhook_test_detail.py` & `ubiops-4.4.0/ubiops/models/webhook_test_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/models/webhook_update.py` & `ubiops-4.4.0/ubiops/models/webhook_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/rest.py` & `ubiops-4.4.0/ubiops/rest.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/__init__.py` & `ubiops-4.4.0/ubiops/training/__init__.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_create.py` & `ubiops-4.4.0/ubiops/training/experiment_create.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_detail.py` & `ubiops-4.4.0/ubiops/training/experiment_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_list.py` & `ubiops-4.4.0/ubiops/training/experiment_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_run_create.py` & `ubiops-4.4.0/ubiops/training/experiment_run_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             if isinstance(value, list):
                 result[attr] = list(map(lambda x: x.to_dict() if hasattr(x, "to_dict") else x, value))
             elif hasattr(value, "to_dict"):
                 result[attr] = value.to_dict()
             elif isinstance(value, dict):
                 result[attr] = dict(
                     map(
-                        lambda item: (item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item,
+                        lambda item: ((item[0], item[1].to_dict()) if hasattr(item[1], "to_dict") else item),
                         value.items(),
                     )
                 )
             else:
                 result[attr] = value
 
         return result
```

### Comparing `ubiops-4.3.0/ubiops/training/experiment_run_create_response.py` & `ubiops-4.4.0/ubiops/training/experiment_run_create_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,32 @@
     UbiOps
 
     Client Library to interact with the UbiOps API
 """
 
 
 from ubiops.training.constants import DEFAULT_TRAINING_DEPLOYMENT_NAME
-from ubiops.models.deployment_request_batch_create_response import DeploymentRequestBatchCreateResponse
+from ubiops.models.deployment_request_batch_create_response import (
+    DeploymentRequestBatchCreateResponse,
+)
 
 
 class ExperimentRunCreateResponse(DeploymentRequestBatchCreateResponse):
-    openapi_types = {"id": "str", "experiment": "str", "status": "str", "time_created": "datetime"}
-    attribute_map = {"id": "id", "experiment": "experiment", "status": "status", "time_created": "time_created"}
+    openapi_types = {
+        "id": "str",
+        "experiment": "str",
+        "status": "str",
+        "time_created": "datetime",
+    }
+    attribute_map = {
+        "id": "id",
+        "experiment": "experiment",
+        "status": "status",
+        "time_created": "time_created",
+    }
 
     def __init__(self, id=None, experiment=None, status=None, time_created=None, **kwargs):
         """
         ExperimentRunCreateResponse
         """
 
         kwargs.pop("version", None)  # To make sure we don't pass the version twice
```

### Comparing `ubiops-4.3.0/ubiops/training/experiment_run_detail.py` & `ubiops-4.4.0/ubiops/training/experiment_run_detail.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_run_list.py` & `ubiops-4.4.0/ubiops/training/experiment_run_list.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/experiment_run_update_response.py` & `ubiops-4.4.0/ubiops/training/experiment_run_update_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 """
     UbiOps
 
     Client Library to interact with the UbiOps API.
 """
 
 from ubiops.training.constants import DEFAULT_TRAINING_DEPLOYMENT_NAME
-from ubiops.models.deployment_request_update_response import DeploymentRequestUpdateResponse
+from ubiops.models.deployment_request_update_response import (
+    DeploymentRequestUpdateResponse,
+)
 
 
 class ExperimentRunUpdateResponse(DeploymentRequestUpdateResponse):
     openapi_types = {
         "id": "str",
         "experiment": "str",
         "status": "str",
```

### Comparing `ubiops-4.3.0/ubiops/training/experiment_update.py` & `ubiops-4.4.0/ubiops/training/experiment_update.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/training/training.py` & `ubiops-4.4.0/ubiops/training/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,17 @@
 
         # Get the environment. If not existing it will throw an exception.
         try:
             self.core_api.environments_get(project_name=project_name, environment_name=environment_name)
         except ApiException as e:
             if e.status == 404:
                 raise ApiException(
-                    status=e.status, reason="Not Found", body=f"Environment {environment_name} not found"
+                    status=e.status,
+                    reason="Not Found",
+                    body=f"Environment {environment_name} not found",
                 )
             else:
                 raise
 
     def _verify_bucket_exists(self, project_name, bucket):
         """
         Check if the bucket exists
@@ -119,15 +121,19 @@
         """
 
         # Get the bucket for training artifacts. If not existing it will throw an exception.
         try:
             self.core_api.buckets_get(project_name=project_name, bucket_name=bucket)
         except ApiException as e:
             if e.status == 404:
-                raise ApiException(status=e.status, reason="Not Found", body=f"Bucket {bucket} not found")
+                raise ApiException(
+                    status=e.status,
+                    reason="Not Found",
+                    body=f"Bucket {bucket} not found",
+                )
             else:
                 raise
 
     def _get_template_deployment(self):
         """
         Get the training template deployment
 
@@ -142,34 +148,40 @@
             for template_deployment in template_deployments:
                 if template_deployment.details["name"] == TEMPLATE_DEPLOYMENT_NAME:
                     training_template_deployment_id = template_deployment.id
                     training_template_deployment = template_deployment.details
 
             if training_template_deployment is None:
                 raise ApiException(
-                    status=500, reason="Internal Error", body="Could not obtain a template training deployment"
+                    status=500,
+                    reason="Internal Error",
+                    body="Could not obtain a template training deployment",
                 )
 
             return training_template_deployment_id, training_template_deployment
         except (AttributeError, KeyError):
             raise ApiException(
-                status=500, reason="Internal Error", body="Could not obtain a template training deployment"
+                status=500,
+                reason="Internal Error",
+                body="Could not obtain a template training deployment",
             )
 
     def _get_default_bucket(self, project_name, experiment_name):
         """
         Get the default bucket for the experiment
 
         :param str project_name: the name of the project
         :param str experiment_name: the name of the experiment
         """
 
         try:
             env_vars = self.core_api.deployment_version_environment_variables_list(
-                project_name=project_name, deployment_name=self.training_deployment_name, version=experiment_name
+                project_name=project_name,
+                deployment_name=self.training_deployment_name,
+                version=experiment_name,
             )
             for env_var in env_vars:
                 if env_var.name == DEFAULT_TRAINING_BUCKET_NAME:
                     return env_var.value
 
         except ApiException as e:
             raise self.wrap_exception(e)
@@ -183,25 +195,29 @@
         :param str project_name: the name of the project
         :param str experiment_name: the name of the experiment
         :param str bucket_name: the new bucket to use for the training experiment
         """
 
         try:
             env_vars = self.core_api.deployment_version_environment_variables_list(
-                project_name=project_name, deployment_name=self.training_deployment_name, version=experiment_name
+                project_name=project_name,
+                deployment_name=self.training_deployment_name,
+                version=experiment_name,
             )
             for env_var in env_vars:
                 if env_var.name == DEFAULT_TRAINING_BUCKET_NAME:
                     self.core_api.deployment_version_environment_variables_update(
                         project_name=project_name,
                         deployment_name=self.training_deployment_name,
                         version=experiment_name,
                         id=env_var.id,
                         data=ubiops.EnvironmentVariableCreate(
-                            name=DEFAULT_TRAINING_BUCKET_NAME, value=bucket_name, secret=False
+                            name=DEFAULT_TRAINING_BUCKET_NAME,
+                            value=bucket_name,
+                            secret=False,
                         ),
                     )
                     return
 
             # Environment variable DEFAULT_TRAINING_BUCKET_NAME does not exist yet
             self.core_api.deployment_version_environment_variables_create(
                 project_name=project_name,
@@ -285,15 +301,17 @@
         if data.default_bucket:
             try:
                 self.core_api.deployment_version_environment_variables_create(
                     project_name=project_name,
                     deployment_name=self.training_deployment_name,
                     version=data.name,
                     data=ubiops.EnvironmentVariableCreate(
-                        name=DEFAULT_TRAINING_BUCKET_NAME, value=data.default_bucket, secret=False
+                        name=DEFAULT_TRAINING_BUCKET_NAME,
+                        value=data.default_bucket,
+                        secret=False,
                     ),
                     **kwargs,
                 )
             except ApiException as e:
                 raise self.wrap_exception(e)
 
         # Upload a default training zip file package
@@ -314,15 +332,18 @@
             experiment_name=data.name,
             revision_id=response.revision,
             quiet=False,
         )
 
         try:
             deployment_version = self.core_api.deployment_versions_get(
-                project_name=project_name, deployment_name=self.training_deployment_name, version=data.name, **kwargs
+                project_name=project_name,
+                deployment_name=self.training_deployment_name,
+                version=data.name,
+                **kwargs,
             )
         except ApiException as e:
             raise self.wrap_exception(e)
 
         from ubiops.training.experiment_list import ExperimentList
 
         return ExperimentList(name=deployment_version.version, **deployment_version.to_dict())
@@ -387,15 +408,17 @@
 
         # Get the default bucket
         default_bucket = self._get_default_bucket(project_name=project_name, experiment_name=experiment_name)
 
         from ubiops.training.experiment_detail import ExperimentDetail
 
         return ExperimentDetail(
-            name=deployment_version.version, default_bucket=default_bucket, **deployment_version.to_dict()
+            name=deployment_version.version,
+            default_bucket=default_bucket,
+            **deployment_version.to_dict(),
         )
 
     def experiments_list(self, project_name, **kwargs):
         """
         List experiments
 
         :param str project_name: the name of the project (required)
@@ -408,15 +431,17 @@
         if project_name is not None and not isinstance(project_name, str):
             raise ApiValueError("Parameter `project_name` must be a string")
 
         self._verify_deployment_exists(project_name=project_name)
 
         try:
             deployment_versions = self.core_api.deployment_versions_list(
-                project_name=project_name, deployment_name=self.training_deployment_name, **kwargs
+                project_name=project_name,
+                deployment_name=self.training_deployment_name,
+                **kwargs,
             )
         except ApiException as e:
             raise self.wrap_exception(e)
 
         from ubiops.training.experiment_list import ExperimentList
 
         return [ExperimentList(name=version.version, **version.to_dict()) for version in deployment_versions]
@@ -452,15 +477,17 @@
                 raise ApiValueError("Parameter `data` must be an instance of ExperimentUpdate")
 
         if data.environment:
             self._verify_environment_exists(project_name=project_name, environment_name=data.environment)
         if data.default_bucket:
             self._verify_bucket_exists(project_name=project_name, bucket=data.default_bucket)
             self._update_default_bucket(
-                project_name=project_name, experiment_name=experiment_name, bucket_name=data.default_bucket
+                project_name=project_name,
+                experiment_name=experiment_name,
+                bucket_name=data.default_bucket,
             )
 
         version_template = ubiops.DeploymentVersionUpdate(version=data.name, **data.to_dict())
 
         try:
             deployment_version = self.core_api.deployment_versions_update(
                 project_name=project_name,
@@ -471,24 +498,28 @@
             )
         except ApiException as e:
             raise self.wrap_exception(e)
 
         from ubiops.training.experiment_detail import ExperimentDetail
 
         return ExperimentDetail(
-            name=deployment_version.version, default_bucket=data.default_bucket, **deployment_version.to_dict()
+            name=deployment_version.version,
+            default_bucket=data.default_bucket,
+            **deployment_version.to_dict(),
         )
 
     def experiment_runs_create(self, project_name, experiment_name, data, **kwargs):
         """
         Create experiment run
 
         :param str project_name: the name of the project (required)
         :param str experiment_name: the name of the experiment (required)
         :param ExperimentRunCreate data: the details of the experiment run (required)
+        :param kwargs:
+            - int timeout
 
         :return: ExperimentRunCreateResponse
         """
 
         if project_name is None:
             raise ApiValueError("Missing the required parameter `project_name`")
         if experiment_name is None:
@@ -551,26 +582,29 @@
                 version=experiment_name,
                 data=[
                     {
                         "name": data.name,
                         "description": data.description,
                         "training_code": data.training_code,
                         "training_data": data.training_data,
-                        "parameters": data.parameters if data.parameters is not None else {},
+                        "parameters": (data.parameters if data.parameters is not None else {}),
                     }
                 ],
                 **kwargs,
             )[0]
         except ApiException as e:
             raise self.wrap_exception(e)
 
-        from ubiops.training.experiment_run_create_response import ExperimentRunCreateResponse
+        from ubiops.training.experiment_run_create_response import (
+            ExperimentRunCreateResponse,
+        )
 
         return ExperimentRunCreateResponse(
-            experiment=deployment_version_request.version, **deployment_version_request.to_dict()
+            experiment=deployment_version_request.version,
+            **deployment_version_request.to_dict(),
         )
 
     def experiment_runs_delete(self, project_name, experiment_name, run_id, **kwargs):
         """
         Delete run
 
         :param str project_name: the name of the project (required)
@@ -723,15 +757,17 @@
                 request_id=run_id,
                 data=data,
                 **kwargs,
             )
         except ApiException as e:
             raise self.wrap_exception(e)
 
-        from ubiops.training.experiment_run_update_response import ExperimentRunUpdateResponse
+        from ubiops.training.experiment_run_update_response import (
+            ExperimentRunUpdateResponse,
+        )
 
         return ExperimentRunUpdateResponse(experiment=request.version, **request.to_dict())
 
     def experiment_environment_variables_create(self, project_name, experiment_name, data, **kwargs):
         """
         Create an environment variable for the experiment. Variables inherited from the project can be shadowed by
         creating a variable with the same name.
@@ -750,15 +786,17 @@
         if data is None:
             raise ApiValueError("Missing the required parameter `data`")
         if project_name is not None and not isinstance(project_name, str):
             raise ApiValueError("Parameter `project_name` must be a string")
         if experiment_name is not None and not isinstance(experiment_name, str):
             raise ApiValueError("Parameter `experiment_name` must be a string")
         if data is not None:
-            from ubiops.models.environment_variable_create import EnvironmentVariableCreate
+            from ubiops.models.environment_variable_create import (
+                EnvironmentVariableCreate,
+            )
 
             if isinstance(data, dict):
                 data = EnvironmentVariableCreate(**data)
 
             elif not isinstance(data, EnvironmentVariableCreate):
                 raise ApiValueError("Parameter `data` must be an instance of EnvironmentVariableCreate")
 
@@ -896,15 +934,17 @@
         if project_name is not None and not isinstance(project_name, str):
             raise ApiValueError("Parameter `project_name` must be a string")
         if experiment_name is not None and not isinstance(experiment_name, str):
             raise ApiValueError("Parameter `experiment_name` must be a string")
         if id is not None and not isinstance(id, str):
             raise ApiValueError("Parameter `id` must be a string")
         if data is not None:
-            from ubiops.models.environment_variable_create import EnvironmentVariableCreate
+            from ubiops.models.environment_variable_create import (
+                EnvironmentVariableCreate,
+            )
 
             if isinstance(data, dict):
                 data = EnvironmentVariableCreate(**data)
 
             elif not isinstance(data, EnvironmentVariableCreate):
                 raise ApiValueError("Parameter `data` must be an instance of EnvironmentVariableCreate")
```

### Comparing `ubiops-4.3.0/ubiops/utils/__init__.py` & `ubiops-4.4.0/ubiops/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .file_operations import download_file, handle_file_input, UbiOpsFile, upload_file
+from .metrics.metric_client import MetricClient
 from .run_local import run_local
 from .validate import validate_requirements_file, validate_yaml_file
 from .wait_for import (
     wait_for_deployment_version,
     wait_for_environment,
     wait_for_experiment,
     wait_for_revision,
```

### Comparing `ubiops-4.3.0/ubiops/utils/metrics/metric_client.py` & `ubiops-4.4.0/ubiops/utils/metrics/metric_client.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/utils/metrics/metric_utils.py` & `ubiops-4.4.0/ubiops/utils/metrics/metric_utils.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/utils/run_local.py` & `ubiops-4.4.0/ubiops/utils/run_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,32 +180,43 @@
         raise FileNotFoundError("Deployment directory not found")
 
     _append_libraries_to_sys_path(deployment_directory=deployment_directory)
 
     # Create module from spec and initialize it
     module_from_spec = _create_module_from_spec(deployment_directory=deployment_directory)
     deployment_instance = _create_deployment_instance(
-        module_from_spec=module_from_spec, deployment_directory=deployment_directory, context=init_context
+        module_from_spec=module_from_spec,
+        deployment_directory=deployment_directory,
+        context=init_context,
     )
 
     # Return the result
     if hasattr(deployment_instance, "request") and not isinstance(data, list):
         # 'request' function and data is a single item
         return _create_request(
-            deployment_instance=deployment_instance, request_function="request", data=data, context=request_context
+            deployment_instance=deployment_instance,
+            request_function="request",
+            data=data,
+            context=request_context,
         )
     elif hasattr(deployment_instance, "requests") and isinstance(data, list):
         # 'requests' function and data is a list
         return _create_request(
-            deployment_instance=deployment_instance, request_function="requests", data=data, context=request_context
+            deployment_instance=deployment_instance,
+            request_function="requests",
+            data=data,
+            context=request_context,
         )
     elif hasattr(deployment_instance, "requests") and not isinstance(data, list):
         # 'requests' function and data is NOT a list -> make it a list
         return _create_request(
-            deployment_instance=deployment_instance, request_function="requests", data=[data], context=request_context
+            deployment_instance=deployment_instance,
+            request_function="requests",
+            data=[data],
+            context=request_context,
         )
     elif hasattr(deployment_instance, "request") and isinstance(data, list):
         # 'request' function and data is a list -> loop over the items in the list
         result = []
         for data_item in data:
             result.append(
                 _create_request(
```

### Comparing `ubiops-4.3.0/ubiops/utils/validate.py` & `ubiops-4.4.0/ubiops/utils/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import logging
 
 import yaml
 
 from .exceptions import ValidateError, ValidateSkip, ValidateWarning
-from .validators import validate_requirement_line, validate_yaml_apt, validate_yaml_env_vars
+from .validators import (
+    validate_requirement_line,
+    validate_yaml_apt,
+    validate_yaml_env_vars,
+)
 
 
 logger = logging.getLogger("Validate")
 
 
 def validate_requirements_file(file_path):
     """
```

### Comparing `ubiops-4.3.0/ubiops/utils/validators/validate_requirements_file.py` & `ubiops-4.4.0/ubiops/utils/validators/validate_requirements_file.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/utils/validators/validate_yaml_file.py` & `ubiops-4.4.0/ubiops/utils/validators/validate_yaml_file.py`

 * *Files identical despite different names*

### Comparing `ubiops-4.3.0/ubiops/utils/wait_for.py` & `ubiops-4.4.0/ubiops/utils/wait_for.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 LOGS_COMPLETION_SECONDS = 20
 NO_LOGS_MESSAGE_SECONDS = 20
 PENDING_REQUEST_STATUS = "pending"
 SUCCESS_STATUSES = ["available", "completed", "confirmation", "success"]
 FAILED_STATUSES = ["failed", "cancelled"]
 
 
-def _wait_for(client, retrieve_method, retrieve_kwargs, object_name="Deployment version", timeout=1800, quiet=False):
+def _wait_for(
+    client,
+    retrieve_method,
+    retrieve_kwargs,
+    object_name="Deployment version",
+    timeout=1800,
+    quiet=False,
+):
     """
     Wait for base method. Prints status updates with dots if quiet=False.
 
     :param str retrieve_method: retrieve method to get status updates
     :param dict retrieve_kwargs: the data to pass to the retrieve method
     :param str object_name: reference name for the object to wait for, used to print messages
     :param float timeout: the maximum time to wait
@@ -155,20 +162,25 @@
             if has_logs:
                 date = None
                 log_id = logs[-1].id
                 last_retrieve_time = time()
 
             if time() - last_retrieve_time > NO_LOGS_MESSAGE_SECONDS:
                 print(
-                    "No logs have been received for the last %.0f seconds" % (time() - last_retrieve_time), flush=True
+                    "No logs have been received for the last %.0f seconds" % (time() - last_retrieve_time),
+                    flush=True,
                 )
 
             # Handle timeout
             if time() - start_time > timeout:
-                raise ApiException(status=504, reason=f"{object_name} Timeout", body="Timeout was reached")
+                raise ApiException(
+                    status=504,
+                    reason=f"{object_name} Timeout",
+                    body="Timeout was reached",
+                )
 
             sleep(3)
 
             if not has_logs:
                 sleep(3)
                 break
 
@@ -280,15 +292,20 @@
         object_name=object_name,
         start_date=request_details.time_created.isoformat(timespec="milliseconds"),
         timeout=timeout,
     )
 
 
 def _wait_for_logs_pipeline_request(
-    client, project_name, retrieve_method, retrieve_kwargs, object_name="Pipeline request", timeout=1800
+    client,
+    project_name,
+    retrieve_method,
+    retrieve_kwargs,
+    object_name="Pipeline request",
+    timeout=1800,
 ):
     """
     Wait for a pipeline request to be completed and stream logs while waiting
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param retrieve_method: retrieve method to get status updates
@@ -332,26 +349,32 @@
             if object_type == "deployment":
                 _wait_for_logs_deployment_request(
                     client=client,
                     project_name=project_name,
                     deployment_name=request.deployment,
                     request_id=request.id,
                     retrieve_method="deployment_version_requests_get",
-                    retrieve_kwargs={**object_retrieve_kwargs, "deployment_name": request.deployment},
+                    retrieve_kwargs={
+                        **object_retrieve_kwargs,
+                        "deployment_name": request.deployment,
+                    },
                     object_name=object_request_name,
                     timeout=timeout,
                 )
 
             # Sub-pipelines
             elif object_type == "pipeline":
                 _wait_for_logs_pipeline_request(
                     client=client,
                     project_name=project_name,
                     retrieve_method="pipeline_version_requests_get",
-                    retrieve_kwargs={**object_retrieve_kwargs, "pipeline_name": request.pipeline},
+                    retrieve_kwargs={
+                        **object_retrieve_kwargs,
+                        "pipeline_name": request.pipeline,
+                    },
                     object_name=object_request_name,
                     timeout=timeout,
                 )
 
         if request_details.status in SUCCESS_STATUSES:
             print(f"{object_name}: {request_details.status}", flush=True)
             return
@@ -360,15 +383,22 @@
 
         # We are not waiting for any deployment request in this iteration, just waiting for the pipeline request status
         if not waiting_for_requests:
             sleep(2)
 
 
 def wait_for_deployment_version(
-    client, project_name, deployment_name, version, revision_id=None, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    deployment_name,
+    version,
+    revision_id=None,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a deployment version to be ready: wait for the environment build and deployment revision to complete
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str deployment_name: the name of the deployment
@@ -395,15 +425,21 @@
             object_name="Deployment version",
         )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_experiment(
-    client, project_name, experiment_name, revision_id=None, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    experiment_name,
+    revision_id=None,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for an experiment to be ready
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str experiment_name: the name of the experiment
@@ -455,30 +491,37 @@
     if environment.base_environment is None:
         # Environment is a base environment, it doesn't need to build
         if not quiet:
             print("Environment: success", flush=True)
         return
 
     if not environment.latest_build or not environment.latest_revision:
-        raise ApiException(status=404, reason="Not Found", body=f"No build found for environment {environment_name}")
+        raise ApiException(
+            status=404,
+            reason="Not Found",
+            body=f"No build found for environment {environment_name}",
+        )
 
     retrieve_method = "environment_builds_get"
     retrieve_kwargs = {
         "project_name": project_name,
         "environment_name": environment_name,
         "revision_id": environment.latest_revision,
         "build_id": environment.latest_build,
     }
 
     try:
         if stream_logs and not quiet:
             _wait_for_logs(
                 client=client,
                 project_name=project_name,
-                filters={"environment_name": environment_name, "environment_build_id": environment.latest_build},
+                filters={
+                    "environment_name": environment_name,
+                    "environment_build_id": environment.latest_build,
+                },
                 retrieve_method=retrieve_method,
                 retrieve_kwargs=retrieve_kwargs,
                 object_name="Environment",
                 start_date=environment.last_updated.isoformat(timespec="milliseconds"),
                 timeout=timeout,
             )
         else:
@@ -491,15 +534,22 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_revision(
-    client, project_name, deployment_name, version, revision_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    deployment_name,
+    version,
+    revision_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a deployment revision to be ready
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str deployment_name: the name of the deployment
@@ -550,15 +600,21 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_deployment_request(
-    client, project_name, deployment_name, request_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    deployment_name,
+    request_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a deployment request to be completed
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str deployment_name: the name of the deployment
@@ -603,15 +659,22 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_deployment_version_request(
-    client, project_name, deployment_name, version, request_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    deployment_name,
+    version,
+    request_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a deployment version request to be completed
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str deployment_name: the name of the deployment
@@ -658,15 +721,21 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_experiment_run(
-    client, project_name, experiment_name, run_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    experiment_name,
+    run_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for an experiment run to be completed
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str experiment_name: the name of the experiment
@@ -712,15 +781,21 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_pipeline_request(
-    client, project_name, pipeline_name, request_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    pipeline_name,
+    request_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a pipeline request to be completed
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str pipeline_name: the name of the pipeline
@@ -763,15 +838,22 @@
                 quiet=quiet,
             )
     except KeyboardInterrupt:
         pass
 
 
 def wait_for_pipeline_version_request(
-    client, project_name, pipeline_name, version, request_id, timeout=1800, quiet=False, stream_logs=False
+    client,
+    project_name,
+    pipeline_name,
+    version,
+    request_id,
+    timeout=1800,
+    quiet=False,
+    stream_logs=False,
 ):
     """
     Wait for a pipeline version request to be completed
 
     :param ubiops.ApiClient client: a preconfigured UbiOps client
     :param str project_name: the name of the project
     :param str pipeline_name: the name of the pipeline
```

### Comparing `ubiops-4.3.0/ubiops.egg-info/PKG-INFO` & `ubiops-4.4.0/ubiops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiops
-Version: 4.3.0
+Version: 4.4.0
 Summary: UbiOps
 Home-page: https://github.com/UbiOps/client-library-python.git
 Author: UbiOps
 License: Apache 2.0
 Description: # ubiops
         Client Library to interact with the [UbiOps](https://ubiops.com) API (v2.1).
```

### Comparing `ubiops-4.3.0/ubiops.egg-info/SOURCES.txt` & `ubiops-4.4.0/ubiops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 ubiops/models/deployment_request_single_detail.py
 ubiops/models/deployment_request_update.py
 ubiops/models/deployment_request_update_response.py
 ubiops/models/deployment_update.py
 ubiops/models/deployment_version_create.py
 ubiops/models/deployment_version_detail.py
 ubiops/models/deployment_version_list.py
+ubiops/models/deployment_version_port.py
 ubiops/models/deployment_version_update.py
 ubiops/models/direct_pipeline_request_deployment_request.py
 ubiops/models/direct_pipeline_request_operator_request.py
 ubiops/models/direct_pipeline_request_pipeline_request.py
 ubiops/models/environment_build_dependency.py
 ubiops/models/environment_build_list.py
 ubiops/models/environment_build_update.py
@@ -81,16 +82,18 @@
 ubiops/models/environment_variable_list.py
 ubiops/models/export_create.py
 ubiops/models/export_detail.py
 ubiops/models/export_list.py
 ubiops/models/expression_evaluate.py
 ubiops/models/expression_evaluate_response.py
 ubiops/models/expression_input_field_create.py
+ubiops/models/file_complete_multipart_upload.py
 ubiops/models/file_detail.py
 ubiops/models/file_item.py
+ubiops/models/file_multipart_upload.py
 ubiops/models/file_upload_response.py
 ubiops/models/import_detail.py
 ubiops/models/import_list.py
 ubiops/models/import_update.py
 ubiops/models/inherited_environment_variable_list.py
 ubiops/models/input_field_widget_create.py
 ubiops/models/input_output_field_base.py
@@ -173,14 +176,15 @@
 ubiops/models/time_series_data_create.py
 ubiops/models/time_series_data_list.py
 ubiops/models/time_series_data_point_create.py
 ubiops/models/time_series_data_point_list.py
 ubiops/models/time_series_search.py
 ubiops/models/user_pending_create.py
 ubiops/models/user_pending_detail.py
+ubiops/models/voucher.py
 ubiops/models/webhook_create.py
 ubiops/models/webhook_detail.py
 ubiops/models/webhook_header.py
 ubiops/models/webhook_test_create.py
 ubiops/models/webhook_test_detail.py
 ubiops/models/webhook_update.py
 ubiops/training/__init__.py
```

