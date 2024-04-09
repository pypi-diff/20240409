# Comparing `tmp/platform-plugin-aspects-0.5.0.tar.gz` & `tmp/platform-plugin-aspects-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-plugin-aspects-0.5.0.tar", last modified: Mon Apr  1 16:46:20 2024, max compression
+gzip compressed data, was "platform-plugin-aspects-0.6.0.tar", last modified: Tue Apr  9 16:29:01 2024, max compression
```

## Comparing `platform-plugin-aspects-0.5.0.tar` & `platform-plugin-aspects-0.6.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.766943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.766943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.120888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.116888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.116888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 16:29:01.000000 platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 16:29:01.124888 platform-plugin-aspects-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-09 16:28:58.000000 platform-plugin-aspects-0.6.0/setup.py
```

### Comparing `platform-plugin-aspects-0.5.0/CHANGELOG.rst` & `platform-plugin-aspects-0.6.0/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,30 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.6.0 - 2024-04-08
+******************
+
+Added
+=====
+
+* Allow to embed translated Superset Dashboards.
+
 0.5.0 - 2024-04-01
 ******************
 
 Added
 =====
 
 * Load testing and test monitoring scripts.
 
-
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
@@ -39,21 +46,23 @@
 Added
 =====
 
 * Fixed development server configuration.
 
 0.3.0 – 2024-03-10
 ******************
+
 Added
 =====
 
 * Imported XBlock code from platform-plugin-superset
 
 0.2.0 – 2024-03-05
 ******************
+
 Added
 =====
 
 * Imported code from event-sink-clickhouse.
 
 0.1.0 – 2024-02-29
 **********************************************
```

### Comparing `platform-plugin-aspects-0.5.0/LICENSE` & `platform-plugin-aspects-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/PKG-INFO` & `platform-plugin-aspects-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.5.0
+Version: 0.6.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: celery
-Requires-Dist: django-rest-framework
 Requires-Dist: django_crum
+Requires-Dist: djangorestframework
 Requires-Dist: edx-django-utils
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles
 Requires-Dist: openedx-atlas
 Requires-Dist: openedx-filters
 Requires-Dist: redis
 Requires-Dist: requests
@@ -146,23 +146,30 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.6.0 - 2024-04-08
+******************
+
+Added
+=====
+
+* Allow to embed translated Superset Dashboards.
+
 0.5.0 - 2024-04-01
 ******************
 
 Added
 =====
 
 * Load testing and test monitoring scripts.
 
-
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
@@ -173,21 +180,23 @@
 Added
 =====
 
 * Fixed development server configuration.
 
 0.3.0 – 2024-03-10
 ******************
+
 Added
 =====
 
 * Imported XBlock code from platform-plugin-superset
 
 0.2.0 – 2024-03-05
 ******************
+
 Added
 =====
 
 * Imported code from event-sink-clickhouse.
 
 0.1.0 – 2024-02-29
 **********************************************
```

### Comparing `platform-plugin-aspects-0.5.0/README.rst` & `platform-plugin-aspects-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/apps.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/filters.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/extensions/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pkg_resources
 from crum import get_current_user
 from django.conf import settings
 from django.template import Context, Template
 from openedx_filters import PipelineStep
 from web_fragments.fragment import Fragment
 
-from platform_plugin_aspects.utils import generate_superset_context
+from platform_plugin_aspects.utils import _, generate_superset_context, get_model
 
 TEMPLATE_ABSOLUTE_PATH = "/instructor_dashboard/"
 BLOCK_CATEGORY = "aspects"
 
 ASPECTS_SECURITY_FILTERS_FORMAT = [
     "org = '{course.org}'",
     "course_name = '{course.display_name}'",
@@ -38,30 +38,38 @@
         dashboards = settings.ASPECTS_INSTRUCTOR_DASHBOARDS
         extra_filters_format = settings.SUPERSET_EXTRA_FILTERS_FORMAT
 
         filters = ASPECTS_SECURITY_FILTERS_FORMAT + extra_filters_format
 
         user = get_current_user()
 
+        user_language = (
+            get_model("user_preference").get_value(user, "pref-lang") or "en_US"
+        )
+        formatted_language = user_language.replace("-", "_")
+        if formatted_language not in settings.SUPERSET_DASHBOARD_LOCALES:
+            formatted_language = "en_US"
+
         context = generate_superset_context(
             context,
             user,
             dashboards=dashboards,
             filters=filters,
+            language=formatted_language,
         )
 
         template = Template(self.resource_string("static/html/superset.html"))
         html = template.render(Context(context))
         frag = Fragment(html)
         frag.add_css(self.resource_string("static/css/superset.css"))
         frag.add_javascript(self.resource_string("static/js/embed_dashboard.js"))
         section_data = {
             "fragment": frag,
             "section_key": BLOCK_CATEGORY,
-            "section_display_name": BLOCK_CATEGORY.title(),
+            "section_display_name": _("Analytics"),
             "course_id": str(course.id),
             "superset_url": str(context.get("superset_url")),
             "template_path_prefix": TEMPLATE_ABSOLUTE_PATH,
         }
         context["sections"].append(section_data)
         return {
             "context": context,
```

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/common.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,21 @@
         "internal_service_url": "http://superset:8088",
         "username": "superset",
         "password": "superset",
     }
     settings.ASPECTS_INSTRUCTOR_DASHBOARDS = [
         {
             "name": "Instructor Dashboard",
+            "slug": "instructor-dashboard",
             "uuid": "1d6bf904-f53f-47fd-b1c9-6cd7e284d286",
+            "allow_translations": True,
         },
     ]
     settings.SUPERSET_EXTRA_FILTERS_FORMAT = []
+    settings.SUPERSET_DASHBOARD_LOCALES = ["en_US"]
     settings.EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG = {
         # URL to a running ClickHouse server's HTTP interface. ex: https://foo.openedx.org:8443/ or
         # http://foo.openedx.org:8123/ . Note that we only support the ClickHouse HTTP interface
         # to avoid pulling in more dependencies to the platform than necessary.
         "url": "http://clickhouse:8123",
         "username": "ch_cms",
         "password": "password",
@@ -60,8 +63,12 @@
             "module": "openedx.core.djangoapps.external_user_ids.models",
             "model": "ExternalId",
         },
         "custom_course_edx": {
             "module": "lms.djangoapps.ccx.models",
             "model": "CustomCourseForEdX",
         },
+        "user_preference": {
+            "module": "openedx.core.djangoapps.user_api.models",
+            "model": "UserPreference",
+        },
     }
```

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/production.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/settings/production.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     )
     settings.ASPECTS_INSTRUCTOR_DASHBOARDS = getattr(settings, "ENV_TOKENS", {}).get(
         "ASPECTS_INSTRUCTOR_DASHBOARDS", settings.ASPECTS_INSTRUCTOR_DASHBOARDS
     )
     settings.SUPERSET_EXTRA_FILTERS_FORMAT = getattr(settings, "ENV_TOKENS", {}).get(
         "SUPERSET_EXTRA_FILTERS_FORMAT", settings.SUPERSET_EXTRA_FILTERS_FORMAT
     )
+    settings.SUPERSET_DASHBOARD_LOCALES = getattr(settings, "ENV_TOKENS", {}).get(
+        "SUPERSET_DASHBOARD_LOCALES", settings.SUPERSET_DASHBOARD_LOCALES
+    )
     settings.EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG = settings.ENV_TOKENS.get(
         "EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG",
         settings.EVENT_SINK_CLICKHOUSE_BACKEND_CONFIG,
     )
     settings.EVENT_SINK_CLICKHOUSE_PII_MODELS = settings.ENV_TOKENS.get(
         "EVENT_SINK_CLICKHOUSE_PII_MODELS",
         settings.EVENT_SINK_CLICKHOUSE_PII_MODELS,
```

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/signals.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/base_sink.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/external_id_sink.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/serializers.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/superset.css` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset.html` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/superset.js` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/tasks.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/utils.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Utilities for the Aspects app.
 """
 
 from __future__ import annotations
 
 import logging
 import os
+import uuid
 from importlib import import_module
 
 from django.conf import settings
 from supersetapiclient.client import SupersetClient
 from xblock.reference.user_service import XBlockUser
 
 logger = logging.getLogger(__name__)
@@ -26,28 +27,37 @@
 
 
 def generate_superset_context(  # pylint: disable=dangerous-default-value
     context,
     user,
     dashboards,
     filters=[],
+    language=None,
 ):
     """
     Update context with superset token and dashboard id.
 
     Args:
         context (dict): the context for the instructor dashboard. It must include a course object
         user (XBlockUser or User): the current user.
         superset_config (dict): superset config.
         dashboards (list): list of superset dashboard uuid.
         filters (list): list of filters to apply to the dashboard.
+        language (str): the language code of the end user.
     """
     course = context["course"]
     superset_config = settings.SUPERSET_CONFIG
 
+    if language:
+        for dashboard in dashboards:
+            if not dashboard["allow_translations"]:
+                continue
+            dashboard["slug"] = f"{dashboard['slug']}-{language}"
+            dashboard["uuid"] = str(get_uuid5(dashboard["uuid"], language))
+
     superset_token, dashboards = _generate_guest_token(
         user=user,
         course=course,
         superset_config=superset_config,
         dashboards=dashboards,
         filters=filters,
     )
@@ -216,7 +226,16 @@
 def get_ccx_courses(course_id):
     """
     Get the CCX courses for a given course.
     """
     if settings.FEATURES.get("CUSTOM_COURSES_EDX"):
         return get_model("custom_course_edx").objects.filter(course_id=course_id)
     return []
+
+
+def get_uuid5(base_uuid, language):
+    """
+    Generate an idempotent uuid.
+    """
+    base_uuid = uuid.UUID(base_uuid)
+    base_namespace = uuid.uuid5(base_uuid, "superset")
+    return uuid.uuid5(base_namespace, language)
```

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects/xblock.py` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/PKG-INFO` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.5.0
+Version: 0.6.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django
 Requires-Dist: XBlock
 Requires-Dist: celery
-Requires-Dist: django-rest-framework
 Requires-Dist: django_crum
+Requires-Dist: djangorestframework
 Requires-Dist: edx-django-utils
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles
 Requires-Dist: openedx-atlas
 Requires-Dist: openedx-filters
 Requires-Dist: redis
 Requires-Dist: requests
@@ -146,23 +146,30 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.6.0 - 2024-04-08
+******************
+
+Added
+=====
+
+* Allow to embed translated Superset Dashboards.
+
 0.5.0 - 2024-04-01
 ******************
 
 Added
 =====
 
 * Load testing and test monitoring scripts.
 
-
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
@@ -173,21 +180,23 @@
 Added
 =====
 
 * Fixed development server configuration.
 
 0.3.0 – 2024-03-10
 ******************
+
 Added
 =====
 
 * Imported XBlock code from platform-plugin-superset
 
 0.2.0 – 2024-03-05
 ******************
+
 Added
 =====
 
 * Imported code from event-sink-clickhouse.
 
 0.1.0 – 2024-02-29
 **********************************************
```

### Comparing `platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform-plugin-aspects-0.6.0/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/requirements/constraints.txt` & `platform-plugin-aspects-0.6.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.5.0/setup.py` & `platform-plugin-aspects-0.6.0/setup.py`

 * *Files identical despite different names*

