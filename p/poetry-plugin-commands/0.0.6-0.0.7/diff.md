# Comparing `tmp/poetry_plugin_commands-0.0.6.tar.gz` & `tmp/poetry_plugin_commands-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_commands-0.0.6.tar", max compression
+gzip compressed data, was "poetry_plugin_commands-0.0.7.tar", max compression
```

## Comparing `poetry_plugin_commands-0.0.6.tar` & `poetry_plugin_commands-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.6/LICENSE
--rw-r--r--   0        0        0     1928 2024-04-08 01:11:27.879544 poetry_plugin_commands-0.0.6/README.md
--rw-r--r--   0        0        0     3210 2024-04-08 01:21:41.313509 poetry_plugin_commands-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-08 00:27:30.593692 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/command.py
--rw-r--r--   0        0        0     1644 2024-04-08 00:44:09.905636 poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/plugins.py
--rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:26:56.337907 poetry_plugin_commands-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1926 2024-04-09 00:19:07.509029 poetry_plugin_commands-0.0.7/README.md
+-rw-r--r--   0        0        0     3199 2024-04-09 00:23:27.609015 poetry_plugin_commands-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      170 2024-04-07 16:47:18.853243 poetry_plugin_commands-0.0.7/src/poetry_plugin_commands/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-08 12:02:04.146390 poetry_plugin_commands-0.0.7/src/poetry_plugin_commands/command.py
+-rw-r--r--   0        0        0     1637 2024-04-09 00:20:46.991024 poetry_plugin_commands-0.0.7/src/poetry_plugin_commands/plugins.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 poetry_plugin_commands-0.0.7/PKG-INFO
```

### Comparing `poetry_plugin_commands-0.0.6/LICENSE` & `poetry_plugin_commands-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_commands-0.0.6/README.md` & `poetry_plugin_commands-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
    ```bash
    poetry self add poetry-plugin-commands
    ```
 
 2. **Define Aliases**:
 
-   Add your aliases to the `pyproject.toml` file under the `[tool.poetry.plugins.commands]` section:
+   Add your aliases to the `pyproject.toml` file under the `[tool.poetry-plugin-commands]` section:
 
    ```toml
-   [tool.poetry.plugins.commands]
+   [tool.poetry-plugin-commands]
    stree = "tree src"
    test_var = "echo $VAR"
    run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
    ```
 
    Here, `stree`, `test_var`, and `run_app` are the custom aliases, and their corresponding commands are specified.
```

### Comparing `poetry_plugin_commands-0.0.6/pyproject.toml` & `poetry_plugin_commands-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-commands"
-version = "0.0.6"
+version = "0.0.7"
 description = "Poetry plugin for simple custom user commands execution."
 readme = "README.md"
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
@@ -32,20 +32,20 @@
 
 [tool.poetry.urls]
 Homepage = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"
 Documentation = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"  # TODO: ...
 Repository = "https://github.com/BlackCatDevel0per/poetry-plugin-commands"
 
 ## Simple example
-# [tool.poetry.plugins.commands]
-# stree = "tree src"
-# test_var = "echo $VAR"
+[tool.poetry-plugin-commands]
+stree = "tree src"
+test_var = "echo $VAR"
 # Test this plugin without installing
-# run_env_stree = ".venv/bin/poetry stree"
-# run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
+run_env_stree = ".venv/bin/poetry stree"
+run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
 
 [tool.ruff]
 line-length = 100
 select = [
 	"RUF",
 	"FBT",
 	"FURB",
```

### Comparing `poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/command.py` & `poetry_plugin_commands-0.0.7/src/poetry_plugin_commands/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from os import system
+from shlex import split as command_split
+from subprocess import Popen
 from typing import TYPE_CHECKING
 
 from poetry.console.commands.group_command import GroupCommand
 from poetry.core.packages.dependency_group import MAIN_GROUP
 
 if TYPE_CHECKING:
 	...
@@ -47,8 +48,11 @@
 	@property
 	def default_groups(self: UserCommand) -> set[str]:
 		return {MAIN_GROUP}
 
 
 	def handle(self: UserCommand) -> int:
 		# TODO: Optionally show execution command..
-		return system(self.command)  # noqa: S605
+		print(command_split(self.command))
+		import os
+		os.environ['VAR'] = '1'
+		return Popen(command_split(self.command)).returncode  # noqa: S602
```

### Comparing `poetry_plugin_commands-0.0.6/src/poetry_plugin_commands/plugins.py` & `poetry_plugin_commands-0.0.7/src/poetry_plugin_commands/plugins.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 	from poetry.console.commands.command import Command
 	from poetry.poetry import Poetry
 
 
 class UserCommandsApplicationPlugin(ApplicationPlugin):
 	"""Main class of the plugin."""
 
-	plugin_section: Final[str] = 'commands'
+	plugin_section: Final[str] = 'poetry-plugin-commands'
 
 	@property
 	def commands(self: UserCommandsApplicationPlugin) -> list[type[Command]]:
 		"""Property with plugin own commands and user's commands.
 
 		User's commands are auto-generated from toml plugin's section shell commands.
 		"""
 		toml_content: dict[str, Any] = self.poetry.pyproject.data
 
 		# TODO: Exec field or catch options of poetry's run command (mb better make something like crun?)
 		# TODO: Make profiles for ux..
-		user_commands = toml_content['tool']['poetry']['plugins'][self.plugin_section]
+		user_commands = toml_content['tool'][self.plugin_section]
 
 		# TODO: Support python commands using toml's optioned values..
 		commands = [
 			UserCommand._new_cls(alias, command)  # noqa: SLF001
 			for alias, command in user_commands.items()
 		]
```

### Comparing `poetry_plugin_commands-0.0.6/PKG-INFO` & `poetry_plugin_commands-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-commands
-Version: 0.0.6
+Version: 0.0.7
 Summary: Poetry plugin for simple custom user commands execution.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -56,18 +56,18 @@
 
    ```bash
    poetry self add poetry-plugin-commands
    ```
 
 2. **Define Aliases**:
 
-   Add your aliases to the `pyproject.toml` file under the `[tool.poetry.plugins.commands]` section:
+   Add your aliases to the `pyproject.toml` file under the `[tool.poetry-plugin-commands]` section:
 
    ```toml
-   [tool.poetry.plugins.commands]
+   [tool.poetry-plugin-commands]
    stree = "tree src"
    test_var = "echo $VAR"
    run_app = "PYTHONPATH=src:. poetry run python src/app_launch/main.py"
    ```
 
    Here, `stree`, `test_var`, and `run_app` are the custom aliases, and their corresponding commands are specified.
```

