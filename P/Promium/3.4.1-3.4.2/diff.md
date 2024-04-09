# Comparing `tmp/Promium-3.4.1.tar.gz` & `tmp/Promium-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Promium-3.4.1.tar", last modified: Tue Mar 26 13:35:32 2024, max compression
+gzip compressed data, was "Promium-3.4.2.tar", last modified: Tue Apr  9 07:53:14 2024, max compression
```

## Comparing `Promium-3.4.1.tar` & `Promium-3.4.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1063 2024-02-21 11:34:03.000000 Promium-3.4.1/LICENSE
--rw-r--r--   0 promium   (1000) promium   (1000)     4888 2024-03-26 13:35:32.899646 Promium-3.4.1/PKG-INFO
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/Promium.egg-info/
--rw-r--r--   0 promium   (1000) promium   (1000)     4888 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/PKG-INFO
--rw-r--r--   0 promium   (1000) promium   (1000)     1388 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/SOURCES.txt
--rw-r--r--   0 promium   (1000) promium   (1000)        1 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/dependency_links.txt
--rw-r--r--   0 promium   (1000) promium   (1000)       36 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/entry_points.txt
--rw-r--r--   0 promium   (1000) promium   (1000)      175 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/requires.txt
--rw-r--r--   0 promium   (1000) promium   (1000)       18 2024-03-26 13:35:32.000000 Promium-3.4.1/Promium.egg-info/top_level.txt
--rw-rw-rw-   0 promium   (1000) promium   (1000)     3822 2024-03-22 15:01:46.000000 Promium-3.4.1/README.rst
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.895646 Promium-3.4.1/doc/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/doc/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      945 2024-02-23 13:10:58.000000 Promium-3.4.1/doc/conf.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.895646 Promium-3.4.1/promium/
--rw-rw-rw-   0 promium   (1000) promium   (1000)      727 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    18734 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/assertions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    24900 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/base.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9170 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/browsers.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9619 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/common.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1725 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/device_config.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/promium/elements/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      335 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/checkbox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      953 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/drop_downs.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      245 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/frame.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1935 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/input_field.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1515 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/elements/link.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      631 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/multiselect_listbox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1118 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/radio_button.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)       98 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/textarea_field.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      200 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/elements/upload_button.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      545 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/exceptions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1724 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/expected_conditions.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1738 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/helpers.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8622 2024-03-22 15:01:46.000000 Promium-3.4.1/promium/logger.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    15366 2024-03-22 15:01:46.000000 Promium-3.4.1/promium/plugin.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/promium/support/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/support/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     9091 2024-02-21 11:34:03.000000 Promium-3.4.1/promium/support/settings.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8066 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/test_case.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8962 2024-03-26 13:27:15.000000 Promium-3.4.1/promium/waits.py
--rw-r--r--   0 promium   (1000) promium   (1000)       38 2024-03-26 13:35:32.899646 Promium-3.4.1/setup.cfg
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1359 2024-03-26 13:27:15.000000 Promium-3.4.1/setup.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/tests/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)       58 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/config.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)       43 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/conftest.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/tests/pages/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/pages/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      624 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/pages/catalog_404_page.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      483 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/pages/catalog_gallery_page.py
-drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-03-26 13:35:32.899646 Promium-3.4.1/tests/settings/
--rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/__init__.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8278 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_base.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     2448 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_chrome.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      896 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_edge.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     4369 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_firefox.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1341 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_ie.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      196 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/settings/test_opera.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1285 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/test_catalog_404.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1447 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/test_catalog_gallery.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     1457 2024-02-24 20:33:12.000000 Promium-3.4.1/tests/test_enviroment.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      801 2024-03-26 13:29:24.000000 Promium-3.4.1/tests/test_requests.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)    13115 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/test_soft_asserts.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)     8461 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/test_waits.py
--rw-rw-rw-   0 promium   (1000) promium   (1000)      445 2024-02-21 11:34:03.000000 Promium-3.4.1/tests/urls.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1063 2024-02-21 11:26:00.000000 Promium-3.4.2/LICENSE
+-rw-r--r--   0 promium   (1000) promium   (1000)     4888 2024-04-09 07:53:14.582391 Promium-3.4.2/PKG-INFO
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/Promium.egg-info/
+-rw-r--r--   0 promium   (1000) promium   (1000)     4888 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/PKG-INFO
+-rw-r--r--   0 promium   (1000) promium   (1000)     1388 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/SOURCES.txt
+-rw-r--r--   0 promium   (1000) promium   (1000)        1 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/dependency_links.txt
+-rw-r--r--   0 promium   (1000) promium   (1000)       36 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/entry_points.txt
+-rw-r--r--   0 promium   (1000) promium   (1000)      175 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/requires.txt
+-rw-r--r--   0 promium   (1000) promium   (1000)       18 2024-04-09 07:53:14.000000 Promium-3.4.2/Promium.egg-info/top_level.txt
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     3822 2024-03-03 13:38:20.000000 Promium-3.4.2/README.rst
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.578391 Promium-3.4.2/doc/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/doc/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      945 2024-02-24 19:27:05.000000 Promium-3.4.2/doc/conf.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.578391 Promium-3.4.2/promium/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      727 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)    18734 2024-03-25 08:24:46.000000 Promium-3.4.2/promium/assertions.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)    24957 2024-04-09 07:49:58.000000 Promium-3.4.2/promium/base.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     9170 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/browsers.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     9619 2024-03-25 08:24:46.000000 Promium-3.4.2/promium/common.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1725 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/device_config.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/promium/elements/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      335 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/checkbox.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      953 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/drop_downs.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      245 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/frame.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1935 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/input_field.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1515 2024-03-25 08:24:46.000000 Promium-3.4.2/promium/elements/link.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      631 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/multiselect_listbox.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1118 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/radio_button.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)       98 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/textarea_field.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      200 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/elements/upload_button.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      545 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/exceptions.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1724 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/expected_conditions.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1738 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/helpers.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     8622 2024-03-25 08:00:37.000000 Promium-3.4.2/promium/logger.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)    15366 2024-03-25 08:00:37.000000 Promium-3.4.2/promium/plugin.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/promium/support/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/support/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     9091 2024-02-21 11:26:00.000000 Promium-3.4.2/promium/support/settings.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     8066 2024-03-26 13:13:10.000000 Promium-3.4.2/promium/test_case.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     8962 2024-03-25 08:24:46.000000 Promium-3.4.2/promium/waits.py
+-rw-r--r--   0 promium   (1000) promium   (1000)       38 2024-04-09 07:53:14.582391 Promium-3.4.2/setup.cfg
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1359 2024-04-09 07:49:58.000000 Promium-3.4.2/setup.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/tests/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)       58 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/config.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)       43 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/conftest.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/tests/pages/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/pages/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      624 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/pages/catalog_404_page.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      483 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/pages/catalog_gallery_page.py
+drwxr-xr-x   0 promium   (1000) promium   (1000)        0 2024-04-09 07:53:14.582391 Promium-3.4.2/tests/settings/
+-rw-rw-rw-   0 promium   (1000) promium   (1000)        0 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/__init__.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     8278 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_base.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     2448 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_chrome.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      896 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_edge.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     4369 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_firefox.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1341 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_ie.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      196 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/settings/test_opera.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1285 2024-02-21 11:44:45.000000 Promium-3.4.2/tests/test_catalog_404.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1447 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/test_catalog_gallery.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     1457 2024-02-24 20:33:42.000000 Promium-3.4.2/tests/test_enviroment.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      801 2024-04-09 07:49:58.000000 Promium-3.4.2/tests/test_requests.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)    13115 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/test_soft_asserts.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)     8461 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/test_waits.py
+-rw-rw-rw-   0 promium   (1000) promium   (1000)      445 2024-02-21 11:26:00.000000 Promium-3.4.2/tests/urls.py
```

### Comparing `Promium-3.4.1/LICENSE` & `Promium-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/PKG-INFO` & `Promium-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Promium
-Version: 3.4.1
+Version: 3.4.2
 Summary: Selenium wrapper for testing Web UI
 Author: Denis Korytkin, Nataliia Guieva, Roman Zaporozhets, Vladimir Kritov, Oleh Dykusha
 Project-URL: Home page, https://none
 Project-URL: Documentation, https://none
 Keywords: Testing UI,Selenium,PageObject,Selenium wrapper
 Platform: linux
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `Promium-3.4.1/Promium.egg-info/PKG-INFO` & `Promium-3.4.2/Promium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Promium
-Version: 3.4.1
+Version: 3.4.2
 Summary: Selenium wrapper for testing Web UI
 Author: Denis Korytkin, Nataliia Guieva, Roman Zaporozhets, Vladimir Kritov, Oleh Dykusha
 Project-URL: Home page, https://none
 Project-URL: Documentation, https://none
 Keywords: Testing UI,Selenium,PageObject,Selenium wrapper
 Platform: linux
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `Promium-3.4.1/Promium.egg-info/SOURCES.txt` & `Promium-3.4.2/Promium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/README.rst` & `Promium-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/doc/conf.py` & `Promium-3.4.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/__init__.py` & `Promium-3.4.2/promium/__init__.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/assertions.py` & `Promium-3.4.2/promium/assertions.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/base.py` & `Promium-3.4.2/promium/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,18 @@
         return get_web_driver(driver._parent)
     error = 'Wrong driver instance. Supported WebDriver and WebElement only'
     raise PromiumException(error)
 
 
 class Page(object):
 
-    def __init__(self, driver):
+    def __init__(self, driver, monkeypatch=None):
         self._driver = driver
         self.previous_window_handle = self.driver.current_window_handle
+        self.monkeypatch = monkeypatch
 
     url = None
 
     @property
     def driver(self):
         return self._driver
```

### Comparing `Promium-3.4.1/promium/browsers.py` & `Promium-3.4.2/promium/browsers.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/common.py` & `Promium-3.4.2/promium/common.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/device_config.py` & `Promium-3.4.2/promium/device_config.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/elements/drop_downs.py` & `Promium-3.4.2/promium/elements/drop_downs.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/elements/input_field.py` & `Promium-3.4.2/promium/elements/input_field.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/elements/link.py` & `Promium-3.4.2/promium/elements/link.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/elements/multiselect_listbox.py` & `Promium-3.4.2/promium/elements/multiselect_listbox.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/elements/radio_button.py` & `Promium-3.4.2/promium/elements/radio_button.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/exceptions.py` & `Promium-3.4.2/promium/exceptions.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/expected_conditions.py` & `Promium-3.4.2/promium/expected_conditions.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/helpers.py` & `Promium-3.4.2/promium/helpers.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/logger.py` & `Promium-3.4.2/promium/logger.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/plugin.py` & `Promium-3.4.2/promium/plugin.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/support/settings.py` & `Promium-3.4.2/promium/support/settings.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/test_case.py` & `Promium-3.4.2/promium/test_case.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/promium/waits.py` & `Promium-3.4.2/promium/waits.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/setup.py` & `Promium-3.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     'deepdiff>=5.7.0',
     'selenium>=4.10.0',
 ]
 
 
 setup(
     name='Promium',
-    version='3.4.1',
+    version='3.4.2',
     install_requires=REQUIREMENTS,
     author='Denis Korytkin, Nataliia Guieva, '
            'Roman Zaporozhets, Vladimir Kritov, '
            'Oleh Dykusha',
     project_urls={
         'Home page': 'https://none',
         'Documentation': 'https://none',
```

### Comparing `Promium-3.4.1/tests/pages/catalog_404_page.py` & `Promium-3.4.2/tests/pages/catalog_404_page.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/settings/test_base.py` & `Promium-3.4.2/tests/settings/test_base.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/settings/test_chrome.py` & `Promium-3.4.2/tests/settings/test_chrome.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/settings/test_edge.py` & `Promium-3.4.2/tests/settings/test_edge.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/settings/test_firefox.py` & `Promium-3.4.2/tests/settings/test_firefox.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/settings/test_ie.py` & `Promium-3.4.2/tests/settings/test_ie.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_catalog_404.py` & `Promium-3.4.2/tests/test_catalog_404.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_catalog_gallery.py` & `Promium-3.4.2/tests/test_catalog_gallery.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_enviroment.py` & `Promium-3.4.2/tests/test_enviroment.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_requests.py` & `Promium-3.4.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_soft_asserts.py` & `Promium-3.4.2/tests/test_soft_asserts.py`

 * *Files identical despite different names*

### Comparing `Promium-3.4.1/tests/test_waits.py` & `Promium-3.4.2/tests/test_waits.py`

 * *Files identical despite different names*

