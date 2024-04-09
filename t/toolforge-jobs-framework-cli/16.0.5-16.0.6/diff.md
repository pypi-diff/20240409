# Comparing `tmp/toolforge-jobs-framework-cli-16.0.5.tar.gz` & `tmp/toolforge-jobs-framework-cli-16.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-jobs-framework-cli-16.0.5.tar", last modified: Mon Apr  8 08:51:44 2024, max compression
+gzip compressed data, was "toolforge-jobs-framework-cli-16.0.6.tar", last modified: Tue Apr  9 12:05:37 2024, max compression
```

## Comparing `toolforge-jobs-framework-cli-16.0.5.tar` & `toolforge-jobs-framework-cli-16.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.105943 toolforge-jobs-framework-cli-16.0.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    32109 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11108 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    32483 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-09 12:05:33.000000 toolforge-jobs-framework-cli-16.0.6/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 12:05:37.846223 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 12:05:37.000000 toolforge-jobs-framework-cli-16.0.6/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge-jobs-framework-cli-16.0.5/LICENSE` & `toolforge-jobs-framework-cli-16.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/README.md` & `toolforge-jobs-framework-cli-16.0.6/README.md`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/tests/test_api.py` & `toolforge-jobs-framework-cli-16.0.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/tests/test_dump.py` & `toolforge-jobs-framework-cli-16.0.6/tests/test_dump.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "filelog_stdout": "/data/project/tf-test/emails-test.out",
         "filelog_stderr": "/data/project/tf-test/emails-test.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "all",
+        "health_check": None,
     },
     "dump_job": {
         "name": "emails-test",
         "command": "./mycommand.sh --argument1",
         "image": "bullseye",
         "emails": "all",
     },
@@ -68,14 +69,15 @@
         "filelog_stdout": "/data/project/tf-test/normal-job-with-custom-retry-policy.out",
         "filelog_stderr": "/data/project/tf-test/normal-job-with-custom-retry-policy.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "emails": "none",
         "mount": "all",
         "retry": 2,
+        "health_check": None,
     },
     "dump_job": {
         "name": "normal-job-with-custom-retry-policy",
         "command": "./mycommand.sh --argument1",
         "image": "bullseye",
         "retry": 2,
     },
@@ -91,14 +93,15 @@
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "mount-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "mount": "all",
     },
@@ -114,14 +117,15 @@
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "mount-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
     },
 }
@@ -136,14 +140,15 @@
         "filelog_stdout": "/something",
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
         "filelog-stdout": "/something",
@@ -160,14 +165,15 @@
         "filelog_stdout": None,
         "filelog_stderr": "/something",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
         "filelog-stderr": "/something",
@@ -184,14 +190,15 @@
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
     },
 }
@@ -206,14 +213,15 @@
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "none",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "tool-tf-test/tool-tf-test:latest",
         "filelog": "yes",
     },
@@ -229,14 +237,15 @@
         "filelog_stdout": None,
         "filelog_stderr": None,
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "filelog-test",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "no-filelog": "true",
     },
@@ -253,14 +262,15 @@
         "filelog_stderr": "/data/project/tf-test/mem.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
         "memory": "1G",
+        "health_check": None,
     },
     "dump_job": {
         "name": "mem",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "mem": "1G",
     },
@@ -276,24 +286,53 @@
         "filelog_stdout": "/data/project/tf-test/dir/something.out",
         "filelog_stderr": "$TOOL_DATA_DIR/dir/something.err",
         "status_short": "Running for 1m24s",
         "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
         "retry": 0,
         "mount": "all",
         "emails": "none",
+        "health_check": None,
     },
     "dump_job": {
         "name": "short",
         "command": "./mycommand.sh --argument1",
         "image": "bookworm",
         "filelog-stdout": "dir/something.out",
         "filelog-stderr": "dir/something.err",
     },
 }
 
+DumpTestCase_11_healthcheck = {
+    "api_job": {
+        "name": "short",
+        "cmd": "./mycommand.sh --argument1",
+        "image": "bookworm",
+        "image_state": "stable",
+        "filelog": None,
+        "filelog_stdout": None,
+        "filelog_stderr": None,
+        "status_short": "Running for 1m24s",
+        "status_long": "Last run at 2024-03-15T12:47:37Z. Pod in 'Failed' phase. [..]",
+        "retry": 0,
+        "mount": "all",
+        "emails": "none",
+        "health_check": {
+            "type": "script",
+            "script": "./some-healthcheck-script.sh",
+        },
+    },
+    "dump_job": {
+        "name": "short",
+        "command": "./mycommand.sh --argument1",
+        "image": "bookworm",
+        "no-filelog": "true",
+        "health-check-script": "./some-healthcheck-script.sh",
+    },
+}
+
 
 @pytest.mark.parametrize(
     ["testcase"],
     [
         [DumpTestCase_1_emails],
         [DumpTestCase_2_retry],
         [DumpTestCase_3_mount],
@@ -301,13 +340,14 @@
         [DumpTestCase_5_filelog_stdout],
         [DumpTestCase_5_filelog_stderr],
         [DumpTestCase_6_filelog_buildservice],
         [DumpTestCase_7_filelog_buildservice],
         [DumpTestCase_8_filelog_non_buildservice],
         [DumpTestCase_9_memory],
         [DumpTestCase_10_filelog_path_shorten],
+        [DumpTestCase_11_healthcheck],
     ],
 )
 def test_job_prepare_for_dump(mock_tool_account: None, testcase: dict[str, Any]) -> None:
     api_job = testcase["api_job"]
     job_prepare_for_dump(api_job)
     assert api_job == testcase["dump_job"]
```

### Comparing `toolforge-jobs-framework-cli-16.0.5/tests/test_loader.py` & `toolforge-jobs-framework-cli-16.0.6/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/tjf_cli/api.py` & `toolforge-jobs-framework-cli-16.0.6/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/tjf_cli/cli.py` & `toolforge-jobs-framework-cli-16.0.6/tjf_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -895,23 +895,32 @@
     if emails == "none":
         job.pop("emails")
 
     mem = job.get("memory")
     if mem:
         job["mem"] = mem
 
+    health_check = job.get("health_check")
+    if health_check:
+        # not using .get() on purpose to let it break in case of wrong entries
+        if health_check["type"] == "script":
+            job["health-check-script"] = health_check["script"]
+        else:
+            logging.warning(f"unknown health_check from jobs-api: {health_check}")
+
     remove_keys = [
         "cmd",
         "memory",
         "image_state",
         "status_short",
         "status_long",
         "schedule_actual",
         "filelog_stdout",
         "filelog_stderr",
+        "health_check",
     ]
 
     for key in remove_keys:
         try:
             job.pop(key)
         except KeyError:
             # we don't care, this is harmless anyway. For example, schedule_actual is only present on cronjobs
```

### Comparing `toolforge-jobs-framework-cli-16.0.5/tjf_cli/errors.py` & `toolforge-jobs-framework-cli-16.0.6/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.5/tjf_cli/loader.py` & `toolforge-jobs-framework-cli-16.0.6/tjf_cli/loader.py`

 * *Files identical despite different names*

