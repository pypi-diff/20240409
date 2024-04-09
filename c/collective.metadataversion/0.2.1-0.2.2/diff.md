# Comparing `tmp/collective.metadataversion-0.2.1.tar.gz` & `tmp/collective.metadataversion-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.metadataversion-0.2.1.tar", last modified: Fri Mar  4 12:19:24 2022, max compression
+gzip compressed data, was "dist/collective.metadataversion-0.2.2.tar", last modified: Tue Feb 14 17:26:19 2023, max compression
```

## Comparing `collective.metadataversion-0.2.1.tar` & `collective.metadataversion-0.2.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2021-08-30 15:30:31.000000 collective.metadataversion-0.2.1/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      679 2021-08-30 16:22:08.000000 collective.metadataversion-0.2.1/docs/LICENSE.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/Extensions/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      559 2021-09-20 09:47:10.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/Extensions/install.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/LC_MESSAGES/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1408 2022-03-04 12:19:23.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.mo
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2128 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.po
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/LC_MESSAGES/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1273 2022-03-04 12:19:23.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.mo
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1985 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.po
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1479 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/locales/collective.metadataversion.pot
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/default/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      472 2021-09-09 09:30:42.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/default/catalog.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       63 2021-09-09 09:33:51.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/default/collective.metadataversion-default.marker
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       69 2021-09-09 09:35:00.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/default/metadata.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      139 2021-09-16 10:31:43.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/default/registry.xml
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/uninstall/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      150 2021-09-16 14:35:09.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles/uninstall/registry.xml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      215 2021-09-20 09:40:21.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      235 2021-09-20 09:40:21.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/_i18n.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      635 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/catalog.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      542 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/config.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      592 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2023 2021-09-09 11:48:17.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/decorator.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1422 2021-09-16 10:10:12.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/exceptions.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1522 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/interfaces.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      986 2021-09-16 11:37:15.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1533 2021-09-20 09:30:52.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    14074 2022-02-24 17:38:56.000000 collective.metadataversion-0.2.1/src/collective/metadataversion/utils.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2021-08-30 15:33:55.000000 collective.metadataversion-0.2.1/src/collective/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8421 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1869 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-09-13 16:37:05.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       72 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      547 2022-03-04 12:18:36.000000 collective.metadataversion-0.2.1/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2021-08-30 15:30:31.000000 collective.metadataversion-0.2.1/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      198 2021-09-13 17:03:00.000000 collective.metadataversion-0.2.1/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5165 2021-11-16 15:02:25.000000 collective.metadataversion-0.2.1/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2022-02-24 17:38:56.000000 collective.metadataversion-0.2.1/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2021-11-16 17:05:08.000000 collective.metadataversion-0.2.1/pyproject.toml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1404 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6288 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.1/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8421 2022-03-04 12:19:24.000000 collective.metadataversion-0.2.1/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2021-08-30 15:30:31.000000 collective.metadataversion-0.2.2/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      679 2021-08-30 16:22:08.000000 collective.metadataversion-0.2.2/docs/LICENSE.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/Extensions/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      559 2021-09-20 09:47:10.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/Extensions/install.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/LC_MESSAGES/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1408 2023-02-14 17:26:14.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.mo
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2128 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.po
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/LC_MESSAGES/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1273 2023-02-14 17:26:14.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.mo
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1985 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.po
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1479 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/locales/collective.metadataversion.pot
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/default/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      472 2021-09-09 09:30:42.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/default/catalog.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       63 2021-09-09 09:33:51.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/default/collective.metadataversion-default.marker
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       69 2021-09-09 09:35:00.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/default/metadata.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      139 2021-09-16 10:31:43.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/default/registry.xml
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/uninstall/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      150 2021-09-16 14:35:09.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles/uninstall/registry.xml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      215 2021-09-20 09:40:21.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      235 2021-09-20 09:40:21.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/_i18n.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      635 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/catalog.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      542 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/config.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      635 2023-02-13 14:33:20.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2023 2021-09-09 11:48:17.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/decorator.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1422 2021-09-16 10:10:12.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/exceptions.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1522 2021-12-06 09:30:44.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/interfaces.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      986 2021-09-16 11:37:15.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1533 2021-09-20 09:30:52.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    17090 2023-02-14 17:21:09.000000 collective.metadataversion-0.2.2/src/collective/metadataversion/utils.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2021-08-30 15:33:55.000000 collective.metadataversion-0.2.2/src/collective/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10600 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1869 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-09-13 16:37:05.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       72 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       11 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1298 2023-02-14 17:26:05.000000 collective.metadataversion-0.2.2/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2021-08-30 15:30:31.000000 collective.metadataversion-0.2.2/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      198 2021-09-13 17:03:00.000000 collective.metadataversion-0.2.2/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6217 2023-02-14 11:15:37.000000 collective.metadataversion-0.2.2/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2023-02-13 14:33:20.000000 collective.metadataversion-0.2.2/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       88 2021-11-16 17:05:08.000000 collective.metadataversion-0.2.2/pyproject.toml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1539 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6662 2023-02-13 14:33:25.000000 collective.metadataversion-0.2.2/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10600 2023-02-14 17:26:19.000000 collective.metadataversion-0.2.2/PKG-INFO
```

### Comparing `collective.metadataversion-0.2.1/docs/LICENSE.GPL` & `collective.metadataversion-0.2.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/docs/LICENSE.rst` & `collective.metadataversion-0.2.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/Extensions/install.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/Extensions/install.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.mo` & `collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.mo`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.po` & `collective.metadataversion-0.2.2/src/collective/metadataversion/locales/de/LC_MESSAGES/collective.metadataversion.po`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.mo` & `collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.mo`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.po` & `collective.metadataversion-0.2.2/src/collective/metadataversion/locales/en/LC_MESSAGES/collective.metadataversion.po`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/locales/collective.metadataversion.pot` & `collective.metadataversion-0.2.2/src/collective/metadataversion/locales/collective.metadataversion.pot`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/catalog.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/catalog.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/config.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/config.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/configure.zcml` & `collective.metadataversion-0.2.2/src/collective/metadataversion/configure.zcml`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     xmlns:zcml="http://namespaces.zope.org/zcml">
 
   <i18n:registerTranslations directory="locales" />
 
   <adapter
       name="metadata_version"
       factory=".catalog.metadata_version"
-      />
+      /><!-- gf:
+          catalog.py
+          -->
 
   <include file="profiles.zcml" />
 
   <!-- -*- extra stuff goes here -*- -->
 
 </configure>
```

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/decorator.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/decorator.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/exceptions.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/interfaces.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/profiles.zcml` & `collective.metadataversion-0.2.2/src/collective/metadataversion/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/setuphandlers.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/src/collective/metadataversion/utils.py` & `collective.metadataversion-0.2.2/src/collective/metadataversion/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -88,32 +88,35 @@
     ...     _update_mmu_kwargs(None, None, metadata_version, kwargs)
     ...     return sorted(kwargs.items())
 
     We can specify a smaller than the recorded version, which will be used for
     comparisons as intended; but it won't be stored by default:
     >>> kw = {}
     >>> ummu(41, kw)                          # doctest: +NORMALIZE_WHITESPACE
-    [('idxs', ['getId']),
+    [('change',        None),
+     ('idxs',         ['getId']),
      ('minimum_version', 41),
      ('new_version',   None),
      ('old_version',     42)]
 
     ... unless we force it to be accepted:
     >>> kw = dict(force_version=1)
     >>> ummu(41, kw)                          # doctest: +NORMALIZE_WHITESPACE
-    [('idxs', ['getId']),
+    [('change',        None),
+     ('idxs',         ['getId']),
      ('minimum_version', 41),
      ('new_version',     41),
      ('old_version',     42)]
 
     This has updated our registry value; thus, a call without a new version
     will result in:
     >>> kw = {}
     >>> ummu(None, kw)                        # doctest: +NORMALIZE_WHITESPACE
-    [('idxs', ['getId']),
+    [('change',        None),
+     ('idxs',         ['getId']),
      ('minimum_version', 41),
      ('new_version',   None),
      ('old_version',     41)]
 
     While we don't necessarily handle *all* legal options here,
     we still reject unknown options, raising the usual TypeError:
 
@@ -135,14 +138,15 @@
                                   ' found %(metadata_version)r'
                                   % locals())
     elif force_version:
         raise UsageValueError('With force_version given, '
                               'we expect a non-None metadata_version!')
     unused = set(kwargs) - set(['idxs', 'force_indexes',
                                 'update_metadata',
+                                'change',  # a function(object, logger)
                                 'debug',
                                 ])
     if unused:
         unused = sorted(unused)
         if strict:
             raise UsageTypeError('Illegal argument(s): %s'
                                  % ', '.join(unused))
@@ -169,14 +173,15 @@
     if 'idxs' not in kwargs:
         if kwargs.get('force_indexes'):
             idxs = None  # refresh all indexes
         else:
             idxs = list(registry[FULL_IDXS_KEY])  # default: a cheap subset
         kwargs['idxs'] = idxs
 
+    kwargs.setdefault('change', None)  # a function(object, logger)
     kwargs.update({
         # metadata_version value, stored in the registry:
         'new_version':     new_version,  # if not None, written to registry
         'old_version':     old_version,  # ... from registry
         # the metadata_version (always a number >= 0)
         # the brain objects are compared to:
         'minimum_version': minimum_version,
@@ -221,14 +226,25 @@
             or not.
     force_indexes -- Refresh the indexes (according to the idxs option above)
             even if the metadata is already up-to-date.
 
     Thus, if you *specify* ``idxs=None`` but not `force_indexes`, all indexes
     will be updated as well if the metadata is considered outdated.
 
+    change -- a function(object, logger) to be called before reindexing is
+              performed.
+              As what we do depends on the metadata_version found in the
+              catalog object, this function call does so as well:
+              If our negotiation concludes to not reindex, this function won't
+              be called, either.
+              Currently the returned value is ignored;
+              if the changes applied by the function might cause more idxs to
+              rot, you currently need to add those to the list (for all),
+              or to specify idxs=None (which will include all indexes).
+
     ... and finally:
 
     update_metadata -- Refresh the metadata columns?
 
         We are not sure yet whether the non-default values make any sense.
         However, the possible values are:
 
@@ -271,14 +287,23 @@
              idxs and 'indexes: ' + ', '.join(idxs) or 'all indexes',
              ]
     debug = kwargs.pop('debug', False)
     if debug:
         _info.append('DEBUG')
 
     logger.info('make_metadata_updater: ' + '; '.join(_info))
+    change = kwargs['change']
+    if change is None:
+        pass
+    elif not callable(change):
+        raise ValueError("change option is expected to be a function"
+                '(object, logger); found %s' % (type(change),))
+    else:
+        logger.info('The %(change)r function(object, logger) will be '
+                    'called before reindexing an object', locals())
 
     def reindex(brain):
         """
         Reindex the object given as brain.
         """
         # if this fails, there is a general problem;
         # e.g., you need to run catalog.xml first
@@ -313,16 +338,51 @@
         else:
             if o is None:
                 txt = '%(brain)r.getObject() returned None!' % locals()
                 logger.error(txt)
                 raise ObjectNotFound(txt, e)
 
         try:
+            if change is not None:
+                res = change(o, logger)
+                if res is not None:
+                    logger.debug('%(res)r <-- change(%(o)r, ...)', locals())
+                    # we might e.g. inject indexes to be updated ...
+                    logger.warn('change(%(o)r: Currently, the returned value '
+                                'is ignored!', locals())
             catalog_reindex(o, idxs=idxs, update_metadata=refresh_metadata)
-        except (ConflictError, KeyboardInterrupt):
+        except IOError as e:
+            # There is a likely source for IOError exception:
+            # PIL (or Pillow), objecting to an unsupported image format.
+            # Of course such errors should be caught by the respective indexer,
+            # allowing for the rest of the objects to be reindexed;
+            # but for now, we like to avoid the whole job to fail
+            # just because of very few foul objects.
+            msg = e.message
+            fail = 1
+            cause = ''
+            if msg is not None:
+                if (msg == 'unrecognized data stream contents'
+                           ' when reading image file'
+                    or msg.startswith('cannot find loader for this ')
+                    ):
+                    cause = ' (PIL)'
+                    fail = 0
+            logger.error('IOError reindexing %(o)r%(cause)s: %(e)r', locals())
+            if fail:
+                raise ReindexingError('Error reindexing %(o)r' % locals(),
+                                      e)
+            else:
+                return False
+        except ConflictError as e:
+            logger.error('ConflictError reindexing %(o)r: %(e)r', locals())
+            # ConflictErrors must never be masked, right?
+            raise
+        except KeyboardInterrupt:
+            logger.error('INTERRUPTED reindexing %(o)r!', locals())
             raise
         except Exception as e:
             logger.error('error reindexing %(o)r: %(e)r', locals())
             raise ReindexingError('Error reindexing %(o)r' % locals(),
                                   e)
         else:
             return True
@@ -368,14 +428,15 @@
     """
     res = {}
     get = (kw.pop if do_pop else kw.get)
     for key in (
         'metadata_version',
         'idxs',
         'force_version', 'force_indexes',
+        'change',  # function(object, logger)
         ):
         if key in kw:
             res[key] = get(key)
     return res
 
 
 if __name__ == '__main__':
```

### Comparing `collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/PKG-INFO` & `collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.metadataversion
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple metadata evolution tracking
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/collective/metadataversion
 Project-URL: Documentation, https://pypi.org/project/collective.metadataversion
@@ -24,15 +24,15 @@
         
         The portal catalog of Zope / Plone sites holds socalled "brains" which have
         metadata attributes  containing the data to be used when the catalog is
         searched and the search results are listed.
         
         Those metadata columns -- like index values -- can be customized,
         and they can evolve over time, as your customization package(s) evolve(s).
-        If your database is small, you'll happily reindex the whole data
+        If your database is small, you might happily reindex the whole database
         whenenver you change something to your metadata (or indexes).
         Or if your metadata is really cheap.
         
         But perhaps this is not the case.
         
         Perhaps you like to be able to reindex the most important parts first,
         and the rest can simply become reindexed when changed.
@@ -63,48 +63,64 @@
         This is how the `.utils.make_metadata_updater` utility function is used.
         
         In your policy package's setuphandler module, you may have::
         
           from collective.metadataversion.decorator import step
           from collective.metadataversion.utils import make_metadata_updater
         
+          #  1 - introduce metadata_version
+          #  2 - append slash to .landing_path
+          #  3 - adjust .landing_path for FancyType objects
+          METADATA_VERSION = 3
+        
           ...
           @step
           def update_metadata_of_prominent_objects(context, logger):
-              reindex = make_metadata_updater(context, logger, 42)
+              reindex = make_metadata_updater(context, logger, METADATA_VERSION)
               catalog = getToolByName(context, 'portal_catalog')
               updated, skipped = 0, 0
-              for brain in catalog(<my fancy query>):
+              for brain in catalog(<fancy query>):
                   if reindex(brain):
                       updated += 1
                   else:
                       skipped += 1
               (... logging ad libitum ...)
         
           @step
           def update_metadata_of_remaining_objects(context, logger):
-              reindex = make_metadata_updater(context, logger, 42)
+              reindex = make_metadata_updater(context, logger, METADATA_VERSION)
               catalog = getToolByName(context, 'portal_catalog')
               updated, skipped = 0, 0
               for brain in catalog({}):
                   if reindex(brain):
                       updated += 1
                   else:
                       skipped += 1
               (... logging ad libitum ...)
         
+          @step
+          def adjust_metadata_version_only(context, logger):
+              """
+              We don't need to reindex anything just now,
+              or we just want to quickly activate the new version
+              (which will then be applied on any change to an object)
+              before starting a really long-running job.
+              """
+              # just use the side effect: persistently update the metadata_version
+              make_metadata_updater(context, logger, METADATA_VERSION)
+        
         The `reindex` function returned by make_metadata_updater() will reindex every
         object (given by brain) which has not been recently reindexed (with
         metadata_version=42), and by default refresh a "cheap" selection of indexes.
         
         Starting with the 2nd call to the first upgrade step, nothing will be actually
         reindexed anymore (unless your <fancy query> spans some more objects now), since
         everything is up-to-date;
         the 2nd upgrade step will update all remaining objects (which might not need to
-        be updated so urgently), and skip all objects caught by the <fancy query>.
+        be updated so urgently), and skip all objects caught by the `<fancy query>`.
         
         
         Notes
         -----
         
         - The ``@step`` decorator makes sure you have a non-None logger.
         
@@ -113,34 +129,39 @@
           the old one (or forced).
         
           This is currently the only utility we provide for this purpose.
           However, you can adjust the registry key directly yourself, if you prefer.
         
         - There are a few keyword-only options for customization.
         
+        - It is theoretically possible to update single metadata columns
+          (see e.g.  plone.app.upgrade_.utils.updateIconsInBrains);
+          such cases are of course not taken into account.
+          We update our `metadata_version` whenever the metadata is updated,
+          using the normally used API.
+        
         
         Translations
         ============
         
         This product has been translated into
         
         - English
         - German
         
         
         Installation
         ============
         
-        Install collective.metadataversion by adding it to your buildout::
+        Install collective.metadataversion_ by adding it to your buildout::
         
             [buildout]
             ...
             eggs =
-                collective.metadataversion
-        
+                collective.metadataversion_
         
         and then running ``bin/buildout``.
         
         After your Zope instance was restarted, you'll have the
         ``collective.metadataversion`` package in your extensions view
         (``/prefs_install_products_form``), or in the "Quick installer";
         select and activate it.
@@ -164,29 +185,55 @@
         
         
         License
         =======
         
         The project is licensed under the GPLv2.
         
+        .. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
         .. _`issue tracker`: https://github.com/collective/metadataversion/issues
+        .. _plone.app.upgrade: https://pypi.org/project/plone.app.upgrade
         
         .. vim: tw=79 cc=+1 sw=4 sts=4 si et
         
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
+        0.2.2 (2023-02-14)
+        ------------------
+        
+        New Features:
+        
+        - `change` option to .utils.make_metadata_updater
+          (a function(object, logger), called before reindexing)
+        
+        Improved exception handling:
+        
+        - When catching IOErrors while reindexing, we inspect the message text;
+          quite likely it's PIL (or Pillow) objecting to an unsupported image format.
+          If so, we log the error, return False, and proceed to the next object.
+          This usually implies the indexes and metadata refresh for the respective object to *fail,*
+          but for the whole rest we should succeed.
+        
+          *Of course,* the error handling should better happen in the respective indexer!
+        
+        - `ConflictError` and `KeyboardInterrupt` exceptions during reindexing are logged
+          and re-raised.
+        
+        [tobiasherp]
+        
+        
         0.2.1 (2022-03-04)
         ------------------
         
         New Features:
         
         - New function .utils.extract_mmu_kwargs
```

### Comparing `collective.metadataversion-0.2.1/src/collective.metadataversion.egg-info/SOURCES.txt` & `collective.metadataversion-0.2.2/src/collective.metadataversion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.metadataversion-0.2.1/README.rst` & `collective.metadataversion-0.2.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 The portal catalog of Zope / Plone sites holds socalled "brains" which have
 metadata attributes  containing the data to be used when the catalog is
 searched and the search results are listed.
 
 Those metadata columns -- like index values -- can be customized,
 and they can evolve over time, as your customization package(s) evolve(s).
-If your database is small, you'll happily reindex the whole data
+If your database is small, you might happily reindex the whole database
 whenenver you change something to your metadata (or indexes).
 Or if your metadata is really cheap.
 
 But perhaps this is not the case.
 
 Perhaps you like to be able to reindex the most important parts first,
 and the rest can simply become reindexed when changed.
@@ -52,48 +52,64 @@
 This is how the `.utils.make_metadata_updater` utility function is used.
 
 In your policy package's setuphandler module, you may have::
 
   from collective.metadataversion.decorator import step
   from collective.metadataversion.utils import make_metadata_updater
 
+  #  1 - introduce metadata_version
+  #  2 - append slash to .landing_path
+  #  3 - adjust .landing_path for FancyType objects
+  METADATA_VERSION = 3
+
   ...
   @step
   def update_metadata_of_prominent_objects(context, logger):
-      reindex = make_metadata_updater(context, logger, 42)
+      reindex = make_metadata_updater(context, logger, METADATA_VERSION)
       catalog = getToolByName(context, 'portal_catalog')
       updated, skipped = 0, 0
-      for brain in catalog(<my fancy query>):
+      for brain in catalog(<fancy query>):
           if reindex(brain):
               updated += 1
           else:
               skipped += 1
       (... logging ad libitum ...)
 
   @step
   def update_metadata_of_remaining_objects(context, logger):
-      reindex = make_metadata_updater(context, logger, 42)
+      reindex = make_metadata_updater(context, logger, METADATA_VERSION)
       catalog = getToolByName(context, 'portal_catalog')
       updated, skipped = 0, 0
       for brain in catalog({}):
           if reindex(brain):
               updated += 1
           else:
               skipped += 1
       (... logging ad libitum ...)
 
+  @step
+  def adjust_metadata_version_only(context, logger):
+      """
+      We don't need to reindex anything just now,
+      or we just want to quickly activate the new version
+      (which will then be applied on any change to an object)
+      before starting a really long-running job.
+      """
+      # just use the side effect: persistently update the metadata_version
+      make_metadata_updater(context, logger, METADATA_VERSION)
+
 The `reindex` function returned by make_metadata_updater() will reindex every
 object (given by brain) which has not been recently reindexed (with
 metadata_version=42), and by default refresh a "cheap" selection of indexes.
 
 Starting with the 2nd call to the first upgrade step, nothing will be actually
 reindexed anymore (unless your <fancy query> spans some more objects now), since
 everything is up-to-date;
 the 2nd upgrade step will update all remaining objects (which might not need to
-be updated so urgently), and skip all objects caught by the <fancy query>.
+be updated so urgently), and skip all objects caught by the `<fancy query>`.
 
 
 Notes
 -----
 
 - The ``@step`` decorator makes sure you have a non-None logger.
 
@@ -102,34 +118,39 @@
   the old one (or forced).
 
   This is currently the only utility we provide for this purpose.
   However, you can adjust the registry key directly yourself, if you prefer.
 
 - There are a few keyword-only options for customization.
 
+- It is theoretically possible to update single metadata columns
+  (see e.g.  plone.app.upgrade_.utils.updateIconsInBrains);
+  such cases are of course not taken into account.
+  We update our `metadata_version` whenever the metadata is updated,
+  using the normally used API.
+
 
 Translations
 ============
 
 This product has been translated into
 
 - English
 - German
 
 
 Installation
 ============
 
-Install collective.metadataversion by adding it to your buildout::
+Install collective.metadataversion_ by adding it to your buildout::
 
     [buildout]
     ...
     eggs =
-        collective.metadataversion
-
+        collective.metadataversion_
 
 and then running ``bin/buildout``.
 
 After your Zope instance was restarted, you'll have the
 ``collective.metadataversion`` package in your extensions view
 (``/prefs_install_products_form``), or in the "Quick installer";
 select and activate it.
@@ -153,10 +174,12 @@
 
 
 License
 =======
 
 The project is licensed under the GPLv2.
 
+.. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
 .. _`issue tracker`: https://github.com/collective/metadataversion/issues
+.. _plone.app.upgrade: https://pypi.org/project/plone.app.upgrade
 
 .. vim: tw=79 cc=+1 sw=4 sts=4 si et
```

### Comparing `collective.metadataversion-0.2.1/setup.cfg` & `collective.metadataversion-0.2.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 import_heading_setup = Setup tools:
 known_plone = plone,Products.CMFPlone
 import_heading_plone = Plone:
 import_heading_stdlib = Standard library:
 import_heading_stdlibold = Standard library (Python 2):
 import_heading_thirdparty = 3rd party:
 import_heading_localfolder = Local imports:
-sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,ZOPE,PLONE,THIRDPARTY,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
+known_pdfreactor = pdfreactor
+import_heading_pdfreactor = PDFreactor (by RealObjects; Python integration by visaplan GmbH):
+sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,PDFREACTOR,ZOPE,PLONE,THIRDPARTY,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
 dedup_headings = True
 multi_line_output = 8
 include_trailing_comma = True
 
 [check-manifest]
 ignore = 
 	*.cfg
```

### Comparing `collective.metadataversion-0.2.1/setup.py` & `collective.metadataversion-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def valid_suffix(suffix):
     """
     Enforce our suffix convention
     """
     suffix = suffix.strip()
     if not suffix:
         return suffix
-    allowed = set('dev.0123456789rcpost')
+    allowed = set('edv.0123456789rcpost')
     disallowed = set(suffix).difference(allowed)
     if disallowed:
         disallowed = ''.join(sorted(disallowed))
         raise ValueError('Version suffix contains disallowed characters'
                          ' (%(disallowed)s)'
                          % locals())
     chunks = suffix.split('.')
@@ -54,14 +54,15 @@
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' starts with a digit'
                              % locals())
         char = chunk[-1]
         if char not in '0123456789':
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' doesn\'t end with a digit'
+                             ' (normalization would append a "0")'
                              % locals())
     return suffix  # ... valid_suffix
     # ... get the version ...
     # ... get the version ...
 VERSION = read_version('VERSION',
                        'VERSION_SUFFIX')
 # -------------------------------------------- ] ... get the version ]
@@ -111,20 +112,25 @@
     if pop_user:
         assert 'pick_user' not in kwargs
         assert 'user' not in kwargs
         user = pkg_list.pop(0)
         package = '.'.join(pkg_list)
     else:
         pick_user = pop('pick_user', 'user' not in kwargs)
+        given_user = pop('user', None)
         if pick_user:
             user = pkg_list[0]
-            if 'user' in kwargs:
-                assert pop('user') == user
+            if given_user is not None and given_user != user:
+                raise ValueError('given user %(given_user)r mismatches '
+                                 'user picked from package %(user)r!'
+                                 % locals())
+        elif given_user is not None:
+            user = given_user
         else:
-            user = pop('user')
+            raise ValueError('no user given nor picked!')
     if pop('travis', False):  # reqires github to be trueish
         res.update({  # CHECKME: is there a de-facto standard key for this?
             'Tests': 'https://travis-ci.org/%(user)s/%(package)s' % locals()
             })
     base = 'https://github.com/%(user)s/%(package)s' % locals()
     res.update({
         'Source': base,
```

### Comparing `collective.metadataversion-0.2.1/PKG-INFO` & `collective.metadataversion-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.metadataversion
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple metadata evolution tracking
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/collective/metadataversion
 Project-URL: Documentation, https://pypi.org/project/collective.metadataversion
@@ -24,15 +24,15 @@
         
         The portal catalog of Zope / Plone sites holds socalled "brains" which have
         metadata attributes  containing the data to be used when the catalog is
         searched and the search results are listed.
         
         Those metadata columns -- like index values -- can be customized,
         and they can evolve over time, as your customization package(s) evolve(s).
-        If your database is small, you'll happily reindex the whole data
+        If your database is small, you might happily reindex the whole database
         whenenver you change something to your metadata (or indexes).
         Or if your metadata is really cheap.
         
         But perhaps this is not the case.
         
         Perhaps you like to be able to reindex the most important parts first,
         and the rest can simply become reindexed when changed.
@@ -63,48 +63,64 @@
         This is how the `.utils.make_metadata_updater` utility function is used.
         
         In your policy package's setuphandler module, you may have::
         
           from collective.metadataversion.decorator import step
           from collective.metadataversion.utils import make_metadata_updater
         
+          #  1 - introduce metadata_version
+          #  2 - append slash to .landing_path
+          #  3 - adjust .landing_path for FancyType objects
+          METADATA_VERSION = 3
+        
           ...
           @step
           def update_metadata_of_prominent_objects(context, logger):
-              reindex = make_metadata_updater(context, logger, 42)
+              reindex = make_metadata_updater(context, logger, METADATA_VERSION)
               catalog = getToolByName(context, 'portal_catalog')
               updated, skipped = 0, 0
-              for brain in catalog(<my fancy query>):
+              for brain in catalog(<fancy query>):
                   if reindex(brain):
                       updated += 1
                   else:
                       skipped += 1
               (... logging ad libitum ...)
         
           @step
           def update_metadata_of_remaining_objects(context, logger):
-              reindex = make_metadata_updater(context, logger, 42)
+              reindex = make_metadata_updater(context, logger, METADATA_VERSION)
               catalog = getToolByName(context, 'portal_catalog')
               updated, skipped = 0, 0
               for brain in catalog({}):
                   if reindex(brain):
                       updated += 1
                   else:
                       skipped += 1
               (... logging ad libitum ...)
         
+          @step
+          def adjust_metadata_version_only(context, logger):
+              """
+              We don't need to reindex anything just now,
+              or we just want to quickly activate the new version
+              (which will then be applied on any change to an object)
+              before starting a really long-running job.
+              """
+              # just use the side effect: persistently update the metadata_version
+              make_metadata_updater(context, logger, METADATA_VERSION)
+        
         The `reindex` function returned by make_metadata_updater() will reindex every
         object (given by brain) which has not been recently reindexed (with
         metadata_version=42), and by default refresh a "cheap" selection of indexes.
         
         Starting with the 2nd call to the first upgrade step, nothing will be actually
         reindexed anymore (unless your <fancy query> spans some more objects now), since
         everything is up-to-date;
         the 2nd upgrade step will update all remaining objects (which might not need to
-        be updated so urgently), and skip all objects caught by the <fancy query>.
+        be updated so urgently), and skip all objects caught by the `<fancy query>`.
         
         
         Notes
         -----
         
         - The ``@step`` decorator makes sure you have a non-None logger.
         
@@ -113,34 +129,39 @@
           the old one (or forced).
         
           This is currently the only utility we provide for this purpose.
           However, you can adjust the registry key directly yourself, if you prefer.
         
         - There are a few keyword-only options for customization.
         
+        - It is theoretically possible to update single metadata columns
+          (see e.g.  plone.app.upgrade_.utils.updateIconsInBrains);
+          such cases are of course not taken into account.
+          We update our `metadata_version` whenever the metadata is updated,
+          using the normally used API.
+        
         
         Translations
         ============
         
         This product has been translated into
         
         - English
         - German
         
         
         Installation
         ============
         
-        Install collective.metadataversion by adding it to your buildout::
+        Install collective.metadataversion_ by adding it to your buildout::
         
             [buildout]
             ...
             eggs =
-                collective.metadataversion
-        
+                collective.metadataversion_
         
         and then running ``bin/buildout``.
         
         After your Zope instance was restarted, you'll have the
         ``collective.metadataversion`` package in your extensions view
         (``/prefs_install_products_form``), or in the "Quick installer";
         select and activate it.
@@ -164,29 +185,55 @@
         
         
         License
         =======
         
         The project is licensed under the GPLv2.
         
+        .. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
         .. _`issue tracker`: https://github.com/collective/metadataversion/issues
+        .. _plone.app.upgrade: https://pypi.org/project/plone.app.upgrade
         
         .. vim: tw=79 cc=+1 sw=4 sts=4 si et
         
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
+        0.2.2 (2023-02-14)
+        ------------------
+        
+        New Features:
+        
+        - `change` option to .utils.make_metadata_updater
+          (a function(object, logger), called before reindexing)
+        
+        Improved exception handling:
+        
+        - When catching IOErrors while reindexing, we inspect the message text;
+          quite likely it's PIL (or Pillow) objecting to an unsupported image format.
+          If so, we log the error, return False, and proceed to the next object.
+          This usually implies the indexes and metadata refresh for the respective object to *fail,*
+          but for the whole rest we should succeed.
+        
+          *Of course,* the error handling should better happen in the respective indexer!
+        
+        - `ConflictError` and `KeyboardInterrupt` exceptions during reindexing are logged
+          and re-raised.
+        
+        [tobiasherp]
+        
+        
         0.2.1 (2022-03-04)
         ------------------
         
         New Features:
         
         - New function .utils.extract_mmu_kwargs
```

