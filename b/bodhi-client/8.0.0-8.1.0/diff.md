# Comparing `tmp/bodhi_client-8.0.0.tar.gz` & `tmp/bodhi_client-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_client-8.0.0.tar", max compression
+gzip compressed data, was "bodhi_client-8.1.0.tar", max compression
```

## Comparing `bodhi_client-8.0.0.tar` & `bodhi_client-8.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/COPYING
--rw-r--r--   0        0        0      935 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/bodhi/client/__init__.py
--rw-r--r--   0        0        0    41276 2023-12-05 13:18:07.000000 bodhi_client-8.0.0/bodhi/client/bindings.py
--rw-r--r--   0        0        0    55426 2023-12-05 13:18:07.000000 bodhi_client-8.0.0/bodhi/client/cli.py
--rw-r--r--   0        0        0      628 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/bodhi/client/constants.py
--rw-r--r--   0        0        0    12718 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/bodhi/client/oidcclient.py
--rwxr-xr-x   0        0        0      236 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/bodhi-client.bash
--rw-r--r--   0        0        0      776 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/docs/Makefile
--rw-r--r--   0        0        0     1115 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/docs/conf.py
--rw-r--r--   0        0        0        0 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/docs/index.rst
--rw-r--r--   0        0        0    18967 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/docs/man_pages/bodhi.rst
--rw-r--r--   0        0        0     1815 2023-12-09 14:51:40.000000 bodhi_client-8.0.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/tests/__init__.py
--rw-r--r--   0        0        0    46868 2023-12-05 13:18:07.000000 bodhi_client-8.0.0/tests/fixtures.py
--rw-r--r--   0        0        0    75092 2023-12-05 13:18:07.000000 bodhi_client-8.0.0/tests/test_bindings.py
--rw-r--r--   0        0        0   124282 2023-12-05 13:18:07.000000 bodhi_client-8.0.0/tests/test_cli.py
--rw-r--r--   0        0        0    15528 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/tests/test_oidcclient.py
--rw-r--r--   0        0        0     2327 2023-05-13 08:55:56.000000 bodhi_client-8.0.0/tests/utils.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 bodhi_client-8.0.0/setup.py
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 bodhi_client-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18018 2024-02-09 16:37:01.445329 bodhi_client-8.1.0/COPYING
+-rw-r--r--   0        0        0      935 2024-02-09 16:37:01.446329 bodhi_client-8.1.0/bodhi/client/__init__.py
+-rw-r--r--   0        0        0    41276 2024-02-09 16:37:01.446329 bodhi_client-8.1.0/bodhi/client/bindings.py
+-rw-r--r--   0        0        0    55426 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/bodhi/client/cli.py
+-rw-r--r--   0        0        0      628 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/bodhi/client/constants.py
+-rw-r--r--   0        0        0    12718 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/bodhi/client/oidcclient.py
+-rwxr-xr-x   0        0        0      236 2024-02-09 16:37:01.445329 bodhi_client-8.1.0/bodhi-client.bash
+-rw-r--r--   0        0        0      776 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1115 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/docs/conf.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/docs/index.rst
+-rw-r--r--   0        0        0    18967 2024-02-09 16:37:01.447329 bodhi_client-8.1.0/docs/man_pages/bodhi.rst
+-rw-r--r--   0        0        0     1815 2024-04-09 11:57:53.241559 bodhi_client-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-02-09 16:37:01.449329 bodhi_client-8.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    46868 2024-02-09 16:37:01.449329 bodhi_client-8.1.0/tests/fixtures.py
+-rw-r--r--   0        0        0    75092 2024-02-09 16:37:01.450329 bodhi_client-8.1.0/tests/test_bindings.py
+-rw-r--r--   0        0        0   124282 2024-02-09 16:37:01.450329 bodhi_client-8.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0    15528 2024-02-09 16:37:01.450329 bodhi_client-8.1.0/tests/test_oidcclient.py
+-rw-r--r--   0        0        0     2327 2024-02-09 16:37:01.450329 bodhi_client-8.1.0/tests/utils.py
+-rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 bodhi_client-8.1.0/setup.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 bodhi_client-8.1.0/PKG-INFO
```

### Comparing `bodhi_client-8.0.0/COPYING` & `bodhi_client-8.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/bodhi/client/__init__.py` & `bodhi_client-8.1.0/bodhi/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/bodhi/client/bindings.py` & `bodhi_client-8.1.0/bodhi/client/bindings.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/bodhi/client/cli.py` & `bodhi_client-8.1.0/bodhi/client/cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/bodhi/client/constants.py` & `bodhi_client-8.1.0/bodhi/client/constants.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/bodhi/client/oidcclient.py` & `bodhi_client-8.1.0/bodhi/client/oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/docs/Makefile` & `bodhi_client-8.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/docs/conf.py` & `bodhi_client-8.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/docs/man_pages/bodhi.rst` & `bodhi_client-8.1.0/docs/man_pages/bodhi.rst`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/pyproject.toml` & `bodhi_client-8.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-client"
-version = "8.0.0"
+version = "8.1.0"
 description = "Bodhi client"
 authors = ["Fedora Infrastructure team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 homepage = "https://bodhi.fedoraproject.org/"
 repository = "https://github.com/fedora-infra/bodhi"
 keywords = ["fedora"]
 license = "GPL-2.0-or-later"
```

### Comparing `bodhi_client-8.0.0/tests/fixtures.py` & `bodhi_client-8.1.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/tests/test_bindings.py` & `bodhi_client-8.1.0/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/tests/test_cli.py` & `bodhi_client-8.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/tests/test_oidcclient.py` & `bodhi_client-8.1.0/tests/test_oidcclient.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/tests/utils.py` & `bodhi_client-8.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_client-8.0.0/setup.py` & `bodhi_client-8.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.27,<3.0']
 
 entry_points = \
 {'console_scripts': ['bodhi = bodhi.client.cli:cli']}
 
 setup_kwargs = {
     'name': 'bodhi-client',
-    'version': '8.0.0',
+    'version': '8.1.0',
     'description': 'Bodhi client',
     'long_description': 'None',
     'author': 'Fedora Infrastructure team',
     'author_email': 'None',
     'maintainer': 'Fedora Infrastructure Team',
     'maintainer_email': 'infrastructure@lists.fedoraproject.org',
     'url': 'https://bodhi.fedoraproject.org/',
```

### Comparing `bodhi_client-8.0.0/PKG-INFO` & `bodhi_client-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-client
-Version: 8.0.0
+Version: 8.1.0
 Summary: Bodhi client
 Home-page: https://bodhi.fedoraproject.org/
 License: GPL-2.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

