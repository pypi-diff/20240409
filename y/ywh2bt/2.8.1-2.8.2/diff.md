# Comparing `tmp/ywh2bt-2.8.1.tar.gz` & `tmp/ywh2bt-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywh2bt-2.8.1.tar", max compression
+gzip compressed data, was "ywh2bt-2.8.2.tar", max compression
```

## Comparing `ywh2bt-2.8.1.tar` & `ywh2bt-2.8.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     5309 2024-02-28 08:52:55.983249 ywh2bt-2.8.1/README.md
--rw-r--r--   0        0        0     3108 2024-02-28 09:09:03.570098 ywh2bt-2.8.1/pyproject.toml
--rw-r--r--   0        0        0       66 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/__init__.py
--rw-r--r--   0        0        0       47 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/__init__.py
--rw-r--r--   0        0        0       45 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/__init__.py
--rw-r--r--   0        0        0     2349 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/convert.py
--rw-r--r--   0        0        0      878 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/schema.py
--rw-r--r--   0        0        0     1486 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/synchronize.py
--rw-r--r--   0        0        0     1359 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/test.py
--rw-r--r--   0        0        0      680 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/commands/validate.py
--rw-r--r--   0        0        0      147 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/error.py
--rw-r--r--   0        0        0     7302 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/listener.py
--rw-r--r--   0        0        0     6218 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/cli/main.py
--rw-r--r--   0        0        0       66 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/__init__.py
--rw-r--r--   0        0        0       49 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/__init__.py
--rw-r--r--   0        0        0      274 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/client.py
--rw-r--r--   0        0        0       61 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/formatter/__init__.py
--rw-r--r--   0        0        0    11464 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/formatter/formatter.py
--rw-r--r--   0        0        0     3871 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/formatter/markdown.py
--rw-r--r--   0        0        0    12602 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/mapping.py
--rw-r--r--   0        0        0       14 2024-02-23 16:17:02.541699 ywh2bt-2.8.1/ywh2bt/core/api/models/__init__.py
--rw-r--r--   0        0        0     8104 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/models/report.py
--rw-r--r--   0        0        0     7644 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/tracker.py
--rw-r--r--   0        0        0       95 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/__init__.py
--rw-r--r--   0        0        0       96 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/github/__init__.py
--rw-r--r--   0        0        0     9460 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/github/attachment.py
--rw-r--r--   0        0        0    19721 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/github/tracker.py
--rw-r--r--   0        0        0    17796 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/gitlab.py
--rw-r--r--   0        0        0       94 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/jira/__init__.py
--rw-r--r--   0        0        0     6751 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/jira/formatter.py
--rw-r--r--   0        0        0    20811 2024-02-26 09:54:13.099748 ywh2bt-2.8.1/ywh2bt/core/api/trackers/jira/tracker.py
--rw-r--r--   0        0        0      100 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/__init__.py
--rw-r--r--   0        0        0     3513 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/formatter.py
--rw-r--r--   0        0        0     3175 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/model.py
--rw-r--r--   0        0        0    31829 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/tracker.py
--rw-r--r--   0        0        0    13748 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/api/yeswehack.py
--rw-r--r--   0        0        0       80 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/__init__.py
--rw-r--r--   0        0        0    21308 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/attribute.py
--rw-r--r--   0        0        0     2680 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/error.py
--rw-r--r--   0        0        0      354 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/exportable.py
--rw-r--r--   0        0        0      206 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/headers.py
--rw-r--r--   0        0        0     4363 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/root.py
--rw-r--r--   0        0        0     5871 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/subtypable.py
--rw-r--r--   0        0        0     2309 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/tracker.py
--rw-r--r--   0        0        0       47 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/__init__.py
--rw-r--r--   0        0        0     4910 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/github.py
--rw-r--r--   0        0        0     2615 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/gitlab.py
--rw-r--r--   0        0        0     3289 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/jira.py
--rw-r--r--   0        0        0     2604 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/servicenow.py
--rw-r--r--   0        0        0      619 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/validatable.py
--rw-r--r--   0        0        0     3691 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/validator.py
--rw-r--r--   0        0        0    12001 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/configuration/yeswehack.py
--rw-r--r--   0        0        0       56 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/converter/__init__.py
--rw-r--r--   0        0        0    29194 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/converter/html2jira.py
--rw-r--r--   0        0        0     8859 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/converter/jira2markdown.py
--rw-r--r--   0        0        0     3556 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/core.py
--rw-r--r--   0        0        0       50 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/crypt/__init__.py
--rw-r--r--   0        0        0     1195 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/crypt/decrypt.py
--rw-r--r--   0        0        0     1166 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/crypt/encrypt.py
--rw-r--r--   0        0        0      100 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/crypt/error.py
--rw-r--r--   0        0        0     1485 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/crypt/key.py
--rw-r--r--   0        0        0     3663 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/error.py
--rw-r--r--   0        0        0      102 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/exceptions.py
--rw-r--r--   0        0        0       17 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/factories/__init__.py
--rw-r--r--   0        0        0     5449 2024-02-23 16:17:02.545700 ywh2bt-2.8.1/ywh2bt/core/factories/tracker_clients.py
--rw-r--r--   0        0        0     1892 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/factories/yeswehack_api_clients.py
--rw-r--r--   0        0        0     4700 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/html.py
--rw-r--r--   0        0        0      508 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/listener.py
--rw-r--r--   0        0        0     3912 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/loader.py
--rw-r--r--   0        0        0      800 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/markdown.py
--rw-r--r--   0        0        0       44 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/__init__.py
--rw-r--r--   0        0        0      160 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/error.py
--rw-r--r--   0        0        0     7877 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/json.py
--rw-r--r--   0        0        0     5490 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/markdown.py
--rw-r--r--   0        0        0      247 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/protocol.py
--rw-r--r--   0        0        0     5044 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/schema/text.py
--rw-r--r--   0        0        0      833 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/serde.py
--rw-r--r--   0        0        0       72 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/serializers/__init__.py
--rw-r--r--   0        0        0     1223 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/serializers/json.py
--rw-r--r--   0        0        0     1334 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/serializers/yaml.py
--rw-r--r--   0        0        0       57 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/state/__init__.py
--rw-r--r--   0        0        0     2317 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/state/decrypt.py
--rw-r--r--   0        0        0     2112 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/state/encrypt.py
--rw-r--r--   0        0        0      100 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/state/error.py
--rw-r--r--   0        0        0      294 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/state/state.py
--rw-r--r--   0        0        0       89 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/synchronizer/__init__.py
--rw-r--r--   0        0        0      185 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/synchronizer/error.py
--rw-r--r--   0        0        0     2785 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/synchronizer/listener.py
--rw-r--r--   0        0        0    38097 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/synchronizer/synchronizer.py
--rw-r--r--   0        0        0       78 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/tester/__init__.py
--rw-r--r--   0        0        0      165 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/tester/error.py
--rw-r--r--   0        0        0     1928 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/tester/listener.py
--rw-r--r--   0        0        0     5135 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/core/tester/tester.py
--rw-r--r--   0        0        0       44 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/__init__.py
--rw-r--r--   0        0        0       22 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/dialog/__init__.py
--rw-r--r--   0        0        0     1561 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/dialog/error.py
--rw-r--r--   0        0        0     2461 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/dialog/file.py
--rw-r--r--   0        0        0     2190 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/dialog/schema.py
--rw-r--r--   0        0        0      667 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/hashing.py
--rw-r--r--   0        0        0     3037 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/main.py
--rw-r--r--   0        0        0    10953 2024-02-23 16:17:02.549700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/hide.png
--rw-r--r--   0        0        0     9963 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/show.png
--rw-r--r--   0        0        0     8215 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png
--rw-r--r--   0        0        0     6601 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png
--rw-r--r--   0        0        0    11199 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png
--rw-r--r--   0        0        0     7837 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png
--rw-r--r--   0        0        0     9711 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png
--rw-r--r--   0        0        0     7608 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png
--rw-r--r--   0        0        0     2375 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png
--rw-r--r--   0        0        0     1551 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png
--rw-r--r--   0        0        0     1713 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png
--rw-r--r--   0        0        0      909 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png
--rw-r--r--   0        0        0     1342 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/icons/ywh2bt.png
--rw-r--r--   0        0        0      103 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/translations/fr_FR.qm
--rw-r--r--   0        0        0      311 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/resources/translations/fr_FR.ts
--rw-r--r--   0        0        0   204272 2024-02-28 09:10:02.701205 ywh2bt-2.8.1/ywh2bt/gui/resources.py
--rw-r--r--   0        0        0     1184 2024-02-28 09:09:57.968956 ywh2bt-2.8.1/ywh2bt/gui/resources.qrc
--rw-r--r--   0        0        0      135 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/settings.py
--rw-r--r--   0        0        0     1641 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/update_resources_file.py
--rw-r--r--   0        0        0       22 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/__init__.py
--rw-r--r--   0        0        0       44 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/__init__.py
--rw-r--r--   0        0        0      342 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry.py
--rw-r--r--   0        0        0     3110 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py
--rw-r--r--   0        0        0    14047 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py
--rw-r--r--   0        0        0     7088 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py
--rw-r--r--   0        0        0    19142 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_widget.py
--rw-r--r--   0        0        0    11183 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py
--rw-r--r--   0        0        0    10705 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/exportable_list_widget.py
--rw-r--r--   0        0        0      804 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/constants.py
--rw-r--r--   0        0        0     3034 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/hinted_check_box_widget.py
--rw-r--r--   0        0        0     5466 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/logs_widget.py
--rw-r--r--   0        0        0    18444 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/main_window.py
--rw-r--r--   0        0        0     7560 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configuration_entry.py
--rw-r--r--   0        0        0    17921 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configuration_widget.py
--rw-r--r--   0        0        0    13841 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configurations_widget.py
--rw-r--r--   0        0        0     3047 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/secret_line_edit_widget.py
--rw-r--r--   0        0        0      496 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/tab_widget_helper.py
--rw-r--r--   0        0        0       51 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/thread/__init__.py
--rw-r--r--   0        0        0     7883 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/thread/synchronizer.py
--rw-r--r--   0        0        0     5260 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/thread/tester.py
--rw-r--r--   0        0        0      474 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/gui/widgets/typing.py
--rw-r--r--   0        0        0      935 2024-02-23 16:17:02.553700 ywh2bt-2.8.1/ywh2bt/size.py
--rw-r--r--   0        0        0      652 2024-02-23 16:17:02.557700 ywh2bt-2.8.1/ywh2bt/version.py
--rw-r--r--   0        0        0     7870 1970-01-01 00:00:00.000000 ywh2bt-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     5415 2024-04-08 13:43:02.897126 ywh2bt-2.8.2/README.md
+-rw-r--r--   0        0        0     3108 2024-04-08 13:43:02.905126 ywh2bt-2.8.2/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2349 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/convert.py
+-rw-r--r--   0        0        0      878 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/schema.py
+-rw-r--r--   0        0        0     1486 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/synchronize.py
+-rw-r--r--   0        0        0     1359 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/test.py
+-rw-r--r--   0        0        0      680 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/commands/validate.py
+-rw-r--r--   0        0        0      147 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/error.py
+-rw-r--r--   0        0        0     7302 2024-04-08 12:44:25.356427 ywh2bt-2.8.2/ywh2bt/cli/listener.py
+-rw-r--r--   0        0        0     6218 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/cli/main.py
+-rw-r--r--   0        0        0       66 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/client.py
+-rw-r--r--   0        0        0       61 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/formatter/__init__.py
+-rw-r--r--   0        0        0    11464 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/formatter/formatter.py
+-rw-r--r--   0        0        0     3871 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/formatter/markdown.py
+-rw-r--r--   0        0        0    12602 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/mapping.py
+-rw-r--r--   0        0        0       14 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/models/__init__.py
+-rw-r--r--   0        0        0     8104 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/models/report.py
+-rw-r--r--   0        0        0     7644 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/tracker.py
+-rw-r--r--   0        0        0       95 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/github/__init__.py
+-rw-r--r--   0        0        0     9460 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/github/attachment.py
+-rw-r--r--   0        0        0    19721 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/github/tracker.py
+-rw-r--r--   0        0        0    17796 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/gitlab.py
+-rw-r--r--   0        0        0       94 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/jira/__init__.py
+-rw-r--r--   0        0        0     6751 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/jira/formatter.py
+-rw-r--r--   0        0        0    20811 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/jira/tracker.py
+-rw-r--r--   0        0        0      100 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/__init__.py
+-rw-r--r--   0        0        0     3513 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/formatter.py
+-rw-r--r--   0        0        0     3175 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/model.py
+-rw-r--r--   0        0        0    31829 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/tracker.py
+-rw-r--r--   0        0        0    13748 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/api/yeswehack.py
+-rw-r--r--   0        0        0       80 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/configuration/__init__.py
+-rw-r--r--   0        0        0    21308 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/configuration/attribute.py
+-rw-r--r--   0        0        0     2680 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/configuration/error.py
+-rw-r--r--   0        0        0      354 2024-04-08 12:44:25.360427 ywh2bt-2.8.2/ywh2bt/core/configuration/exportable.py
+-rw-r--r--   0        0        0      206 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/headers.py
+-rw-r--r--   0        0        0     4363 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/root.py
+-rw-r--r--   0        0        0     5871 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/subtypable.py
+-rw-r--r--   0        0        0     2309 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/tracker.py
+-rw-r--r--   0        0        0       47 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/github.py
+-rw-r--r--   0        0        0     2615 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/gitlab.py
+-rw-r--r--   0        0        0     3289 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/jira.py
+-rw-r--r--   0        0        0     2604 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/servicenow.py
+-rw-r--r--   0        0        0      619 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/validatable.py
+-rw-r--r--   0        0        0     3691 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/validator.py
+-rw-r--r--   0        0        0    12001 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/configuration/yeswehack.py
+-rw-r--r--   0        0        0       56 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/converter/__init__.py
+-rw-r--r--   0        0        0    29194 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/converter/html2jira.py
+-rw-r--r--   0        0        0     8859 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/converter/jira2markdown.py
+-rw-r--r--   0        0        0     3556 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/core.py
+-rw-r--r--   0        0        0       50 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/crypt/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/crypt/decrypt.py
+-rw-r--r--   0        0        0     1166 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/crypt/encrypt.py
+-rw-r--r--   0        0        0      100 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/crypt/error.py
+-rw-r--r--   0        0        0     1485 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/crypt/key.py
+-rw-r--r--   0        0        0     3663 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/error.py
+-rw-r--r--   0        0        0      102 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/exceptions.py
+-rw-r--r--   0        0        0       17 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/factories/__init__.py
+-rw-r--r--   0        0        0     5449 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/factories/tracker_clients.py
+-rw-r--r--   0        0        0     1892 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/factories/yeswehack_api_clients.py
+-rw-r--r--   0        0        0     4757 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/html.py
+-rw-r--r--   0        0        0      508 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/listener.py
+-rw-r--r--   0        0        0     3912 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/loader.py
+-rw-r--r--   0        0        0      800 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/markdown.py
+-rw-r--r--   0        0        0       44 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/schema/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/schema/error.py
+-rw-r--r--   0        0        0     7877 2024-04-08 12:44:25.364427 ywh2bt-2.8.2/ywh2bt/core/schema/json.py
+-rw-r--r--   0        0        0     5490 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/schema/markdown.py
+-rw-r--r--   0        0        0      247 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/schema/protocol.py
+-rw-r--r--   0        0        0     5044 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/schema/text.py
+-rw-r--r--   0        0        0      833 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/serde.py
+-rw-r--r--   0        0        0       72 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/serializers/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/serializers/json.py
+-rw-r--r--   0        0        0     1334 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/serializers/yaml.py
+-rw-r--r--   0        0        0       57 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/state/__init__.py
+-rw-r--r--   0        0        0     2317 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/state/decrypt.py
+-rw-r--r--   0        0        0     2112 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/state/encrypt.py
+-rw-r--r--   0        0        0      100 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/state/error.py
+-rw-r--r--   0        0        0      294 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/state/state.py
+-rw-r--r--   0        0        0       89 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/synchronizer/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/synchronizer/error.py
+-rw-r--r--   0        0        0     2785 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/synchronizer/listener.py
+-rw-r--r--   0        0        0    38097 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/synchronizer/synchronizer.py
+-rw-r--r--   0        0        0       78 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/tester/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/tester/error.py
+-rw-r--r--   0        0        0     1928 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/tester/listener.py
+-rw-r--r--   0        0        0     5135 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/core/tester/tester.py
+-rw-r--r--   0        0        0       44 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/dialog/__init__.py
+-rw-r--r--   0        0        0     1561 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/dialog/error.py
+-rw-r--r--   0        0        0     2461 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/dialog/file.py
+-rw-r--r--   0        0        0     2190 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/dialog/schema.py
+-rw-r--r--   0        0        0      667 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/hashing.py
+-rw-r--r--   0        0        0     3037 2024-04-08 12:44:25.368427 ywh2bt-2.8.2/ywh2bt/gui/main.py
+-rw-r--r--   0        0        0    10953 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/hide.png
+-rw-r--r--   0        0        0     9963 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/show.png
+-rw-r--r--   0        0        0     8215 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png
+-rw-r--r--   0        0        0     6601 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png
+-rw-r--r--   0        0        0    11199 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png
+-rw-r--r--   0        0        0     7837 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png
+-rw-r--r--   0        0        0     9711 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png
+-rw-r--r--   0        0        0     7608 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png
+-rw-r--r--   0        0        0     2375 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png
+-rw-r--r--   0        0        0     1551 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png
+-rw-r--r--   0        0        0     1713 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png
+-rw-r--r--   0        0        0      909 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png
+-rw-r--r--   0        0        0     1342 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/icons/ywh2bt.png
+-rw-r--r--   0        0        0      103 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/translations/fr_FR.qm
+-rw-r--r--   0        0        0      311 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/resources/translations/fr_FR.ts
+-rw-r--r--   0        0        0   204317 2024-04-08 13:54:12.600320 ywh2bt-2.8.2/ywh2bt/gui/resources.py
+-rw-r--r--   0        0        0     1184 2024-04-08 13:53:55.808241 ywh2bt-2.8.2/ywh2bt/gui/resources.qrc
+-rw-r--r--   0        0        0      135 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/settings.py
+-rw-r--r--   0        0        0     1641 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/update_resources_file.py
+-rw-r--r--   0        0        0       22 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry.py
+-rw-r--r--   0        0        0     3110 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py
+-rw-r--r--   0        0        0    14047 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py
+-rw-r--r--   0        0        0     7088 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py
+-rw-r--r--   0        0        0    19142 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_widget.py
+-rw-r--r--   0        0        0    11183 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py
+-rw-r--r--   0        0        0    10705 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/exportable_list_widget.py
+-rw-r--r--   0        0        0      804 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/constants.py
+-rw-r--r--   0        0        0     3034 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/hinted_check_box_widget.py
+-rw-r--r--   0        0        0     5466 2024-04-08 12:44:25.372427 ywh2bt-2.8.2/ywh2bt/gui/widgets/logs_widget.py
+-rw-r--r--   0        0        0    18444 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/main_window.py
+-rw-r--r--   0        0        0     7560 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configuration_entry.py
+-rw-r--r--   0        0        0    17921 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configuration_widget.py
+-rw-r--r--   0        0        0    13841 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configurations_widget.py
+-rw-r--r--   0        0        0     3047 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/secret_line_edit_widget.py
+-rw-r--r--   0        0        0      496 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/tab_widget_helper.py
+-rw-r--r--   0        0        0       51 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/thread/__init__.py
+-rw-r--r--   0        0        0     7883 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/thread/synchronizer.py
+-rw-r--r--   0        0        0     5260 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/thread/tester.py
+-rw-r--r--   0        0        0      474 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/gui/widgets/typing.py
+-rw-r--r--   0        0        0      935 2024-04-08 12:44:25.376427 ywh2bt-2.8.2/ywh2bt/size.py
+-rw-r--r--   0        0        0      652 2024-04-08 12:44:25.380427 ywh2bt-2.8.2/ywh2bt/version.py
+-rw-r--r--   0        0        0     7976 1970-01-01 00:00:00.000000 ywh2bt-2.8.2/PKG-INFO
```

### Comparing `ywh2bt-2.8.1/README.md` & `ywh2bt-2.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 ## Changelog
 
 - v2.8:
     - improved Python versions support (>=3.7 to <=3.12)
     - removed the GUI from the default installation (use `pip install 'ywh2bt[gui]'` to include the GUI)
     - fixed an issue with github when the title of an issue is longer than 255 characters
     - fixed an issue with jira image previews when multiple attached images have the same name
+    - fixed an issue when a report/comment has no attachments and the description contains an invalid URL
 - v2.7:
     - added synchronization of "fix verification" logs when "Upload status updates" is checked
     - fixed an issue with jira when scope contains special markdown characters
     - fixed an issue when "Download bug trackers comments" feedback option is activated
       and bug tracker attachments do not meet platform attachments requirements (unacceptable mime-type, maximum allowed size exceeded)
     - fixed an issue with jira when the title of an issue is longer than 255 characters
 - v2.6:
```

### Comparing `ywh2bt-2.8.1/pyproject.toml` & `ywh2bt-2.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ywh2bt"
-version = "2.8.1"
+version = "2.8.2"
 description = "ywh2bt - YesWeHack to Bug Tracker"
 readme = "README.md"
 authors = ["m.honel <m.honel@yeswehack.com>"]
 maintainers = ["YesWeHack <project@yeswehack.com>"]
 repository = "https://github.com/yeswehack/ywh2bugtracker"
 classifiers = [
     "Environment :: Console",
```

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/commands/convert.py` & `ywh2bt-2.8.2/ywh2bt/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/commands/schema.py` & `ywh2bt-2.8.2/ywh2bt/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/commands/synchronize.py` & `ywh2bt-2.8.2/ywh2bt/cli/commands/synchronize.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/commands/test.py` & `ywh2bt-2.8.2/ywh2bt/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/commands/validate.py` & `ywh2bt-2.8.2/ywh2bt/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/listener.py` & `ywh2bt-2.8.2/ywh2bt/cli/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/cli/main.py` & `ywh2bt-2.8.2/ywh2bt/cli/main.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/formatter/formatter.py` & `ywh2bt-2.8.2/ywh2bt/core/api/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/formatter/markdown.py` & `ywh2bt-2.8.2/ywh2bt/core/api/formatter/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/mapping.py` & `ywh2bt-2.8.2/ywh2bt/core/api/mapping.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/models/report.py` & `ywh2bt-2.8.2/ywh2bt/core/api/models/report.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/tracker.py` & `ywh2bt-2.8.2/ywh2bt/core/api/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/github/attachment.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/github/attachment.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/github/tracker.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/github/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/gitlab.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/gitlab.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/jira/formatter.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/jira/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/jira/tracker.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/jira/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/formatter.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/formatter.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/model.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/model.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/trackers/servicenow/tracker.py` & `ywh2bt-2.8.2/ywh2bt/core/api/trackers/servicenow/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/api/yeswehack.py` & `ywh2bt-2.8.2/ywh2bt/core/api/yeswehack.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/attribute.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/attribute.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/error.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/root.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/root.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/subtypable.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/subtypable.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/tracker.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/tracker.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/github.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/github.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/gitlab.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/gitlab.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/jira.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/jira.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/trackers/servicenow.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/trackers/servicenow.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/validatable.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/validatable.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/validator.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/validator.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/configuration/yeswehack.py` & `ywh2bt-2.8.2/ywh2bt/core/configuration/yeswehack.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/converter/html2jira.py` & `ywh2bt-2.8.2/ywh2bt/core/converter/html2jira.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/converter/jira2markdown.py` & `ywh2bt-2.8.2/ywh2bt/core/converter/jira2markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/core.py` & `ywh2bt-2.8.2/ywh2bt/core/core.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/crypt/decrypt.py` & `ywh2bt-2.8.2/ywh2bt/core/crypt/decrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/crypt/encrypt.py` & `ywh2bt-2.8.2/ywh2bt/core/crypt/encrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/crypt/key.py` & `ywh2bt-2.8.2/ywh2bt/core/crypt/key.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/error.py` & `ywh2bt-2.8.2/ywh2bt/core/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/factories/tracker_clients.py` & `ywh2bt-2.8.2/ywh2bt/core/factories/tracker_clients.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/factories/yeswehack_api_clients.py` & `ywh2bt-2.8.2/ywh2bt/core/factories/yeswehack_api_clients.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/html.py` & `ywh2bt-2.8.2/ywh2bt/core/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,16 @@
     Args:
         html: an html
         attachments: a list of attachments
 
     Returns:
         the cleaned html
     """
+    if not attachments:
+        return html, attachments
     clean_attachments = []
     clean_attachments_urls = []
     attachments_domains: Set[str] = set()
     for attachment in attachments:
         parsed_url = urlsplit(attachment.url)
         attachments_domains.add(parsed_url.netloc)
         clean_attachment = deepcopy(attachment)
```

### Comparing `ywh2bt-2.8.1/ywh2bt/core/loader.py` & `ywh2bt-2.8.2/ywh2bt/core/loader.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/markdown.py` & `ywh2bt-2.8.2/ywh2bt/core/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/schema/json.py` & `ywh2bt-2.8.2/ywh2bt/core/schema/json.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/schema/markdown.py` & `ywh2bt-2.8.2/ywh2bt/core/schema/markdown.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/schema/text.py` & `ywh2bt-2.8.2/ywh2bt/core/schema/text.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/serde.py` & `ywh2bt-2.8.2/ywh2bt/core/serde.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/serializers/json.py` & `ywh2bt-2.8.2/ywh2bt/core/serializers/json.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/serializers/yaml.py` & `ywh2bt-2.8.2/ywh2bt/core/serializers/yaml.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/state/decrypt.py` & `ywh2bt-2.8.2/ywh2bt/core/state/decrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/state/encrypt.py` & `ywh2bt-2.8.2/ywh2bt/core/state/encrypt.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/synchronizer/listener.py` & `ywh2bt-2.8.2/ywh2bt/core/synchronizer/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/synchronizer/synchronizer.py` & `ywh2bt-2.8.2/ywh2bt/core/synchronizer/synchronizer.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/tester/listener.py` & `ywh2bt-2.8.2/ywh2bt/core/tester/listener.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/core/tester/tester.py` & `ywh2bt-2.8.2/ywh2bt/core/tester/tester.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/dialog/error.py` & `ywh2bt-2.8.2/ywh2bt/gui/dialog/error.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/dialog/file.py` & `ywh2bt-2.8.2/ywh2bt/gui/dialog/file.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/dialog/schema.py` & `ywh2bt-2.8.2/ywh2bt/gui/dialog/schema.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/hashing.py` & `ywh2bt-2.8.2/ywh2bt/gui/hashing.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/main.py` & `ywh2bt-2.8.2/ywh2bt/gui/main.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/hide.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/hide.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/show.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/show.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitHubConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/GitLabConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/JiraConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration-2x.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/types/YesWeHackConfiguration.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources/icons/ywh2bt.png` & `ywh2bt-2.8.2/ywh2bt/gui/resources/icons/ywh2bt.png`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources.py` & `ywh2bt-2.8.2/ywh2bt/gui/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -5168,47 +5168,47 @@
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x02\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x18\x00\x02\x00\x00\x00\x04\x00\x00\x00\x06\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00(\x00\x02\x00\x00\x00\x02\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00F\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x00\x5c\x00\x00\x00\x00\x00\x01\x00\x00\x01;\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x00r\x00\x02\x00\x00\x00\x03\x00\x00\x00\x0a\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\xae\x00\x00\x00\x00\x00\x01\x00\x00Sb\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x00\x98\x00\x00\x00\x00\x00\x01\x00\x00,s\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x00\x82\x00\x00\x00\x00\x00\x01\x00\x00\x01\xa6\
-\x00\x00\x01\x8d\xd6\xc1\x82U\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x010\x00\x00\x00\x00\x00\x01\x00\x00\x5c5\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x00\xc8\x00\x00\x00\x00\x00\x01\x00\x00X\xa4\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x01\x02\x00\x02\x00\x00\x00\x08\x00\x00\x00\x0d\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x02\xc0\x00\x00\x00\x00\x00\x01\x00\x00\xe8\x8d\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x02\x16\x00\x00\x00\x00\x00\x01\x00\x00\xa6\xd4\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x02J\x00\x00\x00\x00\x00\x01\x00\x00\xc0\xa1\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x01\xac\x00\x00\x00\x00\x00\x01\x00\x00h\xfd\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x01p\x00\x00\x00\x00\x00\x01\x00\x00b\xea\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x01\x0e\x80\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x01\xdc\x00\x00\x00\x00\x00\x01\x00\x00\x86\xb9\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 \x00\x00\x02~\x00\x00\x00\x00\x00\x01\x00\x00\xdfB\
-\x00\x00\x01\x8d\xd6\xc1\x82Y\
+\x00\x00\x01\x8e\xbd\xbd\x05\x9c\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/resources.qrc` & `ywh2bt-2.8.2/ywh2bt/gui/resources.qrc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!DOCTYPE RCC>
 <RCC version="1.0">
     <qresource>
+        <file>resources/translations/fr_FR.qm</file>
+        <file>resources/translations/fr_FR.ts</file>
         <file>resources/icons/hide.png</file>
         <file>resources/icons/ywh2bt.png</file>
         <file>resources/icons/show.png</file>
-        <file>resources/icons/types/YesWeHackConfiguration.png</file>
         <file>resources/icons/types/YesWeHackConfiguration-2x.png</file>
-        <file>resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png</file>
+        <file>resources/icons/types/YesWeHackConfiguration.png</file>
+        <file>resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png</file>
         <file>resources/icons/types/TrackerConfiguration/GitLabConfiguration-2x.png</file>
-        <file>resources/icons/types/TrackerConfiguration/GitLabConfiguration.png</file>
+        <file>resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png</file>
         <file>resources/icons/types/TrackerConfiguration/ServiceNowConfiguration.png</file>
-        <file>resources/icons/types/TrackerConfiguration/ServiceNowConfiguration-2x.png</file>
-        <file>resources/icons/types/TrackerConfiguration/GitHubConfiguration.png</file>
+        <file>resources/icons/types/TrackerConfiguration/JiraConfiguration-2x.png</file>
+        <file>resources/icons/types/TrackerConfiguration/GitLabConfiguration.png</file>
         <file>resources/icons/types/TrackerConfiguration/JiraConfiguration.png</file>
-        <file>resources/icons/types/TrackerConfiguration/GitHubConfiguration-2x.png</file>
-        <file>resources/translations/fr_FR.qm</file>
-        <file>resources/translations/fr_FR.ts</file>
+        <file>resources/icons/types/TrackerConfiguration/GitHubConfiguration.png</file>
     </qresource>
 </RCC>
```

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/update_resources_file.py` & `ywh2bt-2.8.2/ywh2bt/gui/update_resources_file.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_dict_entry_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_dict_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_list_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/attributes_container_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/attributes_container_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/exportable_dict_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/attribute/exportable_list_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/attribute/exportable_list_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/constants.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/constants.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/hinted_check_box_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/hinted_check_box_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/logs_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/logs_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/main_window.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configuration_entry.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configuration_entry.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configuration_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configuration_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/root_configurations_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/root_configurations_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/secret_line_edit_widget.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/secret_line_edit_widget.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/thread/synchronizer.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/thread/synchronizer.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/gui/widgets/thread/tester.py` & `ywh2bt-2.8.2/ywh2bt/gui/widgets/thread/tester.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/size.py` & `ywh2bt-2.8.2/ywh2bt/size.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/ywh2bt/version.py` & `ywh2bt-2.8.2/ywh2bt/version.py`

 * *Files identical despite different names*

### Comparing `ywh2bt-2.8.1/PKG-INFO` & `ywh2bt-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ywh2bt
-Version: 2.8.1
+Version: 2.8.2
 Summary: ywh2bt - YesWeHack to Bug Tracker
 Home-page: https://github.com/yeswehack/ywh2bugtracker
 Author: m.honel
 Author-email: m.honel@yeswehack.com
 Maintainer: YesWeHack
 Maintainer-email: project@yeswehack.com
 Requires-Python: >=3.7.0,<3.13
@@ -107,14 +107,15 @@
 ## Changelog
 
 - v2.8:
     - improved Python versions support (>=3.7 to <=3.12)
     - removed the GUI from the default installation (use `pip install 'ywh2bt[gui]'` to include the GUI)
     - fixed an issue with github when the title of an issue is longer than 255 characters
     - fixed an issue with jira image previews when multiple attached images have the same name
+    - fixed an issue when a report/comment has no attachments and the description contains an invalid URL
 - v2.7:
     - added synchronization of "fix verification" logs when "Upload status updates" is checked
     - fixed an issue with jira when scope contains special markdown characters
     - fixed an issue when "Download bug trackers comments" feedback option is activated
       and bug tracker attachments do not meet platform attachments requirements (unacceptable mime-type, maximum allowed size exceeded)
     - fixed an issue with jira when the title of an issue is longer than 255 characters
 - v2.6:
```

