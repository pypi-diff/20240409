# Comparing `tmp/prelude-sdk-1.7.0.tar.gz` & `tmp/prelude-sdk-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.7.0.tar", last modified: Tue Mar 12 21:38:43 2024, max compression
+gzip compressed data, was "prelude-sdk-1.7.1.tar", last modified: Tue Apr  9 20:52:02 2024, max compression
```

## Comparing `prelude-sdk-1.7.0.tar` & `prelude-sdk-1.7.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.731169 prelude-sdk-1.7.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.7.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-03-12 21:38:43.731096 prelude-sdk-1.7.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.7.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.724744 prelude-sdk-1.7.0/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.0/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.727600 prelude-sdk-1.7.0/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4305 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     5618 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     7692 2024-01-05 14:14:44.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3113 2023-12-08 16:31:30.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-12-08 16:31:30.000000 prelude-sdk-1.7.0/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.728399 prelude-sdk-1.7.0/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.0/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.7.0/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     4545 2024-03-01 18:30:16.000000 prelude-sdk-1.7.0/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.730864 prelude-sdk-1.7.0/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-03-12 21:38:43.000000 prelude-sdk-1.7.0/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      752 2024-03-12 21:38:43.000000 prelude-sdk-1.7.0/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-03-12 21:38:43.000000 prelude-sdk-1.7.0/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2024-03-12 21:38:43.000000 prelude-sdk-1.7.0/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-03-12 21:38:43.000000 prelude-sdk-1.7.0/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.7.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2024-03-12 21:38:43.731508 prelude-sdk-1.7.0/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.730512 prelude-sdk-1.7.0/tests/
--rw-r--r--   0 pack       (501) staff       (20)     1258 2024-03-01 18:30:16.000000 prelude-sdk-1.7.0/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-03-12 21:38:43.730717 prelude-sdk-1.7.0/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.7.0/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     5961 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/tests/test_build.py
--rw-r--r--   0 pack       (501) staff       (20)     5018 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/tests/test_detect.py
--rw-r--r--   0 pack       (501) staff       (20)     7694 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/tests/test_iam.py
--rw-r--r--   0 pack       (501) staff       (20)    12179 2024-03-01 18:30:16.000000 prelude-sdk-1.7.0/tests/test_partner.py
--rw-r--r--   0 pack       (501) staff       (20)     3857 2024-03-12 19:51:09.000000 prelude-sdk-1.7.0/tests/test_probe.py
--rw-r--r--   0 pack       (501) staff       (20)      971 2024-03-01 18:30:16.000000 prelude-sdk-1.7.0/tests/testutils.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601940 prelude-sdk-1.7.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-09 20:52:02.601780 prelude-sdk-1.7.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.7.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.592973 prelude-sdk-1.7.1/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.596385 prelude-sdk-1.7.1/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     5859 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6376 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      958 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/generate_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     7692 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3581 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.597579 prelude-sdk-1.7.1/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.7.1/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     4642 2024-04-09 20:41:14.000000 prelude-sdk-1.7.1/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601459 prelude-sdk-1.7.1/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      799 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-09 20:52:02.602232 prelude-sdk-1.7.1/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.600237 prelude-sdk-1.7.1/tests/
+-rw-r--r--   0 pack       (501) staff       (20)     1258 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601175 prelude-sdk-1.7.1/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.7.1/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     8164 2024-04-03 22:19:39.000000 prelude-sdk-1.7.1/tests/test_build.py
+-rw-r--r--   0 pack       (501) staff       (20)     5018 2024-03-12 19:51:09.000000 prelude-sdk-1.7.1/tests/test_detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     7801 2024-04-03 22:19:39.000000 prelude-sdk-1.7.1/tests/test_iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    12179 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/test_partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     3857 2024-03-12 19:51:09.000000 prelude-sdk-1.7.1/tests/test_probe.py
+-rw-r--r--   0 pack       (501) staff       (20)      971 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/testutils.py
```

### Comparing `prelude-sdk-1.7.0/LICENSE` & `prelude-sdk-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/PKG-INFO` & `prelude-sdk-1.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.0
+Version: 1.7.1
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.7.0/README.md` & `prelude-sdk-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.7.1/prelude_sdk/controllers/build_controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 
 from prelude_sdk.models.account import verify_credentials
+from prelude_sdk.models.codes import Control
 
 
 class BuildController:
 
     def __init__(self, account):
         self.account = account
 
@@ -75,25 +76,23 @@
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def create_threat(self, name, threat_id=None, source_id=None, source=None, published=None, tests=None):
+    def create_threat(self, name, published, threat_id=None, source_id=None, source=None, tests=None):
         """ Create a threat """
-        body = dict(name=name)
+        body = dict(name=name, published=published)
         if threat_id:
             body['id'] = threat_id
         if source_id:
             body['source_id'] = source_id
         if source:
             body['source'] = source
-        if published:
-            body['published'] = published
         if tests:
             body['tests'] = tests
 
         res = requests.post(
             f'{self.account.hq}/build/threats',
             json=body,
             headers=self.account.headers,
@@ -136,7 +135,57 @@
             json=dict(purge=purge),
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
+
+    @verify_credentials
+    def create_detection(self, rule: str, test_id: str, detection_id=None, rule_id=None):
+        """ Create a detection """
+        body = dict(rule=rule, test_id=test_id)
+        if detection_id:
+            body['detection_id'] = detection_id
+        if rule_id:
+            body['rule_id'] = rule_id
+
+        res = requests.post(
+            f'{self.account.hq}/build/detections',
+            json=body,
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
+    @verify_credentials
+    def update_detection(self, detection_id: str, rule=None, test_id=None):
+        """ Update a detection """
+        body = dict()
+        if rule:
+            body['rule'] = rule
+        if test_id:
+            body['test_id'] = test_id
+
+        res = requests.post(
+            f'{self.account.hq}/build/detections/{detection_id}',
+            json=body,
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
+    @verify_credentials
+    def delete_detection(self, detection_id: str):
+        """ Delete an existing detection """
+        res = requests.delete(
+            f'{self.account.hq}/build/detections/{detection_id}',
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
```

### Comparing `prelude-sdk-1.7.0/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.7.1/prelude_sdk/controllers/detect_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from prelude_sdk.models.codes import RunCode
 from prelude_sdk.models.account import verify_credentials
+from prelude_sdk.models.codes import RunCode
 
 
 class DetectController:
 
     def __init__(self, account):
         self.account = account
 
@@ -130,14 +130,39 @@
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
+    @verify_credentials
+    def list_detections(self):
+        """ List detections """
+        res = requests.get(
+            f'{self.account.hq}/detect/detections',
+            headers=self.account.headers,
+            params={},
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
+    @verify_credentials
+    def get_detection(self, detection_id):
+        """ Get properties of an existing detection """
+        res = requests.get(
+            f'{self.account.hq}/detect/detections/{detection_id}',
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
     @verify_credentials
     def download(self, test_id, filename):
         """ Clone a test file or attachment"""
         res = requests.get(
             f'{self.account.hq}/detect/tests/{test_id}/{filename}',
             headers=self.account.headers,
             timeout=10
```

### Comparing `prelude-sdk-1.7.0/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.7.1/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.7.1/prelude_sdk/controllers/partner_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,7 +84,21 @@
             headers=self.account.headers,
             json=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
+
+    @verify_credentials
+    def list_reports(self, partner: Control, test_id: str):
+        """ Get reports to a partner for a test """
+        params = dict(test_id=test_id)
+        res = requests.get(
+            f'{self.account.hq}/partner/reports/{partner.name}',
+            headers=self.account.headers,
+            json=params,
+            timeout=30
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
```

### Comparing `prelude-sdk-1.7.0/prelude_sdk/models/account.py` & `prelude-sdk-1.7.1/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/prelude_sdk/models/codes.py` & `prelude-sdk-1.7.1/prelude_sdk/models/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         return Permission.INVALID
 
 
 class ExitCode(Enum):
     MISSING = -1
     UNKNOWN_ERROR = 1
     MALFORMED_TEST = 2
+    UNREPORTED = 3
     PROCESS_BLOCKED = 9
     PROCESS_BLOCKED_GRACEFULLY = 15
     PROTECTED = 100
     UNPROTECTED = 101
     TIMED_OUT = 102
     FAILED_CLEANUP = 103
     TEST_NOT_RELEVANT = 104
@@ -100,42 +101,43 @@
     UNPROTECTED = 2
     ERROR = 3
     NOT_RELEVANT = 4
 
     @classmethod
     def mapping(cls):
         return {
+            State.ERROR: [
+                ExitCode.FAILED_CLEANUP,
+                ExitCode.MALFORMED_TEST,
+                ExitCode.TIMED_OUT,
+                ExitCode.UNEXPECTED_ERROR,
+                ExitCode.UNKNOWN_ERROR,
+                ExitCode.UNREPORTED,
+            ],
             State.NONE: [ExitCode.MISSING],
+            State.NOT_RELEVANT: [
+                ExitCode.ENDPOINT_NOT_RELEVANT,
+                ExitCode.TEST_NOT_RELEVANT,
+            ],
             State.PROTECTED: [
+                ExitCode.BLOCKED,
+                ExitCode.BLOCKED_AT_PERIMETER,
+                ExitCode.DYNAMIC_QUARANTINE,
+                ExitCode.ENDPOINT_NOT_RELEVANT,
+                ExitCode.EXPLOIT_PREVENTED,
                 ExitCode.PROCESS_BLOCKED,
                 ExitCode.PROCESS_BLOCKED_GRACEFULLY,
                 ExitCode.PROTECTED,
-                ExitCode.DYNAMIC_QUARANTINE,
-                ExitCode.BLOCKED_AT_PERIMETER,
-                ExitCode.BLOCKED,
-                ExitCode.EXPLOIT_PREVENTED,
-                ExitCode.TEST_DISALLOWED,
                 ExitCode.STATIC_QUARANTINE,
+                ExitCode.TEST_DISALLOWED,
                 ExitCode.TEST_NOT_RELEVANT,
-                ExitCode.ENDPOINT_NOT_RELEVANT
             ],
             State.UNPROTECTED: [
                 ExitCode.UNPROTECTED,
             ],
-            State.ERROR: [
-                ExitCode.UNKNOWN_ERROR,
-                ExitCode.MALFORMED_TEST,
-                ExitCode.TIMED_OUT,
-                ExitCode.FAILED_CLEANUP,
-                ExitCode.UNEXPECTED_ERROR
-            ],
-            State.NOT_RELEVANT: [
-                ExitCode.TEST_NOT_RELEVANT,
-                ExitCode.ENDPOINT_NOT_RELEVANT
-            ]
         }
 
 
 class DOS(Enum):
     none = 'none'
     arm64 = 'arm64'
     x86_64 = 'x86_64'
@@ -166,35 +168,36 @@
     def _missing_(cls, value):
         return Control.INVALID
 
 
 class AuditEvent(Enum, metaclass=MissingItem):
     INVALID = 0
     ATTACH_PARTNER = 1
+    CREATE_DETECTION = 25
     CREATE_TEST = 2
     CREATE_THREAT = 18
     CREATE_USER = 3
+    DELETE_DETECTION = 26
     DELETE_ENDPOINT = 4
     DELETE_TEST = 5
     DELETE_THREAT = 20
     DELETE_USER = 6
     DETACH_PARTNER = 7
     DISABLE_TEST = 8
     DOWNLOAD_TEST_ATTACHMENT = 9
     ENABLE_TEST = 10
-    GET_THREAT = 21
-    LIST_THREATS = 22
     PARTNER_BLOCK_TEST = 11
     REGISTER_ENDPOINT = 12
     SCHEDULE = 23
     UNSCHEDULE = 24
     UPDATE_ACCOUNT = 13
+    UPDATE_DETECTIONS = 27
     UPDATE_ENDPOINT = 14
     UPDATE_TEST = 15
     UPDATE_THREAT = 19
     UPDATE_USER = 17
     UPLOAD_TEST_ATTACHMENT = 16
-    # Next value: 25
+    # Next value: 28
 
     @classmethod
     def _missing_(cls, value):
         return AuditEvent.INVALID
```

### Comparing `prelude-sdk-1.7.0/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.7.1/prelude_sdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.0
+Version: 1.7.1
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.7.0/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.7.1/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 prelude_sdk.egg-info/SOURCES.txt
 prelude_sdk.egg-info/dependency_links.txt
 prelude_sdk.egg-info/requires.txt
 prelude_sdk.egg-info/top_level.txt
 prelude_sdk/controllers/__init__.py
 prelude_sdk/controllers/build_controller.py
 prelude_sdk/controllers/detect_controller.py
+prelude_sdk/controllers/generate_controller.py
 prelude_sdk/controllers/iam_controller.py
 prelude_sdk/controllers/partner_controller.py
 prelude_sdk/controllers/probe_controller.py
 prelude_sdk/models/__init__.py
 prelude_sdk/models/account.py
 prelude_sdk/models/codes.py
 tests/conftest.py
```

### Comparing `prelude-sdk-1.7.0/setup.cfg` & `prelude-sdk-1.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.7.0
+version = 1.7.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.7.0/tests/conftest.py` & `prelude-sdk-1.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/tests/test_build.py` & `prelude-sdk-1.7.1/tests/test_build.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
     def setup_class(self):
         self.build = BuildController(pytest.account)
         self.detect = DetectController(pytest.account)
 
         self.test_id = str(uuid.uuid4())
         self.name = 'test'
-        self.updated_name = 'updated_test'
         self.unit = 'custom'
         self.technique = 'T1234.001'
 
-    def test_create_test(self, unwrap):
+    def test_create_test(self, unwrap, email):
         res = unwrap(self.build.create_test)(self.build, test_id=self.test_id, name=self.name, unit=self.unit)
 
         pytest.test_id = self.test_id
         pytest.expected_test = dict(
             account_id=pytest.account.headers['account'],
+            author=email,
             id=self.test_id,
             name=self.name,
             unit=self.unit,
             technique=None,
             attachments=[],
             tombstoned=None
         )
@@ -86,17 +86,18 @@
         mine = [r for r in res if r['account_id'] == pytest.account.headers['account']]
         assert 1 == len(mine)
         del pytest.expected_test['attachments']
         diffs = check_dict_items(pytest.expected_test, mine[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_update_test(self, unwrap):
-        res = unwrap(self.build.update_test)(self.build, test_id=self.test_id, name=self.updated_name, technique=self.technique)
+        updated_name = 'updated_test'
+        res = unwrap(self.build.update_test)(self.build, test_id=self.test_id, name=updated_name, technique=self.technique)
 
-        pytest.expected_test['name'] = self.updated_name
+        pytest.expected_test['name'] = updated_name
         pytest.expected_test['technique'] = self.technique
 
         diffs = check_dict_items(pytest.expected_test, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_download(self, unwrap):
         filename = f'{self.test_id}.go'
@@ -122,37 +123,80 @@
             unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
 
 
 @pytest.mark.order(3)
 class TestThreat:
 
     def setup_class(self):
+        self.build = BuildController(pytest.account)
         self.detect = DetectController(pytest.account)
 
-        self.threat_id = '09d1a6b6-64d0-4473-af02-9a72b386cc79'
-
-    def test_get_threat(self, unwrap):
-        res = unwrap(self.detect.get_threat)(self.detect, threat_id=self.threat_id)
+        self.threat_id = str(uuid.uuid4())
+        self.name = 'threat'
+        self.published = '2023-11-13'
+        self.source_id = 'aa23-061a'
+        self.source = 'https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-061a'
+        self.tests = ['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54', pytest.test_id]
+
+    def test_create_threat(self, unwrap, email):
+        res = unwrap(self.build.create_threat)(self.build, name=self.name, published=self.published,
+                                               threat_id=self.threat_id, source_id=self.source_id, source=self.source,
+                                               tests=','.join(self.tests))
 
         pytest.threat_id = self.threat_id
         pytest.expected_threat = dict(
-            account_id='prelude',
+            account_id=pytest.account.headers['account'],
+            author=email,
             id=self.threat_id,
-            source_id='aa23-061a',
-            name='#StopRansomware: Royal Ransomware',
-            source='https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-061a',
-            published='2023-11-13',
-            tests=['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54'],
+            source_id=self.source_id,
+            name=self.name,
+            source=self.source,
+            published=self.published,
+            tests=self.tests,
             tombstoned=None
         )
 
         diffs = check_dict_items(pytest.expected_threat, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
+    def test_get_threat(self, unwrap):
+        res = unwrap(self.detect.get_threat)(self.detect, threat_id=self.threat_id)
+
+        diffs = check_dict_items(pytest.expected_threat, res)
+        assert not diffs, json.dumps(diffs, indent=2)
+
     def test_list_threats(self, unwrap):
         res = unwrap(self.detect.list_threats)(self.detect)
         owners = set([r['account_id'] for r in res])
-        assert owners == {'prelude'}
+        assert owners == {'prelude', pytest.account.headers['account']}
 
-        threat = [r for r in res if r['id'] == pytest.threat_id][0]
-        diffs = check_dict_items(pytest.expected_threat, threat)
+        mine = [r for r in res if r['account_id'] == pytest.account.headers['account']]
+        assert 1 == len(mine)
+        diffs = check_dict_items(pytest.expected_threat, mine[0])
         assert not diffs, json.dumps(diffs, indent=2)
+
+    def test_update_threat(self, unwrap):
+        updated_name = 'updated-threat'
+        updated_tests = ['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54']
+        res = unwrap(self.build.update_threat)(self.build, threat_id=self.threat_id, name=updated_name, source='',
+                                               tests=','.join(updated_tests))
+
+        pytest.expected_threat['name'] = updated_name
+        pytest.expected_threat['source'] = None
+        pytest.expected_threat['tests'] = updated_tests
+
+        diffs = check_dict_items(pytest.expected_threat, res)
+        assert not diffs, json.dumps(diffs, indent=2)
+
+    @pytest.mark.order(-3)
+    def test_delete_threat(self, unwrap):
+        unwrap(self.build.delete_threat)(self.build, threat_id=pytest.threat_id, purge=False)
+        res = unwrap(self.detect.get_threat)(self.detect, threat_id=pytest.threat_id)
+        pytest.expected_threat['tombstoned'] = res['tombstoned']
+
+        diffs = check_dict_items(pytest.expected_threat, res)
+        assert not diffs, json.dumps(diffs, indent=2)
+        assert parse(res['tombstoned']) <= datetime.utcnow() + timedelta(minutes=1)
+
+        unwrap(self.build.delete_threat)(self.build, threat_id=pytest.threat_id, purge=True)
+        with pytest.raises(Exception):
+            unwrap(self.detect.get_threat)(self.detect, threat_id=pytest.threat_id)
```

### Comparing `prelude-sdk-1.7.0/tests/test_detect.py` & `prelude-sdk-1.7.1/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/tests/test_iam.py` & `prelude-sdk-1.7.1/tests/test_iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,19 @@
                 dict(
                     run_code=RunCode.SMART.value,
                     tag='autopilot'
                 )
             ],
             probe_sleep='600s',
             oidc=dict(),
-            oidc_enabled=False
+            features=dict(
+                oidc=False,
+                threat_intel=False,
+                detections=False
+            )
         )
 
     def test_account_subscribe(self, unwrap, manual, email):
         if not manual:
             pytest.skip("Not manual mode")
 
         res = unwrap(self.iam.subscribe)(self.iam, event=AuditEvent.CREATE_USER)
```

### Comparing `prelude-sdk-1.7.0/tests/test_partner.py` & `prelude-sdk-1.7.1/tests/test_partner.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/tests/test_probe.py` & `prelude-sdk-1.7.1/tests/test_probe.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.0/tests/testutils.py` & `prelude-sdk-1.7.1/tests/testutils.py`

 * *Files identical despite different names*

