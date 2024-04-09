# Comparing `tmp/buildenv-1.5.0.tar.gz` & `tmp/buildenv-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildenv-1.5.0.tar", last modified: Sun Mar  3 16:13:15 2024, max compression
+gzip compressed data, was "buildenv-1.5.1.tar", last modified: Tue Apr  9 13:03:54 2024, max compression
```

## Comparing `buildenv-1.5.0.tar` & `buildenv-1.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.543913 buildenv-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-03 16:12:44.000000 buildenv-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-03 16:13:15.543913 buildenv-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-03 16:13:12.000000 buildenv-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-03 16:13:15.543913 buildenv-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-03 16:13:12.000000 buildenv-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.535913 buildenv-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.539913 buildenv-1.5.0/src/buildenv/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.539913 buildenv-1.5.0/src/buildenv/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/_internal/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.543913 buildenv-1.5.0/src/buildenv/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/activate.cmd.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/activate.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/buildenv.cmd.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/buildenv.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/command.cmd.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/command.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/completion.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/gitattributes.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/gitignore.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/shell.cmd.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/shell.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/venv_prompt.sh.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-03 16:12:44.000000 buildenv-1.5.0/src/buildenv/templates/warning.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 16:13:15.543913 buildenv-1.5.0/src/buildenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-03 16:13:15.000000 buildenv-1.5.0/src/buildenv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.909592 buildenv-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 13:03:24.000000 buildenv-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 13:03:54.909592 buildenv-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 13:03:51.000000 buildenv-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 13:03:54.909592 buildenv-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 13:03:51.000000 buildenv-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.905591 buildenv-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.905591 buildenv-1.5.1/src/buildenv/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.905591 buildenv-1.5.1/src/buildenv/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/_internal/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.909592 buildenv-1.5.1/src/buildenv/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/activate.cmd.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/activate.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/buildenv.cmd.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/buildenv.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/command.cmd.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/command.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/completion.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/gitattributes.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/gitignore.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/shell.cmd.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/shell.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/venv_prompt.sh.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 13:03:24.000000 buildenv-1.5.1/src/buildenv/templates/warning.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:03:54.909592 buildenv-1.5.1/src/buildenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 13:03:54.000000 buildenv-1.5.1/src/buildenv.egg-info/top_level.txt
```

### Comparing `buildenv-1.5.0/LICENSE` & `buildenv-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/PKG-INFO` & `buildenv-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildenv
-Version: 1.5.0
+Version: 1.5.1
 Summary: Build environment setup system, based on Python venv
 Home-page: https://github.com/dynod/buildenv
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `buildenv-1.5.0/README.md` & `buildenv-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/setup.cfg` & `buildenv-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 exclude = 
 	__pycache__
 
 [metadata]
 name = buildenv
 author = The dynod project
 maintainer = The dynod project
-version = 1.5.0
+version = 1.5.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Mozilla Public License Version 2.0
 classifiers = 
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `buildenv-1.5.0/src/buildenv/__init__.py` & `buildenv-1.5.1/src/buildenv/__init__.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/__main__.py` & `buildenv-1.5.1/src/buildenv/__main__.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/_internal/parser.py` & `buildenv-1.5.1/src/buildenv/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/_internal/render.py` & `buildenv-1.5.1/src/buildenv/_internal/render.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/extension.py` & `buildenv-1.5.1/src/buildenv/extension.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/loader.py` & `buildenv-1.5.1/src/buildenv/loader.py`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/manager.py` & `buildenv-1.5.1/src/buildenv/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,17 @@
 
         :param options: Input command line parsed options
         """
 
         # Checks
         self._command_checks("shell", options)
 
+        # Refuse to do anything in CI
+        assert not self.loader.is_ci, "Can't use shell command in CI environment."
+
         # Nothing more to do than telling loading script to spawn an interactive shell
         raise RCHolder(RC_START_SHELL)
 
     def run(self, options: Namespace):
         """
         Verify that the context is OK to run a command, then:
```

### Comparing `buildenv-1.5.0/src/buildenv/templates/buildenv.cmd.jinja` & `buildenv-1.5.1/src/buildenv/templates/buildenv.cmd.jinja`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv/templates/buildenv.sh.jinja` & `buildenv-1.5.1/src/buildenv/templates/buildenv.sh.jinja`

 * *Files identical despite different names*

### Comparing `buildenv-1.5.0/src/buildenv.egg-info/PKG-INFO` & `buildenv-1.5.1/src/buildenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildenv
-Version: 1.5.0
+Version: 1.5.1
 Summary: Build environment setup system, based on Python venv
 Home-page: https://github.com/dynod/buildenv
 Author: The dynod project
 Maintainer: The dynod project
 License: Mozilla Public License Version 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `buildenv-1.5.0/src/buildenv.egg-info/SOURCES.txt` & `buildenv-1.5.1/src/buildenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

