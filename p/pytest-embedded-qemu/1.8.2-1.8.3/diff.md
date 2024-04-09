# Comparing `tmp/pytest_embedded_qemu-1.8.2.tar.gz` & `tmp/pytest_embedded_qemu-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_qemu-1.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_qemu-1.8.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_qemu-1.8.2.tar` & `pytest_embedded_qemu-1.8.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/LICENSE
--rw-r--r--   0        0        0      552 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/README.md
--rw-r--r--   0        0        0     3369 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      369 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/__init__.py
--rw-r--r--   0        0        0     6452 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/app.py
--rw-r--r--   0        0        0      473 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/dut.py
--rw-r--r--   0        0        0     4113 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/qemu.py
--rw-r--r--   0        0        0     4481 2024-04-02 08:52:22.108840 pytest_embedded_qemu-1.8.2/tests/test_qemu.py
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pytest_embedded_qemu-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/LICENSE
+-rw-r--r--   0        0        0      552 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/README.md
+-rw-r--r--   0        0        0     3369 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      369 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0        0        0     6452 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/app.py
+-rw-r--r--   0        0        0      473 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/dut.py
+-rw-r--r--   0        0        0     4113 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/qemu.py
+-rw-r--r--   0        0        0     4481 2024-04-09 09:44:39.840723 pytest_embedded_qemu-1.8.3/tests/test_qemu.py
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pytest_embedded_qemu-1.8.3/PKG-INFO
```

### Comparing `pytest_embedded_qemu-1.8.2/LICENSE` & `pytest_embedded_qemu-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.2/README.md` & `pytest_embedded_qemu-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.2/pyproject.toml` & `pytest_embedded_qemu-1.8.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.8.2",
+    "pytest-embedded~=1.8.3",
     "qemu.qmp==0.0.3"
 ]
 
 [project.optional-dependencies]
 idf = [
-    "pytest-embedded-idf~=1.8.2",
+    "pytest-embedded-idf~=1.8.3",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
```

### Comparing `pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/app.py` & `pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.2/pytest_embedded_qemu/qemu.py` & `pytest_embedded_qemu-1.8.3/pytest_embedded_qemu/qemu.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.2/tests/test_qemu.py` & `pytest_embedded_qemu-1.8.3/tests/test_qemu.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_qemu-1.8.2/PKG-INFO` & `pytest_embedded_qemu-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.8.2
+Version: 1.8.3
 Summary: Make pytest-embedded plugin work with QEMU.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.8.2
+Requires-Dist: pytest-embedded~=1.8.3
 Requires-Dist: qemu.qmp==0.0.3
-Requires-Dist: pytest-embedded-idf~=1.8.2 ; extra == "idf"
+Requires-Dist: pytest-embedded-idf~=1.8.3 ; extra == "idf"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-qemu
```

