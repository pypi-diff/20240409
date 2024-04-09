# Comparing `tmp/dev_shell-0.7.0.tar.gz` & `tmp/dev_shell-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev_shell-0.7.0.tar", max compression
+gzip compressed data, was "dev_shell-0.8.0.tar", max compression
```

## Comparing `dev_shell-0.7.0.tar` & `dev_shell-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-03-16 07:34:18.881453 dev_shell-0.7.0/LICENSE
--rw-r--r--   0        0        0     6154 2023-04-25 15:15:45.398151 dev_shell-0.7.0/README.md
--rw-r--r--   0        0        0       22 2023-04-25 15:20:04.837368 dev_shell-0.7.0/dev_shell/__init__.py
--rw-r--r--   0        0        0     2478 2023-03-16 07:34:18.881453 dev_shell-0.7.0/dev_shell/base_cmd2_app.py
--rw-r--r--   0        0        0     4464 2023-03-16 07:34:18.881453 dev_shell-0.7.0/dev_shell/bootstrap-source.py
--rw-r--r--   0        0        0      222 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/command_sets/__init__.py
--rw-r--r--   0        0        0     4511 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/command_sets/dev_shell_commands.py
--rw-r--r--   0        0        0      934 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/config.py
--rw-r--r--   0        0        0      463 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/constants.py
--rw-r--r--   0        0        0      976 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/dev_shell_app.py
--rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/__init__.py
--rw-r--r--   0        0        0      513 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/constants.py
--rw-r--r--   0        0        0     1584 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/fixtures.py
--rw-r--r--   0        0        0     4162 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_bootstrap.py
--rw-r--r--   0        0        0     4182 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_dev_shell_app.py
--rw-r--r--   0        0        0     1390 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_source_file.py
--rw-r--r--   0        0        0     6838 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/tests/test_subprocess_utils.py
--rw-r--r--   0        0        0     1884 2023-04-25 15:15:45.406151 dev_shell-0.7.0/dev_shell/tests/utils.py
--rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/__init__.py
--rw-r--r--   0        0        0      534 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/assertion.py
--rw-r--r--   0        0        0     1669 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/colorful.py
--rw-r--r--   0        0        0     5306 2023-03-16 07:34:18.885454 dev_shell-0.7.0/dev_shell/utils/subprocess_utils.py
--rw-r--r--   0        0        0     2359 2023-04-25 15:20:58.233206 dev_shell-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6788 1970-01-01 00:00:00.000000 dev_shell-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-16 07:34:18.881453 dev_shell-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6323 2024-04-09 09:09:07.187201 dev_shell-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-09 09:25:36.437564 dev_shell-0.8.0/dev_shell/__init__.py
+-rw-r--r--   0        0        0     2478 2023-03-16 07:34:18.881453 dev_shell-0.8.0/dev_shell/base_cmd2_app.py
+-rw-r--r--   0        0        0     4639 2024-04-09 09:08:36.463232 dev_shell-0.8.0/dev_shell/bootstrap-source.py
+-rw-r--r--   0        0        0      222 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/command_sets/__init__.py
+-rw-r--r--   0        0        0     4511 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/command_sets/dev_shell_commands.py
+-rw-r--r--   0        0        0      934 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/config.py
+-rw-r--r--   0        0        0      463 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/constants.py
+-rw-r--r--   0        0        0      976 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/dev_shell_app.py
+-rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/__init__.py
+-rw-r--r--   0        0        0      513 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/constants.py
+-rw-r--r--   0        0        0     1584 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/fixtures.py
+-rw-r--r--   0        0        0     4276 2024-04-09 09:08:47.771219 dev_shell-0.8.0/dev_shell/tests/test_bootstrap.py
+-rw-r--r--   0        0        0     4182 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/test_dev_shell_app.py
+-rw-r--r--   0        0        0     1390 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/test_source_file.py
+-rw-r--r--   0        0        0     6838 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/tests/test_subprocess_utils.py
+-rw-r--r--   0        0        0     1906 2024-04-09 09:05:47.259544 dev_shell-0.8.0/dev_shell/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/utils/__init__.py
+-rw-r--r--   0        0        0      534 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/utils/assertion.py
+-rw-r--r--   0        0        0     1669 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/utils/colorful.py
+-rw-r--r--   0        0        0     5306 2023-03-16 07:34:18.885454 dev_shell-0.8.0/dev_shell/utils/subprocess_utils.py
+-rw-r--r--   0        0        0     2242 2024-04-09 09:26:59.097374 dev_shell-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 dev_shell-0.8.0/PKG-INFO
```

### Comparing `dev_shell-0.7.0/LICENSE` & `dev_shell-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/README.md` & `dev_shell-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -100,16 +100,20 @@
 | >=v0.5.0          | Linux + MacOS + Windows | 3.10, 3.9, 3.8, 3.7 |
 | >=v0.0.1          | Linux + MacOS + Windows | 3.9, 3.8, 3.7       |
 
 See also github test configuration: [.github/workflows/test.yml](https://github.com/jedie/dev-shell/blob/main/.github/workflows/test.yml)
 
 ## History
 
-* [*dev*](https://github.com/jedie/dev-shell/compare/v0.7.0...main)
+* [*dev*](https://github.com/jedie/dev-shell/compare/v0.8.0...main)
   * TBC
+* [0.8.0 - 2024-04-09](https://github.com/jedie/dev-shell/compare/v0.7.0...v0.8.0)
+  * Remove "gnureadline" as dependency
+  * update boot script
+  * update requirements
 * [0.7.0 - 2023-04-25](https://github.com/jedie/dev-shell/compare/v0.6.1...v0.7.0)
   * Update test matrix
   * update requirements
 * [0.6.1 - 2022-09-02](https://github.com/jedie/dev-shell/compare/v0.6.0...v0.6.1)
   * Set default subprocess timeout to 5 Min.
   * Skip buggy Poetry v1.2.0
   * Update requirements
```

### Comparing `dev_shell-0.7.0/dev_shell/base_cmd2_app.py` & `dev_shell-0.8.0/dev_shell/base_cmd2_app.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/bootstrap-source.py` & `dev_shell-0.8.0/dev_shell/bootstrap-source.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,38 +5,46 @@
     ~~~~~~~~~~~~~~~
 
     Just call this file, and the magic happens ;)
 
     This file is from: https://pypi.org/project/dev-shell/
     Source: https://github.com/jedie/dev-shell/blob/main/devshell.py
 
-    :copyleft: 2021-2022 by Jens Diemer
+    :copyleft: 2021-2024 by Jens Diemer
     :license: GNU GPL v3 or above
 """
-
 import argparse
 import hashlib
+import shlex
 import signal
 import subprocess
 import sys
 import venv
 from pathlib import Path
 
 
+def print_no_pip_error():
+    print('Error: Pip not available!')
+    print('Hint: "apt-get install python3-venv"\n')
+
+
 try:
-    import ensurepip  # noqa
+    from ensurepip import version
 except ModuleNotFoundError as err:
     print(err)
     print('-' * 100)
-    print('Error: Pip not available!')
-    print('Hint: "apt-get install python3-venv"\n')
+    print_no_pip_error()
     raise
+else:
+    if not version():
+        print_no_pip_error()
+        sys.exit(-1)
 
 
-assert sys.version_info >= (3, 7), 'Python version is too old!'
+assert sys.version_info >= (3, 9), f'Python version {sys.version_info} is too old!'
 
 
 if sys.platform == 'win32':  # wtf
     # Files under Windows, e.g.: .../.venv/Scripts/python.exe
     BIN_NAME = 'Scripts'
     FILE_EXT = '.exe'
 else:
@@ -56,41 +64,39 @@
 
 # script file defined in pyproject.toml as [tool.poetry.scripts]
 # (Under Windows: ".exe" not added!)
 PROJECT_SHELL_SCRIPT = BIN_PATH / 'devshell'
 
 
 def get_dep_hash():
-    """ Get SHA512 hash from poetry.lock content. """
+    """Get SHA512 hash from lock file content."""
     return hashlib.sha512(DEP_LOCK_PATH.read_bytes()).hexdigest()
 
 
 def store_dep_hash():
-    """ Generate /.venv/.dep_hash """
+    """Generate .venv/.dep_hash"""
     DEP_HASH_PATH.write_text(get_dep_hash())
 
 
 def venv_up2date():
-    """ Is existing .venv is up-to-date? """
+    """Is existing .venv is up-to-date?"""
     if DEP_HASH_PATH.is_file():
         return DEP_HASH_PATH.read_text() == get_dep_hash()
     return False
 
 
 def verbose_check_call(*popen_args):
-    popen_args = [str(arg) for arg in popen_args]  # e.g.: Path() -> str for python 3.7
-    print(f'\n+ {" ".join(popen_args)}\n')
+    print(f'\n+ {shlex.join(str(arg) for arg in popen_args)}\n')
     return subprocess.check_call(popen_args)
 
 
 def noop_signal_handler(signal_num, frame):
     """
     Signal handler that does nothing: Used to ignore "Ctrl-C" signals
     """
-    pass
 
 
 def main(argv):
     assert DEP_LOCK_PATH.is_file(), f'File not found: "{DEP_LOCK_PATH}" !'
 
     if len(argv) == 2 and argv[1] in ('--update', '--help'):
         parser = argparse.ArgumentParser(
@@ -115,20 +121,22 @@
         extra_args = argv[1:]
 
     # Create virtual env in ".../.venv/":
     if not PYTHON_PATH.is_file() or force_update:
         print('Create virtual env here:', VENV_PATH.absolute())
         builder = venv.EnvBuilder(symlinks=True, upgrade=True, with_pip=True)
         builder.create(env_dir=VENV_PATH)
+        # Update pip
+        verbose_check_call(PYTHON_PATH, '-m', 'pip', 'install', '-U', 'pip')
 
     # install/update "pip" and "poetry":
     if not POETRY_PATH.is_file() or force_update:
         # Note: Under Windows pip.exe can't replace this own .exe file, so use the module way:
         verbose_check_call(PYTHON_PATH, '-m', 'pip', 'install', '-U', 'pip', 'setuptools')
-        verbose_check_call(PIP_PATH, 'install', 'poetry!=1.2.0')
+        verbose_check_call(PIP_PATH, 'install', 'poetry')
 
     # install via poetry, if:
     #   1. .venv not exists
     #   2. "--update" used
     #   3. poetry.lock file was changed
     if not PROJECT_SHELL_SCRIPT.is_file() or force_update or not venv_up2date():
         verbose_check_call(POETRY_PATH, 'install')
```

### Comparing `dev_shell-0.7.0/dev_shell/command_sets/dev_shell_commands.py` & `dev_shell-0.8.0/dev_shell/command_sets/dev_shell_commands.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/config.py` & `dev_shell-0.8.0/dev_shell/config.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/dev_shell_app.py` & `dev_shell-0.8.0/dev_shell/dev_shell_app.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/constants.py` & `dev_shell-0.8.0/dev_shell/tests/constants.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/fixtures.py` & `dev_shell-0.8.0/dev_shell/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/test_bootstrap.py` & `dev_shell-0.8.0/dev_shell/tests/test_bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,20 +84,24 @@
         # So we mock this call here.
         with mock.patch('venv.EnvBuilder.create') as create_mock:
             check_calls, stdout, stderr = call_devsetup_main('devshell.py', '--update')
 
         assert stderr == ''
         assert f'{VENV_POETRY} install' in stdout
         assert f'{DEVSHELL_CALL}\n' in stdout
-        assert check_calls == [
-            f'{VENV_PYTHON} -m pip install -U pip setuptools',
-            f'{VENV_PIP} install poetry!=1.2.0',
-            f'{VENV_POETRY} install',
-            DEVSHELL_CALL
-        ]
+        self.assertEqual(
+            check_calls,
+            [
+                f'{VENV_PYTHON} -m pip install -U pip',
+                f'{VENV_PYTHON} -m pip install -U pip setuptools',
+                f'{VENV_PIP} install poetry',
+                f'{VENV_POETRY} install',
+                DEVSHELL_CALL,
+            ],
+        )
         create_mock.assert_called_once_with(env_dir=VENV_PATH)
 
     def test_help(self):
         check_calls, stdout, stderr = call_devsetup_main(
             'devshell.py', '--help',
             catch_sys_exit=True
         )
```

### Comparing `dev_shell-0.7.0/dev_shell/tests/test_dev_shell_app.py` & `dev_shell-0.8.0/dev_shell/tests/test_dev_shell_app.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/test_source_file.py` & `dev_shell-0.8.0/dev_shell/tests/test_source_file.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/test_subprocess_utils.py` & `dev_shell-0.8.0/dev_shell/tests/test_subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/tests/utils.py` & `dev_shell-0.8.0/dev_shell/tests/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             # TODO: Use "call.kwargs" and "call.args" if we drop Python 3.7 support!
             args, kwargs = args_list
 
             popenargs = args[0]
             if isinstance(popenargs, str):
                 command_str = popenargs
             else:
-                command_str = ' '.join(popenargs)
+                command_str = ' '.join([str(arg) for arg in popenargs])
 
             cwd = kwargs.get('cwd')
             if cwd:
                 command_str = f'{cwd}$ {command_str}'
 
             check_calls.append(command_str)
```

### Comparing `dev_shell-0.7.0/dev_shell/utils/assertion.py` & `dev_shell-0.8.0/dev_shell/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/utils/colorful.py` & `dev_shell-0.8.0/dev_shell/utils/colorful.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/dev_shell/utils/subprocess_utils.py` & `dev_shell-0.8.0/dev_shell/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dev_shell-0.7.0/pyproject.toml` & `dev_shell-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [tool.poetry]
 name = "dev-shell"
-version = "0.7.0"
-description = "Devloper shell for easy startup..."
+version = "0.8.0"
+description = "Developer shell for easy startup..."
 readme = "README.md"
 authors = ["Jens Diemer <python@jensdiemer.de>"]
 homepage = "https://github.com/jedie/dev-shell"
 license = "GNU General Public License v3.0"
 packages = [
     { include = "dev_shell" },
 ]
 
 [tool.poetry.scripts]
 devshell = 'dev_shell.dev_shell_app:devshell_cmdloop'
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0.0"
+python = ">=3.9,<4.0"
 cmd2 = "*"  # https://github.com/python-cmd2/cmd2
 
-# fix completion for Mac OS:
-gnureadline = { version = "*", markers = "sys_platform == 'darwin'" }
-
-
 [tool.poetry.dev-dependencies]
 cmd2_ext_test = "*"
 poetry-publish = "*"  # https://github.com/jedie/poetry-publish
 pytest = "*"
 pytest-randomly = "*"
 pytest-cov = "*"
 darker = "*"  # https://github.com/akaihola/darker
@@ -38,15 +34,14 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.darker]
 src = ['.',]
 revision = "origin/main..."
 line_length = 100
-verbose = true
 skip_string_normalization = true
 diff = false
 check = false
 stdout = false
 isort = true
 lint = [
     "flake8",
```

### Comparing `dev_shell-0.7.0/PKG-INFO` & `dev_shell-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: dev-shell
-Version: 0.7.0
-Summary: Devloper shell for easy startup...
+Version: 0.8.0
+Summary: Developer shell for easy startup...
 Home-page: https://github.com/jedie/dev-shell
 License: GNU General Public License v3.0
 Author: Jens Diemer
 Author-email: python@jensdiemer.de
-Requires-Python: >=3.9,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cmd2
-Requires-Dist: gnureadline ; sys_platform == "darwin"
 Description-Content-Type: text/markdown
 
 # A "dev-shell" for Python projects ;)
 
 [![Test](https://github.com/jedie/dev-shell/actions/workflows/test.yml/badge.svg?branch=bugfix-path)](https://github.com/jedie/dev-shell/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/jedie/dev-shell/branch/main/graph/badge.svg)](https://codecov.io/gh/jedie/dev-shell)
 
@@ -118,16 +117,20 @@
 | >=v0.5.0          | Linux + MacOS + Windows | 3.10, 3.9, 3.8, 3.7 |
 | >=v0.0.1          | Linux + MacOS + Windows | 3.9, 3.8, 3.7       |
 
 See also github test configuration: [.github/workflows/test.yml](https://github.com/jedie/dev-shell/blob/main/.github/workflows/test.yml)
 
 ## History
 
-* [*dev*](https://github.com/jedie/dev-shell/compare/v0.7.0...main)
+* [*dev*](https://github.com/jedie/dev-shell/compare/v0.8.0...main)
   * TBC
+* [0.8.0 - 2024-04-09](https://github.com/jedie/dev-shell/compare/v0.7.0...v0.8.0)
+  * Remove "gnureadline" as dependency
+  * update boot script
+  * update requirements
 * [0.7.0 - 2023-04-25](https://github.com/jedie/dev-shell/compare/v0.6.1...v0.7.0)
   * Update test matrix
   * update requirements
 * [0.6.1 - 2022-09-02](https://github.com/jedie/dev-shell/compare/v0.6.0...v0.6.1)
   * Set default subprocess timeout to 5 Min.
   * Skip buggy Poetry v1.2.0
   * Update requirements
```

