# Comparing `tmp/xls_updater-0.1.8.tar.gz` & `tmp/xls_updater-0.1.9.tar.gz`

## Comparing `xls_updater-0.1.8.tar` & `xls_updater-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.pylintrc
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 xls_updater-0.1.8/Makefile
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 xls_updater-0.1.8/requirements-dev.txt
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xls_updater-0.1.8/requirements-test.txt
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/actions/prepare-environment/action.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/black.yml
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/isort.yml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/mypy.yml
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.github/workflows/validation.yaml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_app.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_big.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_cli.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/test_samples.py
--rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample1.xls
--rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample2.xls
--rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.8/tests/samples/sample3.xls
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/__main__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/app.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.8/xls_updater/cli.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 xls_updater-0.1.8/.gitignore
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.8/README.md
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 xls_updater-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 xls_updater-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.pylintrc
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 xls_updater-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 xls_updater-0.1.9/Makefile
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 xls_updater-0.1.9/requirements-dev.txt
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 xls_updater-0.1.9/requirements-test.txt
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater.spec
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/actions/prepare-environment/action.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/black.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/isort.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/mypy.yml
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.github/workflows/validation.yaml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_app.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_big.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/test_samples.py
+-rw-r--r--   0        0        0    30208 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample1.xls
+-rw-r--r--   0        0        0    39424 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample2.xls
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 xls_updater-0.1.9/tests/samples/sample3.xls
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/__main__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/app.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 xls_updater-0.1.9/xls_updater/cli.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 xls_updater-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 xls_updater-0.1.9/README.md
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 xls_updater-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xls_updater-0.1.9/PKG-INFO
```

### Comparing `xls_updater-0.1.8/.pre-commit-config.yaml` & `xls_updater-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/.pylintrc` & `xls_updater-0.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/CONTRIBUTING.md` & `xls_updater-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/Makefile` & `xls_updater-0.1.9/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,14 @@
 
 run:
 	python3 xls_updater/app.py
 
 setup:
 	python3 -m pip install '.[dev, test, release]'
 
-setup-dev:
-	python3 -m pip install --editable '.[dev]'
-
-setup-test:
-	python3 -m pip install --editable '.[test]'
-
-setup-relase:
-	python3 -m pip install --editable '.[release]'
-
 pip-clean:
 	python3 -m pip uninstall -y -r <(pip freeze)
 
 clean:
 	rm -rf **/__pycache__ .pytest_cache/ dist/ .mypy_cache/ .coverage *.egg-info build
 
 check-black:
```

### Comparing `xls_updater-0.1.8/requirements-dev.txt` & `xls_updater-0.1.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/requirements-test.txt` & `xls_updater-0.1.9/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/.github/workflows/coverage.yml` & `xls_updater-0.1.9/.github/workflows/coverage.yml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     branches: master
   pull_request:
     branches: master
   workflow_dispatch:
 
 
 jobs:
-  build:
+  coverage:
     name: Coverage Validation
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
     - name: Install dependencies
       run: |
```

### Comparing `xls_updater-0.1.8/.github/workflows/pytest.yml` & `xls_updater-0.1.9/.github/workflows/pytest.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Pytest
 on: [ pull_request, workflow_dispatch ]
 
 jobs:
-  build:
+  pytest:
     name: Pytest Validation
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v4
```

### Comparing `xls_updater-0.1.8/.github/workflows/validation.yaml` & `xls_updater-0.1.9/.github/workflows/validation.yaml`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/test_app.py` & `xls_updater-0.1.9/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/test_big.py` & `xls_updater-0.1.9/tests/test_big.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/test_cli.py` & `xls_updater-0.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/test_samples.py` & `xls_updater-0.1.9/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/samples/sample1.xls` & `xls_updater-0.1.9/tests/samples/sample1.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/samples/sample2.xls` & `xls_updater-0.1.9/tests/samples/sample2.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/tests/samples/sample3.xls` & `xls_updater-0.1.9/tests/samples/sample3.xls`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/xls_updater/app.py` & `xls_updater-0.1.9/xls_updater/app.py`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/.gitignore` & `xls_updater-0.1.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 *.egg
 MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
-*.spec
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
```

### Comparing `xls_updater-0.1.8/README.md` & `xls_updater-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xls_updater-0.1.8/pyproject.toml` & `xls_updater-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     "pytest_mock",
 ]
 release = [
     "semvergit",
     "build",
     "twine",
 ]
+bin = [
+    "pyinstaller",
+]
 
 [project.scripts]
 xls-updater = "xls_updater.cli:cli"
 
 [project.urls]
 homepage = "https://github.com/Tranquility2/xls_updater"
 repository = "https://github.com/Tranquility2/xls_updater"
```

### Comparing `xls_updater-0.1.8/PKG-INFO` & `xls_updater-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xls-updater
-Version: 0.1.8
+Version: 0.1.9
 Summary: Convert legacy xls data to newer xlsx format.
 Project-URL: homepage, https://github.com/Tranquility2/xls_updater
 Project-URL: repository, https://github.com/Tranquility2/xls_updater
 Author-email: Roy Moore <roy@moore.co.il>
 Keywords: converter,excel,fileformat,spreadsheet,xls,xlsx
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,16 @@
 Classifier: Topic :: File Formats
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Requires-Python: >=3.10
 Requires-Dist: click==8.1.7
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: xlrd==2.0.1
+Provides-Extra: bin
+Requires-Dist: pyinstaller; extra == 'bin'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Provides-Extra: release
```

