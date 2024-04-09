# Comparing `tmp/imioweb.core-1.0a4.tar.gz` & `tmp/imioweb.core-1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imioweb.core-1.0a4.tar", last modified: Thu Mar  7 10:20:51 2024, max compression
+gzip compressed data, was "imioweb.core-1.0a5.tar", last modified: Tue Apr  9 10:48:33 2024, max compression
```

## Comparing `imioweb.core-1.0a4.tar` & `imioweb.core-1.0a5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1926 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/.gitlab-ci.yml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1020 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/.travis.yml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      416 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       66 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      123 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2903 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1399 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.703289 imioweb.core-1.0a4/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7907 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       59 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2448 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.695289 imioweb.core-1.0a4/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.703289 imioweb.core-1.0a4/src/imioweb/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.707289 imioweb.core-1.0a4/src/imioweb/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.707289 imioweb.core-1.0a4/src/imioweb/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      964 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      570 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/contact_info.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.707289 imioweb.core-1.0a4/src/imioweb/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/overrides/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2275 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/overrides/plone.app.contenttypes.browser.templates.listing_summary.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.707289 imioweb.core-1.0a4/src/imioweb/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      629 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/browser/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1330 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      261 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/interfaces.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/locales/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      611 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.699288 imioweb.core-1.0a4/src/imioweb/core/locales/en/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/locales/en/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/en/LC_MESSAGES/imioweb.core.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/imioweb.core.pot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1738 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/update.py
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      473 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/locales/update.sh
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.699288 imioweb.core-1.0a4/src/imioweb/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1163 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      162 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      195 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      170 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      118 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      122 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      613 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1455 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/testing.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      238 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/testing.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.711289 imioweb.core-1.0a4/src/imioweb/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1979 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2378 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2347 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb/core/tests/test_view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-07 10:20:51.707289 imioweb.core-1.0a4/src/imioweb.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2903 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1834 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      117 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/entry_points.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      193 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2024-03-07 10:20:51.000000 imioweb.core-1.0a4/src/imioweb.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1926 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/.gitlab-ci.yml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1020 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/.travis.yml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       66 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      123 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3009 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1399 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7970 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       59 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2448 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.751778 imioweb.core-1.0a5/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      964 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      548 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/contact_info.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/overrides/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2275 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/overrides/plone.app.contenttypes.browser.templates.listing_summary.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      629 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/browser/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1330 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      261 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/interfaces.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/locales/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      611 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/README.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.755777 imioweb.core-1.0a5/src/imioweb/core/locales/en/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/en/LC_MESSAGES/imioweb.core.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/imioweb.core.pot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1739 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/update.py
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      473 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/locales/update.sh
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.755777 imioweb.core-1.0a5/src/imioweb/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1163 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      162 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      105 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      195 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      170 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      118 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      122 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      613 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1455 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/testing.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      238 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/testing.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.763778 imioweb.core-1.0a5/src/imioweb/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1979 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      922 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2275 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2344 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb/core/tests/test_view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-04-09 10:48:33.759777 imioweb.core-1.0a5/src/imioweb.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3009 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1834 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      117 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/entry_points.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      193 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        8 2024-04-09 10:48:33.000000 imioweb.core-1.0a5/src/imioweb.core.egg-info/top_level.txt
```

### Comparing `imioweb.core-1.0a4/.gitlab-ci.yml` & `imioweb.core-1.0a5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/.travis.yml` & `imioweb.core-1.0a5/.travis.yml`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/DEVELOP.rst` & `imioweb.core-1.0a5/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/LICENSE.GPL` & `imioweb.core-1.0a5/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/LICENSE.rst` & `imioweb.core-1.0a5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/PKG-INFO` & `imioweb.core-1.0a5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imioweb.core
-Version: 1.0a4
+Version: 1.0a5
 Summary: Core package for imioweb
 Home-page: https://github.com/collective/imioweb.core
 Author: Benoit Suttor
 Author-email: benoit.suttor@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imioweb.core
 Project-URL: Source, https://github.com/collective/imioweb.core
@@ -105,14 +105,21 @@
 - Benoit Suttor, benoit.suttor@imio.be
 
 
 Changelog
 =========
 
 
+1.0a5 (2024-04-09)
+------------------
+
+- WEB-4089 : Fix recaptcha field must not be required
+  [boulch]
+
+
 1.0a4 (2024-03-07)
 ------------------
 
 - WEB-4089 : Add recaptcha to contact-info form
   [boulch]
```

### Comparing `imioweb.core-1.0a4/README.rst` & `imioweb.core-1.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/docs/conf.py` & `imioweb.core-1.0a5/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,229 +11,226 @@
 
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = []
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'imioweb.core'
-copyright = u'Benoit Suttor (bsuttor)'
-author = u'Benoit Suttor (bsuttor)'
+project = "imioweb.core"
+copyright = "Benoit Suttor (bsuttor)"
+author = "Benoit Suttor (bsuttor)"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u'3.0'
+version = "3.0"
 # The full version, including alpha/beta/rc tags.
-release = u'3.0'
+release = "3.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.
 # "<project> v<release> documentation" by default.
-#html_title = u'bobtemplates.plone v3.0'
+# html_title = u'bobtemplates.plone v3.0'
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (relative to this directory) to use as a favicon of
 # the docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not None, a 'Last updated on:' timestamp is inserted at every page
 # bottom, using the given strftime format.
 # The empty string is equivalent to '%b %d, %Y'.
-#html_last_updated_fmt = None
+# html_last_updated_fmt = None
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr', 'zh'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # 'ja' uses this config value.
 # 'zh' user can custom change `jieba` dictionary path.
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'imioweb.coredoc'
+htmlhelp_basename = "imioweb.coredoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
```

### Comparing `imioweb.core-1.0a4/setup.py` & `imioweb.core-1.0a5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imioweb.core",
-    version='1.0a4',
+    version="1.0a5",
     description="Core package for imioweb",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imioweb.core-1.0a4/src/imioweb/core/browser/configure.zcml` & `imioweb.core-1.0a5/src/imioweb/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/browser/overrides/plone.app.contenttypes.browser.templates.listing_summary.pt` & `imioweb.core-1.0a5/src/imioweb/core/browser/overrides/plone.app.contenttypes.browser.templates.listing_summary.pt`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/browser/view.py` & `imioweb.core-1.0a5/src/imioweb/core/browser/view.py`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/configure.zcml` & `imioweb.core-1.0a5/src/imioweb/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/locales/README.rst` & `imioweb.core-1.0a5/src/imioweb/core/locales/README.rst`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/locales/update.py` & `imioweb.core-1.0a5/src/imioweb/core/locales/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 # -*- coding: utf-8 -*-
 
 import os
 import pkg_resources
 import subprocess
 
 
-domain = 'imioweb.core'
-os.chdir(pkg_resources.resource_filename(domain, ''))
-os.chdir('../../../')
-target_path = 'src/imioweb/core/'
-locale_path = target_path + 'locales/'
-i18ndude = './bin/i18ndude'
+domain = "imioweb.core"
+os.chdir(pkg_resources.resource_filename(domain, ""))
+os.chdir("../../../")
+target_path = "src/imioweb/core/"
+locale_path = target_path + "locales/"
+i18ndude = "./bin/i18ndude"
 
 # ignore node_modules files resulting in errors
 excludes = '"*.html *json-schema*.xml"'
 
 
 def locale_folder_setup():
     os.chdir(locale_path)
-    languages = [d for d in os.listdir('.') if os.path.isdir(d)]
+    languages = [d for d in os.listdir(".") if os.path.isdir(d)]
     for lang in languages:
         folder = os.listdir(lang)
-        if 'LC_MESSAGES' in folder:
+        if "LC_MESSAGES" in folder:
             continue
         else:
-            lc_messages_path = lang + '/LC_MESSAGES/'
+            lc_messages_path = lang + "/LC_MESSAGES/"
             os.mkdir(lc_messages_path)
-            cmd = 'msginit --locale={0} --input={1}.pot --output={2}/LC_MESSAGES/{3}.po'.format(  # NOQA: E501
+            cmd = "msginit --locale={0} --input={1}.pot --output={2}/LC_MESSAGES/{3}.po".format(  # NOQA: E501
                 lang,
                 domain,
                 lang,
                 domain,
             )
             subprocess.call(
                 cmd,
                 shell=True,
             )
 
-    os.chdir('../../../../')
+    os.chdir("../../../../")
 
 
 def _rebuild():
-    cmd = '{i18ndude} rebuild-pot --pot {locale_path}/{domain}.pot --exclude {excludes} --create {domain} {target_path}'.format(  # NOQA: E501
+    cmd = "{i18ndude} rebuild-pot --pot {locale_path}/{domain}.pot --exclude {excludes} --create {domain} {target_path}".format(  # NOQA: E501
         i18ndude=i18ndude,
         locale_path=locale_path,
         domain=domain,
         target_path=target_path,
-        exclude=excludes
+        exclude=excludes,
     )
     subprocess.call(
         cmd,
         shell=True,
     )
 
 
 def _sync():
-    cmd = '{0} sync --pot {1}/{2}.pot {3}*/LC_MESSAGES/{4}.po'.format(
+    cmd = "{0} sync --pot {1}/{2}.pot {3}*/LC_MESSAGES/{4}.po".format(
         i18ndude,
         locale_path,
         domain,
         locale_path,
         domain,
     )
     subprocess.call(
```

### Comparing `imioweb.core-1.0a4/src/imioweb/core/profiles/default/actions.xml` & `imioweb.core-1.0a5/src/imioweb/core/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/setuphandlers.py` & `imioweb.core-1.0a5/src/imioweb/core/setuphandlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @implementer(INonInstallable)
 class HiddenProfiles(object):
 
     def getNonInstallableProfiles(self):
         """Hide uninstall profile from site-creation and quickinstaller."""
         return [
-            'imioweb.core:uninstall',
+            "imioweb.core:uninstall",
         ]
 
 
 def post_install(context):
     """Post install script"""
     # Do something at the end of the installation of this package.
```

### Comparing `imioweb.core-1.0a4/src/imioweb/core/testing.py` & `imioweb.core-1.0a5/src/imioweb/core/testing.py`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/tests/robot/test_example.robot` & `imioweb.core-1.0a5/src/imioweb/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imioweb.core-1.0a4/src/imioweb/core/tests/test_robot.py` & `imioweb.core-1.0a5/src/imioweb/core/tests/test_robot.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 import robotsuite
 import unittest
 
 
 def test_suite():
     suite = unittest.TestSuite()
     current_dir = os.path.abspath(os.path.dirname(__file__))
-    robot_dir = os.path.join(current_dir, 'robot')
+    robot_dir = os.path.join(current_dir, "robot")
     robot_tests = [
-        os.path.join('robot', doc) for doc in os.listdir(robot_dir)
-        if doc.endswith('.robot') and doc.startswith('test_')
+        os.path.join("robot", doc)
+        for doc in os.listdir(robot_dir)
+        if doc.endswith(".robot") and doc.startswith("test_")
     ]
     for robot_test in robot_tests:
         robottestsuite = robotsuite.RobotTestSuite(robot_test)
         robottestsuite.level = ROBOT_TEST_LEVEL
-        suite.addTests([
-            layered(
-                robottestsuite,
-                layer=IMIOWEB_CORE_ACCEPTANCE_TESTING,
-            ),
-        ])
+        suite.addTests(
+            [
+                layered(
+                    robottestsuite,
+                    layer=IMIOWEB_CORE_ACCEPTANCE_TESTING,
+                ),
+            ]
+        )
     return suite
```

### Comparing `imioweb.core-1.0a4/src/imioweb/core/tests/test_setup.py` & `imioweb.core-1.0a5/src/imioweb/core/tests/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,56 +17,50 @@
 class TestSetup(unittest.TestCase):
     """Test that imioweb.core is properly installed."""
 
     layer = IMIOWEB_CORE_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
         if get_installer:
-            self.installer = get_installer(self.portal, self.layer['request'])
+            self.installer = get_installer(self.portal, self.layer["request"])
         else:
-            self.installer = api.portal.get_tool('portal_quickinstaller')
+            self.installer = api.portal.get_tool("portal_quickinstaller")
 
     def test_product_installed(self):
         """Test if imioweb.core is installed."""
-        self.assertTrue(self.installer.isProductInstalled(
-            'imioweb.core'))
+        self.assertTrue(self.installer.isProductInstalled("imioweb.core"))
 
     def test_browserlayer(self):
         """Test that IImiowebCoreLayer is registered."""
-        from imioweb.core.interfaces import (
-            IImiowebCoreLayer)
+        from imioweb.core.interfaces import IImiowebCoreLayer
         from plone.browserlayer import utils
-        self.assertIn(
-            IImiowebCoreLayer,
-            utils.registered_layers())
+
+        self.assertIn(IImiowebCoreLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
 
     layer = IMIOWEB_CORE_INTEGRATION_TESTING
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
         if get_installer:
-            self.installer = get_installer(self.portal, self.layer['request'])
+            self.installer = get_installer(self.portal, self.layer["request"])
         else:
-            self.installer = api.portal.get_tool('portal_quickinstaller')
+            self.installer = api.portal.get_tool("portal_quickinstaller")
         roles_before = api.user.get_roles(TEST_USER_ID)
-        setRoles(self.portal, TEST_USER_ID, ['Manager'])
-        self.installer.uninstallProducts(['imioweb.core'])
+        setRoles(self.portal, TEST_USER_ID, ["Manager"])
+        self.installer.uninstallProducts(["imioweb.core"])
         setRoles(self.portal, TEST_USER_ID, roles_before)
 
     def test_product_uninstalled(self):
         """Test if imioweb.core is cleanly uninstalled."""
-        self.assertFalse(self.installer.isProductInstalled(
-            'imioweb.core'))
+        self.assertFalse(self.installer.isProductInstalled("imioweb.core"))
 
     def test_browserlayer_removed(self):
         """Test that IImiowebCoreLayer is removed."""
-        from imioweb.core.interfaces import \
-            IImiowebCoreLayer
+        from imioweb.core.interfaces import IImiowebCoreLayer
         from plone.browserlayer import utils
-        self.assertNotIn(
-            IImiowebCoreLayer,
-            utils.registered_layers())
+
+        self.assertNotIn(IImiowebCoreLayer, utils.registered_layers())
```

### Comparing `imioweb.core-1.0a4/src/imioweb/core/tests/test_view.py` & `imioweb.core-1.0a5/src/imioweb/core/tests/test_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         applyProfile(self.portal, "collective.taxonomy:examples")
         utility = queryUtility(ITaxonomy, name="collective.taxonomy.test")
         document = api.content.create(
             container=self.portal, type="Document", id="document"
         )
 
         taxonomy_test = schema.Set(
-            title=u"taxonomy_test",
-            description=u"taxonomy description schema",
+            title="taxonomy_test",
+            description="taxonomy description schema",
             required=False,
-            value_type=schema.Choice(vocabulary=u"collective.taxonomy.test"),
+            value_type=schema.Choice(vocabulary="collective.taxonomy.test"),
         )
         portal_types = api.portal.get_tool("portal_types")
         fti = portal_types.get("Document")
         doc_schema = fti.lookupSchema()
         schemaeditor = IEditableSchema(doc_schema)
         schemaeditor.addField(taxonomy_test, name="taxonomy_test")
         notify(ObjectAddedEvent(taxonomy_test, doc_schema))
```

### Comparing `imioweb.core-1.0a4/src/imioweb.core.egg-info/PKG-INFO` & `imioweb.core-1.0a5/src/imioweb.core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imioweb.core
-Version: 1.0a4
+Version: 1.0a5
 Summary: Core package for imioweb
 Home-page: https://github.com/collective/imioweb.core
 Author: Benoit Suttor
 Author-email: benoit.suttor@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imioweb.core
 Project-URL: Source, https://github.com/collective/imioweb.core
@@ -105,14 +105,21 @@
 - Benoit Suttor, benoit.suttor@imio.be
 
 
 Changelog
 =========
 
 
+1.0a5 (2024-04-09)
+------------------
+
+- WEB-4089 : Fix recaptcha field must not be required
+  [boulch]
+
+
 1.0a4 (2024-03-07)
 ------------------
 
 - WEB-4089 : Add recaptcha to contact-info form
   [boulch]
```

### Comparing `imioweb.core-1.0a4/src/imioweb.core.egg-info/SOURCES.txt` & `imioweb.core-1.0a5/src/imioweb.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

