# Comparing `tmp/shimoku-2.3.0.tar.gz` & `tmp/shimoku-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimoku-2.3.0.tar", last modified: Mon Apr  8 15:57:03 2024, max compression
+gzip compressed data, was "shimoku-2.3.1.tar", last modified: Tue Apr  9 08:02:16 2024, max compression
```

## Comparing `shimoku-2.3.0.tar` & `shimoku-2.3.1.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.118333 shimoku-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 15:56:48.000000 shimoku-2.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.066332 shimoku-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 15:56:48.000000 shimoku-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 15:56:48.000000 shimoku-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 15:56:48.000000 shimoku-2.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 15:56:48.000000 shimoku-2.3.0/.github/workflows/publish-testpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-08 15:56:48.000000 shimoku-2.3.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 15:56:48.000000 shimoku-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 15:56:48.000000 shimoku-2.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-08 15:56:48.000000 shimoku-2.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-08 15:56:48.000000 shimoku-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 15:56:48.000000 shimoku-2.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 15:56:48.000000 shimoku-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-08 15:57:03.118333 shimoku-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-08 15:56:48.000000 shimoku-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 15:56:48.000000 shimoku-2.3.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 15:56:48.000000 shimoku-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 15:56:48.000000 shimoku-2.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-08 15:56:48.000000 shimoku-2.3.0/scripts/user_classes_header_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-08 15:57:03.118333 shimoku-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-08 15:56:48.000000 shimoku-2.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 15:56:48.000000 shimoku-2.3.0/setup_browser.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.062332 shimoku-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/src/shimoku/
--rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/src/shimoku/actions_execution/
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/actions_execution/execute_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/actions_execution/front_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/src/shimoku/ai/
--rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/ai/ai_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.070332 shimoku-2.3.0/src/shimoku/ai/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/ai/generated_headers/AILayerHeader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.074332 shimoku-2.3.0/src/shimoku/api/
--rw-r--r--   0 runner    (1001) docker     (127)    30469 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/base_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.074332 shimoku-2.3.0/src/shimoku/api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/action_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/activity_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/business_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.074332 shimoku-2.3.0/src/shimoku/api/resources/reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.078332 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/annotated_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/echart.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/charts/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/filter_data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/tabs_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/reports/unsupported.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/resources/universe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.078332 shimoku-2.3.0/src/shimoku/api/user_access_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/actions_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/activities_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/activity_templates_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/apps_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/businesses_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/dashboards_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/data_sets_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/files_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.082332 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/reports_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/user_access_classes/universes_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/async_execution_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.082332 shimoku-2.3.0/src/shimoku/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/cli/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/cascade_get_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/cloud_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.086332 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/file_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/main_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/tree_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/code_gen/utils_code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/execution_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.090332 shimoku-2.3.0/src/shimoku/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/playground/execute_local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/playground/local_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/playground/schema_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/playground/schema_parameter_classses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/playground/websockets_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.090332 shimoku-2.3.0/src/shimoku/plt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.094333 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/default_echart_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/line_and_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/top_bottom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/EChart_definitions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/bentobox_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.094333 shimoku-2.3.0/src/shimoku/plt/generated_headers/
--rw-r--r--   0 runner    (1001) docker     (127)    37704 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)    88204 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/plt_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/plt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-08 15:56:48.000000 shimoku-2.3.0/src/shimoku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.118333 shimoku-2.3.0/src/shimoku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:57:02.000000 shimoku-2.3.0/src/shimoku.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 15:57:03.000000 shimoku-2.3.0/src/shimoku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.094333 shimoku-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/Jupyter_notebook_test.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.098333 shimoku-2.3.0/tests/mockable_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.098333 shimoku-2.3.0/tests/mockable_tests/correct_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/correct_action_scripts/correct_action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.102332 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_rename_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/needs_action_function.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/needs_import_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_activity_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_app_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_business_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_dashboard_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.110333 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/area.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/bentobox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:03.118333 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/doughnut.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/free_echarts.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/infographics.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/input_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/line.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/marked_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/modal.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/pie.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/predictive_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rose.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/summary_line.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/sunburst.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/treemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/waterfall.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_report_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/mockable_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/test_ai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/test_components_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/test_data_managing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/test_file_metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 15:56:48.000000 shimoku-2.3.0/tests/test_universe_metadata_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.319191 shimoku-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-09 08:02:04.000000 shimoku-2.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.271191 shimoku-2.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.271191 shimoku-2.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 08:02:04.000000 shimoku-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 08:02:04.000000 shimoku-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 08:02:04.000000 shimoku-2.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.271191 shimoku-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 08:02:04.000000 shimoku-2.3.1/.github/workflows/publish-testpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-09 08:02:04.000000 shimoku-2.3.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 08:02:04.000000 shimoku-2.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 08:02:04.000000 shimoku-2.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-09 08:02:04.000000 shimoku-2.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 08:02:04.000000 shimoku-2.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-09 08:02:04.000000 shimoku-2.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 08:02:04.000000 shimoku-2.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 08:02:16.319191 shimoku-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-09 08:02:04.000000 shimoku-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-09 08:02:04.000000 shimoku-2.3.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 08:02:04.000000 shimoku-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 08:02:04.000000 shimoku-2.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.271191 shimoku-2.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-09 08:02:04.000000 shimoku-2.3.1/scripts/user_classes_header_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 08:02:16.319191 shimoku-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 08:02:04.000000 shimoku-2.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 08:02:04.000000 shimoku-2.3.1/setup_browser.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.267191 shimoku-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.275191 shimoku-2.3.1/src/shimoku/
+-rw-r--r--   0 runner    (1001) docker     (127)    17476 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.275191 shimoku-2.3.1/src/shimoku/actions_execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/actions_execution/execute_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/actions_execution/front_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.275191 shimoku-2.3.1/src/shimoku/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)    33016 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/ai/ai_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.275191 shimoku-2.3.1/src/shimoku/ai/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/ai/generated_headers/AILayerHeader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.275191 shimoku-2.3.1/src/shimoku/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    30469 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/base_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19697 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.279191 shimoku-2.3.1/src/shimoku/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/action_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/activity_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/business_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.279191 shimoku-2.3.1/src/shimoku/api/resources/reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.279191 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/annotated_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/charts/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/filter_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/tabs_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/reports/unsupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/resources/universe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.283191 shimoku-2.3.1/src/shimoku/api/user_access_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/actions_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/activities_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/activity_templates_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/apps_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/businesses_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/dashboards_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/data_sets_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/files_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.283191 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/reports_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/user_access_classes/universes_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20693 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/async_execution_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/cli/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/cascade_get_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32158 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/cloud_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.287191 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.291191 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.291191 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/file_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/main_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/tree_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/code_gen/utils_code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/execution_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.291191 shimoku-2.3.1/src/shimoku/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/playground/execute_local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35031 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/playground/local_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40234 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/playground/schema_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/playground/schema_parameter_classses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/playground/websockets_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.295191 shimoku-2.3.1/src/shimoku/plt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.295191 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/default_echart_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20924 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/line_and_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/shimoku_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/top_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/EChart_definitions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/bentobox_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.295191 shimoku-2.3.1/src/shimoku/plt/generated_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)    37818 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/generated_headers/PlotLayerHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88351 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/plt_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/plt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-09 08:02:04.000000 shimoku-2.3.1/src/shimoku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.319191 shimoku-2.3.1/src/shimoku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:02:15.000000 shimoku-2.3.1/src/shimoku.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 08:02:16.000000 shimoku-2.3.1/src/shimoku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.299191 shimoku-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/Jupyter_notebook_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.299191 shimoku-2.3.1/tests/mockable_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.299191 shimoku-2.3.1/tests/mockable_tests/correct_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/correct_action_scripts/correct_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.303191 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/action_cant_have_no_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/action_param_must_be_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_annotate_client_param_to_arb_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_client_to_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_assign_to_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_action_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_define_more_than_one_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_arb_params_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_client_as_part_of_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_have_non_annotated_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_import_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_import_from_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_pass_incorrect_type_to_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_rename_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/cant_return_shimoku_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/needs_action_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/needs_import_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/error_action_scripts/shimoku_client_param_must_be_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_activity_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_app_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_business_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_dashboard_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.311191 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/bentobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:02:16.319191 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bentobox_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129464 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/random_waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/segmented_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/suburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/test_stack_distribution.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/zero_centered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/doughnut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/free_echarts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/free_echarts_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/get_input_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator_color_by_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/infographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/input_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/marked_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/pie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/predictive_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter_with_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/speed_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/stacked_horizontal_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/summary_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/sunburst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/table_with_lables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/waterfall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_report_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/mockable_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/test_ai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/test_components_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/test_data_managing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/test_file_metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 08:02:04.000000 shimoku-2.3.1/tests/test_universe_metadata_api.py
```

### Comparing `shimoku-2.3.0/.coveragerc` & `shimoku-2.3.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `shimoku-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `shimoku-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.github/pull_request_template.md` & `shimoku-2.3.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.github/workflows/publish-testpypi.yml` & `shimoku-2.3.1/.github/workflows/publish-testpypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.github/workflows/publish-to-pypi.yml` & `shimoku-2.3.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/.gitignore` & `shimoku-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/CHANGELOG.md` & `shimoku-2.3.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 2.3.1 (2024-09-04)
+
+- Fixed CORS error when deleting resources with Actions
+
 ## 2.3.0 (2024-08-04)
 
 - User accounts handling through the SDK
 
 ## 2.2.3 (2024-05-04)
 
 -  Fixed CORS error with the API from the execution of the Actions
```

### Comparing `shimoku-2.3.0/CODE_OF_CONDUCT.md` & `shimoku-2.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/CONTRIBUTING.md` & `shimoku-2.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/LICENSE.txt` & `shimoku-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/PKG-INFO` & `shimoku-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku
-Version: 2.3.0
+Version: 2.3.1
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-2.3.0/README.md` & `shimoku-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/SECURITY.md` & `shimoku-2.3.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/scripts/user_classes_header_generator.py` & `shimoku-2.3.1/scripts/user_classes_header_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/setup.cfg` & `shimoku-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/setup.py` & `shimoku-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/setup_browser.cfg` & `shimoku-2.3.1/setup_browser.cfg`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/__init__.py` & `shimoku-2.3.1/src/shimoku/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/actions_execution/execute_action.py` & `shimoku-2.3.1/src/shimoku/actions_execution/execute_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/actions_execution/front_connection.py` & `shimoku-2.3.1/src/shimoku/actions_execution/front_connection.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/ai/ai_layer.py` & `shimoku-2.3.1/src/shimoku/ai/ai_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/ai/generated_headers/AILayerHeader.py` & `shimoku-2.3.1/src/shimoku/ai/generated_headers/AILayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/base_resource.py` & `shimoku-2.3.1/src/shimoku/api/base_resource.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/client.py` & `shimoku-2.3.1/src/shimoku/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 headers=headers,
                 body=body
                 if isinstance(body, bytes)
                 else json.dumps(body).encode("utf-8"),
                 timeout=self.timeout,
                 params=query_params,
             )
-            if method == "GET":
+            if not body:
                 del params["body"]
             res = await pyfetch(url, **params)
             if (
                 hasattr(res, "headers")
                 and "application/json" in res.headers.get("content-type")
             ) or ((hasattr(res, "json")) and not hasattr(res, "read")):
                 data = await res.json()
```

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/action.py` & `shimoku-2.3.1/src/shimoku/api/resources/action.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/action_template.py` & `shimoku-2.3.1/src/shimoku/api/resources/action_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/activity.py` & `shimoku-2.3.1/src/shimoku/api/resources/activity.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/activity_template.py` & `shimoku-2.3.1/src/shimoku/api/resources/activity_template.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/app.py` & `shimoku-2.3.1/src/shimoku/api/resources/app.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/business.py` & `shimoku-2.3.1/src/shimoku/api/resources/business.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/business_user.py` & `shimoku-2.3.1/src/shimoku/api/resources/business_user.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/dashboard.py` & `shimoku-2.3.1/src/shimoku/api/resources/dashboard.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/data_set.py` & `shimoku-2.3.1/src/shimoku/api/resources/data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/event.py` & `shimoku-2.3.1/src/shimoku/api/resources/event.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/file.py` & `shimoku-2.3.1/src/shimoku/api/resources/file.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/report.py` & `shimoku-2.3.1/src/shimoku/api/resources/report.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/reports/charts/indicator.py` & `shimoku-2.3.1/src/shimoku/api/resources/reports/charts/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/reports/charts/table.py` & `shimoku-2.3.1/src/shimoku/api/resources/reports/charts/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/reports/filter_data_set.py` & `shimoku-2.3.1/src/shimoku/api/resources/reports/filter_data_set.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/reports/modal.py` & `shimoku-2.3.1/src/shimoku/api/resources/reports/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/reports/tabs_group.py` & `shimoku-2.3.1/src/shimoku/api/resources/reports/tabs_group.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/role.py` & `shimoku-2.3.1/src/shimoku/api/resources/role.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/resources/universe.py` & `shimoku-2.3.1/src/shimoku/api/resources/universe.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/actions_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/actions_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/activities_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/activities_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/activity_templates_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/activity_templates_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/apps_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/apps_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/businesses_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/businesses_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/dashboards_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/dashboards_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/data_sets_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/data_sets_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/files_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/files_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActionsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivitiesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ActivityTemplatesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/BoardsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/ComponentsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/DataSetsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/FilesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/MenuPathsLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/UniversesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/generated_headers/WorkspacesLayerHeader.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/reports_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/reports_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/user_access_classes/universes_layer.py` & `shimoku-2.3.1/src/shimoku/api/user_access_classes/universes_layer.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/api/utils.py` & `shimoku-2.3.1/src/shimoku/api/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/async_execution_pool.py` & `shimoku-2.3.1/src/shimoku/async_execution_pool.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/__init__.py` & `shimoku-2.3.1/src/shimoku/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/cascade_get_resources.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/cascade_get_resources.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/create.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/create.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/delete.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/delete.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/execute.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/execute.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/get.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/get.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/list.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/list.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud/update.py` & `shimoku-2.3.1/src/shimoku/cli/cloud/update.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/cloud_parser.py` & `shimoku-2.3.1/src/shimoku/cli/cloud_parser.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/configuration.py` & `shimoku-2.3.1/src/shimoku/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/listen.py` & `shimoku-2.3.1/src/shimoku/cli/listen.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/main.py` & `shimoku-2.3.1/src/shimoku/cli/main.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/persistence.py` & `shimoku-2.3.1/src/shimoku/cli/persistence.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/playground.py` & `shimoku-2.3.1/src/shimoku/cli/playground.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/cli/utils.py` & `shimoku-2.3.1/src/shimoku/cli/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/code_gen_from_apps.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/data_sets_code_gen/code_gen_from_data_sets.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/code_gen_from_reports.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_annotated_echart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_button.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_filter.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_html.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_iframe.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_other.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_table.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/apps_code_gen/reports_code_gen/report_types_code_gen/code_gen_from_tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py` & `shimoku-2.3.1/src/shimoku/code_gen/business_code_gen/code_gen_from_business.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/file_generator.py` & `shimoku-2.3.1/src/shimoku/code_gen/file_generator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/main_code_gen.py` & `shimoku-2.3.1/src/shimoku/code_gen/main_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/tree_generation.py` & `shimoku-2.3.1/src/shimoku/code_gen/tree_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/code_gen/utils_code_gen.py` & `shimoku-2.3.1/src/shimoku/code_gen/utils_code_gen.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/exceptions.py` & `shimoku-2.3.1/src/shimoku/exceptions.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/execution_logger.py` & `shimoku-2.3.1/src/shimoku/execution_logger.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/playground/execute_local_server.py` & `shimoku-2.3.1/src/shimoku/playground/execute_local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/playground/local_server.py` & `shimoku-2.3.1/src/shimoku/playground/local_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/playground/schema_classes.py` & `shimoku-2.3.1/src/shimoku/playground/schema_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/playground/schema_parameter_classses.py` & `shimoku-2.3.1/src/shimoku/playground/schema_parameter_classses.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/playground/websockets_server.py` & `shimoku-2.3.1/src/shimoku/playground/websockets_server.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/bar.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/default_echart_options.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/default_echart_options.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/funnel.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/funnel.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/gauge.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/gauge_indicator.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/heatmap.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/line.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/line.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/line_and_bar.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/line_and_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/pie.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/pie.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/radar.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/sankey.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/sankey.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/scatter.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/shimoku_gauge.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/shimoku_gauge.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/sunburst.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/sunburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/top_bottom.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/top_bottom.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/tree.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/treemap.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/treemap.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/EChart_definitions/waterfall.py` & `shimoku-2.3.1/src/shimoku/plt/EChart_definitions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/bentobox_charts.py` & `shimoku-2.3.1/src/shimoku/plt/bentobox_charts.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/plt/generated_headers/PlotLayerHeader.py` & `shimoku-2.3.1/src/shimoku/plt/generated_headers/PlotLayerHeader.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,14 +321,15 @@
         next_group_label: Optional[str] = "Next",
         rows_size: Optional[int] = 3,
         cols_size: int = 12,
         padding: Optional[str] = None,
         modal: Optional[str] = None,
         activity_id: Optional[str] = None,
         activity_name: Optional[str] = None,
+        action_id: Optional[str] = None,
         on_submit_events: Optional[list[dict]] = None,
     ):
         """Easier way to create an input form.
         :param menu_path: the menu path of the input form
         :param order: the order of the input form
         :param form_groups: the form groups of the input form
         :param dynamic_sequential_show: whether to show the next group after submitting the current group
@@ -336,14 +337,15 @@
         :param next_group_label: the label of the next group button
         :param rows_size: the rows size of the input form
         :param cols_size: the columns size of the input form
         :param padding: the padding of the input form
         :param modal: the modal to open after submitting the form
         :param activity_id: the activity id to run after submitting the form
         :param activity_name: the activity name to run after submitting the form
+        :param action_id: the action id to run after submitting the form
         :param on_submit_events: the events to run after submitting the form
         """
         pass
 
     def get_component_by_order(
         self,
         order: int,
```

### Comparing `shimoku-2.3.0/src/shimoku/plt/plt_layer.py` & `shimoku-2.3.1/src/shimoku/plt/plt_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3912,1602 +3912,1611 @@
 0000f470: 6d6f 6461 6c3a 204f 7074 696f 6e61 6c5b  modal: Optional[
 0000f480: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
 0000f490: 2020 2020 2061 6374 6976 6974 795f 6964       activity_id
 0000f4a0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
 0000f4b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
 0000f4c0: 6163 7469 7669 7479 5f6e 616d 653a 204f  activity_name: O
 0000f4d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000f4e0: 6f6e 652c 0a20 2020 2020 2020 206f 6e5f  one,.        on_
-0000f4f0: 7375 626d 6974 5f65 7665 6e74 733a 204f  submit_events: O
-0000f500: 7074 696f 6e61 6c5b 6c69 7374 5b64 6963  ptional[list[dic
-0000f510: 745d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  t]] = None,.    
-0000f520: 293a 0a20 2020 2020 2020 2022 2222 4561  ):.        """Ea
-0000f530: 7369 6572 2077 6179 2074 6f20 6372 6561  sier way to crea
-0000f540: 7465 2061 6e20 696e 7075 7420 666f 726d  te an input form
-0000f550: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000f560: 206d 656e 755f 7061 7468 3a20 7468 6520   menu_path: the 
-0000f570: 6d65 6e75 2070 6174 6820 6f66 2074 6865  menu path of the
-0000f580: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000f590: 2020 2020 3a70 6172 616d 206f 7264 6572      :param order
-0000f5a0: 3a20 7468 6520 6f72 6465 7220 6f66 2074  : the order of t
-0000f5b0: 6865 2069 6e70 7574 2066 6f72 6d0a 2020  he input form.  
-0000f5c0: 2020 2020 2020 3a70 6172 616d 2066 6f72        :param for
-0000f5d0: 6d5f 6772 6f75 7073 3a20 7468 6520 666f  m_groups: the fo
-0000f5e0: 726d 2067 726f 7570 7320 6f66 2074 6865  rm groups of the
-0000f5f0: 2069 6e70 7574 2066 6f72 6d0a 2020 2020   input form.    
-0000f600: 2020 2020 3a70 6172 616d 2064 796e 616d      :param dynam
-0000f610: 6963 5f73 6571 7565 6e74 6961 6c5f 7368  ic_sequential_sh
-0000f620: 6f77 3a20 7768 6574 6865 7220 746f 2073  ow: whether to s
-0000f630: 686f 7720 7468 6520 6e65 7874 2067 726f  how the next gro
-0000f640: 7570 2061 6674 6572 2073 7562 6d69 7474  up after submitt
-0000f650: 696e 6720 7468 6520 6375 7272 656e 7420  ing the current 
-0000f660: 6772 6f75 700a 2020 2020 2020 2020 3a70  group.        :p
-0000f670: 6172 616d 2061 7574 6f5f 7365 6e64 3a20  aram auto_send: 
-0000f680: 7768 6574 6865 7220 746f 2061 7574 6f6d  whether to autom
-0000f690: 6174 6963 616c 6c79 2073 656e 6420 7468  atically send th
-0000f6a0: 6520 666f 726d 2061 6674 6572 2074 6865  e form after the
-0000f6b0: 206c 6173 7420 6772 6f75 700a 2020 2020   last group.    
-0000f6c0: 2020 2020 3a70 6172 616d 206e 6578 745f      :param next_
-0000f6d0: 6772 6f75 705f 6c61 6265 6c3a 2074 6865  group_label: the
-0000f6e0: 206c 6162 656c 206f 6620 7468 6520 6e65   label of the ne
-0000f6f0: 7874 2067 726f 7570 2062 7574 746f 6e0a  xt group button.
-0000f700: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-0000f710: 6f77 735f 7369 7a65 3a20 7468 6520 726f  ows_size: the ro
-0000f720: 7773 2073 697a 6520 6f66 2074 6865 2069  ws size of the i
-0000f730: 6e70 7574 2066 6f72 6d0a 2020 2020 2020  nput form.      
-0000f740: 2020 3a70 6172 616d 2063 6f6c 735f 7369    :param cols_si
-0000f750: 7a65 3a20 7468 6520 636f 6c75 6d6e 7320  ze: the columns 
-0000f760: 7369 7a65 206f 6620 7468 6520 696e 7075  size of the inpu
-0000f770: 7420 666f 726d 0a20 2020 2020 2020 203a  t form.        :
-0000f780: 7061 7261 6d20 7061 6464 696e 673a 2074  param padding: t
-0000f790: 6865 2070 6164 6469 6e67 206f 6620 7468  he padding of th
-0000f7a0: 6520 696e 7075 7420 666f 726d 0a20 2020  e input form.   
-0000f7b0: 2020 2020 203a 7061 7261 6d20 6d6f 6461       :param moda
-0000f7c0: 6c3a 2074 6865 206d 6f64 616c 2074 6f20  l: the modal to 
-0000f7d0: 6f70 656e 2061 6674 6572 2073 7562 6d69  open after submi
-0000f7e0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
-0000f7f0: 2020 2020 2020 203a 7061 7261 6d20 6163         :param ac
-0000f800: 7469 7669 7479 5f69 643a 2074 6865 2061  tivity_id: the a
-0000f810: 6374 6976 6974 7920 6964 2074 6f20 7275  ctivity id to ru
-0000f820: 6e20 6166 7465 7220 7375 626d 6974 7469  n after submitti
-0000f830: 6e67 2074 6865 2066 6f72 6d0a 2020 2020  ng the form.    
-0000f840: 2020 2020 3a70 6172 616d 2061 6374 6976      :param activ
-0000f850: 6974 795f 6e61 6d65 3a20 7468 6520 6163  ity_name: the ac
-0000f860: 7469 7669 7479 206e 616d 6520 746f 2072  tivity name to r
-0000f870: 756e 2061 6674 6572 2073 7562 6d69 7474  un after submitt
-0000f880: 696e 6720 7468 6520 666f 726d 0a20 2020  ing the form.   
-0000f890: 2020 2020 203a 7061 7261 6d20 6f6e 5f73       :param on_s
-0000f8a0: 7562 6d69 745f 6576 656e 7473 3a20 7468  ubmit_events: th
-0000f8b0: 6520 6576 656e 7473 2074 6f20 7275 6e20  e events to run 
-0000f8c0: 6166 7465 7220 7375 626d 6974 7469 6e67  after submitting
-0000f8d0: 2074 6865 2066 6f72 6d0a 2020 2020 2020   the form.      
-0000f8e0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000f8f0: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
-0000f900: 6f70 6572 7469 6573 203d 207b 2266 6965  operties = {"fie
-0000f910: 6c64 7322 3a20 5b5d 7d0a 2020 2020 2020  lds": []}.      
-0000f920: 2020 6966 2061 7574 6f5f 7365 6e64 3a0a    if auto_send:.
-0000f930: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-0000f940: 7274 5f64 6174 615f 7365 745f 7072 6f70  rt_data_set_prop
-0000f950: 6572 7469 6573 5b22 7661 7269 616e 7422  erties["variant"
-0000f960: 5d20 3d20 2261 7574 6f53 656e 6422 0a0a  ] = "autoSend"..
-0000f970: 2020 2020 2020 2020 725f 6861 7368 203d          r_hash =
-0000f980: 2073 656c 662e 5f67 6574 5f63 6861 7274   self._get_chart
-0000f990: 5f68 6173 6828 6f72 6465 7229 0a0a 2020  _hash(order)..  
-0000f9a0: 2020 2020 2020 6e65 7874 5f69 6420 3d20        next_id = 
-0000f9b0: 6622 7b72 5f68 6173 687d 5f30 2220 6966  f"{r_hash}_0" if
-0000f9c0: 2064 796e 616d 6963 5f73 6571 7565 6e74   dynamic_sequent
-0000f9d0: 6961 6c5f 7368 6f77 2065 6c73 6520 4e6f  ial_show else No
-0000f9e0: 6e65 0a0a 2020 2020 2020 2020 6e65 7874  ne..        next
-0000f9f0: 5f67 726f 7570 5f69 6e64 6578 203d 2031  _group_index = 1
-0000fa00: 0a20 2020 2020 2020 2066 6f72 2066 6f72  .        for for
-0000fa10: 6d5f 6772 6f75 705f 6e61 6d65 2c20 666f  m_group_name, fo
-0000fa20: 726d 5f67 726f 7570 2069 6e20 666f 726d  rm_group in form
-0000fa30: 5f67 726f 7570 732e 6974 656d 7328 293a  _groups.items():
-0000fa40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000fa50: 6d5f 6772 6f75 705f 6a73 6f6e 203d 207b  m_group_json = {
-0000fa60: 2274 6974 6c65 223a 2066 6f72 6d5f 6772  "title": form_gr
-0000fa70: 6f75 705f 6e61 6d65 2c20 2266 6965 6c64  oup_name, "field
-0000fa80: 7322 3a20 666f 726d 5f67 726f 7570 7d0a  s": form_group}.
-0000fa90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000faa0: 6578 745f 6964 3a0a 2020 2020 2020 2020  ext_id:.        
-0000fab0: 2020 2020 2020 2020 666f 726d 5f67 726f          form_gro
-0000fac0: 7570 5f6a 736f 6e5b 2269 6422 5d20 3d20  up_json["id"] = 
-0000fad0: 6e65 7874 5f69 640a 2020 2020 2020 2020  next_id.        
-0000fae0: 2020 2020 2020 2020 6e65 7874 5f69 6420          next_id 
-0000faf0: 3d20 6622 7b72 5f68 6173 687d 5f7b 6e65  = f"{r_hash}_{ne
-0000fb00: 7874 5f67 726f 7570 5f69 6e64 6578 7d22  xt_group_index}"
-0000fb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb20: 2066 6f72 6d5f 6772 6f75 705f 6a73 6f6e   form_group_json
-0000fb30: 5b22 6e65 7874 466f 726d 4772 6f75 7022  ["nextFormGroup"
-0000fb40: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-0000fb50: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-0000fb60: 6e65 7874 5f69 642c 0a20 2020 2020 2020  next_id,.       
-0000fb70: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-0000fb80: 6265 6c22 3a20 6e65 7874 5f67 726f 7570  bel": next_group
-0000fb90: 5f6c 6162 656c 2c0a 2020 2020 2020 2020  _label,.        
-0000fba0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0000fbb0: 2020 2020 2020 2020 2020 6e65 7874 5f67            next_g
-0000fbc0: 726f 7570 5f69 6e64 6578 202b 3d20 310a  roup_index += 1.
-0000fbd0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
-0000fbe0: 7274 5f64 6174 615f 7365 745f 7072 6f70  rt_data_set_prop
-0000fbf0: 6572 7469 6573 5b22 6669 656c 6473 225d  erties["fields"]
-0000fc00: 202b 3d20 5b66 6f72 6d5f 6772 6f75 705f   += [form_group_
-0000fc10: 6a73 6f6e 5d0a 0a20 2020 2020 2020 2069  json]..        i
-0000fc20: 6620 6e65 7874 5f69 643a 0a20 2020 2020  f next_id:.     
-0000fc30: 2020 2020 2020 2064 656c 2072 6570 6f72         del repor
-0000fc40: 745f 6461 7461 5f73 6574 5f70 726f 7065  t_data_set_prope
-0000fc50: 7274 6965 735b 2266 6965 6c64 7322 5d5b  rties["fields"][
-0000fc60: 2d31 5d5b 226e 6578 7446 6f72 6d47 726f  -1]["nextFormGro
-0000fc70: 7570 225d 0a0a 2020 2020 2020 2020 7365  up"]..        se
-0000fc80: 6c66 2e69 6e70 7574 5f66 6f72 6d28 0a20  lf.input_form(. 
-0000fc90: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-0000fca0: 6e73 3d72 6570 6f72 745f 6461 7461 5f73  ns=report_data_s
-0000fcb0: 6574 5f70 726f 7065 7274 6965 732c 0a20  et_properties,. 
-0000fcc0: 2020 2020 2020 2020 2020 206f 7264 6572             order
-0000fcd0: 3d6f 7264 6572 2c0a 2020 2020 2020 2020  =order,.        
-0000fce0: 2020 2020 726f 7773 5f73 697a 653d 726f      rows_size=ro
-0000fcf0: 7773 5f73 697a 652c 0a20 2020 2020 2020  ws_size,.       
-0000fd00: 2020 2020 2063 6f6c 735f 7369 7a65 3d63       cols_size=c
-0000fd10: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
-0000fd20: 2020 2020 2020 7061 6464 696e 673d 7061        padding=pa
-0000fd30: 6464 696e 672c 0a20 2020 2020 2020 2020  dding,.         
-0000fd40: 2020 206d 6f64 616c 3d6d 6f64 616c 2c0a     modal=modal,.
-0000fd50: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-0000fd60: 7669 7479 5f69 643d 6163 7469 7669 7479  vity_id=activity
-0000fd70: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-0000fd80: 2061 6374 6976 6974 795f 6e61 6d65 3d61   activity_name=a
-0000fd90: 6374 6976 6974 795f 6e61 6d65 2c0a 2020  ctivity_name,.  
-0000fda0: 2020 2020 2020 2020 2020 6f6e 5f73 7562            on_sub
-0000fdb0: 6d69 745f 6576 656e 7473 3d6f 6e5f 7375  mit_events=on_su
-0000fdc0: 626d 6974 5f65 7665 6e74 732c 0a20 2020  bmit_events,.   
-0000fdd0: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
-0000fde0: 6320 6465 6620 5f67 6574 5f69 6e70 7574  c def _get_input
-0000fdf0: 5f66 6f72 6d5f 6461 7461 2873 656c 662c  _form_data(self,
-0000fe00: 2069 6e70 7574 5f66 6f72 6d3a 2049 6e70   input_form: Inp
-0000fe10: 7574 466f 726d 2920 2d3e 2064 6963 743a  utForm) -> dict:
-0000fe20: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
-0000fe30: 7468 6520 696e 7075 7420 666f 726d 2064  the input form d
-0000fe40: 6174 612e 2222 220a 2020 2020 2020 2020  ata.""".        
-0000fe50: 7265 706f 7274 5f64 6174 615f 7365 7420  report_data_set 
-0000fe60: 3d20 2861 7761 6974 2069 6e70 7574 5f66  = (await input_f
-0000fe70: 6f72 6d2e 6765 745f 7265 706f 7274 5f64  orm.get_report_d
-0000fe80: 6174 615f 7365 7473 2829 295b 305d 0a20  ata_sets())[0]. 
-0000fe90: 2020 2020 2020 2064 6174 615f 7365 7420         data_set 
-0000fea0: 3d20 6177 6169 7420 7365 6c66 2e5f 6170  = await self._ap
-0000feb0: 702e 6765 745f 6461 7461 5f73 6574 2872  p.get_data_set(r
-0000fec0: 6570 6f72 745f 6461 7461 5f73 6574 5b22  eport_data_set["
-0000fed0: 6461 7461 5365 7449 6422 5d29 0a20 2020  dataSetId"]).   
-0000fee0: 2020 2020 2064 6174 615f 706f 696e 7420       data_point 
-0000fef0: 3d20 6177 6169 7420 6461 7461 5f73 6574  = await data_set
-0000ff00: 2e67 6574 5f6f 6e65 5f64 6174 615f 706f  .get_one_data_po
-0000ff10: 696e 7428 290a 2020 2020 2020 2020 6c6f  int().        lo
-0000ff20: 6767 6572 2e69 6e66 6f28 6622 476f 7420  gger.info(f"Got 
-0000ff30: 696e 7075 7420 666f 726d 2064 6174 6120  input form data 
-0000ff40: 666f 7220 7b73 7472 2869 6e70 7574 5f66  for {str(input_f
-0000ff50: 6f72 6d29 7d22 290a 2020 2020 2020 2020  orm)}").        
-0000ff60: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-0000ff70: 2020 2020 2022 7265 706f 7274 4964 223a       "reportId":
-0000ff80: 2069 6e70 7574 5f66 6f72 6d5b 2269 6422   input_form["id"
-0000ff90: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-0000ffa0: 6f72 6465 7222 3a20 696e 7075 745f 666f  order": input_fo
-0000ffb0: 726d 5b22 6f72 6465 7222 5d2c 0a20 2020  rm["order"],.   
-0000ffc0: 2020 2020 2020 2020 2022 6461 7461 223a           "data":
-0000ffd0: 2064 6174 615f 706f 696e 745b 2263 7573   data_point["cus
-0000ffe0: 746f 6d46 6965 6c64 3122 5d20 6966 2064  tomField1"] if d
-0000fff0: 6174 615f 706f 696e 7420 656c 7365 204e  ata_point else N
-00010000: 6f6e 652c 0a20 2020 2020 2020 207d 0a0a  one,.        }..
-00010010: 2020 2020 6173 796e 6320 6465 6620 6765      async def ge
-00010020: 745f 696e 7075 745f 666f 726d 7328 7365  t_input_forms(se
-00010030: 6c66 2920 2d3e 206c 6973 745b 6469 6374  lf) -> list[dict
-00010040: 5d3a 0a20 2020 2020 2020 2022 2222 4765  ]:.        """Ge
-00010050: 7420 616c 6c20 7468 6520 696e 7075 7420  t all the input 
-00010060: 666f 726d 7320 696e 2074 6865 2063 7572  forms in the cur
-00010070: 7265 6e74 206d 656e 755f 7061 7468 2e22  rent menu_path."
-00010080: 2222 0a20 2020 2020 2020 2072 6570 6f72  "".        repor
-00010090: 7473 3a20 6c69 7374 203d 205b 0a20 2020  ts: list = [.   
-000100a0: 2020 2020 2020 2020 2072 6570 6f72 740a           report.
-000100b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000100c0: 7265 706f 7274 2069 6e20 6177 6169 7420  report in await 
-000100d0: 7365 6c66 2e5f 6170 702e 6765 745f 7265  self._app.get_re
-000100e0: 706f 7274 7328 290a 2020 2020 2020 2020  ports().        
-000100f0: 2020 2020 6966 2072 6570 6f72 745b 2272      if report["r
-00010100: 6570 6f72 7454 7970 6522 5d20 3d3d 2022  eportType"] == "
-00010110: 464f 524d 220a 2020 2020 2020 2020 2020  FORM".          
-00010120: 2020 616e 6420 2872 6570 6f72 745b 2270    and (report["p
-00010130: 6174 6822 5d20 3d3d 2073 656c 662e 5f63  ath"] == self._c
-00010140: 7572 7265 6e74 5f70 6174 6820 6f72 206e  urrent_path or n
-00010150: 6f74 2073 656c 662e 5f63 7572 7265 6e74  ot self._current
-00010160: 5f70 6174 6829 0a20 2020 2020 2020 205d  _path).        ]
-00010170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010180: 6c69 7374 280a 2020 2020 2020 2020 2020  list(.          
-00010190: 2020 6177 6169 7420 6173 796e 6369 6f2e    await asyncio.
-000101a0: 6761 7468 6572 280a 2020 2020 2020 2020  gather(.        
-000101b0: 2020 2020 2020 2020 2a5b 7365 6c66 2e5f          *[self._
-000101c0: 6765 745f 696e 7075 745f 666f 726d 5f64  get_input_form_d
-000101d0: 6174 6128 7265 706f 7274 2920 666f 7220  ata(report) for 
-000101e0: 7265 706f 7274 2069 6e20 7265 706f 7274  report in report
-000101f0: 735d 0a20 2020 2020 2020 2020 2020 2029  s].            )
-00010200: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00010210: 4061 6464 5f74 6f5f 6765 6e65 7261 6c5f  @add_to_general_
-00010220: 6173 796e 635f 6772 6f75 700a 2020 2020  async_group.    
-00010230: 6173 796e 6320 6465 6620 616e 6e6f 7461  async def annota
-00010240: 7465 645f 6368 6172 7428 0a20 2020 2020  ted_chart(.     
-00010250: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00010260: 2064 6174 613a 2055 6e69 6f6e 5b6c 6973   data: Union[lis
-00010270: 745b 4461 7461 4672 616d 655d 2c20 6c69  t[DataFrame], li
-00010280: 7374 5b6c 6973 745b 6469 6374 5d5d 5d2c  st[list[dict]]],
-00010290: 0a20 2020 2020 2020 206f 7264 6572 3a20  .        order: 
-000102a0: 696e 742c 0a20 2020 2020 2020 2078 3a20  int,.        x: 
-000102b0: 7374 722c 0a20 2020 2020 2020 2079 3a20  str,.        y: 
-000102c0: 556e 696f 6e5b 7374 722c 206c 6973 745b  Union[str, list[
-000102d0: 7374 725d 5d2c 0a20 2020 2020 2020 2061  str]],.        a
-000102e0: 6e6e 6f74 6174 696f 6e73 3a20 7374 7220  nnotations: str 
-000102f0: 3d20 2261 6e6e 6f74 6174 696f 6e22 2c0a  = "annotation",.
-00010300: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
-00010310: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
-00010320: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00010330: 2063 6f6c 735f 7369 7a65 3a20 4f70 7469   cols_size: Opti
-00010340: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00010350: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
-00010360: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
-00010370: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00010380: 2074 6974 6c65 3a20 4f70 7469 6f6e 616c   title: Optional
-00010390: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-000103a0: 2020 2020 2020 795f 6178 6973 5f6e 616d        y_axis_nam
-000103b0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-000103c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000103d0: 2073 6c69 6465 725f 636f 6e66 6967 3a20   slider_config: 
-000103e0: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
-000103f0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00010400: 6c69 6465 725f 6d61 726b 733a 204f 7074  lider_marks: Opt
-00010410: 696f 6e61 6c5b 6c69 7374 5b74 7570 6c65  ional[list[tuple
-00010420: 5d5d 203d 204e 6f6e 652c 0a20 2020 2029  ]] = None,.    )
-00010430: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00010440: 2020 2020 2020 4372 6561 7465 2061 6e20        Create an 
-00010450: 616e 6e6f 7461 7465 6420 6368 6172 7420  annotated chart 
-00010460: 696e 2074 6865 206d 656e 7520 7061 7468  in the menu path
-00010470: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00010480: 2064 6174 613a 2074 6865 2064 6174 6120   data: the data 
-00010490: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-000104a0: 2020 2020 203a 7061 7261 6d20 6f72 6465       :param orde
-000104b0: 723a 2074 6865 206f 7264 6572 206f 6620  r: the order of 
-000104c0: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
-000104d0: 2020 3a70 6172 616d 2078 3a20 7468 6520    :param x: the 
-000104e0: 7820 6178 6973 0a20 2020 2020 2020 203a  x axis.        :
-000104f0: 7061 7261 6d20 793a 2074 6865 2079 2061  param y: the y a
-00010500: 7869 730a 2020 2020 2020 2020 3a70 6172  xis.        :par
-00010510: 616d 2061 6e6e 6f74 6174 696f 6e73 3a20  am annotations: 
-00010520: 7468 6520 616e 6e6f 7461 7469 6f6e 730a  the annotations.
-00010530: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-00010540: 6f77 735f 7369 7a65 3a20 7468 6520 726f  ows_size: the ro
-00010550: 7773 2073 697a 6520 6f66 2074 6865 2063  ws size of the c
-00010560: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
-00010570: 7261 6d20 636f 6c73 5f73 697a 653a 2074  ram cols_size: t
-00010580: 6865 2063 6f6c 756d 6e73 2073 697a 6520  he columns size 
-00010590: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
-000105a0: 2020 2020 203a 7061 7261 6d20 7061 6464       :param padd
-000105b0: 696e 673a 2074 6865 2070 6164 6469 6e67  ing: the padding
-000105c0: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
-000105d0: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
-000105e0: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
-000105f0: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-00010600: 2020 203a 7061 7261 6d20 795f 6178 6973     :param y_axis
-00010610: 5f6e 616d 653a 2074 6865 206e 616d 6520  _name: the name 
-00010620: 6f66 2074 6865 2079 2061 7869 730a 2020  of the y axis.  
-00010630: 2020 2020 2020 3a70 6172 616d 2073 6c69        :param sli
-00010640: 6465 725f 636f 6e66 6967 3a20 7468 6520  der_config: the 
-00010650: 736c 6964 6572 2063 6f6e 6669 670a 2020  slider config.  
-00010660: 2020 2020 2020 3a70 6172 616d 2073 6c69        :param sli
-00010670: 6465 725f 6d61 726b 733a 2074 6865 2073  der_marks: the s
-00010680: 6c69 6465 7220 6d61 726b 730a 2020 2020  lider marks.    
-00010690: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000106a0: 6966 2069 7369 6e73 7461 6e63 6528 6461  if isinstance(da
-000106b0: 7461 2c20 7374 7229 3a0a 2020 2020 2020  ta, str):.      
-000106c0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-000106d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106e0: 206c 6f67 6765 722c 0a20 2020 2020 2020   logger,.       
-000106f0: 2020 2020 2020 2020 2022 416e 6e6f 7461           "Annota
-00010700: 7465 6420 6368 6172 7420 646f 6573 206e  ted chart does n
-00010710: 6f74 2073 7570 706f 7274 2074 6865 2075  ot support the u
-00010720: 7365 206f 6620 7368 6172 6564 2064 6174  se of shared dat
-00010730: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
-00010740: 2020 2020 4461 7461 4572 726f 722c 0a20      DataError,. 
-00010750: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00010760: 2020 2020 2020 6966 2073 6c69 6465 725f        if slider_
-00010770: 636f 6e66 6967 2069 7320 4e6f 6e65 3a0a  config is None:.
-00010780: 2020 2020 2020 2020 2020 2020 736c 6964              slid
-00010790: 6572 5f63 6f6e 6669 6720 3d20 7b7d 0a0a  er_config = {}..
-000107a0: 2020 2020 2020 2020 6966 2073 6c69 6465          if slide
-000107b0: 725f 6d61 726b 733a 0a20 2020 2020 2020  r_marks:.       
-000107c0: 2020 2020 2073 6c69 6465 725f 636f 6e66       slider_conf
-000107d0: 6967 5b22 6d61 726b 7322 5d20 3d20 5b0a  ig["marks"] = [.
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 7b22 6c61 6265 6c22 3a20 6d61 726b 5b30  {"label": mark[0
-00010800: 5d2c 2022 7661 6c75 6522 3a20 6d61 726b  ], "value": mark
-00010810: 5b31 5d7d 2066 6f72 206d 6172 6b20 696e  [1]} for mark in
-00010820: 2073 6c69 6465 725f 6d61 726b 730a 2020   slider_marks.  
-00010830: 2020 2020 2020 2020 2020 5d0a 0a20 2020            ]..   
-00010840: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00010850: 6365 2879 2c20 7374 7229 3a0a 2020 2020  ce(y, str):.    
-00010860: 2020 2020 2020 2020 7920 3d20 5b79 5d0a          y = [y].
-00010870: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00010880: 6c65 6e28 7929 203d 3d20 6c65 6e28 6461  len(y) == len(da
-00010890: 7461 293a 0a20 2020 2020 2020 2020 2020  ta):.           
-000108a0: 206c 6f67 5f65 7272 6f72 280a 2020 2020   log_error(.    
-000108b0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000108c0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000108d0: 2020 2020 6622 4e75 6d62 6572 206f 6620      f"Number of 
-000108e0: 7920 7661 6c75 6573 2028 7b6c 656e 2879  y values ({len(y
-000108f0: 297d 2920 646f 6573 206e 6f74 206d 6174  )}) does not mat
-00010900: 6368 206e 756d 6265 7220 6f66 2064 6174  ch number of dat
-00010910: 6166 7261 6d65 7320 287b 6c65 6e28 6461  aframes ({len(da
-00010920: 7461 297d 2922 2c0a 2020 2020 2020 2020  ta)})",.        
-00010930: 2020 2020 2020 2020 4461 7461 4572 726f          DataErro
-00010940: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
-00010950: 0a0a 2020 2020 2020 2020 5f2c 2072 6570  ..        _, rep
-00010960: 6f72 7420 3d20 6177 6169 7420 7365 6c66  ort = await self
-00010970: 2e5f 6765 745f 6368 6172 745f 7265 706f  ._get_chart_repo
-00010980: 7274 286f 7264 6572 2c20 416e 6e6f 7461  rt(order, Annota
-00010990: 7465 6445 4368 6172 7429 0a0a 2020 2020  tedEChart)..    
-000109a0: 2020 2020 6466 7320 3d20 5b76 616c 6964      dfs = [valid
-000109b0: 6174 655f 6461 7461 5f69 735f 7061 6e64  ate_data_is_pand
-000109c0: 6172 6162 6c65 2864 6629 2066 6f72 2064  arable(df) for d
-000109d0: 6620 696e 2064 6174 615d 0a20 2020 2020  f in data].     
-000109e0: 2020 2064 6174 615f 7365 745f 7461 736b     data_set_task
-000109f0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-00010a00: 6f72 2064 662c 2079 5f76 616c 2069 6e20  or df, y_val in 
-00010a10: 7a69 7028 6466 732c 2079 293a 0a20 2020  zip(dfs, y):.   
-00010a20: 2020 2020 2020 2020 2064 665b 785d 203d           df[x] =
-00010a30: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
-00010a40: 6466 5b78 5d29 0a20 2020 2020 2020 2020  df[x]).         
-00010a50: 2020 2069 6620 616e 6e6f 7461 7469 6f6e     if annotation
-00010a60: 7320 696e 2064 663a 0a20 2020 2020 2020  s in df:.       
-00010a70: 2020 2020 2020 2020 2064 665b 616e 6e6f           df[anno
-00010a80: 7461 7469 6f6e 735d 203d 2028 0a20 2020  tations] = (.   
-00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010aa0: 2064 665b 616e 6e6f 7461 7469 6f6e 735d   df[annotations]
-00010ab0: 2e72 6570 6c61 6365 286e 702e 6e61 6e2c  .replace(np.nan,
-00010ac0: 2022 222c 2072 6567 6578 3d54 7275 6529   "", regex=True)
-00010ad0: 2e61 7374 7970 6528 7374 7229 0a20 2020  .astype(str).   
-00010ae0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00010af0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00010b00: 7365 745f 7461 736b 732e 6170 7065 6e64  set_tasks.append
-00010b10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010b20: 2020 7365 6c66 2e5f 6372 6561 7465 5f64    self._create_d
-00010b30: 6174 615f 7365 7428 6e61 6d65 3d66 227b  ata_set(name=f"{
-00010b40: 7265 706f 7274 5b27 6964 275d 7d5f 7b79  report['id']}_{y
-00010b50: 5f76 616c 7d22 2c20 6461 7461 3d64 6629  _val}", data=df)
-00010b60: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00010b70: 2020 2020 2020 2020 6461 7461 5f73 6574          data_set
-00010b80: 5f64 6963 7473 203d 2061 7761 6974 2061  _dicts = await a
-00010b90: 7379 6e63 696f 2e67 6174 6865 7228 2a64  syncio.gather(*d
-00010ba0: 6174 615f 7365 745f 7461 736b 7329 0a20  ata_set_tasks). 
-00010bb0: 2020 2020 2020 2064 6174 615f 7365 7473         data_sets
-00010bc0: 203d 205b 6473 5b79 5f76 616c 5d5b 315d   = [ds[y_val][1]
-00010bd0: 2066 6f72 2064 732c 2079 5f76 616c 2069   for ds, y_val i
-00010be0: 6e20 7a69 7028 6461 7461 5f73 6574 5f64  n zip(data_set_d
-00010bf0: 6963 7473 2c20 7929 5d0a 0a20 2020 2020  icts, y)]..     
-00010c00: 2020 2072 645f 6964 7320 3d20 4e6f 6e65     rd_ids = None
-00010c10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00010c20: 2e72 6575 7365 5f64 6174 615f 7365 7473  .reuse_data_sets
-00010c30: 3a0a 2020 2020 2020 2020 2020 2020 7264  :.            rd
-00010c40: 5f69 6473 203d 2067 6574 5f75 7569 6473  _ids = get_uuids
-00010c50: 5f66 726f 6d5f 6469 6374 2872 6570 6f72  _from_dict(repor
-00010c60: 745b 2270 726f 7065 7274 6965 7322 5d5b  t["properties"][
-00010c70: 226f 7074 696f 6e22 5d29 0a20 2020 2020  "option"]).     
-00010c80: 2020 2020 2020 2069 6620 6c65 6e28 7264         if len(rd
-00010c90: 5f69 6473 2920 3d3d 206c 656e 2879 293a  _ids) == len(y):
-00010ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010cb0: 2072 6570 5f64 733a 206c 6973 745b 5265   rep_ds: list[Re
-00010cc0: 706f 7274 2e52 6570 6f72 7444 6174 6153  port.ReportDataS
-00010cd0: 6574 5d20 3d20 6177 6169 7420 7265 706f  et] = await repo
-00010ce0: 7274 2e67 6574 5f72 6570 6f72 745f 6461  rt.get_report_da
-00010cf0: 7461 5f73 6574 7328 290a 2020 2020 2020  ta_sets().      
-00010d00: 2020 2020 2020 2020 2020 7265 705f 6473            rep_ds
-00010d10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00010d20: 2020 2020 2020 2020 206e 6578 7428 2872           next((r
-00010d30: 6420 666f 7220 7264 2069 6e20 7265 705f  d for rd in rep_
-00010d40: 6473 2069 6620 7264 5b22 6964 225d 203d  ds if rd["id"] =
-00010d50: 3d20 7264 5f69 6429 2c20 4e6f 6e65 290a  = rd_id), None).
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2020 2020 666f 7220 7264 5f69 6420 696e      for rd_id in
-00010d80: 2072 645f 6964 730a 2020 2020 2020 2020   rd_ids.        
-00010d90: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00010da0: 2020 2020 2020 2020 2020 6966 2061 6e79            if any
-00010db0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010dc0: 2020 2020 2020 7264 5b22 6461 7461 5365        rd["dataSe
-00010dd0: 7449 6422 5d20 213d 2064 735b 2269 6422  tId"] != ds["id"
-00010de0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00010df0: 2020 2020 2020 6f72 2072 645b 2270 726f        or rd["pro
-00010e00: 7065 7274 6965 7322 5d5b 226d 6170 7069  perties"]["mappi
-00010e10: 6e67 225d 0a20 2020 2020 2020 2020 2020  ng"].           
-00010e20: 2020 2020 2020 2020 2021 3d20 7b22 7661           != {"va
-00010e30: 6c75 6573 223a 205b 2264 6174 6546 6965  lues": ["dateFie
-00010e40: 6c64 3122 2c20 2269 6e74 4669 656c 6431  ld1", "intField1
-00010e50: 225d 2c20 226c 6162 656c 223a 2022 7374  "], "label": "st
-00010e60: 7269 6e67 4669 656c 6431 227d 0a20 2020  ringField1"}.   
-00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e80: 2066 6f72 2072 642c 2064 7320 696e 207a   for rd, ds in z
-00010e90: 6970 2872 6570 5f64 732c 2064 6174 615f  ip(rep_ds, data_
-00010ea0: 7365 7473 290a 2020 2020 2020 2020 2020  sets).          
-00010eb0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00010ec0: 2020 2020 2020 2020 2020 2020 2072 645f               rd_
-00010ed0: 6964 7320 3d20 4e6f 6e65 0a0a 2020 2020  ids = None..    
-00010ee0: 2020 2020 6966 206e 6f74 2072 645f 6964      if not rd_id
-00010ef0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00010f00: 7761 6974 2072 6570 6f72 742e 6465 6c65  wait report.dele
-00010f10: 7465 5f72 6570 6f72 745f 6461 7461 5f73  te_report_data_s
-00010f20: 6574 7328 6c6f 673d 5472 7565 290a 2020  ets(log=True).  
-00010f30: 2020 2020 2020 2020 2020 6d61 7070 696e            mappin
-00010f40: 673a 204d 6170 7069 6e67 203d 207b 0a20  g: Mapping = {. 
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010f60: 7661 6c75 6573 223a 205b 2264 6174 6546  values": ["dateF
-00010f70: 6965 6c64 3122 2c20 2269 6e74 4669 656c  ield1", "intFiel
-00010f80: 6431 225d 2c0a 2020 2020 2020 2020 2020  d1"],.          
-00010f90: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
-00010fa0: 7374 7269 6e67 4669 656c 6431 222c 0a20  stringField1",. 
-00010fb0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00010fc0: 2020 2020 2020 2020 2072 6570 6f72 745f           report_
-00010fd0: 6461 7461 5f73 6574 7320 3d20 6177 6169  data_sets = awai
-00010fe0: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
-00010ff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011000: 2020 2a5b 0a20 2020 2020 2020 2020 2020    *[.           
-00011010: 2020 2020 2020 2020 2072 6570 6f72 742e           report.
-00011020: 6372 6561 7465 5f72 6570 6f72 745f 6461  create_report_da
-00011030: 7461 5f73 6574 2828 6d61 7070 696e 672c  ta_set((mapping,
-00011040: 2064 6174 615f 7365 742c 204e 6f6e 6529   data_set, None)
-00011050: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011060: 2020 2020 2020 666f 7220 6461 7461 5f73        for data_s
-00011070: 6574 2069 6e20 6461 7461 5f73 6574 730a  et in data_sets.
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-000110a0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
-000110b0: 6473 203d 205b 7264 5b22 6964 225d 2066  ds = [rd["id"] f
-000110c0: 6f72 2072 6420 696e 2072 6570 6f72 745f  or rd in report_
-000110d0: 6461 7461 5f73 6574 735d 0a0a 2020 2020  data_sets]..    
-000110e0: 2020 2020 6368 6172 745f 6f70 7469 6f6e      chart_option
-000110f0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-00011100: 2020 2279 4178 6973 223a 207b 0a20 2020    "yAxis": {.   
-00011110: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-00011120: 6d65 223a 2079 5f61 7869 735f 6e61 6d65  me": y_axis_name
-00011130: 206f 7220 2222 2c0a 2020 2020 2020 2020   or "",.        
-00011140: 2020 2020 2020 2020 2266 6f6e 7422 2022          "font" "
-00011150: 7479 7065 223a 2022 7661 6c75 6522 2c0a  type": "value",.
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 226e 616d 654c 6f63 6174 696f 6e22 3a20  "nameLocation": 
-00011180: 226d 6964 646c 6522 2c0a 2020 2020 2020  "middle",.      
-00011190: 2020 2020 2020 2020 2020 226e 616d 6547            "nameG
-000111a0: 6170 223a 2033 302c 0a20 2020 2020 2020  ap": 30,.       
-000111b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000111c0: 2020 2020 2278 4178 6973 223a 207b 0a20      "xAxis": {. 
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000111e0: 7479 7065 223a 2022 7469 6d65 222c 0a20  type": "time",. 
-000111f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011200: 6e61 6d65 4c6f 6361 7469 6f6e 223a 2022  nameLocation": "
-00011210: 6d69 6464 6c65 222c 0a20 2020 2020 2020  middle",.       
-00011220: 2020 2020 2020 2020 2022 6e61 6d65 4761           "nameGa
-00011230: 7022 3a20 3330 2c0a 2020 2020 2020 2020  p": 30,.        
-00011240: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00011250: 2020 2022 7365 7269 6573 223a 205b 0a20     "series": [. 
-00011260: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00011270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011280: 2020 2020 2022 6461 7461 223a 2022 237b       "data": "#{
-00011290: 2220 2b20 7264 5f69 6420 2b20 227d 222c  " + rd_id + "}",
-000112a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112b0: 2020 2020 2022 7479 7065 223a 2022 6c69       "type": "li
-000112c0: 6e65 222c 0a20 2020 2020 2020 2020 2020  ne",.           
-000112d0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-000112e0: 2079 5f6e 616d 652c 0a20 2020 2020 2020   y_name,.       
-000112f0: 2020 2020 2020 2020 2020 2020 2022 6974               "it
-00011300: 656d 5374 796c 6522 3a20 7b0a 2020 2020  emStyle": {.    
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 2262 6f72 6465 7252 6164 6975      "borderRadiu
-00011330: 7322 3a20 5b39 2c20 392c 2030 2c20 305d  s": [9, 9, 0, 0]
-00011340: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011350: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00011360: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00011370: 2020 2020 2020 2020 2020 2066 6f72 2079             for y
-00011380: 5f6e 616d 652c 2072 645f 6964 2069 6e20  _name, rd_id in 
-00011390: 7a69 7028 792c 2072 645f 6964 7329 0a20  zip(y, rd_ids). 
-000113a0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-000113b0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000113c0: 6177 6169 7420 7365 6c66 2e5f 6372 6561  await self._crea
-000113d0: 7465 5f63 6861 7274 280a 2020 2020 2020  te_chart(.      
-000113e0: 2020 2020 2020 6368 6172 745f 636c 6173        chart_clas
-000113f0: 733d 416e 6e6f 7461 7465 6445 4368 6172  s=AnnotatedEChar
-00011400: 742c 0a20 2020 2020 2020 2020 2020 206f  t,.            o
-00011410: 7264 6572 3d6f 7264 6572 2c0a 2020 2020  rder=order,.    
-00011420: 2020 2020 2020 2020 7369 7a65 5061 6464          sizePadd
-00011430: 696e 673d 7061 6464 696e 672c 0a20 2020  ing=padding,.   
-00011440: 2020 2020 2020 2020 2073 697a 6552 6f77           sizeRow
-00011450: 733d 726f 7773 5f73 697a 652c 0a20 2020  s=rows_size,.   
-00011460: 2020 2020 2020 2020 2073 697a 6543 6f6c           sizeCol
-00011470: 756d 6e73 3d63 6f6c 735f 7369 7a65 2c0a  umns=cols_size,.
-00011480: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00011490: 653d 7469 746c 652c 0a20 2020 2020 2020  e=title,.       
-000114a0: 2020 2020 2070 726f 7065 7274 6965 733d       properties=
-000114b0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-000114c0: 2020 2020 2020 736c 6964 6572 3d73 6c69        slider=sli
-000114d0: 6465 725f 636f 6e66 6967 2c0a 2020 2020  der_config,.    
-000114e0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-000114f0: 6f6e 3d63 6861 7274 5f6f 7074 696f 6e73  on=chart_options
-00011500: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-00011510: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00011520: 6173 796e 6320 6465 6620 5f67 6574 5f72  async def _get_r
-00011530: 6570 6f72 745f 6461 7461 5f73 6574 735f  eport_data_sets_
-00011540: 7065 725f 6d61 7070 696e 6728 0a20 2020  per_mapping(.   
-00011550: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00011560: 2020 2072 6570 6f72 743a 2052 6570 6f72     report: Repor
-00011570: 742c 0a20 2020 2020 2020 2064 6174 615f  t,.        data_
-00011580: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-00011590: 3a20 6469 6374 2c0a 2020 2020 2020 2020  : dict,.        
-000115a0: 6669 656c 6473 3a20 6c69 7374 5b55 6e69  fields: list[Uni
-000115b0: 6f6e 5b74 7570 6c65 2c20 6469 6374 5d5d  on[tuple, dict]]
-000115c0: 2c0a 2020 2020 2920 2d3e 206c 6973 745b  ,.    ) -> list[
-000115d0: 5265 706f 7274 2e52 6570 6f72 7444 6174  Report.ReportDat
-000115e0: 6153 6574 5d3a 0a20 2020 2020 2020 2022  aSet]:.        "
-000115f0: 2222 4372 6561 7465 2061 2064 6174 615f  ""Create a data_
-00011600: 7365 7420 7065 7220 6669 656c 6420 6f66  set per field of
-00011610: 2061 2064 6174 6166 7261 6d65 2e0a 2020   a dataframe..  
-00011620: 2020 2020 2020 3a70 6172 616d 2072 6570        :param rep
-00011630: 6f72 743a 2074 6865 2072 6570 6f72 740a  ort: the report.
-00011640: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00011650: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00011660: 7570 6c65 3a20 7468 6520 6d61 7070 696e  uple: the mappin
-00011670: 6720 6f66 2074 6865 2064 6174 610a 2020  g of the data.  
-00011680: 2020 2020 2020 3a70 6172 616d 2066 6965        :param fie
-00011690: 6c64 733a 2074 6865 2066 6965 6c64 7320  lds: the fields 
-000116a0: 6f66 2074 6865 2064 6174 6120 746f 2062  of the data to b
-000116b0: 6520 7573 6564 0a20 2020 2020 2020 203a  e used.        :
-000116c0: 7265 7475 726e 3a20 7468 6520 6c69 7374  return: the list
-000116d0: 206f 6620 6461 7461 2073 6574 7320 7061   of data sets pa
-000116e0: 7274 6974 696f 6e65 6420 6279 2061 7869  rtitioned by axi
-000116f0: 7320 616e 6420 6669 656c 6473 0a20 2020  s and fields.   
-00011700: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011710: 2074 6173 6b73 203d 205b 5d0a 2020 2020   tasks = [].    
-00011720: 2020 2020 6669 656c 6473 203d 2066 6965      fields = fie
-00011730: 6c64 7320 6966 2066 6965 6c64 7320 656c  lds if fields el
-00011740: 7365 205b 5d0a 2020 2020 2020 2020 666f  se [].        fo
-00011750: 7220 692c 2066 2069 6e20 656e 756d 6572  r i, f in enumer
-00011760: 6174 6528 6669 656c 6473 293a 0a20 2020  ate(fields):.   
-00011770: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
-00011780: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00011790: 2020 6461 7461 5f73 6574 203d 204e 6f6e    data_set = Non
-000117a0: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
-000117b0: 735f 736f 7274 203d 204e 6f6e 650a 2020  s_sort = None.  
-000117c0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-000117d0: 6e73 7461 6e63 6528 662c 2073 7472 293a  nstance(f, str):
-000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000117f0: 2069 6620 6620 6e6f 7420 696e 2064 6174   if f not in dat
-00011800: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00011810: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00011820: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-00011830: 7228 6c6f 6767 6572 2c20 6622 4669 656c  r(logger, f"Fiel
-00011840: 6420 7b66 7d20 6e6f 7420 666f 756e 6420  d {f} not found 
-00011850: 696e 2064 6174 6122 2c20 4461 7461 4572  in data", DataEr
-00011860: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
-00011870: 2020 2020 206d 6170 7069 6e67 2c20 6461       mapping, da
-00011880: 7461 5f73 6574 2c20 7265 735f 736f 7274  ta_set, res_sort
-00011890: 203d 2064 6174 615f 6d61 7070 696e 675f   = data_mapping_
-000118a0: 746f 5f74 7570 6c65 5b66 5d0a 2020 2020  to_tuple[f].    
-000118b0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000118c0: 6e73 7461 6e63 6528 662c 2028 7475 706c  nstance(f, (tupl
-000118d0: 652c 206c 6973 7429 293a 0a20 2020 2020  e, list)):.     
-000118e0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-000118f0: 5f20 696e 2066 3a0a 2020 2020 2020 2020  _ in f:.        
-00011900: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00011910: 5f20 6e6f 7420 696e 2064 6174 615f 6d61  _ not in data_ma
-00011920: 7070 696e 675f 746f 5f74 7570 6c65 3a0a  pping_to_tuple:.
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2020 2020 6c6f 675f 6572 726f          log_erro
-00011950: 7228 6c6f 6767 6572 2c20 6622 4669 656c  r(logger, f"Fiel
-00011960: 6420 7b66 5f7d 206e 6f74 2066 6f75 6e64  d {f_} not found
-00011970: 2069 6e20 6461 7461 222c 2044 6174 6145   in data", DataE
-00011980: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00011990: 2020 2020 2020 2020 2020 6d61 7070 696e            mappin
-000119a0: 675f 2c20 6461 7461 5f73 6574 5f2c 2072  g_, data_set_, r
-000119b0: 6573 5f73 6f72 745f 203d 2064 6174 615f  es_sort_ = data_
-000119c0: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-000119d0: 5b66 5f5d 0a20 2020 2020 2020 2020 2020  [f_].           
-000119e0: 2020 2020 2020 2020 206d 6170 7069 6e67           mapping
-000119f0: 2e61 7070 656e 6428 6d61 7070 696e 675f  .append(mapping_
-00011a00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011a10: 2020 2020 2020 6461 7461 5f73 6574 203d        data_set =
-00011a20: 2064 6174 615f 7365 7420 6966 2064 6174   data_set if dat
-00011a30: 615f 7365 7420 656c 7365 2064 6174 615f  a_set else data_
-00011a40: 7365 745f 0a20 2020 2020 2020 2020 2020  set_.           
-00011a50: 2020 2020 2020 2020 2072 6573 5f73 6f72           res_sor
-00011a60: 7420 3d20 7265 735f 736f 7274 2069 6620  t = res_sort if 
-00011a70: 7265 735f 736f 7274 2065 6c73 6520 7265  res_sort else re
-00011a80: 735f 736f 7274 5f0a 2020 2020 2020 2020  s_sort_.        
-00011a90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00011aa0: 7274 2064 6174 615f 7365 7420 3d3d 2064  rt data_set == d
-00011ab0: 6174 615f 7365 745f 0a20 2020 2020 2020  ata_set_.       
-00011ac0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00011ad0: 6572 7420 7265 735f 736f 7274 203d 3d20  ert res_sort == 
-00011ae0: 7265 735f 736f 7274 5f0a 2020 2020 2020  res_sort_.      
-00011af0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00011b00: 7461 6e63 6528 662c 2064 6963 7429 3a0a  tance(f, dict):.
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 6d61 7070 696e 6720 3d20 7b6b 3a20 5b5d  mapping = {k: []
-00011b30: 2066 6f72 206b 2069 6e20 662e 6b65 7973   for k in f.keys
-00011b40: 2829 7d0a 2020 2020 2020 2020 2020 2020  ()}.            
-00011b50: 2020 2020 666f 7220 6b2c 2066 5f20 696e      for k, f_ in
-00011b60: 2066 2e69 7465 6d73 2829 3a0a 2020 2020   f.items():.    
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 6966 2066 5f20 6e6f 7420 696e 2064 6174  if f_ not in dat
-00011b90: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00011ba0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00011bb0: 2020 2020 2020 2020 2020 2020 6c6f 675f              log_
-00011bc0: 6572 726f 7228 6c6f 6767 6572 2c20 6622  error(logger, f"
-00011bd0: 4669 656c 6420 7b66 5f7d 206e 6f74 2066  Field {f_} not f
-00011be0: 6f75 6e64 2069 6e20 6461 7461 222c 2044  ound in data", D
-00011bf0: 6174 6145 7272 6f72 290a 2020 2020 2020  ataError).      
-00011c00: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00011c10: 7070 696e 675f 2c20 6461 7461 5f73 6574  pping_, data_set
-00011c20: 5f2c 2072 6573 5f73 6f72 745f 203d 2064  _, res_sort_ = d
-00011c30: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00011c40: 7570 6c65 5b66 5f5d 0a20 2020 2020 2020  uple[f_].       
-00011c50: 2020 2020 2020 2020 2020 2020 206d 6170               map
-00011c60: 7069 6e67 5b6b 5d20 3d20 6d61 7070 696e  ping[k] = mappin
-00011c70: 675f 0a20 2020 2020 2020 2020 2020 2020  g_.             
-00011c80: 2020 2020 2020 2064 6174 615f 7365 7420         data_set 
-00011c90: 3d20 6461 7461 5f73 6574 2069 6620 6461  = data_set if da
-00011ca0: 7461 5f73 6574 2065 6c73 6520 6461 7461  ta_set else data
-00011cb0: 5f73 6574 5f0a 2020 2020 2020 2020 2020  _set_.          
-00011cc0: 2020 2020 2020 2020 2020 7265 735f 736f            res_so
-00011cd0: 7274 203d 2072 6573 5f73 6f72 7420 6966  rt = res_sort if
-00011ce0: 2072 6573 5f73 6f72 7420 656c 7365 2072   res_sort else r
-00011cf0: 6573 5f73 6f72 745f 0a20 2020 2020 2020  es_sort_.       
-00011d00: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00011d10: 6572 7420 6461 7461 5f73 6574 203d 3d20  ert data_set == 
-00011d20: 6461 7461 5f73 6574 5f0a 2020 2020 2020  data_set_.      
-00011d30: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00011d40: 7365 7274 2072 6573 5f73 6f72 7420 3d3d  sert res_sort ==
-00011d50: 2072 6573 5f73 6f72 745f 0a20 2020 2020   res_sort_.     
-00011d60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00011d70: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00011d80: 5f65 7272 6f72 280a 2020 2020 2020 2020  _error(.        
-00011d90: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00011da0: 6572 2c20 6622 4669 656c 6420 7b66 7d20  er, f"Field {f} 
-00011db0: 6973 206e 6f74 2061 2073 7472 696e 672c  is not a string,
-00011dc0: 2074 7570 6c65 2c20 6c69 7374 206f 7220   tuple, list or 
-00011dd0: 6469 6374 222c 2044 6174 6145 7272 6f72  dict", DataError
-00011de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011df0: 2029 0a20 2020 2020 2020 2020 2020 2074   ).            t
-00011e00: 6173 6b73 2e61 7070 656e 6428 0a20 2020  asks.append(.   
-00011e10: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-00011e20: 6f72 742e 6372 6561 7465 5f72 6570 6f72  ort.create_repor
-00011e30: 745f 6461 7461 5f73 6574 280a 2020 2020  t_data_set(.    
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 6d61 7070 696e 675f 6461 7461 5f73 6574  mapping_data_set
-00011e60: 5f73 6f72 743d 286d 6170 7069 6e67 2c20  _sort=(mapping, 
-00011e70: 6461 7461 5f73 6574 2c20 7265 735f 736f  data_set, res_so
-00011e80: 7274 290a 2020 2020 2020 2020 2020 2020  rt).            
-00011e90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011ea0: 2020 290a 0a20 2020 2020 2020 2072 6570    )..        rep
-00011eb0: 6f72 745f 6461 7461 5f73 6574 7320 3d20  ort_data_sets = 
-00011ec0: 6177 6169 7420 6173 796e 6369 6f2e 6761  await asyncio.ga
-00011ed0: 7468 6572 282a 7461 736b 7329 0a20 2020  ther(*tasks).   
-00011ee0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00011ef0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-00011f00: 4372 6561 7465 6420 7b6c 656e 2872 6570  Created {len(rep
-00011f10: 6f72 745f 6461 7461 5f73 6574 7329 7d20  ort_data_sets)} 
-00011f20: 636f 6d70 6f6e 656e 7420 6461 7461 2073  component data s
-00011f30: 6574 206c 696e 6b73 2066 6f72 2063 6f6d  et links for com
-00011f40: 706f 6e65 6e74 207b 7374 7228 7265 706f  ponent {str(repo
-00011f50: 7274 297d 220a 2020 2020 2020 2020 290a  rt)}".        ).
-00011f60: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00011f70: 6570 6f72 745f 6461 7461 5f73 6574 730a  eport_data_sets.
-00011f80: 0a20 2020 2064 6566 205f 7570 6461 7465  .    def _update
-00011f90: 5f6f 7074 696f 6e73 2873 656c 662c 206f  _options(self, o
-00011fa0: 7074 696f 6e73 3a20 6469 6374 2c20 6f70  ptions: dict, op
-00011fb0: 7469 6f6e 5f6d 6f64 6966 6963 6174 696f  tion_modificatio
-00011fc0: 6e73 3a20 4f70 7469 6f6e 616c 5b64 6963  ns: Optional[dic
-00011fd0: 745d 293a 0a20 2020 2020 2020 2022 2222  t]):.        """
-00011fe0: 5570 6461 7465 2074 6865 206f 7074 696f  Update the optio
-00011ff0: 6e73 206f 6620 616e 2065 6368 6172 742e  ns of an echart.
-00012000: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00012010: 6f70 7469 6f6e 733a 2074 6865 206f 7074  options: the opt
-00012020: 696f 6e73 206f 6620 7468 6520 6563 6861  ions of the echa
-00012030: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
-00012040: 6d20 6f70 7469 6f6e 5f6d 6f64 6966 6963  m option_modific
-00012050: 6174 696f 6e73 3a20 7468 6520 6d6f 6469  ations: the modi
-00012060: 6669 6361 7469 6f6e 7320 746f 2061 7070  fications to app
-00012070: 6c79 2074 6f20 7468 6520 6f70 7469 6f6e  ly to the option
-00012080: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-00012090: 2020 2020 2020 6966 206e 6f74 206f 7074        if not opt
-000120a0: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
-000120b0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-000120c0: 6574 7572 6e0a 2020 2020 2020 2020 666f  eturn.        fo
-000120d0: 7220 6b2c 2076 2069 6e20 6f70 7469 6f6e  r k, v in option
-000120e0: 5f6d 6f64 6966 6963 6174 696f 6e73 2e69  _modifications.i
-000120f0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00012100: 2020 2020 6966 206b 203d 3d20 2273 6572      if k == "ser
-00012110: 6965 7322 3a0a 2020 2020 2020 2020 2020  ies":.          
-00012120: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
-00012130: 6c6f 6767 6572 2c20 2253 6572 6965 7320  logger, "Series 
-00012140: 6361 6e6e 6f74 2062 6520 6d6f 6469 6669  cannot be modifi
-00012150: 6564 222c 2044 6174 6145 7272 6f72 290a  ed", DataError).
-00012160: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00012170: 203d 3d20 2278 4178 6973 2220 6f72 206b   == "xAxis" or k
-00012180: 203d 3d20 2279 4178 6973 223a 0a20 2020   == "yAxis":.   
-00012190: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000121a0: 6973 696e 7374 616e 6365 2876 2c20 6469  isinstance(v, di
-000121b0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-000121c0: 2020 2020 2020 2020 2076 203d 205b 765d           v = [v]
-000121d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000121e0: 2069 6620 6c65 6e28 7629 2021 3d20 6c65   if len(v) != le
-000121f0: 6e28 6f70 7469 6f6e 735b 6b5d 293a 0a20  n(options[k]):. 
-00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012210: 2020 206c 6f67 5f65 7272 6f72 286c 6f67     log_error(log
-00012220: 6765 722c 2066 2254 6865 206e 756d 6265  ger, f"The numbe
-00012230: 7220 6f66 207b 6b7d 206d 7573 7420 6265  r of {k} must be
-00012240: 207b 6c65 6e28 7629 7d22 2c20 4461 7461   {len(v)}", Data
-00012250: 4572 726f 7229 0a20 2020 2020 2020 2020  Error).         
-00012260: 2020 2020 2020 2066 6f72 2069 2c20 765f         for i, v_
-00012270: 2069 6e20 656e 756d 6572 6174 6528 7629   in enumerate(v)
-00012280: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012290: 2020 2020 2020 6f70 7469 6f6e 735b 6b5d        options[k]
-000122a0: 5b69 5d2e 7570 6461 7465 2876 5f29 0a20  [i].update(v_). 
-000122b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000122c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000122d0: 206f 7074 696f 6e73 5b6b 5d20 3d20 760a   options[k] = v.
-000122e0: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
-000122f0: 6372 6561 7465 5f65 6368 6172 7428 0a20  create_echart(. 
-00012300: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00012310: 2020 2020 206f 7074 696f 6e73 3a20 6469       options: di
-00012320: 6374 2c0a 2020 2020 2020 2020 6f72 6465  ct,.        orde
-00012330: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
-00012340: 6669 656c 6473 3a20 6c69 7374 5b55 6e69  fields: list[Uni
-00012350: 6f6e 5b73 7472 2c20 7475 706c 652c 2064  on[str, tuple, d
-00012360: 6963 745d 5d2c 0a20 2020 2020 2020 2064  ict]],.        d
-00012370: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
-00012380: 7570 6c65 733a 204f 7074 696f 6e61 6c5b  uples: Optional[
-00012390: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
-000123a0: 2020 2020 2020 6461 7461 3a20 4f70 7469        data: Opti
-000123b0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-000123c0: 7064 2e44 6174 6146 7261 6d65 5d5d 203d  pd.DataFrame]] =
-000123d0: 204e 6f6e 652c 0a20 2020 2020 2020 2064   None,.        d
-000123e0: 756d 705f 7768 6f6c 653a 2062 6f6f 6c20  ump_whole: bool 
-000123f0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-00012400: 206f 7074 696f 6e5f 6d6f 6469 6669 6361   option_modifica
-00012410: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00012420: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
-00012430: 2020 2020 2020 7469 746c 653a 204f 7074        title: Opt
-00012440: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00012450: 652c 0a20 2020 2020 2020 2072 6f77 735f  e,.        rows_
-00012460: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
-00012470: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
-00012480: 2020 2020 636f 6c73 5f73 697a 653a 204f      cols_size: O
-00012490: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-000124a0: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
-000124b0: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
-000124c0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000124d0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-000124e0: 2020 2020 2020 2043 7265 6174 6520 616e         Create an
-000124f0: 2065 6368 6172 7420 696e 2074 6865 2064   echart in the d
-00012500: 6173 6862 6f61 7264 2c20 6669 6c6c 2069  ashboard, fill i
-00012510: 6e20 7468 6520 6461 7461 2072 6566 6572  n the data refer
-00012520: 656e 6365 6420 696e 2074 6865 2065 6368  enced in the ech
-00012530: 6172 745f 6f70 7469 6f6e 7320 616e 6420  art_options and 
-00012540: 6372 6561 7465 206f 720a 2020 2020 2020  create or.      
-00012550: 2020 7570 6461 7465 2074 6865 2063 6861    update the cha
-00012560: 7274 2061 6e64 2064 6174 6120 7365 7420  rt and data set 
-00012570: 6c69 6e6b 732e 0a20 2020 2020 2020 203a  links..        :
-00012580: 7061 7261 6d20 6f70 7469 6f6e 733a 2074  param options: t
-00012590: 6865 206f 7074 696f 6e73 206f 6620 7468  he options of th
-000125a0: 6520 6563 6861 7274 0a20 2020 2020 2020  e echart.       
-000125b0: 203a 7061 7261 6d20 6461 7461 5f6d 6170   :param data_map
-000125c0: 7069 6e67 5f74 6f5f 7475 706c 6573 3a20  ping_to_tuples: 
-000125d0: 7468 6520 6d61 7070 696e 6720 6f66 2074  the mapping of t
-000125e0: 6865 2064 6174 6120 746f 2074 6865 2074  he data to the t
-000125f0: 7570 6c65 730a 2020 2020 2020 2020 3a70  uples.        :p
-00012600: 6172 616d 2064 6174 613a 2074 6865 2064  aram data: the d
-00012610: 6174 6120 6f66 2074 6865 2065 6368 6172  ata of the echar
-00012620: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
-00012630: 2064 756d 705f 7768 6f6c 653a 2077 6865   dump_whole: whe
-00012640: 7468 6572 2074 6f20 6475 6d70 2074 6865  ther to dump the
-00012650: 2077 686f 6c65 2064 6174 610a 2020 2020   whole data.    
-00012660: 2020 2020 3a70 6172 616d 206f 7074 696f      :param optio
-00012670: 6e5f 6d6f 6469 6669 6361 7469 6f6e 733a  n_modifications:
-00012680: 2074 6865 206d 6f64 6966 6963 6174 696f   the modificatio
-00012690: 6e73 2074 6f20 6170 706c 7920 746f 2074  ns to apply to t
-000126a0: 6865 206f 7074 696f 6e73 0a20 2020 2020  he options.     
-000126b0: 2020 203a 7061 7261 6d20 7469 746c 653a     :param title:
-000126c0: 2074 6865 2074 6974 6c65 206f 6620 7468   the title of th
-000126d0: 6520 6563 6861 7274 0a20 2020 2020 2020  e echart.       
-000126e0: 203a 7061 7261 6d20 726f 7773 5f73 697a   :param rows_siz
-000126f0: 653a 2074 6865 2072 6f77 7320 7369 7a65  e: the rows size
-00012700: 206f 6620 7468 6520 6563 6861 7274 0a20   of the echart. 
-00012710: 2020 2020 2020 203a 7061 7261 6d20 636f         :param co
-00012720: 6c73 5f73 697a 653a 2074 6865 2063 6f6c  ls_size: the col
-00012730: 756d 6e73 2073 697a 6520 6f66 2074 6865  umns size of the
-00012740: 2065 6368 6172 740a 2020 2020 2020 2020   echart.        
-00012750: 3a70 6172 616d 2070 6164 6469 6e67 3a20  :param padding: 
-00012760: 7468 6520 7061 6464 696e 6720 6f66 2074  the padding of t
-00012770: 6865 2065 6368 6172 740a 2020 2020 2020  he echart.      
-00012780: 2020 2222 220a 0a20 2020 2020 2020 2069    """..        i
-00012790: 6620 6461 7461 2069 7320 6e6f 7420 4e6f  f data is not No
-000127a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000127b0: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
-000127c0: 7475 706c 6573 203d 2061 7761 6974 2073  tuples = await s
-000127d0: 656c 662e 5f63 686f 6f73 655f 6461 7461  elf._choose_data
-000127e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000127f0: 2020 6f72 6465 722c 2064 6174 612c 2064    order, data, d
-00012800: 756d 705f 7768 6f6c 653d 6475 6d70 5f77  ump_whole=dump_w
-00012810: 686f 6c65 0a20 2020 2020 2020 2020 2020  hole.           
-00012820: 2029 0a0a 2020 2020 2020 2020 6461 7461   )..        data
-00012830: 5f6b 6579 5f65 6e74 7269 6573 203d 2067  _key_entries = g
-00012840: 6574 5f64 6174 615f 7265 6665 7265 6e63  et_data_referenc
-00012850: 6573 5f66 726f 6d5f 6469 6374 286f 7074  es_from_dict(opt
-00012860: 696f 6e73 290a 2020 2020 2020 2020 5f2c  ions).        _,
-00012870: 2072 6570 6f72 7420 3d20 6177 6169 7420   report = await 
-00012880: 7365 6c66 2e5f 6765 745f 6368 6172 745f  self._get_chart_
-00012890: 7265 706f 7274 286f 7264 6572 2c20 4543  report(order, EC
-000128a0: 6861 7274 290a 0a20 2020 2020 2020 2072  hart)..        r
-000128b0: 645f 6964 7320 3d20 4e6f 6e65 0a20 2020  d_ids = None.   
-000128c0: 2020 2020 2069 6620 7365 6c66 2e72 6575       if self.reu
-000128d0: 7365 5f64 6174 615f 7365 7473 3a0a 2020  se_data_sets:.  
-000128e0: 2020 2020 2020 2020 2020 7264 5f69 6473            rd_ids
-000128f0: 203d 2067 6574 5f75 7569 6473 5f66 726f   = get_uuids_fro
-00012900: 6d5f 6469 6374 2872 6570 6f72 745b 2270  m_dict(report["p
-00012910: 726f 7065 7274 6965 7322 5d5b 226f 7074  roperties"]["opt
-00012920: 696f 6e22 5d29 0a20 2020 2020 2020 2020  ion"]).         
-00012930: 2020 2069 6620 6c65 6e28 7264 5f69 6473     if len(rd_ids
-00012940: 2920 3d3d 206c 656e 2866 6965 6c64 7329  ) == len(fields)
-00012950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012960: 2020 7265 705f 6473 3a20 6c69 7374 5b52    rep_ds: list[R
-00012970: 6570 6f72 742e 5265 706f 7274 4461 7461  eport.ReportData
-00012980: 5365 745d 203d 2061 7761 6974 2072 6570  Set] = await rep
-00012990: 6f72 742e 6765 745f 7265 706f 7274 5f64  ort.get_report_d
-000129a0: 6174 615f 7365 7473 2829 0a20 2020 2020  ata_sets().     
-000129b0: 2020 2020 2020 2020 2020 206d 6170 7065             mappe
-000129c0: 645f 6620 3d20 5b0a 2020 2020 2020 2020  d_f = [.        
-000129d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000129e0: 2e5f 6765 745f 6669 656c 645f 6d61 7070  ._get_field_mapp
-000129f0: 696e 6728 6669 656c 642c 2064 6174 615f  ing(field, data_
-00012a00: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-00012a10: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00012a20: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
-00012a30: 2069 6e20 6669 656c 6473 0a20 2020 2020   in fields.     
-00012a40: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00012a50: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00012a60: 2069 2c20 7264 5f69 6420 696e 2065 6e75   i, rd_id in enu
-00012a70: 6d65 7261 7465 2872 645f 6964 7329 3a0a  merate(rd_ids):.
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2020 7265 706f 7274 5f64 6174 615f      report_data_
-00012aa0: 7365 7420 3d20 6e65 7874 280a 2020 2020  set = next(.    
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 2020 2872 6420 666f 7220 7264 2069      (rd for rd i
-00012ad0: 6e20 7265 705f 6473 2069 6620 7264 5b22  n rep_ds if rd["
-00012ae0: 6964 225d 203d 3d20 7264 5f69 6429 2c20  id"] == rd_id), 
-00012af0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00012b00: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012b20: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00012b30: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
-00012b40: 7265 706f 7274 5f64 6174 615f 7365 740a  report_data_set.
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b60: 2020 2020 2020 2020 6f72 206e 6f74 2073          or not s
-00012b70: 656c 662e 5f63 6865 636b 5f6d 6170 7069  elf._check_mappi
-00012b80: 6e67 5f69 6e5f 7265 706f 7274 5f64 6174  ng_in_report_dat
-00012b90: 615f 7365 7428 0a20 2020 2020 2020 2020  a_set(.         
+0000f4e0: 6f6e 652c 0a20 2020 2020 2020 2061 6374  one,.        act
+0000f4f0: 696f 6e5f 6964 3a20 4f70 7469 6f6e 616c  ion_id: Optional
+0000f500: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000f510: 2020 2020 2020 6f6e 5f73 7562 6d69 745f        on_submit_
+0000f520: 6576 656e 7473 3a20 4f70 7469 6f6e 616c  events: Optional
+0000f530: 5b6c 6973 745b 6469 6374 5d5d 203d 204e  [list[dict]] = N
+0000f540: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+0000f550: 2020 2020 2222 2245 6173 6965 7220 7761      """Easier wa
+0000f560: 7920 746f 2063 7265 6174 6520 616e 2069  y to create an i
+0000f570: 6e70 7574 2066 6f72 6d2e 0a20 2020 2020  nput form..     
+0000f580: 2020 203a 7061 7261 6d20 6d65 6e75 5f70     :param menu_p
+0000f590: 6174 683a 2074 6865 206d 656e 7520 7061  ath: the menu pa
+0000f5a0: 7468 206f 6620 7468 6520 696e 7075 7420  th of the input 
+0000f5b0: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
+0000f5c0: 7261 6d20 6f72 6465 723a 2074 6865 206f  ram order: the o
+0000f5d0: 7264 6572 206f 6620 7468 6520 696e 7075  rder of the inpu
+0000f5e0: 7420 666f 726d 0a20 2020 2020 2020 203a  t form.        :
+0000f5f0: 7061 7261 6d20 666f 726d 5f67 726f 7570  param form_group
+0000f600: 733a 2074 6865 2066 6f72 6d20 6772 6f75  s: the form grou
+0000f610: 7073 206f 6620 7468 6520 696e 7075 7420  ps of the input 
+0000f620: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
+0000f630: 7261 6d20 6479 6e61 6d69 635f 7365 7175  ram dynamic_sequ
+0000f640: 656e 7469 616c 5f73 686f 773a 2077 6865  ential_show: whe
+0000f650: 7468 6572 2074 6f20 7368 6f77 2074 6865  ther to show the
+0000f660: 206e 6578 7420 6772 6f75 7020 6166 7465   next group afte
+0000f670: 7220 7375 626d 6974 7469 6e67 2074 6865  r submitting the
+0000f680: 2063 7572 7265 6e74 2067 726f 7570 0a20   current group. 
+0000f690: 2020 2020 2020 203a 7061 7261 6d20 6175         :param au
+0000f6a0: 746f 5f73 656e 643a 2077 6865 7468 6572  to_send: whether
+0000f6b0: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
+0000f6c0: 7920 7365 6e64 2074 6865 2066 6f72 6d20  y send the form 
+0000f6d0: 6166 7465 7220 7468 6520 6c61 7374 2067  after the last g
+0000f6e0: 726f 7570 0a20 2020 2020 2020 203a 7061  roup.        :pa
+0000f6f0: 7261 6d20 6e65 7874 5f67 726f 7570 5f6c  ram next_group_l
+0000f700: 6162 656c 3a20 7468 6520 6c61 6265 6c20  abel: the label 
+0000f710: 6f66 2074 6865 206e 6578 7420 6772 6f75  of the next grou
+0000f720: 7020 6275 7474 6f6e 0a20 2020 2020 2020  p button.       
+0000f730: 203a 7061 7261 6d20 726f 7773 5f73 697a   :param rows_siz
+0000f740: 653a 2074 6865 2072 6f77 7320 7369 7a65  e: the rows size
+0000f750: 206f 6620 7468 6520 696e 7075 7420 666f   of the input fo
+0000f760: 726d 0a20 2020 2020 2020 203a 7061 7261  rm.        :para
+0000f770: 6d20 636f 6c73 5f73 697a 653a 2074 6865  m cols_size: the
+0000f780: 2063 6f6c 756d 6e73 2073 697a 6520 6f66   columns size of
+0000f790: 2074 6865 2069 6e70 7574 2066 6f72 6d0a   the input form.
+0000f7a0: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+0000f7b0: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
+0000f7c0: 696e 6720 6f66 2074 6865 2069 6e70 7574  ing of the input
+0000f7d0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
+0000f7e0: 6172 616d 206d 6f64 616c 3a20 7468 6520  aram modal: the 
+0000f7f0: 6d6f 6461 6c20 746f 206f 7065 6e20 6166  modal to open af
+0000f800: 7465 7220 7375 626d 6974 7469 6e67 2074  ter submitting t
+0000f810: 6865 2066 6f72 6d0a 2020 2020 2020 2020  he form.        
+0000f820: 3a70 6172 616d 2061 6374 6976 6974 795f  :param activity_
+0000f830: 6964 3a20 7468 6520 6163 7469 7669 7479  id: the activity
+0000f840: 2069 6420 746f 2072 756e 2061 6674 6572   id to run after
+0000f850: 2073 7562 6d69 7474 696e 6720 7468 6520   submitting the 
+0000f860: 666f 726d 0a20 2020 2020 2020 203a 7061  form.        :pa
+0000f870: 7261 6d20 6163 7469 7669 7479 5f6e 616d  ram activity_nam
+0000f880: 653a 2074 6865 2061 6374 6976 6974 7920  e: the activity 
+0000f890: 6e61 6d65 2074 6f20 7275 6e20 6166 7465  name to run afte
+0000f8a0: 7220 7375 626d 6974 7469 6e67 2074 6865  r submitting the
+0000f8b0: 2066 6f72 6d0a 2020 2020 2020 2020 3a70   form.        :p
+0000f8c0: 6172 616d 2061 6374 696f 6e5f 6964 3a20  aram action_id: 
+0000f8d0: 7468 6520 6163 7469 6f6e 2069 6420 746f  the action id to
+0000f8e0: 2072 756e 2061 6674 6572 2073 7562 6d69   run after submi
+0000f8f0: 7474 696e 6720 7468 6520 666f 726d 0a20  tting the form. 
+0000f900: 2020 2020 2020 203a 7061 7261 6d20 6f6e         :param on
+0000f910: 5f73 7562 6d69 745f 6576 656e 7473 3a20  _submit_events: 
+0000f920: 7468 6520 6576 656e 7473 2074 6f20 7275  the events to ru
+0000f930: 6e20 6166 7465 7220 7375 626d 6974 7469  n after submitti
+0000f940: 6e67 2074 6865 2066 6f72 6d0a 2020 2020  ng the form.    
+0000f950: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f960: 7265 706f 7274 5f64 6174 615f 7365 745f  report_data_set_
+0000f970: 7072 6f70 6572 7469 6573 203d 207b 2266  properties = {"f
+0000f980: 6965 6c64 7322 3a20 5b5d 7d0a 2020 2020  ields": []}.    
+0000f990: 2020 2020 6966 2061 7574 6f5f 7365 6e64      if auto_send
+0000f9a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f9b0: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
+0000f9c0: 6f70 6572 7469 6573 5b22 7661 7269 616e  operties["varian
+0000f9d0: 7422 5d20 3d20 2261 7574 6f53 656e 6422  t"] = "autoSend"
+0000f9e0: 0a0a 2020 2020 2020 2020 725f 6861 7368  ..        r_hash
+0000f9f0: 203d 2073 656c 662e 5f67 6574 5f63 6861   = self._get_cha
+0000fa00: 7274 5f68 6173 6828 6f72 6465 7229 0a0a  rt_hash(order)..
+0000fa10: 2020 2020 2020 2020 6e65 7874 5f69 6420          next_id 
+0000fa20: 3d20 6622 7b72 5f68 6173 687d 5f30 2220  = f"{r_hash}_0" 
+0000fa30: 6966 2064 796e 616d 6963 5f73 6571 7565  if dynamic_seque
+0000fa40: 6e74 6961 6c5f 7368 6f77 2065 6c73 6520  ntial_show else 
+0000fa50: 4e6f 6e65 0a0a 2020 2020 2020 2020 6e65  None..        ne
+0000fa60: 7874 5f67 726f 7570 5f69 6e64 6578 203d  xt_group_index =
+0000fa70: 2031 0a20 2020 2020 2020 2066 6f72 2066   1.        for f
+0000fa80: 6f72 6d5f 6772 6f75 705f 6e61 6d65 2c20  orm_group_name, 
+0000fa90: 666f 726d 5f67 726f 7570 2069 6e20 666f  form_group in fo
+0000faa0: 726d 5f67 726f 7570 732e 6974 656d 7328  rm_groups.items(
+0000fab0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+0000fac0: 6f72 6d5f 6772 6f75 705f 6a73 6f6e 203d  orm_group_json =
+0000fad0: 207b 2274 6974 6c65 223a 2066 6f72 6d5f   {"title": form_
+0000fae0: 6772 6f75 705f 6e61 6d65 2c20 2266 6965  group_name, "fie
+0000faf0: 6c64 7322 3a20 666f 726d 5f67 726f 7570  lds": form_group
+0000fb00: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+0000fb10: 206e 6578 745f 6964 3a0a 2020 2020 2020   next_id:.      
+0000fb20: 2020 2020 2020 2020 2020 666f 726d 5f67            form_g
+0000fb30: 726f 7570 5f6a 736f 6e5b 2269 6422 5d20  roup_json["id"] 
+0000fb40: 3d20 6e65 7874 5f69 640a 2020 2020 2020  = next_id.      
+0000fb50: 2020 2020 2020 2020 2020 6e65 7874 5f69            next_i
+0000fb60: 6420 3d20 6622 7b72 5f68 6173 687d 5f7b  d = f"{r_hash}_{
+0000fb70: 6e65 7874 5f67 726f 7570 5f69 6e64 6578  next_group_index
+0000fb80: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000fb90: 2020 2066 6f72 6d5f 6772 6f75 705f 6a73     form_group_js
+0000fba0: 6f6e 5b22 6e65 7874 466f 726d 4772 6f75  on["nextFormGrou
+0000fbb0: 7022 5d20 3d20 7b0a 2020 2020 2020 2020  p"] = {.        
+0000fbc0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+0000fbd0: 3a20 6e65 7874 5f69 642c 0a20 2020 2020  : next_id,.     
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fbf0: 6c61 6265 6c22 3a20 6e65 7874 5f67 726f  label": next_gro
+0000fc00: 7570 5f6c 6162 656c 2c0a 2020 2020 2020  up_label,.      
+0000fc10: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+0000fc20: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+0000fc30: 5f67 726f 7570 5f69 6e64 6578 202b 3d20  _group_index += 
+0000fc40: 310a 2020 2020 2020 2020 2020 2020 7265  1.            re
+0000fc50: 706f 7274 5f64 6174 615f 7365 745f 7072  port_data_set_pr
+0000fc60: 6f70 6572 7469 6573 5b22 6669 656c 6473  operties["fields
+0000fc70: 225d 202b 3d20 5b66 6f72 6d5f 6772 6f75  "] += [form_grou
+0000fc80: 705f 6a73 6f6e 5d0a 0a20 2020 2020 2020  p_json]..       
+0000fc90: 2069 6620 6e65 7874 5f69 643a 0a20 2020   if next_id:.   
+0000fca0: 2020 2020 2020 2020 2064 656c 2072 6570           del rep
+0000fcb0: 6f72 745f 6461 7461 5f73 6574 5f70 726f  ort_data_set_pro
+0000fcc0: 7065 7274 6965 735b 2266 6965 6c64 7322  perties["fields"
+0000fcd0: 5d5b 2d31 5d5b 226e 6578 7446 6f72 6d47  ][-1]["nextFormG
+0000fce0: 726f 7570 225d 0a0a 2020 2020 2020 2020  roup"]..        
+0000fcf0: 7365 6c66 2e69 6e70 7574 5f66 6f72 6d28  self.input_form(
+0000fd00: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+0000fd10: 696f 6e73 3d72 6570 6f72 745f 6461 7461  ions=report_data
+0000fd20: 5f73 6574 5f70 726f 7065 7274 6965 732c  _set_properties,
+0000fd30: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+0000fd40: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
+0000fd50: 2020 2020 2020 726f 7773 5f73 697a 653d        rows_size=
+0000fd60: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
+0000fd70: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
+0000fd80: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
+0000fd90: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
+0000fda0: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
+0000fdb0: 2020 2020 206d 6f64 616c 3d6d 6f64 616c       modal=modal
+0000fdc0: 2c0a 2020 2020 2020 2020 2020 2020 6163  ,.            ac
+0000fdd0: 7469 7669 7479 5f69 643d 6163 7469 7669  tivity_id=activi
+0000fde0: 7479 5f69 642c 0a20 2020 2020 2020 2020  ty_id,.         
+0000fdf0: 2020 2061 6374 6976 6974 795f 6e61 6d65     activity_name
+0000fe00: 3d61 6374 6976 6974 795f 6e61 6d65 2c0a  =activity_name,.
+0000fe10: 2020 2020 2020 2020 2020 2020 6f6e 5f73              on_s
+0000fe20: 7562 6d69 745f 6576 656e 7473 3d6f 6e5f  ubmit_events=on_
+0000fe30: 7375 626d 6974 5f65 7665 6e74 732c 0a20  submit_events,. 
+0000fe40: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+0000fe50: 6e5f 6964 3d61 6374 696f 6e5f 6964 2c0a  n_id=action_id,.
+0000fe60: 2020 2020 2020 2020 290a 0a20 2020 2061          )..    a
+0000fe70: 7379 6e63 2064 6566 205f 6765 745f 696e  sync def _get_in
+0000fe80: 7075 745f 666f 726d 5f64 6174 6128 7365  put_form_data(se
+0000fe90: 6c66 2c20 696e 7075 745f 666f 726d 3a20  lf, input_form: 
+0000fea0: 496e 7075 7446 6f72 6d29 202d 3e20 6469  InputForm) -> di
+0000feb0: 6374 3a0a 2020 2020 2020 2020 2222 2247  ct:.        """G
+0000fec0: 6574 2074 6865 2069 6e70 7574 2066 6f72  et the input for
+0000fed0: 6d20 6461 7461 2e22 2222 0a20 2020 2020  m data.""".     
+0000fee0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
+0000fef0: 6574 203d 2028 6177 6169 7420 696e 7075  et = (await inpu
+0000ff00: 745f 666f 726d 2e67 6574 5f72 6570 6f72  t_form.get_repor
+0000ff10: 745f 6461 7461 5f73 6574 7328 2929 5b30  t_data_sets())[0
+0000ff20: 5d0a 2020 2020 2020 2020 6461 7461 5f73  ].        data_s
+0000ff30: 6574 203d 2061 7761 6974 2073 656c 662e  et = await self.
+0000ff40: 5f61 7070 2e67 6574 5f64 6174 615f 7365  _app.get_data_se
+0000ff50: 7428 7265 706f 7274 5f64 6174 615f 7365  t(report_data_se
+0000ff60: 745b 2264 6174 6153 6574 4964 225d 290a  t["dataSetId"]).
+0000ff70: 2020 2020 2020 2020 6461 7461 5f70 6f69          data_poi
+0000ff80: 6e74 203d 2061 7761 6974 2064 6174 615f  nt = await data_
+0000ff90: 7365 742e 6765 745f 6f6e 655f 6461 7461  set.get_one_data
+0000ffa0: 5f70 6f69 6e74 2829 0a20 2020 2020 2020  _point().       
+0000ffb0: 206c 6f67 6765 722e 696e 666f 2866 2247   logger.info(f"G
+0000ffc0: 6f74 2069 6e70 7574 2066 6f72 6d20 6461  ot input form da
+0000ffd0: 7461 2066 6f72 207b 7374 7228 696e 7075  ta for {str(inpu
+0000ffe0: 745f 666f 726d 297d 2229 0a20 2020 2020  t_form)}").     
+0000fff0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+00010000: 2020 2020 2020 2020 2272 6570 6f72 7449          "reportI
+00010010: 6422 3a20 696e 7075 745f 666f 726d 5b22  d": input_form["
+00010020: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
+00010030: 2020 226f 7264 6572 223a 2069 6e70 7574    "order": input
+00010040: 5f66 6f72 6d5b 226f 7264 6572 225d 2c0a  _form["order"],.
+00010050: 2020 2020 2020 2020 2020 2020 2264 6174              "dat
+00010060: 6122 3a20 6461 7461 5f70 6f69 6e74 5b22  a": data_point["
+00010070: 6375 7374 6f6d 4669 656c 6431 225d 2069  customField1"] i
+00010080: 6620 6461 7461 5f70 6f69 6e74 2065 6c73  f data_point els
+00010090: 6520 4e6f 6e65 2c0a 2020 2020 2020 2020  e None,.        
+000100a0: 7d0a 0a20 2020 2061 7379 6e63 2064 6566  }..    async def
+000100b0: 2067 6574 5f69 6e70 7574 5f66 6f72 6d73   get_input_forms
+000100c0: 2873 656c 6629 202d 3e20 6c69 7374 5b64  (self) -> list[d
+000100d0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+000100e0: 2247 6574 2061 6c6c 2074 6865 2069 6e70  "Get all the inp
+000100f0: 7574 2066 6f72 6d73 2069 6e20 7468 6520  ut forms in the 
+00010100: 6375 7272 656e 7420 6d65 6e75 5f70 6174  current menu_pat
+00010110: 682e 2222 220a 2020 2020 2020 2020 7265  h.""".        re
+00010120: 706f 7274 733a 206c 6973 7420 3d20 5b0a  ports: list = [.
+00010130: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00010140: 7274 0a20 2020 2020 2020 2020 2020 2066  rt.            f
+00010150: 6f72 2072 6570 6f72 7420 696e 2061 7761  or report in awa
+00010160: 6974 2073 656c 662e 5f61 7070 2e67 6574  it self._app.get
+00010170: 5f72 6570 6f72 7473 2829 0a20 2020 2020  _reports().     
+00010180: 2020 2020 2020 2069 6620 7265 706f 7274         if report
+00010190: 5b22 7265 706f 7274 5479 7065 225d 203d  ["reportType"] =
+000101a0: 3d20 2246 4f52 4d22 0a20 2020 2020 2020  = "FORM".       
+000101b0: 2020 2020 2061 6e64 2028 7265 706f 7274       and (report
+000101c0: 5b22 7061 7468 225d 203d 3d20 7365 6c66  ["path"] == self
+000101d0: 2e5f 6375 7272 656e 745f 7061 7468 206f  ._current_path o
+000101e0: 7220 6e6f 7420 7365 6c66 2e5f 6375 7272  r not self._curr
+000101f0: 656e 745f 7061 7468 290a 2020 2020 2020  ent_path).      
+00010200: 2020 5d0a 2020 2020 2020 2020 7265 7475    ].        retu
+00010210: 726e 206c 6973 7428 0a20 2020 2020 2020  rn list(.       
+00010220: 2020 2020 2061 7761 6974 2061 7379 6e63       await async
+00010230: 696f 2e67 6174 6865 7228 0a20 2020 2020  io.gather(.     
+00010240: 2020 2020 2020 2020 2020 202a 5b73 656c             *[sel
+00010250: 662e 5f67 6574 5f69 6e70 7574 5f66 6f72  f._get_input_for
+00010260: 6d5f 6461 7461 2872 6570 6f72 7429 2066  m_data(report) f
+00010270: 6f72 2072 6570 6f72 7420 696e 2072 6570  or report in rep
+00010280: 6f72 7473 5d0a 2020 2020 2020 2020 2020  orts].          
+00010290: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
+000102a0: 2020 2040 6164 645f 746f 5f67 656e 6572     @add_to_gener
+000102b0: 616c 5f61 7379 6e63 5f67 726f 7570 0a20  al_async_group. 
+000102c0: 2020 2061 7379 6e63 2064 6566 2061 6e6e     async def ann
+000102d0: 6f74 6174 6564 5f63 6861 7274 280a 2020  otated_chart(.  
+000102e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000102f0: 2020 2020 6461 7461 3a20 556e 696f 6e5b      data: Union[
+00010300: 6c69 7374 5b44 6174 6146 7261 6d65 5d2c  list[DataFrame],
+00010310: 206c 6973 745b 6c69 7374 5b64 6963 745d   list[list[dict]
+00010320: 5d5d 2c0a 2020 2020 2020 2020 6f72 6465  ]],.        orde
+00010330: 723a 2069 6e74 2c0a 2020 2020 2020 2020  r: int,.        
+00010340: 783a 2073 7472 2c0a 2020 2020 2020 2020  x: str,.        
+00010350: 793a 2055 6e69 6f6e 5b73 7472 2c20 6c69  y: Union[str, li
+00010360: 7374 5b73 7472 5d5d 2c0a 2020 2020 2020  st[str]],.      
+00010370: 2020 616e 6e6f 7461 7469 6f6e 733a 2073    annotations: s
+00010380: 7472 203d 2022 616e 6e6f 7461 7469 6f6e  tr = "annotation
+00010390: 222c 0a20 2020 2020 2020 2072 6f77 735f  ",.        rows_
+000103a0: 7369 7a65 3a20 4f70 7469 6f6e 616c 5b69  size: Optional[i
+000103b0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+000103c0: 2020 2020 636f 6c73 5f73 697a 653a 204f      cols_size: O
+000103d0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+000103e0: 6f6e 652c 0a20 2020 2020 2020 2070 6164  one,.        pad
+000103f0: 6469 6e67 3a20 4f70 7469 6f6e 616c 5b73  ding: Optional[s
+00010400: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00010410: 2020 2020 7469 746c 653a 204f 7074 696f      title: Optio
+00010420: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00010430: 0a20 2020 2020 2020 2079 5f61 7869 735f  .        y_axis_
+00010440: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
+00010450: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00010460: 2020 2020 736c 6964 6572 5f63 6f6e 6669      slider_confi
+00010470: 673a 204f 7074 696f 6e61 6c5b 6469 6374  g: Optional[dict
+00010480: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00010490: 2020 736c 6964 6572 5f6d 6172 6b73 3a20    slider_marks: 
+000104a0: 4f70 7469 6f6e 616c 5b6c 6973 745b 7475  Optional[list[tu
+000104b0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
+000104c0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+000104d0: 0a20 2020 2020 2020 2043 7265 6174 6520  .        Create 
+000104e0: 616e 2061 6e6e 6f74 6174 6564 2063 6861  an annotated cha
+000104f0: 7274 2069 6e20 7468 6520 6d65 6e75 2070  rt in the menu p
+00010500: 6174 682e 0a20 2020 2020 2020 203a 7061  ath..        :pa
+00010510: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
+00010520: 7461 206f 6620 7468 6520 6368 6172 740a  ta of the chart.
+00010530: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00010540: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
+00010550: 6f66 2074 6865 2063 6861 7274 0a20 2020  of the chart.   
+00010560: 2020 2020 203a 7061 7261 6d20 783a 2074       :param x: t
+00010570: 6865 2078 2061 7869 730a 2020 2020 2020  he x axis.      
+00010580: 2020 3a70 6172 616d 2079 3a20 7468 6520    :param y: the 
+00010590: 7920 6178 6973 0a20 2020 2020 2020 203a  y axis.        :
+000105a0: 7061 7261 6d20 616e 6e6f 7461 7469 6f6e  param annotation
+000105b0: 733a 2074 6865 2061 6e6e 6f74 6174 696f  s: the annotatio
+000105c0: 6e73 0a20 2020 2020 2020 203a 7061 7261  ns.        :para
+000105d0: 6d20 726f 7773 5f73 697a 653a 2074 6865  m rows_size: the
+000105e0: 2072 6f77 7320 7369 7a65 206f 6620 7468   rows size of th
+000105f0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
+00010600: 3a70 6172 616d 2063 6f6c 735f 7369 7a65  :param cols_size
+00010610: 3a20 7468 6520 636f 6c75 6d6e 7320 7369  : the columns si
+00010620: 7a65 206f 6620 7468 6520 6368 6172 740a  ze of the chart.
+00010630: 2020 2020 2020 2020 3a70 6172 616d 2070          :param p
+00010640: 6164 6469 6e67 3a20 7468 6520 7061 6464  adding: the padd
+00010650: 696e 6720 6f66 2074 6865 2063 6861 7274  ing of the chart
+00010660: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010670: 7469 746c 653a 2074 6865 2074 6974 6c65  title: the title
+00010680: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
+00010690: 2020 2020 2020 3a70 6172 616d 2079 5f61        :param y_a
+000106a0: 7869 735f 6e61 6d65 3a20 7468 6520 6e61  xis_name: the na
+000106b0: 6d65 206f 6620 7468 6520 7920 6178 6973  me of the y axis
+000106c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000106d0: 736c 6964 6572 5f63 6f6e 6669 673a 2074  slider_config: t
+000106e0: 6865 2073 6c69 6465 7220 636f 6e66 6967  he slider config
+000106f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00010700: 736c 6964 6572 5f6d 6172 6b73 3a20 7468  slider_marks: th
+00010710: 6520 736c 6964 6572 206d 6172 6b73 0a20  e slider marks. 
+00010720: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00010730: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00010740: 2864 6174 612c 2073 7472 293a 0a20 2020  (data, str):.   
+00010750: 2020 2020 2020 2020 206c 6f67 5f65 7272           log_err
+00010760: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00010770: 2020 2020 6c6f 6767 6572 2c0a 2020 2020      logger,.    
+00010780: 2020 2020 2020 2020 2020 2020 2241 6e6e              "Ann
+00010790: 6f74 6174 6564 2063 6861 7274 2064 6f65  otated chart doe
+000107a0: 7320 6e6f 7420 7375 7070 6f72 7420 7468  s not support th
+000107b0: 6520 7573 6520 6f66 2073 6861 7265 6420  e use of shared 
+000107c0: 6461 7461 222c 0a20 2020 2020 2020 2020  data",.         
+000107d0: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
+000107e0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+000107f0: 0a20 2020 2020 2020 2069 6620 736c 6964  .        if slid
+00010800: 6572 5f63 6f6e 6669 6720 6973 204e 6f6e  er_config is Non
+00010810: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00010820: 6c69 6465 725f 636f 6e66 6967 203d 207b  lider_config = {
+00010830: 7d0a 0a20 2020 2020 2020 2069 6620 736c  }..        if sl
+00010840: 6964 6572 5f6d 6172 6b73 3a0a 2020 2020  ider_marks:.    
+00010850: 2020 2020 2020 2020 736c 6964 6572 5f63          slider_c
+00010860: 6f6e 6669 675b 226d 6172 6b73 225d 203d  onfig["marks"] =
+00010870: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00010880: 2020 207b 226c 6162 656c 223a 206d 6172     {"label": mar
+00010890: 6b5b 305d 2c20 2276 616c 7565 223a 206d  k[0], "value": m
+000108a0: 6172 6b5b 315d 7d20 666f 7220 6d61 726b  ark[1]} for mark
+000108b0: 2069 6e20 736c 6964 6572 5f6d 6172 6b73   in slider_marks
+000108c0: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
+000108d0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000108e0: 7461 6e63 6528 792c 2073 7472 293a 0a20  tance(y, str):. 
+000108f0: 2020 2020 2020 2020 2020 2079 203d 205b             y = [
+00010900: 795d 0a0a 2020 2020 2020 2020 6966 206e  y]..        if n
+00010910: 6f74 206c 656e 2879 2920 3d3d 206c 656e  ot len(y) == len
+00010920: 2864 6174 6129 3a0a 2020 2020 2020 2020  (data):.        
+00010930: 2020 2020 6c6f 675f 6572 726f 7228 0a20      log_error(. 
+00010940: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00010950: 6f67 6765 722c 0a20 2020 2020 2020 2020  ogger,.         
+00010960: 2020 2020 2020 2066 224e 756d 6265 7220         f"Number 
+00010970: 6f66 2079 2076 616c 7565 7320 287b 6c65  of y values ({le
+00010980: 6e28 7929 7d29 2064 6f65 7320 6e6f 7420  n(y)}) does not 
+00010990: 6d61 7463 6820 6e75 6d62 6572 206f 6620  match number of 
+000109a0: 6461 7461 6672 616d 6573 2028 7b6c 656e  dataframes ({len
+000109b0: 2864 6174 6129 7d29 222c 0a20 2020 2020  (data)})",.     
+000109c0: 2020 2020 2020 2020 2020 2044 6174 6145             DataE
+000109d0: 7272 6f72 2c0a 2020 2020 2020 2020 2020  rror,.          
+000109e0: 2020 290a 0a20 2020 2020 2020 205f 2c20    )..        _, 
+000109f0: 7265 706f 7274 203d 2061 7761 6974 2073  report = await s
+00010a00: 656c 662e 5f67 6574 5f63 6861 7274 5f72  elf._get_chart_r
+00010a10: 6570 6f72 7428 6f72 6465 722c 2041 6e6e  eport(order, Ann
+00010a20: 6f74 6174 6564 4543 6861 7274 290a 0a20  otatedEChart).. 
+00010a30: 2020 2020 2020 2064 6673 203d 205b 7661         dfs = [va
+00010a40: 6c69 6461 7465 5f64 6174 615f 6973 5f70  lidate_data_is_p
+00010a50: 616e 6461 7261 626c 6528 6466 2920 666f  andarable(df) fo
+00010a60: 7220 6466 2069 6e20 6461 7461 5d0a 2020  r df in data].  
+00010a70: 2020 2020 2020 6461 7461 5f73 6574 5f74        data_set_t
+00010a80: 6173 6b73 203d 205b 5d0a 2020 2020 2020  asks = [].      
+00010a90: 2020 666f 7220 6466 2c20 795f 7661 6c20    for df, y_val 
+00010aa0: 696e 207a 6970 2864 6673 2c20 7929 3a0a  in zip(dfs, y):.
+00010ab0: 2020 2020 2020 2020 2020 2020 6466 5b78              df[x
+00010ac0: 5d20 3d20 7064 2e74 6f5f 6461 7465 7469  ] = pd.to_dateti
+00010ad0: 6d65 2864 665b 785d 290a 2020 2020 2020  me(df[x]).      
+00010ae0: 2020 2020 2020 6966 2061 6e6e 6f74 6174        if annotat
+00010af0: 696f 6e73 2069 6e20 6466 3a0a 2020 2020  ions in df:.    
+00010b00: 2020 2020 2020 2020 2020 2020 6466 5b61              df[a
+00010b10: 6e6e 6f74 6174 696f 6e73 5d20 3d20 280a  nnotations] = (.
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2020 6466 5b61 6e6e 6f74 6174 696f      df[annotatio
+00010b40: 6e73 5d2e 7265 706c 6163 6528 6e70 2e6e  ns].replace(np.n
+00010b50: 616e 2c20 2222 2c20 7265 6765 783d 5472  an, "", regex=Tr
+00010b60: 7565 292e 6173 7479 7065 2873 7472 290a  ue).astype(str).
+00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b80: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
+00010b90: 7461 5f73 6574 5f74 6173 6b73 2e61 7070  ta_set_tasks.app
+00010ba0: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+00010bb0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+00010bc0: 655f 6461 7461 5f73 6574 286e 616d 653d  e_data_set(name=
+00010bd0: 6622 7b72 6570 6f72 745b 2769 6427 5d7d  f"{report['id']}
+00010be0: 5f7b 795f 7661 6c7d 222c 2064 6174 613d  _{y_val}", data=
+00010bf0: 6466 290a 2020 2020 2020 2020 2020 2020  df).            
+00010c00: 290a 0a20 2020 2020 2020 2064 6174 615f  )..        data_
+00010c10: 7365 745f 6469 6374 7320 3d20 6177 6169  set_dicts = awai
+00010c20: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
+00010c30: 282a 6461 7461 5f73 6574 5f74 6173 6b73  (*data_set_tasks
+00010c40: 290a 2020 2020 2020 2020 6461 7461 5f73  ).        data_s
+00010c50: 6574 7320 3d20 5b64 735b 795f 7661 6c5d  ets = [ds[y_val]
+00010c60: 5b31 5d20 666f 7220 6473 2c20 795f 7661  [1] for ds, y_va
+00010c70: 6c20 696e 207a 6970 2864 6174 615f 7365  l in zip(data_se
+00010c80: 745f 6469 6374 732c 2079 295d 0a0a 2020  t_dicts, y)]..  
+00010c90: 2020 2020 2020 7264 5f69 6473 203d 204e        rd_ids = N
+00010ca0: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+00010cb0: 656c 662e 7265 7573 655f 6461 7461 5f73  elf.reuse_data_s
+00010cc0: 6574 733a 0a20 2020 2020 2020 2020 2020  ets:.           
+00010cd0: 2072 645f 6964 7320 3d20 6765 745f 7575   rd_ids = get_uu
+00010ce0: 6964 735f 6672 6f6d 5f64 6963 7428 7265  ids_from_dict(re
+00010cf0: 706f 7274 5b22 7072 6f70 6572 7469 6573  port["properties
+00010d00: 225d 5b22 6f70 7469 6f6e 225d 290a 2020  "]["option"]).  
+00010d10: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00010d20: 2872 645f 6964 7329 203d 3d20 6c65 6e28  (rd_ids) == len(
+00010d30: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
+00010d40: 2020 2020 7265 705f 6473 3a20 6c69 7374      rep_ds: list
+00010d50: 5b52 6570 6f72 742e 5265 706f 7274 4461  [Report.ReportDa
+00010d60: 7461 5365 745d 203d 2061 7761 6974 2072  taSet] = await r
+00010d70: 6570 6f72 742e 6765 745f 7265 706f 7274  eport.get_report
+00010d80: 5f64 6174 615f 7365 7473 2829 0a20 2020  _data_sets().   
+00010d90: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00010da0: 5f64 7320 3d20 5b0a 2020 2020 2020 2020  _ds = [.        
+00010db0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00010dc0: 2828 7264 2066 6f72 2072 6420 696e 2072  ((rd for rd in r
+00010dd0: 6570 5f64 7320 6966 2072 645b 2269 6422  ep_ds if rd["id"
+00010de0: 5d20 3d3d 2072 645f 6964 292c 204e 6f6e  ] == rd_id), Non
+00010df0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00010e00: 2020 2020 2020 2066 6f72 2072 645f 6964         for rd_id
+00010e10: 2069 6e20 7264 5f69 6473 0a20 2020 2020   in rd_ids.     
+00010e20: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00010e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010e40: 616e 7928 0a20 2020 2020 2020 2020 2020  any(.           
+00010e50: 2020 2020 2020 2020 2072 645b 2264 6174           rd["dat
+00010e60: 6153 6574 4964 225d 2021 3d20 6473 5b22  aSetId"] != ds["
+00010e70: 6964 225d 0a20 2020 2020 2020 2020 2020  id"].           
+00010e80: 2020 2020 2020 2020 206f 7220 7264 5b22           or rd["
+00010e90: 7072 6f70 6572 7469 6573 225d 5b22 6d61  properties"]["ma
+00010ea0: 7070 696e 6722 5d0a 2020 2020 2020 2020  pping"].        
+00010eb0: 2020 2020 2020 2020 2020 2020 213d 207b              != {
+00010ec0: 2276 616c 7565 7322 3a20 5b22 6461 7465  "values": ["date
+00010ed0: 4669 656c 6431 222c 2022 696e 7446 6965  Field1", "intFie
+00010ee0: 6c64 3122 5d2c 2022 6c61 6265 6c22 3a20  ld1"], "label": 
+00010ef0: 2273 7472 696e 6746 6965 6c64 3122 7d0a  "stringField1"}.
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2020 2020 666f 7220 7264 2c20 6473 2069      for rd, ds i
+00010f20: 6e20 7a69 7028 7265 705f 6473 2c20 6461  n zip(rep_ds, da
+00010f30: 7461 5f73 6574 7329 0a20 2020 2020 2020  ta_sets).       
+00010f40: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f60: 7264 5f69 6473 203d 204e 6f6e 650a 0a20  rd_ids = None.. 
+00010f70: 2020 2020 2020 2069 6620 6e6f 7420 7264         if not rd
+00010f80: 5f69 6473 3a0a 2020 2020 2020 2020 2020  _ids:.          
+00010f90: 2020 6177 6169 7420 7265 706f 7274 2e64    await report.d
+00010fa0: 656c 6574 655f 7265 706f 7274 5f64 6174  elete_report_dat
+00010fb0: 615f 7365 7473 286c 6f67 3d54 7275 6529  a_sets(log=True)
+00010fc0: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
+00010fd0: 7069 6e67 3a20 4d61 7070 696e 6720 3d20  ping: Mapping = 
+00010fe0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00010ff0: 2020 2276 616c 7565 7322 3a20 5b22 6461    "values": ["da
+00011000: 7465 4669 656c 6431 222c 2022 696e 7446  teField1", "intF
+00011010: 6965 6c64 3122 5d2c 0a20 2020 2020 2020  ield1"],.       
+00011020: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00011030: 3a20 2273 7472 696e 6746 6965 6c64 3122  : "stringField1"
+00011040: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+00011050: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+00011060: 7274 5f64 6174 615f 7365 7473 203d 2061  rt_data_sets = a
+00011070: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
+00011080: 6865 7228 0a20 2020 2020 2020 2020 2020  her(.           
+00011090: 2020 2020 202a 5b0a 2020 2020 2020 2020       *[.        
+000110a0: 2020 2020 2020 2020 2020 2020 7265 706f              repo
+000110b0: 7274 2e63 7265 6174 655f 7265 706f 7274  rt.create_report
+000110c0: 5f64 6174 615f 7365 7428 286d 6170 7069  _data_set((mappi
+000110d0: 6e67 2c20 6461 7461 5f73 6574 2c20 4e6f  ng, data_set, No
+000110e0: 6e65 2929 0a20 2020 2020 2020 2020 2020  ne)).           
+000110f0: 2020 2020 2020 2020 2066 6f72 2064 6174           for dat
+00011100: 615f 7365 7420 696e 2064 6174 615f 7365  a_set in data_se
+00011110: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00011120: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00011130: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+00011140: 645f 6964 7320 3d20 5b72 645b 2269 6422  d_ids = [rd["id"
+00011150: 5d20 666f 7220 7264 2069 6e20 7265 706f  ] for rd in repo
+00011160: 7274 5f64 6174 615f 7365 7473 5d0a 0a20  rt_data_sets].. 
+00011170: 2020 2020 2020 2063 6861 7274 5f6f 7074         chart_opt
+00011180: 696f 6e73 203d 207b 0a20 2020 2020 2020  ions = {.       
+00011190: 2020 2020 2022 7941 7869 7322 3a20 7b0a       "yAxis": {.
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 226e 616d 6522 3a20 795f 6178 6973 5f6e  "name": y_axis_n
+000111c0: 616d 6520 6f72 2022 222c 0a20 2020 2020  ame or "",.     
+000111d0: 2020 2020 2020 2020 2020 2022 666f 6e74             "font
+000111e0: 2220 2274 7970 6522 3a20 2276 616c 7565  " "type": "value
+000111f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00011200: 2020 2022 6e61 6d65 4c6f 6361 7469 6f6e     "nameLocation
+00011210: 223a 2022 6d69 6464 6c65 222c 0a20 2020  ": "middle",.   
+00011220: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+00011230: 6d65 4761 7022 3a20 3330 2c0a 2020 2020  meGap": 30,.    
+00011240: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00011250: 2020 2020 2020 2022 7841 7869 7322 3a20         "xAxis": 
+00011260: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00011270: 2020 2274 7970 6522 3a20 2274 696d 6522    "type": "time"
+00011280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011290: 2020 226e 616d 654c 6f63 6174 696f 6e22    "nameLocation"
+000112a0: 3a20 226d 6964 646c 6522 2c0a 2020 2020  : "middle",.    
+000112b0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+000112c0: 6547 6170 223a 2033 302c 0a20 2020 2020  eGap": 30,.     
+000112d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000112e0: 2020 2020 2020 2273 6572 6965 7322 3a20        "series": 
+000112f0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00011300: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00011310: 2020 2020 2020 2020 2264 6174 6122 3a20          "data": 
+00011320: 2223 7b22 202b 2072 645f 6964 202b 2022  "#{" + rd_id + "
+00011330: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+00011340: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00011350: 226c 696e 6522 2c0a 2020 2020 2020 2020  "line",.        
+00011360: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00011370: 6522 3a20 795f 6e61 6d65 2c0a 2020 2020  e": y_name,.    
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2269 7465 6d53 7479 6c65 223a 207b 0a20  "itemStyle": {. 
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2022 626f 7264 6572 5261         "borderRa
+000113c0: 6469 7573 223a 205b 392c 2039 2c20 302c  dius": [9, 9, 0,
+000113d0: 2030 5d2c 0a20 2020 2020 2020 2020 2020   0],.           
+000113e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000113f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00011400: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011410: 7220 795f 6e61 6d65 2c20 7264 5f69 6420  r y_name, rd_id 
+00011420: 696e 207a 6970 2879 2c20 7264 5f69 6473  in zip(y, rd_ids
+00011430: 290a 2020 2020 2020 2020 2020 2020 5d2c  ).            ],
+00011440: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00011450: 2020 2061 7761 6974 2073 656c 662e 5f63     await self._c
+00011460: 7265 6174 655f 6368 6172 7428 0a20 2020  reate_chart(.   
+00011470: 2020 2020 2020 2020 2063 6861 7274 5f63           chart_c
+00011480: 6c61 7373 3d41 6e6e 6f74 6174 6564 4543  lass=AnnotatedEC
+00011490: 6861 7274 2c0a 2020 2020 2020 2020 2020  hart,.          
+000114a0: 2020 6f72 6465 723d 6f72 6465 722c 0a20    order=order,. 
+000114b0: 2020 2020 2020 2020 2020 2073 697a 6550             sizeP
+000114c0: 6164 6469 6e67 3d70 6164 6469 6e67 2c0a  adding=padding,.
+000114d0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+000114e0: 526f 7773 3d72 6f77 735f 7369 7a65 2c0a  Rows=rows_size,.
+000114f0: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00011500: 436f 6c75 6d6e 733d 636f 6c73 5f73 697a  Columns=cols_siz
+00011510: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
+00011520: 6974 6c65 3d74 6974 6c65 2c0a 2020 2020  itle=title,.    
+00011530: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
+00011540: 6573 3d64 6963 7428 0a20 2020 2020 2020  es=dict(.       
+00011550: 2020 2020 2020 2020 2073 6c69 6465 723d           slider=
+00011560: 736c 6964 6572 5f63 6f6e 6669 672c 0a20  slider_config,. 
+00011570: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00011580: 7074 696f 6e3d 6368 6172 745f 6f70 7469  ption=chart_opti
+00011590: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+000115a0: 2029 2c0a 2020 2020 2020 2020 290a 0a20   ),.        ).. 
+000115b0: 2020 2061 7379 6e63 2064 6566 205f 6765     async def _ge
+000115c0: 745f 7265 706f 7274 5f64 6174 615f 7365  t_report_data_se
+000115d0: 7473 5f70 6572 5f6d 6170 7069 6e67 280a  ts_per_mapping(.
+000115e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000115f0: 2020 2020 2020 7265 706f 7274 3a20 5265        report: Re
+00011600: 706f 7274 2c0a 2020 2020 2020 2020 6461  port,.        da
+00011610: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00011620: 706c 653a 2064 6963 742c 0a20 2020 2020  ple: dict,.     
+00011630: 2020 2066 6965 6c64 733a 206c 6973 745b     fields: list[
+00011640: 556e 696f 6e5b 7475 706c 652c 2064 6963  Union[tuple, dic
+00011650: 745d 5d2c 0a20 2020 2029 202d 3e20 6c69  t]],.    ) -> li
+00011660: 7374 5b52 6570 6f72 742e 5265 706f 7274  st[Report.Report
+00011670: 4461 7461 5365 745d 3a0a 2020 2020 2020  DataSet]:.      
+00011680: 2020 2222 2243 7265 6174 6520 6120 6461    """Create a da
+00011690: 7461 5f73 6574 2070 6572 2066 6965 6c64  ta_set per field
+000116a0: 206f 6620 6120 6461 7461 6672 616d 652e   of a dataframe.
+000116b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000116c0: 7265 706f 7274 3a20 7468 6520 7265 706f  report: the repo
+000116d0: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+000116e0: 6d20 6461 7461 5f6d 6170 7069 6e67 5f74  m data_mapping_t
+000116f0: 6f5f 7475 706c 653a 2074 6865 206d 6170  o_tuple: the map
+00011700: 7069 6e67 206f 6620 7468 6520 6461 7461  ping of the data
+00011710: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00011720: 6669 656c 6473 3a20 7468 6520 6669 656c  fields: the fiel
+00011730: 6473 206f 6620 7468 6520 6461 7461 2074  ds of the data t
+00011740: 6f20 6265 2075 7365 640a 2020 2020 2020  o be used.      
+00011750: 2020 3a72 6574 7572 6e3a 2074 6865 206c    :return: the l
+00011760: 6973 7420 6f66 2064 6174 6120 7365 7473  ist of data sets
+00011770: 2070 6172 7469 7469 6f6e 6564 2062 7920   partitioned by 
+00011780: 6178 6973 2061 6e64 2066 6965 6c64 730a  axis and fields.
+00011790: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000117a0: 2020 2020 7461 736b 7320 3d20 5b5d 0a20      tasks = []. 
+000117b0: 2020 2020 2020 2066 6965 6c64 7320 3d20         fields = 
+000117c0: 6669 656c 6473 2069 6620 6669 656c 6473  fields if fields
+000117d0: 2065 6c73 6520 5b5d 0a20 2020 2020 2020   else [].       
+000117e0: 2066 6f72 2069 2c20 6620 696e 2065 6e75   for i, f in enu
+000117f0: 6d65 7261 7465 2866 6965 6c64 7329 3a0a  merate(fields):.
+00011800: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
+00011810: 696e 6720 3d20 5b5d 0a20 2020 2020 2020  ing = [].       
+00011820: 2020 2020 2064 6174 615f 7365 7420 3d20       data_set = 
+00011830: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00011840: 2072 6573 5f73 6f72 7420 3d20 4e6f 6e65   res_sort = None
+00011850: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011860: 6973 696e 7374 616e 6365 2866 2c20 7374  isinstance(f, st
+00011870: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00011880: 2020 2020 6966 2066 206e 6f74 2069 6e20      if f not in 
+00011890: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
+000118a0: 7475 706c 653a 0a20 2020 2020 2020 2020  tuple:.         
+000118b0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+000118c0: 7272 6f72 286c 6f67 6765 722c 2066 2246  rror(logger, f"F
+000118d0: 6965 6c64 207b 667d 206e 6f74 2066 6f75  ield {f} not fou
+000118e0: 6e64 2069 6e20 6461 7461 222c 2044 6174  nd in data", Dat
+000118f0: 6145 7272 6f72 290a 2020 2020 2020 2020  aError).        
+00011900: 2020 2020 2020 2020 6d61 7070 696e 672c          mapping,
+00011910: 2064 6174 615f 7365 742c 2072 6573 5f73   data_set, res_s
+00011920: 6f72 7420 3d20 6461 7461 5f6d 6170 7069  ort = data_mappi
+00011930: 6e67 5f74 6f5f 7475 706c 655b 665d 0a20  ng_to_tuple[f]. 
+00011940: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00011950: 6973 696e 7374 616e 6365 2866 2c20 2874  isinstance(f, (t
+00011960: 7570 6c65 2c20 6c69 7374 2929 3a0a 2020  uple, list)):.  
+00011970: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011980: 7220 665f 2069 6e20 663a 0a20 2020 2020  r f_ in f:.     
+00011990: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000119a0: 6620 665f 206e 6f74 2069 6e20 6461 7461  f f_ not in data
+000119b0: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
+000119c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000119d0: 2020 2020 2020 2020 2020 206c 6f67 5f65             log_e
+000119e0: 7272 6f72 286c 6f67 6765 722c 2066 2246  rror(logger, f"F
+000119f0: 6965 6c64 207b 665f 7d20 6e6f 7420 666f  ield {f_} not fo
+00011a00: 756e 6420 696e 2064 6174 6122 2c20 4461  und in data", Da
+00011a10: 7461 4572 726f 7229 0a20 2020 2020 2020  taError).       
+00011a20: 2020 2020 2020 2020 2020 2020 206d 6170               map
+00011a30: 7069 6e67 5f2c 2064 6174 615f 7365 745f  ping_, data_set_
+00011a40: 2c20 7265 735f 736f 7274 5f20 3d20 6461  , res_sort_ = da
+00011a50: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00011a60: 706c 655b 665f 5d0a 2020 2020 2020 2020  ple[f_].        
+00011a70: 2020 2020 2020 2020 2020 2020 6d61 7070              mapp
+00011a80: 696e 672e 6170 7065 6e64 286d 6170 7069  ing.append(mappi
+00011a90: 6e67 5f29 0a20 2020 2020 2020 2020 2020  ng_).           
+00011aa0: 2020 2020 2020 2020 2064 6174 615f 7365           data_se
+00011ab0: 7420 3d20 6461 7461 5f73 6574 2069 6620  t = data_set if 
+00011ac0: 6461 7461 5f73 6574 2065 6c73 6520 6461  data_set else da
+00011ad0: 7461 5f73 6574 5f0a 2020 2020 2020 2020  ta_set_.        
+00011ae0: 2020 2020 2020 2020 2020 2020 7265 735f              res_
+00011af0: 736f 7274 203d 2072 6573 5f73 6f72 7420  sort = res_sort 
+00011b00: 6966 2072 6573 5f73 6f72 7420 656c 7365  if res_sort else
+00011b10: 2072 6573 5f73 6f72 745f 0a20 2020 2020   res_sort_.     
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00011b30: 7373 6572 7420 6461 7461 5f73 6574 203d  ssert data_set =
+00011b40: 3d20 6461 7461 5f73 6574 5f0a 2020 2020  = data_set_.    
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 6173 7365 7274 2072 6573 5f73 6f72 7420  assert res_sort 
+00011b70: 3d3d 2072 6573 5f73 6f72 745f 0a20 2020  == res_sort_.   
+00011b80: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00011b90: 696e 7374 616e 6365 2866 2c20 6469 6374  instance(f, dict
+00011ba0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011bb0: 2020 206d 6170 7069 6e67 203d 207b 6b3a     mapping = {k:
+00011bc0: 205b 5d20 666f 7220 6b20 696e 2066 2e6b   [] for k in f.k
+00011bd0: 6579 7328 297d 0a20 2020 2020 2020 2020  eys()}.         
+00011be0: 2020 2020 2020 2066 6f72 206b 2c20 665f         for k, f_
+00011bf0: 2069 6e20 662e 6974 656d 7328 293a 0a20   in f.items():. 
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 2020 2069 6620 665f 206e 6f74 2069 6e20     if f_ not in 
+00011c20: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
+00011c30: 7475 706c 653a 0a20 2020 2020 2020 2020  tuple:.         
+00011c40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011c50: 6f67 5f65 7272 6f72 286c 6f67 6765 722c  og_error(logger,
+00011c60: 2066 2246 6965 6c64 207b 665f 7d20 6e6f   f"Field {f_} no
+00011c70: 7420 666f 756e 6420 696e 2064 6174 6122  t found in data"
+00011c80: 2c20 4461 7461 4572 726f 7229 0a20 2020  , DataError).   
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 206d 6170 7069 6e67 5f2c 2064 6174 615f   mapping_, data_
+00011cb0: 7365 745f 2c20 7265 735f 736f 7274 5f20  set_, res_sort_ 
+00011cc0: 3d20 6461 7461 5f6d 6170 7069 6e67 5f74  = data_mapping_t
+00011cd0: 6f5f 7475 706c 655b 665f 5d0a 2020 2020  o_tuple[f_].    
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cf0: 6d61 7070 696e 675b 6b5d 203d 206d 6170  mapping[k] = map
+00011d00: 7069 6e67 5f0a 2020 2020 2020 2020 2020  ping_.          
+00011d10: 2020 2020 2020 2020 2020 6461 7461 5f73            data_s
+00011d20: 6574 203d 2064 6174 615f 7365 7420 6966  et = data_set if
+00011d30: 2064 6174 615f 7365 7420 656c 7365 2064   data_set else d
+00011d40: 6174 615f 7365 745f 0a20 2020 2020 2020  ata_set_.       
+00011d50: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00011d60: 5f73 6f72 7420 3d20 7265 735f 736f 7274  _sort = res_sort
+00011d70: 2069 6620 7265 735f 736f 7274 2065 6c73   if res_sort els
+00011d80: 6520 7265 735f 736f 7274 5f0a 2020 2020  e res_sort_.    
+00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011da0: 6173 7365 7274 2064 6174 615f 7365 7420  assert data_set 
+00011db0: 3d3d 2064 6174 615f 7365 745f 0a20 2020  == data_set_.   
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dd0: 2061 7373 6572 7420 7265 735f 736f 7274   assert res_sort
+00011de0: 203d 3d20 7265 735f 736f 7274 5f0a 2020   == res_sort_.  
+00011df0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
+00011e20: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011e30: 6f67 6765 722c 2066 2246 6965 6c64 207b  ogger, f"Field {
+00011e40: 667d 2069 7320 6e6f 7420 6120 7374 7269  f} is not a stri
+00011e50: 6e67 2c20 7475 706c 652c 206c 6973 7420  ng, tuple, list 
+00011e60: 6f72 2064 6963 7422 2c20 4461 7461 4572  or dict", DataEr
+00011e70: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+00011e80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00011e90: 2020 7461 736b 732e 6170 7065 6e64 280a    tasks.append(.
+00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011eb0: 7265 706f 7274 2e63 7265 6174 655f 7265  report.create_re
+00011ec0: 706f 7274 5f64 6174 615f 7365 7428 0a20  port_data_set(. 
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 206d 6170 7069 6e67 5f64 6174 615f     mapping_data_
+00011ef0: 7365 745f 736f 7274 3d28 6d61 7070 696e  set_sort=(mappin
+00011f00: 672c 2064 6174 615f 7365 742c 2072 6573  g, data_set, res
+00011f10: 5f73 6f72 7429 0a20 2020 2020 2020 2020  _sort).         
+00011f20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00011f30: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00011f40: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
+00011f50: 203d 2061 7761 6974 2061 7379 6e63 696f   = await asyncio
+00011f60: 2e67 6174 6865 7228 2a74 6173 6b73 290a  .gather(*tasks).
+00011f70: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00011f80: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00011f90: 2066 2243 7265 6174 6564 207b 6c65 6e28   f"Created {len(
+00011fa0: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
+00011fb0: 297d 2063 6f6d 706f 6e65 6e74 2064 6174  )} component dat
+00011fc0: 6120 7365 7420 6c69 6e6b 7320 666f 7220  a set links for 
+00011fd0: 636f 6d70 6f6e 656e 7420 7b73 7472 2872  component {str(r
+00011fe0: 6570 6f72 7429 7d22 0a20 2020 2020 2020  eport)}".       
+00011ff0: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+00012000: 6e20 7265 706f 7274 5f64 6174 615f 7365  n report_data_se
+00012010: 7473 0a0a 2020 2020 6465 6620 5f75 7064  ts..    def _upd
+00012020: 6174 655f 6f70 7469 6f6e 7328 7365 6c66  ate_options(self
+00012030: 2c20 6f70 7469 6f6e 733a 2064 6963 742c  , options: dict,
+00012040: 206f 7074 696f 6e5f 6d6f 6469 6669 6361   option_modifica
+00012050: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+00012060: 6469 6374 5d29 3a0a 2020 2020 2020 2020  dict]):.        
+00012070: 2222 2255 7064 6174 6520 7468 6520 6f70  """Update the op
+00012080: 7469 6f6e 7320 6f66 2061 6e20 6563 6861  tions of an echa
+00012090: 7274 2e0a 2020 2020 2020 2020 3a70 6172  rt..        :par
+000120a0: 616d 206f 7074 696f 6e73 3a20 7468 6520  am options: the 
+000120b0: 6f70 7469 6f6e 7320 6f66 2074 6865 2065  options of the e
+000120c0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
+000120d0: 6172 616d 206f 7074 696f 6e5f 6d6f 6469  aram option_modi
+000120e0: 6669 6361 7469 6f6e 733a 2074 6865 206d  fications: the m
+000120f0: 6f64 6966 6963 6174 696f 6e73 2074 6f20  odifications to 
+00012100: 6170 706c 7920 746f 2074 6865 206f 7074  apply to the opt
+00012110: 696f 6e73 0a20 2020 2020 2020 2022 2222  ions.        """
+00012120: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00012130: 6f70 7469 6f6e 5f6d 6f64 6966 6963 6174  option_modificat
+00012140: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00012150: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00012160: 2066 6f72 206b 2c20 7620 696e 206f 7074   for k, v in opt
+00012170: 696f 6e5f 6d6f 6469 6669 6361 7469 6f6e  ion_modification
+00012180: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+00012190: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
+000121a0: 7365 7269 6573 223a 0a20 2020 2020 2020  series":.       
+000121b0: 2020 2020 2020 2020 206c 6f67 5f65 7272           log_err
+000121c0: 6f72 286c 6f67 6765 722c 2022 5365 7269  or(logger, "Seri
+000121d0: 6573 2063 616e 6e6f 7420 6265 206d 6f64  es cannot be mod
+000121e0: 6966 6965 6422 2c20 4461 7461 4572 726f  ified", DataErro
+000121f0: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
+00012200: 6620 6b20 3d3d 2022 7841 7869 7322 206f  f k == "xAxis" o
+00012210: 7220 6b20 3d3d 2022 7941 7869 7322 3a0a  r k == "yAxis":.
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 6966 2069 7369 6e73 7461 6e63 6528 762c  if isinstance(v,
+00012240: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00012250: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
+00012260: 5b76 5d0a 2020 2020 2020 2020 2020 2020  [v].            
+00012270: 2020 2020 6966 206c 656e 2876 2920 213d      if len(v) !=
+00012280: 206c 656e 286f 7074 696f 6e73 5b6b 5d29   len(options[k])
+00012290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000122a0: 2020 2020 2020 6c6f 675f 6572 726f 7228        log_error(
+000122b0: 6c6f 6767 6572 2c20 6622 5468 6520 6e75  logger, f"The nu
+000122c0: 6d62 6572 206f 6620 7b6b 7d20 6d75 7374  mber of {k} must
+000122d0: 2062 6520 7b6c 656e 2876 297d 222c 2044   be {len(v)}", D
+000122e0: 6174 6145 7272 6f72 290a 2020 2020 2020  ataError).      
+000122f0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
+00012300: 2076 5f20 696e 2065 6e75 6d65 7261 7465   v_ in enumerate
+00012310: 2876 293a 0a20 2020 2020 2020 2020 2020  (v):.           
+00012320: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+00012330: 5b6b 5d5b 695d 2e75 7064 6174 6528 765f  [k][i].update(v_
+00012340: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00012350: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012360: 2020 2020 6f70 7469 6f6e 735b 6b5d 203d      options[k] =
+00012370: 2076 0a0a 2020 2020 6173 796e 6320 6465   v..    async de
+00012380: 6620 5f63 7265 6174 655f 6563 6861 7274  f _create_echart
+00012390: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000123a0: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
+000123b0: 2064 6963 742c 0a20 2020 2020 2020 206f   dict,.        o
+000123c0: 7264 6572 3a20 696e 742c 0a20 2020 2020  rder: int,.     
+000123d0: 2020 2066 6965 6c64 733a 206c 6973 745b     fields: list[
+000123e0: 556e 696f 6e5b 7374 722c 2074 7570 6c65  Union[str, tuple
+000123f0: 2c20 6469 6374 5d5d 2c0a 2020 2020 2020  , dict]],.      
+00012400: 2020 6461 7461 5f6d 6170 7069 6e67 5f74    data_mapping_t
+00012410: 6f5f 7475 706c 6573 3a20 4f70 7469 6f6e  o_tuples: Option
+00012420: 616c 5b64 6963 745d 203d 204e 6f6e 652c  al[dict] = None,
+00012430: 0a20 2020 2020 2020 2064 6174 613a 204f  .        data: O
+00012440: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+00012450: 722c 2070 642e 4461 7461 4672 616d 655d  r, pd.DataFrame]
+00012460: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00012470: 2020 6475 6d70 5f77 686f 6c65 3a20 626f    dump_whole: bo
+00012480: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00012490: 2020 2020 6f70 7469 6f6e 5f6d 6f64 6966      option_modif
+000124a0: 6963 6174 696f 6e73 3a20 4f70 7469 6f6e  ications: Option
+000124b0: 616c 5b64 6963 745d 203d 204e 6f6e 652c  al[dict] = None,
+000124c0: 0a20 2020 2020 2020 2074 6974 6c65 3a20  .        title: 
+000124d0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000124e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 726f  None,.        ro
+000124f0: 7773 5f73 697a 653a 204f 7074 696f 6e61  ws_size: Optiona
+00012500: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00012510: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
+00012520: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
+00012530: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00012540: 7061 6464 696e 673a 204f 7074 696f 6e61  padding: Optiona
+00012550: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00012560: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00012570: 220a 2020 2020 2020 2020 4372 6561 7465  ".        Create
+00012580: 2061 6e20 6563 6861 7274 2069 6e20 7468   an echart in th
+00012590: 6520 6461 7368 626f 6172 642c 2066 696c  e dashboard, fil
+000125a0: 6c20 696e 2074 6865 2064 6174 6120 7265  l in the data re
+000125b0: 6665 7265 6e63 6564 2069 6e20 7468 6520  ferenced in the 
+000125c0: 6563 6861 7274 5f6f 7074 696f 6e73 2061  echart_options a
+000125d0: 6e64 2063 7265 6174 6520 6f72 0a20 2020  nd create or.   
+000125e0: 2020 2020 2075 7064 6174 6520 7468 6520       update the 
+000125f0: 6368 6172 7420 616e 6420 6461 7461 2073  chart and data s
+00012600: 6574 206c 696e 6b73 2e0a 2020 2020 2020  et links..      
+00012610: 2020 3a70 6172 616d 206f 7074 696f 6e73    :param options
+00012620: 3a20 7468 6520 6f70 7469 6f6e 7320 6f66  : the options of
+00012630: 2074 6865 2065 6368 6172 740a 2020 2020   the echart.    
+00012640: 2020 2020 3a70 6172 616d 2064 6174 615f      :param data_
+00012650: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
+00012660: 733a 2074 6865 206d 6170 7069 6e67 206f  s: the mapping o
+00012670: 6620 7468 6520 6461 7461 2074 6f20 7468  f the data to th
+00012680: 6520 7475 706c 6573 0a20 2020 2020 2020  e tuples.       
+00012690: 203a 7061 7261 6d20 6461 7461 3a20 7468   :param data: th
+000126a0: 6520 6461 7461 206f 6620 7468 6520 6563  e data of the ec
+000126b0: 6861 7274 0a20 2020 2020 2020 203a 7061  hart.        :pa
+000126c0: 7261 6d20 6475 6d70 5f77 686f 6c65 3a20  ram dump_whole: 
+000126d0: 7768 6574 6865 7220 746f 2064 756d 7020  whether to dump 
+000126e0: 7468 6520 7768 6f6c 6520 6461 7461 0a20  the whole data. 
+000126f0: 2020 2020 2020 203a 7061 7261 6d20 6f70         :param op
+00012700: 7469 6f6e 5f6d 6f64 6966 6963 6174 696f  tion_modificatio
+00012710: 6e73 3a20 7468 6520 6d6f 6469 6669 6361  ns: the modifica
+00012720: 7469 6f6e 7320 746f 2061 7070 6c79 2074  tions to apply t
+00012730: 6f20 7468 6520 6f70 7469 6f6e 730a 2020  o the options.  
+00012740: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
+00012750: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
+00012760: 2074 6865 2065 6368 6172 740a 2020 2020   the echart.    
+00012770: 2020 2020 3a70 6172 616d 2072 6f77 735f      :param rows_
+00012780: 7369 7a65 3a20 7468 6520 726f 7773 2073  size: the rows s
+00012790: 697a 6520 6f66 2074 6865 2065 6368 6172  ize of the echar
+000127a0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+000127b0: 2063 6f6c 735f 7369 7a65 3a20 7468 6520   cols_size: the 
+000127c0: 636f 6c75 6d6e 7320 7369 7a65 206f 6620  columns size of 
+000127d0: 7468 6520 6563 6861 7274 0a20 2020 2020  the echart.     
+000127e0: 2020 203a 7061 7261 6d20 7061 6464 696e     :param paddin
+000127f0: 673a 2074 6865 2070 6164 6469 6e67 206f  g: the padding o
+00012800: 6620 7468 6520 6563 6861 7274 0a20 2020  f the echart.   
+00012810: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00012820: 2020 6966 2064 6174 6120 6973 206e 6f74    if data is not
+00012830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012840: 2020 2064 6174 615f 6d61 7070 696e 675f     data_mapping_
+00012850: 746f 5f74 7570 6c65 7320 3d20 6177 6169  to_tuples = awai
+00012860: 7420 7365 6c66 2e5f 6368 6f6f 7365 5f64  t self._choose_d
+00012870: 6174 6128 0a20 2020 2020 2020 2020 2020  ata(.           
+00012880: 2020 2020 206f 7264 6572 2c20 6461 7461       order, data
+00012890: 2c20 6475 6d70 5f77 686f 6c65 3d64 756d  , dump_whole=dum
+000128a0: 705f 7768 6f6c 650a 2020 2020 2020 2020  p_whole.        
+000128b0: 2020 2020 290a 0a20 2020 2020 2020 2064      )..        d
+000128c0: 6174 615f 6b65 795f 656e 7472 6965 7320  ata_key_entries 
+000128d0: 3d20 6765 745f 6461 7461 5f72 6566 6572  = get_data_refer
+000128e0: 656e 6365 735f 6672 6f6d 5f64 6963 7428  ences_from_dict(
+000128f0: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
+00012900: 205f 2c20 7265 706f 7274 203d 2061 7761   _, report = awa
+00012910: 6974 2073 656c 662e 5f67 6574 5f63 6861  it self._get_cha
+00012920: 7274 5f72 6570 6f72 7428 6f72 6465 722c  rt_report(order,
+00012930: 2045 4368 6172 7429 0a0a 2020 2020 2020   EChart)..      
+00012940: 2020 7264 5f69 6473 203d 204e 6f6e 650a    rd_ids = None.
+00012950: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012960: 7265 7573 655f 6461 7461 5f73 6574 733a  reuse_data_sets:
+00012970: 0a20 2020 2020 2020 2020 2020 2072 645f  .            rd_
+00012980: 6964 7320 3d20 6765 745f 7575 6964 735f  ids = get_uuids_
+00012990: 6672 6f6d 5f64 6963 7428 7265 706f 7274  from_dict(report
+000129a0: 5b22 7072 6f70 6572 7469 6573 225d 5b22  ["properties"]["
+000129b0: 6f70 7469 6f6e 225d 290a 2020 2020 2020  option"]).      
+000129c0: 2020 2020 2020 6966 206c 656e 2872 645f        if len(rd_
+000129d0: 6964 7329 203d 3d20 6c65 6e28 6669 656c  ids) == len(fiel
+000129e0: 6473 293a 0a20 2020 2020 2020 2020 2020  ds):.           
+000129f0: 2020 2020 2072 6570 5f64 733a 206c 6973       rep_ds: lis
+00012a00: 745b 5265 706f 7274 2e52 6570 6f72 7444  t[Report.ReportD
+00012a10: 6174 6153 6574 5d20 3d20 6177 6169 7420  ataSet] = await 
+00012a20: 7265 706f 7274 2e67 6574 5f72 6570 6f72  report.get_repor
+00012a30: 745f 6461 7461 5f73 6574 7328 290a 2020  t_data_sets().  
+00012a40: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00012a50: 7070 6564 5f66 203d 205b 0a20 2020 2020  pped_f = [.     
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012a70: 656c 662e 5f67 6574 5f66 6965 6c64 5f6d  elf._get_field_m
+00012a80: 6170 7069 6e67 2866 6965 6c64 2c20 6461  apping(field, da
+00012a90: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00012aa0: 706c 6573 290a 2020 2020 2020 2020 2020  ples).          
+00012ab0: 2020 2020 2020 2020 2020 666f 7220 6669            for fi
+00012ac0: 656c 6420 696e 2066 6965 6c64 730a 2020  eld in fields.  
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 666f 7220 692c 2072 645f 6964 2069 6e20  for i, rd_id in 
+00012b00: 656e 756d 6572 6174 6528 7264 5f69 6473  enumerate(rd_ids
+00012b10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012b20: 2020 2020 2020 2072 6570 6f72 745f 6461         report_da
+00012b30: 7461 5f73 6574 203d 206e 6578 7428 0a20  ta_set = next(. 
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 2020 2020 2020 2028 7264 2066 6f72 2072         (rd for r
+00012b60: 6420 696e 2072 6570 5f64 7320 6966 2072  d in rep_ds if r
+00012b70: 645b 2269 6422 5d20 3d3d 2072 645f 6964  d["id"] == rd_id
+00012b80: 292c 204e 6f6e 650a 2020 2020 2020 2020  ), None.        
+00012b90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2072 6570 6f72 745f 6461 7461 5f73     report_data_s
-00012bc0: 6574 2c20 6d61 7070 6564 5f66 5b69 5d0a  et, mapped_f[i].
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012be0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012bf0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00012c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c10: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
-00012c20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00012c40: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-00012c50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00012c60: 2020 2020 2020 2072 645f 6964 7320 3d20         rd_ids = 
-00012c70: 4e6f 6e65 0a0a 2020 2020 2020 2020 6966  None..        if
-00012c80: 206e 6f74 2072 645f 6964 733a 0a20 2020   not rd_ids:.   
-00012c90: 2020 2020 2020 2020 2061 7761 6974 2072           await r
-00012ca0: 6570 6f72 742e 6465 6c65 7465 5f72 6570  eport.delete_rep
-00012cb0: 6f72 745f 6461 7461 5f73 6574 7328 6c6f  ort_data_sets(lo
-00012cc0: 673d 5472 7565 290a 2020 2020 2020 2020  g=True).        
-00012cd0: 2020 2020 7265 706f 7274 5f64 6174 615f      report_data_
-00012ce0: 7365 7473 203d 2061 7761 6974 2073 656c  sets = await sel
-00012cf0: 662e 5f67 6574 5f72 6570 6f72 745f 6461  f._get_report_da
-00012d00: 7461 5f73 6574 735f 7065 725f 6d61 7070  ta_sets_per_mapp
-00012d10: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00012d20: 2020 2020 2072 6570 6f72 742c 2064 6174       report, dat
-00012d30: 615f 6d61 7070 696e 675f 746f 5f74 7570  a_mapping_to_tup
-00012d40: 6c65 732c 2066 6965 6c64 730a 2020 2020  les, fields.    
-00012d50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00012d60: 2020 2020 2020 7264 5f69 6473 203d 205b        rd_ids = [
-00012d70: 7264 5b22 6964 225d 2066 6f72 2072 6420  rd["id"] for rd 
-00012d80: 696e 2072 6570 6f72 745f 6461 7461 5f73  in report_data_s
-00012d90: 6574 735d 0a0a 2020 2020 2020 2020 7365  ets]..        se
-00012da0: 6c66 2e5f 7570 6461 7465 5f6f 7074 696f  lf._update_optio
-00012db0: 6e73 286f 7074 696f 6e73 2c20 6f70 7469  ns(options, opti
-00012dc0: 6f6e 5f6d 6f64 6966 6963 6174 696f 6e73  on_modifications
-00012dd0: 290a 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
-00012de0: 6e28 7264 5f69 6473 2920 213d 206c 656e  n(rd_ids) != len
-00012df0: 2864 6174 615f 6b65 795f 656e 7472 6965  (data_key_entrie
-00012e00: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00012e10: 6c6f 675f 6572 726f 7228 0a20 2020 2020  log_error(.     
-00012e20: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00012e30: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-00012e40: 2020 2066 2254 6865 206e 756d 6265 7220     f"The number 
-00012e50: 6f66 2064 6174 6120 7265 6665 7265 6e63  of data referenc
-00012e60: 6573 2061 6e64 2066 6965 6c64 7320 6d75  es and fields mu
-00012e70: 7374 2062 6520 6571 7561 6c2c 2022 0a20  st be equal, ". 
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012e90: 2274 6865 7920 6172 6520 7b6c 656e 2864  "they are {len(d
-00012ea0: 6174 615f 6b65 795f 656e 7472 6965 7329  ata_key_entries)
-00012eb0: 7d20 616e 6420 7b6c 656e 2872 645f 6964  } and {len(rd_id
-00012ec0: 7329 7d20 7265 7370 6563 7469 7665 6c79  s)} respectively
-00012ed0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00012ee0: 2020 2020 4461 7461 4572 726f 722c 0a20      DataError,. 
-00012ef0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00012f00: 2020 2020 2020 666f 7220 692c 2064 6174        for i, dat
-00012f10: 615f 6b65 795f 656e 7472 7920 696e 2065  a_key_entry in e
-00012f20: 6e75 6d65 7261 7465 2864 6174 615f 6b65  numerate(data_ke
-00012f30: 795f 656e 7472 6965 7329 3a0a 2020 2020  y_entries):.    
-00012f40: 2020 2020 2020 2020 6461 7461 203d 206f          data = o
-00012f50: 7074 696f 6e73 0a20 2020 2020 2020 2020  ptions.         
-00012f60: 2020 2066 6f72 206b 6579 2069 6e20 6461     for key in da
-00012f70: 7461 5f6b 6579 5f65 6e74 7279 5b3a 2d31  ta_key_entry[:-1
-00012f80: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00012f90: 2020 2064 6174 6120 3d20 6461 7461 5b6b     data = data[k
-00012fa0: 6579 5d0a 2020 2020 2020 2020 2020 2020  ey].            
-00012fb0: 6461 7461 5b64 6174 615f 6b65 795f 656e  data[data_key_en
-00012fc0: 7472 795b 2d31 5d5d 203d 2022 237b 2220  try[-1]] = "#{" 
-00012fd0: 2b20 7264 5f69 6473 5b69 5d20 2b20 227d  + rd_ids[i] + "}
-00012fe0: 220a 0a20 2020 2020 2020 2061 7761 6974  "..        await
-00012ff0: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
-00013000: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
-00013010: 2063 6861 7274 5f63 6c61 7373 3d45 4368   chart_class=ECh
-00013020: 6172 742c 0a20 2020 2020 2020 2020 2020  art,.           
-00013030: 2070 726f 7065 7274 6965 733d 7b22 6f70   properties={"op
-00013040: 7469 6f6e 223a 206f 7074 696f 6e73 7d2c  tion": options},
-00013050: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
-00013060: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
-00013070: 2020 2020 2020 7469 746c 653d 7469 746c        title=titl
-00013080: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
-00013090: 697a 6550 6164 6469 6e67 3d70 6164 6469  izePadding=paddi
-000130a0: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-000130b0: 7369 7a65 526f 7773 3d72 6f77 735f 7369  sizeRows=rows_si
-000130c0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-000130d0: 7369 7a65 436f 6c75 6d6e 733d 636f 6c73  sizeColumns=cols
-000130e0: 5f73 697a 652c 0a20 2020 2020 2020 2029  _size,.        )
-000130f0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00013100: 686f 640a 2020 2020 6465 6620 5f61 7070  hod.    def _app
-00013110: 6c79 5f76 6172 6961 6e74 2865 6368 6172  ly_variant(echar
-00013120: 745f 6f70 7469 6f6e 733a 2064 6963 742c  t_options: dict,
-00013130: 2076 6172 6961 6e74 3a20 4f70 7469 6f6e   variant: Option
-00013140: 616c 5b73 7472 5d29 3a0a 2020 2020 2020  al[str]):.      
-00013150: 2020 6966 2076 6172 6961 6e74 203d 3d20    if variant == 
-00013160: 2263 6c65 616e 223a 0a20 2020 2020 2020  "clean":.       
-00013170: 2020 2020 2065 6368 6172 745f 6f70 7469       echart_opti
-00013180: 6f6e 732e 7570 6461 7465 280a 2020 2020  ons.update(.    
-00013190: 2020 2020 2020 2020 2020 2020 7b22 746f              {"to
-000131a0: 6f6c 626f 7822 3a20 7b22 7368 6f77 223a  olbox": {"show":
-000131b0: 2046 616c 7365 7d2c 2022 6c65 6765 6e64   False}, "legend
-000131c0: 223a 207b 2273 686f 7722 3a20 4661 6c73  ": {"show": Fals
-000131d0: 657d 2c20 2267 7269 6422 3a20 7b7d 7d0a  e}, "grid": {}}.
-000131e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000131f0: 2020 2020 2020 2020 2020 666f 7220 6178            for ax
-00013200: 6973 6c69 7374 2069 6e20 5b65 6368 6172  islist in [echar
-00013210: 745f 6f70 7469 6f6e 735b 2278 4178 6973  t_options["xAxis
-00013220: 225d 2c20 6563 6861 7274 5f6f 7074 696f  "], echart_optio
-00013230: 6e73 5b22 7941 7869 7322 5d5d 3a0a 2020  ns["yAxis"]]:.  
-00013240: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00013250: 7220 6178 6973 2069 6e20 6178 6973 6c69  r axis in axisli
-00013260: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-00013270: 2020 2020 2020 2020 6178 6973 2e75 7064          axis.upd
-00013280: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
-00013290: 2020 2020 2020 2020 2020 2020 207b 2261               {"a
-000132a0: 7869 734c 696e 6522 3a20 7b22 7368 6f77  xisLine": {"show
-000132b0: 223a 2046 616c 7365 7d2c 2022 6178 6973  ": False}, "axis
-000132c0: 5469 636b 223a 207b 2273 686f 7722 3a20  Tick": {"show": 
-000132d0: 4661 6c73 657d 7d0a 2020 2020 2020 2020  False}}.        
-000132e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000132f0: 2020 2020 2020 656c 6966 2076 6172 6961        elif varia
-00013300: 6e74 203d 3d20 226d 696e 696d 616c 223a  nt == "minimal":
-00013310: 0a20 2020 2020 2020 2020 2020 2065 6368  .            ech
-00013320: 6172 745f 6f70 7469 6f6e 732e 7570 6461  art_options.upda
-00013330: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-00013340: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00013350: 2020 2020 2020 2020 2020 2274 6f6f 6c62            "toolb
-00013360: 6f78 223a 207b 2273 686f 7722 3a20 4661  ox": {"show": Fa
-00013370: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
-00013380: 2020 2020 2020 2020 2020 226c 6567 656e            "legen
-00013390: 6422 3a20 7b22 7368 6f77 223a 2046 616c  d": {"show": Fal
-000133a0: 7365 7d2c 0a20 2020 2020 2020 2020 2020  se},.           
-000133b0: 2020 2020 2020 2020 2022 6772 6964 223a           "grid":
-000133c0: 207b 226c 6566 7422 3a20 2231 2522 2c20   {"left": "1%", 
-000133d0: 2272 6967 6874 223a 2022 3125 222c 2022  "right": "1%", "
-000133e0: 746f 7022 3a20 2231 2522 2c20 2262 6f74  top": "1%", "bot
-000133f0: 746f 6d22 3a20 2231 2522 7d2c 0a20 2020  tom": "1%"},.   
-00013400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013410: 2022 746f 6f6c 7469 7022 3a20 7b22 7368   "tooltip": {"sh
-00013420: 6f77 223a 2046 616c 7365 7d2c 0a20 2020  ow": False},.   
-00013430: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00013440: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00013450: 2020 2020 2020 2020 2066 6f72 2061 7869           for axi
-00013460: 736c 6973 7420 696e 205b 6563 6861 7274  slist in [echart
-00013470: 5f6f 7074 696f 6e73 5b22 7841 7869 7322  _options["xAxis"
-00013480: 5d2c 2065 6368 6172 745f 6f70 7469 6f6e  ], echart_option
-00013490: 735b 2279 4178 6973 225d 5d3a 0a20 2020  s["yAxis"]]:.   
-000134a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000134b0: 2061 7869 7320 696e 2061 7869 736c 6973   axis in axislis
-000134c0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000134d0: 2020 2020 2020 2061 7869 732e 7570 6461         axis.upda
-000134e0: 7465 280a 2020 2020 2020 2020 2020 2020  te(.            
-000134f0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013510: 2020 2020 2020 2020 2020 2261 7869 734c            "axisL
-00013520: 696e 6522 3a20 7b22 7368 6f77 223a 2046  ine": {"show": F
-00013530: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 2020 2022 6178 6973 5469 636b 223a 207b     "axisTick": {
-00013560: 2273 686f 7722 3a20 4661 6c73 657d 2c0a  "show": False},.
-00013570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013580: 2020 2020 2020 2020 2020 2020 2273 706c              "spl
-00013590: 6974 4c69 6e65 223a 207b 2273 686f 7722  itLine": {"show"
-000135a0: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
-000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135c0: 2020 2020 2020 2261 7869 734c 6162 656c        "axisLabel
-000135d0: 223a 207b 2273 686f 7722 3a20 4661 6c73  ": {"show": Fals
-000135e0: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
-000135f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013610: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-00013620: 6566 205f 6372 6561 7465 5f74 7265 6e64  ef _create_trend
-00013630: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
-00013640: 7365 6c66 2c0a 2020 2020 2020 2020 6178  self,.        ax
-00013650: 6573 3a20 556e 696f 6e5b 6c69 7374 5b73  es: Union[list[s
-00013660: 7472 5d2c 2073 7472 5d2c 0a20 2020 2020  tr], str],.     
-00013670: 2020 206f 7264 6572 3a20 696e 742c 0a20     order: int,. 
-00013680: 2020 2020 2020 2064 6174 615f 6d61 7070         data_mapp
-00013690: 696e 675f 746f 5f74 7570 6c65 733a 204f  ing_to_tuples: O
-000136a0: 7074 696f 6e61 6c5b 6469 6374 5d2c 0a20  ptional[dict],. 
-000136b0: 2020 2020 2020 2065 6368 6172 745f 6f70         echart_op
-000136c0: 7469 6f6e 733a 2064 6963 742c 0a20 2020  tions: dict,.   
-000136d0: 2020 2020 2073 6572 6965 735f 6f70 7469       series_opti
-000136e0: 6f6e 733a 2055 6e69 6f6e 5b64 6963 742c  ons: Union[dict,
-000136f0: 206c 6973 745b 6469 6374 5d5d 2c0a 2020   list[dict]],.  
-00013700: 2020 2020 2020 7661 6c75 6573 3a20 4f70        values: Op
-00013710: 7469 6f6e 616c 5b55 6e69 6f6e 5b6c 6973  tional[Union[lis
-00013720: 745b 556e 696f 6e5b 7374 722c 2074 7570  t[Union[str, tup
-00013730: 6c65 5d5d 2c20 7374 722c 2074 7570 6c65  le]], str, tuple
-00013740: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00013750: 2020 2078 5f61 7869 735f 6e61 6d65 733a     x_axis_names:
-00013760: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
-00013770: 7374 722c 206c 6973 745b 7374 725d 5d5d  str, list[str]]]
-00013780: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00013790: 2079 5f61 7869 735f 6e61 6d65 733a 204f   y_axis_names: O
-000137a0: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
-000137b0: 722c 206c 6973 745b 7374 725d 5d5d 203d  r, list[str]]] =
-000137c0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-000137d0: 686f 775f 7661 6c75 6573 3a20 4f70 7469  how_values: Opti
-000137e0: 6f6e 616c 5b55 6e69 6f6e 5b6c 6973 745b  onal[Union[list[
-000137f0: 7374 725d 2c20 7374 725d 5d20 3d20 4e6f  str], str]] = No
-00013800: 6e65 2c0a 2020 2020 2020 2020 7661 7269  ne,.        vari
-00013810: 616e 743a 204f 7074 696f 6e61 6c5b 7374  ant: Optional[st
-00013820: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00013830: 2020 202a 2a72 6570 6f72 745f 7061 7261     **report_para
-00013840: 6d73 2c0a 2020 2020 293a 0a20 2020 2020  ms,.    ):.     
-00013850: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00013860: 7265 6174 6520 6120 6c69 6e65 2063 6861  reate a line cha
-00013870: 7274 2069 6e20 7468 6520 6461 7368 626f  rt in the dashbo
-00013880: 6172 642e 0a20 2020 2020 2020 203a 7061  ard..        :pa
-00013890: 7261 6d20 6461 7461 3a20 7468 6520 6461  ram data: the da
-000138a0: 7461 206f 6620 7468 6520 6368 6172 740a  ta of the chart.
-000138b0: 2020 2020 2020 2020 3a70 6172 616d 2061          :param a
-000138c0: 7865 733a 2074 6865 206e 616d 6573 206f  xes: the names o
-000138d0: 6620 7468 6520 636f 6c75 6d6e 7320 746f  f the columns to
-000138e0: 2062 6520 7573 6564 2061 7320 6178 6973   be used as axis
-000138f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00013900: 7661 6c75 6573 3a20 7468 6520 6e61 6d65  values: the name
-00013910: 7320 6f66 2074 6865 2063 6f6c 756d 6e73  s of the columns
-00013920: 2074 6f20 6265 2075 7365 6420 6173 2076   to be used as v
-00013930: 616c 7565 730a 2020 2020 2020 2020 3a70  alues.        :p
-00013940: 6172 616d 2078 5f61 7869 735f 6e61 6d65  aram x_axis_name
-00013950: 733a 2074 6865 206e 616d 6520 6f66 2074  s: the name of t
-00013960: 6865 2078 2061 7865 730a 2020 2020 2020  he x axes.      
-00013970: 2020 3a70 6172 616d 2079 5f61 7869 735f    :param y_axis_
-00013980: 6e61 6d65 733a 2074 6865 206e 616d 6520  names: the name 
-00013990: 6f66 2074 6865 2079 2061 7865 730a 2020  of the y axes.  
-000139a0: 2020 2020 2020 3a70 6172 616d 2065 6368        :param ech
-000139b0: 6172 745f 6f70 7469 6f6e 733a 2074 6865  art_options: the
-000139c0: 206f 7074 696f 6e73 206f 6620 7468 6520   options of the 
-000139d0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
-000139e0: 6172 616d 2073 6572 6965 735f 6f70 7469  aram series_opti
-000139f0: 6f6e 733a 2074 6865 206f 7074 696f 6e73  ons: the options
-00013a00: 206f 6620 7468 6520 7365 7269 6573 206f   of the series o
-00013a10: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
-00013a20: 2020 2020 3a70 6172 616d 2062 6f74 746f      :param botto
-00013a30: 6d5f 746f 6f6c 626f 783a 2077 6865 7468  m_toolbox: wheth
-00013a40: 6572 2074 6f20 7368 6f77 2074 6865 2074  er to show the t
-00013a50: 6f6f 6c62 6f78 206f 6e20 746f 7020 6f66  oolbox on top of
-00013a60: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-00013a70: 2020 203a 7061 7261 6d20 6f72 6465 723a     :param order:
-00013a80: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
-00013a90: 6520 6368 6172 7420 696e 2074 6865 2064  e chart in the d
-00013aa0: 6173 6862 6f61 7264 0a20 2020 2020 2020  ashboard.       
-00013ab0: 203a 7061 7261 6d20 7265 706f 7274 5f70   :param report_p
-00013ac0: 6172 616d 733a 2061 6464 6974 696f 6e61  arams: additiona
-00013ad0: 6c20 7265 706f 7274 2070 6172 616d 6574  l report paramet
-00013ae0: 6572 7320 6173 206b 6579 2d76 616c 7565  ers as key-value
-00013af0: 2070 6169 7273 0a20 2020 2020 2020 2022   pairs.        "
-00013b00: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00013b10: 5f61 7070 6c79 5f76 6172 6961 6e74 2865  _apply_variant(e
-00013b20: 6368 6172 745f 6f70 7469 6f6e 732c 2076  chart_options, v
-00013b30: 6172 6961 6e74 290a 2020 2020 2020 2020  ariant).        
-00013b40: 6966 2069 7369 6e73 7461 6e63 6528 6178  if isinstance(ax
-00013b50: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
-00013b60: 2020 2020 2020 6178 6573 203d 205b 6178        axes = [ax
-00013b70: 6573 5d0a 2020 2020 2020 2020 6966 2069  es].        if i
-00013b80: 7369 6e73 7461 6e63 6528 7661 6c75 6573  sinstance(values
-00013b90: 2c20 7374 7229 206f 7220 6973 696e 7374  , str) or isinst
-00013ba0: 616e 6365 2876 616c 7565 732c 2074 7570  ance(values, tup
-00013bb0: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-00013bc0: 2076 616c 7565 7320 3d20 5b76 616c 7565   values = [value
-00013bd0: 735d 0a20 2020 2020 2020 2069 6620 7368  s].        if sh
-00013be0: 6f77 5f76 616c 7565 7320 6973 204e 6f6e  ow_values is Non
-00013bf0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00013c00: 686f 775f 7661 6c75 6573 203d 205b 5d0a  how_values = [].
-00013c10: 0a20 2020 2020 2020 2069 6620 2278 5f61  .        if "x_a
-00013c20: 7869 735f 6e61 6d65 2220 696e 2072 6570  xis_name" in rep
-00013c30: 6f72 745f 7061 7261 6d73 3a0a 2020 2020  ort_params:.    
-00013c40: 2020 2020 2020 2020 785f 6178 6973 5f6e          x_axis_n
-00013c50: 616d 6573 203d 205b 7265 706f 7274 5f70  ames = [report_p
-00013c60: 6172 616d 735b 2278 5f61 7869 735f 6e61  arams["x_axis_na
-00013c70: 6d65 225d 5d0a 2020 2020 2020 2020 656c  me"]].        el
-00013c80: 6966 2069 7369 6e73 7461 6e63 6528 785f  if isinstance(x_
-00013c90: 6178 6973 5f6e 616d 6573 2c20 7374 7229  axis_names, str)
-00013ca0: 3a0a 2020 2020 2020 2020 2020 2020 785f  :.            x_
-00013cb0: 6178 6973 5f6e 616d 6573 203d 205b 785f  axis_names = [x_
-00013cc0: 6178 6973 5f6e 616d 6573 5d0a 2020 2020  axis_names].    
-00013cd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013ce0: 2020 2020 2020 785f 6178 6973 5f6e 616d        x_axis_nam
-00013cf0: 6573 203d 205b 5d0a 0a20 2020 2020 2020  es = []..       
-00013d00: 2069 6620 2279 5f61 7869 735f 6e61 6d65   if "y_axis_name
-00013d10: 2220 696e 2072 6570 6f72 745f 7061 7261  " in report_para
-00013d20: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00013d30: 795f 6178 6973 5f6e 616d 6573 203d 205b  y_axis_names = [
-00013d40: 7265 706f 7274 5f70 6172 616d 735b 2279  report_params["y
-00013d50: 5f61 7869 735f 6e61 6d65 225d 5d0a 2020  _axis_name"]].  
-00013d60: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00013d70: 7461 6e63 6528 795f 6178 6973 5f6e 616d  tance(y_axis_nam
-00013d80: 6573 2c20 7374 7229 3a0a 2020 2020 2020  es, str):.      
-00013d90: 2020 2020 2020 795f 6178 6973 5f6e 616d        y_axis_nam
-00013da0: 6573 203d 205b 795f 6178 6973 5f6e 616d  es = [y_axis_nam
-00013db0: 6573 5d0a 2020 2020 2020 2020 656c 7365  es].        else
-00013dc0: 3a0a 2020 2020 2020 2020 2020 2020 795f  :.            y_
-00013dd0: 6178 6973 5f6e 616d 6573 203d 205b 5d0a  axis_names = [].
-00013de0: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
-00013df0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00013e00: 5b76 2066 6f72 2076 2069 6e20 6461 7461  [v for v in data
-00013e10: 5f6d 6170 7069 6e67 5f74 6f5f 7475 706c  _mapping_to_tupl
-00013e20: 6573 2e6b 6579 7328 2920 6966 2076 206e  es.keys() if v n
-00013e30: 6f74 2069 6e20 6178 6573 5d0a 2020 2020  ot in axes].    
-00013e40: 2020 2020 2020 2020 6966 2076 616c 7565          if value
-00013e50: 7320 6973 204e 6f6e 650a 2020 2020 2020  s is None.      
-00013e60: 2020 2020 2020 656c 7365 2076 616c 7565        else value
-00013e70: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
-00013e80: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00013e90: 6528 7365 7269 6573 5f6f 7074 696f 6e73  e(series_options
-00013ea0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-00013eb0: 2020 2020 2073 6572 6965 735f 6f70 7469       series_opti
-00013ec0: 6f6e 7320 3d20 5b73 6572 6965 735f 6f70  ons = [series_op
-00013ed0: 7469 6f6e 735d 202a 206c 656e 2876 616c  tions] * len(val
-00013ee0: 7565 7329 0a20 2020 2020 2020 2065 6c69  ues).        eli
-00013ef0: 6620 6c65 6e28 7365 7269 6573 5f6f 7074  f len(series_opt
-00013f00: 696f 6e73 2920 3c20 6c65 6e28 7661 6c75  ions) < len(valu
-00013f10: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
-00013f20: 2073 6572 6965 735f 6f70 7469 6f6e 7320   series_options 
-00013f30: 3d20 7365 7269 6573 5f6f 7074 696f 6e73  = series_options
-00013f40: 202b 205b 7365 7269 6573 5f6f 7074 696f   + [series_optio
-00013f50: 6e73 5b2d 315d 5d20 2a20 280a 2020 2020  ns[-1]] * (.    
-00013f60: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-00013f70: 7661 6c75 6573 2920 2d20 6c65 6e28 7365  values) - len(se
-00013f80: 7269 6573 5f6f 7074 696f 6e73 290a 2020  ries_options).  
-00013f90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00013fa0: 2020 2020 656c 6966 206c 656e 2873 6572      elif len(ser
-00013fb0: 6965 735f 6f70 7469 6f6e 7329 203e 206c  ies_options) > l
-00013fc0: 656e 2876 616c 7565 7329 3a0a 2020 2020  en(values):.    
-00013fd0: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
-00013fe0: 7074 696f 6e73 203d 2073 6572 6965 735f  ptions = series_
-00013ff0: 6f70 7469 6f6e 735b 3a20 6c65 6e28 7661  options[: len(va
-00014000: 6c75 6573 295d 0a0a 2020 2020 2020 2020  lues)]..        
-00014010: 6563 6861 7274 5f6f 7074 696f 6e73 5b22  echart_options["
-00014020: 7365 7269 6573 225d 203d 205b 0a20 2020  series"] = [.   
-00014030: 2020 2020 2020 2020 2064 6565 705f 7570           deep_up
-00014040: 6461 7465 280a 2020 2020 2020 2020 2020  date(.          
-00014050: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00014060: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00014070: 6522 3a20 6e61 6d65 2069 6620 6973 696e  e": name if isin
-00014080: 7374 616e 6365 286e 616d 652c 2073 7472  stance(name, str
-00014090: 2920 656c 7365 2022 20c3 9720 222e 6a6f  ) else " .. ".jo
-000140a0: 696e 286e 616d 6529 2c0a 2020 2020 2020  in(name),.      
-000140b0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-000140c0: 6162 656c 223a 207b 2273 686f 7722 3a20  abel": {"show": 
-000140d0: 7368 6f77 5f76 616c 7565 7320 3d3d 2022  show_values == "
-000140e0: 616c 6c22 206f 7220 6e61 6d65 2069 6e20  all" or name in 
-000140f0: 7368 6f77 5f76 616c 7565 737d 2c0a 2020  show_values},.  
-00014100: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00014110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014120: 2073 6572 6965 735f 6f70 7469 6f6e 735b   series_options[
-00014130: 695d 2c0a 2020 2020 2020 2020 2020 2020  i],.            
-00014140: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-00014150: 7220 692c 206e 616d 6520 696e 2065 6e75  r i, name in enu
-00014160: 6d65 7261 7465 2876 616c 7565 7329 0a20  merate(values). 
-00014170: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00014180: 2020 666f 7220 692c 2061 7869 735f 6f70    for i, axis_op
-00014190: 7469 6f6e 7320 696e 2065 6e75 6d65 7261  tions in enumera
-000141a0: 7465 2865 6368 6172 745f 6f70 7469 6f6e  te(echart_option
-000141b0: 735b 2278 4178 6973 225d 293a 0a20 2020  s["xAxis"]):.   
-000141c0: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
-000141d0: 7469 6f6e 735b 226e 616d 6522 5d20 3d20  tions["name"] = 
-000141e0: 785f 6178 6973 5f6e 616d 6573 5b69 5d20  x_axis_names[i] 
-000141f0: 6966 2069 203c 206c 656e 2878 5f61 7869  if i < len(x_axi
-00014200: 735f 6e61 6d65 7329 2065 6c73 6520 4e6f  s_names) else No
-00014210: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-00014220: 6620 6178 6973 5f6f 7074 696f 6e73 5b22  f axis_options["
-00014230: 6e61 6d65 225d 2061 6e64 2022 6e61 6d65  name"] and "name
-00014240: 4761 7022 206e 6f74 2069 6e20 6178 6973  Gap" not in axis
-00014250: 5f6f 7074 696f 6e73 3a0a 2020 2020 2020  _options:.      
-00014260: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
-00014270: 7074 696f 6e73 5b22 6e61 6d65 4761 7022  ptions["nameGap"
-00014280: 5d20 3d20 3332 0a0a 2020 2020 2020 2020  ] = 32..        
-00014290: 666f 7220 692c 2061 7869 735f 6f70 7469  for i, axis_opti
-000142a0: 6f6e 7320 696e 2065 6e75 6d65 7261 7465  ons in enumerate
-000142b0: 2865 6368 6172 745f 6f70 7469 6f6e 735b  (echart_options[
-000142c0: 2279 4178 6973 225d 293a 0a20 2020 2020  "yAxis"]):.     
-000142d0: 2020 2020 2020 2061 7869 735f 6f70 7469         axis_opti
-000142e0: 6f6e 735b 226e 616d 6522 5d20 3d20 795f  ons["name"] = y_
-000142f0: 6178 6973 5f6e 616d 6573 5b69 5d20 6966  axis_names[i] if
-00014300: 2069 203c 206c 656e 2879 5f61 7869 735f   i < len(y_axis_
-00014310: 6e61 6d65 7329 2065 6c73 6520 4e6f 6e65  names) else None
-00014320: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014330: 6178 6973 5f6f 7074 696f 6e73 5b22 6e61  axis_options["na
-00014340: 6d65 225d 2061 6e64 2022 6e61 6d65 4761  me"] and "nameGa
-00014350: 7022 206e 6f74 2069 6e20 6178 6973 5f6f  p" not in axis_o
-00014360: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-00014370: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
-00014380: 696f 6e73 5b22 6e61 6d65 4761 7022 5d20  ions["nameGap"] 
-00014390: 3d20 2d32 340a 2020 2020 2020 2020 2020  = -24.          
-000143a0: 2020 2020 2020 6178 6973 5f6f 7074 696f        axis_optio
-000143b0: 6e73 5b22 6f66 6673 6574 225d 203d 2033  ns["offset"] = 3
-000143c0: 360a 2020 2020 2020 2020 2020 2020 2020  6.              
-000143d0: 2020 6563 6861 7274 5f6f 7074 696f 6e73    echart_options
-000143e0: 5b22 6772 6964 225d 5b22 6c65 6674 225d  ["grid"]["left"]
-000143f0: 203d 2022 3425 220a 2020 2020 2020 2020   = "4%".        
-00014400: 2020 2020 2020 2020 6178 6973 5f6f 7074          axis_opt
-00014410: 696f 6e73 5b22 6178 6973 5469 636b 225d  ions["axisTick"]
-00014420: 203d 207b 2273 686f 7722 3a20 4661 6c73   = {"show": Fals
-00014430: 657d 0a20 2020 2020 2020 2020 2020 2020  e}.             
-00014440: 2020 2061 7869 735f 6f70 7469 6f6e 735b     axis_options[
-00014450: 2261 7869 734c 696e 6522 5d20 3d20 7b22  "axisLine"] = {"
-00014460: 7368 6f77 223a 2046 616c 7365 7d0a 0a20  show": False}.. 
-00014470: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
-00014480: 662e 5f63 7265 6174 655f 6563 6861 7274  f._create_echart
-00014490: 280a 2020 2020 2020 2020 2020 2020 6f72  (.            or
-000144a0: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
-000144b0: 2020 2020 2020 206f 7074 696f 6e73 3d65         options=e
-000144c0: 6368 6172 745f 6f70 7469 6f6e 732c 0a20  chart_options,. 
-000144d0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000144e0: 6d61 7070 696e 675f 746f 5f74 7570 6c65  mapping_to_tuple
-000144f0: 733d 6461 7461 5f6d 6170 7069 6e67 5f74  s=data_mapping_t
-00014500: 6f5f 7475 706c 6573 2c0a 2020 2020 2020  o_tuples,.      
-00014510: 2020 2020 2020 6669 656c 6473 3d61 7865        fields=axe
-00014520: 7320 2b20 7661 6c75 6573 2c0a 2020 2020  s + values,.    
-00014530: 2020 2020 2020 2020 2a2a 7265 706f 7274          **report
-00014540: 5f70 6172 616d 732c 0a20 2020 2020 2020  _params,.       
-00014550: 2029 0a0a 2020 2020 4061 6464 5f74 6f5f   )..    @add_to_
-00014560: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00014570: 6f75 700a 2020 2020 6173 796e 6320 6465  oup.    async de
-00014580: 6620 6672 6565 5f65 6368 6172 7473 280a  f free_echarts(.
-00014590: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000145a0: 2020 2020 2020 6461 7461 3a20 4f70 7469        data: Opti
-000145b0: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-000145c0: 4461 7461 4672 616d 652c 206c 6973 745b  DataFrame, list[
-000145d0: 6469 6374 5d5d 5d20 3d20 4e6f 6e65 2c0a  dict]]] = None,.
-000145e0: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
-000145f0: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
-00014600: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00014610: 7261 775f 6f70 7469 6f6e 733a 204f 7074  raw_options: Opt
-00014620: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00014630: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
-00014640: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00014650: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00014660: 7469 746c 653a 204f 7074 696f 6e61 6c5b  title: Optional[
-00014670: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00014680: 2020 2020 2072 6f77 735f 7369 7a65 3a20       rows_size: 
-00014690: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-000146a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
-000146b0: 6c73 5f73 697a 653a 204f 7074 696f 6e61  ls_size: Optiona
-000146c0: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
-000146d0: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
-000146e0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000146f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
-00014700: 656c 6473 3a20 4f70 7469 6f6e 616c 5b6c  elds: Optional[l
-00014710: 6973 745d 203d 204e 6f6e 652c 0a20 2020  ist] = None,.   
-00014720: 2020 2020 2064 6174 615f 6973 5f6e 6f74       data_is_not
-00014730: 5f64 663a 2062 6f6f 6c20 3d20 4661 6c73  _df: bool = Fals
-00014740: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00014750: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
-00014760: 6561 7465 2061 6e20 6563 6861 7274 7320  eate an echarts 
-00014770: 6368 6172 7420 7769 7468 2063 7573 746f  chart with custo
-00014780: 6d20 6f70 7469 6f6e 732e 0a20 2020 2020  m options..     
-00014790: 2020 203a 7061 7261 6d20 6461 7461 3a20     :param data: 
-000147a0: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
-000147b0: 6368 6172 740a 2020 2020 2020 2020 3a70  chart.        :p
-000147c0: 6172 616d 206f 7074 696f 6e73 3a20 7468  aram options: th
-000147d0: 6520 6f70 7469 6f6e 7320 6f66 2074 6865  e options of the
-000147e0: 2063 6861 7274 0a20 2020 2020 2020 203a   chart.        :
-000147f0: 7061 7261 6d20 7261 775f 6f70 7469 6f6e  param raw_option
-00014800: 733a 2074 6865 2072 6177 206f 7074 696f  s: the raw optio
-00014810: 6e73 206f 6620 7468 6520 6368 6172 740a  ns of the chart.
-00014820: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
-00014830: 7264 6572 3a20 7468 6520 6f72 6465 7220  rder: the order 
-00014840: 6f66 2074 6865 2063 6861 7274 2069 6e20  of the chart in 
-00014850: 7468 6520 6461 7368 626f 6172 640a 2020  the dashboard.  
-00014860: 2020 2020 2020 3a70 6172 616d 2074 6974        :param tit
-00014870: 6c65 3a20 7468 6520 7469 746c 6520 6f66  le: the title of
-00014880: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
-00014890: 2020 203a 7061 7261 6d20 726f 7773 5f73     :param rows_s
-000148a0: 697a 653a 2074 6865 2072 6f77 7320 7369  ize: the rows si
-000148b0: 7a65 206f 6620 7468 6520 6368 6172 740a  ze of the chart.
-000148c0: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-000148d0: 6f6c 735f 7369 7a65 3a20 7468 6520 636f  ols_size: the co
-000148e0: 6c75 6d6e 7320 7369 7a65 206f 6620 7468  lumns size of th
-000148f0: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-00014900: 3a70 6172 616d 2070 6164 6469 6e67 3a20  :param padding: 
-00014910: 7468 6520 7061 6464 696e 6720 6f66 2074  the padding of t
-00014920: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
-00014930: 203a 7061 7261 6d20 6669 656c 6473 3a20   :param fields: 
-00014940: 7468 6520 6669 656c 6473 206f 6620 7468  the fields of th
-00014950: 6520 6368 6172 740a 2020 2020 2020 2020  e chart.        
-00014960: 3a70 6172 616d 2064 6174 615f 6973 5f6e  :param data_is_n
-00014970: 6f74 5f64 663a 2077 6865 7468 6572 2074  ot_df: whether t
-00014980: 6865 2064 6174 6120 6973 206e 6f74 2061  he data is not a
-00014990: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
-000149a0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000149b0: 6620 6e6f 7420 6f70 7469 6f6e 7320 616e  f not options an
-000149c0: 6420 6e6f 7420 7261 775f 6f70 7469 6f6e  d not raw_option
-000149d0: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-000149e0: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
-000149f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00014a00: 2c20 2245 6974 6865 7220 6f70 7469 6f6e  , "Either option
-00014a10: 7320 6f72 2072 6177 5f6f 7074 696f 6e73  s or raw_options
-00014a20: 206d 7573 7420 6265 2070 726f 7669 6465   must be provide
-00014a30: 6422 2c20 5661 6c75 6545 7272 6f72 0a20  d", ValueError. 
-00014a40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00014a50: 2020 2020 2069 6620 6f70 7469 6f6e 7320       if options 
-00014a60: 616e 6420 6e6f 7420 6973 696e 7374 616e  and not isinstan
-00014a70: 6365 2864 6174 612c 2044 6174 6146 7261  ce(data, DataFra
-00014a80: 6d65 2920 616e 6420 6461 7461 2069 7320  me) and data is 
-00014a90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00014aa0: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
-00014ab0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00014ac0: 6765 722c 2022 6461 7461 206d 7573 7420  ger, "data must 
-00014ad0: 6265 2070 726f 7669 6465 6420 7768 656e  be provided when
-00014ae0: 206f 7074 696f 6e73 2069 7320 7072 6f76   options is prov
-00014af0: 6964 6564 222c 2044 6174 6145 7272 6f72  ided", DataError
-00014b00: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00014b10: 2020 2020 2020 2069 6620 6f70 7469 6f6e         if option
-00014b20: 7320 616e 6420 7261 775f 6f70 7469 6f6e  s and raw_option
-00014b30: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-00014b40: 6f67 5f65 7272 6f72 280a 2020 2020 2020  og_error(.      
-00014b50: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00014b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014b70: 2020 224f 6e6c 7920 6f6e 6520 6f66 206f    "Only one of o
-00014b80: 7074 696f 6e73 2061 6e64 2072 6177 5f6f  ptions and raw_o
-00014b90: 7074 696f 6e73 2063 616e 2062 6520 7072  ptions can be pr
-00014ba0: 6f76 6964 6564 222c 0a20 2020 2020 2020  ovided",.       
-00014bb0: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-00014bc0: 726f 722c 0a20 2020 2020 2020 2020 2020  ror,.           
-00014bd0: 2029 0a0a 2020 2020 2020 2020 6966 2072   )..        if r
-00014be0: 6177 5f6f 7074 696f 6e73 3a0a 2020 2020  aw_options:.    
-00014bf0: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
-00014c00: 3d20 7472 616e 7366 6f72 6d5f 6469 6374  = transform_dict
-00014c10: 5f6a 735f 746f 5f70 7928 7261 775f 6f70  _js_to_py(raw_op
-00014c20: 7469 6f6e 7329 0a20 2020 2020 2020 2020  tions).         
-00014c30: 2020 2064 6174 6120 3d20 7265 7472 6965     data = retrie
-00014c40: 7665 5f64 6174 615f 6672 6f6d 5f6f 7074  ve_data_from_opt
-00014c50: 696f 6e73 286f 7074 696f 6e73 290a 2020  ions(options).  
-00014c60: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00014c70: 735b 2264 6174 6173 6574 225d 203d 207b  s["dataset"] = {
-00014c80: 2273 6f75 7263 6522 3a20 2223 7365 745f  "source": "#set_
-00014c90: 6461 7461 2322 7d0a 2020 2020 2020 2020  data#"}.        
-00014ca0: 2020 2020 6669 656c 6473 203d 205b 6c69      fields = [li
-00014cb0: 7374 2864 6174 615b 305d 2e6b 6579 7328  st(data[0].keys(
-00014cc0: 2929 5d0a 2020 2020 2020 2020 656c 7365  ))].        else
-00014cd0: 3a0a 2020 2020 2020 2020 2020 2020 6f70  :.            op
-00014ce0: 7469 6f6e 7320 3d20 6465 6570 636f 7079  tions = deepcopy
-00014cf0: 286f 7074 696f 6e73 290a 0a20 2020 2020  (options)..     
-00014d00: 2020 2061 7761 6974 2073 656c 662e 5f63     await self._c
-00014d10: 7265 6174 655f 6563 6861 7274 280a 2020  reate_echart(.  
-00014d20: 2020 2020 2020 2020 2020 6f72 6465 723d            order=
-00014d30: 6f72 6465 722c 0a20 2020 2020 2020 2020  order,.         
-00014d40: 2020 2064 6174 615f 6d61 7070 696e 675f     data_mapping_
-00014d50: 746f 5f74 7570 6c65 733d 6177 6169 7420  to_tuples=await 
-00014d60: 7365 6c66 2e5f 6368 6f6f 7365 5f64 6174  self._choose_dat
-00014d70: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
-00014d80: 2020 206f 7264 6572 2c20 6461 7461 2c20     order, data, 
-00014d90: 6475 6d70 5f77 686f 6c65 3d64 6174 615f  dump_whole=data_
-00014da0: 6973 5f6e 6f74 5f64 660a 2020 2020 2020  is_not_df.      
-00014db0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-00014dc0: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
-00014dd0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00014de0: 6f70 7469 6f6e 733d 6f70 7469 6f6e 732c  options=options,
-00014df0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-00014e00: 6c65 3d74 6974 6c65 2c0a 2020 2020 2020  le=title,.      
-00014e10: 2020 2020 2020 726f 7773 5f73 697a 653d        rows_size=
-00014e20: 726f 7773 5f73 697a 652c 0a20 2020 2020  rows_size,.     
-00014e30: 2020 2020 2020 2063 6f6c 735f 7369 7a65         cols_size
-00014e40: 3d63 6f6c 735f 7369 7a65 2c0a 2020 2020  =cols_size,.    
-00014e50: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
-00014e60: 7061 6464 696e 672c 0a20 2020 2020 2020  padding,.       
-00014e70: 2029 0a0a 2020 2020 2320 4543 6861 7274   )..    # EChart
-00014e80: 730a 2020 2020 6c69 6e65 203d 2061 6464  s.    line = add
-00014e90: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
-00014ea0: 635f 6772 6f75 7028 6c69 6e65 5f63 6861  c_group(line_cha
-00014eb0: 7274 290a 2020 2020 6261 7220 3d20 6164  rt).    bar = ad
-00014ec0: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00014ed0: 6e63 5f67 726f 7570 2862 6172 5f63 6861  nc_group(bar_cha
-00014ee0: 7274 290a 2020 2020 7374 6163 6b65 645f  rt).    stacked_
-00014ef0: 6261 7220 3d20 6164 645f 746f 5f67 656e  bar = add_to_gen
-00014f00: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00014f10: 2873 7461 636b 6564 5f62 6172 5f63 6861  (stacked_bar_cha
-00014f20: 7274 290a 2020 2020 6172 6561 203d 2061  rt).    area = a
-00014f30: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00014f40: 796e 635f 6772 6f75 7028 6172 6561 5f63  ync_group(area_c
-00014f50: 6861 7274 290a 2020 2020 7374 6163 6b65  hart).    stacke
-00014f60: 645f 6172 6561 203d 2061 6464 5f74 6f5f  d_area = add_to_
-00014f70: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00014f80: 6f75 7028 7374 6163 6b65 645f 6172 6561  oup(stacked_area
-00014f90: 5f63 6861 7274 290a 2020 2020 7363 6174  _chart).    scat
-00014fa0: 7465 7220 3d20 6164 645f 746f 5f67 656e  ter = add_to_gen
-00014fb0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00014fc0: 2873 6361 7474 6572 5f63 6861 7274 290a  (scatter_chart).
-00014fd0: 2020 2020 686f 7269 7a6f 6e74 616c 5f62      horizontal_b
-00014fe0: 6172 203d 2061 6464 5f74 6f5f 6765 6e65  ar = add_to_gene
-00014ff0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-00015000: 686f 7269 7a6f 6e74 616c 5f62 6172 5f63  horizontal_bar_c
-00015010: 6861 7274 290a 2020 2020 7374 6163 6b65  hart).    stacke
-00015020: 645f 686f 7269 7a6f 6e74 616c 5f62 6172  d_horizontal_bar
-00015030: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-00015040: 6c5f 6173 796e 635f 6772 6f75 7028 7374  l_async_group(st
-00015050: 6163 6b65 645f 686f 7269 7a6f 6e74 616c  acked_horizontal
-00015060: 5f62 6172 5f63 6861 7274 290a 2020 2020  _bar_chart).    
-00015070: 7a65 726f 5f63 656e 7465 7265 645f 6261  zero_centered_ba
-00015080: 7220 3d20 6164 645f 746f 5f67 656e 6572  r = add_to_gener
-00015090: 616c 5f61 7379 6e63 5f67 726f 7570 287a  al_async_group(z
-000150a0: 6572 6f5f 6365 6e74 6572 6564 5f62 6172  ero_centered_bar
-000150b0: 5f63 6861 7274 290a 2020 2020 6675 6e6e  _chart).    funn
-000150c0: 656c 203d 2061 6464 5f74 6f5f 6765 6e65  el = add_to_gene
-000150d0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-000150e0: 6675 6e6e 656c 5f63 6861 7274 290a 2020  funnel_chart).  
-000150f0: 2020 7472 6565 203d 2061 6464 5f74 6f5f    tree = add_to_
-00015100: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-00015110: 6f75 7028 7472 6565 5f63 6861 7274 290a  oup(tree_chart).
-00015120: 2020 2020 7261 6461 7220 3d20 6164 645f      radar = add_
-00015130: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00015140: 5f67 726f 7570 2872 6164 6172 5f63 6861  _group(radar_cha
-00015150: 7274 290a 2020 2020 7069 6520 3d20 6164  rt).    pie = ad
-00015160: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00015170: 6e63 5f67 726f 7570 2870 6965 5f63 6861  nc_group(pie_cha
-00015180: 7274 290a 2020 2020 646f 7567 686e 7574  rt).    doughnut
-00015190: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-000151a0: 6c5f 6173 796e 635f 6772 6f75 7028 646f  l_async_group(do
-000151b0: 7567 686e 7574 5f63 6861 7274 290a 2020  ughnut_chart).  
-000151c0: 2020 726f 7365 203d 2061 6464 5f74 6f5f    rose = add_to_
-000151d0: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-000151e0: 6f75 7028 726f 7365 5f63 6861 7274 290a  oup(rose_chart).
-000151f0: 2020 2020 7375 6e62 7572 7374 203d 2061      sunburst = a
-00015200: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00015210: 796e 635f 6772 6f75 7028 7375 6e62 7572  ync_group(sunbur
-00015220: 7374 5f63 6861 7274 290a 2020 2020 7472  st_chart).    tr
-00015230: 6565 6d61 7020 3d20 6164 645f 746f 5f67  eemap = add_to_g
-00015240: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
-00015250: 7570 2874 7265 656d 6170 5f63 6861 7274  up(treemap_chart
-00015260: 290a 2020 2020 7361 6e6b 6579 203d 2061  ).    sankey = a
-00015270: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
-00015280: 796e 635f 6772 6f75 7028 7361 6e6b 6579  ync_group(sankey
-00015290: 5f63 6861 7274 290a 2020 2020 6865 6174  _chart).    heat
-000152a0: 6d61 7020 3d20 6164 645f 746f 5f67 656e  map = add_to_gen
-000152b0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-000152c0: 2868 6561 746d 6170 5f63 6861 7274 290a  (heatmap_chart).
-000152d0: 2020 2020 7072 6564 6963 7469 7665 5f6c      predictive_l
-000152e0: 696e 6520 3d20 6164 645f 746f 5f67 656e  ine = add_to_gen
-000152f0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-00015300: 2870 7265 6469 6374 6976 655f 6c69 6e65  (predictive_line
-00015310: 5f63 6861 7274 290a 2020 2020 7370 6565  _chart).    spee
-00015320: 645f 6761 7567 6520 3d20 6164 645f 746f  d_gauge = add_to
-00015330: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
-00015340: 726f 7570 2873 7065 6564 5f67 6175 6765  roup(speed_gauge
-00015350: 5f63 6861 7274 290a 2020 2020 7368 696d  _chart).    shim
-00015360: 6f6b 755f 6761 7567 6520 3d20 6164 645f  oku_gauge = add_
-00015370: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-00015380: 5f67 726f 7570 2873 6869 6d6f 6b75 5f67  _group(shimoku_g
-00015390: 6175 6765 5f63 6861 7274 290a 2020 2020  auge_chart).    
-000153a0: 7368 696d 6f6b 755f 6761 7567 6573 5f67  shimoku_gauges_g
-000153b0: 726f 7570 203d 2061 6464 5f74 6f5f 6765  roup = add_to_ge
-000153c0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-000153d0: 7028 7368 696d 6f6b 755f 6761 7567 6573  p(shimoku_gauges
-000153e0: 5f67 726f 7570 290a 2020 2020 6761 7567  _group).    gaug
-000153f0: 655f 696e 6469 6361 746f 7220 3d20 6164  e_indicator = ad
-00015400: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00015410: 6e63 5f67 726f 7570 2867 6175 6765 5f69  nc_group(gauge_i
-00015420: 6e64 6963 6174 6f72 290a 2020 2020 746f  ndicator).    to
-00015430: 705f 626f 7474 6f6d 5f61 7265 6120 3d20  p_bottom_area = 
-00015440: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00015450: 7379 6e63 5f67 726f 7570 2874 6f70 5f62  sync_group(top_b
-00015460: 6f74 746f 6d5f 6172 6561 5f63 6861 7274  ottom_area_chart
-00015470: 7329 0a20 2020 2074 6f70 5f62 6f74 746f  s).    top_botto
-00015480: 6d5f 6c69 6e65 203d 2061 6464 5f74 6f5f  m_line = add_to_
-00015490: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
-000154a0: 6f75 7028 746f 705f 626f 7474 6f6d 5f6c  oup(top_bottom_l
-000154b0: 696e 655f 6368 6172 7473 290a 2020 2020  ine_charts).    
-000154c0: 6c69 6e65 5f77 6974 685f 636f 6e66 6964  line_with_confid
-000154d0: 656e 6365 5f61 7265 6120 3d20 6164 645f  ence_area = add_
-000154e0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-000154f0: 5f67 726f 7570 280a 2020 2020 2020 2020  _group(.        
-00015500: 6c69 6e65 5f77 6974 685f 636f 6e66 6964  line_with_confid
-00015510: 656e 6365 5f61 7265 615f 6368 6172 740a  ence_area_chart.
-00015520: 2020 2020 290a 2020 2020 7363 6174 7465      ).    scatte
-00015530: 725f 7769 7468 5f65 6666 6563 7420 3d20  r_with_effect = 
-00015540: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
-00015550: 7379 6e63 5f67 726f 7570 2873 6361 7474  sync_group(scatt
-00015560: 6572 5f77 6974 685f 6566 6665 6374 5f63  er_with_effect_c
-00015570: 6861 7274 290a 2020 2020 7761 7465 7266  hart).    waterf
-00015580: 616c 6c20 3d20 6164 645f 746f 5f67 656e  all = add_to_gen
-00015590: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
-000155a0: 2877 6174 6572 6661 6c6c 5f63 6861 7274  (waterfall_chart
-000155b0: 290a 2020 2020 6c69 6e65 5f61 6e64 5f62  ).    line_and_b
-000155c0: 6172 5f63 6861 7274 7320 3d20 6164 645f  ar_charts = add_
-000155d0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
-000155e0: 5f67 726f 7570 286c 696e 655f 616e 645f  _group(line_and_
-000155f0: 6261 725f 6368 6172 7473 290a 2020 2020  bar_charts).    
-00015600: 7365 676d 656e 7465 645f 6c69 6e65 203d  segmented_line =
-00015610: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
-00015620: 6173 796e 635f 6772 6f75 7028 7365 676d  async_group(segm
-00015630: 656e 7465 645f 6c69 6e65 5f63 6861 7274  ented_line_chart
-00015640: 290a 2020 2020 6d61 726b 6564 5f6c 696e  ).    marked_lin
-00015650: 6520 3d20 6164 645f 746f 5f67 656e 6572  e = add_to_gener
-00015660: 616c 5f61 7379 6e63 5f67 726f 7570 286d  al_async_group(m
-00015670: 6172 6b65 645f 6c69 6e65 5f63 6861 7274  arked_line_chart
-00015680: 290a 2020 2020 7365 676d 656e 7465 645f  ).    segmented_
-00015690: 6172 6561 203d 2061 6464 5f74 6f5f 6765  area = add_to_ge
-000156a0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-000156b0: 7028 7365 676d 656e 7465 645f 6172 6561  p(segmented_area
-000156c0: 5f63 6861 7274 290a 0a20 2020 2023 2042  _chart)..    # B
-000156d0: 656e 746f 626f 7820 6368 6172 7473 2064  entobox charts d
-000156e0: 6566 696e 6564 2069 6e20 7468 6520 6265  efined in the be
-000156f0: 6e74 6f62 6f78 5f63 6861 7274 732e 7079  ntobox_charts.py
-00015700: 2066 696c 650a 2020 2020 696e 666f 6772   file.    infogr
-00015710: 6170 6869 6373 5f74 6578 745f 6275 6262  aphics_text_bubb
-00015720: 6c65 203d 2061 6464 5f74 6f5f 6765 6e65  le = add_to_gene
-00015730: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-00015740: 696e 666f 6772 6170 6869 6373 5f74 6578  infographics_tex
-00015750: 745f 6275 6262 6c65 290a 2020 2020 6368  t_bubble).    ch
-00015760: 6172 745f 616e 645f 6d6f 6461 6c5f 6275  art_and_modal_bu
-00015770: 7474 6f6e 203d 2061 6464 5f74 6f5f 6765  tton = add_to_ge
-00015780: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
-00015790: 7028 6368 6172 745f 616e 645f 6d6f 6461  p(chart_and_moda
-000157a0: 6c5f 6275 7474 6f6e 290a 2020 2020 6368  l_button).    ch
-000157b0: 6172 745f 616e 645f 696e 6469 6361 746f  art_and_indicato
-000157c0: 7273 203d 2061 6464 5f74 6f5f 6765 6e65  rs = add_to_gene
-000157d0: 7261 6c5f 6173 796e 635f 6772 6f75 7028  ral_async_group(
-000157e0: 6368 6172 745f 616e 645f 696e 6469 6361  chart_and_indica
-000157f0: 746f 7273 290a 2020 2020 696e 6469 6361  tors).    indica
-00015800: 746f 7273 5f77 6974 685f 6865 6164 6572  tors_with_header
-00015810: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
-00015820: 6c5f 6173 796e 635f 6772 6f75 7028 696e  l_async_group(in
-00015830: 6469 6361 746f 7273 5f77 6974 685f 6865  dicators_with_he
-00015840: 6164 6572 290a 2020 2020 6c69 6e65 5f77  ader).    line_w
-00015850: 6974 685f 7375 6d6d 6172 7920 3d20 6164  ith_summary = ad
-00015860: 645f 746f 5f67 656e 6572 616c 5f61 7379  d_to_general_asy
-00015870: 6e63 5f67 726f 7570 286c 696e 655f 7769  nc_group(line_wi
-00015880: 7468 5f73 756d 6d61 7279 290a            th_summary).
+00012bb0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00012bd0: 6f74 2072 6570 6f72 745f 6461 7461 5f73  ot report_data_s
+00012be0: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+00012bf0: 2020 2020 2020 2020 2020 206f 7220 6e6f             or no
+00012c00: 7420 7365 6c66 2e5f 6368 6563 6b5f 6d61  t self._check_ma
+00012c10: 7070 696e 675f 696e 5f72 6570 6f72 745f  pping_in_report_
+00012c20: 6461 7461 5f73 6574 280a 2020 2020 2020  data_set(.      
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 2020 2020 2020 7265 706f 7274 5f64 6174        report_dat
+00012c50: 615f 7365 742c 206d 6170 7065 645f 665b  a_set, mapped_f[
+00012c60: 695d 0a20 2020 2020 2020 2020 2020 2020  i].             
+00012c70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00012ca0: 2020 2020 2020 2020 2020 2020 7264 5f69              rd_i
+00012cb0: 6473 203d 204e 6f6e 650a 2020 2020 2020  ds = None.      
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00012ce0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012cf0: 2020 2020 2020 2020 2020 7264 5f69 6473            rd_ids
+00012d00: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+00012d10: 2069 6620 6e6f 7420 7264 5f69 6473 3a0a   if not rd_ids:.
+00012d20: 2020 2020 2020 2020 2020 2020 6177 6169              awai
+00012d30: 7420 7265 706f 7274 2e64 656c 6574 655f  t report.delete_
+00012d40: 7265 706f 7274 5f64 6174 615f 7365 7473  report_data_sets
+00012d50: 286c 6f67 3d54 7275 6529 0a20 2020 2020  (log=True).     
+00012d60: 2020 2020 2020 2072 6570 6f72 745f 6461         report_da
+00012d70: 7461 5f73 6574 7320 3d20 6177 6169 7420  ta_sets = await 
+00012d80: 7365 6c66 2e5f 6765 745f 7265 706f 7274  self._get_report
+00012d90: 5f64 6174 615f 7365 7473 5f70 6572 5f6d  _data_sets_per_m
+00012da0: 6170 7069 6e67 280a 2020 2020 2020 2020  apping(.        
+00012db0: 2020 2020 2020 2020 7265 706f 7274 2c20          report, 
+00012dc0: 6461 7461 5f6d 6170 7069 6e67 5f74 6f5f  data_mapping_to_
+00012dd0: 7475 706c 6573 2c20 6669 656c 6473 0a20  tuples, fields. 
+00012de0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00012df0: 2020 2020 2020 2020 2072 645f 6964 7320           rd_ids 
+00012e00: 3d20 5b72 645b 2269 6422 5d20 666f 7220  = [rd["id"] for 
+00012e10: 7264 2069 6e20 7265 706f 7274 5f64 6174  rd in report_dat
+00012e20: 615f 7365 7473 5d0a 0a20 2020 2020 2020  a_sets]..       
+00012e30: 2073 656c 662e 5f75 7064 6174 655f 6f70   self._update_op
+00012e40: 7469 6f6e 7328 6f70 7469 6f6e 732c 206f  tions(options, o
+00012e50: 7074 696f 6e5f 6d6f 6469 6669 6361 7469  ption_modificati
+00012e60: 6f6e 7329 0a0a 2020 2020 2020 2020 6966  ons)..        if
+00012e70: 206c 656e 2872 645f 6964 7329 2021 3d20   len(rd_ids) != 
+00012e80: 6c65 6e28 6461 7461 5f6b 6579 5f65 6e74  len(data_key_ent
+00012e90: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
+00012ea0: 2020 206c 6f67 5f65 7272 6f72 280a 2020     log_error(.  
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00012ec0: 6767 6572 2c0a 2020 2020 2020 2020 2020  gger,.          
+00012ed0: 2020 2020 2020 6622 5468 6520 6e75 6d62        f"The numb
+00012ee0: 6572 206f 6620 6461 7461 2072 6566 6572  er of data refer
+00012ef0: 656e 6365 7320 616e 6420 6669 656c 6473  ences and fields
+00012f00: 206d 7573 7420 6265 2065 7175 616c 2c20   must be equal, 
+00012f10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012f20: 2020 6622 7468 6579 2061 7265 207b 6c65    f"they are {le
+00012f30: 6e28 6461 7461 5f6b 6579 5f65 6e74 7269  n(data_key_entri
+00012f40: 6573 297d 2061 6e64 207b 6c65 6e28 7264  es)} and {len(rd
+00012f50: 5f69 6473 297d 2072 6573 7065 6374 6976  _ids)} respectiv
+00012f60: 656c 792e 222c 0a20 2020 2020 2020 2020  ely.",.         
+00012f70: 2020 2020 2020 2044 6174 6145 7272 6f72         DataError
+00012f80: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00012f90: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
+00012fa0: 6461 7461 5f6b 6579 5f65 6e74 7279 2069  data_key_entry i
+00012fb0: 6e20 656e 756d 6572 6174 6528 6461 7461  n enumerate(data
+00012fc0: 5f6b 6579 5f65 6e74 7269 6573 293a 0a20  _key_entries):. 
+00012fd0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00012fe0: 3d20 6f70 7469 6f6e 730a 2020 2020 2020  = options.      
+00012ff0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00013000: 2064 6174 615f 6b65 795f 656e 7472 795b   data_key_entry[
+00013010: 3a2d 315d 3a0a 2020 2020 2020 2020 2020  :-1]:.          
+00013020: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00013030: 615b 6b65 795d 0a20 2020 2020 2020 2020  a[key].         
+00013040: 2020 2064 6174 615b 6461 7461 5f6b 6579     data[data_key
+00013050: 5f65 6e74 7279 5b2d 315d 5d20 3d20 2223  _entry[-1]] = "#
+00013060: 7b22 202b 2072 645f 6964 735b 695d 202b  {" + rd_ids[i] +
+00013070: 2022 7d22 0a0a 2020 2020 2020 2020 6177   "}"..        aw
+00013080: 6169 7420 7365 6c66 2e5f 6372 6561 7465  ait self._create
+00013090: 5f63 6861 7274 280a 2020 2020 2020 2020  _chart(.        
+000130a0: 2020 2020 6368 6172 745f 636c 6173 733d      chart_class=
+000130b0: 4543 6861 7274 2c0a 2020 2020 2020 2020  EChart,.        
+000130c0: 2020 2020 7072 6f70 6572 7469 6573 3d7b      properties={
+000130d0: 226f 7074 696f 6e22 3a20 6f70 7469 6f6e  "option": option
+000130e0: 737d 2c0a 2020 2020 2020 2020 2020 2020  s},.            
+000130f0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
+00013100: 2020 2020 2020 2020 2074 6974 6c65 3d74           title=t
+00013110: 6974 6c65 2c0a 2020 2020 2020 2020 2020  itle,.          
+00013120: 2020 7369 7a65 5061 6464 696e 673d 7061    sizePadding=pa
+00013130: 6464 696e 672c 0a20 2020 2020 2020 2020  dding,.         
+00013140: 2020 2073 697a 6552 6f77 733d 726f 7773     sizeRows=rows
+00013150: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
+00013160: 2020 2073 697a 6543 6f6c 756d 6e73 3d63     sizeColumns=c
+00013170: 6f6c 735f 7369 7a65 2c0a 2020 2020 2020  ols_size,.      
+00013180: 2020 290a 0a20 2020 2040 7374 6174 6963    )..    @static
+00013190: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
+000131a0: 6170 706c 795f 7661 7269 616e 7428 6563  apply_variant(ec
+000131b0: 6861 7274 5f6f 7074 696f 6e73 3a20 6469  hart_options: di
+000131c0: 6374 2c20 7661 7269 616e 743a 204f 7074  ct, variant: Opt
+000131d0: 696f 6e61 6c5b 7374 725d 293a 0a20 2020  ional[str]):.   
+000131e0: 2020 2020 2069 6620 7661 7269 616e 7420       if variant 
+000131f0: 3d3d 2022 636c 6561 6e22 3a0a 2020 2020  == "clean":.    
+00013200: 2020 2020 2020 2020 6563 6861 7274 5f6f          echart_o
+00013210: 7074 696f 6e73 2e75 7064 6174 6528 0a20  ptions.update(. 
+00013220: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00013230: 2274 6f6f 6c62 6f78 223a 207b 2273 686f  "toolbox": {"sho
+00013240: 7722 3a20 4661 6c73 657d 2c20 226c 6567  w": False}, "leg
+00013250: 656e 6422 3a20 7b22 7368 6f77 223a 2046  end": {"show": F
+00013260: 616c 7365 7d2c 2022 6772 6964 223a 207b  alse}, "grid": {
+00013270: 7d7d 0a20 2020 2020 2020 2020 2020 2029  }}.            )
+00013280: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013290: 2061 7869 736c 6973 7420 696e 205b 6563   axislist in [ec
+000132a0: 6861 7274 5f6f 7074 696f 6e73 5b22 7841  hart_options["xA
+000132b0: 7869 7322 5d2c 2065 6368 6172 745f 6f70  xis"], echart_op
+000132c0: 7469 6f6e 735b 2279 4178 6973 225d 5d3a  tions["yAxis"]]:
+000132d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132e0: 2066 6f72 2061 7869 7320 696e 2061 7869   for axis in axi
+000132f0: 736c 6973 743a 0a20 2020 2020 2020 2020  slist:.         
+00013300: 2020 2020 2020 2020 2020 2061 7869 732e             axis.
+00013310: 7570 6461 7465 280a 2020 2020 2020 2020  update(.        
+00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013330: 7b22 6178 6973 4c69 6e65 223a 207b 2273  {"axisLine": {"s
+00013340: 686f 7722 3a20 4661 6c73 657d 2c20 2261  how": False}, "a
+00013350: 7869 7354 6963 6b22 3a20 7b22 7368 6f77  xisTick": {"show
+00013360: 223a 2046 616c 7365 7d7d 0a20 2020 2020  ": False}}.     
+00013370: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00013380: 0a20 2020 2020 2020 2065 6c69 6620 7661  .        elif va
+00013390: 7269 616e 7420 3d3d 2022 6d69 6e69 6d61  riant == "minima
+000133a0: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+000133b0: 6563 6861 7274 5f6f 7074 696f 6e73 2e75  echart_options.u
+000133c0: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
+000133d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000133e0: 2020 2020 2020 2020 2020 2020 2022 746f               "to
+000133f0: 6f6c 626f 7822 3a20 7b22 7368 6f77 223a  olbox": {"show":
+00013400: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+00013410: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
+00013420: 6765 6e64 223a 207b 2273 686f 7722 3a20  gend": {"show": 
+00013430: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
+00013440: 2020 2020 2020 2020 2020 2020 2267 7269              "gri
+00013450: 6422 3a20 7b22 6c65 6674 223a 2022 3125  d": {"left": "1%
+00013460: 222c 2022 7269 6768 7422 3a20 2231 2522  ", "right": "1%"
+00013470: 2c20 2274 6f70 223a 2022 3125 222c 2022  , "top": "1%", "
+00013480: 626f 7474 6f6d 223a 2022 3125 227d 2c0a  bottom": "1%"},.
+00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134a0: 2020 2020 2274 6f6f 6c74 6970 223a 207b      "tooltip": {
+000134b0: 2273 686f 7722 3a20 4661 6c73 657d 2c0a  "show": False},.
+000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134d0: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
+000134e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000134f0: 6178 6973 6c69 7374 2069 6e20 5b65 6368  axislist in [ech
+00013500: 6172 745f 6f70 7469 6f6e 735b 2278 4178  art_options["xAx
+00013510: 6973 225d 2c20 6563 6861 7274 5f6f 7074  is"], echart_opt
+00013520: 696f 6e73 5b22 7941 7869 7322 5d5d 3a0a  ions["yAxis"]]:.
+00013530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013540: 666f 7220 6178 6973 2069 6e20 6178 6973  for axis in axis
+00013550: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+00013560: 2020 2020 2020 2020 2020 6178 6973 2e75            axis.u
+00013570: 7064 6174 6528 0a20 2020 2020 2020 2020  pdate(.         
+00013580: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00013590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135a0: 2020 2020 2020 2020 2020 2020 2022 6178               "ax
+000135b0: 6973 4c69 6e65 223a 207b 2273 686f 7722  isLine": {"show"
+000135c0: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
+000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135e0: 2020 2020 2020 2261 7869 7354 6963 6b22        "axisTick"
+000135f0: 3a20 7b22 7368 6f77 223a 2046 616c 7365  : {"show": False
+00013600: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00013610: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00013620: 7370 6c69 744c 696e 6522 3a20 7b22 7368  splitLine": {"sh
+00013630: 6f77 223a 2046 616c 7365 7d2c 0a20 2020  ow": False},.   
+00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013650: 2020 2020 2020 2020 2022 6178 6973 4c61           "axisLa
+00013660: 6265 6c22 3a20 7b22 7368 6f77 223a 2046  bel": {"show": F
+00013670: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+00013680: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00013690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136a0: 2020 2020 2029 0a0a 2020 2020 6173 796e       )..    asyn
+000136b0: 6320 6465 6620 5f63 7265 6174 655f 7472  c def _create_tr
+000136c0: 656e 645f 6368 6172 7428 0a20 2020 2020  end_chart(.     
+000136d0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000136e0: 2061 7865 733a 2055 6e69 6f6e 5b6c 6973   axes: Union[lis
+000136f0: 745b 7374 725d 2c20 7374 725d 2c0a 2020  t[str], str],.  
+00013700: 2020 2020 2020 6f72 6465 723a 2069 6e74        order: int
+00013710: 2c0a 2020 2020 2020 2020 6461 7461 5f6d  ,.        data_m
+00013720: 6170 7069 6e67 5f74 6f5f 7475 706c 6573  apping_to_tuples
+00013730: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
+00013740: 2c0a 2020 2020 2020 2020 6563 6861 7274  ,.        echart
+00013750: 5f6f 7074 696f 6e73 3a20 6469 6374 2c0a  _options: dict,.
+00013760: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
+00013770: 7074 696f 6e73 3a20 556e 696f 6e5b 6469  ptions: Union[di
+00013780: 6374 2c20 6c69 7374 5b64 6963 745d 5d2c  ct, list[dict]],
+00013790: 0a20 2020 2020 2020 2076 616c 7565 733a  .        values:
+000137a0: 204f 7074 696f 6e61 6c5b 556e 696f 6e5b   Optional[Union[
+000137b0: 6c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  list[Union[str, 
+000137c0: 7475 706c 655d 5d2c 2073 7472 2c20 7475  tuple]], str, tu
+000137d0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
+000137e0: 2020 2020 2020 785f 6178 6973 5f6e 616d        x_axis_nam
+000137f0: 6573 3a20 4f70 7469 6f6e 616c 5b55 6e69  es: Optional[Uni
+00013800: 6f6e 5b73 7472 2c20 6c69 7374 5b73 7472  on[str, list[str
+00013810: 5d5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ]]] = None,.    
+00013820: 2020 2020 795f 6178 6973 5f6e 616d 6573      y_axis_names
+00013830: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00013840: 5b73 7472 2c20 6c69 7374 5b73 7472 5d5d  [str, list[str]]
+00013850: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00013860: 2020 7368 6f77 5f76 616c 7565 733a 204f    show_values: O
+00013870: 7074 696f 6e61 6c5b 556e 696f 6e5b 6c69  ptional[Union[li
+00013880: 7374 5b73 7472 5d2c 2073 7472 5d5d 203d  st[str], str]] =
+00013890: 204e 6f6e 652c 0a20 2020 2020 2020 2076   None,.        v
+000138a0: 6172 6961 6e74 3a20 4f70 7469 6f6e 616c  ariant: Optional
+000138b0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+000138c0: 2020 2020 2020 2a2a 7265 706f 7274 5f70        **report_p
+000138d0: 6172 616d 732c 0a20 2020 2029 3a0a 2020  arams,.    ):.  
+000138e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000138f0: 2020 4372 6561 7465 2061 206c 696e 6520    Create a line 
+00013900: 6368 6172 7420 696e 2074 6865 2064 6173  chart in the das
+00013910: 6862 6f61 7264 2e0a 2020 2020 2020 2020  hboard..        
+00013920: 3a70 6172 616d 2064 6174 613a 2074 6865  :param data: the
+00013930: 2064 6174 6120 6f66 2074 6865 2063 6861   data of the cha
+00013940: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+00013950: 6d20 6178 6573 3a20 7468 6520 6e61 6d65  m axes: the name
+00013960: 7320 6f66 2074 6865 2063 6f6c 756d 6e73  s of the columns
+00013970: 2074 6f20 6265 2075 7365 6420 6173 2061   to be used as a
+00013980: 7869 730a 2020 2020 2020 2020 3a70 6172  xis.        :par
+00013990: 616d 2076 616c 7565 733a 2074 6865 206e  am values: the n
+000139a0: 616d 6573 206f 6620 7468 6520 636f 6c75  ames of the colu
+000139b0: 6d6e 7320 746f 2062 6520 7573 6564 2061  mns to be used a
+000139c0: 7320 7661 6c75 6573 0a20 2020 2020 2020  s values.       
+000139d0: 203a 7061 7261 6d20 785f 6178 6973 5f6e   :param x_axis_n
+000139e0: 616d 6573 3a20 7468 6520 6e61 6d65 206f  ames: the name o
+000139f0: 6620 7468 6520 7820 6178 6573 0a20 2020  f the x axes.   
+00013a00: 2020 2020 203a 7061 7261 6d20 795f 6178       :param y_ax
+00013a10: 6973 5f6e 616d 6573 3a20 7468 6520 6e61  is_names: the na
+00013a20: 6d65 206f 6620 7468 6520 7920 6178 6573  me of the y axes
+00013a30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013a40: 6563 6861 7274 5f6f 7074 696f 6e73 3a20  echart_options: 
+00013a50: 7468 6520 6f70 7469 6f6e 7320 6f66 2074  the options of t
+00013a60: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
+00013a70: 203a 7061 7261 6d20 7365 7269 6573 5f6f   :param series_o
+00013a80: 7074 696f 6e73 3a20 7468 6520 6f70 7469  ptions: the opti
+00013a90: 6f6e 7320 6f66 2074 6865 2073 6572 6965  ons of the serie
+00013aa0: 7320 6f66 2074 6865 2063 6861 7274 0a20  s of the chart. 
+00013ab0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
+00013ac0: 7474 6f6d 5f74 6f6f 6c62 6f78 3a20 7768  ttom_toolbox: wh
+00013ad0: 6574 6865 7220 746f 2073 686f 7720 7468  ether to show th
+00013ae0: 6520 746f 6f6c 626f 7820 6f6e 2074 6f70  e toolbox on top
+00013af0: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
+00013b00: 2020 2020 2020 3a70 6172 616d 206f 7264        :param ord
+00013b10: 6572 3a20 7468 6520 6f72 6465 7220 6f66  er: the order of
+00013b20: 2074 6865 2063 6861 7274 2069 6e20 7468   the chart in th
+00013b30: 6520 6461 7368 626f 6172 640a 2020 2020  e dashboard.    
+00013b40: 2020 2020 3a70 6172 616d 2072 6570 6f72      :param repor
+00013b50: 745f 7061 7261 6d73 3a20 6164 6469 7469  t_params: additi
+00013b60: 6f6e 616c 2072 6570 6f72 7420 7061 7261  onal report para
+00013b70: 6d65 7465 7273 2061 7320 6b65 792d 7661  meters as key-va
+00013b80: 6c75 6520 7061 6972 730a 2020 2020 2020  lue pairs.      
+00013b90: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00013ba0: 6c66 2e5f 6170 706c 795f 7661 7269 616e  lf._apply_varian
+00013bb0: 7428 6563 6861 7274 5f6f 7074 696f 6e73  t(echart_options
+00013bc0: 2c20 7661 7269 616e 7429 0a20 2020 2020  , variant).     
+00013bd0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00013be0: 2861 7865 732c 2073 7472 293a 0a20 2020  (axes, str):.   
+00013bf0: 2020 2020 2020 2020 2061 7865 7320 3d20           axes = 
+00013c00: 5b61 7865 735d 0a20 2020 2020 2020 2069  [axes].        i
+00013c10: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+00013c20: 7565 732c 2073 7472 2920 6f72 2069 7369  ues, str) or isi
+00013c30: 6e73 7461 6e63 6528 7661 6c75 6573 2c20  nstance(values, 
+00013c40: 7475 706c 6529 3a0a 2020 2020 2020 2020  tuple):.        
+00013c50: 2020 2020 7661 6c75 6573 203d 205b 7661      values = [va
+00013c60: 6c75 6573 5d0a 2020 2020 2020 2020 6966  lues].        if
+00013c70: 2073 686f 775f 7661 6c75 6573 2069 7320   show_values is 
+00013c80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00013c90: 2020 7368 6f77 5f76 616c 7565 7320 3d20    show_values = 
+00013ca0: 5b5d 0a0a 2020 2020 2020 2020 6966 2022  []..        if "
+00013cb0: 785f 6178 6973 5f6e 616d 6522 2069 6e20  x_axis_name" in 
+00013cc0: 7265 706f 7274 5f70 6172 616d 733a 0a20  report_params:. 
+00013cd0: 2020 2020 2020 2020 2020 2078 5f61 7869             x_axi
+00013ce0: 735f 6e61 6d65 7320 3d20 5b72 6570 6f72  s_names = [repor
+00013cf0: 745f 7061 7261 6d73 5b22 785f 6178 6973  t_params["x_axis
+00013d00: 5f6e 616d 6522 5d5d 0a20 2020 2020 2020  _name"]].       
+00013d10: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00013d20: 2878 5f61 7869 735f 6e61 6d65 732c 2073  (x_axis_names, s
+00013d30: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00013d40: 2078 5f61 7869 735f 6e61 6d65 7320 3d20   x_axis_names = 
+00013d50: 5b78 5f61 7869 735f 6e61 6d65 735d 0a20  [x_axis_names]. 
+00013d60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013d70: 2020 2020 2020 2020 2078 5f61 7869 735f           x_axis_
+00013d80: 6e61 6d65 7320 3d20 5b5d 0a0a 2020 2020  names = []..    
+00013d90: 2020 2020 6966 2022 795f 6178 6973 5f6e      if "y_axis_n
+00013da0: 616d 6522 2069 6e20 7265 706f 7274 5f70  ame" in report_p
+00013db0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
+00013dc0: 2020 2079 5f61 7869 735f 6e61 6d65 7320     y_axis_names 
+00013dd0: 3d20 5b72 6570 6f72 745f 7061 7261 6d73  = [report_params
+00013de0: 5b22 795f 6178 6973 5f6e 616d 6522 5d5d  ["y_axis_name"]]
+00013df0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00013e00: 696e 7374 616e 6365 2879 5f61 7869 735f  instance(y_axis_
+00013e10: 6e61 6d65 732c 2073 7472 293a 0a20 2020  names, str):.   
+00013e20: 2020 2020 2020 2020 2079 5f61 7869 735f           y_axis_
+00013e30: 6e61 6d65 7320 3d20 5b79 5f61 7869 735f  names = [y_axis_
+00013e40: 6e61 6d65 735d 0a20 2020 2020 2020 2065  names].        e
+00013e50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00013e60: 2079 5f61 7869 735f 6e61 6d65 7320 3d20   y_axis_names = 
+00013e70: 5b5d 0a0a 2020 2020 2020 2020 7661 6c75  []..        valu
+00013e80: 6573 203d 2028 0a20 2020 2020 2020 2020  es = (.         
+00013e90: 2020 205b 7620 666f 7220 7620 696e 2064     [v for v in d
+00013ea0: 6174 615f 6d61 7070 696e 675f 746f 5f74  ata_mapping_to_t
+00013eb0: 7570 6c65 732e 6b65 7973 2829 2069 6620  uples.keys() if 
+00013ec0: 7620 6e6f 7420 696e 2061 7865 735d 0a20  v not in axes]. 
+00013ed0: 2020 2020 2020 2020 2020 2069 6620 7661             if va
+00013ee0: 6c75 6573 2069 7320 4e6f 6e65 0a20 2020  lues is None.   
+00013ef0: 2020 2020 2020 2020 2065 6c73 6520 7661           else va
+00013f00: 6c75 6573 0a20 2020 2020 2020 2029 0a20  lues.        ). 
+00013f10: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00013f20: 616e 6365 2873 6572 6965 735f 6f70 7469  ance(series_opti
+00013f30: 6f6e 732c 2064 6963 7429 3a0a 2020 2020  ons, dict):.    
+00013f40: 2020 2020 2020 2020 7365 7269 6573 5f6f          series_o
+00013f50: 7074 696f 6e73 203d 205b 7365 7269 6573  ptions = [series
+00013f60: 5f6f 7074 696f 6e73 5d20 2a20 6c65 6e28  _options] * len(
+00013f70: 7661 6c75 6573 290a 2020 2020 2020 2020  values).        
+00013f80: 656c 6966 206c 656e 2873 6572 6965 735f  elif len(series_
+00013f90: 6f70 7469 6f6e 7329 203c 206c 656e 2876  options) < len(v
+00013fa0: 616c 7565 7329 3a0a 2020 2020 2020 2020  alues):.        
+00013fb0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
+00013fc0: 6e73 203d 2073 6572 6965 735f 6f70 7469  ns = series_opti
+00013fd0: 6f6e 7320 2b20 5b73 6572 6965 735f 6f70  ons + [series_op
+00013fe0: 7469 6f6e 735b 2d31 5d5d 202a 2028 0a20  tions[-1]] * (. 
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00014000: 656e 2876 616c 7565 7329 202d 206c 656e  en(values) - len
+00014010: 2873 6572 6965 735f 6f70 7469 6f6e 7329  (series_options)
+00014020: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00014030: 2020 2020 2020 2065 6c69 6620 6c65 6e28         elif len(
+00014040: 7365 7269 6573 5f6f 7074 696f 6e73 2920  series_options) 
+00014050: 3e20 6c65 6e28 7661 6c75 6573 293a 0a20  > len(values):. 
+00014060: 2020 2020 2020 2020 2020 2073 6572 6965             serie
+00014070: 735f 6f70 7469 6f6e 7320 3d20 7365 7269  s_options = seri
+00014080: 6573 5f6f 7074 696f 6e73 5b3a 206c 656e  es_options[: len
+00014090: 2876 616c 7565 7329 5d0a 0a20 2020 2020  (values)]..     
+000140a0: 2020 2065 6368 6172 745f 6f70 7469 6f6e     echart_option
+000140b0: 735b 2273 6572 6965 7322 5d20 3d20 5b0a  s["series"] = [.
+000140c0: 2020 2020 2020 2020 2020 2020 6465 6570              deep
+000140d0: 5f75 7064 6174 6528 0a20 2020 2020 2020  _update(.       
+000140e0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000140f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014100: 6e61 6d65 223a 206e 616d 6520 6966 2069  name": name if i
+00014110: 7369 6e73 7461 6e63 6528 6e61 6d65 2c20  sinstance(name, 
+00014120: 7374 7229 2065 6c73 6520 2220 c397 2022  str) else " .. "
+00014130: 2e6a 6f69 6e28 6e61 6d65 292c 0a20 2020  .join(name),.   
+00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014150: 2022 6c61 6265 6c22 3a20 7b22 7368 6f77   "label": {"show
+00014160: 223a 2073 686f 775f 7661 6c75 6573 203d  ": show_values =
+00014170: 3d20 2261 6c6c 2220 6f72 206e 616d 6520  = "all" or name 
+00014180: 696e 2073 686f 775f 7661 6c75 6573 7d2c  in show_values},
+00014190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141a0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+000141b0: 2020 2020 7365 7269 6573 5f6f 7074 696f      series_optio
+000141c0: 6e73 5b69 5d2c 0a20 2020 2020 2020 2020  ns[i],.         
+000141d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000141e0: 2066 6f72 2069 2c20 6e61 6d65 2069 6e20   for i, name in 
+000141f0: 656e 756d 6572 6174 6528 7661 6c75 6573  enumerate(values
+00014200: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
+00014210: 2020 2020 2066 6f72 2069 2c20 6178 6973       for i, axis
+00014220: 5f6f 7074 696f 6e73 2069 6e20 656e 756d  _options in enum
+00014230: 6572 6174 6528 6563 6861 7274 5f6f 7074  erate(echart_opt
+00014240: 696f 6e73 5b22 7841 7869 7322 5d29 3a0a  ions["xAxis"]):.
+00014250: 2020 2020 2020 2020 2020 2020 6178 6973              axis
+00014260: 5f6f 7074 696f 6e73 5b22 6e61 6d65 225d  _options["name"]
+00014270: 203d 2078 5f61 7869 735f 6e61 6d65 735b   = x_axis_names[
+00014280: 695d 2069 6620 6920 3c20 6c65 6e28 785f  i] if i < len(x_
+00014290: 6178 6973 5f6e 616d 6573 2920 656c 7365  axis_names) else
+000142a0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000142b0: 2020 6966 2061 7869 735f 6f70 7469 6f6e    if axis_option
+000142c0: 735b 226e 616d 6522 5d20 616e 6420 226e  s["name"] and "n
+000142d0: 616d 6547 6170 2220 6e6f 7420 696e 2061  ameGap" not in a
+000142e0: 7869 735f 6f70 7469 6f6e 733a 0a20 2020  xis_options:.   
+000142f0: 2020 2020 2020 2020 2020 2020 2061 7869               axi
+00014300: 735f 6f70 7469 6f6e 735b 226e 616d 6547  s_options["nameG
+00014310: 6170 225d 203d 2033 320a 0a20 2020 2020  ap"] = 32..     
+00014320: 2020 2066 6f72 2069 2c20 6178 6973 5f6f     for i, axis_o
+00014330: 7074 696f 6e73 2069 6e20 656e 756d 6572  ptions in enumer
+00014340: 6174 6528 6563 6861 7274 5f6f 7074 696f  ate(echart_optio
+00014350: 6e73 5b22 7941 7869 7322 5d29 3a0a 2020  ns["yAxis"]):.  
+00014360: 2020 2020 2020 2020 2020 6178 6973 5f6f            axis_o
+00014370: 7074 696f 6e73 5b22 6e61 6d65 225d 203d  ptions["name"] =
+00014380: 2079 5f61 7869 735f 6e61 6d65 735b 695d   y_axis_names[i]
+00014390: 2069 6620 6920 3c20 6c65 6e28 795f 6178   if i < len(y_ax
+000143a0: 6973 5f6e 616d 6573 2920 656c 7365 204e  is_names) else N
+000143b0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000143c0: 6966 2061 7869 735f 6f70 7469 6f6e 735b  if axis_options[
+000143d0: 226e 616d 6522 5d20 616e 6420 226e 616d  "name"] and "nam
+000143e0: 6547 6170 2220 6e6f 7420 696e 2061 7869  eGap" not in axi
+000143f0: 735f 6f70 7469 6f6e 733a 0a20 2020 2020  s_options:.     
+00014400: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
+00014410: 6f70 7469 6f6e 735b 226e 616d 6547 6170  options["nameGap
+00014420: 225d 203d 202d 3234 0a20 2020 2020 2020  "] = -24.       
+00014430: 2020 2020 2020 2020 2061 7869 735f 6f70           axis_op
+00014440: 7469 6f6e 735b 226f 6666 7365 7422 5d20  tions["offset"] 
+00014450: 3d20 3336 0a20 2020 2020 2020 2020 2020  = 36.           
+00014460: 2020 2020 2065 6368 6172 745f 6f70 7469       echart_opti
+00014470: 6f6e 735b 2267 7269 6422 5d5b 226c 6566  ons["grid"]["lef
+00014480: 7422 5d20 3d20 2234 2522 0a20 2020 2020  t"] = "4%".     
+00014490: 2020 2020 2020 2020 2020 2061 7869 735f             axis_
+000144a0: 6f70 7469 6f6e 735b 2261 7869 7354 6963  options["axisTic
+000144b0: 6b22 5d20 3d20 7b22 7368 6f77 223a 2046  k"] = {"show": F
+000144c0: 616c 7365 7d0a 2020 2020 2020 2020 2020  alse}.          
+000144d0: 2020 2020 2020 6178 6973 5f6f 7074 696f        axis_optio
+000144e0: 6e73 5b22 6178 6973 4c69 6e65 225d 203d  ns["axisLine"] =
+000144f0: 207b 2273 686f 7722 3a20 4661 6c73 657d   {"show": False}
+00014500: 0a0a 2020 2020 2020 2020 6177 6169 7420  ..        await 
+00014510: 7365 6c66 2e5f 6372 6561 7465 5f65 6368  self._create_ech
+00014520: 6172 7428 0a20 2020 2020 2020 2020 2020  art(.           
+00014530: 206f 7264 6572 3d6f 7264 6572 2c0a 2020   order=order,.  
+00014540: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00014550: 733d 6563 6861 7274 5f6f 7074 696f 6e73  s=echart_options
+00014560: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00014570: 7461 5f6d 6170 7069 6e67 5f74 6f5f 7475  ta_mapping_to_tu
+00014580: 706c 6573 3d64 6174 615f 6d61 7070 696e  ples=data_mappin
+00014590: 675f 746f 5f74 7570 6c65 732c 0a20 2020  g_to_tuples,.   
+000145a0: 2020 2020 2020 2020 2066 6965 6c64 733d           fields=
+000145b0: 6178 6573 202b 2076 616c 7565 732c 0a20  axes + values,. 
+000145c0: 2020 2020 2020 2020 2020 202a 2a72 6570             **rep
+000145d0: 6f72 745f 7061 7261 6d73 2c0a 2020 2020  ort_params,.    
+000145e0: 2020 2020 290a 0a20 2020 2040 6164 645f      )..    @add_
+000145f0: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00014600: 5f67 726f 7570 0a20 2020 2061 7379 6e63  _group.    async
+00014610: 2064 6566 2066 7265 655f 6563 6861 7274   def free_echart
+00014620: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00014630: 0a20 2020 2020 2020 2064 6174 613a 204f  .        data: O
+00014640: 7074 696f 6e61 6c5b 556e 696f 6e5b 7374  ptional[Union[st
+00014650: 722c 2044 6174 6146 7261 6d65 2c20 6c69  r, DataFrame, li
+00014660: 7374 5b64 6963 745d 5d5d 203d 204e 6f6e  st[dict]]] = Non
+00014670: 652c 0a20 2020 2020 2020 206f 7074 696f  e,.        optio
+00014680: 6e73 3a20 4f70 7469 6f6e 616c 5b64 6963  ns: Optional[dic
+00014690: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+000146a0: 2020 2072 6177 5f6f 7074 696f 6e73 3a20     raw_options: 
+000146b0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+000146c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f72  None,.        or
+000146d0: 6465 723a 204f 7074 696f 6e61 6c5b 696e  der: Optional[in
+000146e0: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+000146f0: 2020 2074 6974 6c65 3a20 4f70 7469 6f6e     title: Option
+00014700: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
+00014710: 2020 2020 2020 2020 726f 7773 5f73 697a          rows_siz
+00014720: 653a 204f 7074 696f 6e61 6c5b 696e 745d  e: Optional[int]
+00014730: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00014740: 2063 6f6c 735f 7369 7a65 3a20 4f70 7469   cols_size: Opti
+00014750: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+00014760: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
+00014770: 673a 204f 7074 696f 6e61 6c5b 7374 725d  g: Optional[str]
+00014780: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00014790: 2066 6965 6c64 733a 204f 7074 696f 6e61   fields: Optiona
+000147a0: 6c5b 6c69 7374 5d20 3d20 4e6f 6e65 2c0a  l[list] = None,.
+000147b0: 2020 2020 2020 2020 6461 7461 5f69 735f          data_is_
+000147c0: 6e6f 745f 6466 3a20 626f 6f6c 203d 2046  not_df: bool = F
+000147d0: 616c 7365 2c0a 2020 2020 293a 0a20 2020  alse,.    ):.   
+000147e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000147f0: 2043 7265 6174 6520 616e 2065 6368 6172   Create an echar
+00014800: 7473 2063 6861 7274 2077 6974 6820 6375  ts chart with cu
+00014810: 7374 6f6d 206f 7074 696f 6e73 2e0a 2020  stom options..  
+00014820: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00014830: 613a 2074 6865 2064 6174 6120 6f66 2074  a: the data of t
+00014840: 6865 2063 6861 7274 0a20 2020 2020 2020  he chart.       
+00014850: 203a 7061 7261 6d20 6f70 7469 6f6e 733a   :param options:
+00014860: 2074 6865 206f 7074 696f 6e73 206f 6620   the options of 
+00014870: 7468 6520 6368 6172 740a 2020 2020 2020  the chart.      
+00014880: 2020 3a70 6172 616d 2072 6177 5f6f 7074    :param raw_opt
+00014890: 696f 6e73 3a20 7468 6520 7261 7720 6f70  ions: the raw op
+000148a0: 7469 6f6e 7320 6f66 2074 6865 2063 6861  tions of the cha
+000148b0: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+000148c0: 6d20 6f72 6465 723a 2074 6865 206f 7264  m order: the ord
+000148d0: 6572 206f 6620 7468 6520 6368 6172 7420  er of the chart 
+000148e0: 696e 2074 6865 2064 6173 6862 6f61 7264  in the dashboard
+000148f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00014900: 7469 746c 653a 2074 6865 2074 6974 6c65  title: the title
+00014910: 206f 6620 7468 6520 6368 6172 740a 2020   of the chart.  
+00014920: 2020 2020 2020 3a70 6172 616d 2072 6f77        :param row
+00014930: 735f 7369 7a65 3a20 7468 6520 726f 7773  s_size: the rows
+00014940: 2073 697a 6520 6f66 2074 6865 2063 6861   size of the cha
+00014950: 7274 0a20 2020 2020 2020 203a 7061 7261  rt.        :para
+00014960: 6d20 636f 6c73 5f73 697a 653a 2074 6865  m cols_size: the
+00014970: 2063 6f6c 756d 6e73 2073 697a 6520 6f66   columns size of
+00014980: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+00014990: 2020 203a 7061 7261 6d20 7061 6464 696e     :param paddin
+000149a0: 673a 2074 6865 2070 6164 6469 6e67 206f  g: the padding o
+000149b0: 6620 7468 6520 6368 6172 740a 2020 2020  f the chart.    
+000149c0: 2020 2020 3a70 6172 616d 2066 6965 6c64      :param field
+000149d0: 733a 2074 6865 2066 6965 6c64 7320 6f66  s: the fields of
+000149e0: 2074 6865 2063 6861 7274 0a20 2020 2020   the chart.     
+000149f0: 2020 203a 7061 7261 6d20 6461 7461 5f69     :param data_i
+00014a00: 735f 6e6f 745f 6466 3a20 7768 6574 6865  s_not_df: whethe
+00014a10: 7220 7468 6520 6461 7461 2069 7320 6e6f  r the data is no
+00014a20: 7420 6120 6461 7461 6672 616d 650a 2020  t a dataframe.  
+00014a30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00014a40: 2020 6966 206e 6f74 206f 7074 696f 6e73    if not options
+00014a50: 2061 6e64 206e 6f74 2072 6177 5f6f 7074   and not raw_opt
+00014a60: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00014a70: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
+00014a80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00014a90: 6765 722c 2022 4569 7468 6572 206f 7074  ger, "Either opt
+00014aa0: 696f 6e73 206f 7220 7261 775f 6f70 7469  ions or raw_opti
+00014ab0: 6f6e 7320 6d75 7374 2062 6520 7072 6f76  ons must be prov
+00014ac0: 6964 6564 222c 2056 616c 7565 4572 726f  ided", ValueErro
+00014ad0: 720a 2020 2020 2020 2020 2020 2020 290a  r.            ).
+00014ae0: 2020 2020 2020 2020 6966 206f 7074 696f          if optio
+00014af0: 6e73 2061 6e64 206e 6f74 2069 7369 6e73  ns and not isins
+00014b00: 7461 6e63 6528 6461 7461 2c20 4461 7461  tance(data, Data
+00014b10: 4672 616d 6529 2061 6e64 2064 6174 6120  Frame) and data 
+00014b20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00014b30: 2020 2020 206c 6f67 5f65 7272 6f72 280a       log_error(.
+00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b50: 6c6f 6767 6572 2c20 2264 6174 6120 6d75  logger, "data mu
+00014b60: 7374 2062 6520 7072 6f76 6964 6564 2077  st be provided w
+00014b70: 6865 6e20 6f70 7469 6f6e 7320 6973 2070  hen options is p
+00014b80: 726f 7669 6465 6422 2c20 4461 7461 4572  rovided", DataEr
+00014b90: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
+00014ba0: 290a 2020 2020 2020 2020 6966 206f 7074  ).        if opt
+00014bb0: 696f 6e73 2061 6e64 2072 6177 5f6f 7074  ions and raw_opt
+00014bc0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
+00014bd0: 2020 6c6f 675f 6572 726f 7228 0a20 2020    log_error(.   
+00014be0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00014bf0: 6765 722c 0a20 2020 2020 2020 2020 2020  ger,.           
+00014c00: 2020 2020 2022 4f6e 6c79 206f 6e65 206f       "Only one o
+00014c10: 6620 6f70 7469 6f6e 7320 616e 6420 7261  f options and ra
+00014c20: 775f 6f70 7469 6f6e 7320 6361 6e20 6265  w_options can be
+00014c30: 2070 726f 7669 6465 6422 2c0a 2020 2020   provided",.    
+00014c40: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+00014c50: 6545 7272 6f72 2c0a 2020 2020 2020 2020  eError,.        
+00014c60: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+00014c70: 6620 7261 775f 6f70 7469 6f6e 733a 0a20  f raw_options:. 
+00014c80: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00014c90: 6e73 203d 2074 7261 6e73 666f 726d 5f64  ns = transform_d
+00014ca0: 6963 745f 6a73 5f74 6f5f 7079 2872 6177  ict_js_to_py(raw
+00014cb0: 5f6f 7074 696f 6e73 290a 2020 2020 2020  _options).      
+00014cc0: 2020 2020 2020 6461 7461 203d 2072 6574        data = ret
+00014cd0: 7269 6576 655f 6461 7461 5f66 726f 6d5f  rieve_data_from_
+00014ce0: 6f70 7469 6f6e 7328 6f70 7469 6f6e 7329  options(options)
+00014cf0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+00014d00: 696f 6e73 5b22 6461 7461 7365 7422 5d20  ions["dataset"] 
+00014d10: 3d20 7b22 736f 7572 6365 223a 2022 2373  = {"source": "#s
+00014d20: 6574 5f64 6174 6123 227d 0a20 2020 2020  et_data#"}.     
+00014d30: 2020 2020 2020 2066 6965 6c64 7320 3d20         fields = 
+00014d40: 5b6c 6973 7428 6461 7461 5b30 5d2e 6b65  [list(data[0].ke
+00014d50: 7973 2829 295d 0a20 2020 2020 2020 2065  ys())].        e
+00014d60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014d70: 206f 7074 696f 6e73 203d 2064 6565 7063   options = deepc
+00014d80: 6f70 7928 6f70 7469 6f6e 7329 0a0a 2020  opy(options)..  
+00014d90: 2020 2020 2020 6177 6169 7420 7365 6c66        await self
+00014da0: 2e5f 6372 6561 7465 5f65 6368 6172 7428  ._create_echart(
+00014db0: 0a20 2020 2020 2020 2020 2020 206f 7264  .            ord
+00014dc0: 6572 3d6f 7264 6572 2c0a 2020 2020 2020  er=order,.      
+00014dd0: 2020 2020 2020 6461 7461 5f6d 6170 7069        data_mappi
+00014de0: 6e67 5f74 6f5f 7475 706c 6573 3d61 7761  ng_to_tuples=awa
+00014df0: 6974 2073 656c 662e 5f63 686f 6f73 655f  it self._choose_
+00014e00: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+00014e10: 2020 2020 2020 6f72 6465 722c 2064 6174        order, dat
+00014e20: 612c 2064 756d 705f 7768 6f6c 653d 6461  a, dump_whole=da
+00014e30: 7461 5f69 735f 6e6f 745f 6466 0a20 2020  ta_is_not_df.   
+00014e40: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+00014e50: 2020 2020 2020 2020 6669 656c 6473 3d66          fields=f
+00014e60: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+00014e70: 2020 206f 7074 696f 6e73 3d6f 7074 696f     options=optio
+00014e80: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00014e90: 7469 746c 653d 7469 746c 652c 0a20 2020  title=title,.   
+00014ea0: 2020 2020 2020 2020 2072 6f77 735f 7369           rows_si
+00014eb0: 7a65 3d72 6f77 735f 7369 7a65 2c0a 2020  ze=rows_size,.  
+00014ec0: 2020 2020 2020 2020 2020 636f 6c73 5f73            cols_s
+00014ed0: 697a 653d 636f 6c73 5f73 697a 652c 0a20  ize=cols_size,. 
+00014ee0: 2020 2020 2020 2020 2020 2070 6164 6469             paddi
+00014ef0: 6e67 3d70 6164 6469 6e67 2c0a 2020 2020  ng=padding,.    
+00014f00: 2020 2020 290a 0a20 2020 2023 2045 4368      )..    # ECh
+00014f10: 6172 7473 0a20 2020 206c 696e 6520 3d20  arts.    line = 
+00014f20: 6164 645f 746f 5f67 656e 6572 616c 5f61  add_to_general_a
+00014f30: 7379 6e63 5f67 726f 7570 286c 696e 655f  sync_group(line_
+00014f40: 6368 6172 7429 0a20 2020 2062 6172 203d  chart).    bar =
+00014f50: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
+00014f60: 6173 796e 635f 6772 6f75 7028 6261 725f  async_group(bar_
+00014f70: 6368 6172 7429 0a20 2020 2073 7461 636b  chart).    stack
+00014f80: 6564 5f62 6172 203d 2061 6464 5f74 6f5f  ed_bar = add_to_
+00014f90: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00014fa0: 6f75 7028 7374 6163 6b65 645f 6261 725f  oup(stacked_bar_
+00014fb0: 6368 6172 7429 0a20 2020 2061 7265 6120  chart).    area 
+00014fc0: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+00014fd0: 5f61 7379 6e63 5f67 726f 7570 2861 7265  _async_group(are
+00014fe0: 615f 6368 6172 7429 0a20 2020 2073 7461  a_chart).    sta
+00014ff0: 636b 6564 5f61 7265 6120 3d20 6164 645f  cked_area = add_
+00015000: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015010: 5f67 726f 7570 2873 7461 636b 6564 5f61  _group(stacked_a
+00015020: 7265 615f 6368 6172 7429 0a20 2020 2073  rea_chart).    s
+00015030: 6361 7474 6572 203d 2061 6464 5f74 6f5f  catter = add_to_
+00015040: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00015050: 6f75 7028 7363 6174 7465 725f 6368 6172  oup(scatter_char
+00015060: 7429 0a20 2020 2068 6f72 697a 6f6e 7461  t).    horizonta
+00015070: 6c5f 6261 7220 3d20 6164 645f 746f 5f67  l_bar = add_to_g
+00015080: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015090: 7570 2868 6f72 697a 6f6e 7461 6c5f 6261  up(horizontal_ba
+000150a0: 725f 6368 6172 7429 0a20 2020 2073 7461  r_chart).    sta
+000150b0: 636b 6564 5f68 6f72 697a 6f6e 7461 6c5f  cked_horizontal_
+000150c0: 6261 7220 3d20 6164 645f 746f 5f67 656e  bar = add_to_gen
+000150d0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000150e0: 2873 7461 636b 6564 5f68 6f72 697a 6f6e  (stacked_horizon
+000150f0: 7461 6c5f 6261 725f 6368 6172 7429 0a20  tal_bar_chart). 
+00015100: 2020 207a 6572 6f5f 6365 6e74 6572 6564     zero_centered
+00015110: 5f62 6172 203d 2061 6464 5f74 6f5f 6765  _bar = add_to_ge
+00015120: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+00015130: 7028 7a65 726f 5f63 656e 7465 7265 645f  p(zero_centered_
+00015140: 6261 725f 6368 6172 7429 0a20 2020 2066  bar_chart).    f
+00015150: 756e 6e65 6c20 3d20 6164 645f 746f 5f67  unnel = add_to_g
+00015160: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015170: 7570 2866 756e 6e65 6c5f 6368 6172 7429  up(funnel_chart)
+00015180: 0a20 2020 2074 7265 6520 3d20 6164 645f  .    tree = add_
+00015190: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+000151a0: 5f67 726f 7570 2874 7265 655f 6368 6172  _group(tree_char
+000151b0: 7429 0a20 2020 2072 6164 6172 203d 2061  t).    radar = a
+000151c0: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+000151d0: 796e 635f 6772 6f75 7028 7261 6461 725f  ync_group(radar_
+000151e0: 6368 6172 7429 0a20 2020 2070 6965 203d  chart).    pie =
+000151f0: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
+00015200: 6173 796e 635f 6772 6f75 7028 7069 655f  async_group(pie_
+00015210: 6368 6172 7429 0a20 2020 2064 6f75 6768  chart).    dough
+00015220: 6e75 7420 3d20 6164 645f 746f 5f67 656e  nut = add_to_gen
+00015230: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+00015240: 2864 6f75 6768 6e75 745f 6368 6172 7429  (doughnut_chart)
+00015250: 0a20 2020 2072 6f73 6520 3d20 6164 645f  .    rose = add_
+00015260: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015270: 5f67 726f 7570 2872 6f73 655f 6368 6172  _group(rose_char
+00015280: 7429 0a20 2020 2073 756e 6275 7273 7420  t).    sunburst 
+00015290: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+000152a0: 5f61 7379 6e63 5f67 726f 7570 2873 756e  _async_group(sun
+000152b0: 6275 7273 745f 6368 6172 7429 0a20 2020  burst_chart).   
+000152c0: 2074 7265 656d 6170 203d 2061 6464 5f74   treemap = add_t
+000152d0: 6f5f 6765 6e65 7261 6c5f 6173 796e 635f  o_general_async_
+000152e0: 6772 6f75 7028 7472 6565 6d61 705f 6368  group(treemap_ch
+000152f0: 6172 7429 0a20 2020 2073 616e 6b65 7920  art).    sankey 
+00015300: 3d20 6164 645f 746f 5f67 656e 6572 616c  = add_to_general
+00015310: 5f61 7379 6e63 5f67 726f 7570 2873 616e  _async_group(san
+00015320: 6b65 795f 6368 6172 7429 0a20 2020 2068  key_chart).    h
+00015330: 6561 746d 6170 203d 2061 6464 5f74 6f5f  eatmap = add_to_
+00015340: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00015350: 6f75 7028 6865 6174 6d61 705f 6368 6172  oup(heatmap_char
+00015360: 7429 0a20 2020 2070 7265 6469 6374 6976  t).    predictiv
+00015370: 655f 6c69 6e65 203d 2061 6464 5f74 6f5f  e_line = add_to_
+00015380: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00015390: 6f75 7028 7072 6564 6963 7469 7665 5f6c  oup(predictive_l
+000153a0: 696e 655f 6368 6172 7429 0a20 2020 2073  ine_chart).    s
+000153b0: 7065 6564 5f67 6175 6765 203d 2061 6464  peed_gauge = add
+000153c0: 5f74 6f5f 6765 6e65 7261 6c5f 6173 796e  _to_general_asyn
+000153d0: 635f 6772 6f75 7028 7370 6565 645f 6761  c_group(speed_ga
+000153e0: 7567 655f 6368 6172 7429 0a20 2020 2073  uge_chart).    s
+000153f0: 6869 6d6f 6b75 5f67 6175 6765 203d 2061  himoku_gauge = a
+00015400: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00015410: 796e 635f 6772 6f75 7028 7368 696d 6f6b  ync_group(shimok
+00015420: 755f 6761 7567 655f 6368 6172 7429 0a20  u_gauge_chart). 
+00015430: 2020 2073 6869 6d6f 6b75 5f67 6175 6765     shimoku_gauge
+00015440: 735f 6772 6f75 7020 3d20 6164 645f 746f  s_group = add_to
+00015450: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
+00015460: 726f 7570 2873 6869 6d6f 6b75 5f67 6175  roup(shimoku_gau
+00015470: 6765 735f 6772 6f75 7029 0a20 2020 2067  ges_group).    g
+00015480: 6175 6765 5f69 6e64 6963 6174 6f72 203d  auge_indicator =
+00015490: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
+000154a0: 6173 796e 635f 6772 6f75 7028 6761 7567  async_group(gaug
+000154b0: 655f 696e 6469 6361 746f 7229 0a20 2020  e_indicator).   
+000154c0: 2074 6f70 5f62 6f74 746f 6d5f 6172 6561   top_bottom_area
+000154d0: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+000154e0: 6c5f 6173 796e 635f 6772 6f75 7028 746f  l_async_group(to
+000154f0: 705f 626f 7474 6f6d 5f61 7265 615f 6368  p_bottom_area_ch
+00015500: 6172 7473 290a 2020 2020 746f 705f 626f  arts).    top_bo
+00015510: 7474 6f6d 5f6c 696e 6520 3d20 6164 645f  ttom_line = add_
+00015520: 746f 5f67 656e 6572 616c 5f61 7379 6e63  to_general_async
+00015530: 5f67 726f 7570 2874 6f70 5f62 6f74 746f  _group(top_botto
+00015540: 6d5f 6c69 6e65 5f63 6861 7274 7329 0a20  m_line_charts). 
+00015550: 2020 206c 696e 655f 7769 7468 5f63 6f6e     line_with_con
+00015560: 6669 6465 6e63 655f 6172 6561 203d 2061  fidence_area = a
+00015570: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00015580: 796e 635f 6772 6f75 7028 0a20 2020 2020  ync_group(.     
+00015590: 2020 206c 696e 655f 7769 7468 5f63 6f6e     line_with_con
+000155a0: 6669 6465 6e63 655f 6172 6561 5f63 6861  fidence_area_cha
+000155b0: 7274 0a20 2020 2029 0a20 2020 2073 6361  rt.    ).    sca
+000155c0: 7474 6572 5f77 6974 685f 6566 6665 6374  tter_with_effect
+000155d0: 203d 2061 6464 5f74 6f5f 6765 6e65 7261   = add_to_genera
+000155e0: 6c5f 6173 796e 635f 6772 6f75 7028 7363  l_async_group(sc
+000155f0: 6174 7465 725f 7769 7468 5f65 6666 6563  atter_with_effec
+00015600: 745f 6368 6172 7429 0a20 2020 2077 6174  t_chart).    wat
+00015610: 6572 6661 6c6c 203d 2061 6464 5f74 6f5f  erfall = add_to_
+00015620: 6765 6e65 7261 6c5f 6173 796e 635f 6772  general_async_gr
+00015630: 6f75 7028 7761 7465 7266 616c 6c5f 6368  oup(waterfall_ch
+00015640: 6172 7429 0a20 2020 206c 696e 655f 616e  art).    line_an
+00015650: 645f 6261 725f 6368 6172 7473 203d 2061  d_bar_charts = a
+00015660: 6464 5f74 6f5f 6765 6e65 7261 6c5f 6173  dd_to_general_as
+00015670: 796e 635f 6772 6f75 7028 6c69 6e65 5f61  ync_group(line_a
+00015680: 6e64 5f62 6172 5f63 6861 7274 7329 0a20  nd_bar_charts). 
+00015690: 2020 2073 6567 6d65 6e74 6564 5f6c 696e     segmented_lin
+000156a0: 6520 3d20 6164 645f 746f 5f67 656e 6572  e = add_to_gener
+000156b0: 616c 5f61 7379 6e63 5f67 726f 7570 2873  al_async_group(s
+000156c0: 6567 6d65 6e74 6564 5f6c 696e 655f 6368  egmented_line_ch
+000156d0: 6172 7429 0a20 2020 206d 6172 6b65 645f  art).    marked_
+000156e0: 6c69 6e65 203d 2061 6464 5f74 6f5f 6765  line = add_to_ge
+000156f0: 6e65 7261 6c5f 6173 796e 635f 6772 6f75  neral_async_grou
+00015700: 7028 6d61 726b 6564 5f6c 696e 655f 6368  p(marked_line_ch
+00015710: 6172 7429 0a20 2020 2073 6567 6d65 6e74  art).    segment
+00015720: 6564 5f61 7265 6120 3d20 6164 645f 746f  ed_area = add_to
+00015730: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
+00015740: 726f 7570 2873 6567 6d65 6e74 6564 5f61  roup(segmented_a
+00015750: 7265 615f 6368 6172 7429 0a0a 2020 2020  rea_chart)..    
+00015760: 2320 4265 6e74 6f62 6f78 2063 6861 7274  # Bentobox chart
+00015770: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
+00015780: 2062 656e 746f 626f 785f 6368 6172 7473   bentobox_charts
+00015790: 2e70 7920 6669 6c65 0a20 2020 2069 6e66  .py file.    inf
+000157a0: 6f67 7261 7068 6963 735f 7465 7874 5f62  ographics_text_b
+000157b0: 7562 626c 6520 3d20 6164 645f 746f 5f67  ubble = add_to_g
+000157c0: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+000157d0: 7570 2869 6e66 6f67 7261 7068 6963 735f  up(infographics_
+000157e0: 7465 7874 5f62 7562 626c 6529 0a20 2020  text_bubble).   
+000157f0: 2063 6861 7274 5f61 6e64 5f6d 6f64 616c   chart_and_modal
+00015800: 5f62 7574 746f 6e20 3d20 6164 645f 746f  _button = add_to
+00015810: 5f67 656e 6572 616c 5f61 7379 6e63 5f67  _general_async_g
+00015820: 726f 7570 2863 6861 7274 5f61 6e64 5f6d  roup(chart_and_m
+00015830: 6f64 616c 5f62 7574 746f 6e29 0a20 2020  odal_button).   
+00015840: 2063 6861 7274 5f61 6e64 5f69 6e64 6963   chart_and_indic
+00015850: 6174 6f72 7320 3d20 6164 645f 746f 5f67  ators = add_to_g
+00015860: 656e 6572 616c 5f61 7379 6e63 5f67 726f  eneral_async_gro
+00015870: 7570 2863 6861 7274 5f61 6e64 5f69 6e64  up(chart_and_ind
+00015880: 6963 6174 6f72 7329 0a20 2020 2069 6e64  icators).    ind
+00015890: 6963 6174 6f72 735f 7769 7468 5f68 6561  icators_with_hea
+000158a0: 6465 7220 3d20 6164 645f 746f 5f67 656e  der = add_to_gen
+000158b0: 6572 616c 5f61 7379 6e63 5f67 726f 7570  eral_async_group
+000158c0: 2869 6e64 6963 6174 6f72 735f 7769 7468  (indicators_with
+000158d0: 5f68 6561 6465 7229 0a20 2020 206c 696e  _header).    lin
+000158e0: 655f 7769 7468 5f73 756d 6d61 7279 203d  e_with_summary =
+000158f0: 2061 6464 5f74 6f5f 6765 6e65 7261 6c5f   add_to_general_
+00015900: 6173 796e 635f 6772 6f75 7028 6c69 6e65  async_group(line
+00015910: 5f77 6974 685f 7375 6d6d 6172 7929 0a    _with_summary).
```

### Comparing `shimoku-2.3.0/src/shimoku/plt/utils.py` & `shimoku-2.3.1/src/shimoku/plt/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku/utils.py` & `shimoku-2.3.1/src/shimoku/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/src/shimoku.egg-info/PKG-INFO` & `shimoku-2.3.1/src/shimoku.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shimoku
-Version: 2.3.0
+Version: 2.3.1
 Summary: Shimoku enables you to build Data Products in just hours and allows you to create Predictive Analytics Products with Artificial Intelligence capabilities.
 Home-page: https://github.com/shimoku-tech/shimoku-api-python
 Author: Shimoku
 Author-email: contact@shimoku.com
 License: MIT
 Project-URL: Documentation, https://docs.shimoku.com/
 Platform: any
```

### Comparing `shimoku-2.3.0/src/shimoku.egg-info/SOURCES.txt` & `shimoku-2.3.1/src/shimoku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/Jupyter_notebook_test.ipynb` & `shimoku-2.3.1/tests/Jupyter_notebook_test.ipynb`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/correct_action_scripts/correct_action.py` & `shimoku-2.3.1/tests/mockable_tests/correct_action_scripts/correct_action.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/mock_classes.py` & `shimoku-2.3.1/tests/mockable_tests/mock_classes.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_actions.py` & `shimoku-2.3.1/tests/mockable_tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_activity_metadata_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_activity_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_app_metadata_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_app_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_business_metadata_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_business_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_code_generation.py` & `shimoku-2.3.1/tests/mockable_tests/test_code_generation.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_dashboard_metadata_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_dashboard_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/annotation_chart.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/bar_and_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/bentobox.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/bentobox.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/chart_and_indicators.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/annotation_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/bar_and_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/flow_and_rainfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/free_echarts_raw.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/heatmap.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/indicator.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/input_form.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/noise.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/noise.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_test.csv`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/scatter_with_effect.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/stacked_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/suburst.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/suburst.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/table_with_labels.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/tree.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/data/waterfall.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/data/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/doughnut.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/doughnut.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/dynamic_conditional_and_auto_send_input_form.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/gauge_indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/heatmap.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/heatmap.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/horizontal_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/indicator.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/indicator.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/infographics.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/infographics.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/line_with_confidence_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/modal.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/modal.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/radar.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/radar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_area.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_area.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rainfall_line.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rainfall_line.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/rose.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/rose.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/scatter.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/scatter.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_area_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/segmented_line_chart.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/shimoku_gauges.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/table_with_lables.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/table_with_lables.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/tabs.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/tabs.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/tree.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/tree.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/variants.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/variants.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/waterfall.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/waterfall.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py` & `shimoku-2.3.1/tests/mockable_tests/test_plot_api_functions/zero_centered_bar.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_report_metadata_api.py` & `shimoku-2.3.1/tests/mockable_tests/test_report_metadata_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/test_roles.py` & `shimoku-2.3.1/tests/mockable_tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/mockable_tests/utils.py` & `shimoku-2.3.1/tests/mockable_tests/utils.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/test_ai_api.py` & `shimoku-2.3.1/tests/test_ai_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/test_components_catalog.py` & `shimoku-2.3.1/tests/test_components_catalog.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/test_data_managing_api.py` & `shimoku-2.3.1/tests/test_data_managing_api.py`

 * *Files identical despite different names*

### Comparing `shimoku-2.3.0/tests/test_file_metadata_api.py` & `shimoku-2.3.1/tests/test_file_metadata_api.py`

 * *Files identical despite different names*

