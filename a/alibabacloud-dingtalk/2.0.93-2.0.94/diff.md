# Comparing `tmp/alibabacloud_dingtalk-2.0.93.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.93.tar", last modified: Tue Apr  2 10:37:19 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.94.tar", last modified: Tue Apr  9 03:07:04 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.93.tar` & `alibabacloud_dingtalk-2.0.94.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/
--rw-r--r--   0 root         (0) root         (0)   117264 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3844 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2556 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2641 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17374 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19132 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67784 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    97238 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143446 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   199904 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328156 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   412861 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252718 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   604351 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136559 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208354 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25614 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31620 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   161460 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    87250 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73122 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129616 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194138 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   407479 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   488736 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   727920 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3844 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14081 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/
+-rw-r--r--   0 root         (0) root         (0)   118791 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18818 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71584 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101499 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143706 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   201494 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252718 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   604351 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25614 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31620 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   161460 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73122 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129616 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194138 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   407479 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   488736 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   727920 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14081 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-09 03:07:04.000000 alibabacloud_dingtalk-2.0.94/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-09 03:07:03.000000 alibabacloud_dingtalk-2.0.94/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.93/ChangeLog.md` & `alibabacloud_dingtalk-2.0.94/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-02 Version: 2.0.93
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-03-26 Version: 2.0.92
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-21 Version: 2.0.91
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-20 Version: 2.0.90
```

### Comparing `alibabacloud_dingtalk-2.0.93/LICENSE` & `alibabacloud_dingtalk-2.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/PKG-INFO` & `alibabacloud_dingtalk-2.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.93
+Version: 2.0.94
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,amdp_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dingtalk-2.0.93/README-CN.md` & `alibabacloud_dingtalk-2.0.94/README-CN.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,amdp_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_dingtalk-2.0.93/README.md` & `alibabacloud_dingtalk-2.0.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,amdp_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,16 +123,14 @@
     ) -> dingtalkai_interaction__1__0_models.PrepareResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.content):
             body['content'] = request.content
         if not UtilClient.is_unset(request.content_type):
             body['contentType'] = request.content_type
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
         if not UtilClient.is_unset(request.open_conversation_id):
             body['openConversationId'] = request.open_conversation_id
         if not UtilClient.is_unset(request.union_id):
             body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -166,16 +164,14 @@
     ) -> dingtalkai_interaction__1__0_models.PrepareResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.content):
             body['content'] = request.content
         if not UtilClient.is_unset(request.content_type):
             body['contentType'] = request.content_type
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
         if not UtilClient.is_unset(request.open_conversation_id):
             body['openConversationId'] = request.open_conversation_id
         if not UtilClient.is_unset(request.union_id):
             body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,21 +195,19 @@
 
 
 class PrepareRequest(TeaModel):
     def __init__(
         self,
         content: str = None,
         content_type: str = None,
-        conversation_type: str = None,
         open_conversation_id: str = None,
         union_id: str = None,
     ):
         self.content = content
         self.content_type = content_type
-        self.conversation_type = conversation_type
         self.open_conversation_id = open_conversation_id
         self.union_id = union_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -218,30 +216,26 @@
             return _map
 
         result = dict()
         if self.content is not None:
             result['content'] = self.content
         if self.content_type is not None:
             result['contentType'] = self.content_type
-        if self.conversation_type is not None:
-            result['conversationType'] = self.conversation_type
         if self.open_conversation_id is not None:
             result['openConversationId'] = self.open_conversation_id
         if self.union_id is not None:
             result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('content') is not None:
             self.content = m.get('content')
         if m.get('contentType') is not None:
             self.content_type = m.get('contentType')
-        if m.get('conversationType') is not None:
-            self.conversation_type = m.get('conversationType')
         if m.get('openConversationId') is not None:
             self.open_conversation_id = m.get('openConversationId')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,104 @@
         self,
         request: dingtalkbizfinance__2__0_models.GetProjectRequest,
     ) -> dingtalkbizfinance__2__0_models.GetProjectResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkbizfinance__2__0_models.GetProjectHeaders()
         return await self.get_project_with_options_async(request, headers, runtime)
 
+    def get_receipt_with_options(
+        self,
+        request: dingtalkbizfinance__2__0_models.GetReceiptRequest,
+        headers: dingtalkbizfinance__2__0_models.GetReceiptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.GetReceiptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.code):
+            query['code'] = request.code
+        if not UtilClient.is_unset(request.model_id):
+            query['modelId'] = request.model_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetReceipt',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/receipts/details',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.GetReceiptResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_receipt_with_options_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.GetReceiptRequest,
+        headers: dingtalkbizfinance__2__0_models.GetReceiptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.GetReceiptResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.code):
+            query['code'] = request.code
+        if not UtilClient.is_unset(request.model_id):
+            query['modelId'] = request.model_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetReceipt',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/receipts/details',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.GetReceiptResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_receipt(
+        self,
+        request: dingtalkbizfinance__2__0_models.GetReceiptRequest,
+    ) -> dingtalkbizfinance__2__0_models.GetReceiptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.GetReceiptHeaders()
+        return self.get_receipt_with_options(request, headers, runtime)
+
+    async def get_receipt_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.GetReceiptRequest,
+    ) -> dingtalkbizfinance__2__0_models.GetReceiptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.GetReceiptHeaders()
+        return await self.get_receipt_with_options_async(request, headers, runtime)
+
     def get_supplier_with_options(
         self,
         request: dingtalkbizfinance__2__0_models.GetSupplierRequest,
         headers: dingtalkbizfinance__2__0_models.GetSupplierHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__2__0_models.GetSupplierResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,14 +849,166 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetReceiptHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetReceiptRequest(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        model_id: str = None,
+    ):
+        self.code = code
+        self.model_id = model_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['code'] = self.code
+        if self.model_id is not None:
+            result['modelId'] = self.model_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('modelId') is not None:
+            self.model_id = m.get('modelId')
+        return self
+
+
+class GetReceiptResponseBody(TeaModel):
+    def __init__(
+        self,
+        app_id: str = None,
+        data: str = None,
+        model_id: str = None,
+        source: str = None,
+    ):
+        self.app_id = app_id
+        self.data = data
+        self.model_id = model_id
+        self.source = source
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_id is not None:
+            result['appId'] = self.app_id
+        if self.data is not None:
+            result['data'] = self.data
+        if self.model_id is not None:
+            result['modelId'] = self.model_id
+        if self.source is not None:
+            result['source'] = self.source
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appId') is not None:
+            self.app_id = m.get('appId')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        if m.get('modelId') is not None:
+            self.model_id = m.get('modelId')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        return self
+
+
+class GetReceiptResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetReceiptResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetReceiptResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetSupplierHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1094,14 +1094,16 @@
         headers: dingtalkconference__1__0_models.InviteUsersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.InviteUsersResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.invitee_list):
             body['inviteeList'] = request.invitee_list
+        if not UtilClient.is_unset(request.phone_invitee_list):
+            body['phoneInviteeList'] = request.phone_invitee_list
         if not UtilClient.is_unset(request.union_id):
             body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -1132,14 +1134,16 @@
         headers: dingtalkconference__1__0_models.InviteUsersHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.InviteUsersResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.invitee_list):
             body['inviteeList'] = request.invitee_list
+        if not UtilClient.is_unset(request.phone_invitee_list):
+            body['phoneInviteeList'] = request.phone_invitee_list
         if not UtilClient.is_unset(request.union_id):
             body['unionId'] = request.union_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2384,50 +2384,98 @@
         if m.get('nick') is not None:
             self.nick = m.get('nick')
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         return self
 
 
+class InviteUsersRequestPhoneInviteeList(TeaModel):
+    def __init__(
+        self,
+        nick: str = None,
+        phone_number: str = None,
+    ):
+        self.nick = nick
+        self.phone_number = phone_number
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.nick is not None:
+            result['nick'] = self.nick
+        if self.phone_number is not None:
+            result['phoneNumber'] = self.phone_number
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('nick') is not None:
+            self.nick = m.get('nick')
+        if m.get('phoneNumber') is not None:
+            self.phone_number = m.get('phoneNumber')
+        return self
+
+
 class InviteUsersRequest(TeaModel):
     def __init__(
         self,
         invitee_list: List[InviteUsersRequestInviteeList] = None,
+        phone_invitee_list: List[InviteUsersRequestPhoneInviteeList] = None,
         union_id: str = None,
     ):
         self.invitee_list = invitee_list
+        self.phone_invitee_list = phone_invitee_list
         self.union_id = union_id
 
     def validate(self):
         if self.invitee_list:
             for k in self.invitee_list:
                 if k:
                     k.validate()
+        if self.phone_invitee_list:
+            for k in self.phone_invitee_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         result['inviteeList'] = []
         if self.invitee_list is not None:
             for k in self.invitee_list:
                 result['inviteeList'].append(k.to_map() if k else None)
+        result['phoneInviteeList'] = []
+        if self.phone_invitee_list is not None:
+            for k in self.phone_invitee_list:
+                result['phoneInviteeList'].append(k.to_map() if k else None)
         if self.union_id is not None:
             result['unionId'] = self.union_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.invitee_list = []
         if m.get('inviteeList') is not None:
             for k in m.get('inviteeList'):
                 temp_model = InviteUsersRequestInviteeList()
                 self.invitee_list.append(temp_model.from_map(k))
+        self.phone_invitee_list = []
+        if m.get('phoneInviteeList') is not None:
+            for k in m.get('phoneInviteeList'):
+                temp_model = InviteUsersRequestPhoneInviteeList()
+                self.phone_invitee_list.append(temp_model.from_map(k))
         if m.get('unionId') is not None:
             self.union_id = m.get('unionId')
         return self
 
 
 class InviteUsersResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7087,14 +7087,140 @@
         self,
         request: dingtalkcontact__1__0_models.UpdateSeniorSettingRequest,
     ) -> dingtalkcontact__1__0_models.UpdateSeniorSettingResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcontact__1__0_models.UpdateSeniorSettingHeaders()
         return await self.update_senior_setting_with_options_async(request, headers, runtime)
 
+    def update_title_audit_status_with_options(
+        self,
+        request: dingtalkcontact__1__0_models.UpdateTitleAuditStatusRequest,
+        headers: dingtalkcontact__1__0_models.UpdateTitleAuditStatusHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.auth_status):
+            body['authStatus'] = request.auth_status
+        if not UtilClient.is_unset(request.education_level):
+            body['educationLevel'] = request.education_level
+        if not UtilClient.is_unset(request.extension):
+            body['extension'] = request.extension
+        if not UtilClient.is_unset(request.major):
+            body['major'] = request.major
+        if not UtilClient.is_unset(request.position):
+            body['position'] = request.position
+        if not UtilClient.is_unset(request.reason_code):
+            body['reasonCode'] = request.reason_code
+        if not UtilClient.is_unset(request.reason_msg):
+            body['reasonMsg'] = request.reason_msg
+        if not UtilClient.is_unset(request.school):
+            body['school'] = request.school
+        if not UtilClient.is_unset(request.type):
+            body['type'] = request.type
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.uuid):
+            body['uuid'] = request.uuid
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateTitleAuditStatus',
+            version='contact_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contact/userTitles/auditStatuses',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def update_title_audit_status_with_options_async(
+        self,
+        request: dingtalkcontact__1__0_models.UpdateTitleAuditStatusRequest,
+        headers: dingtalkcontact__1__0_models.UpdateTitleAuditStatusHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.auth_status):
+            body['authStatus'] = request.auth_status
+        if not UtilClient.is_unset(request.education_level):
+            body['educationLevel'] = request.education_level
+        if not UtilClient.is_unset(request.extension):
+            body['extension'] = request.extension
+        if not UtilClient.is_unset(request.major):
+            body['major'] = request.major
+        if not UtilClient.is_unset(request.position):
+            body['position'] = request.position
+        if not UtilClient.is_unset(request.reason_code):
+            body['reasonCode'] = request.reason_code
+        if not UtilClient.is_unset(request.reason_msg):
+            body['reasonMsg'] = request.reason_msg
+        if not UtilClient.is_unset(request.school):
+            body['school'] = request.school
+        if not UtilClient.is_unset(request.type):
+            body['type'] = request.type
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.uuid):
+            body['uuid'] = request.uuid
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateTitleAuditStatus',
+            version='contact_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contact/userTitles/auditStatuses',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def update_title_audit_status(
+        self,
+        request: dingtalkcontact__1__0_models.UpdateTitleAuditStatusRequest,
+    ) -> dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontact__1__0_models.UpdateTitleAuditStatusHeaders()
+        return self.update_title_audit_status_with_options(request, headers, runtime)
+
+    async def update_title_audit_status_async(
+        self,
+        request: dingtalkcontact__1__0_models.UpdateTitleAuditStatusRequest,
+    ) -> dingtalkcontact__1__0_models.UpdateTitleAuditStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontact__1__0_models.UpdateTitleAuditStatusHeaders()
+        return await self.update_title_audit_status_with_options_async(request, headers, runtime)
+
     def update_user_ownness_with_options(
         self,
         user_id: str,
         request: dingtalkcontact__1__0_models.UpdateUserOwnnessRequest,
         headers: dingtalkcontact__1__0_models.UpdateUserOwnnessHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcontact__1__0_models.UpdateUserOwnnessResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13161,14 +13161,202 @@
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
+class UpdateTitleAuditStatusHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class UpdateTitleAuditStatusRequest(TeaModel):
+    def __init__(
+        self,
+        auth_status: str = None,
+        education_level: str = None,
+        extension: str = None,
+        major: str = None,
+        position: str = None,
+        reason_code: str = None,
+        reason_msg: str = None,
+        school: str = None,
+        type: str = None,
+        union_id: str = None,
+        uuid: str = None,
+    ):
+        self.auth_status = auth_status
+        self.education_level = education_level
+        self.extension = extension
+        self.major = major
+        self.position = position
+        self.reason_code = reason_code
+        self.reason_msg = reason_msg
+        self.school = school
+        self.type = type
+        self.union_id = union_id
+        self.uuid = uuid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_status is not None:
+            result['authStatus'] = self.auth_status
+        if self.education_level is not None:
+            result['educationLevel'] = self.education_level
+        if self.extension is not None:
+            result['extension'] = self.extension
+        if self.major is not None:
+            result['major'] = self.major
+        if self.position is not None:
+            result['position'] = self.position
+        if self.reason_code is not None:
+            result['reasonCode'] = self.reason_code
+        if self.reason_msg is not None:
+            result['reasonMsg'] = self.reason_msg
+        if self.school is not None:
+            result['school'] = self.school
+        if self.type is not None:
+            result['type'] = self.type
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.uuid is not None:
+            result['uuid'] = self.uuid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('authStatus') is not None:
+            self.auth_status = m.get('authStatus')
+        if m.get('educationLevel') is not None:
+            self.education_level = m.get('educationLevel')
+        if m.get('extension') is not None:
+            self.extension = m.get('extension')
+        if m.get('major') is not None:
+            self.major = m.get('major')
+        if m.get('position') is not None:
+            self.position = m.get('position')
+        if m.get('reasonCode') is not None:
+            self.reason_code = m.get('reasonCode')
+        if m.get('reasonMsg') is not None:
+            self.reason_msg = m.get('reasonMsg')
+        if m.get('school') is not None:
+            self.school = m.get('school')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('uuid') is not None:
+            self.uuid = m.get('uuid')
+        return self
+
+
+class UpdateTitleAuditStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class UpdateTitleAuditStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateTitleAuditStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = UpdateTitleAuditStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateUserOwnnessHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1119,14 +1119,16 @@
     ) -> dingtalkhrm__1__0_models.HrmPtsServiceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.env):
             body['env'] = request.env
         if not UtilClient.is_unset(request.method):
             body['method'] = request.method
+        if not UtilClient.is_unset(request.outer_id):
+            body['outerId'] = request.outer_id
         if not UtilClient.is_unset(request.params):
             body['params'] = request.params
         if not UtilClient.is_unset(request.path):
             body['path'] = request.path
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
@@ -1160,14 +1162,16 @@
     ) -> dingtalkhrm__1__0_models.HrmPtsServiceResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.env):
             body['env'] = request.env
         if not UtilClient.is_unset(request.method):
             body['method'] = request.method
+        if not UtilClient.is_unset(request.outer_id):
+            body['outerId'] = request.outer_id
         if not UtilClient.is_unset(request.params):
             body['params'] = request.params
         if not UtilClient.is_unset(request.path):
             body['path'] = request.path
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2204,19 +2204,21 @@
 
 
 class HrmPtsServiceRequest(TeaModel):
     def __init__(
         self,
         env: str = None,
         method: str = None,
+        outer_id: str = None,
         params: Any = None,
         path: str = None,
     ):
         self.env = env
         self.method = method
+        self.outer_id = outer_id
         self.params = params
         self.path = path
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2225,26 +2227,30 @@
             return _map
 
         result = dict()
         if self.env is not None:
             result['env'] = self.env
         if self.method is not None:
             result['method'] = self.method
+        if self.outer_id is not None:
+            result['outerId'] = self.outer_id
         if self.params is not None:
             result['params'] = self.params
         if self.path is not None:
             result['path'] = self.path
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('env') is not None:
             self.env = m.get('env')
         if m.get('method') is not None:
             self.method = m.get('method')
+        if m.get('outerId') is not None:
+            self.outer_id = m.get('outerId')
         if m.get('params') is not None:
             self.params = m.get('params')
         if m.get('path') is not None:
             self.path = m.get('path')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -907,14 +907,116 @@
         self,
         request: dingtalkstorage__2__0_models.SearchDentriesRequest,
     ) -> dingtalkstorage__2__0_models.SearchDentriesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkstorage__2__0_models.SearchDentriesHeaders()
         return await self.search_dentries_with_options_async(request, headers, runtime)
 
+    def search_publish_dentries_with_options(
+        self,
+        request: dingtalkstorage__2__0_models.SearchPublishDentriesRequest,
+        headers: dingtalkstorage__2__0_models.SearchPublishDentriesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.SearchPublishDentriesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.keyword):
+            body['keyword'] = request.keyword
+        if not UtilClient.is_unset(request.option):
+            body['option'] = request.option
+        if not UtilClient.is_unset(request.workspace_id):
+            body['workspaceId'] = request.workspace_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SearchPublishDentries',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/publishDentries/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.SearchPublishDentriesResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def search_publish_dentries_with_options_async(
+        self,
+        request: dingtalkstorage__2__0_models.SearchPublishDentriesRequest,
+        headers: dingtalkstorage__2__0_models.SearchPublishDentriesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkstorage__2__0_models.SearchPublishDentriesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operator_id):
+            query['operatorId'] = request.operator_id
+        body = {}
+        if not UtilClient.is_unset(request.keyword):
+            body['keyword'] = request.keyword
+        if not UtilClient.is_unset(request.option):
+            body['option'] = request.option
+        if not UtilClient.is_unset(request.workspace_id):
+            body['workspaceId'] = request.workspace_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SearchPublishDentries',
+            version='storage_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/storage/publishDentries/search',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkstorage__2__0_models.SearchPublishDentriesResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def search_publish_dentries(
+        self,
+        request: dingtalkstorage__2__0_models.SearchPublishDentriesRequest,
+    ) -> dingtalkstorage__2__0_models.SearchPublishDentriesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.SearchPublishDentriesHeaders()
+        return self.search_publish_dentries_with_options(request, headers, runtime)
+
+    async def search_publish_dentries_async(
+        self,
+        request: dingtalkstorage__2__0_models.SearchPublishDentriesRequest,
+    ) -> dingtalkstorage__2__0_models.SearchPublishDentriesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkstorage__2__0_models.SearchPublishDentriesHeaders()
+        return await self.search_publish_dentries_with_options_async(request, headers, runtime)
+
     def search_workspaces_with_options(
         self,
         request: dingtalkstorage__2__0_models.SearchWorkspacesRequest,
         headers: dingtalkstorage__2__0_models.SearchWorkspacesHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkstorage__2__0_models.SearchWorkspacesResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2331,14 +2331,254 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SearchDentriesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SearchPublishDentriesHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SearchPublishDentriesRequestOption(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class SearchPublishDentriesRequest(TeaModel):
+    def __init__(
+        self,
+        keyword: str = None,
+        option: SearchPublishDentriesRequestOption = None,
+        workspace_id: str = None,
+        operator_id: str = None,
+    ):
+        self.keyword = keyword
+        self.option = option
+        self.workspace_id = workspace_id
+        self.operator_id = operator_id
+
+    def validate(self):
+        if self.option:
+            self.option.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.keyword is not None:
+            result['keyword'] = self.keyword
+        if self.option is not None:
+            result['option'] = self.option.to_map()
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        if self.operator_id is not None:
+            result['operatorId'] = self.operator_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('keyword') is not None:
+            self.keyword = m.get('keyword')
+        if m.get('option') is not None:
+            temp_model = SearchPublishDentriesRequestOption()
+            self.option = temp_model.from_map(m['option'])
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        if m.get('operatorId') is not None:
+            self.operator_id = m.get('operatorId')
+        return self
+
+
+class SearchPublishDentriesResponseBodyItems(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        path: str = None,
+        summary: str = None,
+        url: str = None,
+    ):
+        self.name = name
+        self.path = path
+        self.summary = summary
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.path is not None:
+            result['path'] = self.path
+        if self.summary is not None:
+            result['summary'] = self.summary
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('path') is not None:
+            self.path = m.get('path')
+        if m.get('summary') is not None:
+            self.summary = m.get('summary')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class SearchPublishDentriesResponseBody(TeaModel):
+    def __init__(
+        self,
+        items: List[SearchPublishDentriesResponseBodyItems] = None,
+        next_token: str = None,
+    ):
+        self.items = items
+        self.next_token = next_token
+
+    def validate(self):
+        if self.items:
+            for k in self.items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['items'] = []
+        if self.items is not None:
+            for k in self.items:
+                result['items'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.items = []
+        if m.get('items') is not None:
+            for k in m.get('items'):
+                temp_model = SearchPublishDentriesResponseBodyItems()
+                self.items.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class SearchPublishDentriesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SearchPublishDentriesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SearchPublishDentriesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchWorkspacesHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.93
+Version: 2.0.94
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,amdp_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.94/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.93/setup.py` & `alibabacloud_dingtalk-2.0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 02/04/2024
+Created on 09/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

