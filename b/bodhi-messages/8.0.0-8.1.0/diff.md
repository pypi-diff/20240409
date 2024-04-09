# Comparing `tmp/bodhi_messages-8.0.0.tar.gz` & `tmp/bodhi_messages-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_messages-8.0.0.tar", max compression
+gzip compressed data, was "bodhi_messages-8.1.0.tar", max compression
```

## Comparing `bodhi_messages-8.0.0.tar` & `bodhi_messages-8.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    18018 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/COPYING
--rw-r--r--   0        0        0       97 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/README.rst
--rw-r--r--   0        0        0      906 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/__init__.py
--rw-r--r--   0        0        0      793 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/__init__.py
--rw-r--r--   0        0        0     9240 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/base.py
--rw-r--r--   0        0        0     5116 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/buildroot_override.py
--rw-r--r--   0        0        0    11249 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/compose.py
--rw-r--r--   0        0        0     3783 2023-05-13 08:55:56.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/errata.py
--rw-r--r--   0        0        0    38621 2023-12-05 13:18:07.000000 bodhi_messages-8.0.0/bodhi/messages/schemas/update.py
--rw-r--r--   0        0        0     1589 2023-07-30 15:01:32.000000 bodhi_messages-8.0.0/bodhi/messages/utils.py
--rw-r--r--   0        0        0     3803 2023-12-09 14:51:40.000000 bodhi_messages-8.0.0/pyproject.toml
--rw-r--r--   0        0        0      788 2023-06-20 08:06:31.000000 bodhi_messages-8.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2713 2023-06-20 08:06:31.000000 bodhi_messages-8.0.0/tests/test_base.py
--rw-r--r--   0        0        0     3500 2023-06-20 08:06:31.000000 bodhi_messages-8.0.0/tests/test_buildroot_override.py
--rw-r--r--   0        0        0     6651 2023-06-20 08:06:31.000000 bodhi_messages-8.0.0/tests/test_compose.py
--rw-r--r--   0        0        0     5321 2023-06-20 08:06:31.000000 bodhi_messages-8.0.0/tests/test_errata.py
--rw-r--r--   0        0        0    46836 2023-12-05 13:18:07.000000 bodhi_messages-8.0.0/tests/test_update.py
--rw-r--r--   0        0        0     2099 2023-07-30 15:01:32.000000 bodhi_messages-8.0.0/tests/utils.py
--rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 bodhi_messages-8.0.0/setup.py
--rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 bodhi_messages-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18018 2024-02-09 16:37:01.450329 bodhi_messages-8.1.0/COPYING
+-rw-r--r--   0        0        0       97 2024-02-09 16:37:01.450329 bodhi_messages-8.1.0/README.rst
+-rw-r--r--   0        0        0      906 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/__init__.py
+-rw-r--r--   0        0        0      793 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/__init__.py
+-rw-r--r--   0        0        0     9240 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/base.py
+-rw-r--r--   0        0        0     5116 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/buildroot_override.py
+-rw-r--r--   0        0        0    11249 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/compose.py
+-rw-r--r--   0        0        0     3783 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/errata.py
+-rw-r--r--   0        0        0    38621 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/schemas/update.py
+-rw-r--r--   0        0        0     1589 2024-02-09 16:37:01.451329 bodhi_messages-8.1.0/bodhi/messages/utils.py
+-rw-r--r--   0        0        0     3803 2024-04-09 11:58:12.178293 bodhi_messages-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2024-02-09 16:37:01.452329 bodhi_messages-8.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2713 2024-02-09 16:37:01.452329 bodhi_messages-8.1.0/tests/test_base.py
+-rw-r--r--   0        0        0     3500 2024-02-09 16:37:01.452329 bodhi_messages-8.1.0/tests/test_buildroot_override.py
+-rw-r--r--   0        0        0     6651 2024-02-09 16:37:01.452329 bodhi_messages-8.1.0/tests/test_compose.py
+-rw-r--r--   0        0        0     5321 2024-02-09 16:37:01.452329 bodhi_messages-8.1.0/tests/test_errata.py
+-rw-r--r--   0        0        0    46836 2024-02-09 16:37:01.453329 bodhi_messages-8.1.0/tests/test_update.py
+-rw-r--r--   0        0        0     2099 2024-02-09 16:37:01.453329 bodhi_messages-8.1.0/tests/utils.py
+-rw-r--r--   0        0        0     4169 1970-01-01 00:00:00.000000 bodhi_messages-8.1.0/setup.py
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 bodhi_messages-8.1.0/PKG-INFO
```

### Comparing `bodhi_messages-8.0.0/COPYING` & `bodhi_messages-8.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/__init__.py` & `bodhi_messages-8.1.0/bodhi/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/__init__.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/base.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/buildroot_override.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/compose.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/errata.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/schemas/update.py` & `bodhi_messages-8.1.0/bodhi/messages/schemas/update.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/bodhi/messages/utils.py` & `bodhi_messages-8.1.0/bodhi/messages/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/pyproject.toml` & `bodhi_messages-8.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-messages"
-version = "8.0.0"
+version = "8.1.0"
 description = "JSON schema for messages sent by Bodhi"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.org"
 keywords = ["fedora", "fedora-messaging"]
```

### Comparing `bodhi_messages-8.0.0/tests/__init__.py` & `bodhi_messages-8.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/test_base.py` & `bodhi_messages-8.1.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/test_buildroot_override.py` & `bodhi_messages-8.1.0/tests/test_buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/test_compose.py` & `bodhi_messages-8.1.0/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/test_errata.py` & `bodhi_messages-8.1.0/tests/test_errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/test_update.py` & `bodhi_messages-8.1.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/tests/utils.py` & `bodhi_messages-8.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-8.0.0/setup.py` & `bodhi_messages-8.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                      'bodhi.update.status.testing.v2 = '
                      'bodhi.messages.schemas.update:UpdateReadyForTestingV2',
                      'bodhi.update.status.testing.v3 = '
                      'bodhi.messages.schemas.update:UpdateReadyForTestingV3']}
 
 setup_kwargs = {
     'name': 'bodhi-messages',
-    'version': '8.0.0',
+    'version': '8.1.0',
     'description': 'JSON schema for messages sent by Bodhi',
     'long_description': 'Bodhi Messages\n==============\n\nThis package contains the schema for messages published by Bodhi.\n',
     'author': 'Fedora Infrastructure Team',
     'author_email': 'None',
     'maintainer': 'Fedora Infrastructure Team',
     'maintainer_email': 'infrastructure@lists.fedoraproject.org',
     'url': 'https://bodhi.fedoraproject.org',
```

### Comparing `bodhi_messages-8.0.0/PKG-INFO` & `bodhi_messages-8.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-messages
-Version: 8.0.0
+Version: 8.1.0
 Summary: JSON schema for messages sent by Bodhi
 Home-page: https://bodhi.fedoraproject.org
 License: GPL-2.0-or-later
 Keywords: fedora,fedora-messaging
 Author: Fedora Infrastructure Team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

