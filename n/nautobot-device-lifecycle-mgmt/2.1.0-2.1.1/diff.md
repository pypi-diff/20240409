# Comparing `tmp/nautobot_device_lifecycle_mgmt-2.1.0.tar.gz` & `tmp/nautobot_device_lifecycle_mgmt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_device_lifecycle_mgmt-2.1.0.tar", max compression
+gzip compressed data, was "nautobot_device_lifecycle_mgmt-2.1.1.tar", max compression
```

## Comparing `nautobot_device_lifecycle_mgmt-2.1.0.tar` & `nautobot_device_lifecycle_mgmt-2.1.1.tar`

### file list

```diff
@@ -1,90 +1,215 @@
--rw-r--r--   0        0        0      591 2024-01-27 02:25:41.828376 nautobot_device_lifecycle_mgmt-2.1.0/LICENSE
--rw-r--r--   0        0        0     5895 2024-01-27 02:25:41.828376 nautobot_device_lifecycle_mgmt-2.1.0/README.md
--rw-r--r--   0        0        0     1417 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/__init__.py
--rw-r--r--   0        0        0       62 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/__init__.py
--rw-r--r--   0        0        0     3351 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/serializers.py
--rw-r--r--   0        0        0     1253 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/urls.py
--rw-r--r--   0        0        0     4549 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/views.py
--rw-r--r--   0        0        0     2132 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/choices.py
--rw-r--r--   0        0        0    29467 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/filters.py
--rw-r--r--   0        0        0    35314 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/forms.py
--rw-r--r--   0        0        0      663 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/graphql/types.py
--rw-r--r--   0        0        0      393 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/jobs/__init__.py
--rw-r--r--   0        0        0     3054 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
--rw-r--r--   0        0        0     3279 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
--rw-r--r--   0        0        0     9805 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/metrics.py
--rw-r--r--   0        0        0     3448 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
--rw-r--r--   0        0        0     4318 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
--rw-r--r--   0        0        0     5579 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
--rw-r--r--   0        0        0     2681 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0004_squash__0004_0014_0015_0016.py
--rw-r--r--   0        0        0     2377 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
--rw-r--r--   0        0        0     4404 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
--rw-r--r--   0        0        0     4793 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
--rw-r--r--   0        0        0     3130 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
--rw-r--r--   0        0        0     1122 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
--rw-r--r--   0        0        0      611 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
--rw-r--r--   0        0        0      462 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
--rw-r--r--   0        0        0      983 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
--rw-r--r--   0        0        0      901 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
--rw-r--r--   0        0        0      567 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py
--rw-r--r--   0        0        0      709 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0014_pre_nautobot_v2_migrations.py
--rw-r--r--   0        0        0     1473 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0015_role_migration.py
--rw-r--r--   0        0        0     1429 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0016_role_migration_cleanup.py
--rw-r--r--   0        0        0     3453 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0017_set_default_on_text_fields.py
--rw-r--r--   0        0        0     3292 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0018_text_fields_default_and_new_m2m_fields.py
--rw-r--r--   0        0        0     3473 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0019_cve_and_contract_m2m_migration.py
--rw-r--r--   0        0        0     5185 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0020_alter_created_tags.py
--rw-r--r--   0        0        0        0 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/__init__.py
--rw-r--r--   0        0        0    24176 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/models.py
--rw-r--r--   0        0        0    14171 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/navigation.py
--rw-r--r--   0        0        0     3672 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/signals.py
--rw-r--r--   0        0        0     3023 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/software.py
--rw-r--r--   0        0        0     7921 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/software_filters.py
--rw-r--r--   0        0        0    20974 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tables.py
--rw-r--r--   0        0        0     5600 2024-01-27 02:25:41.844376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/template_content.py
--rw-r--r--   0        0        0     2094 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm_retrieve.html
--rw-r--r--   0        0        0     6229 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm_retrieve.html
--rw-r--r--   0        0        0     2848 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm_retrieve.html
--rw-r--r--   0        0        0      492 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
--rw-r--r--   0        0        0      939 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
--rw-r--r--   0        0        0     1523 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
--rw-r--r--   0        0        0     2613 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_retrieve.html
--rw-r--r--   0        0        0     5632 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
--rw-r--r--   0        0        0     2160 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
--rw-r--r--   0        0        0      513 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
--rw-r--r--   0        0        0     1113 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
--rw-r--r--   0        0        0      761 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
--rw-r--r--   0        0        0      365 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
--rw-r--r--   0        0        0      505 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
--rw-r--r--   0        0        0     3605 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm_retrieve.html
--rw-r--r--   0        0        0      263 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
--rw-r--r--   0        0        0     1971 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
--rw-r--r--   0        0        0       92 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
--rw-r--r--   0        0        0     5075 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_retrieve.html
--rw-r--r--   0        0        0      251 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
--rw-r--r--   0        0        0       86 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
--rw-r--r--   0        0        0     3136 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_retrieve.html
--rw-r--r--   0        0        0      420 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
--rw-r--r--   0        0        0     5801 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
--rw-r--r--   0        0        0     5902 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
--rw-r--r--   0        0        0      269 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
--rw-r--r--   0        0        0     1942 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
--rw-r--r--   0        0        0       96 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
--rw-r--r--   0        0        0     5686 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_retrieve.html
--rw-r--r--   0        0        0      625 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
--rw-r--r--   0        0        0     1599 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_retrieve.html
--rw-r--r--   0        0        0       57 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/__init__.py
--rw-r--r--   0        0        0     6051 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/conftest.py
--rw-r--r--   0        0        0    27004 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_api.py
--rw-r--r--   0        0        0     1582 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_basic.py
--rw-r--r--   0        0        0    32326 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py
--rw-r--r--   0        0        0    24380 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py
--rw-r--r--   0        0        0    32779 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_model.py
--rw-r--r--   0        0        0    12835 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
--rw-r--r--   0        0        0    17375 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_views.py
--rw-r--r--   0        0        0     1905 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/urls.py
--rw-r--r--   0        0        0      420 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/utils.py
--rw-r--r--   0        0        0    20109 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/views.py
--rw-r--r--   0        0        0     6554 2024-01-27 02:25:41.848376 nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/viewsets.py
--rw-r--r--   0        0        0     3655 2024-01-27 02:25:48.820355 nautobot_device_lifecycle_mgmt-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6927 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-09 13:08:12.197481 nautobot_device_lifecycle_mgmt-2.1.1/LICENSE
+-rw-r--r--   0        0        0     5908 2024-04-09 13:08:12.197481 nautobot_device_lifecycle_mgmt-2.1.1/README.md
+-rw-r--r--   0        0        0     1407 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/__init__.py
+-rw-r--r--   0        0        0     3351 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/serializers.py
+-rw-r--r--   0        0        0     1253 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/urls.py
+-rw-r--r--   0        0        0     4549 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/views.py
+-rw-r--r--   0        0        0        5 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/app-config-schema.json
+-rw-r--r--   0        0        0     2132 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/choices.py
+-rw-r--r--   0        0        0    29467 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/filters.py
+-rw-r--r--   0        0        0    35306 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/forms.py
+-rw-r--r--   0        0        0      663 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/graphql/types.py
+-rw-r--r--   0        0        0      393 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/jobs/__init__.py
+-rw-r--r--   0        0        0     3054 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py
+-rw-r--r--   0        0        0     3279 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py
+-rw-r--r--   0        0        0     9905 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/metrics.py
+-rw-r--r--   0        0        0     3448 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py
+-rw-r--r--   0        0        0     4318 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py
+-rw-r--r--   0        0        0     5579 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py
+-rw-r--r--   0        0        0     2681 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0004_squash__0004_0014_0015_0016.py
+-rw-r--r--   0        0        0     2377 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py
+-rw-r--r--   0        0        0     4404 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py
+-rw-r--r--   0        0        0     4793 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py
+-rw-r--r--   0        0        0     3130 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py
+-rw-r--r--   0        0        0     1122 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py
+-rw-r--r--   0        0        0      611 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py
+-rw-r--r--   0        0        0      462 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0010_softwareimagelcm_hash_algorithm.py
+-rw-r--r--   0        0        0      983 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py
+-rw-r--r--   0        0        0      901 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py
+-rw-r--r--   0        0        0      567 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py
+-rw-r--r--   0        0        0      709 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0014_pre_nautobot_v2_migrations.py
+-rw-r--r--   0        0        0     1473 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0015_role_migration.py
+-rw-r--r--   0        0        0     1429 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0016_role_migration_cleanup.py
+-rw-r--r--   0        0        0     3453 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0017_set_default_on_text_fields.py
+-rw-r--r--   0        0        0     3292 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0018_text_fields_default_and_new_m2m_fields.py
+-rw-r--r--   0        0        0     3473 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0019_cve_and_contract_m2m_migration.py
+-rw-r--r--   0        0        0     5185 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0020_alter_created_tags.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/__init__.py
+-rw-r--r--   0        0        0    24176 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/models.py
+-rw-r--r--   0        0        0    14171 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/navigation.py
+-rw-r--r--   0        0        0     3672 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/signals.py
+-rw-r--r--   0        0        0     3023 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/software.py
+-rw-r--r--   0        0        0     7921 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/software_filters.py
+-rw-r--r--   0        0        0    35510 2024-04-09 13:08:52.022443 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/404.html
+-rw-r--r--   0        0        0    37632 2024-04-09 13:08:52.046444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    46992 2024-04-09 13:08:52.050444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/install.html
+-rw-r--r--   0        0        0    36967 2024-04-09 13:08:52.058444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    40918 2024-04-09 13:08:52.062444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_0.1.html
+-rw-r--r--   0        0        0    45299 2024-04-09 13:08:52.066444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_0.2.html
+-rw-r--r--   0        0        0    41773 2024-04-09 13:08:52.070444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_0.3.html
+-rw-r--r--   0        0        0    42441 2024-04-09 13:08:52.074444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_0.4.html
+-rw-r--r--   0        0        0    44784 2024-04-09 13:08:52.078444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    46449 2024-04-09 13:08:52.082445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_1.1.html
+-rw-r--r--   0        0        0    41632 2024-04-09 13:08:52.082445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_1.2.html
+-rw-r--r--   0        0        0    45551 2024-04-09 13:08:52.086444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_1.3.html
+-rw-r--r--   0        0        0    42916 2024-04-09 13:08:52.090445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_1.6.html
+-rw-r--r--   0        0        0    50088 2024-04-09 13:08:52.094445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    42977 2024-04-09 13:08:52.098445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/release_notes/version_2.1.html
+-rw-r--r--   0        0        0    39903 2024-04-09 13:08:52.054444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    41392 2024-04-09 13:08:52.058444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-04-09 13:08:51.910440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0    37520 2024-04-09 13:08:52.102445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/arch_decision.html
+-rw-r--r--   0        0        0   143054 2024-04-09 13:08:52.178447 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    37092 2024-04-09 13:08:52.126445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0   355619 2024-04-09 13:08:52.354451 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/code_reference/models.html
+-rw-r--r--   0        0        0    49916 2024-04-09 13:08:52.362451 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    44704 2024-04-09 13:08:52.106445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/contributing.html
+-rw-r--r--   0        0        0   100550 2024-04-09 13:08:52.122445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    37248 2024-04-09 13:08:52.126445 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/dev/extending.html
+-rw-r--r--   0        0        0    23874 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/icon-DeviceLifecycle.png
+-rw-r--r--   0        0        0   265568 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_contract_detail.png
+-rw-r--r--   0        0        0   263083 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_contract_provider_detail.png
+-rw-r--r--   0        0        0   162980 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_contract_providers_view.png
+-rw-r--r--   0        0        0   203621 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_contract_view.png
+-rw-r--r--   0        0        0    18508 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_cve_breadcrumb.png
+-rw-r--r--   0        0        0   101327 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_api_view.png
+-rw-r--r--   0        0        0   102949 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_detail_view.png
+-rw-r--r--   0        0        0   104691 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_device_type_view.png
+-rw-r--r--   0        0        0   217481 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_device_view.png
+-rw-r--r--   0        0        0   251878 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_graphql.png
+-rw-r--r--   0        0        0    75818 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_hardware_list_view.png
+-rw-r--r--   0        0        0    32096 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_breadcrumb.png
+-rw-r--r--   0        0        0    58977 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_detail_view.png
+-rw-r--r--   0        0        0    69828 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_device_view_invalid.png
+-rw-r--r--   0        0        0    71319 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_device_view_valid.png
+-rw-r--r--   0        0        0    53032 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_image_add.png
+-rw-r--r--   0        0        0    70012 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_image_detail_view.png
+-rw-r--r--   0        0        0    74130 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_image_list_view.png
+-rw-r--r--   0        0        0    41032 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_list_view.png
+-rw-r--r--   0        0        0    30488 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_software_add.png
+-rw-r--r--   0        0        0    22706 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_software_add_example.png
+-rw-r--r--   0        0        0    25654 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validated_software_add_example.png
+-rw-r--r--   0        0        0     1425 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_export_button.png
+-rw-r--r--   0        0        0     2934 2024-04-09 13:08:51.902440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_export_button_green.png
+-rw-r--r--   0        0        0   102689 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_csv.png
+-rw-r--r--   0        0        0    21480 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_csv_small.png
+-rw-r--r--   0        0        0    10692 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run.png
+-rw-r--r--   0        0        0    38780 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run_detailed_summary.png
+-rw-r--r--   0        0        0    29164 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run_executive_summary.png
+-rw-r--r--   0        0        0    41626 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run_graph.png
+-rw-r--r--   0        0        0    37689 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run_jobs.png
+-rw-r--r--   0        0        0   116440 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_report_run_results_list.png
+-rw-r--r--   0        0        0    31180 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_software_validation_reports_export_button.png
+-rw-r--r--   0        0        0    51974 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_validated_software_detail_view.png
+-rw-r--r--   0        0        0    32708 2024-04-09 13:08:51.906440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/images/lcm_validated_software_list_view.png
+-rw-r--r--   0        0        0    46068 2024-04-09 13:08:52.042444 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/index.html
+-rw-r--r--   0        0        0      793 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-04-09 13:08:51.898440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/requirements.txt
+-rw-r--r--   0        0        0   191430 2024-04-09 13:08:52.422453 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/search/search_index.json
+-rw-r--r--   0        0        0     7270 2024-04-09 13:08:51.914440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/sitemap.xml
+-rw-r--r--   0        0        0      504 2024-04-09 13:08:51.918440 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    40798 2024-04-09 13:08:52.366451 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    42624 2024-04-09 13:08:52.366451 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/app_overview.html
+-rw-r--r--   0        0        0    54879 2024-04-09 13:08:52.374451 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    45545 2024-04-09 13:08:52.382452 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/cve_tracking.html
+-rw-r--r--   0        0        0    45882 2024-04-09 13:08:52.386452 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/external_interactions.html
+-rw-r--r--   0        0        0    40222 2024-04-09 13:08:52.390452 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/faq.html
+-rw-r--r--   0        0        0    51930 2024-04-09 13:08:52.394452 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/lifecycle_reporting.html
+-rw-r--r--   0        0        0    45514 2024-04-09 13:08:52.398452 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/metrics.html
+-rw-r--r--   0        0        0   104801 2024-04-09 13:08:52.422453 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/static/nautobot_device_lifecycle_mgmt/docs/user/software_lifecycle.html
+-rw-r--r--   0        0        0    20974 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tables.py
+-rw-r--r--   0        0        0     5600 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/template_content.py
+-rw-r--r--   0        0        0     2094 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm_retrieve.html
+-rw-r--r--   0        0        0     6229 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm_retrieve.html
+-rw-r--r--   0        0        0     2848 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm_retrieve.html
+-rw-r--r--   0        0        0      492 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0      939 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html
+-rw-r--r--   0        0        0     1523 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html
+-rw-r--r--   0        0        0     2613 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_retrieve.html
+-rw-r--r--   0        0        0     5632 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html
+-rw-r--r--   0        0        0     2160 2024-04-09 13:08:12.217481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html
+-rw-r--r--   0        0        0      513 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html
+-rw-r--r--   0        0        0     1113 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html
+-rw-r--r--   0        0        0      761 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html
+-rw-r--r--   0        0        0      365 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validatedsoftware_info.html
+-rw-r--r--   0        0        0      505 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html
+-rw-r--r--   0        0        0     3605 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm_retrieve.html
+-rw-r--r--   0        0        0      263 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_delete.html
+-rw-r--r--   0        0        0     1971 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html
+-rw-r--r--   0        0        0       92 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_list.html
+-rw-r--r--   0        0        0     5075 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_retrieve.html
+-rw-r--r--   0        0        0      251 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_delete.html
+-rw-r--r--   0        0        0       86 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_list.html
+-rw-r--r--   0        0        0     3136 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_retrieve.html
+-rw-r--r--   0        0        0      420 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html
+-rw-r--r--   0        0        0     5801 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html
+-rw-r--r--   0        0        0     5902 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html
+-rw-r--r--   0        0        0      269 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_delete.html
+-rw-r--r--   0        0        0     1942 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html
+-rw-r--r--   0        0        0       96 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_list.html
+-rw-r--r--   0        0        0     5686 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_retrieve.html
+-rw-r--r--   0        0        0      625 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html
+-rw-r--r--   0        0        0     1599 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_retrieve.html
+-rw-r--r--   0        0        0       57 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/__init__.py
+-rw-r--r--   0        0        0     7185 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/conftest.py
+-rw-r--r--   0        0        0    27004 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_api.py
+-rw-r--r--   0        0        0     1041 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_basic.py
+-rw-r--r--   0        0        0    32326 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py
+-rw-r--r--   0        0        0    24380 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py
+-rw-r--r--   0        0        0     4155 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_metrics.py
+-rw-r--r--   0        0        0    32779 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_model.py
+-rw-r--r--   0        0        0    12835 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py
+-rw-r--r--   0        0        0    17375 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_views.py
+-rw-r--r--   0        0        0     1868 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/urls.py
+-rw-r--r--   0        0        0      420 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/utils.py
+-rw-r--r--   0        0        0    26112 2024-04-09 13:08:12.221481 nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/views.py
+-rw-r--r--   0        0        0     5832 2024-04-09 13:08:27.821868 nautobot_device_lifecycle_mgmt-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7064 1970-01-01 00:00:00.000000 nautobot_device_lifecycle_mgmt-2.1.1/PKG-INFO
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/LICENSE` & `nautobot_device_lifecycle_mgmt-2.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2023, Network to Code, LLC
+Copyright (c) 2024, Network to Code, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/README.md` & `nautobot_device_lifecycle_mgmt-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Device Lifecycle Management
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-device-lifecycle-mgmt/develop/docs/images/icon-DeviceLifecycle.png" class="logo" height="200px">
   <br>
   <a href="https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt/actions"><img src="https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/device-lifecycle/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-device-lifecycle-mgmt/badge/"></a>
+  <a href="https://docs.nautobot.com/projects/device-lifecycle/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-nautobot-device-lifecycle-mgmt/badge/"></a>
   <a href="https://pypi.org/project/nautobot-device-lifecycle-mgmt/"><img src="https://img.shields.io/pypi/v/nautobot-device-lifecycle-mgmt"></a>
   <a href="https://pypi.org/project/nautobot-device-lifecycle-mgmt/"><img src="https://img.shields.io/pypi/dm/nautobot-device-lifecycle-mgmt"></a>
   <br>
   An App for <a href="https://github.com/nautobot/nautobot">Nautobot</a>.
 </p>
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # Device Lifecycle Management
 [https://raw.githubusercontent.com/nautobot/nautobot-app-device-lifecycle-mgmt/
                  develop/docs/images/icon-DeviceLifecycle.png]
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_a_c_t_i_o_n_s_/
    _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/
-   _n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
-_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
-                                _l_i_f_e_c_y_c_l_e_-_m_g_m_t_]
+_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-
+                            _d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]
                              An App for _N_a_u_t_o_b_o_t.
 ## Overview An app for [Nautobot](https://github.com/nautobot/nautobot) to
 manage device lifecycles. This app works by making related associations to
 Devices, Device Types, and Inventory Items to help provide data about the
 hardware end of life notices, appropriate software versions to be running on
 the devices, and the maintenance contracts associated with devices. This will
 help with the various aspects of planning Lifecycle events, and provides quick
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/__init__.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """App declaration for nautobot_device_lifecycle_mgmt."""
 # Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 from importlib import metadata
 
-__version__ = metadata.version(__name__)
-
+from nautobot.apps import NautobotAppConfig
 from nautobot.core.signals import nautobot_database_ready
-from nautobot.extras.plugins import NautobotAppConfig
+
+__version__ = metadata.version(__name__)
 
 
 class NautobotDeviceLifecycleManagementConfig(NautobotAppConfig):
     """App configuration for the Device Lifecycle Management app."""
 
     name = "nautobot_device_lifecycle_mgmt"
     verbose_name = "Nautobot Device Lifecycle Management"
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/serializers.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/urls.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/api/views.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/choices.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/filters.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/forms.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
         return {"provider": self.request.GET.get("provider")}  # pylint: disable=E1101
 
 
 class ContractLCMBulkEditForm(NautobotBulkEditForm):
     """Device Lifecycle Contrcts bulk edit form."""
 
     pk = forms.ModelMultipleChoiceField(queryset=ContractLCM.objects.all(), widget=forms.MultipleHiddenInput)
-    provider = forms.ModelMultipleChoiceField(queryset=ProviderLCM.objects.all(), required=False)
+    provider = forms.ModelChoiceField(queryset=ProviderLCM.objects.all(), required=False)
     start = forms.DateField(widget=DatePicker(), required=False)
     end = forms.DateField(widget=DatePicker(), required=False)
     cost = forms.FloatField(required=False)
     currency = forms.ChoiceField(required=False, choices=CurrencyChoices.CHOICES)
     contract_type = forms.ChoiceField(choices=ContractTypeChoices.CHOICES, required=False)
     support_level = forms.CharField(required=False)
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/graphql/types.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/graphql/types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/jobs/cve_tracking.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/jobs/lifecycle_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/metrics.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
         GaugeMetricFamily: Prometheus Metrics
     """
     inventory_item_software_compliance_gauge = GaugeMetricFamily(
         "nautobot_lcm_software_compliance_per_inventory_item",
         "Number of devices that have valid/invalid software by inventory item",
         labels=["inventory_item", "is_valid"],
     )
-    inventory_item_part_ids = InventoryItem.objects.exclude(part_id="").order_by().values("part_id").distinct()
+    inventory_item_part_ids = (
+        InventoryItem.objects.exclude(part_id="").without_tree_fields().order_by().values("part_id").distinct()
+    )
 
     # Annotate InventoryItemSoftwareValidationResult with counts for valid and invalid software per part id
     validation_counts = (
         InventoryItemSoftwareValidationResult.objects.exclude(inventory_item__part_id="")
         .order_by()
         .values(part_id=F("inventory_item__part_id"))
         .annotate(
@@ -146,15 +148,16 @@
     ):
         hw_end_of_support_part_number_gauge.add_metric(
             labels=[part_number if part_number else model], value=device_count
         )
 
     # Generate metrics with counts for out of support inventory items per part id
     for part_id, inv_item_count in (
-        InventoryItem.objects.order_by()
+        InventoryItem.objects.without_tree_fields()
+        .order_by()
         .filter(part_id__in=hw_end_of_support_invitems)
         .values("part_id")
         .annotate(inv_item_count=Count("id"))
         .values_list("part_id", "inv_item_count")
     ):
         hw_end_of_support_part_number_gauge.add_metric(labels=[part_id], value=inv_item_count)
 
@@ -192,15 +195,16 @@
         Device.objects.order_by()
         .filter(device_type_id__in=hw_end_of_support_device_types)
         .values(location_name=F("location__name"))
         .annotate(location_count=Count("id"))
     )
     # Get count of out of hw support inventory items per location
     hw_end_of_support_per_location_invitems = (
-        InventoryItem.objects.order_by()
+        InventoryItem.objects.without_tree_fields()
+        .order_by()
         .filter(part_id__in=hw_end_of_support_invitems)
         .values(location_name=F("device__location__name"))
         .annotate(location_count=Count("id"))
     )
 
     # Build subqueries used in the final query offloading count sum to the DB
     hw_end_of_support_per_location_devices_sq = Subquery(
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0001_hardwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0002_softwarelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0003_service_contracts.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0004_squash__0004_0014_0015_0016.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0004_squash__0004_0014_0015_0016.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0004_validated_software_m2m.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0005_software_reporting.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0006_cvelcm_vulnerabilitylcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0007_softwareimagelcm.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0008_software_image_data_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0009_software_remove_image_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0011_add_valid_software_field_to_result.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0012_add_related_name_to_results_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0013_alter_softwareimagelcm_device_types.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0014_pre_nautobot_v2_migrations.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0014_pre_nautobot_v2_migrations.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0015_role_migration.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0015_role_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0016_role_migration_cleanup.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0016_role_migration_cleanup.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0017_set_default_on_text_fields.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0017_set_default_on_text_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0018_text_fields_default_and_new_m2m_fields.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0018_text_fields_default_and_new_m2m_fields.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0019_cve_and_contract_m2m_migration.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0019_cve_and_contract_m2m_migration.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/migrations/0020_alter_created_tags.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/migrations/0020_alter_created_tags.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/models.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/navigation.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/signals.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/software.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/software.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/software_filters.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tables.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/template_content.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contactlcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/contractlcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/cvelcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_delete.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/hardwarelcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/device_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/general_notice.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_and_validatedsoftware_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/software_info.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/inc/validated_report_actions.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/providerlcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwareimagelcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/softwarelcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_edit.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/validatedsoftwarelcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_retrieve.html` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/templates/nautobot_device_lifecycle_mgmt/vulnerabilitylcm_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/conftest.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Params for testing."""
 from datetime import date
 
 from django.contrib.contenttypes.models import ContentType
 from nautobot.dcim.models import Device, DeviceType, InventoryItem, Location, LocationType, Manufacturer, Platform
 from nautobot.extras.models import Role, Status
 
-from nautobot_device_lifecycle_mgmt.models import CVELCM, SoftwareLCM, ValidatedSoftwareLCM
+from nautobot_device_lifecycle_mgmt.models import CVELCM, HardwareLCM, SoftwareLCM, ValidatedSoftwareLCM
 
 
 def create_devices():
     """Create devices for tests."""
     device_platform, _ = Platform.objects.get_or_create(name="cisco_ios")
     manufacturer, _ = Manufacturer.objects.get_or_create(name="Cisco")
     device_type, _ = DeviceType.objects.get_or_create(manufacturer=manufacturer, model="6509-E")
@@ -156,7 +156,38 @@
         software_one,
         software_two,
         validatedsoftwarelcm,
         validatedsoftwarelcm_two,
     )
 
     return validated_items
+
+
+def create_inventory_item_hardware_notices():
+    """Create inventory item hardware notices for tests."""
+
+    return (
+        HardwareLCM.objects.create(
+            inventory_item="VS-S2T-10G",
+            end_of_sale=date(2022, 4, 1),
+            end_of_support=date(2023, 4, 1),
+            end_of_sw_releases=date(2024, 4, 1),
+            end_of_security_patches=date(2025, 4, 1),
+            documentation_url="https://test.com",
+        ),
+        HardwareLCM.objects.create(
+            inventory_item="QSFP-100G-SR4-S",
+            end_of_sale=date(2022, 4, 1),
+            end_of_support=date(2024, 1, 1),
+            end_of_sw_releases=date(2024, 4, 1),
+            end_of_security_patches=date(2025, 4, 1),
+            documentation_url="https://test.com",
+        ),
+        HardwareLCM.objects.create(
+            inventory_item="WS-X6548-GE-TX",
+            end_of_sale=date(2022, 4, 1),
+            end_of_support=date(2999, 1, 1),
+            end_of_sw_releases=date(2024, 4, 1),
+            end_of_security_patches=date(2025, 4, 1),
+            documentation_url="https://test.com",
+        ),
+    )
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_api.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_filters.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_forms.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_model.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_software_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/tests/test_views.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/urls.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Django urlpatterns declaration for the Lifecycle Management app."""
 from django.urls import path
 from nautobot.apps.urls import NautobotUIViewSetRouter
 
-from nautobot_device_lifecycle_mgmt import views, viewsets
+from nautobot_device_lifecycle_mgmt import views
 
 router = NautobotUIViewSetRouter()
-router.register("hardware", viewset=viewsets.HardwareLCMUIViewSet)
-router.register("software", viewset=viewsets.SoftwareLCMUIViewSet)
-router.register("software-image", viewset=viewsets.SoftwareImageLCMUIViewSet)
-router.register("validated-software", viewset=viewsets.ValidatedSoftwareLCMUIViewSet)
-router.register("contract", viewset=viewsets.ContractLCMUIViewSet)
-router.register("provider", viewset=viewsets.ProviderLCMUIViewSet)
-router.register("contact", viewset=viewsets.ContactLCMUIViewSet)
-router.register("cve", viewset=viewsets.CVELCMUIViewSet)
-router.register("vulnerability", viewset=viewsets.VulnerabilityLCMUIViewSet)
+router.register("hardware", viewset=views.HardwareLCMUIViewSet)
+router.register("software", viewset=views.SoftwareLCMUIViewSet)
+router.register("software-image", viewset=views.SoftwareImageLCMUIViewSet)
+router.register("validated-software", viewset=views.ValidatedSoftwareLCMUIViewSet)
+router.register("contract", viewset=views.ContractLCMUIViewSet)
+router.register("provider", viewset=views.ProviderLCMUIViewSet)
+router.register("contact", viewset=views.ContactLCMUIViewSet)
+router.register("cve", viewset=views.CVELCMUIViewSet)
+router.register("vulnerability", viewset=views.VulnerabilityLCMUIViewSet)
 
 urlpatterns = router.urls
 
 urlpatterns += [
     path(
         "software/<uuid:pk>/software-images/",
         views.SoftwareSoftwareImagesLCMView.as_view(),
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/nautobot_device_lifecycle_mgmt/views.py` & `nautobot_device_lifecycle_mgmt-2.1.1/nautobot_device_lifecycle_mgmt/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,67 +6,215 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 from django.conf import settings
 from django.db.models import Count, ExpressionWrapper, F, FloatField, Q
 from django_tables2 import RequestConfig
 from matplotlib.ticker import MaxNLocator
+from nautobot.apps.views import NautobotUIViewSet
+from nautobot.core.forms.search import SearchForm
 from nautobot.core.views import generic
 from nautobot.core.views.mixins import ContentTypePermissionRequiredMixin
 from nautobot.core.views.paginator import EnhancedPaginator, get_paginate_count
+from nautobot.dcim.models import Device
 
-from nautobot_device_lifecycle_mgmt import choices
-from nautobot_device_lifecycle_mgmt.filters import (
-    DeviceSoftwareValidationResultFilterSet,
-    InventoryItemSoftwareValidationResultFilterSet,
-)
-from nautobot_device_lifecycle_mgmt.forms import (
-    DeviceSoftwareValidationResultFilterForm,
-    InventoryItemSoftwareValidationResultFilterForm,
-)
-from nautobot_device_lifecycle_mgmt.models import (
-    DeviceSoftwareValidationResult,
-    InventoryItemSoftwareValidationResult,
-    SoftwareImageLCM,
-    SoftwareLCM,
-)
-from nautobot_device_lifecycle_mgmt.tables import (
-    DeviceSoftwareValidationResultListTable,
-    DeviceSoftwareValidationResultTable,
-    InventoryItemSoftwareValidationResultListTable,
-    InventoryItemSoftwareValidationResultTable,
-    SoftwareImageLCMTable,
-)
+from nautobot_device_lifecycle_mgmt import choices, filters, forms, models, tables
+from nautobot_device_lifecycle_mgmt.api import serializers
 from nautobot_device_lifecycle_mgmt.utils import count_related_m2m
 
 PLUGIN_CFG = settings.PLUGINS_CONFIG["nautobot_device_lifecycle_mgmt"]
 
 logger = logging.getLogger("nautobot_device_lifecycle_mgmt")
 
 # ---------------------------------------------------------------------------------
 #  Hardware Lifecycle Management Views
 # ---------------------------------------------------------------------------------
 GREEN, RED, GREY = ("#D5E8D4", "#F8CECC", "#808080")
 
 
+class HardwareLCMUIViewSet(NautobotUIViewSet):
+    """HardwareLCM UI ViewSet."""
+
+    bulk_update_form_class = forms.HardwareLCMBulkEditForm
+    filterset_class = filters.HardwareLCMFilterSet
+    filterset_form_class = forms.HardwareLCMFilterForm
+    form_class = forms.HardwareLCMForm
+    queryset = models.HardwareLCM.objects.prefetch_related("device_type")
+    serializer_class = serializers.HardwareLCMSerializer
+    table_class = tables.HardwareLCMTable
+
+    def get_extra_context(self, request, instance):  # pylint: disable=signature-differs
+        """Return any additional context data for the template.
+
+        request: The current request
+        instance: The object being viewed
+        """
+        if not instance:
+            return {}
+        if instance.device_type:
+            return {"devices": Device.objects.restrict(request.user, "view").filter(device_type=instance.device_type)}
+        if instance.inventory_item:
+            return {
+                "devices": Device.objects.restrict(request.user, "view").filter(
+                    inventory_items__part_id=instance.inventory_item
+                )
+            }
+        return {"devices": []}
+
+
+class SoftwareLCMUIViewSet(NautobotUIViewSet):
+    """SoftwareLCM UI ViewSet."""
+
+    # TODO: Add bulk edit form
+    # bulk_update_form_class = forms.SoftwareLCMBulkEditForm
+    filterset_class = filters.SoftwareLCMFilterSet
+    filterset_form_class = forms.SoftwareLCMFilterForm
+    form_class = forms.SoftwareLCMForm
+    queryset = models.SoftwareLCM.objects.prefetch_related("device_platform")
+    serializer_class = serializers.SoftwareLCMSerializer
+    table_class = tables.SoftwareLCMTable
+
+    def get_extra_context(self, request, instance):  # pylint: disable=signature-differs
+        """Changes "Softwares" => "Software"."""
+        search_form = SearchForm(data=self.request.GET)
+
+        return {
+            "search_form": search_form,
+            "title": "Software",
+            "verbose_name_plural": "Software",
+        }
+
+
+class SoftwareImageLCMUIViewSet(NautobotUIViewSet):
+    """SoftwareImageLCM UI ViewSet."""
+
+    # TODO: Add bulk edit form
+    # bulk_update_form_class = forms.SoftwareImageLCMBulkEditForm
+    filterset_class = filters.SoftwareImageLCMFilterSet
+    filterset_form_class = forms.SoftwareImageLCMFilterForm
+    form_class = forms.SoftwareImageLCMForm
+    queryset = models.SoftwareImageLCM.objects.all()
+    serializer_class = serializers.SoftwareImageLCMSerializer
+    table_class = tables.SoftwareImageLCMTable
+
+
+class ValidatedSoftwareLCMUIViewSet(NautobotUIViewSet):
+    """ValidatedSoftwareLCM UI ViewSet."""
+
+    # TODO: Add bulk edit form
+    # bulk_update_form_class = forms.ValidatedSoftwareLCMBulkEditForm
+    filterset_class = filters.ValidatedSoftwareLCMFilterSet
+    filterset_form_class = forms.ValidatedSoftwareLCMFilterForm
+    form_class = forms.ValidatedSoftwareLCMForm
+    queryset = models.ValidatedSoftwareLCM.objects.all()
+    serializer_class = serializers.ValidatedSoftwareLCMSerializer
+    table_class = tables.ValidatedSoftwareLCMTable
+
+
+class ContractLCMUIViewSet(NautobotUIViewSet):
+    """ContractLCM UI ViewSet."""
+
+    bulk_update_form_class = forms.ContractLCMBulkEditForm
+    filterset_class = filters.ContractLCMFilterSet
+    filterset_form_class = forms.ContractLCMFilterForm
+    form_class = forms.ContractLCMForm
+    queryset = models.ContractLCM.objects.all()
+    serializer_class = serializers.ContractLCMSerializer
+    table_class = tables.ContractLCMTable
+
+    def get_extra_context(self, request, instance):  # pylint: disable=signature-differs
+        """Return any additional context data for the template.
+
+        request: The current request
+        instance: The object being viewed
+        """
+        return {
+            "contacts": models.ContactLCM.objects.restrict(request.user, "view")
+            .filter(contract=instance)
+            .exclude(type="Owner")
+            .order_by("type", "priority"),
+            "owners": models.ContactLCM.objects.restrict(request.user, "view")
+            .filter(contract=instance, type="Owner")
+            .order_by("type", "priority"),
+        }
+
+
+class ProviderLCMUIViewSet(NautobotUIViewSet):
+    """ProviderLCM UI ViewSet."""
+
+    bulk_update_form_class = forms.ProviderLCMBulkEditForm
+    filterset_class = filters.ProviderLCMFilterSet
+    filterset_form_class = forms.ProviderLCMFilterForm
+    form_class = forms.ProviderLCMForm
+    queryset = models.ProviderLCM.objects.all()
+    serializer_class = serializers.ProviderLCMSerializer
+    table_class = tables.ProviderLCMTable
+
+    def get_extra_context(self, request, instance):  # pylint: disable=signature-differs
+        """Return any additional context data for the template.
+
+        request: The current request
+        instance: The object being viewed
+        """
+        return {"contracts": models.ContractLCM.objects.restrict(request.user, "view").filter(provider=instance)}
+
+
+class ContactLCMUIViewSet(NautobotUIViewSet):
+    """ContactLCM UI ViewSet."""
+
+    bulk_update_form_class = forms.ContactLCMBulkEditForm
+    filterset_class = filters.ContactLCMFilterSet
+    filterset_form_class = forms.ContactLCMFilterForm
+    form_class = forms.ContactLCMForm
+    queryset = models.ContactLCM.objects.all()
+    serializer_class = serializers.ContactLCMSerializer
+    table_class = tables.ContactLCMTable
+
+
+class CVELCMUIViewSet(NautobotUIViewSet):
+    """CVELCM UI ViewSet."""
+
+    bulk_update_form_class = forms.CVELCMBulkEditForm
+    filterset_class = filters.CVELCMFilterSet
+    filterset_form_class = forms.CVELCMFilterForm
+    form_class = forms.CVELCMForm
+    queryset = models.CVELCM.objects.all()
+    serializer_class = serializers.CVELCMSerializer
+    table_class = tables.CVELCMTable
+
+
+class VulnerabilityLCMUIViewSet(NautobotUIViewSet):
+    """VulnerabilityLCM UI ViewSet."""
+
+    bulk_update_form_class = forms.VulnerabilityLCMBulkEditForm
+    filterset_class = filters.VulnerabilityLCMFilterSet
+    filterset_form_class = forms.VulnerabilityLCMFilterForm
+    form_class = forms.VulnerabilityLCMForm
+    queryset = models.VulnerabilityLCM.objects.all()
+    serializer_class = serializers.VulnerabilityLCMSerializer
+    table_class = tables.VulnerabilityLCMTable
+
+
 class SoftwareSoftwareImagesLCMView(generic.ObjectView):
     """Software Images tab for Software view."""
 
-    queryset = SoftwareLCM.objects.all()
+    queryset = models.SoftwareLCM.objects.all()
     template_name = "nautobot_device_lifecycle_mgmt/softwarelcm_software_images.html"
 
     def get_extra_context(self, request, instance):
         """Adds Software Images table."""
         softwareimages = (
-            instance.software_images.annotate(device_type_count=count_related_m2m(SoftwareImageLCM, "device_types"))
-            .annotate(object_tag_count=count_related_m2m(SoftwareImageLCM, "object_tags"))
+            instance.software_images.annotate(
+                device_type_count=count_related_m2m(models.SoftwareImageLCM, "device_types")
+            )
+            .annotate(object_tag_count=count_related_m2m(models.SoftwareImageLCM, "object_tags"))
             .restrict(request.user, "view")
         )
 
-        softwareimages_table = SoftwareImageLCMTable(data=softwareimages, user=request.user, orderable=False)
+        softwareimages_table = tables.SoftwareImageLCMTable(data=softwareimages, user=request.user, orderable=False)
 
         paginate = {
             "paginator_class": EnhancedPaginator,
             "per_page": get_paginate_count(request),
         }
         RequestConfig(request, paginate).configure(softwareimages_table)
 
@@ -203,20 +351,20 @@
             aggr["valid_percent"] = 0
         return aggr
 
 
 class ValidatedSoftwareDeviceReportView(generic.ObjectListView):
     """View for executive report on software Validation."""
 
-    filterset = DeviceSoftwareValidationResultFilterSet
-    filterset_form = DeviceSoftwareValidationResultFilterForm
-    table = DeviceSoftwareValidationResultTable
+    filterset = filters.DeviceSoftwareValidationResultFilterSet
+    filterset_form = forms.DeviceSoftwareValidationResultFilterForm
+    table = tables.DeviceSoftwareValidationResultTable
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftware_device_report.html"
     queryset = (
-        DeviceSoftwareValidationResult.objects.values("device__device_type__model", "device__device_type__pk")
+        models.DeviceSoftwareValidationResult.objects.values("device__device_type__model", "device__device_type__pk")
         .distinct()
         .annotate(
             total=Count("device__device_type__model"),
             valid=Count("device__device_type__model", filter=Q(is_validated=True)),
             invalid=Count("device__device_type__model", filter=Q(is_validated=False) & ~Q(software=None)),
             no_software=Count("device__device_type__model", filter=Q(software=None)),
             valid_percent=ExpressionWrapper(100 * F("valid") / (F("total")), output_field=FloatField()),
@@ -228,24 +376,26 @@
     extra_content = {}
 
     def setup(self, request, *args, **kwargs):
         """Using request object to perform filtering based on query params."""
         super().setup(request, *args, **kwargs)  #
         try:
             report_last_run = (
-                DeviceSoftwareValidationResult.objects.filter(run_type=choices.ReportRunTypeChoices.REPORT_FULL_RUN)
+                models.DeviceSoftwareValidationResult.objects.filter(
+                    run_type=choices.ReportRunTypeChoices.REPORT_FULL_RUN
+                )
                 .latest("last_updated")
                 .last_run
             )
-        except DeviceSoftwareValidationResult.DoesNotExist:  # pylint: disable=no-member
+        except models.DeviceSoftwareValidationResult.DoesNotExist:  # pylint: disable=no-member
             report_last_run = None
 
         device_aggr = self.get_global_aggr(request)
         _platform_qs = (
-            DeviceSoftwareValidationResult.objects.values("device__platform__name")
+            models.DeviceSoftwareValidationResult.objects.values("device__platform__name")
             .distinct()
             .annotate(
                 total=Count("device__platform__name"),
                 valid=Count("device__platform__name", filter=Q(is_validated=True)),
                 invalid=Count("device__platform__name", filter=Q(is_validated=False) & ~Q(software=None)),
                 no_software=Count("device__platform__name", filter=Q(software=None)),
             )
@@ -275,15 +425,15 @@
 
     def get_global_aggr(self, request):
         """Get device and inventory global reports.
 
         Returns:
             device_aggr: device global report dict
         """
-        device_qs = DeviceSoftwareValidationResult.objects
+        device_qs = models.DeviceSoftwareValidationResult.objects
 
         device_aggr = {}
         if self.filterset is not None:
             device_aggr = self.filterset(request.GET, device_qs).qs.aggregate(
                 total=Count("device"),
                 valid=Count("device", filter=Q(is_validated=True)),
                 invalid=Count("device", filter=Q(is_validated=False) & ~Q(software=None)),
@@ -335,31 +485,31 @@
 
         return "\n".join(csv_data)
 
 
 class DeviceSoftwareValidationResultListView(generic.ObjectListView):
     """DeviceSoftawareValidationResult List view."""
 
-    queryset = DeviceSoftwareValidationResult.objects.all()
-    filterset = DeviceSoftwareValidationResultFilterSet
-    filterset_form = DeviceSoftwareValidationResultFilterForm
-    table = DeviceSoftwareValidationResultListTable
+    queryset = models.DeviceSoftwareValidationResult.objects.all()
+    filterset = filters.DeviceSoftwareValidationResultFilterSet
+    filterset_form = forms.DeviceSoftwareValidationResultFilterForm
+    table = tables.DeviceSoftwareValidationResultListTable
     action_buttons = ("export",)
     template_name = "nautobot_device_lifecycle_mgmt/devicesoftwarevalidationresult_list.html"
 
 
 class ValidatedSoftwareInventoryItemReportView(generic.ObjectListView):
     """View for executive report on inventory item software validation."""
 
-    filterset = InventoryItemSoftwareValidationResultFilterSet
-    filterset_form = InventoryItemSoftwareValidationResultFilterForm
-    table = InventoryItemSoftwareValidationResultTable
+    filterset = filters.InventoryItemSoftwareValidationResultFilterSet
+    filterset_form = forms.InventoryItemSoftwareValidationResultFilterForm
+    table = tables.InventoryItemSoftwareValidationResultTable
     template_name = "nautobot_device_lifecycle_mgmt/validatedsoftware_inventoryitem_report.html"
     queryset = (
-        InventoryItemSoftwareValidationResult.objects.values(
+        models.InventoryItemSoftwareValidationResult.objects.values(
             "inventory_item__part_id",
             "inventory_item__name",
             "inventory_item__pk",
             "inventory_item__device__name",
             "inventory_item__device__pk",
         )
         .distinct()
@@ -377,26 +527,26 @@
     extra_content = {}
 
     def setup(self, request, *args, **kwargs):
         """Using request object to perform filtering based on query params."""
         super().setup(request, *args, **kwargs)
         try:
             report_last_run = (
-                InventoryItemSoftwareValidationResult.objects.filter(
+                models.InventoryItemSoftwareValidationResult.objects.filter(
                     run_type=choices.ReportRunTypeChoices.REPORT_FULL_RUN
                 )
                 .latest("last_updated")
                 .last_run
             )
-        except InventoryItemSoftwareValidationResult.DoesNotExist:  # pylint: disable=no-member
+        except models.InventoryItemSoftwareValidationResult.DoesNotExist:  # pylint: disable=no-member
             report_last_run = None
 
         inventory_aggr = self.get_global_aggr(request)
         _platform_qs = (
-            InventoryItemSoftwareValidationResult.objects.values("inventory_item__manufacturer__name")
+            models.InventoryItemSoftwareValidationResult.objects.values("inventory_item__manufacturer__name")
             .distinct()
             .annotate(
                 total=Count("inventory_item__manufacturer__name"),
                 valid=Count("inventory_item__manufacturer__name", filter=Q(is_validated=True)),
                 invalid=Count("inventory_item__manufacturer__name", filter=Q(is_validated=False) & ~Q(software=None)),
                 no_software=Count("inventory_item__manufacturer__name", filter=Q(software=None)),
             )
@@ -428,15 +578,15 @@
 
     def get_global_aggr(self, request):
         """Get device and inventory global reports.
 
         Returns:
             inventory_aggr: inventory item global report dict
         """
-        inventory_item_qs = InventoryItemSoftwareValidationResult.objects
+        inventory_item_qs = models.InventoryItemSoftwareValidationResult.objects
 
         inventory_aggr = {}
         if self.filterset is not None:
             inventory_aggr = self.filterset(request.GET, inventory_item_qs).qs.aggregate(
                 total=Count("inventory_item"),
                 valid=Count("inventory_item", filter=Q(is_validated=True)),
                 invalid=Count("inventory_item", filter=Q(is_validated=False) & ~Q(software=None)),
@@ -495,13 +645,13 @@
 
         return "\n".join(csv_data)
 
 
 class InventoryItemSoftwareValidationResultListView(generic.ObjectListView):
     """InvenotryItemSoftawareValidationResult List view."""
 
-    queryset = InventoryItemSoftwareValidationResult.objects.all()
-    filterset = InventoryItemSoftwareValidationResultFilterSet
-    filterset_form = InventoryItemSoftwareValidationResultFilterForm
-    table = InventoryItemSoftwareValidationResultListTable
+    queryset = models.InventoryItemSoftwareValidationResult.objects.all()
+    filterset = filters.InventoryItemSoftwareValidationResultFilterSet
+    filterset_form = forms.InventoryItemSoftwareValidationResultFilterForm
+    table = tables.InventoryItemSoftwareValidationResultListTable
     action_buttons = ("export",)
     template_name = "nautobot_device_lifecycle_mgmt/inventoryitemsoftwarevalidationresult_list.html"
```

### Comparing `nautobot_device_lifecycle_mgmt-2.1.0/PKG-INFO` & `nautobot_device_lifecycle_mgmt-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: nautobot-device-lifecycle-mgmt
-Version: 2.1.0
+Version: 2.1.1
 Summary: Manages device lifecycles for platforms and software.
 Home-page: https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt
 License: Apache-2.0
-Keywords: nautobot,nautobot-plugin
+Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
 Requires-Dist: matplotlib (>=3.3.4,<4.0.0)
 Requires-Dist: nautobot (>=2.0.0,<3.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
+Project-URL: Documentation, https://docs.nautobot.com/projects/device-lifecycle/en/latest/
 Project-URL: Repository, https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt
 Description-Content-Type: text/markdown
 
 # Device Lifecycle Management
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-device-lifecycle-mgmt/develop/docs/images/icon-DeviceLifecycle.png" class="logo" height="200px">
   <br>
   <a href="https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt/actions"><img src="https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/device-lifecycle/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-device-lifecycle-mgmt/badge/"></a>
+  <a href="https://docs.nautobot.com/projects/device-lifecycle/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-nautobot-device-lifecycle-mgmt/badge/"></a>
   <a href="https://pypi.org/project/nautobot-device-lifecycle-mgmt/"><img src="https://img.shields.io/pypi/v/nautobot-device-lifecycle-mgmt"></a>
   <a href="https://pypi.org/project/nautobot-device-lifecycle-mgmt/"><img src="https://img.shields.io/pypi/dm/nautobot-device-lifecycle-mgmt"></a>
   <br>
   An App for <a href="https://github.com/nautobot/nautobot">Nautobot</a>.
 </p>
 
 ## Overview
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 2.1.0
+Metadata-Version: 2.1 Name: nautobot-device-lifecycle-mgmt Version: 2.1.1
 Summary: Manages device lifecycles for platforms and software. Home-page:
 https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt License: Apache-
-2.0 Keywords: nautobot,nautobot-plugin Author: Network to Code, LLC Author-
-email: info@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
+2.0 Keywords: nautobot,nautobot-app,nautobot-plugin Author: Network to Code,
+LLC Author-email: info@networktocode.com Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: matplotlib (>=3.3.4,<4.0.0) Requires-
-Dist: nautobot (>=2.0.0,<3.0.0) Requires-Dist: pycountry (>=22.3.5,<23.0.0)
-Project-URL: Repository, https://github.com/nautobot/nautobot-app-device-
-lifecycle-mgmt Description-Content-Type: text/markdown # Device Lifecycle
-Management
+Language :: Python :: 3.11 Provides-Extra: all Requires-Dist: matplotlib
+(>=3.3.4,<4.0.0) Requires-Dist: nautobot (>=2.0.0,<3.0.0) Requires-Dist:
+pycountry (>=22.3.5,<23.0.0) Project-URL: Documentation, https://
+docs.nautobot.com/projects/device-lifecycle/en/latest/ Project-URL: Repository,
+https://github.com/nautobot/nautobot-app-device-lifecycle-mgmt Description-
+Content-Type: text/markdown # Device Lifecycle Management
 [https://raw.githubusercontent.com/nautobot/nautobot-app-device-lifecycle-mgmt/
                  develop/docs/images/icon-DeviceLifecycle.png]
    _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_a_c_t_i_o_n_s_/
    _w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/
-   _n_a_u_t_o_b_o_t_-_a_p_p_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
-_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-
-                                _l_i_f_e_c_y_c_l_e_-_m_g_m_t_]
+_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-
+                            _d_e_v_i_c_e_-_l_i_f_e_c_y_c_l_e_-_m_g_m_t_]
                              An App for _N_a_u_t_o_b_o_t.
 ## Overview An app for [Nautobot](https://github.com/nautobot/nautobot) to
 manage device lifecycles. This app works by making related associations to
 Devices, Device Types, and Inventory Items to help provide data about the
 hardware end of life notices, appropriate software versions to be running on
 the devices, and the maintenance contracts associated with devices. This will
 help with the various aspects of planning Lifecycle events, and provides quick
```

