# Comparing `tmp/hookee-2.3.4.tar.gz` & `tmp/hookee-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hookee-2.3.4.tar", last modified: Sun Mar 24 13:46:02 2024, max compression
+gzip compressed data, was "hookee-2.3.5.tar", last modified: Tue Apr  9 16:26:01 2024, max compression
```

## Comparing `hookee-2.3.4.tar` & `hookee-2.3.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 13:46:02.799394 hookee-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-03-24 13:44:58.000000 hookee-2.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-24 13:44:58.000000 hookee-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-24 13:44:58.000000 hookee-2.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-24 13:46:02.799394 hookee-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-24 13:44:58.000000 hookee-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 13:46:02.795395 hookee-2.3.4/hookee/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/banner.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/config_default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/hookeemanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/pluginmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 13:46:02.799394 hookee-2.3.4/hookee/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/blueprint_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/request_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/request_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/request_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/request_url_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/response_echo.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/plugins/response_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-03-24 13:44:58.000000 hookee-2.3.4/hookee/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 13:46:02.799394 hookee-2.3.4/hookee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-24 13:46:02.000000 hookee-2.3.4/hookee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-24 13:44:58.000000 hookee-2.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 13:46:02.799394 hookee-2.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 13:46:02.799394 hookee-2.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_hookee_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_hookee_manager_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-24 13:44:58.000000 hookee-2.3.4/tests/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:26:01.796993 hookee-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-09 16:24:59.000000 hookee-2.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 16:24:59.000000 hookee-2.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 16:24:59.000000 hookee-2.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-09 16:26:01.796993 hookee-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-09 16:24:59.000000 hookee-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:26:01.792993 hookee-2.3.5/hookee/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/banner.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/config_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/hookeemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/pluginmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:26:01.796993 hookee-2.3.5/hookee/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/blueprint_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/request_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/request_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/request_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/request_url_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/response_echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/plugins/response_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-09 16:24:59.000000 hookee-2.3.5/hookee/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:26:01.796993 hookee-2.3.5/hookee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 16:26:01.000000 hookee-2.3.5/hookee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-09 16:24:59.000000 hookee-2.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:26:01.796993 hookee-2.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:26:01.796993 hookee-2.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_hookee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_hookee_manager_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-09 16:24:59.000000 hookee-2.3.5/tests/testcase.py
```

### Comparing `hookee-2.3.4/CHANGELOG.md` & `hookee-2.3.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased](https://github.com/alexdlaird/hookee/compare/2.3.4...HEAD)
+## [Unreleased](https://github.com/alexdlaird/hookee/compare/2.3.5...HEAD)
+
+## [2.3.5](https://github.com/alexdlaird/hookee/compare/2.3.3...2.3.4) - 2024-04-09
+### Added
+- Added support for `ngrok` v3 parameters `domain` and `basic_auth`. Backwards compatible with legacy parameters `hostname` and `auth`. 
+- Build improvements.
 
 ## [2.3.4](https://github.com/alexdlaird/hookee/compare/2.3.3...2.3.4) - 2024-03-24
 ### Added
 - Build and stability improvements.
 
 ## [2.3.3](https://github.com/alexdlaird/hookee/compare/2.3.2...2.3.3) - 2024-03-05
 ### Added
```

### Comparing `hookee-2.3.4/LICENSE` & `hookee-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/PKG-INFO` & `hookee-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hookee
-Version: 2.3.4
+Version: 2.3.5
 Summary: Command line webhooks, on demand.
 Maintainer-email: Alex Laird <contact@alexlaird.com>
 License: MIT License
         
         Copyright (c) 2020-2024 Alex Laird
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hookee-2.3.4/README.md` & `hookee-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/cli.py` & `hookee-2.3.5/hookee/cli.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/conf.py` & `hookee-2.3.5/hookee/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 import confuse
 
 from hookee.exception import HookeeConfigError
 
 template = {
     "port": int,
     "subdomain": confuse.String(default=None),
-    "region": confuse.Choice(["us", "eu", "ap", "au", "sa", "jp", "in"], default=None),
+    "region": confuse.Choice(["us", "eu", "ap", "au", "sa", "jp", "in", "us-cal-1"], default=None),
+    "domain": confuse.String(default=None),
+    # Deprecated, use "domain" instead
     "hostname": confuse.String(default=None),
+    "basic_auth": confuse.String(default=None),
+    # Deprecated, use "basic_auth" instead
     "auth": confuse.String(default=None),
     "host_header": confuse.String(default=None),
     "response": confuse.String(default=None),
     "content_type": confuse.String(default=None),
     "request_script": confuse.Filename(default=None),
     "response_script": confuse.Filename(default=None),
     "auth_token": confuse.String(default=os.environ.get("NGROK_AUTHTOKEN")),
@@ -105,24 +109,26 @@
             if not os.path.exists(plugins_dir):
                 os.makedirs(plugins_dir)
         except confuse.NotFoundError as e:
             raise HookeeConfigError(f"The config file is invalid: {str(e)}.")
         except (confuse.ConfigReadError, ValueError):
             raise HookeeConfigError("The config file is not valid YAML.")
 
-    def get(self, key):
+    def get(self, key, default=None):
         """
         Get the config value for the given key of persisted data.
 
         :param key: The key.
         :type key: str
+        :param default: The default, if config not set.
+        :type key: str
         :return: The config value.
         :rtype: object
         """
-        return self.config_data[key]
+        return self.config_data.get(key, default)
 
     def set(self, key, value):
         """
         Update the config key to the given value, persisting to ``config.yaml``.
 
         :param key: The key.
         :type key: str
```

### Comparing `hookee-2.3.4/hookee/hookeemanager.py` & `hookee-2.3.5/hookee/hookeemanager.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/pluginmanager.py` & `hookee-2.3.5/hookee/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/blueprint_default.py` & `hookee-2.3.5/hookee/plugins/blueprint_default.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/request_body.py` & `hookee-2.3.5/hookee/plugins/request_body.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/request_files.py` & `hookee-2.3.5/hookee/plugins/request_files.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/request_headers.py` & `hookee-2.3.5/hookee/plugins/request_headers.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/request_query_params.py` & `hookee-2.3.5/hookee/plugins/request_query_params.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/request_url_info.py` & `hookee-2.3.5/hookee/plugins/request_url_info.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/response_echo.py` & `hookee-2.3.5/hookee/plugins/response_echo.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/plugins/response_info.py` & `hookee-2.3.5/hookee/plugins/response_info.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee/server.py` & `hookee-2.3.5/hookee/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,16 @@
             while self._server_status() != HTTPStatus.OK:
                 time.sleep(1)
 
             self.print_close_header()
 
     def stop(self):
         """
-        If running, kill the server and cleanup its thread.
+        This method is only useful when the Flask version has been overriden to use asn older version (<2). With recent
+        versions of Flask, the underlying server daemon will terminate when ``hookee` terminates.
         """
         if self._thread:
             req = Request(f"http://127.0.0.1:{self.port}/shutdown", method="POST")
             urlopen(req)
 
             self._thread = None
```

### Comparing `hookee-2.3.4/hookee/tunnel.py` & `hookee-2.3.5/hookee/tunnel.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,27 +75,30 @@
 
             while self.public_url is None:
                 time.sleep(1)
 
             self.print_close_header()
 
     def _start_tunnel(self):
-        options = {"bind_tls": True}
+        options = {"schemes": ["https"]}
         subdomain = self.config.get("subdomain")
-        hostname = self.config.get("hostname")
+        domain = self.config.get("domain", self.config.get("hostname"))
         host_header = self.config.get("host_header")
-        auth = self.config.get("auth")
+        basic_auth = self.config.get("basic_auth", self.config.get("auth"))
         if subdomain:
             options["subdomain"] = subdomain
-        if hostname:
-            options["hostname"] = hostname
+        if domain:
+            options["domain"] = domain
         if host_header:
             options["host_header"] = host_header
-        if auth:
-            options["auth"] = auth
+        if basic_auth:
+            if isinstance(basic_auth, list):
+                options["basic_auth"] = basic_auth
+            else:
+                options["basic_auth"] = [basic_auth]
 
         self.public_url = ngrok.connect(self.port,
                                         **options).public_url
         self.ngrok_process = ngrok.get_ngrok_process()
 
     def stop(self):
         """
```

### Comparing `hookee-2.3.4/hookee/util.py` & `hookee-2.3.5/hookee/util.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/hookee.egg-info/PKG-INFO` & `hookee-2.3.5/hookee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hookee
-Version: 2.3.4
+Version: 2.3.5
 Summary: Command line webhooks, on demand.
 Maintainer-email: Alex Laird <contact@alexlaird.com>
 License: MIT License
         
         Copyright (c) 2020-2024 Alex Laird
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hookee-2.3.4/hookee.egg-info/SOURCES.txt` & `hookee-2.3.5/hookee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/pyproject.toml` & `hookee-2.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_cli.py` & `hookee-2.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_config.py` & `hookee-2.3.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_hookee_manager.py` & `hookee-2.3.5/tests/test_hookee_manager.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_hookee_manager_edges.py` & `hookee-2.3.5/tests/test_hookee_manager_edges.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_plugin_manager.py` & `hookee-2.3.5/tests/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/test_util.py` & `hookee-2.3.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `hookee-2.3.4/tests/testcase.py` & `hookee-2.3.5/tests/testcase.py`

 * *Files identical despite different names*

