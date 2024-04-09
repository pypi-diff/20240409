# Comparing `tmp/pipekit_sdk-0.0.4.tar.gz` & `tmp/pipekit_sdk-1.0.0.tar.gz`

## Comparing `pipekit_sdk-0.0.4.tar` & `pipekit_sdk-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/bandit.yaml
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/examples/coinflip.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/src/pipekit_sdk/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/src/pipekit_sdk/helpers.py
--rw-r--r--   0        0        0    12879 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/src/pipekit_sdk/service.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/bandit.yaml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/examples/coinflip.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/src/pipekit_sdk/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/src/pipekit_sdk/helpers.py
+-rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/src/pipekit_sdk/service.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pipekit_sdk-1.0.0/PKG-INFO
```

### Comparing `pipekit_sdk-0.0.4/bandit.yaml` & `pipekit_sdk-1.0.0/bandit.yaml`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.4/examples/coinflip.ipynb` & `pipekit_sdk-1.0.0/examples/coinflip.ipynb`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.4/src/pipekit_sdk/helpers.py` & `pipekit_sdk-1.0.0/src/pipekit_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.4/src/pipekit_sdk/service.py` & `pipekit_sdk-1.0.0/src/pipekit_sdk/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class PipekitService:
     """
     PipekitService is a wrapper around the Pipekit API.
     It provides a simple interface to interact with Pipekit.
     """
 
     def __init__(
-        self, username="", password="", token="", pipekit_url="https://pipekit.io"
+        self, username="", password="", token="", pipekit_url="https://api.pipekit.io"
     ):
         self.username = username
         self.password = password
 
         pipekit_url = os.getenv("PIPEKIT_URL", pipekit_url)
         if pipekit_url.endswith("/"):
             pipekit_url = pipekit_url[:-1]
```

### Comparing `pipekit_sdk-0.0.4/.gitignore` & `pipekit_sdk-1.0.0/.gitignore`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+*~
 /services/github/infra/burner.env
 /services/ui/dist
 /vendor
-**/node_modules
+node_modules
 services/ui/yarn-error.log
-**/**/.DS_Store
+.DS_Store
 .idea/
 infra/kubeconfig
 dist/
-**/**/.obsidian
+.obsidian
 .npmrc
 .yarnrc*
 .vscode
+.vite
 **/test-results/
 **/playwright-report/
 **/playwright/.cache/
 /services/ui/tests/.auth
 /services/pipekit-agent/helm/charts
 /services/pipekit-agent/helm/Chart.lock
 /services/pipekit-agent/helm/README.md
 /docs/megalinter-reports
 python_sdk/**/__pycache__
 /services/**/coverage.html
 /services/**/coverage.out
 /megalinter-reports
 *megalinter_*.txt
+/.cluster*
+!services/ui/third-party/**
```

### Comparing `pipekit_sdk-0.0.4/LICENSE` & `pipekit_sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.4/README.md` & `pipekit_sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.4/PKG-INFO` & `pipekit_sdk-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pipekit-sdk
-Version: 0.0.4
+Version: 1.0.0
 Summary: Pipekit Python SDK
 Author-email: Pipekit <ci@pipekit.io>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: hera>=5.5.2
```

