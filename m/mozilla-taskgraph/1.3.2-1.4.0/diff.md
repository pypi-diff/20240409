# Comparing `tmp/mozilla-taskgraph-1.3.2.tar.gz` & `tmp/mozilla-taskgraph-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-1.3.2.tar", last modified: Tue Apr  2 13:55:03 2024, max compression
+gzip compressed data, was "mozilla-taskgraph-1.4.0.tar", last modified: Tue Apr  9 15:59:43 2024, max compression
```

## Comparing `mozilla-taskgraph-1.3.2.tar` & `mozilla-taskgraph-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.030306 mozilla-taskgraph-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/release_promotion.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/worker_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-02 13:55:03.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 13:55:02.000000 mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:55:03.034306 mozilla-taskgraph-1.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-02 13:54:59.000000 mozilla-taskgraph-1.3.2/test/test_worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.924080 mozilla-taskgraph-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/actions/release_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 15:59:43.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 15:59:43.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:59:43.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 15:59:43.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:59:43.000000 mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:59:43.928080 mozilla-taskgraph-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-09 15:59:38.000000 mozilla-taskgraph-1.4.0/test/test_worker_types.py
```

### Comparing `mozilla-taskgraph-1.3.2/LICENSE` & `mozilla-taskgraph-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/PKG-INFO` & `mozilla-taskgraph-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.3.2
+Version: 1.4.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.3.2/README.md` & `mozilla-taskgraph-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/pyproject.toml` & `mozilla-taskgraph-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/setup.py` & `mozilla-taskgraph-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/__init__.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/__init__.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/actions/release_promotion.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/actions/release_promotion.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/config.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph/worker_types.py` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph/worker_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from taskgraph.transforms.task import payload_builder
+from taskgraph.transforms.task import payload_builder, taskref_or_string
 from voluptuous import Extra, Optional, Required
 
 
 @payload_builder(
     "scriptworker-bitrise",
     schema={
         Required("bitrise"): {
@@ -10,14 +10,17 @@
                 "app", description="Name of Bitrise App to schedule workflows on."
             ): str,
             Required(
                 "workflows",
                 description="List of workflows to trigger on specified app.",
             ): [str],
             Optional(
+                "env", description="Environment variables to pass into the build"
+            ): {str: taskref_or_string},
+            Optional(
                 "build_params",
                 description="Parameters describing the build context to pass "
                 "onto Bitrise. All keys are optional but specific workflows "
                 "may depend on particular keys being set.",
             ): {
                 Optional(
                     "branch",
@@ -45,15 +48,15 @@
                 Optional(
                     "commit_message",
                     description="The commit message of the commit running the build.",
                 ): str,
                 Optional(
                     "environments",
                     description="Environment variables to pass into the build.",
-                ): dict,
+                ): [{Required("mapped_to"): str, Optional("value"): taskref_or_string}],
                 Optional(
                     "pull_request_author",
                     description="The author of the pull request running the build.",
                 ): str,
                 Optional(
                     "pull_request_id",
                     description="The id of the pull request running the build.",
@@ -79,14 +82,21 @@
     scope_prefix = config.graph_config["scriptworker"]["scope-prefix"]
     scopes = task_def.setdefault("scopes", [])
     scopes.append(f"{scope_prefix}:bitrise:app:{bitrise['app']}")
     scopes.extend(
         [f"{scope_prefix}:bitrise:workflow:{wf}" for wf in bitrise["workflows"]]
     )
 
+    # Normalize environment variables to bitrise's format.
+    env = bitrise.get("env", {})
+    if env:
+        build_params.setdefault("environments", [])
+        for k, v in env.items():
+            build_params["environments"].append({"mapped_to": k, "value": v})
+
     # Set some build_params implicitly from Taskcluster params.
     build_params.setdefault("commit_hash", config.params["head_rev"])
     build_params.setdefault("branch_repo_owner", config.params["head_repository"])
 
     def normref(ref, type="heads"):
         if ref:
             prefix = f"refs/{type}/"
```

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.3.2
+Version: 1.4.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.3.2/src/mozilla_taskgraph.egg-info/SOURCES.txt` & `mozilla-taskgraph-1.4.0/src/mozilla_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/test/test_register.py` & `mozilla-taskgraph-1.4.0/test/test_register.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.3.2/test/test_worker_types.py` & `mozilla-taskgraph-1.4.0/test/test_worker_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,14 +121,49 @@
                     }
                 },
                 "scopes": ["foo:bitrise:app:some-app", "foo:bitrise:workflow:bar"],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="normalize refs wrong type",
         ),
+        pytest.param(
+            {
+                "bitrise": {
+                    "app": "some-app",
+                    "env": {
+                        "FOO": "bar",
+                        "PATH": {"artifact-reference": "<build/target.zip>"},
+                    },
+                    "workflows": ["bar"],
+                }
+            },
+            {},
+            {
+                "payload": {
+                    "build_params": {
+                        "branch": "default",
+                        "branch_repo_owner": "http://example.com/head/repo",
+                        "commit_hash": "abcdef",
+                        "environments": [
+                            {"mapped_to": "FOO", "value": "bar"},
+                            {
+                                "mapped_to": "PATH",
+                                "value": {"artifact-reference": "<build/target.zip>"},
+                            },
+                        ],
+                    },
+                },
+                "scopes": [
+                    "foo:bitrise:app:some-app",
+                    "foo:bitrise:workflow:bar",
+                ],
+                "tags": {"worker-implementation": "scriptworker"},
+            },
+            id="environments",
+        ),
     ),
 )
 def test_build_bitrise_payload(
     make_graph_config, make_transform_config, parameters, worker, extra_params, expected
 ):
     schema = payload_builders["scriptworker-bitrise"].schema
```

