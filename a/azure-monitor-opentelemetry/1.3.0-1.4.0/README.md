# Comparing `tmp/azure-monitor-opentelemetry-1.3.0.tar.gz` & `tmp/azure-monitor-opentelemetry-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-monitor-opentelemetry-1.3.0.tar", last modified: Fri Mar  1 19:34:26 2024, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.4.0.tar", last modified: Mon Apr  8 22:28:42 2024, max compression
```

## Comparing `azure-monitor-opentelemetry-1.3.0.tar` & `azure-monitor-opentelemetry-1.4.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.322264 azure-monitor-opentelemetry-1.3.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10281 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/NOTICE.txt
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20303 2024-03-01 19:34:26.322264 azure-monitor-opentelemetry-1.3.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18734 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.306264 azure-monitor-opentelemetry-1.3.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.306264 azure-monitor-opentelemetry-1.3.0/azure/monitor/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.310264 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.310264 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1469 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2917 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7953 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_configure.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3457 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_constants.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.310264 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3554 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2161 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_types.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.310264 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_util/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      306 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_util/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5761 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_util/configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_version.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.322264 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20303 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3089 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-01 19:34:26.000000 azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.314264 azure-monitor-opentelemetry-1.3.0/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5357 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.314264 azure-monitor-opentelemetry-1.3.0/samples/logging/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/logging/basic.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/logging/correlated_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/logging/custom_properties.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/logging/exception_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/logging/logs_with_traces.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.314264 azure-monitor-opentelemetry-1.3.0/samples/metrics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/metrics/attributes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/metrics/instruments.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/samples/tracing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/azure_core.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/db_psycopg2.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.306264 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/admin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/apps.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/migrations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/migrations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/tests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/views.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/manage.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/asgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/settings.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/wsgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/filter_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1070 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/http_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/http_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/http_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/http_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/http_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/instrumentation_options.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/manually_instrumented.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/modify_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/sampling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/samples/tracing/simple.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-01 19:34:26.322264 azure-monitor-opentelemetry-1.3.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/tests/autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/autoinstrumentation/test_configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3782 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/autoinstrumentation/test_distro.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/tests/configuration/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16159 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/configuration/test_configure.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9729 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/configuration/test_util.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/tests/diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/diagnostics/test_diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/diagnostics/test_status_logger.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.318264 azure-monitor-opentelemetry-1.3.0/tests/exporter/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/exporter/test_exporter.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-01 19:34:26.322264 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_django.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_psycopg2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4985 2024-03-01 19:33:35.000000 azure-monitor-opentelemetry-1.3.0/tests/test_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10782 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/NOTICE.txt
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20741 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3018 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8753 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_configure.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3582 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_types.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.290276 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    20741 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-08 22:28:42.000000 azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/logging/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/basic.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/correlated_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/custom_properties.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/exception_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/logging/logs_with_traces.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.294276 azure-monitor-opentelemetry-1.4.0/samples/metrics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/metrics/attributes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/metrics/instruments.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/azure_core.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/db_psycopg2.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.286276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/admin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/apps.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/migrations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/migrations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/tests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/views.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/manage.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/asgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/settings.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/wsgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/filter_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/instrumentation_options.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/manually_instrumented.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/modify_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/sampling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/samples/tracing/simple.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.298276 azure-monitor-opentelemetry-1.4.0/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3782 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5030 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_status_logger.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/exporter/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/exporter/test_exporter.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_django.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_psycopg2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/test_configure.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 22:28:42.302276 azure-monitor-opentelemetry-1.4.0/tests/utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/utils/test_configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-04-08 22:27:21.000000 azure-monitor-opentelemetry-1.4.0/tests/utils/test_utils.py
```

### Comparing `azure-monitor-opentelemetry-1.3.0/CHANGELOG.md` & `azure-monitor-opentelemetry-1.4.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Release History
 
+## 1.4.0 (2024-04-09)
+
+### Features Added
+
+- Adding diagnostic warning when distro detects RP attach
+    ([#34971](https://github.com/Azure/azure-sdk-for-python/pull/34971))
+- Added `resource` parameter
+    ([#34900](https://github.com/Azure/azure-sdk-for-python/pull/34900))
+
+### Other Changes
+
+- Updated FastAPI sample
+    ([#34738](https://github.com/Azure/azure-sdk-for-python/pull/34738))
+- Refactored constants and utils
+    ([#35066](https://github.com/Azure/azure-sdk-for-python/pull/35066))
+
 ## 1.3.0 (2024-02-29)
 
 ### Features Added
 
 - Add custom span processors configuration option
     ([#34326](https://github.com/Azure/azure-sdk-for-python/pull/34326))
```

### Comparing `azure-monitor-opentelemetry-1.3.0/LICENSE` & `azure-monitor-opentelemetry-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/NOTICE.txt` & `azure-monitor-opentelemetry-1.4.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/PKG-INFO` & `azure-monitor-opentelemetry-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.3.0
+Version: 1.4.0
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,23 +18,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 Requires-Dist: azure-core<2.0.0,>=1.28.0
 Requires-Dist: azure-core-tracing-opentelemetry~=1.0.0b11
-Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b23
+Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b24
 Requires-Dist: opentelemetry-instrumentation-django~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-fastapi~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-flask~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-psycopg2~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-requests~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-urllib~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-urllib3~=0.42b0
-Requires-Dist: opentelemetry-resource-detector-azure~=0.1.2
+Requires-Dist: opentelemetry-resource-detector-azure~=0.1.4
 
 # Azure Monitor Opentelemetry Distro client library for Python
 
 The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] is a "one-stop-shop" telemetry solution, requiring only one line of code to instrument your application. The distro captures telemetry via [OpenTelemetry instrumentations][azure_monitor_opentelemetry_exporters] and reports telemetry to Azure Monitor via the [Azure Monitor exporters][azure_monitor_opentelemetry_exporters].
 
 Prior to using this SDK, please read and understand [Data Collection Basics](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python), especially the section on [telemetry types](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python#telemetry-types). OpenTelemetry terminology differs from Application Insights terminology so it is important to understand the way the telemetry types map to each other.
 
@@ -92,17 +92,19 @@
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
+| `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
-You can configure further with [OpenTelemetry environment variables][ot_env_vars] such as:
+You can configure further with [OpenTelemetry environment variables][ot_env_vars].
+
 | Environment Variable | Description |
 |-------------|----------------------|
 | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes] | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. |
 | `OTEL_LOGS_EXPORTER` | If set to `None`, disables collection and export of logging telemetry. |
 | `OTEL_METRICS_EXPORTER` | If set to `None`, disables collection and export of metric telemetry. |
 | `OTEL_TRACES_EXPORTER` | If set to `None`, disables collection and export of distributed tracing telemetry. |
 | `OTEL_BLRP_SCHEDULE_DELAY` | Specifies the logging export interval in milliseconds. Defaults to 5000. |
```

### Comparing `azure-monitor-opentelemetry-1.3.0/README.md` & `azure-monitor-opentelemetry-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,19 @@
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
+| `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
-You can configure further with [OpenTelemetry environment variables][ot_env_vars] such as:
+You can configure further with [OpenTelemetry environment variables][ot_env_vars].
+
 | Environment Variable | Description |
 |-------------|----------------------|
 | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes] | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. |
 | `OTEL_LOGS_EXPORTER` | If set to `None`, disables collection and export of logging telemetry. |
 | `OTEL_METRICS_EXPORTER` | If set to `None`, disables collection and export of metric telemetry. |
 | `OTEL_TRACES_EXPORTER` | If set to `None`, disables collection and export of distributed tracing telemetry. |
 | `OTEL_BLRP_SCHEDULE_DELAY` | Specifies the logging export interval in milliseconds. Defaults to 5000. |
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 # --------------------------------------------------------------------------
 
 
 from warnings import warn
 
 from opentelemetry.sdk._configuration import _OTelSDKConfigurator
 
-from azure.monitor.opentelemetry._constants import (
-    _is_attach_enabled,
-    _PREVIEW_ENTRY_POINT_WARNING,
-)
+from azure.monitor.opentelemetry.exporter._utils import _is_attach_enabled # pylint: disable=import-error,no-name-in-module
+from azure.monitor.opentelemetry._constants import _PREVIEW_ENTRY_POINT_WARNING
 from azure.monitor.opentelemetry._diagnostics.diagnostic_logging import (
     AzureDiagnosticLogging,
     _ATTACH_FAILURE_CONFIGURATOR,
     _ATTACH_SUCCESS_CONFIGURATOR,
 )
 from azure.monitor.opentelemetry._diagnostics.status_logger import (
     AzureStatusLogger,
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 from opentelemetry.sdk.environment_variables import (
     _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
     OTEL_EXPERIMENTAL_RESOURCE_DETECTORS,
 )
 
 from azure.core.settings import settings
 from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
+from azure.monitor.opentelemetry.exporter._utils import _is_attach_enabled # pylint: disable=import-error,no-name-in-module
 from azure.monitor.opentelemetry._constants import (
-    _is_attach_enabled,
     _AZURE_APP_SERVICE_RESOURCE_DETECTOR_NAME,
     _AZURE_SDK_INSTRUMENTATION_NAME,
     _PREVIEW_ENTRY_POINT_WARNING,
 )
 from azure.monitor.opentelemetry._diagnostics.diagnostic_logging import (
     AzureDiagnosticLogging,
     _ATTACH_FAILURE_DISTRO,
     _ATTACH_SUCCESS_DISTRO,
 )
 from azure.monitor.opentelemetry._diagnostics.status_logger import (
     AzureStatusLogger,
 )
-from azure.monitor.opentelemetry._util.configurations import (
+from azure.monitor.opentelemetry._utils.configurations import (
     _get_otel_disabled_instrumentations,
 )
 
 
 class AzureMonitorDistro(BaseDistro):
     def _configure(self, **kwargs) -> None:
         if not _is_attach_enabled():
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_configure.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,20 @@
 from azure.monitor.opentelemetry._types import ConfigurationValue
 from azure.monitor.opentelemetry.exporter import (  # pylint: disable=import-error,no-name-in-module
     ApplicationInsightsSampler,
     AzureMonitorLogExporter,
     AzureMonitorMetricExporter,
     AzureMonitorTraceExporter,
 )
-from azure.monitor.opentelemetry._util.configurations import (
+from azure.monitor.opentelemetry.exporter._utils import _is_attach_enabled # pylint: disable=import-error,no-name-in-module
+from azure.monitor.opentelemetry._diagnostics.diagnostic_logging import (
+    _DISTRO_DETECTS_ATTACH,
+    AzureDiagnosticLogging,
+)
+from azure.monitor.opentelemetry._utils.configurations import (
     _get_configurations,
     _is_instrumentation_enabled,
 )
 
 _logger = getLogger(__name__)
 
 
@@ -65,21 +70,25 @@
      telemetry records for retry. Defaults to `False`.
     :keyword str logger_name: The name of the Python logger that telemetry will be collected.
     :keyword dict instrumentation_options: A nested dictionary that determines which instrumentations
      to enable or disable.  Instrumentations are referred to by their Library Names. For example,
      `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}`
      will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default
      instrumentations enabled.
+    :keyword ~opentelemetry.sdk.resources.Resource resource: OpenTelemetry Resource object. Passed in Resource
+     Attributes take priority over default attributes and those from Resource Detectors.
     :keyword list[~opentelemetry.sdk.trace.SpanProcessor] span_processors: List of `SpanProcessor` objects
      to process every span prior to exporting. Will be run sequentially.
     :keyword str storage_directory: Storage directory in which to store retry files. Defaults to
      `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
     :rtype: None
     """
 
+    _send_attach_warning()
+
     configurations = _get_configurations(**kwargs)
 
     disable_tracing = configurations[DISABLE_TRACING_ARG]
     disable_logging = configurations[DISABLE_LOGGING_ARG]
     disable_metrics = configurations[DISABLE_METRICS_ARG]
 
     # Setup tracing pipeline
@@ -173,7 +182,15 @@
             instrumentor().instrument(skip_dep_check=True)
         except Exception as ex:  # pylint: disable=broad-except
             _logger.warning(
                 "Exception occurred when instrumenting: %s.",
                 lib_name,
                 exc_info=ex,
             )
+
+
+def _send_attach_warning():
+    if _is_attach_enabled():
+        AzureDiagnosticLogging.warning(
+            "Distro detected that automatic attach may have occurred. Check your data to ensure "
+            "that telemetry is not being duplicated. This may impact your cost.",
+            _DISTRO_DETECTS_ATTACH)
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 
 import logging
 import threading
 from os import makedirs
 from os.path import exists, join
 
-from azure.monitor.opentelemetry._constants import (
+from azure.monitor.opentelemetry._utils import (
     _EXTENSION_VERSION,
     _IS_DIAGNOSTICS_ENABLED,
     _env_var_or_default,
     _get_customer_ikey_from_env_var,
     _get_log_path,
 )
 from azure.monitor.opentelemetry._version import VERSION
@@ -24,14 +24,15 @@
 _SUBSCRIPTION_ID = (
     _SUBSCRIPTION_ID_ENV_VAR.split("+")[0] if _SUBSCRIPTION_ID_ENV_VAR else None
 )
 _logger = logging.getLogger(__name__)
 _logger.propagate = False
 _logger.setLevel(logging.INFO)
 _DIAGNOSTIC_LOG_PATH = _get_log_path()
+_DISTRO_DETECTS_ATTACH = "4100"
 _ATTACH_SUCCESS_DISTRO = "4200"
 _ATTACH_SUCCESS_CONFIGURATOR = "4201"
 _ATTACH_FAILURE_DISTRO = "4400"
 _ATTACH_FAILURE_CONFIGURATOR = "4401"
 
 
 class AzureDiagnosticLogging:
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 
 from json import dumps
 from os import getpid, makedirs
 from os.path import exists, join
 from platform import node
 
-from azure.monitor.opentelemetry._constants import (
+from azure.monitor.opentelemetry._utils import (
     _EXTENSION_VERSION,
     _IS_DIAGNOSTICS_ENABLED,
     _get_customer_ikey_from_env_var,
     _get_log_path,
 )
 from azure.monitor.opentelemetry._version import VERSION
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_types.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/azure/monitor/opentelemetry/_util/configurations.py` & `azure-monitor-opentelemetry-1.4.0/azure/monitor/opentelemetry/_utils/configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,18 @@
 
 
 def _default_resource(configurations):
     environ.setdefault(
         OTEL_EXPERIMENTAL_RESOURCE_DETECTORS,
         ",".join(_SUPPORTED_RESOURCE_DETECTORS)
     )
-    configurations[RESOURCE_ARG] = Resource.create()
+    if RESOURCE_ARG not in configurations:
+        configurations[RESOURCE_ARG] = Resource.create()
+    else:
+        configurations[RESOURCE_ARG] = Resource.create(configurations[RESOURCE_ARG].attributes)
 
 
 # TODO: remove when sampler uses env var instead
 def _default_sampling_ratio(configurations):
     default = 1.0
     if SAMPLING_RATIO_ENV_VAR in environ:
         try:
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.3.0
+Version: 1.4.0
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,23 +18,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 Requires-Dist: azure-core<2.0.0,>=1.28.0
 Requires-Dist: azure-core-tracing-opentelemetry~=1.0.0b11
-Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b23
+Requires-Dist: azure-monitor-opentelemetry-exporter~=1.0.0b24
 Requires-Dist: opentelemetry-instrumentation-django~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-fastapi~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-flask~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-psycopg2~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-requests~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-urllib~=0.42b0
 Requires-Dist: opentelemetry-instrumentation-urllib3~=0.42b0
-Requires-Dist: opentelemetry-resource-detector-azure~=0.1.2
+Requires-Dist: opentelemetry-resource-detector-azure~=0.1.4
 
 # Azure Monitor Opentelemetry Distro client library for Python
 
 The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] is a "one-stop-shop" telemetry solution, requiring only one line of code to instrument your application. The distro captures telemetry via [OpenTelemetry instrumentations][azure_monitor_opentelemetry_exporters] and reports telemetry to Azure Monitor via the [Azure Monitor exporters][azure_monitor_opentelemetry_exporters].
 
 Prior to using this SDK, please read and understand [Data Collection Basics](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python), especially the section on [telemetry types](https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-overview?tabs=python#telemetry-types). OpenTelemetry terminology differs from Application Insights terminology so it is important to understand the way the telemetry types map to each other.
 
@@ -92,17 +92,19 @@
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
+| `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
-You can configure further with [OpenTelemetry environment variables][ot_env_vars] such as:
+You can configure further with [OpenTelemetry environment variables][ot_env_vars].
+
 | Environment Variable | Description |
 |-------------|----------------------|
 | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes] | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. |
 | `OTEL_LOGS_EXPORTER` | If set to `None`, disables collection and export of logging telemetry. |
 | `OTEL_METRICS_EXPORTER` | If set to `None`, disables collection and export of metric telemetry. |
 | `OTEL_TRACES_EXPORTER` | If set to `None`, disables collection and export of distributed tracing telemetry. |
 | `OTEL_BLRP_SCHEDULE_DELAY` | Specifies the logging export interval in milliseconds. Defaults to 5000. |
```

### Comparing `azure-monitor-opentelemetry-1.3.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-1.4.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 azure/monitor/opentelemetry/py.typed
 azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
 azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
 azure/monitor/opentelemetry/_autoinstrumentation/distro.py
 azure/monitor/opentelemetry/_diagnostics/__init__.py
 azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
 azure/monitor/opentelemetry/_diagnostics/status_logger.py
-azure/monitor/opentelemetry/_util/__init__.py
-azure/monitor/opentelemetry/_util/configurations.py
+azure/monitor/opentelemetry/_utils/__init__.py
+azure/monitor/opentelemetry/_utils/configurations.py
 azure_monitor_opentelemetry.egg-info/PKG-INFO
 azure_monitor_opentelemetry.egg-info/SOURCES.txt
 azure_monitor_opentelemetry.egg-info/dependency_links.txt
 azure_monitor_opentelemetry.egg-info/entry_points.txt
 azure_monitor_opentelemetry.egg-info/not-zip-safe
 azure_monitor_opentelemetry.egg-info/requires.txt
 azure_monitor_opentelemetry.egg-info/top_level.txt
@@ -60,22 +60,22 @@
 samples/tracing/django/sample/example/migrations/__init__.py
 samples/tracing/django/sample/sample/__init__.py
 samples/tracing/django/sample/sample/asgi.py
 samples/tracing/django/sample/sample/settings.py
 samples/tracing/django/sample/sample/urls.py
 samples/tracing/django/sample/sample/wsgi.py
 tests/conftest.py
-tests/test_constants.py
+tests/test_configure.py
 tests/autoinstrumentation/test_configurator.py
 tests/autoinstrumentation/test_distro.py
-tests/configuration/test_configure.py
-tests/configuration/test_util.py
 tests/diagnostics/test_diagnostic_logging.py
 tests/diagnostics/test_status_logger.py
 tests/exporter/test_exporter.py
 tests/instrumentation/test_django.py
 tests/instrumentation/test_fastapi.py
 tests/instrumentation/test_flask.py
 tests/instrumentation/test_psycopg2.py
 tests/instrumentation/test_requests.py
 tests/instrumentation/test_urllib.py
-tests/instrumentation/test_urllib3.py
+tests/instrumentation/test_urllib3.py
+tests/utils/test_configurations.py
+tests/utils/test_utils.py
```

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/README.md` & `azure-monitor-opentelemetry-1.4.0/samples/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     - python
 products:
     - azure
     - azure-template
 urlFragment: azure-template-samples
 ---
 
-# Azure Template samples
+# Azure Monitor OpenTelemetry distro samples
 
 Provide an overview of all the samples and explain how to run them.
 
 For guidance on the samples README, visit the [sample guide](https://github.com/Azure/azure-sdk-for-python/blob/main/doc/dev/sample_guide.md#package-sample-readme).
 
 
 |**File Name**|**Description**|
```

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/logging/basic.py` & `azure-monitor-opentelemetry-1.4.0/samples/logging/basic.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/logging/correlated_logs.py` & `azure-monitor-opentelemetry-1.4.0/samples/logging/correlated_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/logging/custom_properties.py` & `azure-monitor-opentelemetry-1.4.0/samples/logging/custom_properties.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/logging/exception_logs.py` & `azure-monitor-opentelemetry-1.4.0/samples/logging/exception_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/logging/logs_with_traces.py` & `azure-monitor-opentelemetry-1.4.0/samples/logging/logs_with_traces.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/metrics/attributes.py` & `azure-monitor-opentelemetry-1.4.0/samples/metrics/attributes.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/metrics/instruments.py` & `azure-monitor-opentelemetry-1.4.0/samples/metrics/instruments.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/azure_core.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/azure_core.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/db_psycopg2.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/db_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/example/views.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/example/views.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/manage.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/manage.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/asgi.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/asgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/settings.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/settings.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/urls.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/urls.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/django/sample/sample/wsgi.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/django/sample/sample/wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/filter_spans.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/filter_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/http_fastapi.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_flask.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License in the project root for
 # license information.
 # --------------------------------------------------------------------------
-import fastapi
 from azure.monitor.opentelemetry import configure_azure_monitor
 
 # Configure Azure monitor collection telemetry pipeline
 configure_azure_monitor()
 
-app = fastapi.FastAPI()
+# Import Flask after running configure_azure_monitor()
+import flask
 
+app = flask.Flask(__name__)
 
-# Requests made to fastapi endpoints will be automatically captured
-@app.get("/")
-async def test():
-    return {"message": "Hello World"}
+
+# Requests sent to the flask application will be automatically captured
+@app.route("/")
+def test():
+    return "Test flask request"
 
 
 # Exceptions that are raised within the request are automatically captured
-@app.get("/exception")
-async def exception():
+@app.route("/exception")
+def exception():
     raise Exception("Hit an exception")
 
 
-# Set the OTEL_PYTHON_EXCLUDE_URLS environment variable to "http://127.0.0.1:8000/exclude"
-# Telemetry from this endpoint will not be captured due to excluded_urls config above
-@app.get("/exclude")
-async def exclude():
-    return {"message": "Telemetry was not captured"}
+# Requests sent to this endpoint will not be tracked due to
+# flask_config configuration
+@app.route("/ignore")
+def ignore():
+    return "Request received but not tracked."
+
+
+if __name__ == "__main__":
+    app.run(host="localhost", port=8080)
```

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/http_requests.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/http_urllib.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/http_urllib3.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/instrumentation_options.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/instrumentation_options.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/manually_instrumented.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/manually_instrumented.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/modify_spans.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/modify_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/sampling.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/sampling.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/samples/tracing/simple.py` & `azure-monitor-opentelemetry-1.4.0/samples/tracing/simple.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/setup.py` & `azure-monitor-opentelemetry-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,23 @@
     package_data={
         "pytyped": ["py.typed"],
     },
     python_requires=">=3.8",
     install_requires=[
         "azure-core<2.0.0,>=1.28.0",
         "azure-core-tracing-opentelemetry~=1.0.0b11",
-        "azure-monitor-opentelemetry-exporter~=1.0.0b23",
+        "azure-monitor-opentelemetry-exporter~=1.0.0b24",
         "opentelemetry-instrumentation-django~=0.42b0",
         "opentelemetry-instrumentation-fastapi~=0.42b0",
         "opentelemetry-instrumentation-flask~=0.42b0",
         "opentelemetry-instrumentation-psycopg2~=0.42b0",
         "opentelemetry-instrumentation-requests~=0.42b0",
         "opentelemetry-instrumentation-urllib~=0.42b0",
         "opentelemetry-instrumentation-urllib3~=0.42b0",
-        "opentelemetry-resource-detector-azure~=0.1.2",
+        "opentelemetry-resource-detector-azure~=0.1.4",
     ],
     entry_points={
         "opentelemetry_distro": [
             "azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry._autoinstrumentation.distro:AzureMonitorDistro"
         ],
         "opentelemetry_configurator": [
             "azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry._autoinstrumentation.configurator:AzureMonitorConfigurator"
```

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/autoinstrumentation/test_configurator.py` & `azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/autoinstrumentation/test_distro.py` & `azure-monitor-opentelemetry-1.4.0/tests/autoinstrumentation/test_distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/configuration/test_configure.py` & `azure-monitor-opentelemetry-1.4.0/tests/test_configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,32 @@
 import unittest
 from unittest.mock import Mock, call, patch
 
 from opentelemetry.sdk.resources import Resource
 
 from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
 from azure.monitor.opentelemetry._configure import (
+    _send_attach_warning,
     _setup_instrumentations,
     _setup_logging,
     _setup_metrics,
     _setup_tracing,
     configure_azure_monitor,
 )
+from azure.monitor.opentelemetry._diagnostics.diagnostic_logging import _DISTRO_DETECTS_ATTACH
 
 
 TEST_RESOURCE = Resource({"foo": "bar"})
 
 
 class TestConfigure(unittest.TestCase):
     @patch(
+        "azure.monitor.opentelemetry._configure._send_attach_warning",
+    )
+    @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_logging",
@@ -44,23 +49,25 @@
     )
     def test_configure_azure_monitor(
         self,
         tracing_mock,
         logging_mock,
         metrics_mock,
         instrumentation_mock,
+        detect_attach_mock,
     ):
         kwargs = {
             "connection_string": "test_cs",
         }
         configure_azure_monitor(**kwargs)
         tracing_mock.assert_called_once()
         logging_mock.assert_called_once()
         metrics_mock.assert_called_once()
         instrumentation_mock.assert_called_once()
+        detect_attach_mock.assert_called_once()
 
     @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
@@ -92,15 +99,16 @@
                 },
                 "django": {
                     "enabled": False
                 },
                 "requests": {
                     "enabled": False
                 },
-            }
+            },
+            "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_not_called()
         logging_mock.assert_called_once_with(configurations)
         metrics_mock.assert_called_once_with(configurations)
         instrumentation_mock.assert_called_once_with(configurations)
@@ -129,14 +137,15 @@
         instrumentation_mock,
     ):
         configurations = {
             "connection_string": "test_cs",
             "disable_tracing": False,
             "disable_logging": True,
             "disable_metrics": False,
+            "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_called_once_with(configurations)
         logging_mock.assert_not_called()
         metrics_mock.assert_called_once_with(configurations)
         instrumentation_mock.assert_called_once_with(configurations)
@@ -165,14 +174,15 @@
         instrumentation_mock,
     ):
         configurations = {
             "connection_string": "test_cs",
             "disable_tracing": False,
             "disable_logging": False,
             "disable_metrics": True,
+            "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_called_once_with(configurations)
         logging_mock.assert_called_once_with(configurations)
         metrics_mock.assert_not_called()
         instrumentation_mock.assert_called_once_with(configurations)
@@ -460,7 +470,32 @@
         enabled_mock.side_effect = [False, True]
         _setup_instrumentations({})
         dep_mock.assert_called_with(ep2_mock.dist)
         ep_mock.load.assert_not_called()
         ep2_mock.load.assert_called_once()
         instrumentor_mock.instrument.assert_called_once()
         logger_mock.debug.assert_called_once()
+
+    @patch("azure.monitor.opentelemetry._configure.AzureDiagnosticLogging")
+    @patch("azure.monitor.opentelemetry._configure._is_attach_enabled")
+    def test_send_attach_warning_true(
+        self,
+        is_attach_enabled_mock,
+        mock_diagnostics,
+    ):
+        is_attach_enabled_mock.return_value = True
+        _send_attach_warning()
+        mock_diagnostics.warning.assert_called_once_with(
+            "Distro detected that automatic attach may have occurred. Check your data to ensure that telemetry is not being duplicated. This may impact your cost.",
+            _DISTRO_DETECTS_ATTACH,
+        )
+
+    @patch("azure.monitor.opentelemetry._configure.AzureDiagnosticLogging")
+    @patch("azure.monitor.opentelemetry._configure._is_attach_enabled")
+    def test_send_attach_warning_false(
+        self,
+        is_attach_enabled_mock,
+        mock_diagnostics,
+    ):
+        is_attach_enabled_mock.return_value = False
+        _send_attach_warning()
+        mock_diagnostics.warning.assert_not_called()
```

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/configuration/test_util.py` & `azure-monitor-opentelemetry-1.4.0/tests/utils/test_configurations.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from os import environ
 from unittest import TestCase
 from unittest.mock import patch
 
 from opentelemetry.instrumentation.environment_variables import (
     OTEL_PYTHON_DISABLED_INSTRUMENTATIONS,
 )
-from azure.monitor.opentelemetry._util.configurations import (
+from azure.monitor.opentelemetry._utils.configurations import (
     SAMPLING_RATIO_ENV_VAR,
     _get_configurations,
 )
 from opentelemetry.environment_variables import (
     OTEL_LOGS_EXPORTER,
     OTEL_METRICS_EXPORTER,
     OTEL_TRACES_EXPORTER,
@@ -32,33 +32,43 @@
 from opentelemetry.sdk.resources import Resource, Attributes
 
 
 TEST_DEFAULT_RESOURCE = Resource({
     "test.attributes.1": "test_value_1",
     "test.attributes.2": "test_value_2"
 })
+TEST_CUSTOM_RESOURCE = Resource({
+    "test.attributes.2": "test_value_4",
+    "test.attributes.3": "test_value_3"
+})
+TEST_MERGED_RESOURCE = Resource({
+    "test.attributes.1": "test_value_1",
+    "test.attributes.2": "test_value_4",
+    "test.attributes.3": "test_value_3"
+})
 
 
-class TestUtil(TestCase):
+class TestConfigurations(TestCase):
     @patch.dict("os.environ", {}, clear=True)
-    @patch("azure.monitor.opentelemetry._util.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
-    @patch("opentelemetry.sdk.resources.Resource.create", return_value=TEST_DEFAULT_RESOURCE)
+    @patch("azure.monitor.opentelemetry._utils.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
+    @patch("opentelemetry.sdk.resources.Resource.create", return_value=TEST_MERGED_RESOURCE)
     def test_get_configurations(self, resource_create_mock):
         configurations = _get_configurations(
             connection_string="test_cs",
             credential="test_credential",
+            resource=TEST_CUSTOM_RESOURCE
         )
 
         self.assertEqual(configurations["connection_string"], "test_cs")
         self.assertEqual(configurations["disable_logging"], False)
         self.assertEqual(configurations["disable_metrics"], False)
         self.assertEqual(configurations["disable_tracing"], False)
-        self.assertEqual(configurations["resource"].attributes, TEST_DEFAULT_RESOURCE.attributes)
+        self.assertEqual(configurations["resource"].attributes, TEST_MERGED_RESOURCE.attributes)
         self.assertEqual(environ[OTEL_EXPERIMENTAL_RESOURCE_DETECTORS], "azure_app_service,azure_vm")
-        resource_create_mock.assert_called_once_with()
+        resource_create_mock.assert_called_once_with(TEST_CUSTOM_RESOURCE.attributes)
         self.assertEqual(configurations["sampling_ratio"], 1.0)
         self.assertEqual(configurations["credential"], ("test_credential"))
         self.assertEqual(configurations["instrumentation_options"], {
             "azure_sdk" : {"enabled": True},
             "django": {"enabled": True},
             "fastapi": {"enabled": True},
             "flask": {"enabled": True},
@@ -156,15 +166,15 @@
         "os.environ",
         {
             OTEL_PYTHON_DISABLED_INSTRUMENTATIONS: "django , urllib3,previewlib1,azure_sdk",
         },
         clear=True,
     )
     @patch("opentelemetry.sdk.resources.Resource.create", return_value=TEST_DEFAULT_RESOURCE)
-    @patch("azure.monitor.opentelemetry._util.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
+    @patch("azure.monitor.opentelemetry._utils.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
     def test_merge_instrumentation_options_conflict(self, resource_create_mock):
         configurations = _get_configurations(
             instrumentation_options = {
                 "azure_sdk" : {"enabled": True},
                 "django" : {"enabled": True},
                 "fastapi" : {"enabled": True},
                 "flask" : {"enabled": False},
@@ -182,15 +192,15 @@
             "previewlib2": {"enabled": False},
             "requests": {"enabled": True},
             "urllib": {"enabled": True},
             "urllib3": {"enabled": False},
         })
 
     @patch.dict("os.environ", {}, clear=True)
-    @patch("azure.monitor.opentelemetry._util.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
+    @patch("azure.monitor.opentelemetry._utils.configurations._PREVIEW_INSTRUMENTED_LIBRARIES", ("previewlib1", "previewlib2"))
     @patch("opentelemetry.sdk.resources.Resource.create", return_value=TEST_DEFAULT_RESOURCE)
     def test_merge_instrumentation_options_extra_args(self, resource_create_mock):
         configurations = _get_configurations(
             instrumentation_options = {
                 "django" : {"enabled": True},
                 "fastapi" : {"enabled": True, "foo": "bar"},
                 "flask" : {"enabled": False, "foo": "bar"},
```

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/conftest.py` & `azure-monitor-opentelemetry-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/diagnostics/test_diagnostic_logging.py` & `azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/diagnostics/test_status_logger.py` & `azure-monitor-opentelemetry-1.4.0/tests/diagnostics/test_status_logger.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/exporter/test_exporter.py` & `azure-monitor-opentelemetry-1.4.0/tests/exporter/test_exporter.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_django.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_django.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_fastapi.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_flask.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_psycopg2.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_requests.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_urllib.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/instrumentation/test_urllib3.py` & `azure-monitor-opentelemetry-1.4.0/tests/instrumentation/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.3.0/tests/test_constants.py` & `azure-monitor-opentelemetry-1.4.0/tests/utils/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,145 +5,127 @@
 # --------------------------------------------------------------------------
 
 from importlib import reload
 from os import environ
 from unittest import TestCase
 from unittest.mock import patch
 
-from azure.monitor.opentelemetry import _constants
+from azure.monitor.opentelemetry import _utils
 
 TEST_VALUE = "TEST_VALUE"
 TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
 TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
 
 
 def clear_env_var(env_var):
     if env_var in environ:
         del environ[env_var]
 
 
-class TestConstants(TestCase):
+class TestUtils(TestCase):
     @patch.dict(
         "os.environ",
         {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
     )
     def test_extension_version(self):
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
+        reload(_utils)
+        self.assertEqual(_utils._EXTENSION_VERSION, TEST_VALUE)
 
     def test_extension_version_default(self):
         clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
+        reload(_utils)
+        self.assertEqual(_utils._EXTENSION_VERSION, "disabled")
 
     @patch.dict(
         "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
     )
     def test_ikey(self):
-        reload(_constants)
+        reload(_utils)
         self.assertEqual(
-            _constants._get_customer_ikey_from_env_var(), TEST_IKEY
+            _utils._get_customer_ikey_from_env_var(), TEST_IKEY
         )
 
     def test_ikey_defaults(self):
         clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
-        reload(_constants)
+        reload(_utils)
         self.assertEqual(
-            _constants._get_customer_ikey_from_env_var(), "unknown"
+            _utils._get_customer_ikey_from_env_var(), "unknown"
         )
 
     @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
     def test_diagnostics_enabled(self):
-        reload(_constants)
-        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
+        reload(_utils)
+        self.assertTrue(_utils._IS_DIAGNOSTICS_ENABLED)
 
     def test_diagnostics_disabled(self):
         clear_env_var("WEBSITE_SITE_NAME")
-        reload(_constants)
-        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
+        reload(_utils)
+        self.assertFalse(_utils._IS_DIAGNOSTICS_ENABLED)
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="Linux",
     )
     def test_log_path_linux(self, mock_system):
         self.assertEqual(
-            _constants._get_log_path(), "/var/log/applicationinsights"
+            _utils._get_log_path(), "/var/log/applicationinsights"
         )
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="Linux",
     )
     def test_status_log_path_linux(self, mock_system):
         self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
+            _utils._get_log_path(status_log_path=True),
             "/var/log/applicationinsights",
         )
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="Windows",
     )
     @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
     def test_log_path_windows(self, mock_system, mock_home):
         self.assertEqual(
-            _constants._get_log_path(),
+            _utils._get_log_path(),
             "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
         )
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="Windows",
     )
     @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
     def test_status_log_path_windows(self, mock_system, mock_home):
         self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
+            _utils._get_log_path(status_log_path=True),
             "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
         )
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="Window",
     )
     def test_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path())
+        self.assertIsNone(_utils._get_log_path())
 
     @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
+        "azure.monitor.opentelemetry._utils.platform.system",
         return_value="linux",
     )
     def test_status_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path(status_log_path=True))
+        self.assertIsNone(_utils._get_log_path(status_log_path=True))
 
     @patch.dict("os.environ", {"key": "value"})
     def test_env_var_or_default(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "value")
+        self.assertEqual(_utils._env_var_or_default("key"), "value")
 
     @patch.dict("os.environ", {})
     def test_env_var_or_default_empty(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "")
+        self.assertEqual(_utils._env_var_or_default("key"), "")
 
     @patch.dict("os.environ", {})
     def test_env_var_or_default_empty_with_defaults(self):
         self.assertEqual(
-            _constants._env_var_or_default("key", default_val="value"), "value"
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.isdir",
-        return_value=True,
-    )
-    def test_attach_enabled(self, mock_isdir):
-        self.assertEqual(
-            _constants._is_attach_enabled(), True
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.isdir",
-        return_value=False,
-    )
-    def test_attach_disabled(self, mock_isdir):
-        self.assertEqual(
-            _constants._is_attach_enabled(), False
+            _utils._env_var_or_default("key", default_val="value"), "value"
         )
```

