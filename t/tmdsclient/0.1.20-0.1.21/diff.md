# Comparing `tmp/tmdsclient-0.1.20.tar.gz` & `tmp/tmdsclient-0.1.21.tar.gz`

## Comparing `tmdsclient-0.1.20.tar` & `tmdsclient-0.1.21.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/README.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/domain-specific-terms.txt
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/requirements.txt
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/_tmdsclient_version.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/py.typed
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/__init__.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/config.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/client/tmdsclient.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/bo4e_stub.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/netzvertrag.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/src/tmdsclient/models/patches.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/pyproject.toml
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmdsclient-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/README.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/domain-specific-terms.txt
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/requirements.txt
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/_tmdsclient_version.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/py.typed
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/client/__init__.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/client/config.py
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/client/tmdsclient.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/models/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/models/bo4e_stub.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/models/netzvertrag.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/src/tmdsclient/models/patches.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/LICENSE
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 tmdsclient-0.1.21/PKG-INFO
```

### Comparing `tmdsclient-0.1.20/.pre-commit-config.yaml` & `tmdsclient-0.1.21/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/README.md` & `tmdsclient-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/requirements.txt` & `tmdsclient-0.1.21/requirements.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/tox.ini` & `tmdsclient-0.1.21/tox.ini`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/dependabot.yml` & `tmdsclient-0.1.21/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/codeql-analysis.yml` & `tmdsclient-0.1.21/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/coverage.yml` & `tmdsclient-0.1.21/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/dependabot_automerge.yml` & `tmdsclient-0.1.21/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/dev_test.yml` & `tmdsclient-0.1.21/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/formatting.yml` & `tmdsclient-0.1.21/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/packaging_test.yml` & `tmdsclient-0.1.21/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/python-publish.yml` & `tmdsclient-0.1.21/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/pythonlint.yml` & `tmdsclient-0.1.21/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.github/workflows/unittests.yml` & `tmdsclient-0.1.21/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/dev_requirements/requirements-linting.txt` & `tmdsclient-0.1.21/dev_requirements/requirements-linting.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/dev_requirements/requirements-packaging.txt` & `tmdsclient-0.1.21/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/dev_requirements/requirements-tests.txt` & `tmdsclient-0.1.21/dev_requirements/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/src/tmdsclient/client/config.py` & `tmdsclient-0.1.21/src/tmdsclient/client/config.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/src/tmdsclient/client/tmdsclient.py` & `tmdsclient-0.1.21/src/tmdsclient/client/tmdsclient.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/src/tmdsclient/models/bo4e_stub.py` & `tmdsclient-0.1.21/src/tmdsclient/models/bo4e_stub.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/src/tmdsclient/models/netzvertrag.py` & `tmdsclient-0.1.21/src/tmdsclient/models/netzvertrag.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 class Vertragsteil(BaseModel):
     """
     BO4E COM Vertragsteil
     """
 
+    guid: UUID | None = None
     vertragsteilbeginn: AwareDatetime
     vertragsteilende: AwareDatetime | None = None
     lokation: str
     jahresverbrauchsprognose: Menge | None = None
     kundenwert: Menge | None = None
```

### Comparing `tmdsclient-0.1.20/src/tmdsclient/models/patches.py` & `tmdsclient-0.1.21/src/tmdsclient/models/patches.py`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/.gitignore` & `tmdsclient-0.1.21/.gitignore`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/LICENSE` & `tmdsclient-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/pyproject.toml` & `tmdsclient-0.1.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tmdsclient-0.1.20/PKG-INFO` & `tmdsclient-0.1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tmdsclient
-Version: 0.1.20
+Version: 0.1.21
 Summary: Fully typed, async client library for Technical Master Data Service (TMDS)
 Project-URL: Changelog, https://github.com/Hochfrequenz/tmdsclient.py/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/tmdsclient.py
 Author-email: Hochfreuqenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: technical master data,tmds
```

