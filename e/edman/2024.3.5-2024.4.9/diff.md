# Comparing `tmp/edman-2024.3.5.tar.gz` & `tmp/edman-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman-2024.3.5.tar", last modified: Tue Mar  5 01:06:47 2024, max compression
+gzip compressed data, was "edman-2024.4.9.tar", last modified: Tue Apr  9 01:32:46 2024, max compression
```

## Comparing `edman-2024.3.5.tar` & `edman-2024.4.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.461206 edman-2024.3.5/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/.github/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/.github/workflows/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1575 2023-10-13 05:07:31.000000 edman-2024.3.5/.github/workflows/unittest.yml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2283 2023-12-04 07:30:57.000000 edman-2024.3.5/.gitignore
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/.idea/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2024.3.5/.idea/.gitignore
--rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2024.3.5/.idea/edman.iml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/.idea/inspectionProfiles/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2024.3.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      414 2023-10-13 05:07:31.000000 edman-2024.3.5/.idea/misc.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2024.3.5/.idea/modules.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2024.3.5/.idea/vcs.xml
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2024.3.5/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)    13449 2024-03-05 01:06:47.461206 edman-2024.3.5/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11982 2023-11-28 01:23:54.000000 edman-2024.3.5/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/edman/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2023-12-06 08:24:02.000000 edman-2024.3.5/edman/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1537 2023-11-15 06:06:42.000000 edman-2024.3.5/edman/config.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16853 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    50847 2024-02-02 05:59:23.000000 edman-2024.3.5/edman/db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      849 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/exceptions.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    26367 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1748 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/json_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2024.3.5/edman/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)    14173 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11156 2023-12-04 07:30:57.000000 edman-2024.3.5/edman/utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.461206 edman-2024.3.5/edman.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    13449 2024-03-05 01:06:47.000000 edman-2024.3.5/edman.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2024-03-05 01:06:47.000000 edman-2024.3.5/edman.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-03-05 01:06:47.000000 edman-2024.3.5/edman.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       60 2024-03-05 01:06:47.000000 edman-2024.3.5/edman.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2024-03-05 01:06:47.000000 edman-2024.3.5/edman.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1129 2024-03-05 01:04:04.000000 edman-2024.3.5/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)      927 2024-03-05 01:04:04.000000 edman-2024.3.5/requirements.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-03-05 01:06:47.461206 edman-2024.3.5/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.461206 edman-2024.3.5/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2024.3.5/tests/__init__.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.461206 edman-2024.3.5/tests/ini/
--rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2024.3.5/tests/ini/test_db.ini.sample
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12919 2023-12-04 07:30:57.000000 edman-2024.3.5/tests/test_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)   109061 2024-02-02 05:59:23.000000 edman-2024.3.5/tests/test_db.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    45802 2023-12-04 07:30:57.000000 edman-2024.3.5/tests/test_file.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     6644 2023-12-04 07:30:57.000000 edman-2024.3.5/tests/test_multiuser.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    38599 2023-12-19 08:12:30.000000 edman-2024.3.5/tests/test_search.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     8682 2023-12-04 07:30:57.000000 edman-2024.3.5/tests/test_utils.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.451206 edman-2024.3.5/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:06:47.461206 edman-2024.3.5/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2024.3.5/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-17 00:07:28.000000 edman-2024.3.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.720610 edman-2024.4.9/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/.github/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/.github/workflows/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1575 2023-10-13 05:07:31.000000 edman-2024.4.9/.github/workflows/unittest.yml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2283 2023-12-04 07:30:57.000000 edman-2024.4.9/.gitignore
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/.idea/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      238 2022-04-13 07:00:02.000000 edman-2024.4.9/.idea/.gitignore
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      557 2023-04-10 07:58:11.000000 edman-2024.4.9/.idea/edman.iml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/.idea/inspectionProfiles/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      179 2022-04-13 07:00:02.000000 edman-2024.4.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      414 2023-10-13 05:07:31.000000 edman-2024.4.9/.idea/misc.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      269 2022-04-13 07:00:02.000000 edman-2024.4.9/.idea/modules.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      185 2022-04-13 07:00:02.000000 edman-2024.4.9/.idea/vcs.xml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-02-17 05:03:50.000000 edman-2024.4.9/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13449 2024-04-09 01:32:46.720610 edman-2024.4.9/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11982 2023-11-28 01:23:54.000000 edman-2024.4.9/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/edman/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      169 2024-04-08 07:28:55.000000 edman-2024.4.9/edman/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1537 2023-11-15 06:06:42.000000 edman-2024.4.9/edman/config.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16853 2023-12-04 07:30:57.000000 edman-2024.4.9/edman/convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    50847 2024-02-02 05:59:23.000000 edman-2024.4.9/edman/db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      849 2023-12-04 07:30:57.000000 edman-2024.4.9/edman/exceptions.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    26367 2023-12-04 07:30:57.000000 edman-2024.4.9/edman/file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1748 2023-12-04 07:30:57.000000 edman-2024.4.9/edman/json_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-22 08:18:53.000000 edman-2024.4.9/edman/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    14173 2024-04-08 07:30:17.000000 edman-2024.4.9/edman/search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11156 2023-12-04 07:30:57.000000 edman-2024.4.9/edman/utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.720610 edman-2024.4.9/edman.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    13449 2024-04-09 01:32:46.000000 edman-2024.4.9/edman.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      986 2024-04-09 01:32:46.000000 edman-2024.4.9/edman.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 01:32:46.000000 edman-2024.4.9/edman.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       60 2024-04-09 01:32:46.000000 edman-2024.4.9/edman.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       34 2024-04-09 01:32:46.000000 edman-2024.4.9/edman.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1129 2024-04-09 01:29:54.000000 edman-2024.4.9/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1000 2024-04-09 01:29:54.000000 edman-2024.4.9/requirements.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 01:32:46.720610 edman-2024.4.9/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.720610 edman-2024.4.9/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2022-04-13 07:00:02.000000 edman-2024.4.9/tests/__init__.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.720610 edman-2024.4.9/tests/ini/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      166 2022-11-15 02:42:20.000000 edman-2024.4.9/tests/ini/test_db.ini.sample
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12919 2023-12-04 07:30:57.000000 edman-2024.4.9/tests/test_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)   109061 2024-02-02 05:59:23.000000 edman-2024.4.9/tests/test_db.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    45802 2023-12-04 07:30:57.000000 edman-2024.4.9/tests/test_file.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     6644 2023-12-04 07:30:57.000000 edman-2024.4.9/tests/test_multiuser.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    38599 2023-12-19 08:12:30.000000 edman-2024.4.9/tests/test_search.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     8682 2023-12-04 07:30:57.000000 edman-2024.4.9/tests/test_utils.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.710610 edman-2024.4.9/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:32:46.720610 edman-2024.4.9/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1725 2023-04-07 00:37:51.000000 edman-2024.4.9/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      632 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      754 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1089 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      831 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      654 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      820 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      626 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      639 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      675 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      911 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      640 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      708 2023-05-17 00:07:28.000000 edman-2024.4.9/venv/bin/rstpep2html.py
```

### Comparing `edman-2024.3.5/.github/workflows/unittest.yml` & `edman-2024.4.9/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/.gitignore` & `edman-2024.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/.idea/edman.iml` & `edman-2024.4.9/.idea/edman.iml`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/LICENSE.txt` & `edman-2024.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/PKG-INFO` & `edman-2024.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
-Requires-Dist: python-dateutil~=2.9.0.post0
-Requires-Dist: jmespath~=1.0.1
+Requires-Dist: pymongo>=4.6.2
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: jmespath>=1.0.1
 
 edman
 =====
 
 |py_version|
 
 |  KEK IMSS SBRC/PF Experimental Data Management System.
```

### Comparing `edman-2024.3.5/README.rst` & `edman-2024.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/config.py` & `edman-2024.4.9/edman/config.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/convert.py` & `edman-2024.4.9/edman/convert.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/db.py` & `edman-2024.4.9/edman/db.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/exceptions.py` & `edman-2024.4.9/edman/exceptions.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/file.py` & `edman-2024.4.9/edman/file.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/json_manager.py` & `edman-2024.4.9/edman/json_manager.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/search.py` & `edman-2024.4.9/edman/search.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman/utils.py` & `edman-2024.4.9/edman/utils.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/edman.egg-info/PKG-INFO` & `edman-2024.4.9/edman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: KEK IMSS SBRC/PF Experimental Data Management System
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Yusuke Yamada, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: pymongo~=4.6.2
-Requires-Dist: python-dateutil~=2.9.0.post0
-Requires-Dist: jmespath~=1.0.1
+Requires-Dist: pymongo>=4.6.2
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: jmespath>=1.0.1
 
 edman
 =====
 
 |py_version|
 
 |  KEK IMSS SBRC/PF Experimental Data Management System.
```

### Comparing `edman-2024.3.5/edman.egg-info/SOURCES.txt` & `edman-2024.4.9/edman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/pyproject.toml` & `edman-2024.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
-    "pymongo~=4.6.2",
-    "python-dateutil~=2.9.0.post0",
-    "jmespath~=1.0.1",
+    "pymongo>=4.6.2",
+    "python-dateutil>=2.9.0.post0",
+    "jmespath>=1.0.1",
 ]
-version = "2024.3.5"
+version = "2024.4.9"
 # dynamic = ["version"]
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman/"
 "repository" = "https://github.com/ryde/edman"
 
 [tool.setuptools.packages.find]
```

### Comparing `edman-2024.3.5/requirements.txt` & `edman-2024.4.9/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-build==1.1.1
+backports.tarfile==1.0.0
+build==1.2.1
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 cryptography==42.0.5
 dnspython==2.6.1
 docutils==0.20.1
 flake8==7.0.0
 idna==3.6
-importlib-metadata==7.0.1
+importlib_metadata==7.1.0
 iniconfig==2.0.0
 isort==5.13.2
-jaraco.classes==3.3.1
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.0
 jeepney==0.8.0
 jmespath==1.0.1
-keyring==24.3.1
+keyring==25.1.0
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-mypy==1.8.0
+mypy==1.9.0
 mypy-extensions==1.0.0
-nh3==0.2.15
-packaging==23.2
+nh3==0.2.17
+packaging==24.0
 pkginfo==1.10.0
 pluggy==1.4.0
 pycodestyle==2.11.1
-pycparser==2.21
+pycparser==2.22
 pyflakes==3.2.0
 Pygments==2.17.2
 pymongo==4.6.2
 pyproject_hooks==1.0.0
-pytest==8.0.2
+pytest==8.1.1
 python-dateutil==2.9.0.post0
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
 six==1.16.0
 toml==0.10.2
 tomli==2.0.1
 twine==5.0.0
 types-jmespath==1.0.2.20240106
-types-python-dateutil==2.8.19.20240106
-typing_extensions==4.10.0
+types-python-dateutil==2.9.0.20240316
+typing_extensions==4.11.0
 urllib3==2.2.1
-zipp==3.17.0
+zipp==3.18.1
```

### Comparing `edman-2024.3.5/tests/test_convert.py` & `edman-2024.4.9/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/tests/test_db.py` & `edman-2024.4.9/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/tests/test_file.py` & `edman-2024.4.9/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/tests/test_multiuser.py` & `edman-2024.4.9/tests/test_multiuser.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/tests/test_search.py` & `edman-2024.4.9/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/tests/test_utils.py` & `edman-2024.4.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/jp.py` & `edman-2024.4.9/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2html.py` & `edman-2024.4.9/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2html4.py` & `edman-2024.4.9/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2html5.py` & `edman-2024.4.9/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2latex.py` & `edman-2024.4.9/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2man.py` & `edman-2024.4.9/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2odt.py` & `edman-2024.4.9/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2odt_prepstyles.py` & `edman-2024.4.9/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2pseudoxml.py` & `edman-2024.4.9/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2s5.py` & `edman-2024.4.9/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2xetex.py` & `edman-2024.4.9/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rst2xml.py` & `edman-2024.4.9/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman-2024.3.5/venv/bin/rstpep2html.py` & `edman-2024.4.9/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

