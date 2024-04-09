# Comparing `tmp/m9s_carrier_weight_volume_combined-7.0.1.tar.gz` & `tmp/m9s_carrier_weight_volume_combined-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_carrier_weight_volume_combined-7.0.1.tar", last modified: Fri Mar  8 19:06:07 2024, max compression
+gzip compressed data, was "m9s_carrier_weight_volume_combined-7.0.2.tar", last modified: Tue Apr  9 11:04:01 2024, max compression
```

## Comparing `m9s_carrier_weight_volume_combined-7.0.1.tar` & `m9s_carrier_weight_volume_combined-7.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.008655 m9s_carrier_weight_volume_combined-7.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      100 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:47.000000 m9s_carrier_weight_volume_combined-7.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3595 2024-03-08 19:06:07.008655 m9s_carrier_weight_volume_combined-7.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1357 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      435 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1782 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/_parcel.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3924 2024-01-21 19:17:04.000000 m9s_carrier_weight_volume_combined-7.0.1/carrier.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      947 2018-02-28 18:25:28.000000 m9s_carrier_weight_volume_combined-7.0.1/carrier.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       75 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      209 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/exceptions.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2166 2021-11-24 18:40:40.000000 m9s_carrier_weight_volume_combined-7.0.1/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.008655 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3595 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1202 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-12-07 09:29:25.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      145 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-03-08 19:06:06.000000 m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      432 2022-02-15 07:52:28.000000 m9s_carrier_weight_volume_combined-7.0.1/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5729 2024-03-08 19:06:02.000000 m9s_carrier_weight_volume_combined-7.0.1/sale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-03-08 19:06:07.008655 m9s_carrier_weight_volume_combined-7.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4721 2024-01-21 17:06:20.000000 m9s_carrier_weight_volume_combined-7.0.1/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2811 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/stock.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      345 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      185 2024-01-21 19:17:34.000000 m9s_carrier_weight_volume_combined-7.0.1/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-08 19:06:07.004655 m9s_carrier_weight_volume_combined-7.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      449 2018-02-28 18:25:28.000000 m9s_carrier_weight_volume_combined-7.0.1/view/carrier_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      333 2020-03-27 12:52:41.000000 m9s_carrier_weight_volume_combined-7.0.1/view/volume_price_list_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      237 2020-03-27 12:52:41.000000 m9s_carrier_weight_volume_combined-7.0.1/view/volume_price_list_tree.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.816429 m9s_carrier_weight_volume_combined-7.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      100 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:22:47.000000 m9s_carrier_weight_volume_combined-7.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3595 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1357 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      435 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1782 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/_parcel.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     5043 2024-04-09 11:03:47.000000 m9s_carrier_weight_volume_combined-7.0.2/carrier.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      947 2018-02-28 18:25:28.000000 m9s_carrier_weight_volume_combined-7.0.2/carrier.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       75 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      209 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/exceptions.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2166 2021-11-24 18:40:40.000000 m9s_carrier_weight_volume_combined-7.0.2/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3595 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1202 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-12-07 09:29:25.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      172 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-09 11:04:01.000000 m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      432 2022-02-15 07:52:28.000000 m9s_carrier_weight_volume_combined-7.0.2/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5729 2024-03-08 19:06:02.000000 m9s_carrier_weight_volume_combined-7.0.2/sale.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-09 11:04:01.816429 m9s_carrier_weight_volume_combined-7.0.2/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4721 2024-01-21 17:06:20.000000 m9s_carrier_weight_volume_combined-7.0.2/setup.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2811 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/stock.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      345 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:57.000000 m9s_carrier_weight_volume_combined-7.0.2/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      198 2024-04-09 11:03:47.000000 m9s_carrier_weight_volume_combined-7.0.2/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-09 11:04:01.812429 m9s_carrier_weight_volume_combined-7.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      449 2018-02-28 18:25:28.000000 m9s_carrier_weight_volume_combined-7.0.2/view/carrier_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      333 2020-03-27 12:52:41.000000 m9s_carrier_weight_volume_combined-7.0.2/view/volume_price_list_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      237 2020-03-27 12:52:41.000000 m9s_carrier_weight_volume_combined-7.0.2/view/volume_price_list_tree.xml
```

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/.drone.yml` & `m9s_carrier_weight_volume_combined-7.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/.gitlab-ci.yml` & `m9s_carrier_weight_volume_combined-7.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/mail_curl.sh` & `m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/report.yml` & `m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/.woodpecker/test.yml` & `m9s_carrier_weight_volume_combined-7.0.2/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/COPYRIGHT` & `m9s_carrier_weight_volume_combined-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/INSTALL` & `m9s_carrier_weight_volume_combined-7.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/LICENSE` & `m9s_carrier_weight_volume_combined-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/PKG-INFO` & `m9s_carrier_weight_volume_combined-7.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_carrier_weight_volume_combined
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton Carrier Weight Volume Combined Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/carrier_weight_volume_combined.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/README.md` & `m9s_carrier_weight_volume_combined-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/_parcel.py` & `m9s_carrier_weight_volume_combined-7.0.2/_parcel.py`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/carrier.py` & `m9s_carrier_weight_volume_combined-7.0.2/carrier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # The COPYRIGHT file at the top level of this repository contains the full
 # copyright notices and license terms.
 from decimal import Decimal
 
 from trytond.model import ModelSQL, ModelView, fields
+from trytond.modules.currency.fields import Monetary
 from trytond.pool import PoolMeta
 from trytond.pyson import Bool, Eval, Id
 from trytond.transaction import Transaction
 
 
 class Carrier(metaclass=PoolMeta):
     __name__ = 'carrier'
     volume_uom = fields.Many2One('product.uom', 'Volume Uom',
         domain=[('category', '=', Id('product', 'uom_cat_volume'))],
         states={
             'invisible': Eval('carrier_cost_method') != 'weight_volume',
             'required': Eval('carrier_cost_method') == 'weight_volume',
-            'readonly': Bool(Eval('weight_price_list', [])),
+            'readonly': Bool(Eval('volume_price_list', [])),
             })
     volume_uom_digits = fields.Function(fields.Integer('Volume Uom Digits'),
         'on_change_with_volume_uom_digits')
     volume_price_list = fields.One2Many('carrier.volume_price_list', 'carrier',
         'Volume Price List',
         states={
             'invisible': Eval('carrier_cost_method') != 'weight_volume',
             'readonly': ~(Eval('volume_uom', 0) & Eval('weight_currency', 0)),
-            })
+            },
+        help="Add price per volume to the carrier service.\n"
+        "The first line for which the volume is greater is used.\n"
+        "The line with volume of 0 is used as default price."
+        )
 
     @classmethod
     def __setup__(cls):
         super(Carrier, cls).__setup__()
         selection = ('weight_volume', 'Weight Volume Combined')
         if selection not in cls.carrier_cost_method.selection:
             cls.carrier_cost_method.selection.append(selection)
@@ -52,47 +57,72 @@
         return 2
 
     def compute_volume_price(self, volume):
         "Compute price based on volume"
         for line in reversed(self.volume_price_list):
             if line.volume < volume:
                 return line.price
+        else:
+            if not line.volume and not volume:
+                return line.price
         return Decimal(0)
 
+    def _get_volume_price(self):
+        volumes = Transaction().context.get('volumes', [])
+        if volumes:
+            volume_price = sum(
+                self.compute_volume_price(v) for v in volumes)
+        else:
+            volume_price = self.compute_volume_price(0)
+        return volume_price, self.weight_currency.id
+
     def get_sale_price(self):
         if self.carrier_cost_method == 'weight_volume':
-            return self._compute_price(), self.weight_currency.id
+            return self._compute_price()
         return super().get_sale_price()
 
     def get_purchase_price(self):
         if self.carrier_cost_method == 'weight_volume':
-            return self._compute_price(), self.weight_currency.id
+            return self._compute_price()
         return super().get_purchase_price()
 
     def _compute_price(self):
         '''
         The highest match for either weight or volume determines the
         necessary price
         '''
-        weight_price = Decimal(0)
-        for weight in Transaction().context.get('weights', []):
-            weight_price += self.compute_weight_price(weight)
-        volume_price = Decimal(0)
-        for volume in Transaction().context.get('volumes', []):
-            volume_price += self.compute_volume_price(volume)
-        return max(weight_price, volume_price)
+        weight_price, currency_id = self._get_weight_price()
+        volume_price, currency_id = self._get_volume_price()
+        return max(weight_price, volume_price), currency_id
 
 
 class VolumePriceList(ModelSQL, ModelView):
     'Carrier Volume Price List'
     __name__ = 'carrier.volume_price_list'
     carrier = fields.Many2One('carrier', 'Carrier', required=True)
-    volume = fields.Float('Volume',
-        digits=(16, Eval('_parent_carrier', {}).get('volume_uom_digits', 2)))
-    price = fields.Numeric('Price',
-        digits=(
-            16, Eval('_parent_carrier', {}).get('weight_currency_digits', 2)))
+    volume = fields.Float('Volume', digits='volume_uom',
+        domain=[
+            ('volume', '>=', 0),
+            ],
+        depends={'carrier'})
+    price = Monetary('Price', currency='currency', digits='currency')
+    currency = fields.Function(fields.Many2One(
+            'currency.currency', "Currency"),
+        'on_change_with_currency')
+    volume_uom = fields.Function(fields.Many2One(
+            'product.uom', "Volume UoM",
+            help="The Unit of Measure of the volume."),
+        'on_change_with_volume_uom')
 
     @classmethod
     def __setup__(cls):
-        super(VolumePriceList, cls).__setup__()
+        super().__setup__()
         cls._order.insert(0, ('volume', 'ASC'))
+
+    @fields.depends('carrier', '_parent_carrier.weight_currency')
+    def on_change_with_currency(self, name=None):
+        if self.carrier and self.carrier.weight_currency:
+            return self.carrier.weight_currency.id
+
+    @fields.depends('carrier', '_parent_carrier.volume_uom')
+    def on_change_with_volume_uom(self, name=None):
+        return self.carrier.volume_uom if self.carrier else None
```

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/carrier.xml` & `m9s_carrier_weight_volume_combined-7.0.2/carrier.xml`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/locale/de.po` & `m9s_carrier_weight_volume_combined-7.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/PKG-INFO` & `m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-carrier-weight-volume-combined
-Version: 7.0.1
+Version: 7.0.2
 Summary: Tryton Carrier Weight Volume Combined Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/carrier_weight_volume_combined.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/m9s_carrier_weight_volume_combined.egg-info/SOURCES.txt` & `m9s_carrier_weight_volume_combined-7.0.2/m9s_carrier_weight_volume_combined.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/sale.py` & `m9s_carrier_weight_volume_combined-7.0.2/sale.py`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/setup.py` & `m9s_carrier_weight_volume_combined-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/stock.py` & `m9s_carrier_weight_volume_combined-7.0.2/stock.py`

 * *Files identical despite different names*

### Comparing `m9s_carrier_weight_volume_combined-7.0.1/tox.ini` & `m9s_carrier_weight_volume_combined-7.0.2/tox.ini`

 * *Files identical despite different names*

