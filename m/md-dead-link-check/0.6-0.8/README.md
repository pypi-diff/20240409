# Comparing `tmp/md_dead_link_check-0.6.tar.gz` & `tmp/md_dead_link_check-0.8.tar.gz`

## Comparing `md_dead_link_check-0.6.tar` & `md_dead_link_check-0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/md_dead_link_check/__main__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/md_dead_link_check/config.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/md_dead_link_check/helpers.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/md_dead_link_check/link_checker.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/md_dead_link_check/preprocess.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/LICENSE
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/README.md
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/pyproject.toml
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 md_dead_link_check-0.6/PKG-INFO
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/md_dead_link_check/__main__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/md_dead_link_check/config.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/md_dead_link_check/helpers.py
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/md_dead_link_check/link_checker.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/md_dead_link_check/preprocess.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/LICENSE
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/README.md
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/pyproject.toml
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 md_dead_link_check-0.8/PKG-INFO
```

### Comparing `md_dead_link_check-0.6/md_dead_link_check/__main__.py` & `md_dead_link_check-0.8/md_dead_link_check/__main__.py`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/md_dead_link_check/config.py` & `md_dead_link_check-0.8/md_dead_link_check/config.py`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/md_dead_link_check/helpers.py` & `md_dead_link_check-0.8/md_dead_link_check/helpers.py`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/md_dead_link_check/link_checker.py` & `md_dead_link_check-0.8/md_dead_link_check/link_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
             "timeout": config.timeout,
             "ssl": config.validate_ssl,
         }
         if any(fnmatch(link, p) for p in config.force_get_requests_for_links):
             response = await session.get(**kwargs)
         else:
             response = await session.head(**kwargs)
-
+            if response.status == 404:
+                # Some web sites are not supports head request and return 404 code
+                response = await session.get(**kwargs)
         response.raise_for_status()
     except ClientResponseError as e:
         if not config.catch_response_codes or e.status in config.catch_response_codes:
             return LinkStatus(link, f"{e.status}: {e.message}")
         return LinkStatus(link, warn_msg=f"{e.status}: {e.message}")
     except asyncio.CancelledError as e:
         return LinkStatus(link, str(e))
```

### Comparing `md_dead_link_check-0.6/md_dead_link_check/preprocess.py` & `md_dead_link_check-0.8/md_dead_link_check/preprocess.py`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/.gitignore` & `md_dead_link_check-0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/LICENSE` & `md_dead_link_check-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `md_dead_link_check-0.6/README.md` & `md_dead_link_check-0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.3
+Name: md_dead_link_check
+Version: 0.8
+Summary: This is a lightweight and fast tool to help you keep your Markdown files free of broken links.
+Project-URL: Repository, https://github.com/AlexanderDokuchaev/md-dead-link-check
+Project-URL: Issues, https://github.com/AlexanderDokuchaev/md-dead-link-check/issues
+License: MIT
+License-File: LICENSE
+Keywords: broken link,broken link checker,dead link,dead link checker,documentation maintenance,link checker,link health,markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: aiohttp<3.10.0,>=3.8.0
+Requires-Dist: gitpython<3.2.0,>=3.1.0
+Requires-Dist: toml<3.11.0,>=0.7.0
+Provides-Extra: dev
+Requires-Dist: pre-commit==3.2.2; extra == 'dev'
+Requires-Dist: pytest==7.4.3; extra == 'dev'
+Provides-Extra: lint
+Requires-Dist: black==24.2.0; extra == 'lint'
+Requires-Dist: isort==5.13.2; extra == 'lint'
+Description-Content-Type: text/markdown
+
 # Markdown Dead Link Checker
 
 [![GitHub Action](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/github_action.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/github_action.yml?query=branch%3Amain)
 [![Ubuntu](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/ubuntu.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/ubuntu.yml?query=branch%3Amain)
 [![Windows](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/win.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/win.yml?query=branch%3Amain)
 [![MacOS](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/mac.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/mac.yml?query=branch%3Amain)
 
@@ -39,28 +69,66 @@
 
 ```yaml
 jobs:
   md-dead-link-check:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
-      - uses: AlexanderDokuchaev/md-dead-link-check@v0.6
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
 ```
 
 ### Option 2: Pre-Commit
 
 Adding to your `.pre-commit-config.yaml` to integrate in [pre-commit](https://pre-commit.com/) tool
 
 ```yaml
   - repo: https://github.com/AlexanderDokuchaev/md-dead-link-check
     rev: "v0.6"
     hooks:
       - id: md-dead-link-check
 ```
 
+> [!NOTE]
+> For the `pull_request` event type, the action will only check external links for files that have been modified.
+> To scan all links, consider using a separate action that runs periodically on target branches.
+> This approach helps prevent pull request merges from being blocked by broken links unrelated to the files
+> modified in the pull request.
+
+```yaml
+# .github/workflows/nightly.yaml
+name: nightly
+on:
+  workflow_dispatch:
+  schedule:
+    - cron: '0 0 * * *'
+jobs:
+  md-dead-link-check:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v4
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
+```
+
+```yaml
+# .github/workflows/pull_request.yaml
+name: pull_request
+on:
+  pull_request:
+    types:
+      - opened
+      - reopened
+      - synchronize
+jobs:
+  md-dead-link-check:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v4
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
+```
+
 ### Option 3: Install from pip
 
 For direct use, install with pip and run:
 
 ```bash
 pip install md-dead-link-check
 md-dead-link-check
```

### Comparing `md_dead_link_check-0.6/pyproject.toml` & `md_dead_link_check-0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "md_dead_link_check"
 description = "This is a lightweight and fast tool to help you keep your Markdown files free of broken links."
 readme = "README.md"
-version = "0.6"
+version = "0.8"
 license = {text = "MIT"}
 requires-python = ">=3.8"
 dependencies = [
   "toml>=0.7.0,<3.11.0",
   "GitPython>=3.1.0,<3.2.0",
   "aiohttp>=3.8.0,<3.10.0"
 ]
```

### Comparing `md_dead_link_check-0.6/PKG-INFO` & `md_dead_link_check-0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.3
-Name: md_dead_link_check
-Version: 0.6
-Summary: This is a lightweight and fast tool to help you keep your Markdown files free of broken links.
-Project-URL: Repository, https://github.com/AlexanderDokuchaev/md-dead-link-check
-Project-URL: Issues, https://github.com/AlexanderDokuchaev/md-dead-link-check/issues
-License: MIT
-License-File: LICENSE
-Keywords: broken link,broken link checker,dead link,dead link checker,documentation maintenance,link checker,link health,markdown
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Requires-Dist: aiohttp<3.10.0,>=3.8.0
-Requires-Dist: gitpython<3.2.0,>=3.1.0
-Requires-Dist: toml<3.11.0,>=0.7.0
-Provides-Extra: dev
-Requires-Dist: pre-commit==3.2.2; extra == 'dev'
-Requires-Dist: pytest==7.4.3; extra == 'dev'
-Provides-Extra: lint
-Requires-Dist: black==24.2.0; extra == 'lint'
-Requires-Dist: isort==5.13.2; extra == 'lint'
-Description-Content-Type: text/markdown
-
 # Markdown Dead Link Checker
 
 [![GitHub Action](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/github_action.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/github_action.yml?query=branch%3Amain)
 [![Ubuntu](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/ubuntu.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/ubuntu.yml?query=branch%3Amain)
 [![Windows](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/win.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/win.yml?query=branch%3Amain)
 [![MacOS](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/mac.yml/badge.svg?branch=main)](https://github.com/AlexanderDokuchaev/md-dead-link-check/actions/workflows/mac.yml?query=branch%3Amain)
 
@@ -69,28 +39,66 @@
 
 ```yaml
 jobs:
   md-dead-link-check:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v4
-      - uses: AlexanderDokuchaev/md-dead-link-check@v0.6
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
 ```
 
 ### Option 2: Pre-Commit
 
 Adding to your `.pre-commit-config.yaml` to integrate in [pre-commit](https://pre-commit.com/) tool
 
 ```yaml
   - repo: https://github.com/AlexanderDokuchaev/md-dead-link-check
     rev: "v0.6"
     hooks:
       - id: md-dead-link-check
 ```
 
+> [!NOTE]
+> For the `pull_request` event type, the action will only check external links for files that have been modified.
+> To scan all links, consider using a separate action that runs periodically on target branches.
+> This approach helps prevent pull request merges from being blocked by broken links unrelated to the files
+> modified in the pull request.
+
+```yaml
+# .github/workflows/nightly.yaml
+name: nightly
+on:
+  workflow_dispatch:
+  schedule:
+    - cron: '0 0 * * *'
+jobs:
+  md-dead-link-check:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v4
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
+```
+
+```yaml
+# .github/workflows/pull_request.yaml
+name: pull_request
+on:
+  pull_request:
+    types:
+      - opened
+      - reopened
+      - synchronize
+jobs:
+  md-dead-link-check:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v4
+      - uses: AlexanderDokuchaev/md-dead-link-check@v0.8
+```
+
 ### Option 3: Install from pip
 
 For direct use, install with pip and run:
 
 ```bash
 pip install md-dead-link-check
 md-dead-link-check
```

