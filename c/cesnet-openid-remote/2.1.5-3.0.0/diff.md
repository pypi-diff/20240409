# Comparing `tmp/cesnet-openid-remote-2.1.5.tar.gz` & `tmp/cesnet-openid-remote-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-openid-remote-2.1.5.tar", last modified: Fri Apr  9 16:53:53 2021, max compression
+gzip compressed data, was "cesnet-openid-remote-3.0.0.tar", last modified: Tue Apr  9 11:27:41 2024, max compression
```

## Comparing `cesnet-openid-remote-2.1.5.tar` & `cesnet-openid-remote-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 16:53:53.355646 cesnet-openid-remote-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5949 2021-04-09 16:53:53.355646 cesnet-openid-remote-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 16:53:53.351646 cesnet-openid-remote-2.1.5/cesnet_openid_remote/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 16:53:53.355646 cesnet-openid-remote-2.1.5/cesnet_openid_remote/alembic/
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/alembic/0f27e899fc55_create_cesnet_openid_remote_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/alembic/7b18e6f52083_initial_cesnet_openid_remote_revision.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/alembic/b2f210a5a578_make_group_display_name_optional.py
--rw-r--r--   0 runner    (1001) docker     (121)     7682 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7311 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-09 16:53:53.355646 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5949 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-09 16:53:40.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-09 16:53:53.000000 cesnet-openid-remote-2.1.5/cesnet_openid_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      646 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      522 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-09 16:53:53.355646 cesnet-openid-remote-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2021-04-09 16:52:13.000000 cesnet-openid-remote-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:27:41.965139 cesnet-openid-remote-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 11:27:41.965139 cesnet-openid-remote-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:27:41.961139 cesnet-openid-remote-3.0.0/cesnet_openid_remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote/communities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:27:41.965139 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 11:27:41.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 11:27:41.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:27:41.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 11:27:41.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:27:41.000000 cesnet-openid-remote-3.0.0/cesnet_openid_remote.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/format.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 11:27:41.965139 cesnet-openid-remote-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 11:26:59.000000 cesnet-openid-remote-3.0.0/setup.py
```

### Comparing `cesnet-openid-remote-2.1.5/.editorconfig` & `cesnet-openid-remote-3.0.0/.editorconfig`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 CESNET.
+# Copyright (C) 2023 CESNET.
 #
 # CESNET-OpenID-Remote is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 root = true
```

### Comparing `cesnet-openid-remote-2.1.5/CONTRIBUTING.rst` & `cesnet-openid-remote-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cesnet-openid-remote-2.1.5/LICENSE` & `cesnet-openid-remote-3.0.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (C) 2021 CESNET.
+Copyright (C) 2023 CESNET.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `cesnet-openid-remote-2.1.5/MANIFEST.in` & `cesnet-openid-remote-3.0.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 CESNET.
+# Copyright (C) 2023 CESNET.
 #
 # CESNET-OpenID-Remote is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 # TODO: Generate this manifest file by running the following commands:
 # (please sort the lines in this file after running below commands)
```

### Comparing `cesnet-openid-remote-2.1.5/README.md` & `cesnet-openid-remote-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
 Cesnet OpenID Remote is on PyPI so all you need is:
 
 ``` console
 $ pip install cesnet-openid-remote
 ```
 
+> **Warning**
+> The following section is not supported in the current version.
+
 Then run the following to ensure `cesnet_group` and `cesnet_group_role` mapping database tables
 are created:
 ```console
 $ invenio alembic upgrade heads
 ```
 
 ## Configuration
@@ -61,19 +64,32 @@
 certain Invenio roles, configure such roles in:
 
 ```python
 OAUTHCLIENT_CESNET_OPENID_PROTECTED_ROLES = ['admin']
 """Role names that shouldn't be managed/(un)assigned to users by this extension."""
 ```
 
+5. Add the remote application to the site's `invenio.cfg`:
+
+```py
+from cesnet_openid_remote import remote
+
+OAUTHCLIENT_REMOTE_APPS = {
+    "perun": remote.REMOTE_APP
+}  # configure external login providers
+```
+
 ## CLI
 
+> **Warning**
+> The following section is not supported in the current version.
+
 To manage CESNET group to Invenio Role mappings you can use the following CLI command group:
 ```
-$ invenio cesnet:groups --help
+$ invenio cesnet:group --help
 Usage: invenio cesnet:group [OPTIONS] COMMAND [ARGS]...
 
   Management commands for CESNET external group mappings.
 
 Options:
   --help  Show this message and exit.
 
@@ -82,26 +98,29 @@
   create  Create an external CESNET group.
   list    List external CESNET groups.
   remove  Remove a CESNET group from an Invenio Role.
 ```
 
 ## Customization
 
+> **Warning**
+> The following section is not supported in the current version.
+
 To customize group handling and validation, refer to your custom validation and parse
 functions using the following config values:
 
 ````python
 OAUTHCLIENT_CESNET_OPENID_GROUP_VALIDATOR = 'cesnet_openid_remote.groups.validate_group_uri'
 """Function used to validate external group URI."""
 
 OAUTHCLIENT_CESNET_OPENID_GROUP_PARSER = 'cesnet_openid_remote.groups.parse_group_uri'
 """Function used to parse external group URI to (UUID, extra_data) pair."""
 ````
 
 Further documentation is available on
 https://cesnet-openid-remote.readthedocs.io/
 
-Copyright (C) 2021 CESNET.
+Copyright (C) 2023 CESNET.
 
 CESNET-OpenID-Remote is free software; you can redistribute it and/or
 modify it under the terms of the MIT License; see LICENSE file for more
 details.
```

