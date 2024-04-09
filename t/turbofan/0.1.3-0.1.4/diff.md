# Comparing `tmp/turbofan-0.1.3.tar.gz` & `tmp/turbofan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbofan-0.1.3.tar", max compression
+gzip compressed data, was "turbofan-0.1.4.tar", max compression
```

## Comparing `turbofan-0.1.3.tar` & `turbofan-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1211 2024-03-30 19:58:06.156642 turbofan-0.1.3/LICENSE
--rw-r--r--   0        0        0      182 2024-03-30 19:58:06.157065 turbofan-0.1.3/README.md
--rw-r--r--   0        0        0     1146 2024-03-30 20:11:57.091684 turbofan-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       24 2024-03-30 19:58:06.160060 turbofan-0.1.3/src/turbofan/__init__.py
--rw-r--r--   0        0        0     1022 2024-03-30 19:58:06.160278 turbofan-0.1.3/src/turbofan/command.py
--rw-r--r--   0        0        0     2847 2024-03-30 19:58:06.160598 turbofan-0.1.3/src/turbofan/database.py
--rw-r--r--   0        0        0      306 2024-03-30 19:58:06.161069 turbofan-0.1.3/src/turbofan/files.py
--rw-r--r--   0        0        0      715 2024-03-30 19:58:06.161288 turbofan-0.1.3/src/turbofan/fixtures.py
--rw-r--r--   0        0        0      809 2024-03-30 19:58:06.161679 turbofan-0.1.3/src/turbofan/project.py
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 turbofan-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-03-30 19:58:06.156642 turbofan-0.1.4/LICENSE
+-rw-r--r--   0        0        0      182 2024-03-30 19:58:06.157065 turbofan-0.1.4/README.md
+-rw-r--r--   0        0        0     1146 2024-04-09 10:47:23.346876 turbofan-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-03-30 19:58:06.160060 turbofan-0.1.4/src/turbofan/__init__.py
+-rw-r--r--   0        0        0     1022 2024-03-30 19:58:06.160278 turbofan-0.1.4/src/turbofan/command.py
+-rw-r--r--   0        0        0     2847 2024-03-30 19:58:06.160598 turbofan-0.1.4/src/turbofan/database.py
+-rw-r--r--   0        0        0      306 2024-03-30 19:58:06.161069 turbofan-0.1.4/src/turbofan/files.py
+-rw-r--r--   0        0        0      727 2024-03-30 20:55:50.159301 turbofan-0.1.4/src/turbofan/fixtures.py
+-rw-r--r--   0        0        0      809 2024-03-30 19:58:06.161679 turbofan-0.1.4/src/turbofan/project.py
+-rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 turbofan-0.1.4/PKG-INFO
```

### Comparing `turbofan-0.1.3/LICENSE` & `turbofan-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `turbofan-0.1.3/pyproject.toml` & `turbofan-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.mypy]
 ignore_missing_imports = true
 # https://stackoverflow.com/questions/62265366/does-mypy-only-type-check-a-function-if-it-declares-a-return-type
 check_untyped_defs = true
 
 [tool.poetry]
 name = "turbofan"
-version = "0.1.3"
+version = "0.1.4"
 description = "Essential Libraries and Tools for Streamlined Development"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicence"
 readme = "README.md"
 packages = [
     { include = "turbofan", from = "src" },
 ]
```

### Comparing `turbofan-0.1.3/src/turbofan/command.py` & `turbofan-0.1.4/src/turbofan/command.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.1.3/src/turbofan/database.py` & `turbofan-0.1.4/src/turbofan/database.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.1.3/src/turbofan/fixtures.py` & `turbofan-0.1.4/src/turbofan/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from turbofan.database import Database, Session
 
 
 @pytest.fixture
 def tmp_db_session(tmp_path: Path, monkeypatch):
     """
-    Creates a database in the path defined by tmpdir and loads all sql files
-    from the migrations folder in the project root.
+    Creates a database in the path defined by tmp_path and loads all sql files
+    from the migrations folder in the project root directory.
     """
 
     # Since Database defines that the environment variable has priority over
     # all other definitions, we set it here, so during the tests, all the
     # database instances use this value for the path.
     monkeypatch.setenv("DATABASE", str(tmp_path))
```

### Comparing `turbofan-0.1.3/src/turbofan/project.py` & `turbofan-0.1.4/src/turbofan/project.py`

 * *Files identical despite different names*

### Comparing `turbofan-0.1.3/PKG-INFO` & `turbofan-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbofan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Essential Libraries and Tools for Streamlined Development
 License: The Unlicence
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

