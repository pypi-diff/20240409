# Comparing `tmp/semvergit-0.2.1.tar.gz` & `tmp/semvergit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semvergit-0.2.1.tar", last modified: Fri Mar 29 13:12:28 2024, max compression
+gzip compressed data, was "semvergit-0.3.0.tar", last modified: Tue Apr  9 17:48:52 2024, max compression
```

## Comparing `semvergit-0.2.1.tar` & `semvergit-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:12:28.013846 semvergit-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-29 13:12:09.000000 semvergit-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-29 13:12:28.013846 semvergit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-29 13:12:09.000000 semvergit-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-29 13:12:09.000000 semvergit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-29 13:12:09.000000 semvergit-0.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-29 13:12:09.000000 semvergit-0.2.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-29 13:12:09.000000 semvergit-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:12:28.013846 semvergit-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:12:28.005846 semvergit-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:12:28.005846 semvergit-0.2.1/src/semvergit/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-29 13:12:09.000000 semvergit-0.2.1/src/semvergit/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:12:28.009846 semvergit-0.2.1/src/semvergit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-29 13:12:27.000000 semvergit-0.2.1/src/semvergit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-29 13:12:28.000000 semvergit-0.2.1/src/semvergit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:12:27.000000 semvergit-0.2.1/src/semvergit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 13:12:27.000000 semvergit-0.2.1/src/semvergit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-29 13:12:27.000000 semvergit-0.2.1/src/semvergit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 13:12:27.000000 semvergit-0.2.1/src/semvergit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:12:28.009846 semvergit-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-29 13:12:09.000000 semvergit-0.2.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-29 13:12:09.000000 semvergit-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-03-29 13:12:09.000000 semvergit-0.2.1/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-29 13:12:09.000000 semvergit-0.2.1/tests/test_log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.974448 semvergit-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 17:48:30.000000 semvergit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 17:48:52.974448 semvergit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-09 17:48:30.000000 semvergit-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-09 17:48:30.000000 semvergit-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.966448 semvergit-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 17:48:30.000000 semvergit-0.3.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 17:48:30.000000 semvergit-0.3.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:48:52.974448 semvergit-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.966448 semvergit-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/src/semvergit/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-09 17:48:30.000000 semvergit-0.3.0/src/semvergit/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/src/semvergit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 17:48:52.000000 semvergit-0.3.0/src/semvergit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:48:52.970448 semvergit-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 17:48:30.000000 semvergit-0.3.0/tests/test_log_utils.py
```

### Comparing `semvergit-0.2.1/LICENSE` & `semvergit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semvergit-0.2.1/PKG-INFO` & `semvergit-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.2.1
+Version: 0.3.0
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click==8.1.7
-Requires-Dist: gitdb==4.0.11
-Requires-Dist: gitpython==3.1.40
-Requires-Dist: loguru==0.7.2
-Requires-Dist: semver==3.0.2
-Requires-Dist: smmap==5.0.1
+Requires-Dist: gitpython>=3.0.0
+Requires-Dist: semver>=3.0.0
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: click>=8.0.0
 Provides-Extra: dev
 Requires-Dist: astroid==3.1.0; extra == "dev"
 Requires-Dist: bandit==1.7.8; extra == "dev"
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: dill==0.3.8; extra == "dev"
@@ -69,18 +67,15 @@
 |-|-|
 | CI/CD   | [![Pytest](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml) [![Publish](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml) [![Coverage Status](https://coveralls.io/repos/github/Tranquility2/semvergit/badge.svg)](https://coveralls.io/github/Tranquility2/semvergit)|
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/semvergit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/semvergit/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/semvergit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/semvergit/)|
 | Meta    | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
 |||
 
 # semvergit
-
-Manage your project's version numbers.
-
-## Semantic Versioning
+![semvergit](assets/semvergit-255.png)
 
 semvergit is a CLI tool to manage your project's version numbers.
 It uses [Semantic Versioning](https://semver.org/) to bump the version number.
 The supported bump types are:
 
 - `major`
 - `minor`
```

### Comparing `semvergit-0.2.1/README.md` & `semvergit-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 |-|-|
 | CI/CD   | [![Pytest](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml) [![Publish](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml) [![Coverage Status](https://coveralls.io/repos/github/Tranquility2/semvergit/badge.svg)](https://coveralls.io/github/Tranquility2/semvergit)|
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/semvergit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/semvergit/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/semvergit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/semvergit/)|
 | Meta    | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
 |||
 
 # semvergit
-
-Manage your project's version numbers.
-
-## Semantic Versioning
+![semvergit](assets/semvergit-255.png)
 
 semvergit is a CLI tool to manage your project's version numbers.
 It uses [Semantic Versioning](https://semver.org/) to bump the version number.
 The supported bump types are:
 
 - `major`
 - `minor`
```

### Comparing `semvergit-0.2.1/pyproject.toml` & `semvergit-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,37 +3,40 @@
 requires = ["setuptools", "versioningit", "wheel"]
 
 [project]
 name = "semvergit"
 description = "Manage your project's version numbers."
 readme = "README.md"
 license = { file = "LICENSE.md" }
-requires-python = ">=3.8"
 keywords = ["packaging", "publishing", "release", "versioning"]
 authors = [{ name = "Roy Moore", email = "roy@moore.co.il" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
+requires-python = ">=3.8"
+dependencies = [
+  "gitpython>=3.0.0",
+  "semver>=3.0.0",
+  "loguru>=0.7.0",
+  "click>=8.0.0",
+]
 
-dynamic = ["version", "dependencies", "optional-dependencies"]
-
-[tool.setuptools.dynamic.dependencies]
-file = ["requirements.txt"]
+dynamic = ["version", "optional-dependencies"]
 
 [tool.setuptools.dynamic.optional-dependencies]
-dev = { file = ["requirements-dev.txt"] }
-test = { file = ["requirements-test.txt"] }
+dev = { file = ["requirements/requirements-dev.txt"] }
+test = { file = ["requirements/requirements-test.txt"] }
 
 [project.scripts]
 semvergit = "semvergit.cli:cli"
 
 [project.urls]
 homepage = "https://github.com/Tranquility2/semvergit"
 repository = "https://github.com/Tranquility2/semvergit"
@@ -46,15 +49,14 @@
 [tool.versioningit.tag2version]
 rmprefix = "v"
 
 [tool.pip-tools]
 quiet = true
 rebuild = true
 strip-extras = true
-no-header = true
 annotation-style = "line"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 line_length = 120
```

### Comparing `semvergit-0.2.1/requirements-dev.txt` & `semvergit-0.3.0/requirements/requirements-dev.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+#
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
+#
+#    pip-compile --annotation-style=line --output-file=requirements/requirements-dev.txt --strip-extras requirements/requirements-dev.in
+#
 astroid==3.1.0            # via pylint
-bandit==1.7.8             # via -r requirements-dev.in
-black==24.3.0             # via -r requirements-dev.in
+bandit==1.7.8             # via -r requirements/requirements-dev.in
+black==24.3.0             # via -r requirements/requirements-dev.in
 cfgv==3.4.0               # via pre-commit
-click==8.1.7              # via -c requirements.txt, black
+click==8.1.7              # via -c requirements/requirements.txt, black
 dill==0.3.8               # via pylint
 distlib==0.3.8            # via virtualenv
 filelock==3.13.3          # via virtualenv
 identify==2.5.35          # via pre-commit
-isort==5.13.2             # via -r requirements-dev.in, pylint
+isort==5.13.2             # via -r requirements/requirements-dev.in, pylint
 markdown-it-py==3.0.0     # via rich
 mccabe==0.7.0             # via pylint
 mdurl==0.1.2              # via markdown-it-py
-mypy==1.9.0               # via -r requirements-dev.in
+mypy==1.9.0               # via -r requirements/requirements-dev.in
 mypy-extensions==1.0.0    # via black, mypy
 nodeenv==1.8.0            # via pre-commit
 packaging==24.0           # via black
 pathspec==0.12.1          # via black
 pbr==6.0.0                # via stevedore
 platformdirs==4.2.0       # via black, pylint, virtualenv
-pre-commit==3.5.0         # via -r requirements-dev.in
+pre-commit==3.5.0         # via -r requirements/requirements-dev.in
 pygments==2.17.2          # via rich
-pylint==3.1.0             # via -r requirements-dev.in
+pylint==3.1.0             # via -r requirements/requirements-dev.in
 pyyaml==6.0.1             # via bandit, pre-commit
 rich==13.7.1              # via bandit
 stevedore==5.2.0          # via bandit
 tomli==2.0.1              # via bandit, black, mypy, pylint
 tomlkit==0.12.4           # via pylint
 typing-extensions==4.10.0  # via astroid, black, mypy, pylint, rich
 virtualenv==20.25.1       # via pre-commit
```

### Comparing `semvergit-0.2.1/src/semvergit/app.py` & `semvergit-0.3.0/src/semvergit/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,18 @@
         self.current_repo = get_repo()
         self.branch = get_active_branch(repo=self.current_repo)
         logger.debug(f"Active branch: {self.branch.name}")
         if pull_branch:
             logger.info("Pulling...")
             pull_remote(self.current_repo)
         self.versions = self.get_versions()
-        self.latest_version = max(self.versions)
+        if self.versions:
+            self.latest_version = max(self.versions)
+        else:
+            self.latest_version = VersionInfo.parse("0.0.0")
 
     def get_versions(self) -> List[VersionInfo]:
         """Get versions."""
         current_repo = get_repo()
         tags = get_tags_with_prefix(repo=current_repo, prefix=self.version_prefix)
         clean_tags = [self.remove_prefix(tag, self.version_prefix) for tag in tags]
         versions = [VersionInfo.parse(tag) for tag in clean_tags]
```

### Comparing `semvergit-0.2.1/src/semvergit/cli.py` & `semvergit-0.3.0/src/semvergit/cli.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.2.1/src/semvergit/git_utils.py` & `semvergit-0.3.0/src/semvergit/git_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.2.1/src/semvergit/log_utils.py` & `semvergit-0.3.0/src/semvergit/log_utils.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.2.1/src/semvergit.egg-info/PKG-INFO` & `semvergit-0.3.0/src/semvergit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semvergit
-Version: 0.2.1
+Version: 0.3.0
 Summary: Manage your project's version numbers.
 Author-email: Roy Moore <roy@moore.co.il>
 Project-URL: homepage, https://github.com/Tranquility2/semvergit
 Project-URL: repository, https://github.com/Tranquility2/semvergit
 Keywords: packaging,publishing,release,versioning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click==8.1.7
-Requires-Dist: gitdb==4.0.11
-Requires-Dist: gitpython==3.1.40
-Requires-Dist: loguru==0.7.2
-Requires-Dist: semver==3.0.2
-Requires-Dist: smmap==5.0.1
+Requires-Dist: gitpython>=3.0.0
+Requires-Dist: semver>=3.0.0
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: click>=8.0.0
 Provides-Extra: dev
 Requires-Dist: astroid==3.1.0; extra == "dev"
 Requires-Dist: bandit==1.7.8; extra == "dev"
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: dill==0.3.8; extra == "dev"
@@ -69,18 +67,15 @@
 |-|-|
 | CI/CD   | [![Pytest](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/pytest.yml) [![Publish](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml/badge.svg)](https://github.com/Tranquility2/semvergit/actions/workflows/publish.yml) [![Coverage Status](https://coveralls.io/repos/github/Tranquility2/semvergit/badge.svg)](https://coveralls.io/github/Tranquility2/semvergit)|
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/semvergit.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/semvergit/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/semvergit.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/semvergit/)|
 | Meta    | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) |
 |||
 
 # semvergit
-
-Manage your project's version numbers.
-
-## Semantic Versioning
+![semvergit](assets/semvergit-255.png)
 
 semvergit is a CLI tool to manage your project's version numbers.
 It uses [Semantic Versioning](https://semver.org/) to bump the version number.
 The supported bump types are:
 
 - `major`
 - `minor`
```

### Comparing `semvergit-0.2.1/src/semvergit.egg-info/requires.txt` & `semvergit-0.3.0/src/semvergit.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-click==8.1.7
-gitdb==4.0.11
-gitpython==3.1.40
-loguru==0.7.2
-semver==3.0.2
-smmap==5.0.1
+gitpython>=3.0.0
+semver>=3.0.0
+loguru>=0.7.0
+click>=8.0.0
 
 [dev]
 astroid==3.1.0
 bandit==1.7.8
 black==24.3.0
 cfgv==3.4.0
 click==8.1.7
```

### Comparing `semvergit-0.2.1/tests/test_cli.py` & `semvergit-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `semvergit-0.2.1/tests/test_git_utils.py` & `semvergit-0.3.0/tests/test_git_utils.py`

 * *Files identical despite different names*

